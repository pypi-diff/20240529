# Comparing `tmp/codefuse_muagent-0.0.3.tar.gz` & `tmp/codefuse_muagent-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefuse_muagent-0.0.3.tar", last modified: Tue Apr 23 09:35:24 2024, max compression
+gzip compressed data, was "codefuse_muagent-0.0.4.tar", last modified: Wed May 29 11:07:33 2024, max compression
```

## Comparing `codefuse_muagent-0.0.3.tar` & `codefuse_muagent-0.0.4.tar`

### file list

```diff
@@ -1,198 +1,197 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.375568 codefuse_muagent-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.370567 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/
--rw-rw-rw-   0        0        0      985 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6243 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-23 09:35:23.000000 codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11906 2024-03-12 06:09:58.000000 codefuse_muagent-0.0.3/LICENSE.md
--rw-rw-rw-   0        0        0      985 2024-04-23 09:35:24.371569 codefuse_muagent-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5358 2024-04-23 08:48:38.000000 codefuse_muagent-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.939085 codefuse_muagent-0.0.3/muagent/
--rw-rw-rw-   0        0        0       98 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.943085 codefuse_muagent-0.0.3/muagent/base_configs/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/base_configs/__init__.py
--rw-rw-rw-   0        0        0     3547 2024-03-12 11:06:58.000000 codefuse_muagent-0.0.3/muagent/base_configs/env_config.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.972071 codefuse_muagent-0.0.3/muagent/chat/
--rw-rw-rw-   0        0        0      296 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/chat/__init__.py
--rw-rw-rw-   0        0        0    18098 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/chat/agent_chat.py
--rw-rw-rw-   0        0        0     8574 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/base_chat.py
--rw-rw-rw-   0        0        0     7571 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/code_chat.py
--rw-rw-rw-   0        0        0     4080 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/knowledge_chat.py
--rw-rw-rw-   0        0        0     1544 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/llm_chat.py
--rw-rw-rw-   0        0        0     5651 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/chat/search_chat.py
--rw-rw-rw-   0        0        0      803 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/chat/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.975073 codefuse_muagent-0.0.3/muagent/codechat/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.991100 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/__init__.py
--rw-rw-rw-   0        0        0     9385 2024-04-10 08:41:08.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_analyzer.py
--rw-rw-rw-   0        0        0      565 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_dedup.py
--rw-rw-rw-   0        0        0     9246 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_intepreter.py
--rw-rw-rw-   0        0        0      228 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_preprocess.py
--rw-rw-rw-   0        0        0      633 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_static_analysis.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:23.995107 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/
--rw-rw-rw-   0        0        0      198 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/__init__.py
--rw-rw-rw-   0        0        0     3783 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.002072 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/
--rw-rw-rw-   0        0        0      227 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/__init__.py
--rw-rw-rw-   0        0        0     1139 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/dir_crawler.py
--rw-rw-rw-   0        0        0      682 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/codechat/code_crawler/zip_crawler.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.012071 codefuse_muagent-0.0.3/muagent/codechat/code_search/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/__init__.py
--rw-rw-rw-   0        0        0     9179 2024-04-10 09:14:02.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/code_search.py
--rw-rw-rw-   0        0        0     2815 2024-04-10 09:06:40.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/cypher_generator.py
--rw-rw-rw-   0        0        0      776 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/code_search/tagger.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.019072 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/__init__.py
--rw-rw-rw-   0        0        0    18942 2024-04-10 08:40:23.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/code_importer.py
--rw-rw-rw-   0        0        0    10625 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/codebase_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.029070 codefuse_muagent-0.0.3/muagent/connector/
--rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.034071 codefuse_muagent-0.0.3/muagent/connector/actions/
--rw-rw-rw-   0        0        0       73 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/actions/__init__.py
--rw-rw-rw-   0        0        0      207 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/actions/base_action.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.046073 codefuse_muagent-0.0.3/muagent/connector/agents/
--rw-rw-rw-   0        0        0      239 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/agents/__init__.py
--rw-rw-rw-   0        0        0    10500 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/base_agent.py
--rw-rw-rw-   0        0        0     8801 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/executor_agent.py
--rw-rw-rw-   0        0        0     7995 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/react_agent.py
--rw-rw-rw-   0        0        0     6041 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/agents/selector_agent.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.051072 codefuse_muagent-0.0.3/muagent/connector/antflow/
--rw-rw-rw-   0        0        0      114 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/antflow/__init__.py
--rw-rw-rw-   0        0        0    11507 2024-04-18 08:41:54.000000 codefuse_muagent-0.0.3/muagent/connector/antflow/flow.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.058071 codefuse_muagent-0.0.3/muagent/connector/chains/
--rw-rw-rw-   0        0        0       68 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/chains/__init__.py
--rw-rw-rw-   0        0        0     6960 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/chains/base_chain.py
--rw-rw-rw-   0        0        0      318 2024-03-13 06:55:36.000000 codefuse_muagent-0.0.3/muagent/connector/chains/chains.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.070113 codefuse_muagent-0.0.3/muagent/connector/configs/
--rw-rw-rw-   0        0        0      434 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/__init__.py
--rw-rw-rw-   0        0        0    10397 2024-03-26 07:36:32.000000 codefuse_muagent-0.0.3/muagent/connector/configs/agent_config.py
--rw-rw-rw-   0        0        0     4104 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/chain_config.py
--rw-rw-rw-   0        0        0     2274 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/phase_config.py
--rw-rw-rw-   0        0        0     5838 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompt_config.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.127104 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/
--rw-rw-rw-   0        0        0     2724 2024-03-19 12:49:14.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/__init__.py
--rw-rw-rw-   0        0        0      829 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/agent_selector_template_prompt.py
--rw-rw-rw-   0        0        0     1928 2024-03-25 09:34:34.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/checker_template_prompt.py
--rw-rw-rw-   0        0        0     3666 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2doc_template_prompt.py
--rw-rw-rw-   0        0        0     3928 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2test_template_prompt.py
--rw-rw-rw-   0        0        0     2246 2024-03-26 04:35:55.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/executor_template_prompt.py
--rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/input_template_prompt.py
--rw-rw-rw-   0        0        0     1409 2024-03-27 08:29:05.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/intention_template_prompt.py
--rw-rw-rw-   0        0        0     7360 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/metagpt_prompt.py
--rw-rw-rw-   0        0        0     4421 2024-03-20 06:14:22.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/planner_template_prompt.py
--rw-rw-rw-   0        0        0     3032 2024-04-10 09:00:47.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/qa_template_prompt.py
--rw-rw-rw-   0        0        0     3872 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_code_prompt.py
--rw-rw-rw-   0        0        0     1639 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_template_prompt.py
--rw-rw-rw-   0        0        0     1860 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py
--rw-rw-rw-   0        0        0     8551 2024-03-25 09:34:43.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_prompt.py
--rw-rw-rw-   0        0        0     2599 2024-03-26 02:46:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_prompt.py
--rw-rw-rw-   0        0        0     1487 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/refine_template_prompt.py
--rw-rw-rw-   0        0        0     2076 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/configs/prompts/summary_template_prompt.py
--rw-rw-rw-   0        0        0    37315 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/memory_manager.py
--rw-rw-rw-   0        0        0    14713 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/message_process.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.132071 codefuse_muagent-0.0.3/muagent/connector/phase/
--rw-rw-rw-   0        0        0       60 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/phase/__init__.py
--rw-rw-rw-   0        0        0    14557 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/phase/base_phase.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.139071 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/
--rw-rw-rw-   0        0        0       72 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/__init__.py
--rw-rw-rw-   0        0        0     2362 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/extend_manager.py
--rw-rw-rw-   0        0        0    28367 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/prompt_manager/prompt_manager.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.149072 codefuse_muagent-0.0.3/muagent/connector/schema/
--rw-rw-rw-   0        0        0      325 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/connector/schema/__init__.py
--rw-rw-rw-   0        0        0     9517 2024-03-26 07:37:47.000000 codefuse_muagent-0.0.3/muagent/connector/schema/general_schema.py
--rw-rw-rw-   0        0        0     7217 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/schema/memory.py
--rw-rw-rw-   0        0        0     5953 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/connector/schema/message.py
--rw-rw-rw-   0        0        0     5529 2024-03-27 08:28:21.000000 codefuse_muagent-0.0.3/muagent/connector/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.152071 codefuse_muagent-0.0.3/muagent/db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.156071 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/__init__.py
--rw-rw-rw-   0        0        0     8783 2024-04-10 09:06:46.000000 codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/nebula_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.162071 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/
--rw-rw-rw-   0        0        0       99 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/__init__.py
--rw-rw-rw-   0        0        0     4947 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/chroma_handler.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.188071 codefuse_muagent-0.0.3/muagent/embeddings/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.193072 codefuse_muagent-0.0.3/muagent/embeddings/commands/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/commands/__init__.py
--rw-rw-rw-   0        0        0      665 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/commands/default_vs_cds.py
--rw-rw-rw-   0        0        0    29854 2024-03-19 03:31:15.000000 codefuse_muagent-0.0.3/muagent/embeddings/faiss_m.py
--rw-rw-rw-   0        0        0     5515 2024-04-18 07:53:55.000000 codefuse_muagent-0.0.3/muagent/embeddings/get_embedding.py
--rw-rw-rw-   0        0        0     5499 2024-04-10 08:42:59.000000 codefuse_muagent-0.0.3/muagent/embeddings/huggingface_embedding.py
--rw-rw-rw-   0        0        0     1651 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/in_memory.py
--rw-rw-rw-   0        0        0     5406 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/openai_embedding.py
--rw-rw-rw-   0        0        0      851 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/embeddings/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.200070 codefuse_muagent-0.0.3/muagent/llm_models/
--rw-rw-rw-   0        0        0      211 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/llm_models/__init__.py
--rw-rw-rw-   0        0        0     1936 2024-03-29 02:51:52.000000 codefuse_muagent-0.0.3/muagent/llm_models/llm_config.py
--rw-rw-rw-   0        0        0     3048 2024-03-22 07:50:16.000000 codefuse_muagent-0.0.3/muagent/llm_models/openai_model.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.208071 codefuse_muagent-0.0.3/muagent/orm/
--rw-rw-rw-   0        0        0      573 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.217071 codefuse_muagent-0.0.3/muagent/orm/commands/
--rw-rw-rw-   0        0        0      452 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/commands/__init__.py
--rw-rw-rw-   0        0        0     2426 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/code_base_cds.py
--rw-rw-rw-   0        0        0     2793 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/document_base_cds.py
--rw-rw-rw-   0        0        0     3157 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/commands/document_file_cds.py
--rw-rw-rw-   0        0        0     1387 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/db.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.222073 codefuse_muagent-0.0.3/muagent/orm/schemas/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/orm/schemas/__init__.py
--rw-rw-rw-   0        0        0     2901 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/schemas/base_schema.py
--rw-rw-rw-   0        0        0      910 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/orm/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.227072 codefuse_muagent-0.0.3/muagent/retrieval/
--rw-rw-rw-   0        0        0      139 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/__init__.py
--rw-rw-rw-   0        0        0     2519 2024-03-21 04:10:28.000000 codefuse_muagent-0.0.3/muagent/retrieval/base_retrieval.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.235071 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/
--rw-rw-rw-   0        0        0      120 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/__init__.py
--rw-rw-rw-   0        0        0     2117 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/json_loader.py
--rw-rw-rw-   0        0        0     2121 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/jsonl_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.243070 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/
--rw-rw-rw-   0        0        0       76 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/__init__.py
--rw-rw-rw-   0        0        0     2837 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/langchain_splitter.py
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.249070 codefuse_muagent-0.0.3/muagent/sandbox/
--rw-rw-rw-   0        0        0      119 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/sandbox/__init__.py
--rw-rw-rw-   0        0        0     3772 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/sandbox/basebox.py
--rw-rw-rw-   0        0        0    20458 2024-04-11 11:32:17.000000 codefuse_muagent-0.0.3/muagent/sandbox/pycodebox.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.276082 codefuse_muagent-0.0.3/muagent/service/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/service/__init__.py
--rw-rw-rw-   0        0        0     5851 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/service/base_service.py
--rw-rw-rw-   0        0        0    10063 2024-04-07 03:54:58.000000 codefuse_muagent-0.0.3/muagent/service/cb_api.py
--rw-rw-rw-   0        0        0     6887 2024-04-10 09:08:37.000000 codefuse_muagent-0.0.3/muagent/service/faiss_db_service.py
--rw-rw-rw-   0        0        0    16377 2024-03-19 05:49:11.000000 codefuse_muagent-0.0.3/muagent/service/kb_api.py
--rw-rw-rw-   0        0        0     5742 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/service/migrate.py
--rw-rw-rw-   0        0        0     5096 2024-03-19 03:31:20.000000 codefuse_muagent-0.0.3/muagent/service/service_factory.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.313567 codefuse_muagent-0.0.3/muagent/tools/
--rw-rw-rw-   0        0        0     1108 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/__init__.py
--rw-rw-rw-   0        0        0     1551 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/abnormal_detection.py
--rw-rw-rw-   0        0        0     2332 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/base_tool.py
--rw-rw-rw-   0        0        0     2577 2024-04-10 08:46:41.000000 codefuse_muagent-0.0.3/muagent/tools/cb_query_tool.py
--rw-rw-rw-   0        0        0     4355 2024-03-27 08:14:38.000000 codefuse_muagent-0.0.3/muagent/tools/codechat_tools.py
--rw-rw-rw-   0        0        0     2070 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/tools/docs_retrieval.py
--rw-rw-rw-   0        0        0     2882 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/duckduckgo_search.py
--rw-rw-rw-   0        0        0     1110 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/metrics_query.py
--rw-rw-rw-   0        0        0     1146 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/multiplier.py
--rw-rw-rw-   0        0        0     4491 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/ocr_tool.py
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/sandbox.py
--rw-rw-rw-   0        0        0     8334 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/tools/stock_tool.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.318567 codefuse_muagent-0.0.3/muagent/tools/tool_datas/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/tool_datas/__init__.py
--rw-rw-rw-   0        0        0   247049 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/tool_datas/stock_data.py
--rw-rw-rw-   0        0        0     4398 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/weather.py
--rw-rw-rw-   0        0        0     7788 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/tools/world_time.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.361568 codefuse_muagent-0.0.3/muagent/utils/
--rw-rw-rw-   0        0        0      209 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/__init__.py
--rw-rw-rw-   0        0        0     2804 2024-04-07 04:53:53.000000 codefuse_muagent-0.0.3/muagent/utils/code2doc_util.py
--rw-rw-rw-   0        0        0     3406 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/utils/common_utils.py
--rw-rw-rw-   0        0        0     2698 2024-03-13 06:55:37.000000 codefuse_muagent-0.0.3/muagent/utils/path_utils.py
--rw-rw-rw-   0        0        0      188 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/postprocess.py
--rw-rw-rw-   0        0        0     7522 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/server_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.363568 codefuse_muagent-0.0.3/muagent/utils/static/
--rw-rw-rw-   0        0        0        0 2024-03-12 07:44:01.000000 codefuse_muagent-0.0.3/muagent/utils/static/__init__.py
--rw-rw-rw-   0        0        0     5107 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/muagent/utils/tbase_util.py
--rw-rw-rw-   0        0        0       42 2024-04-23 09:35:24.375568 codefuse_muagent-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1194 2024-04-23 09:11:12.000000 codefuse_muagent-0.0.3/setup.py
--rw-rw-rw-   0        0        0     1203 2024-04-23 09:33:59.000000 codefuse_muagent-0.0.3/setup_test.py
-drwxrwxrwx   0        0        0        0 2024-04-23 09:35:24.366567 codefuse_muagent-0.0.3/tests/
--rw-rw-rw-   0        0        0     1720 2024-03-26 02:49:26.000000 codefuse_muagent-0.0.3/tests/test_config.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/
+-rw-rw-rw-   0        0        0    11906 2024-04-23 09:12:53.000000 codefuse_muagent-0.0.4/LICENSE.md
+-rw-rw-rw-   0        0        0      985 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5346 2024-05-29 11:01:29.000000 codefuse_muagent-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/
+-rw-rw-rw-   0        0        0      985 2024-05-29 11:07:31.000000 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6030 2024-05-29 11:07:32.000000 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:07:31.000000 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      213 2024-05-29 11:07:31.000000 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 11:07:31.000000 codefuse_muagent-0.0.4/codefuse_muagent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.509706 codefuse_muagent-0.0.4/muagent/
+-rw-rw-rw-   0        0        0       98 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.515705 codefuse_muagent-0.0.4/muagent/base_configs/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/base_configs/__init__.py
+-rw-rw-rw-   0        0        0     3547 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/base_configs/env_config.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.543661 codefuse_muagent-0.0.4/muagent/chat/
+-rw-rw-rw-   0        0        0      296 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/__init__.py
+-rw-rw-rw-   0        0        0    18350 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/agent_chat.py
+-rw-rw-rw-   0        0        0     8574 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/base_chat.py
+-rw-rw-rw-   0        0        0     7805 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/code_chat.py
+-rw-rw-rw-   0        0        0     4080 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/knowledge_chat.py
+-rw-rw-rw-   0        0        0     1544 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/llm_chat.py
+-rw-rw-rw-   0        0        0     5651 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/search_chat.py
+-rw-rw-rw-   0        0        0      803 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/chat/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.543661 codefuse_muagent-0.0.4/muagent/codechat/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.559289 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/__init__.py
+-rw-rw-rw-   0        0        0     9385 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_analyzer.py
+-rw-rw-rw-   0        0        0      565 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_dedup.py
+-rw-rw-rw-   0        0        0     9306 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_intepreter.py
+-rw-rw-rw-   0        0        0      228 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_preprocess.py
+-rw-rw-rw-   0        0        0      633 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_static_analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.574914 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/language_static_analysis/
+-rw-rw-rw-   0        0        0      198 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/language_static_analysis/__init__.py
+-rw-rw-rw-   0        0        0     3783 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.574914 codefuse_muagent-0.0.4/muagent/codechat/code_crawler/
+-rw-rw-rw-   0        0        0      227 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_crawler/__init__.py
+-rw-rw-rw-   0        0        0     1139 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_crawler/dir_crawler.py
+-rw-rw-rw-   0        0        0      682 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_crawler/zip_crawler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.590540 codefuse_muagent-0.0.4/muagent/codechat/code_search/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_search/__init__.py
+-rw-rw-rw-   0        0        0     9179 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_search/code_search.py
+-rw-rw-rw-   0        0        0     2815 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_search/cypher_generator.py
+-rw-rw-rw-   0        0        0      776 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/code_search/tagger.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.606191 codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/__init__.py
+-rw-rw-rw-   0        0        0    18942 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/code_importer.py
+-rw-rw-rw-   0        0        0    10625 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/codebase_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.606191 codefuse_muagent-0.0.4/muagent/connector/
+-rw-rw-rw-   0        0        0      120 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.621788 codefuse_muagent-0.0.4/muagent/connector/actions/
+-rw-rw-rw-   0        0        0       73 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/actions/__init__.py
+-rw-rw-rw-   0        0        0      207 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/actions/base_action.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.637413 codefuse_muagent-0.0.4/muagent/connector/agents/
+-rw-rw-rw-   0        0        0      239 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/agents/__init__.py
+-rw-rw-rw-   0        0        0    10500 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/agents/base_agent.py
+-rw-rw-rw-   0        0        0     8801 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/agents/executor_agent.py
+-rw-rw-rw-   0        0        0     7995 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/agents/react_agent.py
+-rw-rw-rw-   0        0        0     6041 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/agents/selector_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.637413 codefuse_muagent-0.0.4/muagent/connector/antflow/
+-rw-rw-rw-   0        0        0      114 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/antflow/__init__.py
+-rw-rw-rw-   0        0        0    11507 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/antflow/flow.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.657303 codefuse_muagent-0.0.4/muagent/connector/chains/
+-rw-rw-rw-   0        0        0       68 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/chains/__init__.py
+-rw-rw-rw-   0        0        0     6960 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/chains/base_chain.py
+-rw-rw-rw-   0        0        0      318 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/chains/chains.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.674566 codefuse_muagent-0.0.4/muagent/connector/configs/
+-rw-rw-rw-   0        0        0      434 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/__init__.py
+-rw-rw-rw-   0        0        0    10397 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/agent_config.py
+-rw-rw-rw-   0        0        0     4104 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/chain_config.py
+-rw-rw-rw-   0        0        0     2274 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/phase_config.py
+-rw-rw-rw-   0        0        0     5838 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompt_config.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.743178 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/
+-rw-rw-rw-   0        0        0     2724 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/__init__.py
+-rw-rw-rw-   0        0        0      829 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/agent_selector_template_prompt.py
+-rw-rw-rw-   0        0        0     1928 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/checker_template_prompt.py
+-rw-rw-rw-   0        0        0     3666 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/code2doc_template_prompt.py
+-rw-rw-rw-   0        0        0     3928 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/code2test_template_prompt.py
+-rw-rw-rw-   0        0        0     2246 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/executor_template_prompt.py
+-rw-rw-rw-   0        0        0      665 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/input_template_prompt.py
+-rw-rw-rw-   0        0        0     1409 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/intention_template_prompt.py
+-rw-rw-rw-   0        0        0     7360 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/metagpt_prompt.py
+-rw-rw-rw-   0        0        0     4421 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/planner_template_prompt.py
+-rw-rw-rw-   0        0        0     3032 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/qa_template_prompt.py
+-rw-rw-rw-   0        0        0     3872 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_code_prompt.py
+-rw-rw-rw-   0        0        0     1639 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_template_prompt.py
+-rw-rw-rw-   0        0        0     1860 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py
+-rw-rw-rw-   0        0        0     8551 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_code_prompt.py
+-rw-rw-rw-   0        0        0     2599 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_prompt.py
+-rw-rw-rw-   0        0        0     1487 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/refine_template_prompt.py
+-rw-rw-rw-   0        0        0     2076 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/configs/prompts/summary_template_prompt.py
+-rw-rw-rw-   0        0        0    37614 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/memory_manager.py
+-rw-rw-rw-   0        0        0    14713 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/message_process.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.743178 codefuse_muagent-0.0.4/muagent/connector/phase/
+-rw-rw-rw-   0        0        0       60 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/phase/__init__.py
+-rw-rw-rw-   0        0        0    14557 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/phase/base_phase.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.758804 codefuse_muagent-0.0.4/muagent/connector/prompt_manager/
+-rw-rw-rw-   0        0        0       72 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/prompt_manager/__init__.py
+-rw-rw-rw-   0        0        0     2362 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/prompt_manager/extend_manager.py
+-rw-rw-rw-   0        0        0    28367 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/prompt_manager/prompt_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.773104 codefuse_muagent-0.0.4/muagent/connector/schema/
+-rw-rw-rw-   0        0        0      325 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/schema/__init__.py
+-rw-rw-rw-   0        0        0     9517 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/schema/general_schema.py
+-rw-rw-rw-   0        0        0     7217 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/schema/memory.py
+-rw-rw-rw-   0        0        0     5953 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/connector/schema/message.py
+-rw-rw-rw-   0        0        0     5529 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/connector/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.776607 codefuse_muagent-0.0.4/muagent/db_handler/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/db_handler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.781843 codefuse_muagent-0.0.4/muagent/db_handler/graph_db_handler/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/db_handler/graph_db_handler/__init__.py
+-rw-rw-rw-   0        0        0     8783 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/db_handler/graph_db_handler/nebula_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.788842 codefuse_muagent-0.0.4/muagent/db_handler/vector_db_handler/
+-rw-rw-rw-   0        0        0       99 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/db_handler/vector_db_handler/__init__.py
+-rw-rw-rw-   0        0        0     4947 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/db_handler/vector_db_handler/chroma_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.819304 codefuse_muagent-0.0.4/muagent/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.823304 codefuse_muagent-0.0.4/muagent/embeddings/commands/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/commands/__init__.py
+-rw-rw-rw-   0        0        0      665 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/commands/default_vs_cds.py
+-rw-rw-rw-   0        0        0    29854 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/faiss_m.py
+-rw-rw-rw-   0        0        0     5515 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/get_embedding.py
+-rw-rw-rw-   0        0        0     5499 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/huggingface_embedding.py
+-rw-rw-rw-   0        0        0     1651 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/in_memory.py
+-rw-rw-rw-   0        0        0     5406 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/openai_embedding.py
+-rw-rw-rw-   0        0        0      851 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/embeddings/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.833883 codefuse_muagent-0.0.4/muagent/llm_models/
+-rw-rw-rw-   0        0        0      211 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/llm_models/__init__.py
+-rw-rw-rw-   0        0        0     1936 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/llm_models/llm_config.py
+-rw-rw-rw-   0        0        0     3048 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/llm_models/openai_model.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.841883 codefuse_muagent-0.0.4/muagent/orm/
+-rw-rw-rw-   0        0        0      573 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.843202 codefuse_muagent-0.0.4/muagent/orm/commands/
+-rw-rw-rw-   0        0        0      452 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/commands/__init__.py
+-rw-rw-rw-   0        0        0     2426 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/commands/code_base_cds.py
+-rw-rw-rw-   0        0        0     2793 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/commands/document_base_cds.py
+-rw-rw-rw-   0        0        0     3157 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/commands/document_file_cds.py
+-rw-rw-rw-   0        0        0     1387 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/db.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.858828 codefuse_muagent-0.0.4/muagent/orm/schemas/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2901 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/schemas/base_schema.py
+-rw-rw-rw-   0        0        0      910 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/orm/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.865180 codefuse_muagent-0.0.4/muagent/retrieval/
+-rw-rw-rw-   0        0        0      139 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/__init__.py
+-rw-rw-rw-   0        0        0     2519 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/base_retrieval.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.872180 codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/
+-rw-rw-rw-   0        0        0      120 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/__init__.py
+-rw-rw-rw-   0        0        0     2117 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/json_loader.py
+-rw-rw-rw-   0        0        0     2121 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/jsonl_loader.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.880976 codefuse_muagent-0.0.4/muagent/retrieval/text_splitter/
+-rw-rw-rw-   0        0        0       76 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/text_splitter/__init__.py
+-rw-rw-rw-   0        0        0     2837 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/text_splitter/langchain_splitter.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:18.000000 codefuse_muagent-0.0.4/muagent/retrieval/text_splitter/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.888975 codefuse_muagent-0.0.4/muagent/sandbox/
+-rw-rw-rw-   0        0        0      119 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/sandbox/__init__.py
+-rw-rw-rw-   0        0        0     3772 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/sandbox/basebox.py
+-rw-rw-rw-   0        0        0    20458 2024-05-29 11:00:16.000000 codefuse_muagent-0.0.4/muagent/sandbox/pycodebox.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.923226 codefuse_muagent-0.0.4/muagent/service/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/__init__.py
+-rw-rw-rw-   0        0        0     5851 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/base_service.py
+-rw-rw-rw-   0        0        0    10225 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/cb_api.py
+-rw-rw-rw-   0        0        0     6887 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/faiss_db_service.py
+-rw-rw-rw-   0        0        0    16377 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/kb_api.py
+-rw-rw-rw-   0        0        0     5742 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/migrate.py
+-rw-rw-rw-   0        0        0     5096 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/service/service_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.963313 codefuse_muagent-0.0.4/muagent/tools/
+-rw-rw-rw-   0        0        0     1108 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/abnormal_detection.py
+-rw-rw-rw-   0        0        0     2332 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/base_tool.py
+-rw-rw-rw-   0        0        0     2577 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/cb_query_tool.py
+-rw-rw-rw-   0        0        0     4355 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/codechat_tools.py
+-rw-rw-rw-   0        0        0     2070 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/docs_retrieval.py
+-rw-rw-rw-   0        0        0     2882 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/duckduckgo_search.py
+-rw-rw-rw-   0        0        0     1110 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/metrics_query.py
+-rw-rw-rw-   0        0        0     1146 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/multiplier.py
+-rw-rw-rw-   0        0        0     4491 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/ocr_tool.py
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/sandbox.py
+-rw-rw-rw-   0        0        0     8334 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/stock_tool.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.969313 codefuse_muagent-0.0.4/muagent/tools/tool_datas/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/tool_datas/__init__.py
+-rw-rw-rw-   0        0        0   247049 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/tool_datas/stock_data.py
+-rw-rw-rw-   0        0        0     4398 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/weather.py
+-rw-rw-rw-   0        0        0     7788 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/tools/world_time.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.991934 codefuse_muagent-0.0.4/muagent/utils/
+-rw-rw-rw-   0        0        0      209 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/__init__.py
+-rw-rw-rw-   0        0        0     2804 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/code2doc_util.py
+-rw-rw-rw-   0        0        0     3406 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/common_utils.py
+-rw-rw-rw-   0        0        0     2698 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/path_utils.py
+-rw-rw-rw-   0        0        0      188 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/postprocess.py
+-rw-rw-rw-   0        0        0     7522 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/server_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/muagent/utils/static/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/static/__init__.py
+-rw-rw-rw-   0        0        0     5107 2024-05-29 11:00:17.000000 codefuse_muagent-0.0.4/muagent/utils/tbase_util.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2024-05-29 11:01:08.000000 codefuse_muagent-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:07:32.993394 codefuse_muagent-0.0.4/tests/
+-rw-rw-rw-   0        0        0     1720 2024-05-29 11:00:19.000000 codefuse_muagent-0.0.4/tests/test_config.py
```

### Comparing `codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/PKG-INFO` & `codefuse_muagent-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefuse-muagent
-Version: 0.0.3
+Version: 0.0.4
 Summary: A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.
 Home-page: https://github.com/codefuse-ai/CodeFuse-muAgent
 Author: shanshi
 Author-email: wyp311395@antgroup.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `codefuse_muagent-0.0.3/CodeFuse_muAgent.egg-info/SOURCES.txt` & `codefuse_muagent-0.0.4/codefuse_muagent.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 LICENSE.md
 README.md
 setup.py
-setup_test.py
-CodeFuse_muAgent.egg-info/PKG-INFO
-CodeFuse_muAgent.egg-info/SOURCES.txt
-CodeFuse_muAgent.egg-info/dependency_links.txt
-CodeFuse_muAgent.egg-info/requires.txt
-CodeFuse_muAgent.egg-info/top_level.txt
 codefuse_muagent.egg-info/PKG-INFO
 codefuse_muagent.egg-info/SOURCES.txt
 codefuse_muagent.egg-info/dependency_links.txt
 codefuse_muagent.egg-info/requires.txt
 codefuse_muagent.egg-info/top_level.txt
 muagent/__init__.py
 muagent/base_configs/__init__.py
```

