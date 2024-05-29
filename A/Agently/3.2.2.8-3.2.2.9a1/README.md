# Comparing `tmp/Agently-3.2.2.8.tar.gz` & `tmp/Agently-3.2.2.9a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Agently-3.2.2.8.tar", last modified: Wed May  1 11:07:04 2024, max compression
+gzip compressed data, was "Agently-3.2.2.9a1.tar", last modified: Wed May 29 15:53:36 2024, max compression
```

## Comparing `Agently-3.2.2.8.tar` & `Agently-3.2.2.9a1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.884744 Agently-3.2.2.8/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.856281 Agently-3.2.2.8/Agently/
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.857666 Agently-3.2.2.8/Agently/Agent/
--rw-------   0 moxin      (501) staff       (20)    14434 2024-04-18 10:01:01.000000 Agently-3.2.2.8/Agently/Agent/Agent.py
--rw-------   0 moxin      (501) staff       (20)     2437 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Agent/AgentFactory.py
--rw-------   0 moxin      (501) staff       (20)       38 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Agent/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.858235 Agently-3.2.2.8/Agently/Facility/
--rw-------   0 moxin      (501) staff       (20)     1819 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Facility/FacilityManager.py
--rw-------   0 moxin      (501) staff       (20)       44 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Facility/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.858651 Agently-3.2.2.8/Agently/Request/
--rw-------   0 moxin      (501) staff       (20)     9943 2024-04-13 12:52:43.000000 Agently-3.2.2.8/Agently/Request/Request.py
--rw-------   0 moxin      (501) staff       (20)       28 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Request/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.859328 Agently-3.2.2.8/Agently/WebSocket/
--rw-------   0 moxin      (501) staff       (20)     9550 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/WebSocket/WebSocket.py
--rw-------   0 moxin      (501) staff       (20)       55 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/WebSocket/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.860830 Agently-3.2.2.8/Agently/Workflow/
--rw-------   0 moxin      (501) staff       (20)     7650 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/Chunk.py
--rw-------   0 moxin      (501) staff       (20)    16640 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/MainExecutor.py
--rw-------   0 moxin      (501) staff       (20)     6775 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/Schema.py
--rw-------   0 moxin      (501) staff       (20)     3165 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/Workflow.py
--rw-------   0 moxin      (501) staff       (20)       57 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.861501 Agently-3.2.2.8/Agently/Workflow/executors/
--rw-------   0 moxin      (501) staff       (20)       67 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/executors/StartExecutor.py
--rw-------   0 moxin      (501) staff       (20)        0 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/executors/__init__.py
--rw-------   0 moxin      (501) staff       (20)      245 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/executors/install.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.863003 Agently-3.2.2.8/Agently/Workflow/lib/
--rw-------   0 moxin      (501) staff       (20)     1470 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/BreakingHub.py
--rw-------   0 moxin      (501) staff       (20)      656 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/ChunkExecutorABC.py
--rw-------   0 moxin      (501) staff       (20)      426 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/ChunkExecutorManager.py
--rw-------   0 moxin      (501) staff       (20)      500 2024-04-17 12:32:55.000000 Agently-3.2.2.8/Agently/Workflow/lib/Store.py
--rw-------   0 moxin      (501) staff       (20)        0 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/__init__.py
--rw-------   0 moxin      (501) staff       (20)      515 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/constants.py
--rw-------   0 moxin      (501) staff       (20)     2058 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/lib/painter.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.864735 Agently-3.2.2.8/Agently/Workflow/utils/
--rw-------   0 moxin      (501) staff       (20)        0 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/__init__.py
--rw-------   0 moxin      (501) staff       (20)     4599 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/exec_tree.py
--rw-------   0 moxin      (501) staff       (20)     1411 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/find.py
--rw-------   0 moxin      (501) staff       (20)      613 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/logger.py
--rw-------   0 moxin      (501) staff       (20)      892 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/runtime_supports.py
--rw-------   0 moxin      (501) staff       (20)      242 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/utils/verify.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.865288 Agently-3.2.2.8/Agently/Workflow/yamlflow/
--rw-------   0 moxin      (501) staff       (20)       63 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.866378 Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/
--rw-------   0 moxin      (501) staff       (20)      500 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/Print.py
--rw-------   0 moxin      (501) staff       (20)      108 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/Start.py
--rw-------   0 moxin      (501) staff       (20)      289 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
--rw-------   0 moxin      (501) staff       (20)      767 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/__init__.py
--rw-------   0 moxin      (501) staff       (20)     5728 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/Workflow/yamlflow/yamlflow.py
--rw-------   0 moxin      (501) staff       (20)      571 2024-04-18 09:50:44.000000 Agently-3.2.2.8/Agently/__init__.py
--rw-------   0 moxin      (501) staff       (20)      515 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/_global.py
--rw-------   0 moxin      (501) staff       (20)      149 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/global_plugin_manager.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.866667 Agently-3.2.2.8/Agently/plugins/
--rw-------   0 moxin      (501) staff       (20)     4920 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.871470 Agently-3.2.2.8/Agently/plugins/agent_component/
--rw-------   0 moxin      (501) staff       (20)     2913 2024-04-18 10:14:06.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Decorator.py
--rw-------   0 moxin      (501) staff       (20)     2074 2024-04-21 13:45:58.000000 Agently-3.2.2.8/Agently/plugins/agent_component/EventListener.py
--rw-------   0 moxin      (501) staff       (20)     5290 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/OpenAIAssistant.py
--rw-------   0 moxin      (501) staff       (20)      785 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/ReplyReformer.py
--rw-------   0 moxin      (501) staff       (20)     3050 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Role.py
--rw-------   0 moxin      (501) staff       (20)     4075 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Search.py
--rw-------   0 moxin      (501) staff       (20)     9781 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Segment.py
--rw-------   0 moxin      (501) staff       (20)     8280 2024-04-18 12:06:13.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Session.py
--rw-------   0 moxin      (501) staff       (20)     3508 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Status.py
--rw-------   0 moxin      (501) staff       (20)     9970 2024-04-18 14:20:25.000000 Agently-3.2.2.8/Agently/plugins/agent_component/Tool.py
--rw-------   0 moxin      (501) staff       (20)     2977 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/UserInfo.py
--rw-r--r--   0 moxin      (501) staff       (20)     3308 2024-05-01 08:43:29.000000 Agently-3.2.2.8/Agently/plugins/agent_component/YAMLLoader.py
--rw-------   0 moxin      (501) staff       (20)     2220 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/__init__.py
--rw-------   0 moxin      (501) staff       (20)      505 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.871972 Agently-3.2.2.8/Agently/plugins/agent_component/utils/
--rw-------   0 moxin      (501) staff       (20)      588 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/utils/ComponentABC.py
--rw-------   0 moxin      (501) staff       (20)       38 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/agent_component/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.873476 Agently-3.2.2.8/Agently/plugins/facility/
--rw-------   0 moxin      (501) staff       (20)     4633 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/Embedding.py
--rw-------   0 moxin      (501) staff       (20)     1874 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/RoleManager.py
--rw-------   0 moxin      (501) staff       (20)     1216 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/StatusManager.py
--rw-------   0 moxin      (501) staff       (20)     2120 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/__init__.py
--rw-------   0 moxin      (501) staff       (20)       85 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.873936 Agently-3.2.2.8/Agently/plugins/facility/utils/
--rw-------   0 moxin      (501) staff       (20)      266 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/utils/FacilityABC.py
--rw-------   0 moxin      (501) staff       (20)       36 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/facility/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.877104 Agently-3.2.2.8/Agently/plugins/request/
--rw-------   0 moxin      (501) staff       (20)    12099 2024-04-26 13:07:16.000000 Agently-3.2.2.8/Agently/plugins/request/AzureOpenAI.py
--rw-------   0 moxin      (501) staff       (20)     8057 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/Claude.py
--rw-------   0 moxin      (501) staff       (20)    10303 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/ERNIE.py
--rw-------   0 moxin      (501) staff       (20)     7368 2024-04-17 12:29:18.000000 Agently-3.2.2.8/Agently/plugins/request/Google.py
--rw-------   0 moxin      (501) staff       (20)     7769 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/Kimi.py
--rw-------   0 moxin      (501) staff       (20)    12270 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/MiniMax.py
--rw-------   0 moxin      (501) staff       (20)    13476 2024-04-26 13:22:22.000000 Agently-3.2.2.8/Agently/plugins/request/OAIClient.py
--rw-------   0 moxin      (501) staff       (20)    11813 2024-04-24 15:11:10.000000 Agently-3.2.2.8/Agently/plugins/request/OpenAI.py
--rw-------   0 moxin      (501) staff       (20)    12624 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/ZhipuAI.py
--rw-------   0 moxin      (501) staff       (20)     2120 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/__init__.py
--rw-------   0 moxin      (501) staff       (20)      139 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.878144 Agently-3.2.2.8/Agently/plugins/request/utils/
--rw-------   0 moxin      (501) staff       (20)     5307 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/utils/RequestABC.py
--rw-------   0 moxin      (501) staff       (20)      162 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/utils/__init__.py
--rw-------   0 moxin      (501) staff       (20)     2728 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/utils/format.py
--rw-------   0 moxin      (501) staff       (20)     4330 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/request/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.879101 Agently-3.2.2.8/Agently/plugins/storage/
--rw-------   0 moxin      (501) staff       (20)     3156 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/storage/FileStorage.py
--rw-------   0 moxin      (501) staff       (20)     2120 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/storage/__init__.py
--rw-------   0 moxin      (501) staff       (20)      131 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/storage/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.879521 Agently-3.2.2.8/Agently/plugins/storage/utils/
--rw-------   0 moxin      (501) staff       (20)      745 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/storage/utils/StorageABC.py
--rw-------   0 moxin      (501) staff       (20)       34 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/storage/utils/__init__.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.880550 Agently-3.2.2.8/Agently/plugins/tool/
--rw-------   0 moxin      (501) staff       (20)     1828 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/Code.py
--rw-------   0 moxin      (501) staff       (20)     5915 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/Web.py
--rw-------   0 moxin      (501) staff       (20)     2120 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/__init__.py
--rw-------   0 moxin      (501) staff       (20)      104 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/config.ini
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.881123 Agently-3.2.2.8/Agently/plugins/tool/utils/
--rw-------   0 moxin      (501) staff       (20)      443 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/utils/ToolABC.py
--rw-------   0 moxin      (501) staff       (20)       28 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/plugins/tool/utils/__init__.py
--rw-------   0 moxin      (501) staff       (20)      213 2024-04-18 14:35:43.000000 Agently-3.2.2.8/Agently/requirements.txt
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.883704 Agently-3.2.2.8/Agently/utils/
--rw-------   0 moxin      (501) staff       (20)     2896 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/AliasManager.py
--rw-------   0 moxin      (501) staff       (20)     6706 2024-04-18 09:58:41.000000 Agently-3.2.2.8/Agently/utils/DataOps.py
--rw-------   0 moxin      (501) staff       (20)      323 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/IdGenerator.py
--rw-------   0 moxin      (501) staff       (20)     2282 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/PluginManager.py
--rw-------   0 moxin      (501) staff       (20)     2418 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/RuntimeCtx.py
--rw-------   0 moxin      (501) staff       (20)     1934 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/StorageDelegate.py
--rw-------   0 moxin      (501) staff       (20)     4963 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/ToolManager.py
--rw-------   0 moxin      (501) staff       (20)      491 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/__init__.py
--rw-------   0 moxin      (501) staff       (20)     1928 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/check_version.py
--rw-------   0 moxin      (501) staff       (20)     2868 2024-04-13 12:56:10.000000 Agently-3.2.2.8/Agently/utils/load_json.py
--rw-------   0 moxin      (501) staff       (20)     4328 2024-04-12 12:30:56.000000 Agently-3.2.2.8/Agently/utils/transform.py
-drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-01 11:07:04.883978 Agently-3.2.2.8/Agently.egg-info/
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-05-01 11:07:04.000000 Agently-3.2.2.8/Agently.egg-info/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-05-01 11:07:04.000000 Agently-3.2.2.8/Agently.egg-info/SOURCES.txt
--rw-r--r--   0 moxin      (501) staff       (20)        1 2024-05-01 11:07:04.000000 Agently-3.2.2.8/Agently.egg-info/dependency_links.txt
--rw-r--r--   0 moxin      (501) staff       (20)      130 2024-05-01 11:07:04.000000 Agently-3.2.2.8/Agently.egg-info/requires.txt
--rw-r--r--   0 moxin      (501) staff       (20)        8 2024-05-01 11:07:04.000000 Agently-3.2.2.8/Agently.egg-info/top_level.txt
--rw-r--r--   0 moxin      (501) staff       (20)      846 2024-05-01 11:07:04.884445 Agently-3.2.2.8/PKG-INFO
--rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-01 11:07:04.884801 Agently-3.2.2.8/setup.cfg
--rw-r--r--   0 moxin      (501) staff       (20)      973 2024-05-01 11:06:52.000000 Agently-3.2.2.8/setup.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.359912 Agently-3.2.2.9a1/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.328159 Agently-3.2.2.9a1/Agently/
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.329615 Agently-3.2.2.9a1/Agently/Agent/
+-rw-r--r--   0 moxin      (501) staff       (20)    14491 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/Agent.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2437 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/AgentFactory.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Agent/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.330717 Agently-3.2.2.9a1/Agently/Facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     1819 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Facility/FacilityManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)       44 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Facility/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.331097 Agently-3.2.2.9a1/Agently/Request/
+-rw-r--r--   0 moxin      (501) staff       (20)    10000 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Request/Request.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Request/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.331514 Agently-3.2.2.9a1/Agently/WebSocket/
+-rw-r--r--   0 moxin      (501) staff       (20)     9550 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/WebSocket/WebSocket.py
+-rw-r--r--   0 moxin      (501) staff       (20)       55 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/WebSocket/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.333120 Agently-3.2.2.9a1/Agently/Workflow/
+-rw-r--r--   0 moxin      (501) staff       (20)     7650 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Chunk.py
+-rw-r--r--   0 moxin      (501) staff       (20)    16640 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/MainExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6775 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Schema.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3222 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/Workflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)       57 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.334395 Agently-3.2.2.9a1/Agently/Workflow/executors/
+-rw-r--r--   0 moxin      (501) staff       (20)       67 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/StartExecutor.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      245 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/executors/install.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.335401 Agently-3.2.2.9a1/Agently/Workflow/lib/
+-rw-r--r--   0 moxin      (501) staff       (20)     1470 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/BreakingHub.py
+-rw-r--r--   0 moxin      (501) staff       (20)      656 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      426 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/Store.py
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/constants.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2058 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/lib/painter.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.337165 Agently-3.2.2.9a1/Agently/Workflow/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)        0 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4599 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/exec_tree.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1411 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/find.py
+-rw-r--r--   0 moxin      (501) staff       (20)      613 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/logger.py
+-rw-r--r--   0 moxin      (501) staff       (20)      892 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/runtime_supports.py
+-rw-r--r--   0 moxin      (501) staff       (20)      242 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/utils/verify.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.338693 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/
+-rw-r--r--   0 moxin      (501) staff       (20)       63 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.339396 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/
+-rw-r--r--   0 moxin      (501) staff       (20)      500 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/Print.py
+-rw-r--r--   0 moxin      (501) staff       (20)      108 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/Start.py
+-rw-r--r--   0 moxin      (501) staff       (20)      289 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/UserInput.py
+-rw-r--r--   0 moxin      (501) staff       (20)      767 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5728 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/Workflow/yamlflow/yamlflow.py
+-rw-r--r--   0 moxin      (501) staff       (20)      571 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      515 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/_global.py
+-rw-r--r--   0 moxin      (501) staff       (20)      149 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/global_plugin_manager.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.339597 Agently-3.2.2.9a1/Agently/plugins/
+-rw-r--r--   0 moxin      (501) staff       (20)     4920 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.344391 Agently-3.2.2.9a1/Agently/plugins/agent_component/
+-rw-r--r--   0 moxin      (501) staff       (20)     2913 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Decorator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2074 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/EventListener.py
+-rw-r--r--   0 moxin      (501) staff       (20)     5290 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/OpenAIAssistant.py
+-rw-r--r--   0 moxin      (501) staff       (20)      785 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/ReplyReformer.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3050 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Role.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4075 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Search.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9781 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Segment.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8280 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Session.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3508 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Status.py
+-rw-r--r--   0 moxin      (501) staff       (20)     9970 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/Tool.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2977 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/UserInfo.py
+-rw-r--r--   0 moxin      (501) staff       (20)     3849 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/YAMLLoader.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2220 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      505 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.345807 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      588 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/ComponentABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.346544 Agently-3.2.2.9a1/Agently/plugins/facility/
+-rw-r--r--   0 moxin      (501) staff       (20)     4633 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/Embedding.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1874 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/RoleManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1216 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/StatusManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)       85 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.346874 Agently-3.2.2.9a1/Agently/plugins/facility/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      266 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/utils/FacilityABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       36 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/facility/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.352241 Agently-3.2.2.9a1/Agently/plugins/request/
+-rw-r--r--   0 moxin      (501) staff       (20)    12099 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/AzureOpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     8057 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Claude.py
+-rw-r--r--   0 moxin      (501) staff       (20)    10461 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/ERNIE.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7368 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Google.py
+-rw-r--r--   0 moxin      (501) staff       (20)     7769 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/Kimi.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12270 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/MiniMax.py
+-rw-r--r--   0 moxin      (501) staff       (20)    13476 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/OAIClient.py
+-rw-r--r--   0 moxin      (501) staff       (20)    11813 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/OpenAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)    12624 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/ZhipuAI.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      139 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.352786 Agently-3.2.2.9a1/Agently/plugins/request/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     5307 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/RequestABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)      162 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2728 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/format.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4455 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/request/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.353285 Agently-3.2.2.9a1/Agently/plugins/storage/
+-rw-r--r--   0 moxin      (501) staff       (20)     3156 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/FileStorage.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      131 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.353553 Agently-3.2.2.9a1/Agently/plugins/storage/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      745 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/utils/StorageABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       34 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/storage/utils/__init__.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.355134 Agently-3.2.2.9a1/Agently/plugins/tool/
+-rw-r--r--   0 moxin      (501) staff       (20)     1828 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/Code.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6400 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/Web.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2120 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      104 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/config.ini
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.355409 Agently-3.2.2.9a1/Agently/plugins/tool/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)      443 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/utils/ToolABC.py
+-rw-r--r--   0 moxin      (501) staff       (20)       28 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/plugins/tool/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)      213 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/requirements.txt
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.359394 Agently-3.2.2.9a1/Agently/utils/
+-rw-r--r--   0 moxin      (501) staff       (20)     2896 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/AliasManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     6706 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/DataOps.py
+-rw-r--r--   0 moxin      (501) staff       (20)      323 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/IdGenerator.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2282 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/PluginManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2418 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/RuntimeCtx.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1934 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/StorageDelegate.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4963 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/ToolManager.py
+-rw-r--r--   0 moxin      (501) staff       (20)      491 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/__init__.py
+-rw-r--r--   0 moxin      (501) staff       (20)     1928 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/check_version.py
+-rw-r--r--   0 moxin      (501) staff       (20)     2868 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/load_json.py
+-rw-r--r--   0 moxin      (501) staff       (20)     4328 2024-05-29 15:11:33.000000 Agently-3.2.2.9a1/Agently/utils/transform.py
+drwxr-xr-x   0 moxin      (501) staff       (20)        0 2024-05-29 15:53:36.328705 Agently-3.2.2.9a1/Agently.egg-info/
+-rw-r--r--   0 moxin      (501) staff       (20)      850 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)     3824 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/SOURCES.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        1 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/dependency_links.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      130 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/requires.txt
+-rw-r--r--   0 moxin      (501) staff       (20)        8 2024-05-29 15:53:36.000000 Agently-3.2.2.9a1/Agently.egg-info/top_level.txt
+-rw-r--r--   0 moxin      (501) staff       (20)      850 2024-05-29 15:53:36.359707 Agently-3.2.2.9a1/PKG-INFO
+-rw-r--r--   0 moxin      (501) staff       (20)       38 2024-05-29 15:53:36.359960 Agently-3.2.2.9a1/setup.cfg
+-rw-------   0 moxin      (501) staff       (20)     1014 2024-05-29 15:13:08.000000 Agently-3.2.2.9a1/setup.py
```

### Comparing `Agently-3.2.2.8/Agently/Agent/Agent.py` & `Agently-3.2.2.9a1/Agently/Agent/Agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,14 +234,16 @@
             if self.settings.get_trace_back("is_debug"):
                 reply = loop.run_until_complete(self.start_async(request_type))
                 reply_queue.put_nowait(reply)
             else:
                 try:
                     reply = loop.run_until_complete(self.start_async(request_type))
                     reply_queue.put_nowait(reply)
