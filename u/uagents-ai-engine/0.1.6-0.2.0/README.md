# Comparing `tmp/uagents_ai_engine-0.1.6.tar.gz` & `tmp/uagents_ai_engine-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_ai_engine-0.1.6.tar", max compression
+gzip compressed data, was "uagents_ai_engine-0.2.0.tar", max compression
```

## Comparing `uagents_ai_engine-0.1.6.tar` & `uagents_ai_engine-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.1.6/README.md
--rw-r--r--   0        0        0      394 2024-04-11 12:32:46.289573 uagents_ai_engine-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.1.6/src/ai_engine/__init__.py
--rw-r--r--   0        0        0     4487 2024-04-04 04:31:33.596581 uagents_ai_engine-0.1.6/src/ai_engine/chitchat.py
--rw-r--r--   0        0        0     2302 2024-04-11 12:32:46.290062 uagents_ai_engine-0.1.6/src/ai_engine/dialogue.py
--rw-r--r--   0        0        0     2967 2024-04-04 08:59:10.091701 uagents_ai_engine-0.1.6/src/ai_engine/messages.py
--rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.1.6/src/ai_engine/types.py
--rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      209 2024-03-15 19:58:48.912304 uagents_ai_engine-0.2.0/README.md
+-rw-r--r--   0        0        0      394 2024-05-28 12:31:58.624725 uagents_ai_engine-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-03-15 19:58:57.112803 uagents_ai_engine-0.2.0/src/ai_engine/__init__.py
+-rw-r--r--   0        0        0     4682 2024-05-28 16:32:58.359073 uagents_ai_engine-0.2.0/src/ai_engine/chitchat.py
+-rw-r--r--   0        0        0     1405 2024-05-28 11:19:53.827379 uagents_ai_engine-0.2.0/src/ai_engine/dialogue.py
+-rw-r--r--   0        0        0     2967 2024-04-04 08:59:10.091701 uagents_ai_engine-0.2.0/src/ai_engine/messages.py
+-rw-r--r--   0        0        0      765 2024-03-15 19:58:48.914653 uagents_ai_engine-0.2.0/src/ai_engine/types.py
+-rw-r--r--   0        0        0      853 1970-01-01 00:00:00.000000 uagents_ai_engine-0.2.0/PKG-INFO
```

### Comparing `uagents_ai_engine-0.1.6/src/ai_engine/chitchat.py` & `uagents_ai_engine-0.2.0/src/ai_engine/chitchat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,50 @@
 """Specific dialogue class for the AI enabled chit-chat dialogue."""
 
 from typing import Type
 
 from uagents import Model
-from uagents.experimental.dialogues import Dialogue
+from uagents.experimental.dialogues import Dialogue, Node
 
-from .dialogue import create_edge, create_node
+from .dialogue import create_edge
 
 
 # Node definition for the dialogue states
-init_state = create_node(
+# Node definition for the dialogue states
+default_state = Node(
+    name="Default State",
+    description=(
+        "This is the default state of the dialogue. Every session starts in "
+        "this state and is automatically updated once the dialogue starts."
+    ),
+    initial=True,
+)
+init_state = Node(
     name="Initiated",
     description=(
         "This is the initial state of the dialogue that is only available at "
         "the receiving agent."
     ),
-    initial=True,
 )
-chatting_state = create_node(
+chatting_state = Node(
     name="Chit Chatting",
     description="This is the state in which messages are exchanged.",
 )
-end_state = create_node(
+end_state = Node(
     name="Concluded",
     description="This is the state after the dialogue has been concluded.",
-    terminal=True,
 )
 
 # Edge definition for the dialogue transitions
 init_session = create_edge(
     name="Initiate session",
     description="Every dialogue starts with this transition.",
     target="user",
     observable=True,
-    parent=None,
+    parent=default_state,
     child=init_state,
 )
 reject_session = create_edge(
     name="Reject dialogue",
     description=("This is the transition for when the dialogue is rejected"),
     target="user",
     observable=True,
@@ -78,21 +85,20 @@
     This is the specific definition of the rules for the chit-chat dialogue
     The rules will be predefined and the actual messages will be passed into it
     """
 
     def __init__(
         self,
         version: str,
-        agent_address: str,
     ) -> None:
         super().__init__(
             name="ChitChatDialogue",
             version=version,
-            agent_address=agent_address,
             nodes=[
+                default_state,
                 init_state,
                 chatting_state,
                 end_state,
             ],
             edges=[
                 init_session,
                 reject_session,
```

### Comparing `uagents_ai_engine-0.1.6/src/ai_engine/dialogue.py` & `uagents_ai_engine-0.2.0/src/ai_engine/dialogue.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,78 +4,34 @@
 from uagents.experimental.dialogues import Edge, Node
 
 
 # Extending dialogues with metadata for AI Engine support.
 # This will move to the uagents.experimental.dialogues module in the future.
 
 
-class NodeMetadata(BaseModel):
-    """Metadata for the nodes"""
-
-    # is the node an initial node
-    initial: bool = False
-
-    # is the node a terminal node
-    terminal: bool = False
-
-
 class EdgeMetadata(BaseModel):
     """Metadata for the edges"""
 
     # what is the target of this transition, user means direct message to the user, ai, system involves AI Engine processing
     target: Literal["user", "ai", "system", "agent"]
 
     # can the AI Engine observe this transition, and process the information
     observable: bool
 
 
-class NodeDescription(BaseModel):
-    """Temporary type to add structure to the node description"""
-
-    # the original description of the node
-    description: str
-
-    # the metadata of the node
-    metadata: NodeMetadata
-
-
 class EdgeDescription(BaseModel):
     """Temporary type to add structure to the edge description"""
 
     # the original description of the edge
     description: str
 
     # the metadata of the edge
     metadata: EdgeMetadata
 
 
-def create_node(
-    name: str,
-    description: str,
-    initial: bool = False,
-    terminal: bool = False,
-):
-    """Create a node with metadata"""
-
-    # create the metadata
-    metadata = NodeMetadata(initial=initial, terminal=terminal)
-
-    # description of the node
-    description = NodeDescription(
-        description=description,
-        metadata=metadata,
-    )
-
-    # create a new node
-    return Node(
-        name=name,
-        description=description.json(),
-    )
-
-
 def create_edge(
     name: str,
     description: str,
     target: Literal["user", "ai", "system", "agent"],
     observable: bool,
     parent: Node,
     child: Node,
```

### Comparing `uagents_ai_engine-0.1.6/src/ai_engine/messages.py` & `uagents_ai_engine-0.2.0/src/ai_engine/messages.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.6/src/ai_engine/types.py` & `uagents_ai_engine-0.2.0/src/ai_engine/types.py`

 * *Files identical despite different names*

### Comparing `uagents_ai_engine-0.1.6/PKG-INFO` & `uagents_ai_engine-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: uagents-ai-engine
-Version: 0.1.6
+Version: 0.2.0
 Summary: Integrating AI-Engine with UAgents
 License: Apache 2.0
 Keywords: uagents,agents,ai,ai-engine,fetch.ai
 Author: Fetch.AI Limited
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
-Requires-Dist: uagents (>=0.11.0)
+Requires-Dist: uagents (>=0.12.0)
 Description-Content-Type: text/markdown
 
 ## AI-Engine Integration
 
 📌 **Overview**
 
 This integration adds types required by AI-Engine to UAgents.
```