### Comparing `codefuse_muagent-0.0.3/LICENSE.md` & `codefuse_muagent-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/PKG-INFO` & `codefuse_muagent-0.0.4/codefuse_muagent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefuse-muagent
-Version: 0.0.3
+Version: 0.0.4
 Summary: A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.
 Home-page: https://github.com/codefuse-ai/CodeFuse-muAgent
 Author: shanshi
 Author-email: wyp311395@antgroup.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `codefuse_muagent-0.0.3/README.md` & `codefuse_muagent-0.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,20 +99,20 @@
     )
 output_message3, output_memory3 = phase.step(query)
 print(output_memory3.to_str_messages(return_all=True, content_key="parsed_output_list"))
 ```
 
 ## Key Technologies
 
-● Agent Base：Four fundamental Agent types are constructed – BaseAgent, ReactAgent, ExecutorAgent, SelectorAgent, supporting basic activities across various scenarios 
-● Communication: Information transmission between Agents is accomplished through Message and Parse Message entities, interacting with Memory Manager and managing memories in the Memory Pool 
-● Prompt Manager: Customized Agent Prompts are automatically assembled with the aid of Role Handler, Doc/Tool Handler, Session Handler, and Customized Handler 
-● Memory Manager: Facilitates the management of chat history storage, information compression, and memory retrieval, culminating in storage within databases, local systems, and vector databases via the Memory Pool 
-● Component: Auxiliary ecosystem components to construct Agents, including Retrieval, Tool, Action, Sandbox, etc. 
-● Customized Model: Supports the integration of private LLM and Embedding models
+- Agent Base：Four fundamental Agent types are constructed – BaseAgent, ReactAgent, ExecutorAgent, SelectorAgent, supporting basic activities across various scenarios 
+- Communication: Information transmission between Agents is accomplished through Message and Parse Message entities, interacting with Memory Manager and managing memories in the Memory Pool 
+- Prompt Manager: Customized Agent Prompts are automatically assembled with the aid of Role Handler, Doc/Tool Handler, Session Handler, and Customized Handler 
+- Memory Manager: Facilitates the management of chat history storage, information compression, and memory retrieval, culminating in storage within databases, local systems, and vector databases via the Memory Pool 
+- Component: Auxiliary ecosystem components to construct Agents, including Retrieval, Tool, Action, Sandbox, etc. 
+- Customized Model: Supports the integration of private LLM and Embedding models
 
 ##  Contribution
 We are deeply grateful for your interest in the Codefuse project and warmly welcome any suggestions, opinions (including criticism), comments, and contributions. 
 
 Feel free to raise your suggestions, opinions, and comments directly through GitHub Issues. There are numerous ways to participate in and contribute to the Codefuse project: code implementation, writing tests, process tool improvements, documentation enhancements, etc. 
 
 We welcome any contribution and will add you to the list of contributors. See [Contribution Guide...](docs/contribution/contribute_guide.md)
