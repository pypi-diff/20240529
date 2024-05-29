# Comparing `tmp/vellum_ai-0.6.0.tar.gz` & `tmp/vellum_ai-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.6.0.tar", max compression
+gzip compressed data, was "vellum_ai-0.6.1.tar", max compression
```

## Comparing `vellum_ai-0.6.0.tar` & `vellum_ai-0.6.1.tar`

### file list

```diff
@@ -1,434 +1,436 @@
--rw-r--r--   0        0        0     1073 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/LICENSE
--rw-r--r--   0        0        0     2980 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/README.md
--rw-r--r--   0        0        0      632 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    42011 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/__init__.py
--rw-r--r--   0        0        0    97089 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/client.py
--rw-r--r--   0        0        0      853 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1697 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/core/request_options.py
--rw-r--r--   0        0        0      498 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/environment.py
--rw-r--r--   0        0        0      343 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/errors/not_found_error.py
--rw-r--r--   0        0        0       79 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/__init__.py
--rw-r--r--   0        0        0       77 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/__init__.py
--rw-r--r--   0        0        0      116 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/constants.py
--rw-r--r--   0        0        0       56 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/exceptions.py
--rw-r--r--   0        0        0    12323 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/test_suites/resources.py
--rw-r--r--   0        0        0        0 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/__init__.py
--rw-r--r--   0        0        0      298 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/env.py
--rw-r--r--   0        0        0       49 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/exceptions.py
--rw-r--r--   0        0        0      698 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/lib/utils/paginator.py
--rw-r--r--   0        0        0        0 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/py.typed
--rw-r--r--   0        0        0      730 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0      157 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/__init__.py
--rw-r--r--   0        0        0    19588 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/client.py
--rw-r--r--   0        0        0      183 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/types/__init__.py
--rw-r--r--   0        0        0      174 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/deployments/types/deployments_list_request_status.py
--rw-r--r--   0        0        0      165 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/__init__.py
--rw-r--r--   0        0        0    40388 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/client.py
--rw-r--r--   0        0        0      196 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/types/__init__.py
--rw-r--r--   0        0        0      178 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
--rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0    34322 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/folder_entities/__init__.py
--rw-r--r--   0        0        0     6435 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/folder_entities/client.py
--rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0    12738 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/__init__.py
--rw-r--r--   0        0        0    18728 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/client.py
--rw-r--r--   0        0        0       65 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suites/__init__.py
--rw-r--r--   0        0        0    18982 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/test_suites/client.py
--rw-r--r--   0        0        0      173 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/__init__.py
--rw-r--r--   0        0        0    11158 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/client.py
--rw-r--r--   0        0        0      208 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/types/__init__.py
--rw-r--r--   0        0        0      182 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
--rw-r--r--   0        0        0      454 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/__init__.py
--rw-r--r--   0        0        0      473 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/_jsii/__init__.py
--rw-r--r--   0        0        0    15887 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
--rw-r--r--   0        0        0       43 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/constraints.json
--rw-r--r--   0        0        0    21484 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/data_vellum_document_index/__init__.py
--rw-r--r--   0        0        0    25018 2024-05-24 00:54:57.737661 vellum_ai-0.6.0/src/vellum/terraform/document_index/__init__.py
--rw-r--r--   0        0        0    10298 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/provider/__init__.py
--rw-r--r--   0        0        0        1 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/py.typed
--rw-r--r--   0        0        0       56 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/terraform/versions.json
--rw-r--r--   0        0        0    56092 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/__init__.py
--rw-r--r--   0        0        0       92 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/add_openai_api_key_enum.py
--rw-r--r--   0        0        0      983 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/api_node_result.py
--rw-r--r--   0        0        0     1161 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/api_node_result_data.py
--rw-r--r--   0        0        0     1030 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content.py
--rw-r--r--   0        0        0     1297 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item.py
--rw-r--r--   0        0        0     1421 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item_request.py
--rw-r--r--   0        0        0     1059 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_enum.py
--rw-r--r--   0        0        0     2228 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_variable_value_item.py
--rw-r--r--   0        0        0     2166 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/array_vellum_value_item.py
--rw-r--r--   0        0        0     1004 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py
--rw-r--r--   0        0        0     1011 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large_request.py
--rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py
--rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request.py
--rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py
--rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request.py
--rw-r--r--   0        0        0      129 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_history_enum.py
--rw-r--r--   0        0        0     1121 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_history_input_request.py
--rw-r--r--   0        0        0     1213 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0     1573 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_content.py
--rw-r--r--   0        0        0     1737 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_content_request.py
--rw-r--r--   0        0        0     1242 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      182 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0      996 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_array_result.py
--rw-r--r--   0        0        0      967 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_chat_history_result.py
--rw-r--r--   0        0        0      948 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_error_result.py
--rw-r--r--   0        0        0      958 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_function_call_result.py
--rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_json_result.py
--rw-r--r--   0        0        0      905 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_number_result.py
--rw-r--r--   0        0        0     1034 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result.py
--rw-r--r--   0        0        0     1016 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_data.py
--rw-r--r--   0        0        0     3377 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_output.py
--rw-r--r--   0        0        0      972 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_search_results_result.py
--rw-r--r--   0        0        0      903 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/code_execution_node_string_result.py
--rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/conditional_node_result.py
--rw-r--r--   0        0        0      898 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/conditional_node_result_data.py
--rw-r--r--   0        0        0      898 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/deployment_provider_payload_response.py
--rw-r--r--   0        0        0     1938 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/deployment_read.py
--rw-r--r--   0        0        0     1532 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1383 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_chunking.py
--rw-r--r--   0        0        0     1498 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_chunking_request.py
--rw-r--r--   0        0        0     1075 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config.py
--rw-r--r--   0        0        0     1126 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config_request.py
--rw-r--r--   0        0        0     1753 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_index_read.py
--rw-r--r--   0        0        0     2200 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_read.py
--rw-r--r--   0        0        0      122 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/document_status.py
--rw-r--r--   0        0        0     2108 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      158 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/entity_status.py
--rw-r--r--   0        0        0      179 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/environment_enum.py
--rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_enum.py
--rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_variable_value.py
--rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/error_vellum_value.py
--rw-r--r--   0        0        0      948 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_api_error_response.py
--rw-r--r--   0        0        0     1636 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_event.py
--rw-r--r--   0        0        0      914 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_prompt_response.py
--rw-r--r--   0        0        0      947 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_error_response.py
--rw-r--r--   0        0        0     1085 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_response.py
--rw-r--r--   0        0        0      953 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_stream_error_response.py
--rw-r--r--   0        0        0     1067 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1099 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_array_vellum_value.py
--rw-r--r--   0        0        0     1070 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_chat_history_vellum_value.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_error_vellum_value.py
--rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_function_call_vellum_value.py
--rw-r--r--   0        0        0     1029 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_json_vellum_value.py
--rw-r--r--   0        0        0     1008 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_number_vellum_value.py
--rw-r--r--   0        0        0     1075 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_search_results_vellum_value.py
--rw-r--r--   0        0        0     1006 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_string_vellum_value.py
--rw-r--r--   0        0        0     3144 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/execution_vellum_value.py
--rw-r--r--   0        0        0     1125 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/external_test_case_execution.py
--rw-r--r--   0        0        0     1154 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/external_test_case_execution_request.py
--rw-r--r--   0        0        0      169 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      124 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_enum.py
--rw-r--r--   0        0        0     1235 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_event.py
--rw-r--r--   0        0        0     1457 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_response.py
--rw-r--r--   0        0        0     1089 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1228 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_prompt_execution_meta.py
--rw-r--r--   0        0        0     1373 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/fulfilled_workflow_node_result_event.py
--rw-r--r--   0        0        0     1081 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call.py
--rw-r--r--   0        0        0     1065 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content.py
--rw-r--r--   0        0        0     1094 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_request.py
--rw-r--r--   0        0        0     1013 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value.py
--rw-r--r--   0        0        0     1020 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value_request.py
--rw-r--r--   0        0        0      131 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_enum.py
--rw-r--r--   0        0        0     1088 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_request.py
--rw-r--r--   0        0        0      936 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_variable_value.py
--rw-r--r--   0        0        0      993 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/function_call_vellum_value.py
--rw-r--r--   0        0        0      940 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0     1079 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1572 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1342 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1394 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0     1087 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      949 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0      934 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_response.py
--rw-r--r--   0        0        0     1101 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_result.py
--rw-r--r--   0        0        0      991 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/generate_stream_result_data.py
--rw-r--r--   0        0        0      144 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_enum.py
--rw-r--r--   0        0        0     1017 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer.py
--rw-r--r--   0        0        0     1046 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer_request.py
--rw-r--r--   0        0        0      975 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_chat_message_content.py
--rw-r--r--   0        0        0     1004 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_chat_message_content_request.py
--rw-r--r--   0        0        0      116 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_enum.py
--rw-r--r--   0        0        0     1000 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_variable_value.py
--rw-r--r--   0        0        0      998 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/image_vellum_value.py
--rw-r--r--   0        0        0     3802 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer.py
--rw-r--r--   0        0        0     4061 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer_request.py
--rw-r--r--   0        0        0      213 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      124 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_enum.py
--rw-r--r--   0        0        0     1134 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_execute_prompt_event.py
--rw-r--r--   0        0        0     1181 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_prompt_execution_meta.py
--rw-r--r--   0        0        0     1377 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/initiated_workflow_node_result_event.py
--rw-r--r--   0        0        0     1025 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config.py
--rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config_request.py
--rw-r--r--   0        0        0      163 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/intfloat_multilingual_e_5_large_enum.py
--rw-r--r--   0        0        0      114 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_enum.py
--rw-r--r--   0        0        0     1048 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_input_request.py
--rw-r--r--   0        0        0      904 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_variable_value.py
--rw-r--r--   0        0        0      959 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/json_vellum_value.py
--rw-r--r--   0        0        0      487 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/logical_operator.py
--rw-r--r--   0        0        0      151 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0     1355 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_config_request.py
--rw-r--r--   0        0        0      165 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_combinator.py
--rw-r--r--   0        0        0     1371 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_request.py
--rw-r--r--   0        0        0      118 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metric_enum.py
--rw-r--r--   0        0        0      907 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/metric_node_result.py
--rw-r--r--   0        0        0     1086 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/ml_model_usage.py
--rw-r--r--   0        0        0     1098 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1043 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_request.py
--rw-r--r--   0        0        0     1006 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_scenario_input_string_variable_value_request.py
--rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1073 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py
--rw-r--r--   0        0        0     1018 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value.py
--rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value_request.py
--rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1065 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value_request.py
--rw-r--r--   0        0        0      995 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value.py
--rw-r--r--   0        0        0     1002 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value_request.py
--rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value.py
--rw-r--r--   0        0        0      983 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value_request.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value.py
--rw-r--r--   0        0        0     1080 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value_request.py
--rw-r--r--   0        0        0      974 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value.py
--rw-r--r--   0        0        0      981 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value_request.py
--rw-r--r--   0        0        0     3021 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value.py
--rw-r--r--   0        0        0     3280 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value_request.py
--rw-r--r--   0        0        0     1019 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_array_value.py
--rw-r--r--   0        0        0      990 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_chat_history_value.py
--rw-r--r--   0        0        0      971 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_error_value.py
--rw-r--r--   0        0        0      976 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_function_call.py
--rw-r--r--   0        0        0      949 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_json_value.py
--rw-r--r--   0        0        0      928 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_number_value.py
--rw-r--r--   0        0        0      995 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_search_results_value.py
--rw-r--r--   0        0        0      926 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_compiled_string_value.py
--rw-r--r--   0        0        0     3354 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_input_variable_compiled_value.py
--rw-r--r--   0        0        0     1214 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_array_value.py
--rw-r--r--   0        0        0     1198 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_chat_history_value.py
--rw-r--r--   0        0        0     1172 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_error_value.py
--rw-r--r--   0        0        0     1190 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_function_call_value.py
--rw-r--r--   0        0        0     1149 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_json_value.py
--rw-r--r--   0        0        0     1130 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_number_value.py
--rw-r--r--   0        0        0     1205 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_search_results_value.py
--rw-r--r--   0        0        0     1128 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_string_value.py
--rw-r--r--   0        0        0     3275 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/node_output_compiled_value.py
--rw-r--r--   0        0        0     1000 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0     1008 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      118 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_enum.py
--rw-r--r--   0        0        0      883 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_variable_value.py
--rw-r--r--   0        0        0      933 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/number_vellum_value.py
--rw-r--r--   0        0        0     1037 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config.py
--rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config_request.py
--rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large_request.py
--rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small_request.py
--rw-r--r--   0        0        0     1022 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002_request.py
--rw-r--r--   0        0        0     1091 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_document_index_read_list.py
--rw-r--r--   0        0        0     1095 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_deployment_read_list.py
--rw-r--r--   0        0        0     1070 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0     1111 2024-05-24 00:54:57.741661 vellum_ai-0.6.0/src/vellum/types/paginated_slim_workflow_deployment_list.py
--rw-r--r--   0        0        0     1060 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_run_execution_list.py
--rw-r--r--   0        0        0     1044 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_test_case_list.py
--rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/processing_failure_reason_enum.py
--rw-r--r--   0        0        0      190 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0     2044 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py
--rw-r--r--   0        0        0     1233 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_deployment_input_request.py
--rw-r--r--   0        0        0     1370 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_execution_meta.py
--rw-r--r--   0        0        0      997 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_node_result.py
--rw-r--r--   0        0        0      988 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_node_result_data.py
--rw-r--r--   0        0        0     1418 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/prompt_output.py
--rw-r--r--   0        0        0     1210 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/raw_prompt_execution_overrides_request.py
--rw-r--r--   0        0        0      948 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config.py
--rw-r--r--   0        0        0      955 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config_request.py
--rw-r--r--   0        0        0      135 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunker_enum.py
--rw-r--r--   0        0        0      998 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunking.py
--rw-r--r--   0        0        0     1027 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/reducto_chunking_request.py
--rw-r--r--   0        0        0      122 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_enum.py
--rw-r--r--   0        0        0     1159 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_event.py
--rw-r--r--   0        0        0     1417 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_response.py
--rw-r--r--   0        0        0     1103 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1138 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_prompt_execution_meta.py
--rw-r--r--   0        0        0     1293 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/rejected_workflow_node_result_event.py
--rw-r--r--   0        0        0     1144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0      907 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input.py
--rw-r--r--   0        0        0     1071 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input_chat_history_variable_value.py
--rw-r--r--   0        0        0     1001 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/scenario_input_string_variable_value.py
--rw-r--r--   0        0        0      938 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0     1218 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0      997 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_node_result.py
--rw-r--r--   0        0        0     1143 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_node_result_data.py
--rw-r--r--   0        0        0     1622 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1304 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result.py
--rw-r--r--   0        0        0     1437 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_document.py
--rw-r--r--   0        0        0     1365 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_document_request.py
--rw-r--r--   0        0        0      972 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0     1333 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_result_request.py
--rw-r--r--   0        0        0      133 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_results_enum.py
--rw-r--r--   0        0        0     1128 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     1003 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config.py
--rw-r--r--   0        0        0     1010 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config_request.py
--rw-r--r--   0        0        0      137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunker_enum.py
--rw-r--r--   0        0        0     1003 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunking.py
--rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_chunking_request.py
--rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_cos_v_1_enum.py
--rw-r--r--   0        0        0      195 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_dot_v_1_enum.py
--rw-r--r--   0        0        0     1753 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_deployment_read.py
--rw-r--r--   0        0        0     2975 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0     2104 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/slim_workflow_deployment.py
--rw-r--r--   0        0        0      124 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_enum.py
--rw-r--r--   0        0        0     1388 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_execute_prompt_event.py
--rw-r--r--   0        0        0     1030 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_prompt_execution_meta.py
--rw-r--r--   0        0        0     1383 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/streaming_workflow_node_result_event.py
--rw-r--r--   0        0        0      930 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_chat_message_content.py
--rw-r--r--   0        0        0      937 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_chat_message_content_request.py
--rw-r--r--   0        0        0      118 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_enum.py
--rw-r--r--   0        0        0     1026 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_input_request.py
--rw-r--r--   0        0        0      881 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_variable_value.py
--rw-r--r--   0        0        0      931 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/string_vellum_value.py
--rw-r--r--   0        0        0     1825 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      875 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0     1487 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/submit_workflow_execution_actual_request.py
--rw-r--r--   0        0        0      128 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/subworkflow_enum.py
--rw-r--r--   0        0        0      917 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/subworkflow_node_result.py
--rw-r--r--   0        0        0      993 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_array_result.py
--rw-r--r--   0        0        0      964 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_chat_history_result.py
--rw-r--r--   0        0        0      945 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_error_result.py
--rw-r--r--   0        0        0      955 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_function_call_result.py
--rw-r--r--   0        0        0      923 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_json_result.py
--rw-r--r--   0        0        0      902 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_number_result.py
--rw-r--r--   0        0        0     1017 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result.py
--rw-r--r--   0        0        0      956 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result_data.py
--rw-r--r--   0        0        0     3246 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_result_output.py
--rw-r--r--   0        0        0      969 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_search_results_result.py
--rw-r--r--   0        0        0      900 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/templating_node_string_result.py
--rw-r--r--   0        0        0     1142 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_array_result.py
--rw-r--r--   0        0        0     1113 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_chat_history_result.py
--rw-r--r--   0        0        0     1094 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_error_result.py
--rw-r--r--   0        0        0     1104 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_function_call_result.py
--rw-r--r--   0        0        0     1072 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_json_result.py
--rw-r--r--   0        0        0     1051 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_number_result.py
--rw-r--r--   0        0        0     1007 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result.py
--rw-r--r--   0        0        0      948 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result_data.py
--rw-r--r--   0        0        0     3164 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_result_output.py
--rw-r--r--   0        0        0     1118 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_search_results_result.py
--rw-r--r--   0        0        0     1049 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/terminal_node_string_result.py
--rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0     1036 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_error_variable_value.py
--rw-r--r--   0        0        0     1053 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_function_call_variable_value.py
--rw-r--r--   0        0        0     1012 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_json_variable_value.py
--rw-r--r--   0        0        0      996 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_number_variable_value.py
--rw-r--r--   0        0        0     1068 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_search_results_variable_value.py
--rw-r--r--   0        0        0      991 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_string_variable_value.py
--rw-r--r--   0        0        0     2834 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_case_variable_value.py
--rw-r--r--   0        0        0     1373 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
--rw-r--r--   0        0        0     1228 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1235 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1411 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      174 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1483 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config.py
--rw-r--r--   0        0        0     1598 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config_request.py
--rw-r--r--   0        0        0     1158 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution.py
--rw-r--r--   0        0        0     1115 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_chat_history_output.py
--rw-r--r--   0        0        0     1089 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_error_output.py
--rw-r--r--   0        0        0     1107 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_function_call_output.py
--rw-r--r--   0        0        0     1066 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_json_output.py
--rw-r--r--   0        0        0      973 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_definition.py
--rw-r--r--   0        0        0     1218 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_result.py
--rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_number_output.py
--rw-r--r--   0        0        0     3057 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_output.py
--rw-r--r--   0        0        0     1122 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_search_results_output.py
--rw-r--r--   0        0        0     1045 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_string_output.py
--rw-r--r--   0        0        0     1331 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config.py
--rw-r--r--   0        0        0     1115 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data.py
--rw-r--r--   0        0        0     1144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py
--rw-r--r--   0        0        0     1360 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_request.py
--rw-r--r--   0        0        0      148 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
--rw-r--r--   0        0        0     1005 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output.py
--rw-r--r--   0        0        0      144 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
--rw-r--r--   0        0        0      963 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output.py
--rw-r--r--   0        0        0      146 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
--rw-r--r--   0        0        0     1291 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_output.py
--rw-r--r--   0        0        0      961 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output.py
--rw-r--r--   0        0        0      146 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
--rw-r--r--   0        0        0     1500 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_read.py
--rw-r--r--   0        0        0      197 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_state.py
--rw-r--r--   0        0        0      896 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_test_suite.py
--rw-r--r--   0        0        0     1367 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
--rw-r--r--   0        0        0     1241 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
--rw-r--r--   0        0        0     1248 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
--rw-r--r--   0        0        0     1405 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
--rw-r--r--   0        0        0      170 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
--rw-r--r--   0        0        0     1086 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/test_suite_test_case.py
--rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_3_large_enum.py
--rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_3_small_enum.py
--rw-r--r--   0        0        0      147 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/text_embedding_ada_002_enum.py
--rw-r--r--   0        0        0     1025 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config.py
--rw-r--r--   0        0        0     1032 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config_request.py
--rw-r--r--   0        0        0      167 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_enum.py
--rw-r--r--   0        0        0     1077 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking.py
--rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking_request.py
--rw-r--r--   0        0        0      866 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      946 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      937 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error.py
--rw-r--r--   0        0        0      233 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error_code_enum.py
--rw-r--r--   0        0        0      944 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_error_request.py
--rw-r--r--   0        0        0      914 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_image.py
--rw-r--r--   0        0        0      921 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_image_request.py
--rw-r--r--   0        0        0      944 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_variable.py
--rw-r--r--   0        0        0      281 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/vellum_variable_type.py
--rw-r--r--   0        0        0     2110 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_deployment_read.py
--rw-r--r--   0        0        0      981 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_event_error.py
--rw-r--r--   0        0        0     2223 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_chat_history_request.py
--rw-r--r--   0        0        0     2160 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_json_request.py
--rw-r--r--   0        0        0     2137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_string_request.py
--rw-r--r--   0        0        0      425 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_event_error_code.py
--rw-r--r--   0        0        0      170 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_event_type.py
--rw-r--r--   0        0        0     1139 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_node_result_event.py
--rw-r--r--   0        0        0     1134 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_execution_workflow_result_event.py
--rw-r--r--   0        0        0     3299 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_data.py
--rw-r--r--   0        0        0     1745 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event.py
--rw-r--r--   0        0        0      209 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event_state.py
--rw-r--r--   0        0        0     3212 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output.py
--rw-r--r--   0        0        0     1148 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_array.py
--rw-r--r--   0        0        0     1131 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_chat_history.py
--rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_error.py
--rw-r--r--   0        0        0     1123 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_function_call.py
--rw-r--r--   0        0        0     1106 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_image.py
--rw-r--r--   0        0        0     1082 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_json.py
--rw-r--r--   0        0        0     1063 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_number.py
--rw-r--r--   0        0        0     1138 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_search_results.py
--rw-r--r--   0        0        0     1061 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_output_string.py
--rw-r--r--   0        0        0     1137 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_chat_history_input_request.py
--rw-r--r--   0        0        0     1772 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_input_request.py
--rw-r--r--   0        0        0     1066 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_json_input_request.py
--rw-r--r--   0        0        0     1047 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_number_input_request.py
--rw-r--r--   0        0        0     1045 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_request_string_input_request.py
--rw-r--r--   0        0        0     1475 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event.py
--rw-r--r--   0        0        0     3529 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data.py
--rw-r--r--   0        0        0     1423 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_array.py
--rw-r--r--   0        0        0     1400 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_chat_history.py
--rw-r--r--   0        0        0     1375 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_error.py
--rw-r--r--   0        0        0     1392 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_function_call.py
--rw-r--r--   0        0        0     1351 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_json.py
--rw-r--r--   0        0        0     1332 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_number.py
--rw-r--r--   0        0        0     1407 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_search_results.py
--rw-r--r--   0        0        0     1482 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_string.py
--rw-r--r--   0        0        0      911 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/types/workflow_stream_event.py
--rw-r--r--   0        0        0       77 2024-05-24 00:54:57.745661 vellum_ai-0.6.0/src/vellum/version.py
--rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 vellum_ai-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3022 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/README.md
+-rw-r--r--   0        0        0      632 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    42157 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/__init__.py
+-rw-r--r--   0        0        0    97089 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/client.py
+-rw-r--r--   0        0        0      853 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1697 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      329 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/pydantic_utilities.py
+-rw-r--r--   0        0        0      330 2024-05-29 20:53:45.757509 vellum_ai-0.6.1/src/vellum/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/core/request_options.py
+-rw-r--r--   0        0        0      498 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/environment.py
+-rw-r--r--   0        0        0      343 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/errors/not_found_error.py
+-rw-r--r--   0        0        0       79 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/test_suites/__init__.py
+-rw-r--r--   0        0        0      116 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/test_suites/constants.py
+-rw-r--r--   0        0        0       56 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/test_suites/exceptions.py
+-rw-r--r--   0        0        0    12323 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/test_suites/resources.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/utils/__init__.py
+-rw-r--r--   0        0        0      298 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/utils/env.py
+-rw-r--r--   0        0        0       49 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/utils/exceptions.py
+-rw-r--r--   0        0        0      698 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/lib/utils/paginator.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/py.typed
+-rw-r--r--   0        0        0      730 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      157 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/deployments/__init__.py
+-rw-r--r--   0        0        0    19588 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/deployments/client.py
+-rw-r--r--   0        0        0      183 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/deployments/types/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/deployments/types/deployments_list_request_status.py
+-rw-r--r--   0        0        0      165 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/document_indexes/__init__.py
+-rw-r--r--   0        0        0    40388 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/document_indexes/client.py
+-rw-r--r--   0        0        0      196 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/document_indexes/types/__init__.py
+-rw-r--r--   0        0        0      178 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/document_indexes/types/document_indexes_list_request_status.py
+-rw-r--r--   0        0        0       65 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0    34322 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/folder_entities/__init__.py
+-rw-r--r--   0        0        0     6435 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/folder_entities/client.py
+-rw-r--r--   0        0        0       65 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0    12738 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0       65 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/test_suite_runs/__init__.py
+-rw-r--r--   0        0        0    18728 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/test_suite_runs/client.py
+-rw-r--r--   0        0        0       65 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/test_suites/__init__.py
+-rw-r--r--   0        0        0    18982 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/test_suites/client.py
+-rw-r--r--   0        0        0      173 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/workflow_deployments/__init__.py
+-rw-r--r--   0        0        0    11158 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/workflow_deployments/client.py
+-rw-r--r--   0        0        0      208 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/workflow_deployments/types/__init__.py
+-rw-r--r--   0        0        0      182 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
+-rw-r--r--   0        0        0      454 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/_jsii/__init__.py
+-rw-r--r--   0        0        0    15887 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz
+-rw-r--r--   0        0        0       43 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/constraints.json
+-rw-r--r--   0        0        0    21484 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/data_vellum_document_index/__init__.py
+-rw-r--r--   0        0        0    25018 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/document_index/__init__.py
+-rw-r--r--   0        0        0    10298 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/provider/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/py.typed
+-rw-r--r--   0        0        0       56 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/terraform/versions.json
+-rw-r--r--   0        0        0    56283 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0       92 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/add_openai_api_key_enum.py
+-rw-r--r--   0        0        0      983 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/api_node_result.py
+-rw-r--r--   0        0        0     1161 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/api_node_result_data.py
+-rw-r--r--   0        0        0     1030 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_chat_message_content.py
+-rw-r--r--   0        0        0     1297 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_item.py
+-rw-r--r--   0        0        0     1421 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_item_request.py
+-rw-r--r--   0        0        0     1059 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_enum.py
+-rw-r--r--   0        0        0     2228 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_variable_value_item.py
+-rw-r--r--   0        0        0     2166 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/array_vellum_value_item.py
+-rw-r--r--   0        0        0     1004 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py
+-rw-r--r--   0        0        0     1011 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large_request.py
+-rw-r--r--   0        0        0     1036 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py
+-rw-r--r--   0        0        0     1043 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request.py
+-rw-r--r--   0        0        0     1036 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py
+-rw-r--r--   0        0        0     1043 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request.py
+-rw-r--r--   0        0        0      129 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_history_enum.py
+-rw-r--r--   0        0        0     1121 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_history_input_request.py
+-rw-r--r--   0        0        0     1213 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0     1573 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_message_content.py
+-rw-r--r--   0        0        0     1737 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_message_content_request.py
+-rw-r--r--   0        0        0     1242 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      182 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0      996 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_array_result.py
+-rw-r--r--   0        0        0      967 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_chat_history_result.py
+-rw-r--r--   0        0        0      948 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_error_result.py
+-rw-r--r--   0        0        0      958 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_function_call_result.py
+-rw-r--r--   0        0        0      926 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_json_result.py
+-rw-r--r--   0        0        0      905 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_number_result.py
+-rw-r--r--   0        0        0     1034 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_result.py
+-rw-r--r--   0        0        0     1016 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_result_data.py
+-rw-r--r--   0        0        0     3377 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_result_output.py
+-rw-r--r--   0        0        0      972 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_search_results_result.py
+-rw-r--r--   0        0        0      903 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/code_execution_node_string_result.py
+-rw-r--r--   0        0        0     1022 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/conditional_node_result.py
+-rw-r--r--   0        0        0      898 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/conditional_node_result_data.py
+-rw-r--r--   0        0        0      898 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/deployment_provider_payload_response.py
+-rw-r--r--   0        0        0     1938 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/deployment_read.py
+-rw-r--r--   0        0        0     1532 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1383 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_index_chunking.py
+-rw-r--r--   0        0        0     1498 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_index_chunking_request.py
+-rw-r--r--   0        0        0     1075 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_index_indexing_config.py
+-rw-r--r--   0        0        0     1126 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_index_indexing_config_request.py
+-rw-r--r--   0        0        0     1753 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_index_read.py
+-rw-r--r--   0        0        0     2200 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_read.py
+-rw-r--r--   0        0        0      122 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/document_status.py
+-rw-r--r--   0        0        0     2108 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      158 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/entity_status.py
+-rw-r--r--   0        0        0      179 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/environment_enum.py
+-rw-r--r--   0        0        0      116 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/error_enum.py
+-rw-r--r--   0        0        0      926 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/error_variable_value.py
+-rw-r--r--   0        0        0      976 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/error_vellum_value.py
+-rw-r--r--   0        0        0      948 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_prompt_api_error_response.py
+-rw-r--r--   0        0        0     1636 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_prompt_event.py
+-rw-r--r--   0        0        0      914 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_prompt_response.py
+-rw-r--r--   0        0        0      947 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_workflow_error_response.py
+-rw-r--r--   0        0        0     1085 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_workflow_response.py
+-rw-r--r--   0        0        0      953 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_workflow_stream_error_response.py
+-rw-r--r--   0        0        0     1067 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1099 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_array_vellum_value.py
+-rw-r--r--   0        0        0     1070 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_chat_history_vellum_value.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_error_vellum_value.py
+-rw-r--r--   0        0        0     1061 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_function_call_vellum_value.py
+-rw-r--r--   0        0        0     1029 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_json_vellum_value.py
+-rw-r--r--   0        0        0     1008 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_number_vellum_value.py
+-rw-r--r--   0        0        0     1075 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_search_results_vellum_value.py
+-rw-r--r--   0        0        0     1006 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_string_vellum_value.py
+-rw-r--r--   0        0        0     3144 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/execution_vellum_value.py
+-rw-r--r--   0        0        0     1125 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/external_test_case_execution.py
+-rw-r--r--   0        0        0     1154 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/external_test_case_execution_request.py
+-rw-r--r--   0        0        0      169 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      124 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_enum.py
+-rw-r--r--   0        0        0     1235 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_prompt_event.py
+-rw-r--r--   0        0        0     1457 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_prompt_response.py
+-rw-r--r--   0        0        0     1089 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1228 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1373 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/fulfilled_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1081 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/function_call.py
+-rw-r--r--   0        0        0     1065 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content.py
+-rw-r--r--   0        0        0     1094 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_request.py
+-rw-r--r--   0        0        0     1013 2024-05-29 20:53:45.761509 vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_value.py
+-rw-r--r--   0        0        0     1020 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_value_request.py
+-rw-r--r--   0        0        0      131 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/function_call_enum.py
+-rw-r--r--   0        0        0     1088 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/function_call_request.py
+-rw-r--r--   0        0        0      936 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/function_call_variable_value.py
+-rw-r--r--   0        0        0      993 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/function_call_vellum_value.py
+-rw-r--r--   0        0        0      940 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0     1079 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1572 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1342 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1394 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0     1087 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      949 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      934 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_stream_response.py
+-rw-r--r--   0        0        0     1101 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_stream_result.py
+-rw-r--r--   0        0        0      991 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/generate_stream_result_data.py
+-rw-r--r--   0        0        0      144 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/hkunlp_instructor_xl_enum.py
+-rw-r--r--   0        0        0     1017 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/hkunlp_instructor_xl_vectorizer.py
+-rw-r--r--   0        0        0     1046 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/hkunlp_instructor_xl_vectorizer_request.py
+-rw-r--r--   0        0        0      975 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/image_chat_message_content.py
+-rw-r--r--   0        0        0     1004 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/image_chat_message_content_request.py
+-rw-r--r--   0        0        0      116 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/image_enum.py
+-rw-r--r--   0        0        0     1000 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/image_variable_value.py
+-rw-r--r--   0        0        0      998 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/image_vellum_value.py
+-rw-r--r--   0        0        0     3802 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/indexing_config_vectorizer.py
+-rw-r--r--   0        0        0     4061 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/indexing_config_vectorizer_request.py
+-rw-r--r--   0        0        0      213 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      124 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/initiated_enum.py
+-rw-r--r--   0        0        0     1134 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/initiated_execute_prompt_event.py
+-rw-r--r--   0        0        0     1181 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/initiated_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1377 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/initiated_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1025 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/instructor_vectorizer_config.py
+-rw-r--r--   0        0        0     1032 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/instructor_vectorizer_config_request.py
+-rw-r--r--   0        0        0      163 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/intfloat_multilingual_e_5_large_enum.py
+-rw-r--r--   0        0        0      114 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/json_enum.py
+-rw-r--r--   0        0        0     1048 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/json_input_request.py
+-rw-r--r--   0        0        0      904 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/json_variable_value.py
+-rw-r--r--   0        0        0      959 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/json_vellum_value.py
+-rw-r--r--   0        0        0      487 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/logical_operator.py
+-rw-r--r--   0        0        0      151 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0      116 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/merge_enum.py
+-rw-r--r--   0        0        0      905 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/merge_node_result.py
+-rw-r--r--   0        0        0     1355 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/metadata_filter_config_request.py
+-rw-r--r--   0        0        0      165 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/metadata_filter_rule_combinator.py
+-rw-r--r--   0        0        0     1371 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/metadata_filter_rule_request.py
+-rw-r--r--   0        0        0      118 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/metric_enum.py
+-rw-r--r--   0        0        0      907 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/metric_node_result.py
+-rw-r--r--   0        0        0     1086 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/ml_model_usage.py
+-rw-r--r--   0        0        0     1098 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1043 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_scenario_input_request.py
+-rw-r--r--   0        0        0     1006 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_scenario_input_string_variable_value_request.py
+-rw-r--r--   0        0        0     1044 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1073 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0     1018 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1047 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_error_variable_value_request.py
+-rw-r--r--   0        0        0     1036 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1065 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_function_call_variable_value_request.py
+-rw-r--r--   0        0        0      995 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_json_variable_value.py
+-rw-r--r--   0        0        0     1002 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_json_variable_value_request.py
+-rw-r--r--   0        0        0      976 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_number_variable_value.py
+-rw-r--r--   0        0        0      983 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_number_variable_value_request.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0     1080 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_search_results_variable_value_request.py
+-rw-r--r--   0        0        0      974 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_string_variable_value.py
+-rw-r--r--   0        0        0      981 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_string_variable_value_request.py
+-rw-r--r--   0        0        0     3021 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_variable_value.py
+-rw-r--r--   0        0        0     3280 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/named_test_case_variable_value_request.py
+-rw-r--r--   0        0        0     1019 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_array_value.py
+-rw-r--r--   0        0        0      990 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      971 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_error_value.py
+-rw-r--r--   0        0        0      976 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_function_call.py
+-rw-r--r--   0        0        0      949 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_json_value.py
+-rw-r--r--   0        0        0      928 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_number_value.py
+-rw-r--r--   0        0        0      995 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_search_results_value.py
+-rw-r--r--   0        0        0      926 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_compiled_string_value.py
+-rw-r--r--   0        0        0     3354 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_input_variable_compiled_value.py
+-rw-r--r--   0        0        0     1214 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_array_value.py
+-rw-r--r--   0        0        0     1198 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_chat_history_value.py
+-rw-r--r--   0        0        0     1172 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_error_value.py
+-rw-r--r--   0        0        0     1190 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_function_call_value.py
+-rw-r--r--   0        0        0     1149 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_json_value.py
+-rw-r--r--   0        0        0     1130 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_number_value.py
+-rw-r--r--   0        0        0     1205 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_search_results_value.py
+-rw-r--r--   0        0        0     1128 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_string_value.py
+-rw-r--r--   0        0        0     3275 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/node_output_compiled_value.py
+-rw-r--r--   0        0        0     1000 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0     1008 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      118 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/number_enum.py
+-rw-r--r--   0        0        0      883 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/number_variable_value.py
+-rw-r--r--   0        0        0      933 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/number_vellum_value.py
+-rw-r--r--   0        0        0     1037 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_config.py
+-rw-r--r--   0        0        0     1044 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_config_request.py
+-rw-r--r--   0        0        0     1022 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_large.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_large_request.py
+-rw-r--r--   0        0        0     1022 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_small.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_small_request.py
+-rw-r--r--   0        0        0     1022 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002_request.py
+-rw-r--r--   0        0        0     1091 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_document_index_read_list.py
+-rw-r--r--   0        0        0     1095 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_slim_deployment_read_list.py
+-rw-r--r--   0        0        0     1070 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0     1111 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_slim_workflow_deployment_list.py
+-rw-r--r--   0        0        0     1060 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_test_suite_run_execution_list.py
+-rw-r--r--   0        0        0     1044 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/paginated_test_suite_test_case_list.py
+-rw-r--r--   0        0        0      195 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/processing_failure_reason_enum.py
+-rw-r--r--   0        0        0      190 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0     2044 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_deployment_expand_meta_request_request.py
+-rw-r--r--   0        0        0     1233 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_deployment_input_request.py
+-rw-r--r--   0        0        0     1370 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_execution_meta.py
+-rw-r--r--   0        0        0      997 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_node_result.py
+-rw-r--r--   0        0        0      988 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_node_result_data.py
+-rw-r--r--   0        0        0     1418 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/prompt_output.py
+-rw-r--r--   0        0        0     1210 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/raw_prompt_execution_overrides_request.py
+-rw-r--r--   0        0        0      948 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/reducto_chunker_config.py
+-rw-r--r--   0        0        0      955 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/reducto_chunker_config_request.py
+-rw-r--r--   0        0        0      135 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/reducto_chunker_enum.py
+-rw-r--r--   0        0        0      998 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/reducto_chunking.py
+-rw-r--r--   0        0        0     1027 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/reducto_chunking_request.py
+-rw-r--r--   0        0        0      122 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_enum.py
+-rw-r--r--   0        0        0     1159 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_execute_prompt_event.py
+-rw-r--r--   0        0        0     1417 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_execute_prompt_response.py
+-rw-r--r--   0        0        0     1103 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1138 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1293 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/rejected_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1144 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0      907 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/scenario_input.py
+-rw-r--r--   0        0        0     1071 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/scenario_input_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1001 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/scenario_input_string_variable_value.py
+-rw-r--r--   0        0        0      938 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0     1218 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0      997 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_node_result.py
+-rw-r--r--   0        0        0     1143 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_node_result_data.py
+-rw-r--r--   0        0        0     1622 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0     1047 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1304 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0     1466 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_result_document.py
+-rw-r--r--   0        0        0     1473 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_result_document_request.py
+-rw-r--r--   0        0        0      972 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0     1333 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_result_request.py
+-rw-r--r--   0        0        0      133 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_results_enum.py
+-rw-r--r--   0        0        0     1128 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     1003 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_chunker_config.py
+-rw-r--r--   0        0        0     1010 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_chunker_config_request.py
+-rw-r--r--   0        0        0      137 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_chunker_enum.py
+-rw-r--r--   0        0        0     1003 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_chunking.py
+-rw-r--r--   0        0        0     1032 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_chunking_request.py
+-rw-r--r--   0        0        0      195 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_cos_v_1_enum.py
+-rw-r--r--   0        0        0      195 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/sentence_transformers_multi_qa_mpnet_base_dot_v_1_enum.py
+-rw-r--r--   0        0        0     1753 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/slim_deployment_read.py
+-rw-r--r--   0        0        0     2975 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0     2104 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/slim_workflow_deployment.py
+-rw-r--r--   0        0        0      124 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/streaming_enum.py
+-rw-r--r--   0        0        0     1388 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/streaming_execute_prompt_event.py
+-rw-r--r--   0        0        0     1030 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/streaming_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1383 2024-05-29 20:53:45.765509 vellum_ai-0.6.1/src/vellum/types/streaming_workflow_node_result_event.py
+-rw-r--r--   0        0        0      930 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_chat_message_content.py
+-rw-r--r--   0        0        0      937 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_chat_message_content_request.py
+-rw-r--r--   0        0        0      118 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_enum.py
+-rw-r--r--   0        0        0     1026 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_input_request.py
+-rw-r--r--   0        0        0      881 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_variable_value.py
+-rw-r--r--   0        0        0      931 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/string_vellum_value.py
+-rw-r--r--   0        0        0     2010 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      875 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0     1487 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/submit_workflow_execution_actual_request.py
+-rw-r--r--   0        0        0      128 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/subworkflow_enum.py
+-rw-r--r--   0        0        0      917 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/subworkflow_node_result.py
+-rw-r--r--   0        0        0      993 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_array_result.py
+-rw-r--r--   0        0        0      964 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_chat_history_result.py
+-rw-r--r--   0        0        0      945 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_error_result.py
+-rw-r--r--   0        0        0      955 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_function_call_result.py
+-rw-r--r--   0        0        0      923 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_json_result.py
+-rw-r--r--   0        0        0      902 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_number_result.py
+-rw-r--r--   0        0        0     1017 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_result.py
+-rw-r--r--   0        0        0      956 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_result_data.py
+-rw-r--r--   0        0        0     3246 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_result_output.py
+-rw-r--r--   0        0        0      969 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_search_results_result.py
+-rw-r--r--   0        0        0      900 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/templating_node_string_result.py
+-rw-r--r--   0        0        0     1142 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_array_result.py
+-rw-r--r--   0        0        0     1113 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_chat_history_result.py
+-rw-r--r--   0        0        0     1094 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_error_result.py
+-rw-r--r--   0        0        0     1104 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_function_call_result.py
+-rw-r--r--   0        0        0     1072 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_json_result.py
+-rw-r--r--   0        0        0     1051 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_number_result.py
+-rw-r--r--   0        0        0     1007 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_result.py
+-rw-r--r--   0        0        0      948 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_result_data.py
+-rw-r--r--   0        0        0     3164 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_result_output.py
+-rw-r--r--   0        0        0     1118 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_search_results_result.py
+-rw-r--r--   0        0        0     1049 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/terminal_node_string_result.py
+-rw-r--r--   0        0        0     1061 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0     1036 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_error_variable_value.py
+-rw-r--r--   0        0        0     1053 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_function_call_variable_value.py
+-rw-r--r--   0        0        0     1012 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_json_variable_value.py
+-rw-r--r--   0        0        0      996 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_number_variable_value.py
+-rw-r--r--   0        0        0     1068 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0      991 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_string_variable_value.py
+-rw-r--r--   0        0        0     2834 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_case_variable_value.py
+-rw-r--r--   0        0        0     1373 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1228 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1235 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1411 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      174 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1483 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_exec_config.py
+-rw-r--r--   0        0        0     1598 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_exec_config_request.py
+-rw-r--r--   0        0        0     1158 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution.py
+-rw-r--r--   0        0        0     1115 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_chat_history_output.py
+-rw-r--r--   0        0        0     1089 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_error_output.py
+-rw-r--r--   0        0        0     1107 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_function_call_output.py
+-rw-r--r--   0        0        0     1066 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_json_output.py
+-rw-r--r--   0        0        0      973 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_metric_definition.py
+-rw-r--r--   0        0        0     1218 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_metric_result.py
+-rw-r--r--   0        0        0     1047 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_number_output.py
+-rw-r--r--   0        0        0     3057 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_output.py
+-rw-r--r--   0        0        0     1122 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_search_results_output.py
+-rw-r--r--   0        0        0     1045 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_string_output.py
+-rw-r--r--   0        0        0     1331 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config.py
+-rw-r--r--   0        0        0     1115 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_data.py
+-rw-r--r--   0        0        0     1144 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_data_request.py
+-rw-r--r--   0        0        0     1360 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_request.py
+-rw-r--r--   0        0        0      148 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1005 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_error_output.py
+-rw-r--r--   0        0        0      144 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_error_output_type_enum.py
+-rw-r--r--   0        0        0      963 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_number_output.py
+-rw-r--r--   0        0        0      146 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_number_output_type_enum.py
+-rw-r--r--   0        0        0     1291 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_output.py
+-rw-r--r--   0        0        0      961 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_string_output.py
+-rw-r--r--   0        0        0      146 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_string_output_type_enum.py
+-rw-r--r--   0        0        0     1500 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_read.py
+-rw-r--r--   0        0        0      197 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_state.py
+-rw-r--r--   0        0        0      896 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_test_suite.py
+-rw-r--r--   0        0        0     1367 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py
+-rw-r--r--   0        0        0     1241 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py
+-rw-r--r--   0        0        0     1248 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py
+-rw-r--r--   0        0        0     1405 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py
+-rw-r--r--   0        0        0      170 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_type_enum.py
+-rw-r--r--   0        0        0     1086 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/test_suite_test_case.py
+-rw-r--r--   0        0        0      147 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/text_embedding_3_large_enum.py
+-rw-r--r--   0        0        0      147 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/text_embedding_3_small_enum.py
+-rw-r--r--   0        0        0      147 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/text_embedding_ada_002_enum.py
+-rw-r--r--   0        0        0     1025 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunker_config.py
+-rw-r--r--   0        0        0     1032 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunker_config_request.py
+-rw-r--r--   0        0        0      167 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunker_enum.py
+-rw-r--r--   0        0        0     1077 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunking.py
+-rw-r--r--   0        0        0     1106 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunking_request.py
+-rw-r--r--   0        0        0      866 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      946 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      937 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_error.py
+-rw-r--r--   0        0        0      233 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_error_code_enum.py
+-rw-r--r--   0        0        0      944 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_error_request.py
+-rw-r--r--   0        0        0      914 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_image.py
+-rw-r--r--   0        0        0      921 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_image_request.py
+-rw-r--r--   0        0        0      944 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_variable.py
+-rw-r--r--   0        0        0      281 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/vellum_variable_type.py
+-rw-r--r--   0        0        0     2110 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_deployment_read.py
+-rw-r--r--   0        0        0      981 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_event_error.py
+-rw-r--r--   0        0        0     2223 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_chat_history_request.py
+-rw-r--r--   0        0        0     2160 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_json_request.py
+-rw-r--r--   0        0        0     2137 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_string_request.py
+-rw-r--r--   0        0        0      425 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_event_error_code.py
+-rw-r--r--   0        0        0      170 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_event_type.py
+-rw-r--r--   0        0        0     1139 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_node_result_event.py
+-rw-r--r--   0        0        0     1134 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_execution_workflow_result_event.py
+-rw-r--r--   0        0        0     3625 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_node_result_data.py
+-rw-r--r--   0        0        0     1745 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_node_result_event.py
+-rw-r--r--   0        0        0      209 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_node_result_event_state.py
+-rw-r--r--   0        0        0     3212 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output.py
+-rw-r--r--   0        0        0     1148 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_array.py
+-rw-r--r--   0        0        0     1131 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_chat_history.py
+-rw-r--r--   0        0        0     1106 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_error.py
+-rw-r--r--   0        0        0     1123 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_function_call.py
+-rw-r--r--   0        0        0     1106 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_image.py
+-rw-r--r--   0        0        0     1082 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_json.py
+-rw-r--r--   0        0        0     1063 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_number.py
+-rw-r--r--   0        0        0     1138 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_search_results.py
+-rw-r--r--   0        0        0     1061 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_output_string.py
+-rw-r--r--   0        0        0     1137 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_request_chat_history_input_request.py
+-rw-r--r--   0        0        0     1772 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_request_input_request.py
+-rw-r--r--   0        0        0     1066 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_request_json_input_request.py
+-rw-r--r--   0        0        0     1047 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_request_number_input_request.py
+-rw-r--r--   0        0        0     1045 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_request_string_input_request.py
+-rw-r--r--   0        0        0     1475 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event.py
+-rw-r--r--   0        0        0     3529 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data.py
+-rw-r--r--   0        0        0     1423 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_array.py
+-rw-r--r--   0        0        0     1400 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_chat_history.py
+-rw-r--r--   0        0        0     1375 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_error.py
+-rw-r--r--   0        0        0     1392 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_function_call.py
+-rw-r--r--   0        0        0     1351 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_json.py
+-rw-r--r--   0        0        0     1332 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_number.py
+-rw-r--r--   0        0        0     1407 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_search_results.py
+-rw-r--r--   0        0        0     1482 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_string.py
+-rw-r--r--   0        0        0      911 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/types/workflow_stream_event.py
+-rw-r--r--   0        0        0       77 2024-05-29 20:53:45.769509 vellum_ai-0.6.1/src/vellum/version.py
+-rw-r--r--   0        0        0     3591 1970-01-01 00:00:00.000000 vellum_ai-0.6.1/PKG-INFO
```

### Comparing `vellum_ai-0.6.0/LICENSE` & `vellum_ai-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/README.md` & `vellum_ai-0.6.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Vellum Python Library
 
 [![pypi](https://img.shields.io/pypi/v/vellum-ai.svg)](https://pypi.python.org/pypi/vellum-ai)
-[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
-
+[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://buildwithfern.com/?utm_source=vellum-ai/vellum-client-python/readme)
 
 The Vellum Python Library provides access to the Vellum API from python.
 
 
 ## API Docs
 You can find Vellum's complete API docs at [docs.vellum.ai](https://docs.vellum.ai).
```

### Comparing `vellum_ai-0.6.0/pyproject.toml` & `vellum_ai-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vellum-ai"
-version = "0.6.0"
+version = "0.6.1"
 description = ""
 readme = "README.md"
 authors = []
 packages = [
     { include = "vellum", from = "src"}
 ]
```

### Comparing `vellum_ai-0.6.0/src/vellum/__init__.py` & `vellum_ai-0.6.1/src/vellum/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,14 +187,16 @@
     IntfloatMultilingualE5LargeEnum,
     JsonEnum,
     JsonInputRequest,
     JsonVariableValue,
     JsonVellumValue,
     LogicalOperator,
     LogprobsEnum,
+    MergeEnum,
+    MergeNodeResult,
     MetadataFilterConfigRequest,
     MetadataFilterRuleCombinator,
     MetadataFilterRuleRequest,
     MetricEnum,
     MetricNodeResult,
     MlModelUsage,
     NamedScenarioInputChatHistoryVariableValueRequest,
@@ -493,14 +495,15 @@
     WorkflowExecutionEventType,
     WorkflowExecutionNodeResultEvent,
     WorkflowExecutionWorkflowResultEvent,
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
+    WorkflowNodeResultData_Merge,
     WorkflowNodeResultData_Metric,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
     WorkflowNodeResultEvent,
@@ -768,14 +771,16 @@
     "IntfloatMultilingualE5LargeEnum",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
     "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
+    "MergeEnum",
+    "MergeNodeResult",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
     "MetricEnum",
     "MetricNodeResult",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
@@ -1077,14 +1082,15 @@
     "WorkflowExecutionEventType",
     "WorkflowExecutionNodeResultEvent",
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
+    "WorkflowNodeResultData_Merge",
     "WorkflowNodeResultData_Metric",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
     "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
```

### Comparing `vellum_ai-0.6.0/src/vellum/client.py` & `vellum_ai-0.6.1/src/vellum/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/__init__.py` & `vellum_ai-0.6.1/src/vellum/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/client_wrapper.py` & `vellum_ai-0.6.1/src/vellum/core/client_wrapper.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         self._environment = environment
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vellum-ai",
-            "X-Fern-SDK-Version": "0.6.0",
+            "X-Fern-SDK-Version": "0.6.1",
         }
         headers["X_API_KEY"] = self.api_key
         return headers
 
     def get_environment(self) -> VellumEnvironment:
         return self._environment
```

### Comparing `vellum_ai-0.6.0/src/vellum/core/datetime_utils.py` & `vellum_ai-0.6.1/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/file.py` & `vellum_ai-0.6.1/src/vellum/core/file.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/http_client.py` & `vellum_ai-0.6.1/src/vellum/core/http_client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.6.1/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/core/request_options.py` & `vellum_ai-0.6.1/src/vellum/core/request_options.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/lib/test_suites/resources.py` & `vellum_ai-0.6.1/src/vellum/lib/test_suites/resources.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/lib/utils/paginator.py` & `vellum_ai-0.6.1/src/vellum/lib/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/__init__.py` & `vellum_ai-0.6.1/src/vellum/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/deployments/client.py` & `vellum_ai-0.6.1/src/vellum/resources/deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/document_indexes/client.py` & `vellum_ai-0.6.1/src/vellum/resources/document_indexes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/documents/client.py` & `vellum_ai-0.6.1/src/vellum/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/folder_entities/client.py` & `vellum_ai-0.6.1/src/vellum/resources/folder_entities/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/sandboxes/client.py` & `vellum_ai-0.6.1/src/vellum/resources/sandboxes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/test_suite_runs/client.py` & `vellum_ai-0.6.1/src/vellum/resources/test_suite_runs/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/test_suites/client.py` & `vellum_ai-0.6.1/src/vellum/resources/test_suites/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/resources/workflow_deployments/client.py` & `vellum_ai-0.6.1/src/vellum/resources/workflow_deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz` & `vellum_ai-0.6.1/src/vellum/terraform/_jsii/vellum-ai_vellum@0.0.0.jsii.tgz`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/terraform/data_vellum_document_index/__init__.py` & `vellum_ai-0.6.1/src/vellum/terraform/data_vellum_document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/terraform/document_index/__init__.py` & `vellum_ai-0.6.1/src/vellum/terraform/document_index/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/terraform/provider/__init__.py` & `vellum_ai-0.6.1/src/vellum/terraform/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/__init__.py` & `vellum_ai-0.6.1/src/vellum/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,16 @@
 from .intfloat_multilingual_e_5_large_enum import IntfloatMultilingualE5LargeEnum
 from .json_enum import JsonEnum
 from .json_input_request import JsonInputRequest
 from .json_variable_value import JsonVariableValue
 from .json_vellum_value import JsonVellumValue
 from .logical_operator import LogicalOperator
 from .logprobs_enum import LogprobsEnum
+from .merge_enum import MergeEnum
+from .merge_node_result import MergeNodeResult
 from .metadata_filter_config_request import MetadataFilterConfigRequest
 from .metadata_filter_rule_combinator import MetadataFilterRuleCombinator
 from .metadata_filter_rule_request import MetadataFilterRuleRequest
 from .metric_enum import MetricEnum
 from .metric_node_result import MetricNodeResult
 from .ml_model_usage import MlModelUsage
 from .named_scenario_input_chat_history_variable_value_request import NamedScenarioInputChatHistoryVariableValueRequest
@@ -565,14 +567,15 @@
 from .workflow_execution_node_result_event import WorkflowExecutionNodeResultEvent
 from .workflow_execution_workflow_result_event import WorkflowExecutionWorkflowResultEvent
 from .workflow_node_result_data import (
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
+    WorkflowNodeResultData_Merge,
     WorkflowNodeResultData_Metric,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
 )
@@ -825,14 +828,16 @@
     "IntfloatMultilingualE5LargeEnum",
     "JsonEnum",
     "JsonInputRequest",
     "JsonVariableValue",
     "JsonVellumValue",
     "LogicalOperator",
     "LogprobsEnum",
+    "MergeEnum",
+    "MergeNodeResult",
     "MetadataFilterConfigRequest",
     "MetadataFilterRuleCombinator",
     "MetadataFilterRuleRequest",
     "MetricEnum",
     "MetricNodeResult",
     "MlModelUsage",
     "NamedScenarioInputChatHistoryVariableValueRequest",
@@ -1131,14 +1136,15 @@
     "WorkflowExecutionEventType",
     "WorkflowExecutionNodeResultEvent",
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
+    "WorkflowNodeResultData_Merge",
     "WorkflowNodeResultData_Metric",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
     "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/api_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/api_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/api_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/api_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content.py` & `vellum_ai-0.6.1/src/vellum/types/array_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item.py` & `vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_item_request.py` & `vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_item_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_chat_message_content_request.py` & `vellum_ai-0.6.1/src/vellum/types/array_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_variable_value_item.py` & `vellum_ai-0.6.1/src/vellum/types/array_variable_value_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/array_vellum_value_item.py` & `vellum_ai-0.6.1/src/vellum/types/array_vellum_value_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large_request.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_intfloat_multilingual_e_5_large_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_cos_v_1_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request.py` & `vellum_ai-0.6.1/src/vellum/types/basic_vectorizer_sentence_transformers_multi_qa_mpnet_base_dot_v_1_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/chat_history_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/chat_message.py` & `vellum_ai-0.6.1/src/vellum/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/chat_message_content.py` & `vellum_ai-0.6.1/src/vellum/types/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/chat_message_content_request.py` & `vellum_ai-0.6.1/src/vellum/types/chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/chat_message_request.py` & `vellum_ai-0.6.1/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_array_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_chat_history_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_error_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_function_call_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_json_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_number_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_result_output.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_search_results_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/code_execution_node_string_result.py` & `vellum_ai-0.6.1/src/vellum/types/code_execution_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/conditional_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/conditional_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/conditional_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/conditional_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/deployment_provider_payload_response.py` & `vellum_ai-0.6.1/src/vellum/types/deployment_provider_payload_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/deployment_read.py` & `vellum_ai-0.6.1/src/vellum/types/deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.6.1/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_index_chunking.py` & `vellum_ai-0.6.1/src/vellum/types/document_index_chunking.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_index_chunking_request.py` & `vellum_ai-0.6.1/src/vellum/types/document_index_chunking_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config.py` & `vellum_ai-0.6.1/src/vellum/types/document_index_indexing_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_index_indexing_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/document_index_indexing_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_index_read.py` & `vellum_ai-0.6.1/src/vellum/types/document_index_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/document_read.py` & `vellum_ai-0.6.1/src/vellum/types/document_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.6.1/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/error_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/error_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/error_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_prompt_api_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/execute_prompt_api_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_prompt_event.py` & `vellum_ai-0.6.1/src/vellum/types/execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_prompt_response.py` & `vellum_ai-0.6.1/src/vellum/types/execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_workflow_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/execute_workflow_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_workflow_response.py` & `vellum_ai-0.6.1/src/vellum/types/execute_workflow_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_workflow_stream_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/execute_workflow_stream_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_array_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_array_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_chat_history_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_chat_history_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_error_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_error_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_function_call_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_function_call_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_json_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_json_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_number_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_number_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_search_results_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_search_results_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_string_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_string_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/execution_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/execution_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/external_test_case_execution.py` & `vellum_ai-0.6.1/src/vellum/types/external_test_case_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/external_test_case_execution_request.py` & `vellum_ai-0.6.1/src/vellum/types/external_test_case_execution_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_event.py` & `vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_prompt_response.py` & `vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/fulfilled_prompt_execution_meta.py` & `vellum_ai-0.6.1/src/vellum/types/fulfilled_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/fulfilled_workflow_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/fulfilled_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call.py` & `vellum_ai-0.6.1/src/vellum/types/function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_request.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_chat_message_content_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_chat_message_content_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_request.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/function_call_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/function_call_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_options_request.py` & `vellum_ai-0.6.1/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_request.py` & `vellum_ai-0.6.1/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_response.py` & `vellum_ai-0.6.1/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_result.py` & `vellum_ai-0.6.1/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_result_error.py` & `vellum_ai-0.6.1/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_stream_response.py` & `vellum_ai-0.6.1/src/vellum/types/generate_stream_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_stream_result.py` & `vellum_ai-0.6.1/src/vellum/types/generate_stream_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/generate_stream_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/generate_stream_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer.py` & `vellum_ai-0.6.1/src/vellum/types/hkunlp_instructor_xl_vectorizer.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/hkunlp_instructor_xl_vectorizer_request.py` & `vellum_ai-0.6.1/src/vellum/types/hkunlp_instructor_xl_vectorizer_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/image_chat_message_content.py` & `vellum_ai-0.6.1/src/vellum/types/image_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/image_chat_message_content_request.py` & `vellum_ai-0.6.1/src/vellum/types/image_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/image_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/image_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/image_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/image_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer.py` & `vellum_ai-0.6.1/src/vellum/types/indexing_config_vectorizer.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/indexing_config_vectorizer_request.py` & `vellum_ai-0.6.1/src/vellum/types/indexing_config_vectorizer_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/initiated_execute_prompt_event.py` & `vellum_ai-0.6.1/src/vellum/types/initiated_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/initiated_prompt_execution_meta.py` & `vellum_ai-0.6.1/src/vellum/types/initiated_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/initiated_workflow_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/initiated_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config.py` & `vellum_ai-0.6.1/src/vellum/types/instructor_vectorizer_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/instructor_vectorizer_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/instructor_vectorizer_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/json_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/json_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/json_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/json_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/metadata_filter_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/metadata_filter_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/metadata_filter_rule_request.py` & `vellum_ai-0.6.1/src/vellum/types/metadata_filter_rule_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/metric_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/metric_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/ml_model_usage.py` & `vellum_ai-0.6.1/src/vellum/types/ml_model_usage.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_scenario_input_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_scenario_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_scenario_input_string_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_scenario_input_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_chat_history_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_error_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_error_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_function_call_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_function_call_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_json_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_json_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_number_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_number_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_search_results_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_search_results_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_string_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/named_test_case_variable_value_request.py` & `vellum_ai-0.6.1/src/vellum/types/named_test_case_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_array_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_array_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_chat_history_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_error_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_function_call.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_json_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_number_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_search_results_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_compiled_string_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_input_variable_compiled_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_input_variable_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_array_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_array_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_chat_history_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_error_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_function_call_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_function_call_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_json_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_number_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_search_results_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_string_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/node_output_compiled_value.py` & `vellum_ai-0.6.1/src/vellum/types/node_output_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.6.1/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.6.1/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/number_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/number_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/number_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_large.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_large_request.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_large_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_small.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_3_small_request.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_3_small_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002_request.py` & `vellum_ai-0.6.1/src/vellum/types/open_ai_vectorizer_text_embedding_ada_002_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_document_index_read_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_document_index_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_slim_deployment_read_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_slim_deployment_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_slim_workflow_deployment_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_slim_workflow_deployment_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_run_execution_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_test_suite_run_execution_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/paginated_test_suite_test_case_list.py` & `vellum_ai-0.6.1/src/vellum/types/paginated_test_suite_test_case_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_deployment_expand_meta_request_request.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_deployment_expand_meta_request_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_deployment_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_deployment_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_execution_meta.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/prompt_output.py` & `vellum_ai-0.6.1/src/vellum/types/prompt_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/raw_prompt_execution_overrides_request.py` & `vellum_ai-0.6.1/src/vellum/types/raw_prompt_execution_overrides_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config.py` & `vellum_ai-0.6.1/src/vellum/types/reducto_chunker_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/reducto_chunker_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/reducto_chunker_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/reducto_chunking.py` & `vellum_ai-0.6.1/src/vellum/types/reducto_chunking.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/reducto_chunking_request.py` & `vellum_ai-0.6.1/src/vellum/types/reducto_chunking_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_event.py` & `vellum_ai-0.6.1/src/vellum/types/rejected_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/rejected_execute_prompt_response.py` & `vellum_ai-0.6.1/src/vellum/types/rejected_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/rejected_execute_workflow_workflow_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/rejected_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/rejected_prompt_execution_meta.py` & `vellum_ai-0.6.1/src/vellum/types/rejected_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/rejected_workflow_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/rejected_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.6.1/src/vellum/types/sandbox_scenario.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/scenario_input.py` & `vellum_ai-0.6.1/src/vellum/types/scenario_input.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/scenario_input_chat_history_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/scenario_input_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/scenario_input_string_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/scenario_input_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_filters_request.py` & `vellum_ai-0.6.1/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/search_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/search_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.6.1/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_response.py` & `vellum_ai-0.6.1/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_result.py` & `vellum_ai-0.6.1/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_result_document.py` & `vellum_ai-0.6.1/src/vellum/types/search_weights_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,23 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class SearchResultDocument(pydantic_v1.BaseModel):
-    id: str = pydantic_v1.Field()
+class SearchWeightsRequest(pydantic_v1.BaseModel):
+    semantic_similarity: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The ID of the document.
+    The relative weight to give to semantic similarity
     """
 
-    label: str = pydantic_v1.Field()
+    keywords: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    The human-readable name for the document.
-    """
-
-    external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The unique ID of the document as represented in an external system and specified when it was originally uploaded.
-    """
-
-    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
-    """
-    A previously supplied JSON object containing metadata that can be filtered on when searching.
+    The relative weight to give to keywords
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_result_document_request.py` & `vellum_ai-0.6.1/src/vellum/types/search_result_document.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class SearchResultDocumentRequest(pydantic_v1.BaseModel):
+class SearchResultDocument(pydantic_v1.BaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The ID of the document.
+    """
+
     label: str = pydantic_v1.Field()
     """
     The human-readable name for the document.
     """
 
     external_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.6.1/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_result_request.py` & `vellum_ai-0.6.1/src/vellum/types/search_result_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/search_weights_request.py` & `vellum_ai-0.6.1/src/vellum/types/sentence_chunker_config_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,21 @@
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
 
 
-class SearchWeightsRequest(pydantic_v1.BaseModel):
-    semantic_similarity: typing.Optional[float] = pydantic_v1.Field(default=None)
+class SentenceChunkerConfigRequest(pydantic_v1.BaseModel):
     """
-    The relative weight to give to semantic similarity
+    Configuration for sentence chunking
     """
 
-    keywords: typing.Optional[float] = pydantic_v1.Field(default=None)
-    """
-    The relative weight to give to keywords
-    """
+    character_limit: typing.Optional[int] = None
+    min_overlap_ratio: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config.py` & `vellum_ai-0.6.1/src/vellum/types/sentence_chunker_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/sentence_chunker_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/sentence_chunking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .sentence_chunker_config import SentenceChunkerConfig
 
 
-class SentenceChunkerConfigRequest(pydantic_v1.BaseModel):
+class SentenceChunking(pydantic_v1.BaseModel):
     """
-    Configuration for sentence chunking
+    Sentence chunking
     """
 
-    character_limit: typing.Optional[int] = None
-    min_overlap_ratio: typing.Optional[float] = None
+    chunker_config: typing.Optional[SentenceChunkerConfig] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/sentence_chunking.py` & `vellum_ai-0.6.1/src/vellum/types/sentence_chunking_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .sentence_chunker_config import SentenceChunkerConfig
+from .sentence_chunker_config_request import SentenceChunkerConfigRequest
 
 
-class SentenceChunking(pydantic_v1.BaseModel):
+class SentenceChunkingRequest(pydantic_v1.BaseModel):
     """
     Sentence chunking
     """
 
-    chunker_config: typing.Optional[SentenceChunkerConfig] = None
+    chunker_config: typing.Optional[SentenceChunkerConfigRequest] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/sentence_chunking_request.py` & `vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunker_config_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .sentence_chunker_config_request import SentenceChunkerConfigRequest
 
 
-class SentenceChunkingRequest(pydantic_v1.BaseModel):
+class TokenOverlappingWindowChunkerConfigRequest(pydantic_v1.BaseModel):
     """
-    Sentence chunking
+    Configuration for token overlapping window chunking
     """
 
-    chunker_config: typing.Optional[SentenceChunkerConfigRequest] = None
+    token_limit: typing.Optional[int] = None
+    overlap_ratio: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/slim_deployment_read.py` & `vellum_ai-0.6.1/src/vellum/types/slim_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/slim_document.py` & `vellum_ai-0.6.1/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/slim_workflow_deployment.py` & `vellum_ai-0.6.1/src/vellum/types/slim_workflow_deployment.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/streaming_execute_prompt_event.py` & `vellum_ai-0.6.1/src/vellum/types/streaming_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/streaming_prompt_execution_meta.py` & `vellum_ai-0.6.1/src/vellum/types/streaming_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/streaming_workflow_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/streaming_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/string_chat_message_content.py` & `vellum_ai-0.6.1/src/vellum/types/string_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/string_chat_message_content_request.py` & `vellum_ai-0.6.1/src/vellum/types/string_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/string_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/string_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/string_vellum_value.py` & `vellum_ai-0.6.1/src/vellum/types/string_vellum_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.6.1/src/vellum/types/submit_completion_actual_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     """
 
     timestamp: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
     """
     Optionally provide the timestamp representing when this feedback was collected. Used for reporting purposes.
     """
 
+    metadata: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    """
+    Optionally provide additional metadata about the feedback submission.
+    """
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/submit_workflow_execution_actual_request.py` & `vellum_ai-0.6.1/src/vellum/types/submit_workflow_execution_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/subworkflow_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/subworkflow_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_array_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_chat_history_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_error_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_function_call_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_json_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_number_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_result_output.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_search_results_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/templating_node_string_result.py` & `vellum_ai-0.6.1/src/vellum/types/templating_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_array_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_array_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_chat_history_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_error_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_function_call_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_function_call_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_json_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_number_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_result_output.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_search_results_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/terminal_node_string_result.py` & `vellum_ai-0.6.1/src/vellum/types/terminal_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_chat_history_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_error_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_function_call_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_json_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_number_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_search_results_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_string_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_case_variable_value.py` & `vellum_ai-0.6.1/src/vellum/types/test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_deployment_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_exec_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_chat_history_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_chat_history_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_error_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_function_call_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_function_call_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_json_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_json_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_definition.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_metric_definition.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_metric_result.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_metric_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_number_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_search_results_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_search_results_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_execution_string_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_execution_string_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_data_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_external_exec_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_external_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_error_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_error_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_number_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_number_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_metric_string_output.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_metric_string_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_read.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_test_suite.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_test_suite.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_run_workflow_release_tag_exec_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/test_suite_test_case.py` & `vellum_ai-0.6.1/src/vellum/types/test_suite_test_case.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config.py` & `vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunker_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunker_config_request.py` & `vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunking_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
+from .token_overlapping_window_chunker_config_request import TokenOverlappingWindowChunkerConfigRequest
 
 
-class TokenOverlappingWindowChunkerConfigRequest(pydantic_v1.BaseModel):
+class TokenOverlappingWindowChunkingRequest(pydantic_v1.BaseModel):
     """
-    Configuration for token overlapping window chunking
+    Token overlapping window chunking
     """
 
-    token_limit: typing.Optional[int] = None
-    overlap_ratio: typing.Optional[float] = None
+    chunker_config: typing.Optional[TokenOverlappingWindowChunkerConfigRequest] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking.py` & `vellum_ai-0.6.1/src/vellum/types/token_overlapping_window_chunking.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/token_overlapping_window_chunking_request.py` & `vellum_ai-0.6.1/src/vellum/types/merge_node_result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
 from ..core.pydantic_utilities import pydantic_v1
-from .token_overlapping_window_chunker_config_request import TokenOverlappingWindowChunkerConfigRequest
 
 
-class TokenOverlappingWindowChunkingRequest(pydantic_v1.BaseModel):
+class MergeNodeResult(pydantic_v1.BaseModel):
     """
-    Token overlapping window chunking
+    A Node Result Event emitted from a Merge Node.
     """
 
-    chunker_config: typing.Optional[TokenOverlappingWindowChunkerConfigRequest] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.6.1/src/vellum/types/upload_document_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/upload_document_response.py` & `vellum_ai-0.6.1/src/vellum/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/vellum_error.py` & `vellum_ai-0.6.1/src/vellum/types/vellum_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/vellum_error_request.py` & `vellum_ai-0.6.1/src/vellum/types/vellum_error_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/vellum_image.py` & `vellum_ai-0.6.1/src/vellum/types/vellum_image.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/vellum_image_request.py` & `vellum_ai-0.6.1/src/vellum/types/vellum_image_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/vellum_variable.py` & `vellum_ai-0.6.1/src/vellum/types/vellum_variable.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_deployment_read.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_event_error.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_event_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_chat_history_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_chat_history_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_json_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_json_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_execution_actual_string_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_execution_actual_string_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_execution_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_execution_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_execution_workflow_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_execution_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_node_result_data.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_node_result_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 
 import typing
 
 from .api_node_result import ApiNodeResult
 from .code_execution_node_result import CodeExecutionNodeResult
 from .conditional_node_result import ConditionalNodeResult
+from .merge_node_result import MergeNodeResult
 from .metric_node_result import MetricNodeResult
 from .prompt_node_result import PromptNodeResult
 from .search_node_result import SearchNodeResult
 from .subworkflow_node_result import SubworkflowNodeResult
 from .templating_node_result import TemplatingNodeResult
 from .terminal_node_result import TerminalNodeResult
 
@@ -81,14 +82,24 @@
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
 
 
+class WorkflowNodeResultData_Merge(MergeNodeResult):
+    type: typing.Literal["MERGE"] = "MERGE"
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
+
+
 class WorkflowNodeResultData_Subworkflow(SubworkflowNodeResult):
     type: typing.Literal["SUBWORKFLOW"] = "SUBWORKFLOW"
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
@@ -109,10 +120,11 @@
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_Terminal,
+    WorkflowNodeResultData_Merge,
     WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Metric,
 ]
```

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_node_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_array.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_array.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_chat_history.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_error.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_function_call.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_image.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_image.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_json.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_number.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_search_results.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_output_string.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_output_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_request_chat_history_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_request_chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_request_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_request_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_request_json_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_request_json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_request_number_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_request_number_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_request_string_input_request.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_request_string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_array.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_array.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_chat_history.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_error.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_function_call.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_json.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_number.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_search_results.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_result_event_output_data_string.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_result_event_output_data_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/src/vellum/types/workflow_stream_event.py` & `vellum_ai-0.6.1/src/vellum/types/workflow_stream_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.6.0/PKG-INFO` & `vellum_ai-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.6.0
+Version: 0.6.1
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -14,16 +14,15 @@
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: typing_extensions (>=4.0.0)
 Description-Content-Type: text/markdown
 
 # Vellum Python Library
 
 [![pypi](https://img.shields.io/pypi/v/vellum-ai.svg)](https://pypi.python.org/pypi/vellum-ai)
-[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://github.com/fern-api/fern)
-
+[![fern shield](https://img.shields.io/badge/%F0%9F%8C%BF-SDK%20generated%20by%20Fern-brightgreen)](https://buildwithfern.com/?utm_source=vellum-ai/vellum-client-python/readme)
 
 The Vellum Python Library provides access to the Vellum API from python.
 
 
 ## API Docs
 You can find Vellum's complete API docs at [docs.vellum.ai](https://docs.vellum.ai).
```