+                except:
+                    reply = None
                 finally:
                     loop.close()
         theard = threading.Thread(target=start_in_theard)
         theard.start()
         theard.join()
         try:        
             reply = reply_queue.get_nowait()
```

### Comparing `Agently-3.2.2.8/Agently/Agent/AgentFactory.py` & `Agently-3.2.2.9a1/Agently/Agent/AgentFactory.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Facility/FacilityManager.py` & `Agently-3.2.2.9a1/Agently/Facility/FacilityManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Request/Request.py` & `Agently-3.2.2.9a1/Agently/Request/Request.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,16 @@
             if self.settings.get_trace_back("is_debug"):
                 reply = loop.run_until_complete(self.get_result_async(request_type))
                 reply_queue.put_nowait(reply)
             else:
                 try:
                     reply = loop.run_until_complete(self.get_result_async(request_type))
                     reply_queue.put_nowait(reply)
+                except:
+                    reply = None
                 finally:
                     loop.close()
         theard = threading.Thread(target=start_in_theard)
         theard.start()
         theard.join()        
         reply = reply_queue.get_nowait()
         return reply
```

### Comparing `Agently-3.2.2.8/Agently/WebSocket/WebSocket.py` & `Agently-3.2.2.9a1/Agently/WebSocket/WebSocket.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/Chunk.py` & `Agently-3.2.2.9a1/Agently/Workflow/Chunk.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/MainExecutor.py` & `Agently-3.2.2.9a1/Agently/Workflow/MainExecutor.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/Schema.py` & `Agently-3.2.2.9a1/Agently/Workflow/Schema.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/Workflow.py` & `Agently-3.2.2.9a1/Agently/Workflow/Workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.executor = MainExecutor(self.workflow_id, self.settings)
         # 装载内置类型
         mount_built_in_executors(self.executor)
         # Chunk Storage
         self.chunks = {}
         # Executor Manager
         self.executor_manager = ChunkExecutorManager()