```

#### html2text {}

```diff
@@ -38,30 +38,30 @@
 ( phase_name, embed_config=embed_config, llm_config=llm_config, ) #
 query_content = "what does the remove' function?" query = Message
 ( role_name="user", role_type="human", input_query=query_content,
 code_engine_name=codebase_name, score_threshold=1.0, top_k=3,
 cb_search_type="tag", local_graph_path=CB_ROOT_PATH, use_nh=False )
 output_message3, output_memory3 = phase.step(query) print
 (output_memory3.to_str_messages(return_all=True,
-content_key="parsed_output_list")) ``` ## Key Technologies â Agent
-Baseï¼Four fundamental Agent types are constructed â BaseAgent, ReactAgent,
+content_key="parsed_output_list")) ``` ## Key Technologies - Agent Baseï¼Four
+fundamental Agent types are constructed â BaseAgent, ReactAgent,
 ExecutorAgent, SelectorAgent, supporting basic activities across various
-scenarios â Communication: Information transmission between Agents is
+scenarios - Communication: Information transmission between Agents is
 accomplished through Message and Parse Message entities, interacting with
-Memory Manager and managing memories in the Memory Pool â Prompt Manager:
+Memory Manager and managing memories in the Memory Pool - Prompt Manager:
 Customized Agent Prompts are automatically assembled with the aid of Role
