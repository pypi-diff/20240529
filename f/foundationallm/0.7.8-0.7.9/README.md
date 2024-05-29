# Comparing `tmp/foundationallm-0.7.8.tar.gz` & `tmp/foundationallm-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundationallm-0.7.8.tar", last modified: Mon May 27 12:08:56 2024, max compression
+gzip compressed data, was "foundationallm-0.7.9.tar", last modified: Mon May 27 12:16:51 2024, max compression
```

## Comparing `foundationallm-0.7.8.tar` & `foundationallm-0.7.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.554396 foundationallm-0.7.8/
--rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.8/LICENSE
--rw-rw-rw-   0        0        0      892 2024-05-27 12:08:56.552891 foundationallm-0.7.8/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-23 14:45:46.000000 foundationallm-0.7.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.801257 foundationallm-0.7.8/foundationallm/
--rw-rw-rw-   0        0        0       71 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/__init__.py
--rw-rw-rw-   0        0        0       23 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.849299 foundationallm-0.7.8/foundationallm/config/
--rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/config/__init__.py
--rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.8/foundationallm/config/configuration.py
--rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/config/context.py
--rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.8/foundationallm/config/environment_variables.py
--rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/config/user_identity.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.858840 foundationallm-0.7.8/foundationallm/langchain/
--rw-rw-rw-   0        0        0       39 2023-10-19 14:24:41.000000 foundationallm-0.7.8/foundationallm/langchain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.896203 foundationallm-0.7.8/foundationallm/langchain/agents/
--rw-rw-rw-   0        0        0      211 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/agents/__init__.py
--rw-rw-rw-   0        0        0     1903 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/agents/agent_factory.py
--rw-rw-rw-   0        0        0    14295 2024-05-27 12:04:46.000000 foundationallm-0.7.8/foundationallm/langchain/agents/langchain_agent_base.py
--rw-rw-rw-   0        0        0     5617 2024-05-27 12:07:10.000000 foundationallm-0.7.8/foundationallm/langchain/agents/langchain_knowledge_management_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.910200 foundationallm-0.7.8/foundationallm/langchain/data_sources/
--rw-rw-rw-   0        0        0       64 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.923795 foundationallm-0.7.8/foundationallm/langchain/data_sources/blob/
--rw-rw-rw-   0        0        0       66 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/blob/__init__.py
--rw-rw-rw-   0        0        0      485 2024-01-24 21:43:50.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/blob/blob_storage_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.937765 foundationallm-0.7.8/foundationallm/langchain/data_sources/cxo/
--rw-rw-rw-   0        0        0       49 2024-01-24 21:43:50.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/cxo/__init__.py
--rw-rw-rw-   0        0        0      421 2024-01-24 21:43:50.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/cxo/cxo_configuration.py
--rw-rw-rw-   0        0        0      125 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/data_source_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.951769 foundationallm-0.7.8/foundationallm/langchain/data_sources/search_service/
--rw-rw-rw-   0        0        0      103 2024-01-09 18:22:07.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/search_service/__init__.py
--rw-rw-rw-   0        0        0      655 2024-01-24 21:43:50.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/search_service/search_service_configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.041977 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/
--rw-rw-rw-   0        0        0      351 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mariadb.py
--rw-rw-rw-   0        0        0     1304 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mssql.py
--rw-rw-rw-   0        0        0     1158 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mysql.py
--rw-rw-rw-   0        0        0     1153 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/postgresql.py
--rw-rw-rw-   0        0        0      632 2024-01-24 21:43:50.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_configuration.py
--rw-rw-rw-   0        0        0     2516 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_datasource.py
--rw-rw-rw-   0        0        0      208 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_dialects.py
--rw-rw-rw-   0        0        0     1919 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.056778 foundationallm-0.7.8/foundationallm/langchain/exceptions/
--rw-rw-rw-   0        0        0       53 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/exceptions/__init__.py
--rw-rw-rw-   0        0        0      195 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/exceptions/langchain_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.080781 foundationallm-0.7.8/foundationallm/langchain/language_models/
--rw-rw-rw-   0        0        0      139 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/language_models/__init__.py
--rw-rw-rw-   0        0        0      943 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/language_models/language_model_base.py
--rw-rw-rw-   0        0        0      856 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/language_models/language_model_factory.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.096781 foundationallm-0.7.8/foundationallm/langchain/language_models/openai/
--rw-rw-rw-   0        0        0       75 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/language_models/openai/__init__.py
--rw-rw-rw-   0        0        0     4760 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/language_models/openai/openai_model.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.112782 foundationallm-0.7.8/foundationallm/langchain/orchestration/
--rw-rw-rw-   0        0        0       57 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/orchestration/__init__.py
--rw-rw-rw-   0        0        0     2242 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/orchestration/orchestration_manager.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.157875 foundationallm-0.7.8/foundationallm/langchain/retrievers/
--rw-rw-rw-   0        0        0      262 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/__init__.py
--rw-rw-rw-   0        0        0      265 2024-03-15 16:01:06.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/agent_parameter_retriever_keys.py
--rw-rw-rw-   0        0        0     6011 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/azure_ai_search_service_retriever.py
--rw-rw-rw-   0        0        0      522 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/citation_retrieval_base.py
--rw-rw-rw-   0        0        0     4779 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/retriever_factory.py
--rw-rw-rw-   0        0        0     4738 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/retrievers/search_service_filter_retriever.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.180878 foundationallm-0.7.8/foundationallm/langchain/toolkits/
--rw-rw-rw-   0        0        0      131 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/toolkits/__init__.py
--rw-rw-rw-   0        0        0     1777 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/toolkits/anomaly_detection_toolkit.py
--rw-rw-rw-   0        0        0     3245 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/toolkits/secure_sql_database_toolkit.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.204878 foundationallm-0.7.8/foundationallm/langchain/tools/
--rw-rw-rw-   0        0        0      200 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/langchain/tools/__init__.py
--rw-rw-rw-   0        0        0     2450 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/tools/query_pandas_dataframe_tool.py
--rw-rw-rw-   0        0        0     1656 2024-01-29 10:28:21.000000 foundationallm-0.7.8/foundationallm/langchain/tools/secure_sql_database_query_tool.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.221875 foundationallm-0.7.8/foundationallm/models/
--rw-rw-rw-   0        0        0       73 2024-03-15 16:01:06.000000 foundationallm-0.7.8/foundationallm/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.271448 foundationallm-0.7.8/foundationallm/models/agents/
--rw-rw-rw-   0        0        0      409 2024-05-23 14:45:46.000000 foundationallm-0.7.8/foundationallm/models/agents/__init__.py
--rw-rw-rw-   0        0        0      815 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/agents/agent_base.py
--rw-rw-rw-   0        0        0      316 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/agents/agent_conversation_history_settings.py
--rw-rw-rw-   0        0        0      274 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/agents/agent_gatekeeper_settings.py
--rw-rw-rw-   0        0        0      594 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/agents/agent_vectorization_settings.py
--rw-rw-rw-   0        0        0      361 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/agents/knowledge_management_agent.py
--rw-rw-rw-   0        0        0      518 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/agents/knowledge_management_completion_request.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.287447 foundationallm-0.7.8/foundationallm/models/authentication/
--rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/authentication/__init__.py
--rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/authentication/authentication_types.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.316451 foundationallm-0.7.8/foundationallm/models/language_models/
--rw-rw-rw-   0        0        0      187 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/language_models/__init__.py
--rw-rw-rw-   0        0        0      690 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/language_models/embedding_model.py
--rw-rw-rw-   0        0        0      175 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/models/language_models/language_model_provider.py
--rw-rw-rw-   0        0        0      138 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/models/language_models/language_model_type.py
--rw-rw-rw-   0        0        0      101 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/models/list_option.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.380604 foundationallm-0.7.8/foundationallm/models/orchestration/
--rw-rw-rw-   0        0        0      402 2024-05-23 14:45:46.000000 foundationallm-0.7.8/foundationallm/models/orchestration/__init__.py
--rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/orchestration/citation.py
--rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/orchestration/completion_request_base.py
--rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/orchestration/completion_response.py
--rw-rw-rw-   0        0        0      469 2024-05-23 14:45:46.000000 foundationallm-0.7.8/foundationallm/models/orchestration/endpoint_settings.py
--rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/models/orchestration/message_history_item.py
--rw-rw-rw-   0        0        0      154 2024-05-23 14:45:46.000000 foundationallm-0.7.8/foundationallm/models/orchestration/operation_types.py
--rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/orchestration/orchestration_settings.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:55.775745 foundationallm-0.7.8/foundationallm/models/resource_providers/
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.395608 foundationallm-0.7.8/foundationallm/models/resource_providers/prompts/
--rw-rw-rw-   0        0        0       98 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/prompts/__init__.py
--rw-rw-rw-   0        0        0      422 2024-05-07 13:15:07.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/prompts/multipart_prompt.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.427609 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/
--rw-rw-rw-   0        0        0      862 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/__init__.py
--rw-rw-rw-   0        0        0      320 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/configuration_references_base.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.436609 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.452610 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/
--rw-rw-rw-   0        0        0      998 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_configuration_references.py
--rw-rw-rw-   0        0        0     1388 2024-05-27 11:58:33.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_embedding_profile.py
--rw-rw-rw-   0        0        0      324 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/embedding_profile_base.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.460120 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.489159 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/
--rw-rw-rw-   0        0        0      653 2024-04-03 14:03:09.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_configuration_references.py
--rw-rw-rw-   0        0        0     1574 2024-05-27 12:07:41.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_indexing_profile.py
--rw-rw-rw-   0        0        0      649 2024-04-24 17:34:13.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_settings.py
--rw-rw-rw-   0        0        0      310 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/indexing_profile_base.py
--rw-rw-rw-   0        0        0      754 2024-05-27 11:54:11.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/profile_base.py
--rw-rw-rw-   0        0        0      229 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/settings_base.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.503121 foundationallm-0.7.8/foundationallm/models/utils/
--rw-rw-rw-   0        0        0       39 2024-05-27 11:55:25.000000 foundationallm-0.7.8/foundationallm/models/utils/__init__.py
--rw-rw-rw-   0        0        0      876 2024-05-27 11:53:40.000000 foundationallm-0.7.8/foundationallm/models/utils/object_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.529752 foundationallm-0.7.8/foundationallm/storage/
--rw-rw-rw-   0        0        0      108 2023-12-14 16:50:30.000000 foundationallm-0.7.8/foundationallm/storage/__init__.py
--rw-rw-rw-   0        0        0     6092 2024-04-30 12:19:06.000000 foundationallm-0.7.8/foundationallm/storage/blob_storage_manager.py
--rw-rw-rw-   0        0        0     2063 2024-03-15 16:01:06.000000 foundationallm-0.7.8/foundationallm/storage/storage_manager_base.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.546761 foundationallm-0.7.8/foundationallm/telemetry/
--rw-rw-rw-   0        0        0       34 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/telemetry/__init__.py
--rw-rw-rw-   0        0        0     2558 2024-03-11 14:31:54.000000 foundationallm-0.7.8/foundationallm/telemetry/telemetry.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:08:56.550762 foundationallm-0.7.8/foundationallm.egg-info/
--rw-rw-rw-   0        0        0      892 2024-05-27 12:08:55.000000 foundationallm-0.7.8/foundationallm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5801 2024-05-27 12:08:55.000000 foundationallm-0.7.8/foundationallm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:08:55.000000 foundationallm-0.7.8/foundationallm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-27 12:08:55.000000 foundationallm-0.7.8/foundationallm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2024-05-27 12:08:11.000000 foundationallm-0.7.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 12:08:56.554396 foundationallm-0.7.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.366185 foundationallm-0.7.9/
+-rw-rw-rw-   0        0        0      201 2024-05-07 13:15:07.000000 foundationallm-0.7.9/LICENSE
+-rw-rw-rw-   0        0        0      892 2024-05-27 12:16:51.364187 foundationallm-0.7.9/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-23 14:45:46.000000 foundationallm-0.7.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.646970 foundationallm-0.7.9/foundationallm/
+-rw-rw-rw-   0        0        0       71 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.693542 foundationallm-0.7.9/foundationallm/config/
+-rw-rw-rw-   0        0        0      177 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/config/__init__.py
+-rw-rw-rw-   0        0        0     4874 2024-05-23 11:10:06.000000 foundationallm-0.7.9/foundationallm/config/configuration.py
+-rw-rw-rw-   0        0        0      605 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/config/context.py
+-rw-rw-rw-   0        0        0      378 2024-03-15 16:01:06.000000 foundationallm-0.7.9/foundationallm/config/environment_variables.py
+-rw-rw-rw-   0        0        0      556 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/config/user_identity.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.699543 foundationallm-0.7.9/foundationallm/langchain/
+-rw-rw-rw-   0        0        0       39 2023-10-19 14:24:41.000000 foundationallm-0.7.9/foundationallm/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.734202 foundationallm-0.7.9/foundationallm/langchain/agents/
+-rw-rw-rw-   0        0        0      211 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/agents/__init__.py
+-rw-rw-rw-   0        0        0     1903 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/agents/agent_factory.py
+-rw-rw-rw-   0        0        0    14295 2024-05-27 12:04:46.000000 foundationallm-0.7.9/foundationallm/langchain/agents/langchain_agent_base.py
+-rw-rw-rw-   0        0        0     5617 2024-05-27 12:07:10.000000 foundationallm-0.7.9/foundationallm/langchain/agents/langchain_knowledge_management_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.747709 foundationallm-0.7.9/foundationallm/langchain/data_sources/
+-rw-rw-rw-   0        0        0       64 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.761216 foundationallm-0.7.9/foundationallm/langchain/data_sources/blob/
+-rw-rw-rw-   0        0        0       66 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/blob/__init__.py
+-rw-rw-rw-   0        0        0      485 2024-01-24 21:43:50.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/blob/blob_storage_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.774741 foundationallm-0.7.9/foundationallm/langchain/data_sources/cxo/
+-rw-rw-rw-   0        0        0       49 2024-01-24 21:43:50.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/cxo/__init__.py
+-rw-rw-rw-   0        0        0      421 2024-01-24 21:43:50.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/cxo/cxo_configuration.py
+-rw-rw-rw-   0        0        0      125 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/data_source_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.788249 foundationallm-0.7.9/foundationallm/langchain/data_sources/search_service/
+-rw-rw-rw-   0        0        0      103 2024-01-09 18:22:07.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/search_service/__init__.py
+-rw-rw-rw-   0        0        0      655 2024-01-24 21:43:50.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/search_service/search_service_configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.857461 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/
+-rw-rw-rw-   0        0        0      351 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mariadb.py
+-rw-rw-rw-   0        0        0     1304 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mssql.py
+-rw-rw-rw-   0        0        0     1158 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mysql.py
+-rw-rw-rw-   0        0        0     1153 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/postgresql.py
+-rw-rw-rw-   0        0        0      632 2024-01-24 21:43:50.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_configuration.py
+-rw-rw-rw-   0        0        0     2516 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_datasource.py
+-rw-rw-rw-   0        0        0      208 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_dialects.py
+-rw-rw-rw-   0        0        0     1919 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.871500 foundationallm-0.7.9/foundationallm/langchain/exceptions/
+-rw-rw-rw-   0        0        0       53 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      195 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/exceptions/langchain_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.893190 foundationallm-0.7.9/foundationallm/langchain/language_models/
+-rw-rw-rw-   0        0        0      139 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/language_models/__init__.py
+-rw-rw-rw-   0        0        0      943 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/language_models/language_model_base.py
+-rw-rw-rw-   0        0        0      856 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/language_models/language_model_factory.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.908005 foundationallm-0.7.9/foundationallm/langchain/language_models/openai/
+-rw-rw-rw-   0        0        0       75 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/language_models/openai/__init__.py
+-rw-rw-rw-   0        0        0     4760 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/language_models/openai/openai_model.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.922284 foundationallm-0.7.9/foundationallm/langchain/orchestration/
+-rw-rw-rw-   0        0        0       57 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/orchestration/__init__.py
+-rw-rw-rw-   0        0        0     2242 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/orchestration/orchestration_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.969576 foundationallm-0.7.9/foundationallm/langchain/retrievers/
+-rw-rw-rw-   0        0        0      262 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/__init__.py
+-rw-rw-rw-   0        0        0      265 2024-03-15 16:01:06.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/agent_parameter_retriever_keys.py
+-rw-rw-rw-   0        0        0     6011 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/azure_ai_search_service_retriever.py
+-rw-rw-rw-   0        0        0      522 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/citation_retrieval_base.py
+-rw-rw-rw-   0        0        0     4779 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/retriever_factory.py
+-rw-rw-rw-   0        0        0     4738 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/retrievers/search_service_filter_retriever.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.994114 foundationallm-0.7.9/foundationallm/langchain/toolkits/
+-rw-rw-rw-   0        0        0      131 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/toolkits/__init__.py
+-rw-rw-rw-   0        0        0     1777 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/toolkits/anomaly_detection_toolkit.py
+-rw-rw-rw-   0        0        0     3245 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/toolkits/secure_sql_database_toolkit.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.018510 foundationallm-0.7.9/foundationallm/langchain/tools/
+-rw-rw-rw-   0        0        0      200 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/langchain/tools/__init__.py
+-rw-rw-rw-   0        0        0     2450 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/tools/query_pandas_dataframe_tool.py
+-rw-rw-rw-   0        0        0     1656 2024-01-29 10:28:21.000000 foundationallm-0.7.9/foundationallm/langchain/tools/secure_sql_database_query_tool.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.032178 foundationallm-0.7.9/foundationallm/models/
+-rw-rw-rw-   0        0        0       73 2024-03-15 16:01:06.000000 foundationallm-0.7.9/foundationallm/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.087143 foundationallm-0.7.9/foundationallm/models/agents/
+-rw-rw-rw-   0        0        0      409 2024-05-23 14:45:46.000000 foundationallm-0.7.9/foundationallm/models/agents/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/agents/agent_base.py
+-rw-rw-rw-   0        0        0      316 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/agents/agent_conversation_history_settings.py
+-rw-rw-rw-   0        0        0      274 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/agents/agent_gatekeeper_settings.py
+-rw-rw-rw-   0        0        0      594 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/agents/agent_vectorization_settings.py
+-rw-rw-rw-   0        0        0      361 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/agents/knowledge_management_agent.py
+-rw-rw-rw-   0        0        0      518 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/agents/knowledge_management_completion_request.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.101154 foundationallm-0.7.9/foundationallm/models/authentication/
+-rw-rw-rw-   0        0        0       55 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/authentication/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/authentication/authentication_types.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.130176 foundationallm-0.7.9/foundationallm/models/language_models/
+-rw-rw-rw-   0        0        0      187 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/language_models/__init__.py
+-rw-rw-rw-   0        0        0      690 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/language_models/embedding_model.py
+-rw-rw-rw-   0        0        0      175 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/models/language_models/language_model_provider.py
+-rw-rw-rw-   0        0        0      138 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/models/language_models/language_model_type.py
+-rw-rw-rw-   0        0        0      101 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/models/list_option.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.187358 foundationallm-0.7.9/foundationallm/models/orchestration/
+-rw-rw-rw-   0        0        0      402 2024-05-23 14:45:46.000000 foundationallm-0.7.9/foundationallm/models/orchestration/__init__.py
+-rw-rw-rw-   0        0        0      272 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/orchestration/citation.py
+-rw-rw-rw-   0        0        0      502 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/orchestration/completion_request_base.py
+-rw-rw-rw-   0        0        0      523 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/orchestration/completion_response.py
+-rw-rw-rw-   0        0        0      469 2024-05-23 14:45:46.000000 foundationallm-0.7.9/foundationallm/models/orchestration/endpoint_settings.py
+-rw-rw-rw-   0        0        0      370 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/models/orchestration/message_history_item.py
+-rw-rw-rw-   0        0        0      154 2024-05-23 14:45:46.000000 foundationallm-0.7.9/foundationallm/models/orchestration/operation_types.py
+-rw-rw-rw-   0        0        0      939 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/orchestration/orchestration_settings.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:50.621954 foundationallm-0.7.9/foundationallm/models/resource_providers/
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.202385 foundationallm-0.7.9/foundationallm/models/resource_providers/prompts/
+-rw-rw-rw-   0        0        0       98 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/prompts/__init__.py
+-rw-rw-rw-   0        0        0      422 2024-05-07 13:15:07.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/prompts/multipart_prompt.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.231543 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/
+-rw-rw-rw-   0        0        0      862 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/__init__.py
+-rw-rw-rw-   0        0        0      320 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/configuration_references_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.238548 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.254570 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/
+-rw-rw-rw-   0        0        0      998 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_configuration_references.py
+-rw-rw-rw-   0        0        0     1371 2024-05-27 12:16:26.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_embedding_profile.py
+-rw-rw-rw-   0        0        0      324 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/embedding_profile_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.264089 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.291815 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/
+-rw-rw-rw-   0        0        0      653 2024-04-03 14:03:09.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_configuration_references.py
+-rw-rw-rw-   0        0        0     1556 2024-05-27 12:16:11.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_indexing_profile.py
+-rw-rw-rw-   0        0        0      649 2024-04-24 17:34:13.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_settings.py
+-rw-rw-rw-   0        0        0      310 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/indexing_profile_base.py
+-rw-rw-rw-   0        0        0      754 2024-05-27 11:54:11.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/profile_base.py
+-rw-rw-rw-   0        0        0      229 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/settings_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.309327 foundationallm-0.7.9/foundationallm/models/utils/
+-rw-rw-rw-   0        0        0       39 2024-05-27 11:55:25.000000 foundationallm-0.7.9/foundationallm/models/utils/__init__.py
+-rw-rw-rw-   0        0        0      876 2024-05-27 11:53:40.000000 foundationallm-0.7.9/foundationallm/models/utils/object_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.338869 foundationallm-0.7.9/foundationallm/storage/
+-rw-rw-rw-   0        0        0      108 2023-12-14 16:50:30.000000 foundationallm-0.7.9/foundationallm/storage/__init__.py
+-rw-rw-rw-   0        0        0     6092 2024-04-30 12:19:06.000000 foundationallm-0.7.9/foundationallm/storage/blob_storage_manager.py
+-rw-rw-rw-   0        0        0     2063 2024-03-15 16:01:06.000000 foundationallm-0.7.9/foundationallm/storage/storage_manager_base.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.358667 foundationallm-0.7.9/foundationallm/telemetry/
+-rw-rw-rw-   0        0        0       34 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/telemetry/__init__.py
+-rw-rw-rw-   0        0        0     2558 2024-03-11 14:31:54.000000 foundationallm-0.7.9/foundationallm/telemetry/telemetry.py
+drwxrwxrwx   0        0        0        0 2024-05-27 12:16:51.362180 foundationallm-0.7.9/foundationallm.egg-info/
+-rw-rw-rw-   0        0        0      892 2024-05-27 12:16:50.000000 foundationallm-0.7.9/foundationallm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5801 2024-05-27 12:16:50.000000 foundationallm-0.7.9/foundationallm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 12:16:50.000000 foundationallm-0.7.9/foundationallm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-27 12:16:50.000000 foundationallm-0.7.9/foundationallm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      583 2024-05-27 12:16:36.000000 foundationallm-0.7.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-27 12:16:51.366185 foundationallm-0.7.9/setup.cfg
```

### Comparing `foundationallm-0.7.8/PKG-INFO` & `foundationallm-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.8
+Version: 0.7.9
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.8/foundationallm/config/configuration.py` & `foundationallm-0.7.9/foundationallm/config/configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/config/context.py` & `foundationallm-0.7.9/foundationallm/config/context.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/config/user_identity.py` & `foundationallm-0.7.9/foundationallm/config/user_identity.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/agents/agent_factory.py` & `foundationallm-0.7.9/foundationallm/langchain/agents/agent_factory.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/agents/langchain_agent_base.py` & `foundationallm-0.7.9/foundationallm/langchain/agents/langchain_agent_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/agents/langchain_knowledge_management_agent.py` & `foundationallm-0.7.9/foundationallm/langchain/agents/langchain_knowledge_management_agent.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/search_service/search_service_configuration.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/search_service/search_service_configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mariadb.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mariadb.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mssql.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mssql.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/mysql.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/mysql.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/postgresql.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/postgresql.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_configuration.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_configuration.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_datasource.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_datasource.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/data_sources/sql/sql_database_factory.py` & `foundationallm-0.7.9/foundationallm/langchain/data_sources/sql/sql_database_factory.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/language_models/language_model_base.py` & `foundationallm-0.7.9/foundationallm/langchain/language_models/language_model_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/language_models/language_model_factory.py` & `foundationallm-0.7.9/foundationallm/langchain/language_models/language_model_factory.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/language_models/openai/openai_model.py` & `foundationallm-0.7.9/foundationallm/langchain/language_models/openai/openai_model.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/orchestration/orchestration_manager.py` & `foundationallm-0.7.9/foundationallm/langchain/orchestration/orchestration_manager.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/retrievers/azure_ai_search_service_retriever.py` & `foundationallm-0.7.9/foundationallm/langchain/retrievers/azure_ai_search_service_retriever.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/retrievers/citation_retrieval_base.py` & `foundationallm-0.7.9/foundationallm/langchain/retrievers/citation_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/retrievers/retriever_factory.py` & `foundationallm-0.7.9/foundationallm/langchain/retrievers/retriever_factory.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/retrievers/search_service_filter_retriever.py` & `foundationallm-0.7.9/foundationallm/langchain/retrievers/search_service_filter_retriever.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/toolkits/anomaly_detection_toolkit.py` & `foundationallm-0.7.9/foundationallm/langchain/toolkits/anomaly_detection_toolkit.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/toolkits/secure_sql_database_toolkit.py` & `foundationallm-0.7.9/foundationallm/langchain/toolkits/secure_sql_database_toolkit.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/tools/query_pandas_dataframe_tool.py` & `foundationallm-0.7.9/foundationallm/langchain/tools/query_pandas_dataframe_tool.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/langchain/tools/secure_sql_database_query_tool.py` & `foundationallm-0.7.9/foundationallm/langchain/tools/secure_sql_database_query_tool.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/agents/agent_base.py` & `foundationallm-0.7.9/foundationallm/models/agents/agent_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/agents/agent_vectorization_settings.py` & `foundationallm-0.7.9/foundationallm/models/agents/agent_vectorization_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/agents/knowledge_management_completion_request.py` & `foundationallm-0.7.9/foundationallm/models/agents/knowledge_management_completion_request.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/language_models/embedding_model.py` & `foundationallm-0.7.9/foundationallm/models/language_models/embedding_model.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/orchestration/completion_response.py` & `foundationallm-0.7.9/foundationallm/models/orchestration/completion_response.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/orchestration/orchestration_settings.py` & `foundationallm-0.7.9/foundationallm/models/orchestration/orchestration_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/__init__.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/__init__.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_configuration_references.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_configuration_references.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_embedding_profile.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/embedding_profiles/azure_openai/azure_openai_embedding_profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Classes:   
     AzureAISearchIndexingProfile: An Azure AI Search indexing profile.
 Description:
     Settings specific to the Azure AI Search Indexes
 """
-from typing import Any, Optional
+from typing import Any, Self, Optional
 from foundationallm.models.resource_providers.vectorization import SettingsBase, EmbeddingProfileBase
 from .azure_openai_configuration_references import AzureOpenAIConfigurationReferences
 from foundationallm.models.utils import ObjectUtils
 from foundationallm.langchain.exceptions import LangChainException
 
 class AzureOpenAIEmbeddingProfile(EmbeddingProfileBase):
     """
     An Azure AI Search indexing profile.
     """
     settings: Optional[SettingsBase] = None
     configuration_references: AzureOpenAIConfigurationReferences
 
     @staticmethod
-    def from_object(obj: Any) -> AzureOpenAIEmbeddingProfile:
+    def from_object(obj: Any) -> Self:
 
         text_embedding_profile: AzureOpenAIEmbeddingProfile = None
 
         try:
             text_embedding_profile = AzureOpenAIEmbeddingProfile(**ObjectUtils.translate_keys(obj))
         except Exception as e:
             raise LangChainException(f"The text embedding profile object provided in the agent parameters is invalid. {str(e)}", 400)
```

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_configuration_references.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_configuration_references.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_indexing_profile.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_indexing_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 Classes:
     AzureAISearchSettings: Settings for an Azure AI Search indexing profile.
     AzureAISearchConfigurationReferences: Configuration references for an Azure AI Search indexing profile.
     AzureAISearchIndexingProfile: An Azure AI Search indexing profile.
 Description:
     Settings specific to the Azure AI Search Indexes
 """
