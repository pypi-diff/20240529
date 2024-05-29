# Comparing `tmp/camel_ai-0.1.5.tar.gz` & `tmp/camel_ai-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camel_ai-0.1.5.tar", max compression
+gzip compressed data, was "camel_ai-0.1.5.1.tar", max compression
```

## Comparing `camel_ai-0.1.5.tar` & `camel_ai-0.1.5.1.tar`

### file list

```diff
@@ -1,119 +1,119 @@
--rw-r--r--   0        0        0    17382 2024-05-28 13:20:14.164937 camel_ai-0.1.5/README.md
--rw-r--r--   0        0        0      778 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/__init__.py
--rw-r--r--   0        0        0     1494 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/__init__.py
--rw-r--r--   0        0        0     1130 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/base.py
--rw-r--r--   0        0        0    21701 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/chat_agent.py
--rw-r--r--   0        0        0     7377 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/critic_agent.py
--rw-r--r--   0        0        0    13050 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/deductive_reasoner_agent.py
--rw-r--r--   0        0        0     7322 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/embodied_agent.py
--rw-r--r--   0        0        0     8783 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/knowledge_graph_agent.py
--rw-r--r--   0        0        0     4879 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/role_assignment_agent.py
--rw-r--r--   0        0        0    14907 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/task_agent.py
--rw-r--r--   0        0        0      862 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/tool_agents/__init__.py
--rw-r--r--   0        0        0     1399 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/tool_agents/base.py
--rw-r--r--   0        0        0     8723 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/agents/tool_agents/hugging_face_tool_agent.py
--rw-r--r--   0        0        0     1061 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/configs/__init__.py
--rw-r--r--   0        0        0     3315 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/configs/anthropic_config.py
--rw-r--r--   0        0        0      870 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/configs/base_config.py
--rw-r--r--   0        0        0     6603 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/configs/openai_config.py
--rw-r--r--   0        0        0      952 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/embeddings/__init__.py
--rw-r--r--   0        0        0     2208 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/embeddings/base.py
--rw-r--r--   0        0        0     2873 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/embeddings/openai_embedding.py
--rw-r--r--   0        0        0     2312 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/embeddings/sentence_transformers_embeddings.py
--rw-r--r--   0        0        0     1452 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/__init__.py
--rw-r--r--   0        0        0    12468 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/google_maps_function.py
--rw-r--r--   0        0        0     1703 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/math_functions.py
--rw-r--r--   0        0        0    15036 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_function.py
--rw-r--r--   0        0        0      708 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/coursera/__init__.py
--rw-r--r--   0        0        0     1981 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/coursera/openapi.yaml
--rw-r--r--   0        0        0      708 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/klarna/__init__.py
--rw-r--r--   0        0        0     2887 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/klarna/openapi.yaml
--rw-r--r--   0        0        0      708 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/speak/__init__.py
--rw-r--r--   0        0        0     6557 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/open_api_specs/speak/openapi.yaml
--rw-r--r--   0        0        0    14933 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/openai_function.py
--rw-r--r--   0        0        0     2281 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/retrieval_functions.py
--rw-r--r--   0        0        0    12639 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/search_functions.py
--rw-r--r--   0        0        0     8789 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/slack_functions.py
--rw-r--r--   0        0        0    17254 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/twitter_function.py
--rw-r--r--   0        0        0     5881 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/functions/weather_functions.py
--rw-r--r--   0        0        0    10437 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/generators.py
--rw-r--r--   0        0        0     4949 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/human.py
--rw-r--r--   0        0        0     1040 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/interpreters/__init__.py
--rw-r--r--   0        0        0     1904 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/interpreters/base.py
--rw-r--r--   0        0        0    21866 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/interpreters/internal_python_interpreter.py
--rw-r--r--   0        0        0      886 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/interpreters/interpreter_error.py
--rw-r--r--   0        0        0     6835 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/interpreters/subprocess_interpreter.py
--rw-r--r--   0        0        0      856 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/loaders/__init__.py
--rw-r--r--   0        0        0     8664 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/loaders/base_io.py
--rw-r--r--   0        0        0    25870 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/loaders/unstructured_io.py
--rw-r--r--   0        0        0     1364 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/__init__.py
--rw-r--r--   0        0        0     6110 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/agent_memories.py
--rw-r--r--   0        0        0     5003 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/base.py
--rw-r--r--   0        0        0      860 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/blocks/__init__.py
--rw-r--r--   0        0        0     4609 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/blocks/chat_history_block.py
--rw-r--r--   0        0        0     3850 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/blocks/vectordb_block.py
--rw-r--r--   0        0        0      806 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/context_creators/__init__.py
--rw-r--r--   0        0        0     5378 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/context_creators/score_based.py
--rw-r--r--   0        0        0     3618 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/memories/records.py
--rw-r--r--   0        0        0     1468 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/messages/__init__.py
--rw-r--r--   0        0        0    10131 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/messages/base.py
--rw-r--r--   0        0        0     3841 2024-05-28 13:20:14.168937 camel_ai-0.1.5/camel/messages/func_message.py
--rw-r--r--   0        0        0     1168 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/__init__.py
--rw-r--r--   0        0        0     5112 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/anthropic_model.py
--rw-r--r--   0        0        0     3904 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/base_model.py
--rw-r--r--   0        0        0     2418 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/model_factory.py
--rw-r--r--   0        0        0     5856 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/open_source_model.py
--rw-r--r--   0        0        0     9799 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/openai_audio_models.py
--rw-r--r--   0        0        0     4164 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/openai_model.py
--rw-r--r--   0        0        0     3631 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/models/stub_model.py
--rw-r--r--   0        0        0     1790 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/__init__.py
--rw-r--r--   0        0        0     6306 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/ai_society.py
--rw-r--r--   0        0        0     8452 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/base.py
--rw-r--r--   0        0        0     5865 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/code.py
--rw-r--r--   0        0        0     1596 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/evaluation.py
--rw-r--r--   0        0        0     4537 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/misalignment.py
--rw-r--r--   0        0        0     1422 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/object_recognition.py
--rw-r--r--   0        0        0     4134 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/prompt_templates.py
--rw-r--r--   0        0        0     2544 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/role_description_prompt_template.py
--rw-r--r--   0        0        0     2109 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/solution_extraction.py
--rw-r--r--   0        0        0     2590 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/task_prompt_template.py
--rw-r--r--   0        0        0     1902 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/prompts/translation.py
--rw-r--r--   0        0        0      795 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/responses/__init__.py
--rw-r--r--   0        0        0     1714 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/responses/agent_responses.py
--rw-r--r--   0        0        0     1059 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/__init__.py
--rw-r--r--   0        0        0    13364 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/auto_retriever.py
--rw-r--r--   0        0        0     2624 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/base.py
--rw-r--r--   0        0        0     5180 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/bm25_retriever.py
--rw-r--r--   0        0        0     4123 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/cohere_rerank_retriever.py
--rw-r--r--   0        0        0     7185 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/retrievers/vector_retriever.py
--rw-r--r--   0        0        0      832 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/societies/__init__.py
--rw-r--r--   0        0        0    11770 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/societies/babyagi_playing.py
--rw-r--r--   0        0        0    22079 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/societies/role_playing.py
--rw-r--r--   0        0        0     1480 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/__init__.py
--rw-r--r--   0        0        0      897 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/graph_storages/__init__.py
--rw-r--r--   0        0        0     2857 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/graph_storages/base.py
--rw-r--r--   0        0        0     2356 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/graph_storages/graph_element.py
--rw-r--r--   0        0        0    22055 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/graph_storages/neo4j_graph.py
--rw-r--r--   0        0        0      916 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/key_value_storages/__init__.py
--rw-r--r--   0        0        0     2183 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/key_value_storages/base.py
--rw-r--r--   0        0        0     1955 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/key_value_storages/in_memory.py
--rw-r--r--   0        0        0     3471 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/key_value_storages/json.py
--rw-r--r--   0        0        0     1076 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/vectordb_storages/__init__.py
--rw-r--r--   0        0        0     6001 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/vectordb_storages/base.py
--rw-r--r--   0        0        0    13589 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/vectordb_storages/milvus.py
--rw-r--r--   0        0        0    13618 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/storages/vectordb_storages/qdrant.py
--rw-r--r--   0        0        0      997 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/terminators/__init__.py
--rw-r--r--   0        0        0     1396 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/terminators/base.py
--rw-r--r--   0        0        0     4951 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/terminators/response_terminator.py
--rw-r--r--   0        0        0     2087 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/terminators/token_limit_terminator.py
--rw-r--r--   0        0        0      836 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/toolkits/__init__.py
--rw-r--r--   0        0        0      923 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/toolkits/base.py
--rw-r--r--   0        0        0     8822 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/toolkits/github_toolkit.py
--rw-r--r--   0        0        0     1902 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/types/__init__.py
--rw-r--r--   0        0        0     8302 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/types/enums.py
--rw-r--r--   0        0        0     2045 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/types/openai_types.py
--rw-r--r--   0        0        0     1616 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/utils/__init__.py
--rw-r--r--   0        0        0     9930 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/utils/commons.py
--rw-r--r--   0        0        0    12674 2024-05-28 13:20:14.172937 camel_ai-0.1.5/camel/utils/token_counting.py
--rw-r--r--   0        0        0     6244 2024-05-28 13:20:14.184937 camel_ai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    21185 1970-01-01 00:00:00.000000 camel_ai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    17384 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/README.md
+-rw-r--r--   0        0        0      778 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/__init__.py
+-rw-r--r--   0        0        0     1494 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/base.py
+-rw-r--r--   0        0        0    21701 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/chat_agent.py
+-rw-r--r--   0        0        0     7377 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/critic_agent.py
+-rw-r--r--   0        0        0    13050 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/deductive_reasoner_agent.py
+-rw-r--r--   0        0        0     7322 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/embodied_agent.py
+-rw-r--r--   0        0        0     8783 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/knowledge_graph_agent.py
+-rw-r--r--   0        0        0     4879 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/role_assignment_agent.py
+-rw-r--r--   0        0        0    14907 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/task_agent.py
+-rw-r--r--   0        0        0      862 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/tool_agents/__init__.py
+-rw-r--r--   0        0        0     1399 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/tool_agents/base.py
+-rw-r--r--   0        0        0     8723 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/agents/tool_agents/hugging_face_tool_agent.py
+-rw-r--r--   0        0        0     1061 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/configs/__init__.py
+-rw-r--r--   0        0        0     3315 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/configs/anthropic_config.py
+-rw-r--r--   0        0        0      870 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/configs/base_config.py
+-rw-r--r--   0        0        0     6603 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/configs/openai_config.py
+-rw-r--r--   0        0        0      952 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/embeddings/__init__.py
+-rw-r--r--   0        0        0     2208 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/embeddings/base.py
+-rw-r--r--   0        0        0     2873 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/embeddings/openai_embedding.py
+-rw-r--r--   0        0        0     2312 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/embeddings/sentence_transformers_embeddings.py
+-rw-r--r--   0        0        0     1452 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/__init__.py
+-rw-r--r--   0        0        0    12468 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/google_maps_function.py
+-rw-r--r--   0        0        0     1703 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/math_functions.py
+-rw-r--r--   0        0        0    15036 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/open_api_function.py
+-rw-r--r--   0        0        0      708 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/open_api_specs/coursera/__init__.py
+-rw-r--r--   0        0        0     1981 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/open_api_specs/coursera/openapi.yaml
+-rw-r--r--   0        0        0      708 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/open_api_specs/klarna/__init__.py
+-rw-r--r--   0        0        0     2887 2024-05-29 17:22:05.866732 camel_ai-0.1.5.1/camel/functions/open_api_specs/klarna/openapi.yaml
+-rw-r--r--   0        0        0      708 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/open_api_specs/speak/__init__.py
+-rw-r--r--   0        0        0     6557 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/open_api_specs/speak/openapi.yaml
+-rw-r--r--   0        0        0    14933 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/openai_function.py
+-rw-r--r--   0        0        0     2281 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/retrieval_functions.py
+-rw-r--r--   0        0        0    12639 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/search_functions.py
+-rw-r--r--   0        0        0     8789 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/slack_functions.py
+-rw-r--r--   0        0        0    17254 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/twitter_function.py
+-rw-r--r--   0        0        0     5881 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/functions/weather_functions.py
+-rw-r--r--   0        0        0    10437 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/generators.py
+-rw-r--r--   0        0        0     4949 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/human.py
+-rw-r--r--   0        0        0     1040 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/interpreters/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/interpreters/base.py
+-rw-r--r--   0        0        0    21866 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/interpreters/internal_python_interpreter.py
+-rw-r--r--   0        0        0      886 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/interpreters/interpreter_error.py
+-rw-r--r--   0        0        0     6835 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/interpreters/subprocess_interpreter.py
+-rw-r--r--   0        0        0      856 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/loaders/__init__.py
+-rw-r--r--   0        0        0     8664 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/loaders/base_io.py
+-rw-r--r--   0        0        0    25870 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/loaders/unstructured_io.py
+-rw-r--r--   0        0        0     1364 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/__init__.py
+-rw-r--r--   0        0        0     6110 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/agent_memories.py
+-rw-r--r--   0        0        0     5003 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/base.py
+-rw-r--r--   0        0        0      860 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/blocks/__init__.py
+-rw-r--r--   0        0        0     4609 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/blocks/chat_history_block.py
+-rw-r--r--   0        0        0     3850 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/blocks/vectordb_block.py
+-rw-r--r--   0        0        0      806 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/context_creators/__init__.py
+-rw-r--r--   0        0        0     5378 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/context_creators/score_based.py
+-rw-r--r--   0        0        0     3618 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/memories/records.py
+-rw-r--r--   0        0        0     1468 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/messages/__init__.py
+-rw-r--r--   0        0        0    10131 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/messages/base.py
+-rw-r--r--   0        0        0     3841 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/messages/func_message.py
+-rw-r--r--   0        0        0     1168 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/__init__.py
+-rw-r--r--   0        0        0     5112 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/anthropic_model.py
+-rw-r--r--   0        0        0     3904 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/base_model.py
+-rw-r--r--   0        0        0     2418 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/model_factory.py
+-rw-r--r--   0        0        0     5856 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/open_source_model.py
+-rw-r--r--   0        0        0     9799 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/openai_audio_models.py
+-rw-r--r--   0        0        0     4164 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/openai_model.py
+-rw-r--r--   0        0        0     3631 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/models/stub_model.py
+-rw-r--r--   0        0        0     1790 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/__init__.py
+-rw-r--r--   0        0        0     6306 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/ai_society.py
+-rw-r--r--   0        0        0     8452 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/base.py
+-rw-r--r--   0        0        0     5865 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/code.py
+-rw-r--r--   0        0        0     1596 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/evaluation.py
+-rw-r--r--   0        0        0     4537 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/misalignment.py
+-rw-r--r--   0        0        0     1422 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/object_recognition.py
+-rw-r--r--   0        0        0     4134 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/prompt_templates.py
+-rw-r--r--   0        0        0     2544 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/role_description_prompt_template.py
+-rw-r--r--   0        0        0     2109 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/solution_extraction.py
+-rw-r--r--   0        0        0     2590 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/task_prompt_template.py
+-rw-r--r--   0        0        0     1902 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/prompts/translation.py
+-rw-r--r--   0        0        0      795 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/responses/__init__.py
+-rw-r--r--   0        0        0     1714 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/responses/agent_responses.py
+-rw-r--r--   0        0        0     1059 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/__init__.py
+-rw-r--r--   0        0        0    13364 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/auto_retriever.py
+-rw-r--r--   0        0        0     2624 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/base.py
+-rw-r--r--   0        0        0     5180 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/bm25_retriever.py
+-rw-r--r--   0        0        0     4123 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/cohere_rerank_retriever.py
+-rw-r--r--   0        0        0     7185 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/retrievers/vector_retriever.py
+-rw-r--r--   0        0        0      832 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/societies/__init__.py
+-rw-r--r--   0        0        0    11770 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/societies/babyagi_playing.py
+-rw-r--r--   0        0        0    22079 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/societies/role_playing.py
+-rw-r--r--   0        0        0     1480 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/storages/__init__.py
+-rw-r--r--   0        0        0      897 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/storages/graph_storages/__init__.py
+-rw-r--r--   0        0        0     2857 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/storages/graph_storages/base.py
+-rw-r--r--   0        0        0     2356 2024-05-29 17:22:05.870731 camel_ai-0.1.5.1/camel/storages/graph_storages/graph_element.py
+-rw-r--r--   0        0        0    22055 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/graph_storages/neo4j_graph.py
+-rw-r--r--   0        0        0      916 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/key_value_storages/__init__.py
+-rw-r--r--   0        0        0     2183 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/key_value_storages/base.py
+-rw-r--r--   0        0        0     1955 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/key_value_storages/in_memory.py
+-rw-r--r--   0        0        0     3471 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/key_value_storages/json.py
+-rw-r--r--   0        0        0     1076 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/vectordb_storages/__init__.py
+-rw-r--r--   0        0        0     6001 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/vectordb_storages/base.py
+-rw-r--r--   0        0        0    13589 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/vectordb_storages/milvus.py
+-rw-r--r--   0        0        0    13618 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/storages/vectordb_storages/qdrant.py
+-rw-r--r--   0        0        0      997 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/terminators/__init__.py
+-rw-r--r--   0        0        0     1396 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/terminators/base.py
+-rw-r--r--   0        0        0     4951 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/terminators/response_terminator.py
+-rw-r--r--   0        0        0     2087 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/terminators/token_limit_terminator.py
+-rw-r--r--   0        0        0      836 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/toolkits/__init__.py
+-rw-r--r--   0        0        0      923 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/toolkits/base.py
+-rw-r--r--   0        0        0     8822 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/toolkits/github_toolkit.py
+-rw-r--r--   0        0        0     1902 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/types/__init__.py
+-rw-r--r--   0        0        0     8302 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/types/enums.py
+-rw-r--r--   0        0        0     2045 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/types/openai_types.py
+-rw-r--r--   0        0        0     1616 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/utils/__init__.py
+-rw-r--r--   0        0        0     9930 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/utils/commons.py
+-rw-r--r--   0        0        0    12674 2024-05-29 17:22:05.874732 camel_ai-0.1.5.1/camel/utils/token_counting.py
+-rw-r--r--   0        0        0     6246 2024-05-29 17:22:05.886732 camel_ai-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0    21189 1970-01-01 00:00:00.000000 camel_ai-0.1.5.1/PKG-INFO
```

### Comparing `camel_ai-0.1.5/README.md` & `camel_ai-0.1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 # Create a conda virtual environment
 conda create --name camel python=3.10
 
 # Activate camel conda environment
 conda activate camel
 
 # Clone github repo