-Handler, Doc/Tool Handler, Session Handler, and Customized Handler â Memory
+Handler, Doc/Tool Handler, Session Handler, and Customized Handler - Memory
 Manager: Facilitates the management of chat history storage, information
 compression, and memory retrieval, culminating in storage within databases,
-local systems, and vector databases via the Memory Pool â Component:
-Auxiliary ecosystem components to construct Agents, including Retrieval, Tool,
-Action, Sandbox, etc. â Customized Model: Supports the integration of private
-LLM and Embedding models ## Contribution We are deeply grateful for your
-interest in the Codefuse project and warmly welcome any suggestions, opinions
-(including criticism), comments, and contributions. Feel free to raise your
-suggestions, opinions, and comments directly through GitHub Issues. There are
-numerous ways to participate in and contribute to the Codefuse project: code
-implementation, writing tests, process tool improvements, documentation
-enhancements, etc. We welcome any contribution and will add you to the list of
-contributors. See [Contribution Guide...](docs/contribution/
-contribute_guide.md) ## ð Miscellaneous ### ð± Contact Us
+local systems, and vector databases via the Memory Pool - Component: Auxiliary
+ecosystem components to construct Agents, including Retrieval, Tool, Action,
+Sandbox, etc. - Customized Model: Supports the integration of private LLM and
+Embedding models ## Contribution We are deeply grateful for your interest in
+the Codefuse project and warmly welcome any suggestions, opinions (including
+criticism), comments, and contributions. Feel free to raise your suggestions,
+opinions, and comments directly through GitHub Issues. There are numerous ways
+to participate in and contribute to the Codefuse project: code implementation,
+writing tests, process tool improvements, documentation enhancements, etc. We
+welcome any contribution and will add you to the list of contributors. See
+[Contribution Guide...](docs/contribution/contribute_guide.md) ## ð
+Miscellaneous ### ð± Contact Us
                                  width="360">