+        self.chunk("start", type = "Start")(lambda:None)
 
     def chunk(self, chunk_id: str, type=EXECUTOR_TYPE_NORMAL, **chunk_desc):
         if "title" not in chunk_desc or chunk_desc["title"] == "":
             chunk_desc.update({ "title": chunk_id })
         def create_chunk_decorator(func: callable):
             return self.chunks.update({
                 chunk_id: self.schema.create_chunk(
```

### Comparing `Agently-3.2.2.8/Agently/Workflow/lib/BreakingHub.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/BreakingHub.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/lib/ChunkExecutorABC.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/ChunkExecutorABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/lib/constants.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/constants.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/lib/painter.py` & `Agently-3.2.2.9a1/Agently/Workflow/lib/painter.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/utils/exec_tree.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/exec_tree.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/utils/find.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/find.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/utils/logger.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/logger.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/utils/runtime_supports.py` & `Agently-3.2.2.9a1/Agently/Workflow/utils/runtime_supports.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/yamlflow/preset_chunks/__init__.py` & `Agently-3.2.2.9a1/Agently/Workflow/yamlflow/preset_chunks/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/Workflow/yamlflow/yamlflow.py` & `Agently-3.2.2.9a1/Agently/Workflow/yamlflow/yamlflow.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/__init__.py` & `Agently-3.2.2.9a1/Agently/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/_global.py` & `Agently-3.2.2.9a1/Agently/_global.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Decorator.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Decorator.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/EventListener.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/EventListener.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/OpenAIAssistant.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/OpenAIAssistant.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/ReplyReformer.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/ReplyReformer.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Role.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Role.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Search.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Search.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Segment.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Segment.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Session.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Session.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Status.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Status.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/Tool.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/Tool.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/UserInfo.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/UserInfo.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/YAMLLoader.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/YAMLLoader.py`

 * *Files 16% similar despite different names*

```diff
@@ -42,29 +42,38 @@
         yaml_dict = {}
         if variables:
             use_agently_style = True
         if not path and not yaml:
             raise Exception(f"[Agent Component: YAMLReader]: one parameter between `path` or `yaml` must be provided.")
         try:
             if path:
-                with open(path, "r") as yaml_file:
+                with open(path, "r", encoding="utf-8") as yaml_file:
                     yaml_dict = YAML.safe_load(yaml_file)
                     if use_agently_style:
                         yaml_dict = self.transform_to_agently_style(yaml_dict, variables=variables)
             else:
                 yaml_dict = YAML.safe_load(yaml)
                 if use_agently_style:
                     yaml_dict = self.transform_to_agently_style(yaml_dict, variables=variables)
         except Exception as e:
             raise Exception(f"[Agent Component: YAMLReader]: Error occured when read YAML from path '{ path }'.\nError: { str(e) }")
         # run agent alias
         agent_alias_list = dir(self.agent)
         for alias, value in yaml_dict.items():
             if alias in agent_alias_list:
-                getattr(self.agent, alias)(value)
+                args = []
+                kwargs = {}                    
+                if isinstance(value, dict) and ("$args" in value or "$kwargs" in value):
+                    if "$args" in value and isinstance(value["$args"], list):
+                        args = value["$args"].copy()
+                    if "$kwargs" in value and isinstance(value["$kwargs"], dict):
+                        kwargs = value["$kwargs"].copy()
+                    getattr(self.agent, alias)(*args, **kwargs)
+                else:
+                    getattr(self.agent, alias)(value)
         return self.agent
 
     def export(self):
         return {
             "alias": {
                 "load_yaml_prompt": { "func": self.load_yaml_prompt },
             }
```

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/agent_component/utils/ComponentABC.py` & `Agently-3.2.2.9a1/Agently/plugins/agent_component/utils/ComponentABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/facility/Embedding.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/Embedding.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/facility/RoleManager.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/RoleManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/facility/StatusManager.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/StatusManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/facility/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/facility/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/AzureOpenAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/AzureOpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/Claude.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Claude.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/ERNIE.py` & `Agently-3.2.2.9a1/Agently/plugins/request/ERNIE.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,19 +90,20 @@
         access_token = self.model_settings.get_trace_back("auth", {})
         access_token = access_token if isinstance(access_token, dict) else {}
         request_data = {}
         # request type: chat
         if self.request_type == "chat":
             if "model" not in options:
                 options["model"] = "ernie-4.0"
-            if "aistudio" not in access_token:
+            if "aistudio" not in access_token and "qianfan" not in access_token:
                 raise Exception(
-                    f"[Request] ERNIE require 'access-token-for-aistudio' when request type is '{self.request_type}'. Use .set_model_auth({{ 'aistudio': <YOUR-ACCESS-TOKEN-FOR-AISTUDIO> }}) to set.")
-            erniebot.api_type = "aistudio"
-            erniebot.access_token = access_token["aistudio"]
+                    f"[Request] ERNIE require 'access-token-for-aistudio or access-token-for-qianfan' when request type is '{self.request_type}'. Use .set_model_auth({{ 'aistudio': <YOUR-ACCESS-TOKEN-FOR-AISTUDIO> }} or {{ 'qianfan': <YOUR-ACCESS-TOKEN-FOR-QIANFAN> }}) to set.")
+            api_type = next(iter(access_token))
+            erniebot.api_type = api_type
+            erniebot.access_token = access_token[api_type]
             messages = self.construct_request_messages()
             request_messages = []
             system_prompt = ""
             for message in messages:
                 if message["role"] == "system":
                     system_prompt += f"{ message['content'] }\n"
                 else:
```

### Comparing `Agently-3.2.2.8/Agently/plugins/request/Google.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Google.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/Kimi.py` & `Agently-3.2.2.9a1/Agently/plugins/request/Kimi.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/MiniMax.py` & `Agently-3.2.2.9a1/Agently/plugins/request/MiniMax.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/OAIClient.py` & `Agently-3.2.2.9a1/Agently/plugins/request/OAIClient.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/OpenAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/OpenAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/ZhipuAI.py` & `Agently-3.2.2.9a1/Agently/plugins/request/ZhipuAI.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/request/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/utils/RequestABC.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/RequestABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/utils/format.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/format.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/request/utils/transform.py` & `Agently-3.2.2.9a1/Agently/utils/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     elif isinstance(origin, (list, set)):
         json_string = ""
         if layer_count > 0:
             json_string += "\n"
         json_string += ("\t" * layer_count) + "[\n"
         for item in origin:
             json_string += ("\t" * (layer_count + 1)) + to_json_desc(item, layer_count + 1) + ",\n"
-        json_string += ("\t" * (layer_count + 1)) + "\\\\...\n"
+        json_string += ("\t" * (layer_count + 1)) + "...\n"
         if layer_count > 0:
             json_string += ("\t" * layer_count) + "],"
         else:
             json_string += "]"
         return json_string
     elif isinstance(origin, tuple):
         if isinstance(origin[0], (dict, list, set)):
@@ -99,16 +99,16 @@
                         continue
                 if char == "\"":
                     in_quote = True
                 if char == "[" or char == "{":
                     layer += 1
                 elif char == "]" or char == "}":
                     layer -= 1
-                elif char in ("\t", " ", "\n"):
-                    char = ""
+                #elif char in ("\t", " ", "\n"):
+                    #char = ""
                 json_blocks[block_num] += char
             else:
                 if char == "\\":
                     char += origin[index + 1]
                     skip_next = True
                 elif char == "\n":
                     char = "\\n"
```

### Comparing `Agently-3.2.2.8/Agently/plugins/storage/FileStorage.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/storage/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/storage/utils/StorageABC.py` & `Agently-3.2.2.9a1/Agently/plugins/storage/utils/StorageABC.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/tool/Code.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/Code.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/plugins/tool/Web.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/Web.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from .utils import ToolABC
 import time
 import httpx
 from duckduckgo_search import DDGS
 import requests
 from bs4 import BeautifulSoup
 
@@ -61,36 +62,49 @@
         if "timelimit" not in options:
             options.update({ "timelimit": "w" })
         if "max_results" not in options:
             options.update({ "max_results": 10 })
         return self.search(keywords, options=options, proxy=proxy, type=2)
 
     def browse(self, url: str, *, retry_times:int = 0, proxy: str=None):
+        content = ""
         try:
-            request_options = {}
+            request_options = {
+                "headers": { "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36" }
+            }
             if proxy:
                 if proxy.startswith("http:"):
                     request_options.update({ "proxies": { "http": proxy } })
                 elif proxy.startswith("https:"):
                     request_options.update({ "proxies": { "https": proxy } })
-            request_options.update({ "headers": { "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/122.0.0.0 Safari/537.36"} })
-            page_response = requests.get(url, **request_options)
-            soup = BeautifulSoup(page_response.content, 'html.parser')
-            paragraphs = soup.find_all('p')
-            texts = [p.get_text() for p in paragraphs]
-            page_content = '\n'.join(texts)
-            if page_content and page_content != "":
-                return page_content
-            else:
-                return f"Can not get content from url: { url }"
+            page = requests.get(
+                url,
+                **request_options
+            )
+            soup = BeautifulSoup(page.content, "html.parser")
+            # find text in p, list, pre (github code), td
+            chunks = soup.find_all(["h1", "h2", "h3", "h4", "h5", "p", "pre", "td"])
+            for chunk in chunks:
+                if chunk.name.startswith("h"):
+                    content += "#" * int(chunk.name[-1]) + " " + chunk.get_text() + "\n"
+                else:
+                    text = chunk.get_text()
+                    if text and text != "":
+                        content += text + "\n"
+            # find text in div that class=content
+            divs = soup.find("div", class_="content")
+            if divs:
+                chunks_with_text = divs.find_all(text=True)
+                for chunk in chunks_with_text:
+                    if isinstance(chunk, str) and chunk.strip():
+                        content += chunk.strip() + "\n"
+            content = re.sub(r"\n+", "\n", content)
+            return content
         except Exception as e:
-            if retry_times < 3:
-                return self.browse(url, retry_times = retry_times + 1, proxy = proxy)
-            else:
-                return f"Can not get content from url: { url }\nError: { str(e) }"
+            return f"Can not browse '{ url }'.\tError: { str(e) }"
 
     def export(self):
         return {
             "search": {
                 "desc": "search {keywords}.",
                 "args": {
                     "keywords": ("String", "[*Required]keywords to search, seperate keywords by ' '."),
```

### Comparing `Agently-3.2.2.8/Agently/plugins/tool/__init__.py` & `Agently-3.2.2.9a1/Agently/plugins/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/AliasManager.py` & `Agently-3.2.2.9a1/Agently/utils/AliasManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/DataOps.py` & `Agently-3.2.2.9a1/Agently/utils/DataOps.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/PluginManager.py` & `Agently-3.2.2.9a1/Agently/utils/PluginManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/RuntimeCtx.py` & `Agently-3.2.2.9a1/Agently/utils/RuntimeCtx.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/StorageDelegate.py` & `Agently-3.2.2.9a1/Agently/utils/StorageDelegate.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/ToolManager.py` & `Agently-3.2.2.9a1/Agently/utils/ToolManager.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/check_version.py` & `Agently-3.2.2.9a1/Agently/utils/check_version.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/load_json.py` & `Agently-3.2.2.9a1/Agently/utils/load_json.py`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/Agently/utils/transform.py` & `Agently-3.2.2.9a1/Agently/plugins/request/utils/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import json
 import re
 import yaml
 
+def tuple_representer(dumper, data):
+    return dumper.represent_list(data)
+
+yaml.add_representer(tuple, tuple_representer)
+
 def to_prompt_structure(prompt_dict: dict, layer_count: int=1, end: str=""):
     prompt = ""
     for key, content in prompt_dict.items():
         prompt += f"{ '#' * layer_count } { key }:\n"
         if isinstance(content, dict):
             prompt += to_prompt_structure(content, layer_count + 1) + '\n'
         else:
@@ -40,15 +45,15 @@
     elif isinstance(origin, (list, set)):
         json_string = ""
         if layer_count > 0:
             json_string += "\n"
         json_string += ("\t" * layer_count) + "[\n"
         for item in origin:
             json_string += ("\t" * (layer_count + 1)) + to_json_desc(item, layer_count + 1) + ",\n"
-        json_string += ("\t" * (layer_count + 1)) + "...\n"
+        json_string += ("\t" * (layer_count + 1)) + "\\\\...\n"
         if layer_count > 0:
             json_string += ("\t" * layer_count) + "],"
         else:
             json_string += "]"
         return json_string
     elif isinstance(origin, tuple):
         if isinstance(origin[0], (dict, list, set)):
@@ -99,16 +104,16 @@
                         continue
                 if char == "\"":
                     in_quote = True
                 if char == "[" or char == "{":
                     layer += 1
                 elif char == "]" or char == "}":
                     layer -= 1
-                #elif char in ("\t", " ", "\n"):
-                    #char = ""
+                elif char in ("\t", " ", "\n"):
+                    char = ""
                 json_blocks[block_num] += char
             else:
                 if char == "\\":
                     char += origin[index + 1]
                     skip_next = True
                 elif char == "\n":
                     char = "\\n"
```

### Comparing `Agently-3.2.2.8/Agently.egg-info/PKG-INFO` & `Agently-3.2.2.9a1/Agently.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.8
+Version: 3.2.2.9a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.8
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: tornado
 Requires-Dist: openai
 Requires-Dist: erniebot
 Requires-Dist: zhipuai
```

### Comparing `Agently-3.2.2.8/Agently.egg-info/SOURCES.txt` & `Agently-3.2.2.9a1/Agently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Agently-3.2.2.8/PKG-INFO` & `Agently-3.2.2.9a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: Agently
-Version: 3.2.2.8
+Version: 3.2.2.9a1
 Summary: Agently, a framework to build applications based on language model powered intelligent agents.
 Home-page: https://github.com/Maplemx/Agently
 Author: Maplemx
 Author-email: maplemx@gmail.com
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3
+Requires-Python: >=3.8
 Requires-Dist: httpx
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: tornado
 Requires-Dist: openai
 Requires-Dist: erniebot
 Requires-Dist: zhipuai
```

### Comparing `Agently-3.2.2.8/setup.py` & `Agently-3.2.2.9a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,26 +4,28 @@
     origin_requirements = f.read().splitlines()
 
 requirements = []
 for requirement in origin_requirements:
     if not requirement.startswith("#"):
         requirements.append(requirement)
 
+
 setuptools.setup(
     name = "Agently",
-    version = "3.2.2.8",
+    version = "3.2.2.9-alpha-1",
     author = "Maplemx",
     author_email = "maplemx@gmail.com",
     description = "Agently, a framework to build applications based on language model powered intelligent agents.",
     long_description = "https://github.com/Maplemx/Agently",
     url = "https://github.com/Maplemx/Agently",
     license='Apache License, Version 2.0',
+    #packages = ["Agently"],
     packages = setuptools.find_packages(),
     package_data = {"": ["*.txt", "*.ini"]},
     install_requires= requirements,
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3',
-)
+    python_requires=">=3.8",
+)
```

