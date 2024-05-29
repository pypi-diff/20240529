# Comparing `tmp/galileo_core-1.5.0.tar.gz` & `tmp/galileo_core-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-1.5.0.tar", max compression
+gzip compressed data, was "galileo_core-1.6.0.tar", max compression
```

## Comparing `galileo_core-1.5.0.tar` & `galileo_core-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    10946 2024-05-29 16:21:20.273648 galileo_core-1.5.0/LICENSE
--rw-r--r--   0        0        0       80 2024-05-29 16:21:20.273648 galileo_core-1.5.0/README.md
--rw-r--r--   0        0        0     2622 2024-05-29 16:21:21.657652 galileo_core-1.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-29 16:21:21.657652 galileo_core-1.5.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      242 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/constants/processing_headers.py
--rw-r--r--   0        0        0      190 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/constants/request_method.py
--rw-r--r--   0        0        0      424 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     2973 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     6398 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0      369 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/dependencies.py
--rw-r--r--   0        0        0     1291 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/execution.py
--rw-r--r--   0        0        0       60 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0     2146 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/helpers/project.py
--rw-r--r--   0        0        0       60 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/logger.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/py.typed
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/core/__init__.py
--rw-r--r--   0        0        0      738 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/core/project.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      246 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/execution_status.py
--rw-r--r--   0        0        0      890 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      795 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     3905 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0      521 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/response.py
--rw-r--r--   0        0        0     2886 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0      831 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0      758 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      176 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/shared/chains.py
--rw-r--r--   0        0        0      149 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/testing/__init__.py
--rw-r--r--   0        0        0     1144 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/testing/request_mocker.py
--rw-r--r--   0        0        0        0 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/utils/__init__.py
--rw-r--r--   0        0        0      204 2024-05-29 16:21:20.273648 galileo_core-1.5.0/src/galileo_core/utils/name.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 galileo_core-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-05-29 17:14:13.064181 galileo_core-1.6.0/LICENSE
+-rw-r--r--   0        0        0       80 2024-05-29 17:14:13.064181 galileo_core-1.6.0/README.md
+-rw-r--r--   0        0        0     2622 2024-05-29 17:14:14.696178 galileo_core-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-29 17:14:14.700178 galileo_core-1.6.0/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      242 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/constants/processing_headers.py
+-rw-r--r--   0        0        0      190 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/constants/request_method.py
+-rw-r--r--   0        0        0      424 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     2973 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     6398 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0      369 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/dependencies.py
+-rw-r--r--   0        0        0     1291 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/execution.py
+-rw-r--r--   0        0        0       60 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0     2146 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/helpers/project.py
+-rw-r--r--   0        0        0       60 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/logger.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/core/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/core/project.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      246 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/execution_status.py
+-rw-r--r--   0        0        0      890 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      795 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     3702 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0      521 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/response.py
+-rw-r--r--   0        0        0     2886 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0     1053 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1359 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/shared/chains.py
+-rw-r--r--   0        0        0      149 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/testing/__init__.py
+-rw-r--r--   0        0        0     1144 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/testing/request_mocker.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/utils/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-29 17:14:13.068181 galileo_core-1.6.0/src/galileo_core/utils/name.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 galileo_core-1.6.0/PKG-INFO
```

### Comparing `galileo_core-1.5.0/LICENSE` & `galileo_core-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/pyproject.toml` & `galileo_core-1.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-core"
-version = "1.5.0"
+version = "1.6.0"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_core-1.5.0/src/galileo_core/constants/http_headers.py` & `galileo_core-1.6.0/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/helpers/api_client.py` & `galileo_core-1.6.0/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/helpers/config.py` & `galileo_core-1.6.0/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/helpers/execution.py` & `galileo_core-1.6.0/src/galileo_core/helpers/execution.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/helpers/project.py` & `galileo_core-1.6.0/src/galileo_core/helpers/project.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/core/project.py` & `galileo_core-1.6.0/src/galileo_core/schemas/core/project.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/metric.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/metric.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/payload.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/payload.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/request.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 from datetime import timedelta
 from functools import cached_property
 from os import getenv