```

### Comparing `codefuse_muagent-0.0.3/muagent/base_configs/env_config.py` & `codefuse_muagent-0.0.4/muagent/base_configs/env_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/chat/agent_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/agent_chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,15 @@
             embed_model: str = Body("", description="向量模型"),
             embed_model_path: str = Body("", description="向量模型路径"),
             model_device: str = Body("", description="模型加载设备"),
             embed_engine: str = Body("", description="向量模型类型"),
             model_name: str = Body("", description="llm模型名称"),
             temperature: float = Body(0.2, description=""),
             chat_index: str = "",
+            local_graph_path: str = "",
             **kargs
             ) -> Message:
         
         # update configs
         phase_configs, chain_configs, agent_configs = self.update_configs(
             custom_phase_configs, custom_chain_configs, custom_role_configs)
         params = locals()
@@ -118,15 +119,16 @@
             do_doc_retrieval=do_doc_retrieval,
             do_code_retrieval=do_code_retrieval,
             do_tool_retrieval=do_tool_retrieval,
             doc_engine_name=doc_engine_name, search_engine_name=search_engine_name,
             code_engine_name=code_engine_name,
             score_threshold=score_threshold, top_k=top_k,
             history_node_list=history_node_list,
-            tools=tools
+            tools=tools,
+            local_graph_path=local_graph_path
         )
         # history memory mangemant
         history = Memory(messages=[
             Message(chat_index=chat_index,role_name=i["role"], role_type=i["role"], role_content=i["content"]) 
             for i in history
             ])
         # start to execute
@@ -219,14 +221,15 @@
             embed_model: str = Body("", description="向量模型"),
             embed_model_path: str = Body("", description="向量模型路径"),
             model_device: str = Body("", description="模型加载设备"),
             embed_engine: str = Body("", description="向量模型类型"),
             model_name: str = Body("", description="llm模型名称"),
             temperature: float = Body(0.2, description=""),
             chat_index: str = "",