-git clone -b v0.1.5 https://github.com/camel-ai/camel.git
+git clone -b v0.1.5.1 https://github.com/camel-ai/camel.git
 
 # Change directory into project directory
 cd camel
 
 # Install camel from source
 pip install -e .
```

#### html2text {}

```diff
@@ -55,18 +55,18 @@
 github.com/camel-ai/camel.git # Change directory into project directory cd
 camel # Activate camel virtual environment poetry shell # Install camel from
 source # It takes about 90 seconds to resolve dependencies poetry install # Or
 if you want to use all other extra packages poetry install -E all # (Optional)
 # Exit the virtual environment exit ``` Install `CAMEL` from source with conda
 and pip: ```sh # Create a conda virtual environment conda create --name camel
 python=3.10 # Activate camel conda environment conda activate camel # Clone
-github repo git clone -b v0.1.5 https://github.com/camel-ai/camel.git # Change
-directory into project directory cd camel # Install camel from source pip
-install -e . # Or if you want to use all other extra packages pip install -e .
-[all] # (Optional) ``` ## Documentation [CAMEL package documentation pages]
+github repo git clone -b v0.1.5.1 https://github.com/camel-ai/camel.git #
+Change directory into project directory cd camel # Install camel from source
+pip install -e . # Or if you want to use all other extra packages pip install -
+e .[all] # (Optional) ``` ## Documentation [CAMEL package documentation pages]
 (https://camel-ai.github.io/camel/). ## Example You can find a list of tasks
 for different sets of assistant and user role pairs [here](https://
 drive.google.com/file/d/194PPaSTBR07m-PzjS-Ty6KlPLdFIPQDd/view?usp=share_link).
 As an example, to run the `role_playing.py` script: First, you need to add your
 OpenAI API key to system environment variables. The method to do this depends
 on your operating system and the shell you're using. **For Bash shell (Linux,
 macOS, Git Bash on Windows):** ```bash # Export your OpenAI API key export
```