-from typing import Dict, List, Optional, Sequence, Set
+from typing import Dict, List, Optional, Set
 from uuid import UUID
 
 from pydantic import (
     UUID4,
-    BaseModel,
     ConfigDict,
     Field,
     computed_field,
     field_validator,
     model_validator,
 )
 
 from galileo_core.schemas.protect.payload import Payload
 from galileo_core.schemas.protect.rule import Rule
-from galileo_core.schemas.protect.ruleset import Ruleset
+from galileo_core.schemas.protect.ruleset import RulesetsMixin
 
 
-class Request(BaseModel):
+class Request(RulesetsMixin):
     payload: Payload = Field(description="Payload to be processed.")
     project_id: Optional[UUID4] = Field(default=None, description="Project ID.", validate_default=True)
     stage_name: Optional[str] = Field(default=None, description="Stage name.", validate_default=True)
     stage_id: Optional[UUID4] = Field(default=None, description="Stage ID.", validate_default=True)
-    rulesets: Sequence[Ruleset] = Field(
-        default_factory=list,
-        description="Rulesets to be applied to the payload.",
-        validation_alias="prioritized_rulesets",
-    )
     timeout: float = Field(
         default=timedelta(minutes=5).total_seconds(),
         description="Optional timeout for the guardrail execution in seconds. This is not the timeout for the request. If not set, a default timeout of 5 minutes will be used.",
     )
     metadata: Optional[Dict[str, str]] = Field(
         default=None,
         description="Optional additional metadata. This will be echoed back in the response.",
```

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/response.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/response.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/src/galileo_core/schemas/protect/stage.py` & `galileo_core-1.6.0/src/galileo_core/schemas/protect/ruleset.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-from enum import Enum
-from typing import Optional
+from typing import Optional, Sequence
 
-from pydantic import UUID4, BaseModel, Field
+from pydantic import BaseModel, Field, field_validator
 
+from galileo_core.schemas.protect.action import Action, BaseAction, PassthroughAction
+from galileo_core.schemas.protect.rule import Rule
 
-class StageType(str, Enum):
-    local = "local"
-    central = "central"
 
-
-class Stage(BaseModel):
-    name: str = Field(description="Name of the stage. Must be unique within the project.")
-    project_id: UUID4 = Field(description="ID of the project to which this stage belongs.")
-    description: Optional[str] = Field(
-        description="Optional human-readable description of the goals of this guardrail.", default=None
+class Ruleset(BaseModel):
+    rules: Sequence[Rule] = Field(
+        description="List of rules to evaluate. Atleast 1 rule is required.", default_factory=list, min_length=1
     )
-    type: StageType = Field(description="Type of the stage.", default=StageType.local)
-    paused: bool = Field(
-        description="Whether the action is enabled. If False, the action will not be applied.", default=False
+    action: Action = Field(description="Action to take if all the rules are met.", default_factory=PassthroughAction)
+    description: Optional[str] = Field(description="Description of the ruleset.", default=None)
+
+    @field_validator("action", mode="before")
+    def validate_action(cls, value: Optional[BaseAction]) -> BaseAction:
+        if not value:
+            value = PassthroughAction()
+        return value
+
+
+class RulesetsMixin(BaseModel):
+    rulesets: Sequence[Ruleset] = Field(
+        default_factory=list,
+        description="Rulesets to be applied to the payload.",
+        validation_alias="prioritized_rulesets",
     )
```

### Comparing `galileo_core-1.5.0/src/galileo_core/testing/request_mocker.py` & `galileo_core-1.6.0/src/galileo_core/testing/request_mocker.py`

 * *Files identical despite different names*

### Comparing `galileo_core-1.5.0/PKG-INFO` & `galileo_core-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 1.5.0
+Version: 1.6.0
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