+            local_graph_path: str = "",
             **kargs
             ) -> Message:
         
         # update configs
         phase_configs, chain_configs, agent_configs = self.update_configs(
             custom_phase_configs, custom_chain_configs, custom_role_configs)
         
@@ -260,15 +263,16 @@
             do_tool_retrieval=do_tool_retrieval,
             doc_engine_name=doc_engine_name, 
             search_engine_name=search_engine_name,
             code_engine_name=code_engine_name,
             cb_search_type=cb_search_type,
             score_threshold=score_threshold, top_k=top_k,
             history_node_list=history_node_list,
-            tools=tools
+            tools=tools,
+            local_graph_path=local_graph_path
         )
         # history memory mangemant
         history = Memory(messages=[
             Message(role_name=i["role"], role_type=i["role"], role_content=i["content"]) 
             for i in history
             ])
         # start to execute
@@ -288,15 +292,16 @@
                 )
             self.chatPhase_dict[phase_configs[input_message.phase_name]["phase_type"]] = phase
         else:
             phase = self.chatPhase_dict[phase_configs[input_message.phase_name]["phase_type"]]
         
         def chat_iterator(message: Message, local_memory: Memory, isDetailed=False):
             step_content = local_memory.to_str_messages(content_key='step_content', filter_roles=["human"])
-            step_content = "\n\n".join([f"{v}" for parsed_output in local_memory.get_parserd_output_list()[1:] for k, v in parsed_output.items() if k not in ["Action Status"]])
+            step_content = "\n\n".join([f"{v}" for parsed_output in local_memory.get_parserd_output_list() for k, v in parsed_output.items() if k not in ["Action Status", "human", "user"]])
+            # logger.debug(f"{local_memory.get_parserd_output_list()}")
             final_content = message.role_content
             result = {
                 "answer": "",
                 "db_docs": [str(doc) for doc in message.db_docs],
                 "search_docs": [str(doc) for doc in message.search_docs],
                 "code_docs":  [str(doc) for doc in message.code_docs],
                 "related_nodes": [doc.get_related_node() for idx, doc in enumerate(message.code_docs) if idx==0],
@@ -307,15 +312,15 @@
             
             related_nodes, has_nodes = [], [ ]
             for nodes in result["related_nodes"]:
                 for node in nodes:
                     if node not in has_nodes:
                         related_nodes.append(node)
             result["related_nodes"] = related_nodes
-            
+
             # logger.debug(f"{result['figures'].keys()}, isDetailed: {isDetailed}")
             message_str = step_content
             if self.stream:
                 for token in message_str:
                     result["answer"] = token
                     yield json.dumps(result, ensure_ascii=False)
             else:
```

### Comparing `codefuse_muagent-0.0.3/muagent/chat/base_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/base_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/chat/code_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/code_chat.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,29 +49,30 @@
 
     def check_service_status(self) -> BaseResponse:
         cb = cb_exists_api(self.engine_name)
         if not cb:
             return BaseResponse(code=404, msg=f"未找到代码库 {self.engine_name}")
         return BaseResponse(code=200, msg=f"找到代码库 {self.engine_name}")
 
-    def _process(self, query: str, history: List[History], model, llm_config: LLMConfig, embed_config: EmbedConfig):
+    def _process(self, query: str, history: List[History], model, llm_config: LLMConfig, embed_config: EmbedConfig, local_graph_path=""):
         '''process'''
 
         codes_res = search_code(query=query, cb_name=self.engine_name, code_limit=self.code_limit,
                                 search_type=self.cb_search_type,
                                 history_node_list=self.history_node_list,
                                 api_key=llm_config.api_key,
                                 api_base_url=llm_config.api_base_url,
                                 model_name=llm_config.model_name,
                                 temperature=llm_config.temperature,
                                 embed_model=embed_config.embed_model,
                                 embed_model_path=embed_config.embed_model_path,
                                 embed_engine=embed_config.embed_engine,
                                 model_device=embed_config.model_device,
-                                embed_config=embed_config
+                                embed_config=embed_config,
+                                local_graph_path=local_graph_path
                                 )
 
         context = codes_res['context']
         related_vertices = codes_res['related_vertices']
 
         # update node names
         # node_names = [node[0] for node in nodes]
@@ -111,40 +112,41 @@
             api_base_url: str = Body(os.environ.get("API_BASE_URL")),
             embed_model: str = Body("", ),
             embed_model_path: str = Body("", ),
             embed_engine: str = Body("", ),
             model_name: str = Body("", ),
             temperature: float = Body(0.5, ),
             model_device: str = Body("", ),
+            local_graph_path: str=Body(", "),
             **kargs
             ):
         params = locals()
         params.pop("self")
         llm_config: LLMConfig = LLMConfig(**params)
         embed_config: EmbedConfig = EmbedConfig(**params)
         self.engine_name = engine_name if isinstance(engine_name, str) else engine_name.default
         self.code_limit = code_limit
         self.stream = stream if isinstance(stream, bool) else stream.default
         self.local_doc_url = local_doc_url if isinstance(local_doc_url, bool) else local_doc_url.default
         self.request = request
         self.cb_search_type = cb_search_type
-        return self._chat(query, history, llm_config, embed_config, **kargs)
+        return self._chat(query, history, llm_config, embed_config, local_graph_path, **kargs)
 
-    def _chat(self, query: str, history: List[History], llm_config: LLMConfig, embed_config: EmbedConfig, **kargs):
+    def _chat(self, query: str, history: List[History], llm_config: LLMConfig, embed_config: EmbedConfig, local_graph_path: str, **kargs):
         history = [History(**h) if isinstance(h, dict) else h for h in history]
 
         service_status = self.check_service_status()
 
         if service_status.code != 200: return service_status
 
         def chat_iterator(query: str, history: List[History]):
             # model = getChatModel()
             model = getChatModelFromConfig(llm_config)
 
-            result, content = self.create_task(query, history, model, llm_config, embed_config, **kargs)
+            result, content = self.create_task(query, history, model, llm_config, embed_config, local_graph_path, **kargs)
             # logger.info('result={}'.format(result))
             # logger.info('content={}'.format(content))
 
             if self.stream:
                 for token in content["text"]:
                     result["answer"] = token
                     yield json.dumps(result, ensure_ascii=False)
@@ -152,17 +154,17 @@
                 for token in content["text"]:
                     result["answer"] += token
                 yield json.dumps(result, ensure_ascii=False)
 
         return StreamingResponse(chat_iterator(query, history),
                                  media_type="text/event-stream")
 
-    def create_task(self, query: str, history: List[History], model, llm_config: LLMConfig, embed_config: EmbedConfig):
+    def create_task(self, query: str, history: List[History], model, llm_config: LLMConfig, embed_config: EmbedConfig, local_graph_path: str):
         '''构建 llm 生成任务'''
-        chain, context, result = self._process(query, history, model, llm_config, embed_config)
+        chain, context, result = self._process(query, history, model, llm_config, embed_config, local_graph_path)
         logger.info('chain={}'.format(chain))
         try:
             content = chain({"context": context, "question": query})
         except Exception as e:
             content = {"text": str(e)}
         return result, content
```

### Comparing `codefuse_muagent-0.0.3/muagent/chat/knowledge_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/knowledge_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/chat/llm_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/llm_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/chat/search_chat.py` & `codefuse_muagent-0.0.4/muagent/chat/search_chat.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/chat/utils.py` & `codefuse_muagent-0.0.4/muagent/chat/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_analyzer.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_analyzer.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_dedup.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_dedup.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_intepreter.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_intepreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,19 @@
         res = {}
         messages = []
         for code in code_list:
             message = CODE_INTERPERT_TEMPLATE.format(code=code)
             messages.append(message)
 
         try:
-            chat_ress = [chat_model(messages) for message in messages]
-        except:
+            chat_ress = [chat_model.predict(message) for message in messages]
+        except Exception as e:
+            logger.exception(f"{e}")
             chat_ress = chat_model.batch(messages)