### Comparing `camel_ai-0.1.5/camel/__init__.py` & `camel_ai-0.1.5.1/camel/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/__init__.py` & `camel_ai-0.1.5.1/camel/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/base.py` & `camel_ai-0.1.5.1/camel/agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/chat_agent.py` & `camel_ai-0.1.5.1/camel/agents/chat_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/critic_agent.py` & `camel_ai-0.1.5.1/camel/agents/critic_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/deductive_reasoner_agent.py` & `camel_ai-0.1.5.1/camel/agents/deductive_reasoner_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/embodied_agent.py` & `camel_ai-0.1.5.1/camel/agents/embodied_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/knowledge_graph_agent.py` & `camel_ai-0.1.5.1/camel/agents/knowledge_graph_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/role_assignment_agent.py` & `camel_ai-0.1.5.1/camel/agents/role_assignment_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/task_agent.py` & `camel_ai-0.1.5.1/camel/agents/task_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/tool_agents/__init__.py` & `camel_ai-0.1.5.1/camel/agents/tool_agents/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/tool_agents/base.py` & `camel_ai-0.1.5.1/camel/agents/tool_agents/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/agents/tool_agents/hugging_face_tool_agent.py` & `camel_ai-0.1.5.1/camel/agents/tool_agents/hugging_face_tool_agent.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/configs/__init__.py` & `camel_ai-0.1.5.1/camel/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/configs/anthropic_config.py` & `camel_ai-0.1.5.1/camel/configs/anthropic_config.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/configs/base_config.py` & `camel_ai-0.1.5.1/camel/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/configs/openai_config.py` & `camel_ai-0.1.5.1/camel/configs/openai_config.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/embeddings/__init__.py` & `camel_ai-0.1.5.1/camel/embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/embeddings/base.py` & `camel_ai-0.1.5.1/camel/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/embeddings/openai_embedding.py` & `camel_ai-0.1.5.1/camel/embeddings/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/embeddings/sentence_transformers_embeddings.py` & `camel_ai-0.1.5.1/camel/embeddings/sentence_transformers_embeddings.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/__init__.py` & `camel_ai-0.1.5.1/camel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/google_maps_function.py` & `camel_ai-0.1.5.1/camel/functions/google_maps_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/math_functions.py` & `camel_ai-0.1.5.1/camel/functions/math_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_function.py` & `camel_ai-0.1.5.1/camel/functions/open_api_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/coursera/__init__.py` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/coursera/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/coursera/openapi.yaml` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/coursera/openapi.yaml`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/klarna/__init__.py` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/klarna/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/klarna/openapi.yaml` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/klarna/openapi.yaml`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/speak/__init__.py` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/speak/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/open_api_specs/speak/openapi.yaml` & `camel_ai-0.1.5.1/camel/functions/open_api_specs/speak/openapi.yaml`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/openai_function.py` & `camel_ai-0.1.5.1/camel/functions/openai_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/retrieval_functions.py` & `camel_ai-0.1.5.1/camel/functions/retrieval_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/search_functions.py` & `camel_ai-0.1.5.1/camel/functions/search_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/slack_functions.py` & `camel_ai-0.1.5.1/camel/functions/slack_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/twitter_function.py` & `camel_ai-0.1.5.1/camel/functions/twitter_function.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/functions/weather_functions.py` & `camel_ai-0.1.5.1/camel/functions/weather_functions.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/generators.py` & `camel_ai-0.1.5.1/camel/generators.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/human.py` & `camel_ai-0.1.5.1/camel/human.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/interpreters/__init__.py` & `camel_ai-0.1.5.1/camel/interpreters/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/interpreters/base.py` & `camel_ai-0.1.5.1/camel/interpreters/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/interpreters/internal_python_interpreter.py` & `camel_ai-0.1.5.1/camel/interpreters/internal_python_interpreter.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/interpreters/interpreter_error.py` & `camel_ai-0.1.5.1/camel/interpreters/interpreter_error.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/interpreters/subprocess_interpreter.py` & `camel_ai-0.1.5.1/camel/interpreters/subprocess_interpreter.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/loaders/__init__.py` & `camel_ai-0.1.5.1/camel/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/loaders/base_io.py` & `camel_ai-0.1.5.1/camel/loaders/base_io.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/loaders/unstructured_io.py` & `camel_ai-0.1.5.1/camel/loaders/unstructured_io.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/__init__.py` & `camel_ai-0.1.5.1/camel/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/agent_memories.py` & `camel_ai-0.1.5.1/camel/memories/agent_memories.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/base.py` & `camel_ai-0.1.5.1/camel/memories/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/blocks/__init__.py` & `camel_ai-0.1.5.1/camel/memories/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/blocks/chat_history_block.py` & `camel_ai-0.1.5.1/camel/memories/blocks/chat_history_block.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/blocks/vectordb_block.py` & `camel_ai-0.1.5.1/camel/memories/blocks/vectordb_block.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/context_creators/__init__.py` & `camel_ai-0.1.5.1/camel/memories/context_creators/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/context_creators/score_based.py` & `camel_ai-0.1.5.1/camel/memories/context_creators/score_based.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/memories/records.py` & `camel_ai-0.1.5.1/camel/memories/records.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/messages/__init__.py` & `camel_ai-0.1.5.1/camel/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/messages/base.py` & `camel_ai-0.1.5.1/camel/messages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/messages/func_message.py` & `camel_ai-0.1.5.1/camel/messages/func_message.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/__init__.py` & `camel_ai-0.1.5.1/camel/models/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/anthropic_model.py` & `camel_ai-0.1.5.1/camel/models/anthropic_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/base_model.py` & `camel_ai-0.1.5.1/camel/models/base_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/model_factory.py` & `camel_ai-0.1.5.1/camel/models/model_factory.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/open_source_model.py` & `camel_ai-0.1.5.1/camel/models/open_source_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/openai_audio_models.py` & `camel_ai-0.1.5.1/camel/models/openai_audio_models.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/openai_model.py` & `camel_ai-0.1.5.1/camel/models/openai_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/models/stub_model.py` & `camel_ai-0.1.5.1/camel/models/stub_model.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/__init__.py` & `camel_ai-0.1.5.1/camel/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/ai_society.py` & `camel_ai-0.1.5.1/camel/prompts/ai_society.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/base.py` & `camel_ai-0.1.5.1/camel/prompts/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/code.py` & `camel_ai-0.1.5.1/camel/prompts/code.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/evaluation.py` & `camel_ai-0.1.5.1/camel/prompts/evaluation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/misalignment.py` & `camel_ai-0.1.5.1/camel/prompts/misalignment.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/object_recognition.py` & `camel_ai-0.1.5.1/camel/prompts/object_recognition.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/prompt_templates.py` & `camel_ai-0.1.5.1/camel/prompts/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/role_description_prompt_template.py` & `camel_ai-0.1.5.1/camel/prompts/role_description_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/solution_extraction.py` & `camel_ai-0.1.5.1/camel/prompts/solution_extraction.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/task_prompt_template.py` & `camel_ai-0.1.5.1/camel/prompts/task_prompt_template.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/prompts/translation.py` & `camel_ai-0.1.5.1/camel/prompts/translation.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/responses/__init__.py` & `camel_ai-0.1.5.1/camel/responses/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/responses/agent_responses.py` & `camel_ai-0.1.5.1/camel/responses/agent_responses.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/__init__.py` & `camel_ai-0.1.5.1/camel/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/auto_retriever.py` & `camel_ai-0.1.5.1/camel/retrievers/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/base.py` & `camel_ai-0.1.5.1/camel/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/bm25_retriever.py` & `camel_ai-0.1.5.1/camel/retrievers/bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/cohere_rerank_retriever.py` & `camel_ai-0.1.5.1/camel/retrievers/cohere_rerank_retriever.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/retrievers/vector_retriever.py` & `camel_ai-0.1.5.1/camel/retrievers/vector_retriever.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/societies/__init__.py` & `camel_ai-0.1.5.1/camel/societies/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/societies/babyagi_playing.py` & `camel_ai-0.1.5.1/camel/societies/babyagi_playing.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/societies/role_playing.py` & `camel_ai-0.1.5.1/camel/societies/role_playing.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/__init__.py` & `camel_ai-0.1.5.1/camel/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/graph_storages/__init__.py` & `camel_ai-0.1.5.1/camel/storages/graph_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/graph_storages/base.py` & `camel_ai-0.1.5.1/camel/storages/graph_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/graph_storages/graph_element.py` & `camel_ai-0.1.5.1/camel/storages/graph_storages/graph_element.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/graph_storages/neo4j_graph.py` & `camel_ai-0.1.5.1/camel/storages/graph_storages/neo4j_graph.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/key_value_storages/__init__.py` & `camel_ai-0.1.5.1/camel/storages/key_value_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/key_value_storages/base.py` & `camel_ai-0.1.5.1/camel/storages/key_value_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/key_value_storages/in_memory.py` & `camel_ai-0.1.5.1/camel/storages/key_value_storages/in_memory.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/key_value_storages/json.py` & `camel_ai-0.1.5.1/camel/storages/key_value_storages/json.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/vectordb_storages/__init__.py` & `camel_ai-0.1.5.1/camel/storages/vectordb_storages/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/vectordb_storages/base.py` & `camel_ai-0.1.5.1/camel/storages/vectordb_storages/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/vectordb_storages/milvus.py` & `camel_ai-0.1.5.1/camel/storages/vectordb_storages/milvus.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/storages/vectordb_storages/qdrant.py` & `camel_ai-0.1.5.1/camel/storages/vectordb_storages/qdrant.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/terminators/__init__.py` & `camel_ai-0.1.5.1/camel/terminators/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/terminators/base.py` & `camel_ai-0.1.5.1/camel/terminators/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/terminators/response_terminator.py` & `camel_ai-0.1.5.1/camel/terminators/response_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/terminators/token_limit_terminator.py` & `camel_ai-0.1.5.1/camel/terminators/token_limit_terminator.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/toolkits/__init__.py` & `camel_ai-0.1.5.1/camel/toolkits/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/toolkits/base.py` & `camel_ai-0.1.5.1/camel/toolkits/base.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/toolkits/github_toolkit.py` & `camel_ai-0.1.5.1/camel/toolkits/github_toolkit.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/types/__init__.py` & `camel_ai-0.1.5.1/camel/types/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/types/enums.py` & `camel_ai-0.1.5.1/camel/types/enums.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/types/openai_types.py` & `camel_ai-0.1.5.1/camel/types/openai_types.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/utils/__init__.py` & `camel_ai-0.1.5.1/camel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/utils/commons.py` & `camel_ai-0.1.5.1/camel/utils/commons.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/camel/utils/token_counting.py` & `camel_ai-0.1.5.1/camel/utils/token_counting.py`

 * *Files identical despite different names*

### Comparing `camel_ai-0.1.5/pyproject.toml` & `camel_ai-0.1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "camel-ai"
-version = "0.1.5"
+version = "0.1.5.1"
 authors = ["CAMEL-AI.org"]
 description = "Communicative Agents for AI Society Study"
 readme = "README.md"
 keywords = [
     "communicative-ai",
     "ai-societies",
     "artificial-intelligence",
```

### Comparing `camel_ai-0.1.5/PKG-INFO` & `camel_ai-0.1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camel-ai
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Communicative Agents for AI Society Study
 Home-page: https://www.camel-ai.org/
 License: Apache-2.0
 Keywords: communicative-ai,ai-societies,artificial-intelligence,deep-learning,multi-agent-systems,cooperative-ai,natural-language-processing,large-language-models
 Author: CAMEL-AI.org
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -166,15 +166,15 @@
 # Create a conda virtual environment
 conda create --name camel python=3.10
 
 # Activate camel conda environment
 conda activate camel
 
 # Clone github repo
-git clone -b v0.1.5 https://github.com/camel-ai/camel.git
+git clone -b v0.1.5.1 https://github.com/camel-ai/camel.git
 
 # Change directory into project directory
 cd camel
 
 # Install camel from source
 pip install -e .
```

