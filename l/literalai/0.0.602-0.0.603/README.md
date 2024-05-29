# Comparing `tmp/literalai-0.0.602.tar.gz` & `tmp/literalai-0.0.603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literalai-0.0.602.tar", last modified: Fri May 24 10:01:09 2024, max compression
+gzip compressed data, was "literalai-0.0.603.tar", last modified: Tue May 28 14:06:26 2024, max compression
```

## Comparing `literalai-0.0.602.tar` & `literalai-0.0.603.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-24 10:01:01.000000 literalai-0.0.602/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 10:01:09.036695 literalai-0.0.602/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-24 10:01:01.000000 literalai-0.0.602/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/api/
--rw-r--r--   0 runner    (1001) docker     (127)    84883 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/attachment_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/dataset_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/generation_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20968 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/prompt_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/score_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/step_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/thread_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/api/user_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai/callback/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/langchain_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/callback/llama_index_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/event_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/literalai/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/instrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/instrumentation/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/thread.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-24 10:01:01.000000 literalai-0.0.602/literalai/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.032695 literalai-0.0.602/literalai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-24 10:01:09.000000 literalai-0.0.602/literalai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-24 10:01:08.000000 literalai-0.0.602/literalai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 10:01:09.036695 literalai-0.0.602/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-24 10:01:01.000000 literalai-0.0.602/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:09.036695 literalai-0.0.602/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 10:01:01.000000 literalai-0.0.602/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.093573 literalai-0.0.603/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 14:06:13.000000 literalai-0.0.603/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 14:06:26.093573 literalai-0.0.603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 14:06:13.000000 literalai-0.0.603/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.089573 literalai-0.0.603/literalai/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.093573 literalai-0.0.603/literalai/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    86057 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/attachment_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/dataset_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/generation_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21202 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/prompt_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/score_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/step_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/thread_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/api/user_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.093573 literalai-0.0.603/literalai/callback/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/callback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17193 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/callback/langchain_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8446 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/callback/llama_index_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/dataset_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/event_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.093573 literalai-0.0.603/literalai/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/instrumentation/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8852 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10028 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2024-05-28 14:06:13.000000 literalai-0.0.603/literalai/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.089573 literalai-0.0.603/literalai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 14:06:25.000000 literalai-0.0.603/literalai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-28 14:06:26.000000 literalai-0.0.603/literalai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:06:25.000000 literalai-0.0.603/literalai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 14:06:25.000000 literalai-0.0.603/literalai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 14:06:25.000000 literalai-0.0.603/literalai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:06:26.093573 literalai-0.0.603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-28 14:06:13.000000 literalai-0.0.603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:26.093573 literalai-0.0.603/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:06:13.000000 literalai-0.0.603/tests/__init__.py
```

### Comparing `literalai-0.0.602/LICENSE` & `literalai-0.0.603/LICENSE`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/README.md` & `literalai-0.0.603/README.md`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/__init__.py` & `literalai-0.0.603/literalai/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     update_dataset_helper,
 )
 from .generation_helpers import create_generation_helper, get_generations_helper
 from .prompt_helpers import (
     create_prompt_helper,
     create_prompt_lineage_helper,
     get_prompt_helper,
+    promote_prompt_helper,
 )
 from .score_helpers import (
     ScoreUpdate,
     check_scores_finite,
     create_score_helper,
     create_scores_query_builder,
     delete_score_helper,
@@ -1212,27 +1213,32 @@
         """
         return self.gql_helper(
             *add_generation_to_dataset_helper(dataset_id, generation_id, metadata)
         )
 
     # Prompt API
 
-    def create_prompt_lineage(self, name: str, description: Optional[str] = None):
+    def get_or_create_prompt_lineage(self, name: str, description: Optional[str] = None):
         """
         Creates a prompt lineage with the specified name and optional description.
+        If the prompt lineage with that name already exists, it is returned.
 
         Args:
             name (str): The name of the prompt lineage.
             description (Optional[str]): An optional description of the prompt lineage.
 
         Returns:
             Dict: The result of the prompt lineage creation operation.
         """
         return self.gql_helper(*create_prompt_lineage_helper(name, description))
 
+    @deprecated('Please use "get_or_create_prompt_lineage" instead.')
+    def create_prompt_lineage(self, name: str, description: Optional[str] = None):
+        return self.get_or_create_prompt_lineage(name, description)
+
     def get_or_create_prompt(
         self,
         name: str,
         template_messages: List[GenerationMessage],
         settings: Optional[ProviderSettings] = None,
         tools: Optional[List[Dict]] = None,
     ) -> Prompt:
@@ -1245,15 +1251,15 @@
             name (str): The name of the prompt to retrieve or create.
             template_messages (List[GenerationMessage]): A list of template messages for the prompt.
             settings (Optional[Dict]): Optional settings for the prompt.
 
         Returns:
             Prompt: The prompt that was retrieved or created.
         """
-        lineage = self.create_prompt_lineage(name)
+        lineage = self.get_or_create_prompt_lineage(name)
         lineage_id = lineage["id"]
         return self.gql_helper(
             *create_prompt_helper(self, lineage_id, template_messages, settings, tools)
         )
 
     @deprecated('Please use "get_or_create_prompt" instead.')
     def create_prompt(
@@ -1264,15 +1270,15 @@
     ) -> Prompt:
         return self.get_or_create_prompt(name, template_messages, settings)
 
     def get_prompt(
         self,
         id: Optional[str] = None,
         name: Optional[str] = None,
-        version: Optional[int] = 0,
+        version: Optional[int] = None,
     ) -> Prompt:
         """
         Gets a prompt either by:
         - `id`
         - or `name` and (optional) `version`
 
         Either the `id` or the `name` must be provided.
@@ -1288,14 +1294,31 @@
         """
         if id:
             return self.gql_helper(*get_prompt_helper(self, id=id))
         elif name:
             return self.gql_helper(*get_prompt_helper(self, name=name, version=version))
         else:
             raise ValueError("Either the `id` or the `name` must be provided.")
+    
+    def promote_prompt(self, name: str, version: int) -> str:
+        """
+        Promotes the prompt with name to target version.
+
+        Args:
+            name (str): The name of the prompt lineage.
+            version (int): The version number to promote.
+
+        Returns:
+            str: The champion prompt ID.
+        """
+        lineage = self.get_or_create_prompt_lineage(name)
+        lineage_id = lineage["id"]
+
+        return self.gql_helper(*promote_prompt_helper(lineage_id, version))
+
 
     # Misc API
 
     def get_my_project_id(self):
         """
         Retrieves the projectId associated to the API key.
 
@@ -2379,35 +2402,31 @@
         """
         return await self.gql_helper(
             *add_generation_to_dataset_helper(dataset_id, generation_id, metadata)
         )
 
     # Prompt API
 
-    async def create_prompt_lineage(self, name: str, description: Optional[str] = None):
-        """
-        Asynchronously creates a prompt lineage.
+    async def get_or_create_prompt_lineage(self, name: str, description: Optional[str] = None):
+        return await self.gql_helper(*create_prompt_lineage_helper(name, description))
 
-        Args:
-            name (str): The name of the prompt lineage.
-            description (Optional[str]): An optional description of the prompt lineage.
+    get_or_create_prompt_lineage.__doc__ = LiteralAPI.get_or_create_prompt_lineage.__doc__
 
-        Returns:
-            The result of the GraphQL helper function for creating a prompt lineage.
-        """
-        return await self.gql_helper(*create_prompt_lineage_helper(name, description))
+    @deprecated('Please use "get_or_create_prompt_lineage" instead.')
+    async def create_prompt_lineage(self, name: str, description: Optional[str] = None):
+        return await self.get_or_create_prompt_lineage(name, description)
 
     async def get_or_create_prompt(
         self,
         name: str,
         template_messages: List[GenerationMessage],
         settings: Optional[ProviderSettings] = None,
         tools: Optional[List[Dict]] = None,
     ) -> Prompt:
-        lineage = await self.create_prompt_lineage(name)
+        lineage = await self.get_or_create_prompt_lineage(name)
         lineage_id = lineage["id"]
 
         sync_api = LiteralAPI(self.api_key, self.url)
         return await self.gql_helper(
             *create_prompt_helper(
                 sync_api, lineage_id, template_messages, settings, tools
             )
@@ -2424,28 +2443,37 @@
     ):
         return await self.get_or_create_prompt(name, template_messages, settings)
 
     async def get_prompt(
         self,
         id: Optional[str] = None,
         name: Optional[str] = None,
-        version: Optional[int] = 0,
+        version: Optional[int] = None,
     ) -> Prompt:
         sync_api = LiteralAPI(self.api_key, self.url)
         if id:
             return await self.gql_helper(*get_prompt_helper(sync_api, id=id))
         elif name:
             return await self.gql_helper(
                 *get_prompt_helper(sync_api, name=name, version=version)
             )
         else:
             raise ValueError("Either the `id` or the `name` must be provided.")
 
     get_prompt.__doc__ = LiteralAPI.get_prompt.__doc__
 
+    async def promote_prompt(self, name: str, version: int) -> str:
+        lineage = await self.get_or_create_prompt_lineage(name)
+        lineage_id = lineage["id"]
+
+        return await self.gql_helper(*promote_prompt_helper(lineage_id, version))
+
+    promote_prompt.__doc__ = LiteralAPI.promote_prompt.__doc__
+
     # Misc API
 
     async def get_my_project_id(self):
         response = await self.make_rest_call("/my-project", {})
         return response["projectId"]
 
     get_my_project_id.__doc__ = LiteralAPI.get_my_project_id.__doc__
+
```

### Comparing `literalai-0.0.602/literalai/api/attachment_helpers.py` & `literalai-0.0.603/literalai/api/attachment_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/dataset_helpers.py` & `literalai-0.0.603/literalai/api/dataset_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/generation_helpers.py` & `literalai-0.0.603/literalai/api/generation_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/gql.py` & `literalai-0.0.603/literalai/api/gql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1031,14 +1031,27 @@
         lineage {
             name
         }
     }
 }
 """
 
+PROMOTE_PROMPT_VERSION = """mutation promotePromptVersion(
+    $lineageId: String!
+    $version: Int!
+  ) {
+    promotePromptVersion(
+      lineageId: $lineageId
+      version: $version
+    ) {
+      id
+      championId
+    }
+  }"""
+
 
 def serialize_step(event, id):
     result = {}
 
     for key, value in event.items():
         # Only keep the keys that are not None to avoid overriding existing values
         if value is not None:
```

### Comparing `literalai-0.0.602/literalai/api/prompt_helpers.py` & `literalai-0.0.603/literalai/api/prompt_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,7 +55,22 @@
     def process_response(response):
         prompt = response["data"]["promptVersion"]
         return Prompt.from_dict(api, prompt) if prompt else None
 
     description = "get prompt"
 
     return gql.GET_PROMPT_VERSION, description, variables, process_response
+
+
+def promote_prompt_helper(
+        lineage_id: str,
+        version: int,
+):
+    variables = {"lineageId": lineage_id, "version": version}
+
+    def process_response(response) -> str:
+        prompt = response["data"]["promotePromptVersion"]
+        return prompt["championId"] if prompt else None
+
+    description = "promote prompt version"
+
+    return gql.PROMOTE_PROMPT_VERSION, description, variables, process_response
```

### Comparing `literalai-0.0.602/literalai/api/score_helpers.py` & `literalai-0.0.603/literalai/api/score_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/step_helpers.py` & `literalai-0.0.603/literalai/api/step_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/thread_helpers.py` & `literalai-0.0.603/literalai/api/thread_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/api/user_helpers.py` & `literalai-0.0.603/literalai/api/user_helpers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/callback/langchain_callback.py` & `literalai-0.0.603/literalai/callback/langchain_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/callback/llama_index_callback.py` & `literalai-0.0.603/literalai/callback/llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/client.py` & `literalai-0.0.603/literalai/client.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/dataset.py` & `literalai-0.0.603/literalai/dataset.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/dataset_experiment.py` & `literalai-0.0.603/literalai/dataset_experiment.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/dataset_item.py` & `literalai-0.0.603/literalai/dataset_item.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/event_processor.py` & `literalai-0.0.603/literalai/event_processor.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/filter.py` & `literalai-0.0.603/literalai/filter.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/helper.py` & `literalai-0.0.603/literalai/helper.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/instrumentation/openai.py` & `literalai-0.0.603/literalai/instrumentation/openai.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/message.py` & `literalai-0.0.603/literalai/message.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/my_types.py` & `literalai-0.0.603/literalai/my_types.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/prompt.py` & `literalai-0.0.603/literalai/prompt.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,21 @@
             tools=prompt_dict.get("tools", []),
             provider=provider,
             settings=settings,
             variables=prompt_dict.get("variables", []),
             variables_default_values=prompt_dict.get("variablesDefaultValues"),
         )
 
+    def promote(self) -> "Prompt":
+        """
+        Promotes this prompt to champion.
+        """
+        self.api.promote_prompt(self.name, self.version)
+        return self
+
     def format_messages(self, **kwargs: Any) -> List[Any]:
         """
         Formats the prompt's template messages with the given variables.
         Variables may be passed as a dictionary or as keyword arguments.
         Keyword arguments take precedence over variables passed as a dictionary.
 
         Args:
```

### Comparing `literalai-0.0.602/literalai/requirements.py` & `literalai-0.0.603/literalai/requirements.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/step.py` & `literalai-0.0.603/literalai/step.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/thread.py` & `literalai-0.0.603/literalai/thread.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai/wrappers.py` & `literalai-0.0.603/literalai/wrappers.py`

 * *Files identical despite different names*

### Comparing `literalai-0.0.602/literalai.egg-info/SOURCES.txt` & `literalai-0.0.603/literalai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