+
         for chat_res, code in zip(chat_ress, code_list):
             try:
                 res[code] = chat_res.content
             except:
                 res[code] = chat_res
         return res
```

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/code_static_analysis.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/code_static_analysis.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_analyzer/language_static_analysis/java_static_analysis.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_crawler/dir_crawler.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_crawler/dir_crawler.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_crawler/zip_crawler.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_crawler/zip_crawler.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_search/code_search.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_search/code_search.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_search/cypher_generator.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_search/cypher_generator.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/code_search/tagger.py` & `codefuse_muagent-0.0.4/muagent/codechat/code_search/tagger.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/code_importer.py` & `codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/code_importer.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/codechat/codebase_handler/codebase_handler.py` & `codefuse_muagent-0.0.4/muagent/codechat/codebase_handler/codebase_handler.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/agents/base_agent.py` & `codefuse_muagent-0.0.4/muagent/connector/agents/base_agent.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/agents/executor_agent.py` & `codefuse_muagent-0.0.4/muagent/connector/agents/executor_agent.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/agents/react_agent.py` & `codefuse_muagent-0.0.4/muagent/connector/agents/react_agent.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/agents/selector_agent.py` & `codefuse_muagent-0.0.4/muagent/connector/agents/selector_agent.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/antflow/flow.py` & `codefuse_muagent-0.0.4/muagent/connector/antflow/flow.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/chains/base_chain.py` & `codefuse_muagent-0.0.4/muagent/connector/chains/base_chain.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/agent_config.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/agent_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/chain_config.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/chain_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/phase_config.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/phase_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompt_config.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompt_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/__init__.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/agent_selector_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/agent_selector_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/checker_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/checker_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2doc_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/code2doc_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/code2test_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/code2test_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/executor_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/executor_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/input_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/input_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/intention_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/intention_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/metagpt_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/metagpt_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/planner_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/planner_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/qa_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/qa_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_code_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_code_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_code_planner_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_code_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_code_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/react_tool_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/react_tool_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/refine_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/refine_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/configs/prompts/summary_template_prompt.py` & `codefuse_muagent-0.0.4/muagent/connector/configs/prompts/summary_template_prompt.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/memory_manager.py` & `codefuse_muagent-0.0.4/muagent/connector/memory_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -586,27 +586,31 @@
              "toolKey": {"role_name": "tool_selector", "role_type": "assistant", "customed_keys": ["toolDef"]}, 
              "toolParam": {"role_name": "tool_filler", "role_type": "assistant"}, 
              "toolResponse": {"role_name": "function_caller", "role_type": "observation"}, 
              "toolSummary": {"role_name": "function_summary", "role_type": "Summary"}, 
         }
 
         for k, v in tool_map.items():
-            message = Message(
-                chat_index=chat_index,
-                message_index= f"{nodeid}-{uuid.uuid4()}",
-                user_name=user_name,
-                role_name = v["role_name"], # agent 名字，
-                role_type = v["role_type"], # agent 类型，默认assistant，可选observation
-                ## llm output
-                role_content = tool_information[k], # 输入
-                customed_kargs = {
-                    **{kk: vv for kk, vv in tool_information.items() 
-                        if kk in v.get("customed_keys", [])}
-                } # 存储docs、tool等信息
-            )
+            try:
+                message = Message(
+                    chat_index=chat_index,
+                    #message_index= f"{nodeid}-{uuid.uuid4()}",
+                    message_index= f"{nodeid}-{k}",
+                    user_name=user_name,
+                    role_name = v["role_name"], # agent 名字，
+                    role_type = v["role_type"], # agent 类型，默认assistant，可选observation
+                    ## llm output
+                    role_content = tool_information[k], # 输入
+                    customed_kargs = {
+                        **{kk: vv for kk, vv in tool_information.items() 
+                            if kk in v.get("customed_keys", [])}
+                    } # 存储docs、tool等信息
+                )
+            except:
+                pass
             self.append(message)
 
     def get_memory_pool(self, chat_index: str = "") -> Memory:
         return self.get_memory_pool_by_all({"chat_index": chat_index})
 
     def get_memory_pool_by_content(self, content: str, ):
         r = self.th.search(content)
@@ -798,20 +802,24 @@
         '''
         convert redis documents to Message
         '''
         memory = Memory()
         for doc in r_docs.docs:
             tbase_message = {}
             for k, v in doc.__dict__.items():
+                if k in ["role_content", "input_query"]:
+                    tbase_message[k] = v
+                    continue
                 try:
                     v = json.loads(v)
                 except:
                     pass
 
                 tbase_message[k] = v
+
             message = Message(**tbase_message)
             memory.append(message)
 
         for message in memory.messages:
             message.start_datetime = timestampToDateformat(int(message.start_datetime), 1)
             message.end_datetime = timestampToDateformat(int(message.end_datetime), 1)
```

### Comparing `codefuse_muagent-0.0.3/muagent/connector/message_process.py` & `codefuse_muagent-0.0.4/muagent/connector/message_process.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/phase/base_phase.py` & `codefuse_muagent-0.0.4/muagent/connector/phase/base_phase.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/prompt_manager/extend_manager.py` & `codefuse_muagent-0.0.4/muagent/connector/prompt_manager/extend_manager.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/prompt_manager/prompt_manager.py` & `codefuse_muagent-0.0.4/muagent/connector/prompt_manager/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/schema/general_schema.py` & `codefuse_muagent-0.0.4/muagent/connector/schema/general_schema.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/schema/memory.py` & `codefuse_muagent-0.0.4/muagent/connector/schema/memory.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/schema/message.py` & `codefuse_muagent-0.0.4/muagent/connector/schema/message.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/connector/utils.py` & `codefuse_muagent-0.0.4/muagent/connector/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/db_handler/graph_db_handler/nebula_handler.py` & `codefuse_muagent-0.0.4/muagent/db_handler/graph_db_handler/nebula_handler.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/db_handler/vector_db_handler/chroma_handler.py` & `codefuse_muagent-0.0.4/muagent/db_handler/vector_db_handler/chroma_handler.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/commands/default_vs_cds.py` & `codefuse_muagent-0.0.4/muagent/embeddings/commands/default_vs_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/faiss_m.py` & `codefuse_muagent-0.0.4/muagent/embeddings/faiss_m.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/get_embedding.py` & `codefuse_muagent-0.0.4/muagent/embeddings/get_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/huggingface_embedding.py` & `codefuse_muagent-0.0.4/muagent/embeddings/huggingface_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/in_memory.py` & `codefuse_muagent-0.0.4/muagent/embeddings/in_memory.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/openai_embedding.py` & `codefuse_muagent-0.0.4/muagent/embeddings/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/embeddings/utils.py` & `codefuse_muagent-0.0.4/muagent/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/llm_models/llm_config.py` & `codefuse_muagent-0.0.4/muagent/llm_models/llm_config.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/llm_models/openai_model.py` & `codefuse_muagent-0.0.4/muagent/llm_models/openai_model.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/__init__.py` & `codefuse_muagent-0.0.4/muagent/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/commands/code_base_cds.py` & `codefuse_muagent-0.0.4/muagent/orm/commands/code_base_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/commands/document_base_cds.py` & `codefuse_muagent-0.0.4/muagent/orm/commands/document_base_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/commands/document_file_cds.py` & `codefuse_muagent-0.0.4/muagent/orm/commands/document_file_cds.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/db.py` & `codefuse_muagent-0.0.4/muagent/orm/db.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/schemas/base_schema.py` & `codefuse_muagent-0.0.4/muagent/orm/schemas/base_schema.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/orm/utils.py` & `codefuse_muagent-0.0.4/muagent/orm/utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/retrieval/base_retrieval.py` & `codefuse_muagent-0.0.4/muagent/retrieval/base_retrieval.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/json_loader.py` & `codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/json_loader.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/retrieval/document_loaders/jsonl_loader.py` & `codefuse_muagent-0.0.4/muagent/retrieval/document_loaders/jsonl_loader.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/retrieval/text_splitter/langchain_splitter.py` & `codefuse_muagent-0.0.4/muagent/retrieval/text_splitter/langchain_splitter.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/sandbox/basebox.py` & `codefuse_muagent-0.0.4/muagent/sandbox/basebox.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/sandbox/pycodebox.py` & `codefuse_muagent-0.0.4/muagent/sandbox/pycodebox.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/service/base_service.py` & `codefuse_muagent-0.0.4/muagent/service/base_service.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/service/cb_api.py` & `codefuse_muagent-0.0.4/muagent/service/cb_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,15 @@
                     embed_model: bool = Body(..., examples=["samples"]),
                     embed_model_path: bool = Body(..., examples=["samples"]),
                     embed_engine: bool = Body(..., examples=["samples"]),
                     model_name: bool = Body(..., examples=["samples"]),
                     temperature: bool = Body(..., examples=["samples"]),
                     model_device: bool = Body(..., examples=["samples"]),
                     embed_config: EmbedConfig = None,