-from typing import Any
+from typing import Any, Self
 from foundationallm.models.resource_providers.vectorization import IndexingProfileBase
 from .azure_ai_search_settings import AzureAISearchSettings
 from .azure_ai_search_configuration_references import AzureAISearchConfigurationReferences
 from foundationallm.models.utils import ObjectUtils
 from foundationallm.langchain.exceptions import LangChainException
 
 class AzureAISearchIndexingProfile(IndexingProfileBase):
     """
     An Azure AI Search indexing profile.
     """
     settings: AzureAISearchSettings
     configuration_references: AzureAISearchConfigurationReferences
 
     @staticmethod
-    def from_object(obj: Any) -> AzureAISearchIndexingProfile:
+    def from_object(obj: Any) -> Self:
 
         indexing_profile: AzureAISearchIndexingProfile = None
         
         try:
             indexing_profile = AzureAISearchIndexingProfile(**ObjectUtils.translate_keys(obj))
         except Exception as e:
             raise LangChainException(f"The indexing profile object provided in the agent parameters is invalid. {str(e)}", 400)
```

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_settings.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/indexing_profiles/azure_ai_search/azure_ai_search_settings.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/resource_providers/vectorization/profile_base.py` & `foundationallm-0.7.9/foundationallm/models/resource_providers/vectorization/profile_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/models/utils/object_utils.py` & `foundationallm-0.7.9/foundationallm/models/utils/object_utils.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/storage/blob_storage_manager.py` & `foundationallm-0.7.9/foundationallm/storage/blob_storage_manager.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/storage/storage_manager_base.py` & `foundationallm-0.7.9/foundationallm/storage/storage_manager_base.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm/telemetry/telemetry.py` & `foundationallm-0.7.9/foundationallm/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/foundationallm.egg-info/PKG-INFO` & `foundationallm-0.7.9/foundationallm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundationallm
-Version: 0.7.8
+Version: 0.7.9
 Summary: Enables integration with the FoundationaLLM platform.
 Author-email: FoundationaLLM <dev@foundationallm.ai>
 Project-URL: Homepage, https://foundationallm.ai
 Project-URL: Issues, https://github.com/solliancenet/foundationallm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `foundationallm-0.7.8/foundationallm.egg-info/SOURCES.txt` & `foundationallm-0.7.9/foundationallm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `foundationallm-0.7.8/pyproject.toml` & `foundationallm-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "foundationallm"
-version = "0.7.8"
+version = "0.7.9"
 authors = [
   { name="FoundationaLLM", email="dev@foundationallm.ai" },
 ]
 description = "Enables integration with the FoundationaLLM platform."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