+                    local_graph_path: str = '',
                     ) -> BaseResponse:
     logger.info('cb_name={}, zip_path={}, do_interpret={}'.format(cb_name, code_path, do_interpret))
 
     embed_config: EmbedConfig = EmbedConfig(**locals()) if embed_config is None else embed_config
     llm_config: LLMConfig = LLMConfig(**locals())
 
     # Create selected knowledge base
@@ -70,15 +71,15 @@
 
     cb = cb_exists(cb_name)
     if cb:
         return BaseResponse(code=404, msg=f"已存在同名代码知识库 {cb_name}")
 
     try:
         logger.info('start build code base')
-        cbh = CodeBaseHandler(cb_name, code_path, embed_config=embed_config, llm_config=llm_config)
+        cbh = CodeBaseHandler(cb_name, code_path, embed_config=embed_config, llm_config=llm_config, local_graph_path=local_graph_path)
         vertices_num, edge_num, file_num = cbh.import_code(zip_file=zip_file, do_interpret=do_interpret)
         logger.info('build code base done')
 
         # create cb to table
         add_cb_to_db(cb_name, cbh.code_path, vertices_num, file_num, do_interpret)
         logger.info('add cb to mysql table success')
     except Exception as e:
@@ -96,14 +97,15 @@
         embed_model: bool = Body(..., examples=["samples"]),
         embed_model_path: bool = Body(..., examples=["samples"]),
         embed_engine: bool = Body(..., examples=["samples"]),
         model_name: bool = Body(..., examples=["samples"]),
         temperature: bool = Body(..., examples=["samples"]),
         model_device: bool = Body(..., examples=["samples"]),
         embed_config: EmbedConfig = None,
+        local_graph_path: str="",
         ) -> BaseResponse:
     logger.info('cb_name={}'.format(cb_name))
     embed_config: EmbedConfig = EmbedConfig(**locals()) if embed_config is None else embed_config
     llm_config: LLMConfig = LLMConfig(**locals())
     # Create selected knowledge base
     if not validate_kb_name(cb_name):
         return BaseResponse(code=403, msg="Don't attack me")
@@ -115,15 +117,15 @@
         try:
             delete_cb_from_db(cb_name)
 
             # delete local file
             shutil.rmtree(CB_ROOT_PATH + os.sep + cb_name)
 
             # delete from codebase
-            cbh = CodeBaseHandler(cb_name, embed_config=embed_config, llm_config=llm_config)
+            cbh = CodeBaseHandler(cb_name, embed_config=embed_config, llm_config=llm_config, local_graph_path=local_graph_path)
             cbh.delete_codebase(codebase_name=cb_name)
 
         except Exception as e:
             print(e)
             return BaseResponse(code=500, msg=f"删除代码知识库出错： {e}")
 
     return BaseResponse(code=200, msg=f"已删除代码知识库 {cb_name}")
@@ -139,15 +141,15 @@
                 embed_model: bool = Body(..., examples=["samples"]),
                 embed_model_path: bool = Body(..., examples=["samples"]),
                 embed_engine: bool = Body(..., examples=["samples"]),
                 model_name: bool = Body(..., examples=["samples"]),
                 temperature: bool = Body(..., examples=["samples"]),
                 model_device: bool = Body(..., examples=["samples"]),
                 use_nh: bool = True,
-                local_graph_path: str = '',
+                local_graph_path: str = CB_ROOT_PATH,
                 embed_config: EmbedConfig = None,
                 ) -> dict:
     
     if os.environ.get("log_verbose", "0") >= "2":
         logger.info(f'local_graph_path={local_graph_path}')
         logger.info('cb_name={}'.format(cb_name))
         logger.info('query={}'.format(query))
```

### Comparing `codefuse_muagent-0.0.3/muagent/service/faiss_db_service.py` & `codefuse_muagent-0.0.4/muagent/service/faiss_db_service.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/service/kb_api.py` & `codefuse_muagent-0.0.4/muagent/service/kb_api.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/service/migrate.py` & `codefuse_muagent-0.0.4/muagent/service/migrate.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/service/service_factory.py` & `codefuse_muagent-0.0.4/muagent/service/service_factory.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/__init__.py` & `codefuse_muagent-0.0.4/muagent/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/abnormal_detection.py` & `codefuse_muagent-0.0.4/muagent/tools/abnormal_detection.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/base_tool.py` & `codefuse_muagent-0.0.4/muagent/tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/cb_query_tool.py` & `codefuse_muagent-0.0.4/muagent/tools/cb_query_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/codechat_tools.py` & `codefuse_muagent-0.0.4/muagent/tools/codechat_tools.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/docs_retrieval.py` & `codefuse_muagent-0.0.4/muagent/tools/docs_retrieval.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/duckduckgo_search.py` & `codefuse_muagent-0.0.4/muagent/tools/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/metrics_query.py` & `codefuse_muagent-0.0.4/muagent/tools/metrics_query.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/multiplier.py` & `codefuse_muagent-0.0.4/muagent/tools/multiplier.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/ocr_tool.py` & `codefuse_muagent-0.0.4/muagent/tools/ocr_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/stock_tool.py` & `codefuse_muagent-0.0.4/muagent/tools/stock_tool.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/tool_datas/stock_data.py` & `codefuse_muagent-0.0.4/muagent/tools/tool_datas/stock_data.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/weather.py` & `codefuse_muagent-0.0.4/muagent/tools/weather.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/tools/world_time.py` & `codefuse_muagent-0.0.4/muagent/tools/world_time.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/utils/code2doc_util.py` & `codefuse_muagent-0.0.4/muagent/utils/code2doc_util.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/utils/common_utils.py` & `codefuse_muagent-0.0.4/muagent/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/utils/path_utils.py` & `codefuse_muagent-0.0.4/muagent/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/utils/server_utils.py` & `codefuse_muagent-0.0.4/muagent/utils/server_utils.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/muagent/utils/tbase_util.py` & `codefuse_muagent-0.0.4/muagent/utils/tbase_util.py`

 * *Files identical despite different names*

### Comparing `codefuse_muagent-0.0.3/setup.py` & `codefuse_muagent-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 # with open("README.md", "r", encoding="utf-8") as fh:
 #     long_description = fh.read()
 
 setuptools.setup(
-    name="muagent",
-    version="0.0.3",
+    name="codefuse-muagent",
+    version="0.0.4",
     author="shanshi",
     author_email="wyp311395@antgroup.com",
     description="A multi-agent framework that facilitates the rapid construction of collaborative teams of agents.",
     # long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/codefuse-ai/CodeFuse-muAgent",
     packages=setuptools.find_packages(),
```

### Comparing `codefuse_muagent-0.0.3/tests/test_config.py` & `codefuse_muagent-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

