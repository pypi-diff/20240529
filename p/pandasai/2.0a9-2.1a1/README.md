# Comparing `tmp/pandasai-2.0a9.tar.gz` & `tmp/pandasai-2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-2.0a9.tar", max compression
+gzip compressed data, was "pandasai-2.1a1.tar", max compression
```

## Comparing `pandasai-2.0a9.tar` & `pandasai-2.1a1.tar`

### file list

```diff
@@ -1,128 +1,153 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-2.0a9/LICENSE
-drwxr-xr-x   0        0        0        0 2023-11-20 22:14:04.721024 pandasai-2.0a9/LICENSES/
--rw-r--r--   0        0        0     7206 2024-02-21 10:04:57.962885 pandasai-2.0a9/README.md
--rw-r--r--   0        0        0      682 2024-02-21 10:04:57.967562 pandasai-2.0a9/pandasai/__init__.py
--rw-r--r--   0        0        0       45 2024-02-19 14:59:32.858258 pandasai-2.0a9/pandasai/agent/__init__.py
--rw-r--r--   0        0        0    13699 2024-02-21 10:04:57.967914 pandasai-2.0a9/pandasai/agent/base.py
--rw-r--r--   0        0        0      994 2024-02-19 14:59:32.858993 pandasai-2.0a9/pandasai/agent/callbacks.py
--rw-r--r--   0        0        0     1227 2024-02-19 14:59:32.859598 pandasai-2.0a9/pandasai/config.py
--rw-r--r--   0        0        0      908 2024-02-21 10:04:57.968102 pandasai-2.0a9/pandasai/connectors/__init__.py
--rw-r--r--   0        0        0     8777 2024-02-21 10:04:57.968280 pandasai-2.0a9/pandasai/connectors/airtable.py
--rw-r--r--   0        0        0     7750 2024-02-21 10:04:57.968449 pandasai-2.0a9/pandasai/connectors/base.py
--rw-r--r--   0        0        0     2880 2024-02-21 10:04:57.968631 pandasai-2.0a9/pandasai/connectors/databricks.py
--rw-r--r--   0        0        0     2226 2024-02-21 10:04:57.968768 pandasai-2.0a9/pandasai/connectors/google_big_query.py
--rw-r--r--   0        0        0     4422 2024-02-21 10:04:57.968938 pandasai-2.0a9/pandasai/connectors/pandas.py
--rw-r--r--   0        0        0     4164 2024-02-21 10:04:57.969097 pandasai-2.0a9/pandasai/connectors/polars.py
--rw-r--r--   0        0        0     3834 2024-02-21 10:04:57.969289 pandasai-2.0a9/pandasai/connectors/snowflake.py
--rw-r--r--   0        0        0    18682 2024-02-21 10:04:57.969437 pandasai-2.0a9/pandasai/connectors/sql.py
--rw-r--r--   0        0        0     5871 2024-02-21 10:04:57.969757 pandasai-2.0a9/pandasai/connectors/yahoo_finance.py
--rw-r--r--   0        0        0     1711 2024-02-21 10:04:57.969904 pandasai-2.0a9/pandasai/constants.py
--rw-r--r--   0        0        0      507 2024-02-21 10:04:57.970176 pandasai-2.0a9/pandasai/engine.py
--rw-r--r--   0        0        0     5284 2024-02-21 10:04:57.970349 pandasai-2.0a9/pandasai/exceptions.py
--rw-r--r--   0        0        0      446 2024-02-21 10:04:57.970515 pandasai-2.0a9/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4613 2024-02-21 10:04:57.971425 pandasai-2.0a9/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     3019 2024-02-21 10:04:57.971578 pandasai-2.0a9/pandasai/helpers/cache.py
--rw-r--r--   0        0        0    23368 2024-02-21 18:45:03.820108 pandasai-2.0a9/pandasai/helpers/code_manager.py
--rw-r--r--   0        0        0     2397 2024-02-21 10:04:57.972019 pandasai-2.0a9/pandasai/helpers/data_sampler.py
--rw-r--r--   0        0        0     4574 2024-02-21 10:04:57.972177 pandasai-2.0a9/pandasai/helpers/dataframe_serializer.py
--rw-r--r--   0        0        0     5062 2024-02-21 10:04:57.972426 pandasai-2.0a9/pandasai/helpers/df_config_manager.py
--rw-r--r--   0        0        0     1378 2024-02-21 10:04:57.972700 pandasai-2.0a9/pandasai/helpers/df_info.py
--rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.972971 pandasai-2.0a9/pandasai/helpers/df_validator.py
--rw-r--r--   0        0        0      526 2024-02-21 10:04:57.973121 pandasai-2.0a9/pandasai/helpers/env.py
--rw-r--r--   0        0        0      928 2024-02-21 10:04:57.973259 pandasai-2.0a9/pandasai/helpers/file_importer.py
--rw-r--r--   0        0        0      725 2024-02-21 10:04:57.973382 pandasai-2.0a9/pandasai/helpers/folder.py
--rw-r--r--   0        0        0     3717 2024-02-21 10:04:57.973750 pandasai-2.0a9/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     4273 2024-02-21 10:04:57.973959 pandasai-2.0a9/pandasai/helpers/logger.py
--rw-r--r--   0        0        0     2770 2024-02-19 14:59:43.492203 pandasai-2.0a9/pandasai/helpers/memory.py
--rw-r--r--   0        0        0      447 2023-09-13 09:35:53.943189 pandasai-2.0a9/pandasai/helpers/node_visitors.py
--rw-r--r--   0        0        0      213 2023-11-20 22:14:04.734116 pandasai-2.0a9/pandasai/helpers/openai.py
--rw-r--r--   0        0        0     6019 2024-02-21 10:04:57.974150 pandasai-2.0a9/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3898 2023-09-04 21:53:07.384708 pandasai-2.0a9/pandasai/helpers/optional.py
--rw-r--r--   0        0        0     1976 2024-02-21 10:04:57.974259 pandasai-2.0a9/pandasai/helpers/output_types/__init__.py
--rw-r--r--   0        0        0     4658 2024-02-21 10:04:57.974363 pandasai-2.0a9/pandasai/helpers/output_types/_output_types.py
--rw-r--r--   0        0        0     2310 2024-02-21 10:04:57.974537 pandasai-2.0a9/pandasai/helpers/output_validator.py
--rw-r--r--   0        0        0     2074 2023-11-20 22:14:04.734712 pandasai-2.0a9/pandasai/helpers/path.py
--rw-r--r--   0        0        0     8344 2024-02-21 18:45:03.820364 pandasai-2.0a9/pandasai/helpers/query_exec_tracker.py
--rw-r--r--   0        0        0     2466 2024-02-21 10:04:57.974868 pandasai-2.0a9/pandasai/helpers/request.py
--rw-r--r--   0        0        0     1061 2024-02-21 10:04:57.975042 pandasai-2.0a9/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     8579 2024-02-21 10:04:57.975494 pandasai-2.0a9/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     2388 2024-02-21 10:04:57.975669 pandasai-2.0a9/pandasai/helpers/skills_manager.py
--rw-r--r--   0        0        0      426 2024-01-19 10:23:41.929740 pandasai-2.0a9/pandasai/helpers/sql.py
--rw-r--r--   0        0        0      435 2024-02-21 10:04:57.975850 pandasai-2.0a9/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     7002 2024-02-21 10:04:57.977815 pandasai-2.0a9/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0      732 2024-02-21 10:04:57.978008 pandasai-2.0a9/pandasai/llm/bamboo_llm.py
--rw-r--r--   0        0        0    13732 2024-02-21 10:04:57.978209 pandasai-2.0a9/pandasai/llm/base.py
--rw-r--r--   0        0        0      640 2024-02-19 14:59:43.493258 pandasai-2.0a9/pandasai/llm/fake.py
--rw-r--r--   0        0        0     2660 2024-02-21 10:04:57.978791 pandasai-2.0a9/pandasai/llm/google_gemini.py
--rw-r--r--   0        0        0     2737 2024-02-21 10:04:57.979108 pandasai-2.0a9/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     5687 2024-02-21 10:04:57.979290 pandasai-2.0a9/pandasai/llm/google_vertexai.py
--rw-r--r--   0        0        0     4003 2024-02-21 10:04:57.979493 pandasai-2.0a9/pandasai/llm/huggingface_text_gen.py
--rw-r--r--   0        0        0     1168 2024-02-21 10:04:57.979830 pandasai-2.0a9/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.980594 pandasai-2.0a9/pandasai/llm/openai.py
--rw-r--r--   0        0        0      352 2024-02-21 10:04:57.980893 pandasai-2.0a9/pandasai/pandas/__init__.py
--rw-r--r--   0        0        0      206 2024-02-19 14:59:32.870508 pandasai-2.0a9/pandasai/pipelines/__init__.py
--rw-r--r--   0        0        0      353 2023-11-20 22:14:04.741653 pandasai-2.0a9/pandasai/pipelines/abstract_pipeline.py
--rw-r--r--   0        0        0     1062 2024-02-19 14:59:32.870645 pandasai-2.0a9/pandasai/pipelines/base_logic_unit.py
--rw-r--r--   0        0        0     1438 2024-02-19 14:59:32.870772 pandasai-2.0a9/pandasai/pipelines/chat/cache_lookup.py
--rw-r--r--   0        0        0     1253 2024-02-21 10:04:57.981058 pandasai-2.0a9/pandasai/pipelines/chat/cache_population.py
--rw-r--r--   0        0        0      572 2024-02-21 10:04:57.981190 pandasai-2.0a9/pandasai/pipelines/chat/chat_pipeline_input.py
--rw-r--r--   0        0        0     4381 2024-02-21 18:45:03.820554 pandasai-2.0a9/pandasai/pipelines/chat/code_execution.py
--rw-r--r--   0        0        0     1473 2024-02-21 10:04:57.981483 pandasai-2.0a9/pandasai/pipelines/chat/code_generator.py
--rw-r--r--   0        0        0     1479 2024-02-21 10:04:57.981659 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
--rw-r--r--   0        0        0      240 2024-02-19 14:59:32.872442 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
--rw-r--r--   0        0        0     3037 2024-02-21 10:04:57.981791 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
--rw-r--r--   0        0        0     5667 2024-02-21 10:04:57.982189 pandasai-2.0a9/pandasai/pipelines/chat/generate_chat_pipeline.py
--rw-r--r--   0        0        0     2258 2024-02-21 10:04:57.982377 pandasai-2.0a9/pandasai/pipelines/chat/prompt_generation.py
--rw-r--r--   0        0        0     2152 2024-02-21 10:04:57.982525 pandasai-2.0a9/pandasai/pipelines/chat/result_parsing.py
--rw-r--r--   0        0        0     1828 2024-02-21 10:04:57.982661 pandasai-2.0a9/pandasai/pipelines/chat/result_validation.py
--rw-r--r--   0        0        0     1838 2024-02-21 10:04:57.982804 pandasai-2.0a9/pandasai/pipelines/chat/validate_pipeline_input.py
--rw-r--r--   0        0        0      612 2024-02-21 18:45:03.821564 pandasai-2.0a9/pandasai/pipelines/logic_unit_output.py
--rw-r--r--   0        0        0      422 2024-02-21 10:04:57.983209 pandasai-2.0a9/pandasai/pipelines/logic_units/code_executor.py
--rw-r--r--   0        0        0      900 2024-02-21 10:04:57.983722 pandasai-2.0a9/pandasai/pipelines/logic_units/output_logic_unit.py
--rw-r--r--   0        0        0      511 2024-02-21 10:04:57.984328 pandasai-2.0a9/pandasai/pipelines/logic_units/prompt_execution.py
--rw-r--r--   0        0        0     4863 2024-02-21 18:45:03.821756 pandasai-2.0a9/pandasai/pipelines/pipeline.py
--rw-r--r--   0        0        0     1683 2024-02-21 10:04:57.987455 pandasai-2.0a9/pandasai/pipelines/pipeline_context.py
--rw-r--r--   0        0        0      232 2024-02-19 14:59:32.874197 pandasai-2.0a9/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1751 2024-02-21 10:04:57.987648 pandasai-2.0a9/pandasai/prompts/base.py
--rw-r--r--   0        0        0      207 2024-02-19 14:59:32.874683 pandasai-2.0a9/pandasai/prompts/check_if_relevant_to_conversation.py
--rw-r--r--   0        0        0      518 2024-02-21 10:04:57.988163 pandasai-2.0a9/pandasai/prompts/clarification_questions_prompt.py
--rw-r--r--   0        0        0      902 2024-02-19 14:59:43.494778 pandasai-2.0a9/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0      975 2024-02-19 14:59:43.494975 pandasai-2.0a9/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
--rw-r--r--   0        0        0     1058 2024-02-19 14:59:43.495349 pandasai-2.0a9/pandasai/prompts/correct_output_type_error_prompt.py
--rw-r--r--   0        0        0     1867 2024-02-21 10:04:57.988317 pandasai-2.0a9/pandasai/prompts/direct_sql_prompt.py
--rw-r--r--   0        0        0      159 2024-02-19 14:59:32.875691 pandasai-2.0a9/pandasai/prompts/explain_prompt.py
--rw-r--r--   0        0        0     1274 2024-02-21 10:04:57.989230 pandasai-2.0a9/pandasai/prompts/file_based_prompt.py
--rw-r--r--   0        0        0      879 2024-02-19 14:59:43.495788 pandasai-2.0a9/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      268 2024-02-19 14:59:43.495993 pandasai-2.0a9/pandasai/prompts/generate_python_code_with_sql.py
--rw-r--r--   0        0        0      189 2024-02-19 14:59:32.876351 pandasai-2.0a9/pandasai/prompts/generate_system_message.py
--rw-r--r--   0        0        0      172 2024-02-19 14:59:32.876525 pandasai-2.0a9/pandasai/prompts/rephase_query_prompt.py
--rw-r--r--   0        0        0      199 2024-02-19 14:59:32.876929 pandasai-2.0a9/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
--rw-r--r--   0        0        0      571 2024-02-19 14:59:32.877085 pandasai-2.0a9/pandasai/prompts/templates/clarification_questions_prompt.tmpl
--rw-r--r--   0        0        0      342 2024-02-19 14:59:32.877365 pandasai-2.0a9/pandasai/prompts/templates/correct_error_prompt.tmpl
--rw-r--r--   0        0        0      356 2024-02-19 14:59:32.877433 pandasai-2.0a9/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
--rw-r--r--   0        0        0      343 2024-02-21 10:04:57.989599 pandasai-2.0a9/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
--rw-r--r--   0        0        0      325 2024-02-19 14:59:32.878056 pandasai-2.0a9/pandasai/prompts/templates/explain.tmpl
--rw-r--r--   0        0        0      923 2024-02-19 14:59:32.878194 pandasai-2.0a9/pandasai/prompts/templates/generate_python_code.tmpl
--rw-r--r--   0        0        0     1326 2024-02-19 14:59:32.878350 pandasai-2.0a9/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
--rw-r--r--   0        0        0      176 2024-02-19 14:59:32.878491 pandasai-2.0a9/pandasai/prompts/templates/generate_system_message.tmpl
--rw-r--r--   0        0        0      387 2024-02-19 14:59:32.878627 pandasai-2.0a9/pandasai/prompts/templates/rephrase_query.tmpl
--rw-r--r--   0        0        0       91 2024-02-19 14:59:32.878727 pandasai-2.0a9/pandasai/prompts/templates/shared/dataframe.tmpl
--rw-r--r--   0        0        0      916 2024-02-19 14:59:32.878793 pandasai-2.0a9/pandasai/prompts/templates/shared/output_type_template.tmpl
--rw-r--r--   0        0        0      624 2024-02-19 14:59:32.878855 pandasai-2.0a9/pandasai/prompts/templates/shared/vectordb_docs.tmpl
--rw-r--r--   0        0        0      311 2024-02-21 10:04:57.990280 pandasai-2.0a9/pandasai/responses/__init__.py
--rw-r--r--   0        0        0      637 2024-02-19 14:59:32.879294 pandasai-2.0a9/pandasai/responses/context.py
--rw-r--r--   0        0        0     2023 2024-02-21 10:04:57.990747 pandasai-2.0a9/pandasai/responses/response_parser.py
--rw-r--r--   0        0        0     1290 2024-02-21 10:04:57.990963 pandasai-2.0a9/pandasai/responses/response_serializer.py
--rw-r--r--   0        0        0       96 2024-02-19 14:59:32.879758 pandasai-2.0a9/pandasai/responses/response_type.py
--rw-r--r--   0        0        0     1036 2024-02-21 10:04:57.991273 pandasai-2.0a9/pandasai/responses/streamlit_response.py
--rw-r--r--   0        0        0       16 2023-09-04 21:53:07.396618 pandasai-2.0a9/pandasai/schemas/__init__.py
--rw-r--r--   0        0        0     1319 2024-02-21 10:04:57.991469 pandasai-2.0a9/pandasai/schemas/df_config.py
--rw-r--r--   0        0        0     3911 2024-02-21 10:04:57.991644 pandasai-2.0a9/pandasai/skills/__init__.py
--rw-r--r--   0        0        0     8991 2024-02-21 10:04:57.991761 pandasai-2.0a9/pandasai/smart_dataframe/__init__.py
--rw-r--r--   0        0        0     6336 2024-02-21 10:04:57.991865 pandasai-2.0a9/pandasai/smart_datalake/__init__.py
--rw-r--r--   0        0        0      230 2024-02-21 10:04:57.992013 pandasai-2.0a9/pandasai/vectorstores/__init__.py
--rw-r--r--   0        0        0     2394 2024-02-21 10:04:57.992292 pandasai-2.0a9/pandasai/vectorstores/bamboo_vectorstore.py
--rw-r--r--   0        0        0    10443 2024-02-21 10:04:57.993289 pandasai-2.0a9/pandasai/vectorstores/chroma.py
--rw-r--r--   0        0        0     5764 2024-02-21 10:04:57.993455 pandasai-2.0a9/pandasai/vectorstores/vectorstore.py
--rw-r--r--   0        0        0     3203 2024-02-21 18:45:45.718011 pandasai-2.0a9/pyproject.toml
--rw-r--r--   0        0        0    10445 1970-01-01 00:00:00.000000 pandasai-2.0a9/PKG-INFO
+-rw-r--r--   0        0        0     1581 2024-02-29 15:48:26.870599 pandasai-2.1a1/LICENSE
+-rw-r--r--   0        0        0     5825 2024-05-19 03:18:51.906754 pandasai-2.1a1/README.md
+-rw-r--r--   0        0        0      694 2024-04-06 09:34:15.901079 pandasai-2.1a1/pandasai/__init__.py
+-rw-r--r--   0        0        0       87 2024-05-23 12:39:50.244054 pandasai-2.1a1/pandasai/agent/__init__.py
+-rw-r--r--   0        0        0     1845 2024-05-23 12:39:50.244348 pandasai-2.1a1/pandasai/agent/agent.py
+-rw-r--r--   0        0        0    15764 2024-05-23 12:39:50.244732 pandasai-2.1a1/pandasai/agent/base.py
+-rw-r--r--   0        0        0      998 2024-03-26 00:39:20.878687 pandasai-2.1a1/pandasai/agent/callbacks.py
+-rw-r--r--   0        0        0     1350 2024-03-26 00:39:17.325195 pandasai-2.1a1/pandasai/config.py
+-rw-r--r--   0        0        0      749 2024-05-18 23:37:12.274645 pandasai-2.1a1/pandasai/connectors/__init__.py
+-rw-r--r--   0        0        0     8777 2024-03-15 21:22:46.070796 pandasai-2.1a1/pandasai/connectors/airtable.py
+-rw-r--r--   0        0        0     8477 2024-05-23 12:39:50.245442 pandasai-2.1a1/pandasai/connectors/base.py
+-rw-r--r--   0        0        0     5235 2024-05-23 12:39:50.245662 pandasai-2.1a1/pandasai/connectors/pandas.py
+-rw-r--r--   0        0        0     4653 2024-03-09 00:53:54.916215 pandasai-2.1a1/pandasai/connectors/polars.py
+-rw-r--r--   0        0        0    21412 2024-05-23 12:39:50.246483 pandasai-2.1a1/pandasai/connectors/sql.py
+-rw-r--r--   0        0        0     5871 2024-02-29 15:48:26.887142 pandasai-2.1a1/pandasai/connectors/yahoo_finance.py
+-rw-r--r--   0        0        0     2138 2024-05-23 12:39:50.247070 pandasai-2.1a1/pandasai/constants.py
+-rw-r--r--   0        0        0     2183 2024-02-29 15:48:26.887398 pandasai-2.1a1/pandasai/ee/LICENSE
+-rw-r--r--   0        0        0     4797 2024-05-23 12:40:10.986075 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/__init__.py
+-rw-r--r--   0        0        0     1448 2024-05-23 12:39:50.247652 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/Semantic_prompt_generation.py
+-rw-r--r--   0        0        0     6296 2024-05-23 12:39:50.247789 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/code_generator.py
+-rw-r--r--   0        0        0     1790 2024-05-23 12:39:50.248036 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_correction_pipeline.py
+-rw-r--r--   0        0        0     3213 2024-05-23 12:39:50.248177 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py
+-rw-r--r--   0        0        0     1941 2024-05-23 12:39:50.248484 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/llm_call.py
+-rw-r--r--   0        0        0     2764 2024-05-23 12:39:50.248622 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/semantic_chat_pipeline.py
+-rw-r--r--   0        0        0     2380 2024-05-23 12:40:16.694534 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/validate_pipeline_input.py
+-rw-r--r--   0        0        0     1732 2024-05-23 12:39:50.248987 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/generate_df_schema.py
+-rw-r--r--   0        0        0     1193 2024-05-23 12:39:50.249098 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/semantic_agent_prompt.py
+-rw-r--r--   0        0        0     3289 2024-05-23 12:39:50.249263 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/generate_df_schema.tmpl
+-rw-r--r--   0        0        0       83 2024-05-23 12:40:20.998357 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/semantic_agent_prompt.tmpl
+-rw-r--r--   0        0        0       91 2024-05-23 12:39:50.249517 pandasai-2.1a1/pandasai/ee/agents/semantic_agent/prompts/templates/shared/dataframe.tmpl
+-rw-r--r--   0        0        0      418 2024-04-09 07:23:17.860885 pandasai-2.1a1/pandasai/ee/connectors/__init__.py
+-rw-r--r--   0        0        0     2835 2024-02-29 15:48:26.887730 pandasai-2.1a1/pandasai/ee/connectors/databricks.py
+-rw-r--r--   0        0        0     3449 2024-03-15 18:04:31.286624 pandasai-2.1a1/pandasai/ee/connectors/google_big_query.py
+-rw-r--r--   0        0        0      660 2024-04-11 10:03:28.499882 pandasai-2.1a1/pandasai/ee/connectors/relations.py
+-rw-r--r--   0        0        0     3862 2024-02-29 15:48:26.888047 pandasai-2.1a1/pandasai/ee/connectors/snowflake.py
+-rw-r--r--   0        0        0    15531 2024-05-23 12:39:50.249757 pandasai-2.1a1/pandasai/ee/helpers/query_builder.py
+-rw-r--r--   0        0        0      148 2024-03-26 00:39:20.879018 pandasai-2.1a1/pandasai/ee/vectorstores/__init__.py
+-rw-r--r--   0        0        0    10445 2024-02-29 15:48:26.888632 pandasai-2.1a1/pandasai/ee/vectorstores/chroma.py
+-rw-r--r--   0        0        0    14109 2024-03-26 00:39:20.879303 pandasai-2.1a1/pandasai/ee/vectorstores/qdrant.py
+-rw-r--r--   0        0        0      507 2024-02-21 10:04:57.970176 pandasai-2.1a1/pandasai/engine.py
+-rw-r--r--   0        0        0     5665 2024-05-23 12:39:50.250070 pandasai-2.1a1/pandasai/exceptions.py
+-rw-r--r--   0        0        0      446 2024-02-21 10:04:57.970515 pandasai-2.1a1/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4613 2024-02-21 10:04:57.971425 pandasai-2.1a1/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     3020 2024-05-18 23:34:01.413582 pandasai-2.1a1/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0     2397 2024-02-29 15:48:26.889696 pandasai-2.1a1/pandasai/helpers/data_sampler.py
+-rw-r--r--   0        0        0     5557 2024-04-11 10:03:28.500374 pandasai-2.1a1/pandasai/helpers/dataframe_serializer.py
+-rw-r--r--   0        0        0     5062 2024-02-21 10:04:57.972426 pandasai-2.1a1/pandasai/helpers/df_config_manager.py
+-rw-r--r--   0        0        0     1378 2024-04-02 18:08:09.250985 pandasai-2.1a1/pandasai/helpers/df_info.py
+-rw-r--r--   0        0        0     3244 2024-02-27 01:50:10.394311 pandasai-2.1a1/pandasai/helpers/df_validator.py
+-rw-r--r--   0        0        0      291 2024-04-06 07:25:25.510013 pandasai-2.1a1/pandasai/helpers/encoder.py
+-rw-r--r--   0        0        0      526 2024-02-21 10:04:57.973121 pandasai-2.1a1/pandasai/helpers/env.py
+-rw-r--r--   0        0        0      937 2024-03-09 00:53:54.917395 pandasai-2.1a1/pandasai/helpers/file_importer.py
+-rw-r--r--   0        0        0      725 2024-02-29 15:48:26.889894 pandasai-2.1a1/pandasai/helpers/folder.py
+-rw-r--r--   0        0        0     3717 2024-02-21 10:04:57.973750 pandasai-2.1a1/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     4282 2024-05-20 21:21:04.650404 pandasai-2.1a1/pandasai/helpers/logger.py
+-rw-r--r--   0        0        0     3415 2024-03-12 06:39:18.608291 pandasai-2.1a1/pandasai/helpers/memory.py
+-rw-r--r--   0        0        0      447 2023-09-13 09:35:53.943189 pandasai-2.1a1/pandasai/helpers/node_visitors.py
+-rw-r--r--   0        0        0      213 2023-11-20 22:14:04.734116 pandasai-2.1a1/pandasai/helpers/openai.py
+-rw-r--r--   0        0        0     6147 2024-05-18 23:34:01.416531 pandasai-2.1a1/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     4813 2024-05-05 22:29:39.907096 pandasai-2.1a1/pandasai/helpers/optional.py
+-rw-r--r--   0        0        0     1976 2024-02-21 10:04:57.974259 pandasai-2.1a1/pandasai/helpers/output_types/__init__.py
+-rw-r--r--   0        0        0     4658 2024-02-21 10:04:57.974363 pandasai-2.1a1/pandasai/helpers/output_types/_output_types.py
+-rw-r--r--   0        0        0     3708 2024-04-17 17:22:13.619024 pandasai-2.1a1/pandasai/helpers/output_validator.py
+-rw-r--r--   0        0        0     2074 2023-11-20 22:14:04.734712 pandasai-2.1a1/pandasai/helpers/path.py
+-rw-r--r--   0        0        0     8701 2024-05-23 12:39:50.250880 pandasai-2.1a1/pandasai/helpers/query_exec_tracker.py
+-rw-r--r--   0        0        0     2426 2024-04-17 17:22:13.619965 pandasai-2.1a1/pandasai/helpers/request.py
+-rw-r--r--   0        0        0     1061 2024-02-21 10:04:57.975042 pandasai-2.1a1/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     8579 2024-02-21 10:04:57.975494 pandasai-2.1a1/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     2388 2024-04-06 08:15:23.614472 pandasai-2.1a1/pandasai/helpers/skills_manager.py
+-rw-r--r--   0        0        0      306 2024-03-18 23:35:50.459950 pandasai-2.1a1/pandasai/helpers/sql.py
+-rw-r--r--   0        0        0      629 2024-04-26 07:56:14.443046 pandasai-2.1a1/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     7002 2024-03-02 20:32:32.838102 pandasai-2.1a1/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0      624 2024-04-19 09:31:18.969118 pandasai-2.1a1/pandasai/llm/bamboo_llm.py
+-rw-r--r--   0        0        0    13479 2024-05-18 23:34:01.417400 pandasai-2.1a1/pandasai/llm/base.py
+-rw-r--r--   0        0        0     5543 2024-05-18 23:34:01.417873 pandasai-2.1a1/pandasai/llm/bedrock_claude.py
+-rw-r--r--   0        0        0      640 2024-02-29 15:48:26.892045 pandasai-2.1a1/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     2974 2024-03-15 16:20:10.659958 pandasai-2.1a1/pandasai/llm/google_gemini.py
+-rw-r--r--   0        0        0     2757 2024-03-08 19:32:57.678201 pandasai-2.1a1/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     5697 2024-03-08 19:30:08.686882 pandasai-2.1a1/pandasai/llm/google_vertexai.py
+-rw-r--r--   0        0        0     4003 2024-02-29 15:48:26.892474 pandasai-2.1a1/pandasai/llm/huggingface_text_gen.py
+-rw-r--r--   0        0        0     5408 2024-04-26 07:56:14.443204 pandasai-2.1a1/pandasai/llm/ibm_watsonx.py
+-rw-r--r--   0        0        0     1611 2024-03-08 19:30:31.656234 pandasai-2.1a1/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     1419 2024-03-12 19:49:27.179633 pandasai-2.1a1/pandasai/llm/local_llm.py
+-rw-r--r--   0        0        0     3403 2024-05-18 23:34:01.418842 pandasai-2.1a1/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      352 2024-02-28 20:30:56.697841 pandasai-2.1a1/pandasai/pandas/__init__.py
+-rw-r--r--   0        0        0      206 2024-02-29 15:48:26.893218 pandasai-2.1a1/pandasai/pipelines/__init__.py
+-rw-r--r--   0        0        0      353 2023-11-20 22:14:04.741653 pandasai-2.1a1/pandasai/pipelines/abstract_pipeline.py
+-rw-r--r--   0        0        0     1062 2024-02-29 15:48:26.893519 pandasai-2.1a1/pandasai/pipelines/base_logic_unit.py
+-rw-r--r--   0        0        0     1438 2024-02-29 15:48:26.893959 pandasai-2.1a1/pandasai/pipelines/chat/cache_lookup.py
+-rw-r--r--   0        0        0     1253 2024-02-29 15:48:26.894044 pandasai-2.1a1/pandasai/pipelines/chat/cache_population.py
+-rw-r--r--   0        0        0      572 2024-02-29 15:48:26.894142 pandasai-2.1a1/pandasai/pipelines/chat/chat_pipeline_input.py
+-rw-r--r--   0        0        0    18703 2024-05-23 12:39:50.251896 pandasai-2.1a1/pandasai/pipelines/chat/code_cleaning.py
+-rw-r--r--   0        0        0    15802 2024-04-19 09:12:27.360978 pandasai-2.1a1/pandasai/pipelines/chat/code_execution.py
+-rw-r--r--   0        0        0      626 2024-03-09 00:53:51.900905 pandasai-2.1a1/pandasai/pipelines/chat/code_execution_pipeline_input.py
+-rw-r--r--   0        0        0     1473 2024-02-29 15:48:26.894619 pandasai-2.1a1/pandasai/pipelines/chat/code_generator.py
+-rw-r--r--   0        0        0     1638 2024-04-17 17:22:13.622513 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
+-rw-r--r--   0        0        0      240 2024-02-29 15:48:26.894831 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
+-rw-r--r--   0        0        0     3213 2024-03-15 21:22:46.071716 pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
+-rw-r--r--   0        0        0    10679 2024-05-23 12:39:50.252333 pandasai-2.1a1/pandasai/pipelines/chat/generate_chat_pipeline.py
+-rw-r--r--   0        0        0     2258 2024-02-29 15:48:26.895146 pandasai-2.1a1/pandasai/pipelines/chat/prompt_generation.py
+-rw-r--r--   0        0        0     2157 2024-03-08 19:22:54.336427 pandasai-2.1a1/pandasai/pipelines/chat/result_parsing.py
+-rw-r--r--   0        0        0     1828 2024-02-29 15:48:26.895371 pandasai-2.1a1/pandasai/pipelines/chat/result_validation.py
+-rw-r--r--   0        0        0     1994 2024-05-23 12:39:50.252632 pandasai-2.1a1/pandasai/pipelines/chat/validate_pipeline_input.py
+-rw-r--r--   0        0        0      612 2024-02-29 15:48:26.895631 pandasai-2.1a1/pandasai/pipelines/logic_unit_output.py
+-rw-r--r--   0        0        0      422 2024-02-21 10:04:57.983209 pandasai-2.1a1/pandasai/pipelines/logic_units/code_executor.py
+-rw-r--r--   0        0        0      900 2024-02-21 10:04:57.983722 pandasai-2.1a1/pandasai/pipelines/logic_units/output_logic_unit.py
+-rw-r--r--   0        0        0      511 2024-02-21 10:04:57.984328 pandasai-2.1a1/pandasai/pipelines/logic_units/prompt_execution.py
+-rw-r--r--   0        0        0     5833 2024-05-23 12:39:50.253446 pandasai-2.1a1/pandasai/pipelines/pipeline.py
+-rw-r--r--   0        0        0     1783 2024-05-23 12:39:50.253690 pandasai-2.1a1/pandasai/pipelines/pipeline_context.py
+-rw-r--r--   0        0        0      232 2024-02-29 15:48:26.896427 pandasai-2.1a1/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     2098 2024-05-23 12:39:50.254517 pandasai-2.1a1/pandasai/prompts/base.py
+-rw-r--r--   0        0        0      207 2024-02-29 15:48:26.896838 pandasai-2.1a1/pandasai/prompts/check_if_relevant_to_conversation.py
+-rw-r--r--   0        0        0      518 2024-02-29 15:48:26.896953 pandasai-2.1a1/pandasai/prompts/clarification_questions_prompt.py
+-rw-r--r--   0        0        0      902 2024-02-29 15:48:26.897330 pandasai-2.1a1/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0      975 2024-02-29 15:48:26.898228 pandasai-2.1a1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
+-rw-r--r--   0        0        0     1058 2024-02-29 15:48:26.898521 pandasai-2.1a1/pandasai/prompts/correct_output_type_error_prompt.py
+-rw-r--r--   0        0        0     1904 2024-03-09 00:53:54.918124 pandasai-2.1a1/pandasai/prompts/direct_sql_prompt.py
+-rw-r--r--   0        0        0      159 2024-02-29 15:48:26.898919 pandasai-2.1a1/pandasai/prompts/explain_prompt.py
+-rw-r--r--   0        0        0     1274 2024-02-21 10:04:57.989230 pandasai-2.1a1/pandasai/prompts/file_based_prompt.py
+-rw-r--r--   0        0        0      879 2024-02-29 15:48:26.899086 pandasai-2.1a1/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      268 2024-02-29 15:48:26.899212 pandasai-2.1a1/pandasai/prompts/generate_python_code_with_sql.py
+-rw-r--r--   0        0        0      189 2024-02-29 15:48:26.899664 pandasai-2.1a1/pandasai/prompts/generate_system_message.py
+-rw-r--r--   0        0        0      172 2024-02-29 15:48:26.899949 pandasai-2.1a1/pandasai/prompts/rephase_query_prompt.py
+-rw-r--r--   0        0        0      199 2024-02-29 15:48:26.900245 pandasai-2.1a1/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
+-rw-r--r--   0        0        0      571 2024-02-29 15:48:26.900559 pandasai-2.1a1/pandasai/prompts/templates/clarification_questions_prompt.tmpl
+-rw-r--r--   0        0        0      342 2024-02-29 15:48:26.900738 pandasai-2.1a1/pandasai/prompts/templates/correct_error_prompt.tmpl
+-rw-r--r--   0        0        0      356 2024-02-29 15:48:26.900820 pandasai-2.1a1/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
+-rw-r--r--   0        0        0      343 2024-02-29 15:48:26.900888 pandasai-2.1a1/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
+-rw-r--r--   0        0        0      325 2024-02-29 15:48:26.901074 pandasai-2.1a1/pandasai/prompts/templates/explain.tmpl
+-rw-r--r--   0        0        0      923 2024-03-28 17:45:03.638878 pandasai-2.1a1/pandasai/prompts/templates/generate_python_code.tmpl
+-rw-r--r--   0        0        0     1311 2024-04-06 08:15:29.233436 pandasai-2.1a1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
+-rw-r--r--   0        0        0      176 2024-02-29 15:48:26.901720 pandasai-2.1a1/pandasai/prompts/templates/generate_system_message.tmpl
+-rw-r--r--   0        0        0      387 2024-02-29 15:48:26.901838 pandasai-2.1a1/pandasai/prompts/templates/rephrase_query.tmpl
+-rw-r--r--   0        0        0      123 2024-04-02 18:08:09.251668 pandasai-2.1a1/pandasai/prompts/templates/shared/dataframe.tmpl
+-rw-r--r--   0        0        0      916 2024-02-29 15:48:26.902116 pandasai-2.1a1/pandasai/prompts/templates/shared/output_type_template.tmpl
+-rw-r--r--   0        0        0      624 2024-02-29 15:48:26.902323 pandasai-2.1a1/pandasai/prompts/templates/shared/vectordb_docs.tmpl
+-rw-r--r--   0        0        0      102 2024-02-27 01:50:10.394612 pandasai-2.1a1/pandasai/pydantic/__init__.py
+-rw-r--r--   0        0        0      311 2024-02-21 10:04:57.990280 pandasai-2.1a1/pandasai/responses/__init__.py
+-rw-r--r--   0        0        0      637 2024-02-29 15:48:26.902758 pandasai-2.1a1/pandasai/responses/context.py
+-rw-r--r--   0        0        0     2159 2024-04-06 07:25:25.512293 pandasai-2.1a1/pandasai/responses/response_parser.py
+-rw-r--r--   0        0        0     1593 2024-04-11 10:03:31.648509 pandasai-2.1a1/pandasai/responses/response_serializer.py
+-rw-r--r--   0        0        0       96 2024-02-29 15:48:26.903015 pandasai-2.1a1/pandasai/responses/response_type.py
+-rw-r--r--   0        0        0     1036 2024-02-21 10:04:57.991273 pandasai-2.1a1/pandasai/responses/streamlit_response.py
+-rw-r--r--   0        0        0       16 2023-09-04 21:53:07.396618 pandasai-2.1a1/pandasai/schemas/__init__.py
+-rw-r--r--   0        0        0     1305 2024-04-13 15:58:12.089425 pandasai-2.1a1/pandasai/schemas/df_config.py
+-rw-r--r--   0        0        0     3920 2024-02-29 15:48:26.903634 pandasai-2.1a1/pandasai/skills/__init__.py
+-rw-r--r--   0        0        0     8894 2024-05-23 12:39:50.255046 pandasai-2.1a1/pandasai/smart_dataframe/__init__.py
+-rw-r--r--   0        0        0     6256 2024-05-23 12:39:50.255362 pandasai-2.1a1/pandasai/smart_datalake/__init__.py
+-rw-r--r--   0        0        0      193 2024-02-29 15:48:26.904302 pandasai-2.1a1/pandasai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2705 2024-04-02 18:08:09.251824 pandasai-2.1a1/pandasai/vectorstores/bamboo_vectorstore.py
+-rw-r--r--   0        0        0     5764 2024-02-29 15:48:26.904463 pandasai-2.1a1/pandasai/vectorstores/vectorstore.py
+-rw-r--r--   0        0        0     3813 2024-05-23 12:43:33.427720 pandasai-2.1a1/pyproject.toml
+-rw-r--r--   0        0        0     9608 1970-01-01 00:00:00.000000 pandasai-2.1a1/PKG-INFO
```

### Comparing `pandasai-2.0a9/README.md` & `pandasai-2.1a1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,114 +1,110 @@
-# PandasAI 🐼
+# ![PandasAI](images/logo.png)
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
 [![Coverage](https://codecov.io/gh/gventuri/pandas-ai/branch/main/graph/badge.svg)](https://codecov.io/gh/gventuri/pandas-ai)
-[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
 
-PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
+PandasAI is a Python library that makes it easy to ask questions to your data in natural language. It helps you to explore, clean, and analyze your data using generative AI.
 
-<!-- Add images/pandas-ai.png -->
+# 🔧 Getting started
 
-![PandasAI](images/pandas-ai.png?raw=true)
+The documentation for PandasAI to use it with specific LLMs, vector stores and connectors, can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
 
-## 🔧 Quick install
+## 📦 Installation
+
+With pip:
 
 ```bash
 pip install pandasai
 ```
 
-## 🔍 Demo
+With poetry:
 
-Try out PandasAI in your browser:
+```bash
+poetry add pandasai
+```
 
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
+## 🔍 Demo
 
-## 📖 Documentation
+Try out PandasAI yourself in your browser:
 
-The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
 
-## 💻 Usage
+# 🚀 Deploying PandasAI
 
-> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
+PandasAI can be deployed in a variety of ways. You can easily use it in your Jupyter notebooks or streamlit apps, or you can deploy it as a REST API such as with FastAPI or Flask.
 
-PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
+If you are interested in managed PandasAI Cloud or self-hosted Enterprise Offering, take a look at [our website](https://pandas-ai.com) or [book a meeting with us](https://zcal.co/gventuri/pandas-ai-demo).
 
-### Queries
+## 💻 Usage
 
-For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
+### Ask questions
 
 ```python
+import os
 import pandas as pd
-from pandasai import SmartDataframe
+from pandasai import Agent
 
 # Sample DataFrame
-df = pd.DataFrame({
+sales_by_country = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
-    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+    "sales": [5000, 3200, 2900, 4100, 2300, 2100, 2500, 2600, 4500, 7000]
 })
 
-# Instantiate a LLM
-from pandasai.llm import OpenAI
-llm = OpenAI(api_token="YOUR_API_TOKEN")
+# By default, unless you choose a different LLM, it will use BambooLLM.
+# You can get your free API key signing up at https://pandabi.ai (you can also configure it in your .env file)
+os.environ["PANDASAI_API_KEY"] = "YOUR_API_KEY"
 
-df = SmartDataframe(df, config={"llm": llm})
-df.chat('Which are the 5 happiest countries?')
+agent = Agent(sales_by_country)
+agent.chat('Which are the top 5 countries by sales?')
 ```
 
-The above code will return the following:
-
 ```
-6            Canada
-7         Australia
-1    United Kingdom
-3           Germany
-0     United States
-Name: country, dtype: object
+China, United States, Japan, Germany, Australia
 ```
 
-Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
+---
+
+Or you can ask more complex questions:
 
 ```python
-df.chat('What is the sum of the GDPs of the 2 unhappiest countries?')
+agent.chat(
+    "What is the total sales for the top 3 countries by sales?"
+)
 ```
 
-The above code will return the following:
-
 ```
-19012600725504
+The total sales for the top 3 countries by sales is 16500.
 ```
 
-### Charts
+### Visualize charts
 
-You can also ask PandasAI to draw a graph:
+You can also ask PandasAI to generate charts for you:
 
 ```python
-df.chat(
+agent.chat(
     "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
-You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
-
 ### Multiple DataFrames
 
-Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
+You can also pass in multiple dataframes to PandasAI and ask questions relating them.
 
 ```python
+import os
 import pandas as pd
-from pandasai import SmartDatalake
-from pandasai.llm import OpenAI
+from pandasai import Agent
 
 employees_data = {
     'EmployeeID': [1, 2, 3, 4, 5],
     'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
     'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
 }
 
@@ -116,70 +112,47 @@
     'EmployeeID': [1, 2, 3, 4, 5],
     'Salary': [5000, 6000, 4500, 7000, 5500]
 }
 
 employees_df = pd.DataFrame(employees_data)
 salaries_df = pd.DataFrame(salaries_data)
 
+# By default, unless you choose a different LLM, it will use BambooLLM.
+# You can get your free API key signing up at https://pandabi.ai (you can also configure it in your .env file)
+os.environ["PANDASAI_API_KEY"] = "YOUR_API_KEY"
 
-llm = OpenAI()
-dl = SmartDatalake([employees_df, salaries_df], config={"llm": llm})
-dl.chat("Who gets paid the most?")
+agent = Agent([employees_df, salaries_df])
+agent.chat("Who gets paid the most?")
 ```
 
-The above code will return the following:
-
 ```
-Oh, Olivia gets paid the most.
+Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
-### ⚡️ Shortcuts
-
-PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
-
-```python
-# Clean data
-df.clean_data()
+## 🔒 Privacy & Security
 
-# Impute missing values
-df.impute_missing_values()
+In order to generate the Python code to run, we take some random samples from the dataframe, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the randomized head to the LLM.
 
-# Generate features
-df.generate_features()
+If you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-# Plot histogram
-df.plot_histogram(column="gdp")
-```
+## 📜 License
 
-Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
+PandasAI is available under the MIT expat license, except for the `pandasai/ee` directory (which has it's [license here](https://github.com/Sinaptik-AI/pandas-ai/blob/master/pandasai/ee/LICENSE) if applicable.
 
-## 🔒 Privacy & Security
+If you are interested in managed PandasAI Cloud or self-hosted Enterprise Offering, take a look at [our website](https://pandas-ai.com) or [book a meeting with us](https://zcal.co/gventuri/pandas-ai-demo).
 
-In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
+## Resources
 
-Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
+- [Docs](https://pandas-ai.readthedocs.io/en/latest/) for comprehensive documentation
+- [Examples](examples) for example notebooks
+- [Discord](https://discord.gg/kF7FqH2FwS) for discussion with the community and PandasAI team
 
 ## 🤝 Contributing
 
-Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
-For more information, please see the [contributing guidelines](CONTRIBUTING.md).
+Contributions are welcome! Please check the outstanding issues and feel free to open a pull request.
+For more information, please check out the [contributing guidelines](CONTRIBUTING.md).
 
-After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
-
-```bash
-pre-commit install
-```
-
-## Contributors
+### Thank you!
 
 [![Contributors](https://contrib.rocks/image?repo=gventuri/pandas-ai)](https://github.com/gventuri/pandas-ai/graphs/contributors)
-
-## 📜 License
-
-PandasAI is licensed under the MIT License. See the LICENSE file for more details.
-
-## Acknowledgements
-
-- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
-- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
```

### Comparing `pandasai-2.0a9/pandasai/__init__.py` & `pandasai-2.1a1/pandasai/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from .skills import skill
 
 __version__ = importlib.metadata.version(__package__ or __name__)
 
 
 def clear_cache(filename: str = None):
     """Clear the cache"""
-    cache = Cache(filename or "cache_db")
+    cache = Cache(filename) if filename else Cache()
+
     cache.clear()
 
 
 __all__ = [
     "Agent",
     "clear_cache",
     "skill",
```

### Comparing `pandasai-2.0a9/pandasai/agent/base.py` & `pandasai-2.1a1/pandasai/agent/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,144 +1,140 @@
 import json
+import os
 import uuid
-from typing import List, Optional, Type, Union
+from typing import List, Optional, Union
 
-import pandas as pd
-
-from pandasai.pipelines.chat.chat_pipeline_input import (
-    ChatPipelineInput,
+import pandasai.pandas as pd
+from pandasai.llm.bamboo_llm import BambooLLM
+from pandasai.pipelines.chat.chat_pipeline_input import ChatPipelineInput
+from pandasai.pipelines.chat.code_execution_pipeline_input import (
+    CodeExecutionPipelineInput,
 )
 from pandasai.vectorstores.vectorstore import VectorStore
 
 from ..config import load_config_from_json
 from ..connectors import BaseConnector, PandasConnector
 from ..constants import DEFAULT_CACHE_DIRECTORY, DEFAULT_CHART_DIRECTORY
-from ..exceptions import InvalidLLMOutputType
+from ..exceptions import InvalidLLMOutputType, MissingVectorStoreError
 from ..helpers.df_info import df_type
 from ..helpers.folder import Folder
 from ..helpers.logger import Logger
 from ..helpers.memory import Memory
 from ..llm.base import LLM
-from ..llm.langchain import LangchainLLM
-from ..pipelines.chat.generate_chat_pipeline import (
-    GenerateChatPipeline,
-)
+from ..llm.langchain import LangchainLLM, is_langchain_llm
 from ..pipelines.pipeline_context import PipelineContext
 from ..prompts.base import BasePrompt
 from ..prompts.check_if_relevant_to_conversation import (
     CheckIfRelevantToConversationPrompt,
 )
 from ..prompts.clarification_questions_prompt import ClarificationQuestionPrompt
 from ..prompts.explain_prompt import ExplainPrompt
 from ..prompts.rephase_query_prompt import RephraseQueryPrompt
 from ..schemas.df_config import Config
 from ..skills import Skill
 from .callbacks import Callbacks
 
 
-class Agent:
+class BaseAgent:
     """
-    Agent class to improve the conversational experience in PandasAI
+    Base Agent class to improve the conversational experience in PandasAI
     """
 
     def __init__(
         self,
         dfs: Union[
             pd.DataFrame, BaseConnector, List[Union[pd.DataFrame, BaseConnector]]
         ],
         config: Optional[Union[Config, dict]] = None,
         memory_size: Optional[int] = 10,
-        pipeline: Optional[Type[GenerateChatPipeline]] = None,
         vectorstore: Optional[VectorStore] = None,
         description: str = None,
     ):
         """
         Args:
-            df (Union[pd.DataFrame, List[pd.DataFrame]]): Pandas dataframe
+            df (Union[pd.DataFrame, List[pd.DataFrame]]): Pandas or Modin dataframe
             Polars or Database connectors
             memory_size (int, optional): Conversation history to use during chat.
             Defaults to 1.
         """
         self.last_prompt = None
         self.last_prompt_id = None
         self.last_result = None
         self.last_code_generated = None
         self.last_code_executed = None
         self.agent_info = description
 
         self.conversation_id = uuid.uuid4()
 
-        dfs = self.get_dfs(dfs)
-
-        self._vectorstore = vectorstore
+        self.dfs = self.get_dfs(dfs)
 
         # Instantiate the context
-        config = self.get_config(config)
+        self.config = self.get_config(config)
         self.context = PipelineContext(
-            dfs=dfs,
-            config=config,
+            dfs=self.dfs,
+            config=self.config,
             memory=Memory(memory_size, agent_info=description),
             vectorstore=vectorstore,
         )
 
         # Instantiate the logger
-        self.logger = Logger(save_logs=config.save_logs, verbose=config.verbose)
-
-        callbacks = Callbacks(self)
-
-        self.chat_pipeline = (
-            pipeline(
-                self.context,
-                self.logger,
-                on_prompt_generation=callbacks.on_prompt_generation,
-                on_code_generation=callbacks.on_code_generation,
-                on_code_execution=callbacks.on_code_execution,
-                on_result=callbacks.on_result,
-            )
-            if pipeline
-            else GenerateChatPipeline(
-                self.context,
-                self.logger,
-                on_prompt_generation=callbacks.on_prompt_generation,
-                on_code_generation=callbacks.on_code_generation,
-                on_code_execution=callbacks.on_code_execution,
-                on_result=callbacks.on_result,
-            )
+        self.logger = Logger(
+            save_logs=self.config.save_logs, verbose=self.config.verbose
         )
 
+        # Instantiate the vectorstore
         self._vectorstore = vectorstore
 
+        if self._vectorstore is None and os.environ.get("PANDASAI_API_KEY"):
+            try:
+                from pandasai.vectorstores.bamboo_vectorstore import BambooVectorStore
+            except ImportError as e:
+                raise ImportError(
+                    "Could not import BambooVectorStore. Please install the required dependencies."
+                ) from e
+
+            self._vectorstore = BambooVectorStore(logger=self.logger)
+            self.context.vectorstore = self._vectorstore
+
+        self._callbacks = Callbacks(self)
+
         self.configure()
 
-    def configure(self):
-        config = self.context.config
+        self.pipeline = None
 
+    def configure(self):
         # Add project root path if save_charts_path is default
-        if config.save_charts and config.save_charts_path == DEFAULT_CHART_DIRECTORY:
-            Folder.create(config.save_charts_path)
+        if (
+            self.config.save_charts
+            and self.config.save_charts_path == DEFAULT_CHART_DIRECTORY
+        ):
+            Folder.create(self.config.save_charts_path)
 
         # Add project root path if cache_path is default
-        if config.enable_cache:
+        if self.config.enable_cache:
             Folder.create(DEFAULT_CACHE_DIRECTORY)
 
     def get_config(self, config: Union[Config, dict]):
         """
         Load a config to be used to run the queries.
 
         Args:
             config (Union[Config, dict]): Config to be used
         """
 
         config = load_config_from_json(config)
 
-        if isinstance(config, dict) and config.get("llm") is None:
+        if isinstance(config, dict) and config.get("llm") is not None:
             config["llm"] = self.get_llm(config["llm"])
 
         config = Config(**config)
 
+        if config.llm is None:
+            config.llm = BambooLLM()
+
         return config
 
     def get_llm(self, llm: LLM) -> LLM:
         """
         Load a LLM to be used to run the queries.
         Check if it is a PandasAI LLM or a Langchain LLM.
         If it is a Langchain LLM, wrap it in a PandasAI LLM.
@@ -146,15 +142,15 @@
         Args:
             llm (object): LLMs option to be used for API access
 
         Raises:
             BadImportError: If the LLM is a Langchain LLM but the langchain package
             is not installed
         """
-        if LangchainLLM.is_langchain_llm(llm):
+        if is_langchain_llm(llm):
             llm = LangchainLLM(llm)
 
         return llm
 
     def get_dfs(
         self,
         dfs: Union[
@@ -233,27 +229,95 @@
                     raise
                 retry_count += 1
 
     def chat(self, query: str, output_type: Optional[str] = None):
         """
         Simulate a chat interaction with the assistant on Dataframe.
         """
+        if not self.pipeline:
+            return (
+                "Unfortunately, I was not able to get your answers, "
+                "because of the following error: No pipeline exists"
+            )
+
         try:
             self.logger.log(f"Question: {query}")
             self.logger.log(
                 f"Running PandasAI with {self.context.config.llm.type} LLM..."
             )
 
             self.assign_prompt_id()
 
             pipeline_input = ChatPipelineInput(
                 query, output_type, self.conversation_id, self.last_prompt_id
             )
 
-            return self.chat_pipeline.run(pipeline_input)
+            return self.pipeline.run(pipeline_input)
+        except Exception as exception:
+            return (
+                "Unfortunately, I was not able to get your answers, "
+                "because of the following error:\n"
+                f"\n{exception}\n"
+            )
+
+    def generate_code(self, query: str, output_type: Optional[str] = None):
+        """
+        Simulate code generation with the assistant on Dataframe.
+        """
+        if not self.pipeline:
+            return (
+                "Unfortunately, I was not able to get your answers, "
+                "because of the following error: No pipeline exists"
+            )
+        try:
+            self.logger.log(f"Question: {query}")
+            self.logger.log(
+                f"Running PandasAI with {self.context.config.llm.type} LLM..."
+            )
+
+            self.assign_prompt_id()
+
+            pipeline_input = ChatPipelineInput(
+                query, output_type, self.conversation_id, self.last_prompt_id
+            )
+
+            return self.pipeline.run_generate_code(pipeline_input)
+        except Exception as exception:
+            return (
+                "Unfortunately, I was not able to get your answers, "
+                "because of the following error:\n"
+                f"\n{exception}\n"
+            )
+
+    def execute_code(
+        self, code: Optional[str] = None, output_type: Optional[str] = None
+    ):
+        """
+        Execute code Generated with the assistant on Dataframe.
+        """
+        if not self.pipeline:
+            return (
+                "Unfortunately, I was not able to get your answers, "
+                "because of the following error: No pipeline exists to execute try Agent class"
+            )
+        try:
+            if code is None:
+                code = self.last_code_generated
+            self.logger.log(f"Code: {code}")
+            self.logger.log(
+                f"Running PandasAI with {self.context.config.llm.type} LLM..."
+            )
+
+            self.assign_prompt_id()
+
+            pipeline_input = CodeExecutionPipelineInput(
+                code, output_type, self.conversation_id, self.last_prompt_id
+            )
+
+            return self.pipeline.run_execute_code(pipeline_input)
         except Exception as exception:
             return (
                 "Unfortunately, I was not able to get your answers, "
                 "because of the following error:\n"
                 f"\n{exception}\n"
             )
 
@@ -265,28 +329,21 @@
     ) -> None:
         """
         Trains the context to be passed to model
         Args:
             queries (Optional[str], optional): user user
             codes (Optional[str], optional): generated code
             docs (Optional[List[str]], optional): additional docs
-
         Raises:
             ImportError: if default vector db lib is not installed it raises an error
         """
         if self._vectorstore is None:
-            try:
-                from pandasai.vectorstores.bamboo_vectorstore import BambooVectorStore
-            except ImportError as e:
-                raise ImportError(
-                    "Could not import chromadb. Please install it with `pip install chromadb`."
-                ) from e
-
-            self._vectorstore = BambooVectorStore(logger=self.logger)
-            self.context.vectorstore = self._vectorstore
+            raise MissingVectorStoreError(
+                "No vector store provided. Please provide a vector store to train the agent."
+            )
 
         if (queries is not None and codes is None) or (
             queries is None and codes is not None
         ):
             raise ValueError(
                 "If either queries or codes are provided, both must be provided."
             )
@@ -413,12 +470,12 @@
 
     @property
     def logs(self):
         return self.logger.logs
 
     @property
     def last_error(self):
-        return self.chat_pipeline.last_error
+        raise NotImplementedError
 
     @property
     def last_query_log_id(self):
-        return self.chat_pipeline.get_last_track_log_id()
+        raise NotImplementedError
```

### Comparing `pandasai-2.0a9/pandasai/agent/callbacks.py` & `pandasai-2.1a1/pandasai/agent/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         A method to be called after code generation.
 
         Args:
             code (str): A python code
         """
         self.agent.last_code_generated = code
 
-    def on_code_execution(self, code: str):
+    def before_code_execution(self, code: str):
         """
         A method to be called after code execution.
 
         Args:
             code (str): A python code
         """
         self.agent.last_code_executed = code
```

### Comparing `pandasai-2.0a9/pandasai/config.py` & `pandasai-2.1a1/pandasai/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         with open(find_closest("pandasai.json"), "r") as f:
             config = json.load(f)
 
             # if config is a dict
             if config.get("llm") and not override_config.get("llm"):
                 options = config.get("llm_options") or {}
                 config["llm"] = getattr(llm, config["llm"])(**options)
+            elif not config.get("llm") and not override_config.get("llm"):
+                config["llm"] = llm.BambooLLM()
     except FileNotFoundError:
         # Ignore the error if the file does not exist, will use the default config
         pass
 
     if override_config:
         config.update(override_config)
```

### Comparing `pandasai-2.0a9/pandasai/connectors/__init__.py` & `pandasai-2.1a1/pandasai/connectors/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 Connectors are used to connect to databases, external APIs, and other data sources.
 
 The connectors package contains all the connectors that are used by the application.
 """
 
 from .airtable import AirtableConnector
 from .base import BaseConnector
-from .databricks import DatabricksConnector
-from .google_big_query import GoogleBigQueryConnector
 from .pandas import PandasConnector
 from .polars import PolarsConnector
-from .snowflake import SnowFlakeConnector
-from .sql import MySQLConnector, PostgreSQLConnector, SQLConnector, SqliteConnector
+from .sql import (
+    MySQLConnector,
+    OracleConnector,
+    PostgreSQLConnector,
+    SQLConnector,
+    SqliteConnector,
+)
 from .yahoo_finance import YahooFinanceConnector
 
 __all__ = [
     "BaseConnector",
     "SQLConnector",
     "MySQLConnector",
     "PostgreSQLConnector",
     "YahooFinanceConnector",
-    "SnowFlakeConnector",
-    "DatabricksConnector",
     "AirtableConnector",
     "SqliteConnector",
     "PandasConnector",
     "PolarsConnector",
-    "GoogleBigQueryConnector",
+    "OracleConnector",
 ]
```

### Comparing `pandasai-2.0a9/pandasai/connectors/airtable.py` & `pandasai-2.1a1/pandasai/connectors/airtable.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/connectors/base.py` & `pandasai-2.1a1/pandasai/connectors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 Base connector class to be extended by all connectors.
 """
 
 import json
 import os
 from abc import ABC, abstractmethod
 from functools import cache
-from typing import Union
-
-from pydantic import BaseModel
+from typing import TYPE_CHECKING, List, Optional, Union
 
 import pandasai.pandas as pd
 from pandasai.helpers.dataframe_serializer import (
     DataframeSerializer,
     DataframeSerializerType,
 )
+from pandasai.pydantic import BaseModel
 
 from ..helpers.logger import Logger
 
+if TYPE_CHECKING:
+    from pandasai.ee.connectors.relations import AbstractRelation
+
 
 class BaseConnectorConfig(BaseModel):
     """
     Base Connector configuration.
     """
 
     database: str
     table: str
     where: list[list[str]] = None
+    connect_args: Optional[dict] = {}
 
 
 class BaseConnector(ABC):
     """
     Base connector class to be extended by all connectors.
     """
 
@@ -40,14 +43,15 @@
     def __init__(
         self,
         config: Union[BaseConnectorConfig, dict],
         name: str = None,
         description: str = None,
         custom_head: pd.DataFrame = None,
         field_descriptions: dict = None,
+        connector_relations: List["AbstractRelation"] = None,
     ):
         """
         Initialize the connector with the given configuration.
 
         Args:
             config (dict): The configuration for the connector.
         """
@@ -55,14 +59,15 @@
             config = self._load_connector_config(config)
 
         self.config = config
         self.name = name
         self.description = description
         self.custom_head = custom_head
         self.field_descriptions = field_descriptions
+        self.connector_relations = connector_relations
 
     def _load_connector_config(self, config: Union[BaseConnectorConfig, dict]):
         """Loads passed Configuration to object
 
         Args:
             config (BaseConnectorConfig): Construct config in structure
 
@@ -186,14 +191,18 @@
     @property
     def pandas_df(self):
         """
         Returns the pandas dataframe
         """
         raise NotImplementedError
 
+    @property
+    def type(self):
+        return "pd.DataFrame"
+
     def equals(self, other):
         return self.__dict__ == other.__dict__
 
     @cache
     def get_head(self, n: int = 3) -> pd.DataFrame:
         """
         Return the head of the data source that the connector is connected to.
@@ -221,15 +230,15 @@
         """
         df_trunc = self.get_head().copy()
 
         for col in df_trunc.columns:
             if df_trunc[col].dtype == "object":
                 first_val = df_trunc[col].iloc[0]
                 if isinstance(first_val, str) and len(first_val) > max_size:
-                    df_trunc[col] = df_trunc[col].str.slice(0, max_size - 3) + "..."
+                    df_trunc[col] = f"{df_trunc[col].str.slice(0, max_size - 3)}..."
 
         return df_trunc
 
     @cache
     def get_schema(self) -> pd.DataFrame:
         """
         A sample of the dataframe.
@@ -257,32 +266,41 @@
 
     @cache
     def to_string(
         self,
         index: int = 0,
         is_direct_sql: bool = False,
         serializer: DataframeSerializerType = None,
+        enforce_privacy: bool = False,
     ) -> str:
         """
         Convert dataframe to string
         Returns:
             str: dataframe string
         """
+        # If field descriptions are added always use YML. Other formats don't support field descriptions yet
+        if self.field_descriptions or self.connector_relations:
+            serializer = DataframeSerializerType.YML
+
         return DataframeSerializer().serialize(
             self,
             extras={
                 "index": index,
-                "type": "sql" if is_direct_sql else "pd.DataFrame",
+                "type": "pd.DataFrame",
                 "is_direct_sql": is_direct_sql,
+                "enforce_privacy": enforce_privacy,
             },
             type_=serializer,
         )
 
     @cache
     def to_json(self):
         df_head = self.get_head()
 
         return {
             "name": self.name,
             "description": self.description,
             "head": json.loads(df_head.to_json(orient="records", date_format="iso")),
         }
+
+    def register_enable_sql_query(self, table_name=None):
+        raise NotImplementedError
```

### Comparing `pandasai-2.0a9/pandasai/connectors/databricks.py` & `pandasai-2.1a1/pandasai/ee/connectors/databricks.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 Azure, AWS and GCP
 """
 
 from typing import Union
 
 from sqlalchemy import create_engine
 
-from .base import BaseConnectorConfig
-from .sql import SQLBaseConnectorConfig, SQLConnector
+from ...connectors.base import BaseConnectorConfig
+from ...connectors.sql import SQLBaseConnectorConfig, SQLConnector
 
 
 class DatabricksConnectorConfig(SQLBaseConnectorConfig):
     """
     Connector configuration for DataBricks.
     """
 
@@ -81,19 +81,17 @@
             f"database={self.config.database} httpPath={str(self.config.httpPath)}"
         )
 
     def equals(self, other):
         if isinstance(other, self.__class__):
             return (
                 self.config.dialect,
-                self.config.token,
                 self.config.host,
                 self.config.port,
                 self.config.httpPath,
             ) == (
                 other.config.dialect,
-                other.config.token,
                 other.config.host,
                 other.config.port,
                 other.config.httpPath,
             )
         return False
```

### Comparing `pandasai-2.0a9/pandasai/connectors/pandas.py` & `pandasai-2.1a1/pandasai/connectors/polars.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,137 +1,159 @@
 """
-Pandas connector class to handle csv, parquet, xlsx files and pandas dataframes.
+Polars connector class to handle csv, parquet, xlsx files and polars dataframes.
 """
 
-import hashlib
 from functools import cache, cached_property
-from typing import Union
-
-from pydantic import BaseModel
+from typing import TYPE_CHECKING, Any, Union
 
 import pandasai.pandas as pd
 
+# Use a conditional import for type checking
+if TYPE_CHECKING:
+    try:
+        import polars as pl
+
+        PolarsDataFrame = pl.DataFrame
+        PolarsSeries = pl.Series
+    except ImportError:
+        PolarsDataFrame = Any
+        PolarsSeries = Any
+else:
+    PolarsDataFrame = Any
+    PolarsSeries = Any
+
+from pydantic import BaseModel
+
 from ..helpers.data_sampler import DataSampler
 from ..helpers.file_importer import FileImporter
 from ..helpers.logger import Logger
 from .base import BaseConnector
 
 
-class PandasConnectorConfig(BaseModel):
+class PolarsConnectorConfig(BaseModel):
     """
-    Pandas Connector configuration.
+    Polars Connector configuration.
     """
 
-    original_df: Union[pd.DataFrame, pd.Series, str, list, dict]
+    original_df: PolarsDataFrame
 
     class Config:
         arbitrary_types_allowed = True
 
 
-class PandasConnector(BaseConnector):
+class PolarsConnector(BaseConnector):
     """
-    Pandas connector class to handle csv, parquet, xlsx files and pandas dataframes.
+    Polars connector class to handle csv, parquet, xlsx files and polars dataframes.
     """
 
     pandas_df = pd.DataFrame
     _logger: Logger = None
     _additional_filters: list[list[str]] = None
 
     def __init__(
         self,
-        config: Union[PandasConnectorConfig, dict],
+        config: Union[PolarsConnectorConfig, dict],
         **kwargs,
     ):
         """
-        Initialize the Pandas connector with the given configuration.
+        Initialize the Polars connector with the given configuration.
 
         Args:
-            config (PandasConnectorConfig): The configuration for the Pandas connector.
+            config (PolarsConnectorConfig): The configuration for the Polars connector.
         """
+
         super().__init__(config, **kwargs)
 
         self._load_df(self.config.original_df)
 
-    def _load_df(self, df: Union[pd.DataFrame, pd.Series, str, list, dict]):
+    def _load_df(self, df: Union[PolarsDataFrame, PolarsSeries, str, dict]):
         """
-        Load the dataframe from a file or pandas dataframe.
+        Load the dataframe from a file or polars dataframe.
 
         Args:
-            df (Union[pd.DataFrame, pd.Series, str, list, dict]): The dataframe to load.
+            df (Union[pl.DataFrame, pl.Series, str, dict]): The dataframe to load.
         """
-        if isinstance(df, pd.Series):
-            self.pandas_df = df.to_frame()
-        elif isinstance(df, pd.DataFrame):
-            self.pandas_df = df
-        elif isinstance(df, (list, dict)):
+        polars_df = None
+        if isinstance(df, pl.Series):
+            polars_df = df.to_frame()
+        elif isinstance(df, pl.DataFrame):
+            polars_df = df
+        elif isinstance(df, str):
+            polars_df = FileImporter.import_from_file(df)
+        elif isinstance(df, dict):
             try:
-                self.pandas_df = pd.DataFrame(df)
+                polars_df = pl.DataFrame(df)
             except Exception as e:
                 raise ValueError(
                     "Invalid input data. We cannot convert it to a dataframe."
                 ) from e
-        elif isinstance(df, str):
-            self.pandas_df = FileImporter.import_from_file(df)
         else:
             raise ValueError("Invalid input data. We cannot convert it to a dataframe.")
 
+        self.pandas_df = polars_df.to_pandas()
+
     def _load_connector_config(
-        self, config: Union[PandasConnectorConfig, dict]
-    ) -> PandasConnectorConfig:
+        self, config: Union[PolarsConnectorConfig, dict]
+    ) -> PolarsConnectorConfig:
         """
         Loads passed Configuration to object
 
         Args:
-            config (PandasConnectorConfig): Construct config in structure
+            config (PolarsConnectorConfig): Construct config in structure
 
             Returns:
-                config: PandasConnectorConfig
+                config: PolarsConnectorConfig
         """
-        return PandasConnectorConfig(**config)
+        return PolarsConnectorConfig(**config)
 
     @cache
-    def head(self, n: int = 5) -> pd.DataFrame:
+    def head(self, n: int = 5) -> PolarsDataFrame:
         """
         Return the head of the data source that the connector is connected to.
         This information is passed to the LLM to provide the schema of the
         data source.
         """
+        if self.pandas_df is None:
+            return None
+
         sampler = DataSampler(self.pandas_df)
         return sampler.sample(n)
 
     @cache
-    def execute(self) -> pd.DataFrame:
+    def execute(self) -> PolarsDataFrame:
         """
         Execute the given query on the data source that the connector is
         connected to.
         """
         return self.pandas_df
 
     @cached_property
     def rows_count(self):
         """
         Return the number of rows in the data source that the connector is
         connected to.
         """
-        return len(self.pandas_df)
+        return len(self.pandas_df) if self.pandas_df.index else 0
 
     @cached_property
     def columns_count(self):
         """
         Return the number of columns in the data source that the connector is
         connected to.
         """
-        return len(self.pandas_df.columns)
+        return len(self.pandas_df.columns) if self.pandas_df.columns else 0
 
     @property
     def column_hash(self):
         """
         Return the hash code that is unique to the columns of the data source
         that the connector is connected to.
         """
+        import hashlib
+
         columns_str = "".join(self.pandas_df.columns)
         hash_object = hashlib.sha256(columns_str.encode())
         return hash_object.hexdigest()
 
     @cached_property
     def path(self):
         """
@@ -141,14 +163,7 @@
 
     @property
     def fallback_name(self):
         """
         Return the name of the table that the connector is connected to.
         """
         pass
-
-    def equals(self, other: BaseConnector):
-        """
-        Return whether the data source that the connector is connected to is
-        equal to the other data source.
-        """
-        return self._original_df.equals(other._original_df)
```

### Comparing `pandasai-2.0a9/pandasai/connectors/snowflake.py` & `pandasai-2.1a1/pandasai/ee/connectors/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from functools import cache
 from typing import Union
 
 from sqlalchemy import create_engine
 
 import pandasai.pandas as pd
 
-from .base import BaseConnectorConfig
-from .sql import SQLBaseConnectorConfig, SQLConnector
+from ...connectors.base import BaseConnectorConfig
+from ...connectors.sql import SQLBaseConnectorConfig, SQLConnector
 
 
 class SnowFlakeConnectorConfig(SQLBaseConnectorConfig):
     """
     Connector configuration for SnowFlake.
     """
 
@@ -111,17 +111,17 @@
             f"table={self.config.table}>"
         )
 
     def equals(self, other):
         if isinstance(other, self.__class__):
             return (
                 self.config.dialect,
+                self.config.dbSchema,
+                self.config.warehouse,
                 self.config.account,
-                self.config.username,
-                self.config.password,
             ) == (
                 other.config.dialect,
+                other.config.dbSchema,
+                other.config.warehouse,
                 other.config.account,
-                other.config.username,
-                other.config.password,
             )
         return False
```

### Comparing `pandasai-2.0a9/pandasai/connectors/sql.py` & `pandasai-2.1a1/pandasai/connectors/sql.py`

 * *Files 8% similar despite different names*

```diff
@@ -105,29 +105,32 @@
             config (SQLConnectorConfig): Configurations to load database
 
         """
 
         if config.driver:
             self._engine = create_engine(
                 f"{config.dialect}+{config.driver}://{config.username}:{config.password}"
-                f"@{config.host}:{str(config.port)}/{config.database}"
+                f"@{config.host}:{str(config.port)}/{config.database}",
+                connect_args=config.connect_args,
             )
         else:
             self._engine = create_engine(
                 f"{config.dialect}://{config.username}:{config.password}@{config.host}"
-                f":{str(config.port)}/{config.database}"
+                f":{str(config.port)}/{config.database}",
+                connect_args=config.connect_args,
             )
 
         self._connection = self._engine.connect()
 
     def __del__(self):
         """
         Close the connection to the SQL database.
         """
-        self._connection.close()
+        if self._connection:
+            self._connection.close()
 
     def __repr__(self):
         """
         Return the string representation of the SQL connector.
 
         Returns:
             str: The string representation of the SQL connector.
@@ -141,15 +144,15 @@
 
     def _validate_column_name(self, column_name):
         regex = r"^[a-zA-Z0-9_]+$"
         if not re.match(regex, column_name):
             raise ValueError(f"Invalid column name: {column_name}")
 
     def _build_query(self, limit=None, order=None):
-        base_query = select("*").select_from(text(self.config.table))
+        base_query = select("*").select_from(text(self.cs_table_name))
         if self.config.where or self._additional_filters:
             # conditions is the list of where + additional filters
             conditions = []
             if self.config.where:
                 conditions += self.config.where
             if self._additional_filters:
                 conditions += self._additional_filters
@@ -322,15 +325,15 @@
             self.logger.log(
                 "Getting the number of rows in the table "
                 f"{self.config.table} using dialect "
                 f"{self.config.dialect}"
             )
 
         # Run a SQL query to get the number of rows
-        query = select(text("COUNT(*)")).select_from(text(self.config.table))
+        query = select(text("COUNT(*)")).select_from(text(self.cs_table_name))
 
         # Return the number of rows
         self._rows_count = self._connection.execute(query).fetchone()[0]
         return self._rows_count
 
     @cached_property
     def columns_count(self):
@@ -406,23 +409,19 @@
     def equals(self, other):
         if isinstance(other, self.__class__):
             return (
                 self.config.dialect,
                 self.config.driver,
                 self.config.host,
                 self.config.port,
-                self.config.username,
-                self.config.password,
             ) == (
                 other.config.dialect,
                 other.config.driver,
                 other.config.host,
                 other.config.port,
-                other.config.username,
-                other.config.password,
             )
         return False
 
     def _is_sql_query_safe(self, query: str):
         infected_keywords = [
             r"\bINSERT\b",
             r"\bUPDATE\b",
@@ -439,14 +438,22 @@
 
     def execute_direct_sql_query(self, sql_query):
         if not self._is_sql_query_safe(sql_query):
             raise MaliciousQueryError("Malicious query is generated in code")
 
         return pd.read_sql(sql_query, self._connection)
 
+    @property
+    def cs_table_name(self):
+        return self.config.table
+
+    @property
+    def type(self):
+        return self.config.dialect
+
 
 class SqliteConnector(SQLConnector):
     """
     Sqlite connector are used to connect to Sqlite databases.
     """
 
     def __init__(
@@ -490,15 +497,16 @@
         self._engine = create_engine(f"{config.dialect}:///{config.database}")
         self._connection = self._engine.connect()
 
     def __del__(self):
         """
         Close the connection to the SQL database.
         """
-        self._connection.close()
+        if self._connection:
+            self._connection.close()
 
     @cache
     def head(self, n: int = 5) -> pd.DataFrame:
         """
         Return the head of the data source that the connector is connected to.
         This information is passed to the LLM to provide the schema of the data source.
 
@@ -514,27 +522,46 @@
 
         # Run a SQL query to get all the columns names and 5 random rows
         query = self._build_query(limit=n, order="RANDOM()")
 
         # Return the head of the data source
         return pd.read_sql(query, self._connection)
 
+    @property
+    def cs_table_name(self):
+        return f'"{self.config.table}"'
+
     def __repr__(self):
         """
         Return the string representation of the SQL connector.
 
         Returns:
             str: The string representation of the SQL connector.
         """
         return (
             f"<{self.__class__.__name__} dialect={self.config.dialect} "
             f"database={self.config.database} "
             f"table={self.config.table}>"
         )
 
+    def equals(self, other):
+        if isinstance(other, self.__class__):
+            print(self.config.database)
+            print(other.config.database)
+            return (
+                self.config.dialect,
+                self.config.driver,
+                self.config.database,
+            ) == (
+                other.config.dialect,
+                other.config.driver,
+                other.config.database,
+            )
+        return False
+
 
 class MySQLConnector(SQLConnector):
     """
     MySQL connectors are used to connect to MySQL databases.
     """
 
     def __init__(
@@ -576,15 +603,17 @@
     ):
         """
         Initialize the PostgreSQL connector with the given configuration.
 
         Args:
             config (ConnectorConfig): The configuration for the PostgreSQL connector.
         """
-        config["dialect"] = "postgresql"
+        if "dialect" not in config:
+            config["dialect"] = "postgresql"
+
         config["driver"] = "psycopg2"
 
         if isinstance(config, dict):
             postgresql_env_vars = {
                 "host": "POSTGRESQL_HOST",
                 "port": "POSTGRESQL_PORT",
                 "database": "POSTGRESQL_DATABASE",
@@ -612,7 +641,73 @@
             )
 
         # Run a SQL query to get all the columns names and 5 random rows
         query = self._build_query(limit=n, order="RANDOM()")
 
         # Return the head of the data source
         return pd.read_sql(query, self._connection)
+
+    @property
+    def cs_table_name(self):
+        return f'"{self.config.table}"'
+
+    def execute_direct_sql_query(self, sql_query):
+        sql_query = sql_query.replace("`", '"')
+        return super().execute_direct_sql_query(sql_query)
+
+
+class OracleConnector(SQLConnector):
+    """
+    Oracle connectors are used to connect to Oracle databases.
+    """
+
+    def __init__(
+        self,
+        config: Union[SQLConnectorConfig, dict],
+        **kwargs,
+    ):
+        """
+        Initialize the Oracle connector with the given configuration.
+
+        Args:
+            config (ConnectorConfig): The configuration for the Oracle connector.
+        """
+        config["dialect"] = "oracle"
+        config["driver"] = "cx_oracle"
+
+        if isinstance(config, dict):
+            oracle_env_vars = {
+                "host": "ORACLE_HOST",
+                "port": "ORACLE_PORT",
+                "database": "ORACLE_DATABASE",
+                "username": "ORACLE_USERNAME",
+                "password": "ORACLE_PASSWORD",
+            }
+            config = self._populate_config_from_env(config, oracle_env_vars)
+
+        super().__init__(config, **kwargs)
+
+    @cache
+    def head(self, n: int = 5) -> pd.DataFrame:
+        """
+        Return the head of the data source that the connector is connected to.
+        This information is passed to the LLM to provide the schema of the data source.
+
+        Returns:
+            DataFrame: The head of the data source.
+        """
+
+        if self.logger:
+            self.logger.log(
+                f"Getting head of {self.config.table} "
+                f"using dialect {self.config.dialect}"
+            )
+
+        # Run a SQL query to get all the columns names and 5 random rows
+        query = self._build_query(limit=n, order="dbms_random.value")
+
+        # Return the head of the data source
+        return pd.read_sql(query, self._connection)
+
+    @property
+    def cs_table_name(self):
+        return f'"{self.config.table}"'
```

### Comparing `pandasai-2.0a9/pandasai/connectors/yahoo_finance.py` & `pandasai-2.1a1/pandasai/connectors/yahoo_finance.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/constants.py` & `pandasai-2.1a1/pandasai/constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Constants used in the pandasai package.
 
 It includes Start & End Code tags, Whitelisted Python Packages and
 While List Builtin Methods.
 
 """
+
 # Default directory to store chart if user doesn't provide any
 DEFAULT_CHART_DIRECTORY = "exports/charts"
 
 # Default directory for cache
 DEFAULT_CACHE_DIRECTORY = "cache"
 
 # Default permissions for files and directories
@@ -94,8 +95,17 @@
     "datetime",
     "json",
     "io",
     "base64",
     "scipy",
     "streamlit",
     "modin",
+    "scikit-learn",
 ]
+
+PANDASBI_SETUP_MESSAGE = (
+    "The api_key client option must be set either by passing api_key to the client "
+    "or by setting the PANDASAI_API_KEY environment variable. To get the key follow below steps:\n"
+    "1. Go to https://www.pandabi.ai and sign up\n"
+    "2. From settings go to API keys and copy\n"
+    "3. Set environment variable like os.environ['PANDASAI_API_KEY'] = '$2a$10$flb7....'"
+)
```

### Comparing `pandasai-2.0a9/pandasai/exceptions.py` & `pandasai-2.1a1/pandasai/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """PandasAI's custom exceptions.
 
 This module contains the implementation of Custom Exceptions.
 
 """
 
+from pandasai.constants import PANDASBI_SETUP_MESSAGE
+
 
 class InvalidRequestError(Exception):
     """
     Raised when the request is not successful.
 
     Args :
         Exception (Exception): InvalidRequestError
@@ -182,39 +184,65 @@
     """
     Raise error if the output type is invalid
     Args:
         Exception (Exception): InvalidLLMOutputType
     """
 
 
+class InvalidOutputValueMismatch(Exception):
+    """
+    Raise error if the output value doesn't match with type
+    Args:
+        Exception (Exception): InvalidOutputValueMismatch
+    """
+
+
 class ExecuteSQLQueryNotUsed(Exception):
     """
     Raise error if Execute SQL Query is not used
     Args:
         Exception (Exception): ExecuteSQLQueryNotUsed
     """
 
 
+class PipelineConcatenationError(Exception):
+    """
+    Raise error if vector store is not found
+    Args:
+        Exception (Exception): Concatenating wrong pipelines
+    """
+
+
+class MissingVectorStoreError(Exception):
+    """
+    Raise error if vector store is not found
+    Args:
+        Exception (Exception): MissingVectorStoreError
+    """
+
+
 class PandasAIApiKeyError(Exception):
     """
     Raise error if api key is not found for remote vectorstore and llm
     Args:
         Exception (Exception): PandasAIApiKeyError
     """
 
     def __init__(self):
-        message = (
-            "The api_key client option must be set either by passing api_key to the client "
-            "or by setting the PANDASAI_API_KEY environment variable. To get the key follow below steps:\n"
-            "1. Go to https://domer.ai and sign up\n"
-            "2. From settings go to API keys and copy\n"
-            "3. Set environment variable like os.environ['PANDASAI_API_KEY'] = '$2a$10$flb7....'"
-        )
+        message = PANDASBI_SETUP_MESSAGE
         super().__init__(message)
 
 
 class PandasAIApiCallError(Exception):
     """
     Raise error if exception in API request fails
     Args:
         Exception (Exception): PandasAIApiCallError
     """
+
+
+class PandasConnectorTableNotFound(Exception):
+    """
+    Raise error if exception in API request fails
+    Args:
+        Exception (Exception): PandasConnectorTableNotFound
+    """
```

### Comparing `pandasai-2.0a9/pandasai/helpers/anonymizer.py` & `pandasai-2.1a1/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/cache.py` & `pandasai-2.1a1/pandasai/helpers/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """Cache class for caching queries. It is used to cache queries
     to save time and money.
 
     Args:
         filename (str): filename to store the cache.
     """
 
-    def __init__(self, filename="cache_db_0.9", abs_path=None):
+    def __init__(self, filename="cache_db_0.10", abs_path=None):
         # Define cache directory and create directory if it does not exist
         if abs_path:
             cache_dir = abs_path
         else:
             try:
                 cache_dir = os.path.join(find_project_root(), "cache")
             except ValueError:
```

### Comparing `pandasai-2.0a9/pandasai/helpers/data_sampler.py` & `pandasai-2.1a1/pandasai/helpers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/df_config_manager.py` & `pandasai-2.1a1/pandasai/helpers/df_config_manager.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/df_info.py` & `pandasai-2.1a1/pandasai/helpers/df_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/df_validator.py` & `pandasai-2.1a1/pandasai/helpers/df_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict, List
 
-from pydantic import BaseModel, ValidationError
-
 from pandasai.helpers.df_info import DataFrameType, df_type
+from pandasai.pydantic import BaseModel, ValidationError
 
 
 class DfValidationResult:
     """
     Validation results for a dataframe.
 
     Attributes:
```

### Comparing `pandasai-2.0a9/pandasai/helpers/env.py` & `pandasai-2.1a1/pandasai/helpers/env.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/file_importer.py` & `pandasai-2.1a1/pandasai/helpers/file_importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import pandas as pd
+import pandasai.pandas as pd
 
 from .from_google_sheets import from_google_sheets
 
 
 class FileImporter:
     """
     Class to import a dataframe from a file (csv, parquet, xlsx)
```

### Comparing `pandasai-2.0a9/pandasai/helpers/folder.py` & `pandasai-2.1a1/pandasai/helpers/folder.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/from_google_sheets.py` & `pandasai-2.1a1/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/logger.py` & `pandasai-2.1a1/pandasai/helpers/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 import inspect
 import logging
 import sys
 import time
 from typing import List
 
-from pydantic import BaseModel
+from pandasai.pydantic import BaseModel
 
 from .path import find_closest
 
 
 class Log(BaseModel):
     """Log class"""
```

### Comparing `pandasai-2.0a9/pandasai/helpers/memory.py` & `pandasai-2.1a1/pandasai/helpers/memory.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,14 +75,33 @@
         for message in self.all():
             if message["is_user"]:
                 messages.append({"role": "user", "message": message["message"]})
             else:
                 messages.append({"role": "assistant", "message": message["message"]})
         return messages
 
+    def to_openai_messages(self):
+        """
+        Returns the conversation messages in the format expected by the OpenAI API
+        """
+        messages = []
+        if self.agent_info:
+            messages.append(
+                {
+                    "role": "system",
+                    "content": self.get_system_prompt(),
+                }
+            )
+        for message in self.all():
+            if message["is_user"]:
+                messages.append({"role": "user", "content": message["message"]})
+            else:
+                messages.append({"role": "assistant", "content": message["message"]})
+        return messages
+
     def clear(self):
         self._messages = []
 
     @property
     def size(self):
         return self._memory_size
```

### Comparing `pandasai-2.0a9/pandasai/helpers/openai_info.py` & `pandasai-2.1a1/pandasai/helpers/openai_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,22 +5,26 @@
 MODEL_COST_PER_1K_TOKENS = {
     # GPT-4 input
     "gpt-4": 0.03,
     "gpt-4-0613": 0.03,
     "gpt-4-turbo-preview": 0.01,
     "gpt-4-0125-preview": 0.01,
     "gpt-4-1106-preview": 0.01,
+    "gpt-4o": 0.005,
+    "gpt-4o-2024-05-13": 0.005,
     "gpt-4-32k": 0.06,
     "gpt-4-32k-0613": 0.06,
     # GPT-4 output
     "gpt-4-completion": 0.06,
     "gpt-4-0613-completion": 0.06,
     "gpt-4-turbo-preview-completion": 0.03,
     "gpt-4-0125-preview-completion": 0.03,
     "gpt-4-1106-preview-completion": 0.03,
+    "gpt-4o-completion": 0.015,
+    "gpt-4o-2024-05-13-completion": 0.015,
     "gpt-4-32k-completion": 0.12,
     "gpt-4-32k-0613-completion": 0.12,
     # GPT-3.5 input
     "gpt-3.5-turbo": 0.0005,
     "gpt-3.5-turbo-0125": 0.0005,
     "gpt-3.5-turbo-1106": 0.0005,
     "gpt-3.5-turbo-0613": 0.0005,
```

### Comparing `pandasai-2.0a9/pandasai/helpers/optional.py` & `pandasai-2.1a1/pandasai/helpers/optional.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Module to import optional dependencies.
 
 Source: Taken from pandas/compat/_optional.py
 """
+
 from __future__ import annotations
 
 import importlib
 import sys
 import warnings
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, List
 
+import matplotlib.pyplot as plt
+import numpy as np
 from pandas.util.version import Version
 
+import pandasai.pandas as pd
+from pandasai.constants import WHITELISTED_BUILTINS
+
 if TYPE_CHECKING:
     import types
 
 # Minimum version required for each optional dependency
 
 VERSIONS = {
     "sklearn": "1.2.2",
@@ -38,14 +44,40 @@
 
     if version is None:
         raise ImportError(f"Can't determine version for {module.__name__}")
 
     return version
 
 
+def get_environment(additional_deps: List[dict]) -> dict:
+    """
+    Returns the environment for the code to be executed.
+
+    Returns (dict): A dictionary of environment variables
+    """
+    return {
+        "pd": pd,
+        "plt": plt,
+        "np": np,
+        **{
+            lib["alias"]: (
+                getattr(import_dependency(lib["module"]), lib["name"])
+                if hasattr(import_dependency(lib["module"]), lib["name"])
+                else import_dependency(lib["module"])
+            )
+            for lib in additional_deps
+        },
+        "__builtins__": {
+            **{builtin: __builtins__[builtin] for builtin in WHITELISTED_BUILTINS},
+            "__build_class__": __build_class__,
+            "__name__": "__main__",
+        },
+    }
+
+
 def import_dependency(
     name: str,
     extra: str = "",
     errors: str = "raise",
     min_version: str | None = None,
 ):
     """
```

### Comparing `pandasai-2.0a9/pandasai/helpers/output_types/__init__.py` & `pandasai-2.1a1/pandasai/helpers/output_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/output_types/_output_types.py` & `pandasai-2.1a1/pandasai/helpers/output_types/_output_types.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/path.py` & `pandasai-2.1a1/pandasai/helpers/path.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/query_exec_tracker.py` & `pandasai-2.1a1/pandasai/helpers/query_exec_tracker.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 from collections import defaultdict
 from typing import Any, List, TypedDict, Union
 
 import requests
 
 from pandasai.connectors import BaseConnector
+from pandasai.helpers.encoder import CustomEncoder
 from pandasai.pipelines.chat.chat_pipeline_input import (
     ChatPipelineInput,
 )
 from pandasai.pipelines.pipeline_context import PipelineContext
 
 
 class ResponseType(TypedDict):
@@ -42,14 +43,15 @@
 
     def __init__(
         self,
         server_config: Union[dict, None] = None,
     ) -> None:
         self._success = False
         self._start_time = None
+        self._last_log_id = None
         self._server_config = server_config
         self._query_info = {}
 
     def start_new_track(self, input: ChatPipelineInput):
         """
         Resets tracking variables to start new track
         """
@@ -66,15 +68,22 @@
             "conversation_id": str(input.conversation_id),
             "instance": "Agent",
             "query": input.query,
             "output_type": input.output_type,
         }
 
     def convert_dataframe_to_dict(self, df):
-        json_data = json.loads(df.to_json(orient="split", date_format="iso"))
+        json_data = json.loads(
+            df.to_json(
+                orient="split",
+                date_format="iso",
+                default_handler=str,
+                force_ascii=False,
+            )
+        )
         return {"headers": json_data["columns"], "rows": json_data["data"]}
 
     def add_dataframes(self, dfs: List[BaseConnector]) -> None:
         """
         Add used dataframes for the query to query exec tracker
         Args:
             dfs (List[BaseConnector]): List of dataframes
@@ -227,34 +236,39 @@
         Publish Query Summary to remote logging server
         """
         api_key = None
         server_url = None
 
         if self._server_config is None:
             server_url = os.environ.get("PANDASAI_API_URL", "https://api.domer.ai")
-            api_key = os.environ.get("PANDASAI_API_KEY")
+            api_key = os.environ.get("PANDASAI_API_KEY") or None
         else:
             server_url = self._server_config.get(
                 "server_url", os.environ.get("PANDASAI_API_URL", "https://api.domer.ai")
             )
             api_key = self._server_config.get(
                 "api_key", os.environ.get("PANDASAI_API_KEY")
             )
 
-        if api_key is None or server_url is None:
+        if api_key is None:
             return
 
         try:
             log_data = {
                 "json_log": self.get_summary(),
             }
 
+            encoder = CustomEncoder()
+            ecoded_json_str = encoder.encode(log_data)
+
             headers = {"Authorization": f"Bearer {api_key}"}
             response = requests.post(
-                f"{server_url}/api/log/add", json=log_data, headers=headers
+                f"{server_url}/api/log/add",
+                json=json.loads(ecoded_json_str),
+                headers=headers,
             )
             if response.status_code != 200:
                 raise Exception(response.text)
 
             json_data = json.loads(response.text)
 
             if "data" in json_data and json_data["data"] is not None:
```

### Comparing `pandasai-2.0a9/pandasai/helpers/request.py` & `pandasai-2.1a1/pandasai/helpers/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,21 @@
     _endpoint_url: str
     _logger: Logger
 
     def __init__(
         self, endpoint_url: str = None, api_key: str = None, logger: Logger = None
     ) -> None:
         if api_key is None:
-            api_key = os.environ.get("PANDASAI_API_KEY")
+            api_key = os.environ.get("PANDASAI_API_KEY") or None
         if api_key is None:
             raise PandasAIApiKeyError()
         self._api_key = api_key
 
         if endpoint_url is None:
-            endpoint_url = os.environ.get("PANDASAI_API_URL")
-        if endpoint_url is None:
-            endpoint_url = "https://api.domer.ai"
+            endpoint_url = os.environ.get("PANDASAI_API_URL", "https://api.domer.ai")
 
         self._endpoint_url = endpoint_url
         self._version_path = "/api"
         self._logger = logger or Logger()
 
     def get(self, path=None, **kwargs):
         return self.make_request("GET", path, **kwargs)["data"]
@@ -65,15 +63,15 @@
                 params=params,
                 data=data,
                 json=json,
                 timeout=timeout,
             )
 
             data = response.json()
-            if response.status_code == 400:
+            if response.status_code not in [200, 201]:
                 raise PandasAIApiCallError(data["message"])
 
             return data
 
         except requests.exceptions.RequestException as e:
             self._logger.log(f"Request failed: {traceback.format_exc()}", logging.ERROR)
             raise PandasAIApiCallError(f"Request failed: {e}") from e
```

### Comparing `pandasai-2.0a9/pandasai/helpers/save_chart.py` & `pandasai-2.1a1/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/shortcuts.py` & `pandasai-2.1a1/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/helpers/skills_manager.py` & `pandasai-2.1a1/pandasai/helpers/skills_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,11 +74,11 @@
     def prompt_display(self) -> Optional[str]:
         """
         Displays skills for prompt
         """
         if len(self.skills) == 0:
             return None
 
-        return f"You can call the following functions that have been pre-defined for you:\n{self}"
+        return f"You are already provided with the following functions that you can call:\n{self}"
 
     def to_object(self) -> str:
         return [skill.stringify() for skill in self.skills]
```

### Comparing `pandasai-2.0a9/pandasai/llm/azure_openai.py` & `pandasai-2.1a1/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/llm/bamboo_llm.py` & `pandasai-2.1a1/pandasai/llm/bamboo_llm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from typing import Optional
 
-from pandasai.helpers.request import Session
-from pandasai.llm.base import LLM
-from pandasai.pipelines.pipeline_context import PipelineContext
-from pandasai.prompts.base import BasePrompt
+from ..helpers.request import Session
+from ..prompts.base import BasePrompt
+from .base import LLM
 
 
 class BambooLLM(LLM):
     _session: Session
 
     def __init__(
         self, endpoint_url: Optional[str] = None, api_key: Optional[str] = None
     ):
         self._session = Session(endpoint_url=endpoint_url, api_key=api_key)
 
-    def call(self, instruction: BasePrompt, context: PipelineContext = None) -> str:
+    def call(self, instruction: BasePrompt, _context=None) -> str:
         data = instruction.to_json()
         response = self._session.post("/llm/chat", json=data)
         return response["data"]
 
     @property
     def type(self) -> str:
         return "bamboo_llm"
```

### Comparing `pandasai-2.0a9/pandasai/llm/base.py` & `pandasai-2.1a1/pandasai/llm/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     from .base import BaseOpenAI
 
     class CustomLLM(BaseOpenAI):
 
         Custom Class Starts here!!
     ```
 """
+
 from __future__ import annotations
 
 import ast
 import re
 from abc import abstractmethod
 from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Tuple, Union
 
@@ -64,15 +65,15 @@
 
         """
         raise APIKeyNotFoundError("Type has not been implemented")
 
     def _polish_code(self, code: str) -> str:
         """
         Polish the code by removing the leading "python" or "py",  \
-        removing the imports and removing trailing spaces and new lines.
+        removing surrounding '`' characters  and removing trailing spaces and new lines.
 
         Args:
             code (str): A string of Python code.
 
         Returns:
             str: Polished code.
 
@@ -111,17 +112,21 @@
             NoCodeFoundError: No code found in the response
 
         Returns:
             str: Extracted code from the response
 
         """
         code = response
-        if len(code.split(separator)) > 1:
+
+        # If separator is in the response then we want the code in between only
+        if separator in response and len(code.split(separator)) > 1:
             code = code.split(separator)[1]
         code = self._polish_code(code)
+
+        # Even if the separator is not in the response, the output might still be valid python code
         if not self._is_python_code(code):
             raise NoCodeFoundError("No code found in the response")
 
         return code
 
     def prepend_system_prompt(self, prompt: BasePrompt, memory: Memory):
         """
@@ -289,14 +294,15 @@
 
         return {**openai_creds, **self._default_params}
 
     @property
     def _client_params(self) -> Dict[str, any]:
         return {
             "api_key": self.api_token,
+            "base_url": self.api_base,
             "timeout": self.request_timeout,
             "max_retries": self.max_retries,
             "default_headers": self.default_headers,
             "default_query": self.default_query,
             "http_client": self.http_client,
         }
 
@@ -334,31 +340,15 @@
         Args:
             value (str): Prompt
 
         Returns:
             str: LLM response.
 
         """
-        messages = []
-        if memory:
-            if memory.agent_info:
-                messages.append(
-                    {
-                        "role": "system",
-                        "content": memory.get_system_prompt(),
-                    }
-                )
-
-            for message in memory.all():
-                if message["is_user"]:
-                    messages.append({"role": "user", "content": message["message"]})
-                else:
-                    messages.append(
-                        {"role": "assistant", "content": message["message"]}
-                    )
+        messages = memory.to_openai_messages() if memory else []
 
         # adding current prompt as latest query message
         messages.append(
             {
                 "role": "user",
                 "content": value,
             },
@@ -449,15 +439,15 @@
         if self.top_k is not None and not 0 <= self.top_k <= 100:
             raise ValueError("top_k must be in the range [0.0, 100.0]")
 
         if self.max_output_tokens is not None and self.max_output_tokens <= 0:
             raise ValueError("max_output_tokens must be greater than zero")
 
     @abstractmethod
-    def _generate_text(self, prompt: str, memory: Memory) -> str:
+    def _generate_text(self, prompt: str, memory: Optional[Memory] = None) -> str:
         """
         Generates text for prompt, specific to implementation.
 
         Args:
             prompt (str): A string representation of the prompt.
 
         Returns:
```

### Comparing `pandasai-2.0a9/pandasai/llm/fake.py` & `pandasai-2.1a1/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/llm/google_gemini.py` & `pandasai-2.1a1/pandasai/llm/google_gemini.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 https://ai.google.dev/docs/gemini_api_overview.
 
 Example:
     Use below example to call GoogleGemini Model
 
     >>> from pandasai.llm.google_gemini import GoogleGemini
 """
-from typing import Any
+from typing import Any, Optional
 
 from ..exceptions import APIKeyNotFoundError
+from ..helpers.memory import Memory
 from ..helpers.optional import import_dependency
 from .base import BaseGoogle
 
 
 class GoogleGemini(BaseGoogle):
     """Google Gemini LLM
     BaseGoogle class is extended for Google Gemini model. The default and only model
@@ -67,33 +68,39 @@
         """
 
         super()._validate()
 
         if not self.model:
             raise ValueError("model is required.")
 
-    def _generate_text(self, prompt: str) -> str:
+    def _generate_text(self, prompt: str, memory: Optional[Memory] = None) -> str:
         """
         Generates text for prompt.
 
         Args:
             prompt (str): A string representation of the prompt.
 
         Returns:
             str: LLM response.
 
         """
         self._validate()
+        updated_prompt = self.prepend_system_prompt(prompt, memory)
 
-        completion = self.google.GoogleGemini.generate_content(
+        self.last_prompt = updated_prompt
+        completion = self.google_gemini.generate_content(
             contents=prompt,
-            temperature=self.temperature,
-            top_p=self.top_p,
-            top_k=self.top_k,
-            max_output_tokens=self.max_output_tokens,
+            generation_config=dict(
+                {
+                    "temperature": self.temperature,
+                    "top_p": self.top_p,
+                    "top_k": self.top_k,
+                    "max_output_tokens": self.max_output_tokens,
+                }
+            ),
         )
 
         return completion.text
 
     @property
     def type(self) -> str:
         return "google-gemini"
```

### Comparing `pandasai-2.0a9/pandasai/llm/google_palm.py` & `pandasai-2.1a1/pandasai/llm/google_palm.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 https://developers.generativeai.google/products/palm.
 
 Example:
     Use below example to call GooglePalm Model
 
     >>> from pandasai.llm.google_palm import GooglePalm
 """
-from typing import Any
+from typing import Any, Optional
 
 from pandasai.helpers.memory import Memory
 
 from ..exceptions import APIKeyNotFoundError
 from ..helpers.optional import import_dependency
 from .base import BaseGoogle
 
@@ -68,15 +68,15 @@
         """
 
         super()._validate()
 
         if not self.model:
             raise ValueError("model is required.")
 
-    def _generate_text(self, prompt: str, memory: Memory = None) -> str:
+    def _generate_text(self, prompt: str, memory: Optional[Memory] = None) -> str:
         """
         Generates text for prompt.
 
         Args:
             prompt (str): A string representation of the prompt.
 
         Returns:
```

### Comparing `pandasai-2.0a9/pandasai/llm/google_vertexai.py` & `pandasai-2.1a1/pandasai/llm/google_vertexai.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         """
 
         super()._validate()
 
         if not self.model:
             raise ValueError("model is required.")
 
-    def _generate_text(self, prompt: str, memory: Memory = None) -> str:
+    def _generate_text(self, prompt: str, memory: Optional[Memory] = None) -> str:
         """
         Generates text for prompt.
 
         Args:
             prompt (str): A string representation of the prompt.
 
         Returns:
```

### Comparing `pandasai-2.0a9/pandasai/llm/huggingface_text_gen.py` & `pandasai-2.1a1/pandasai/llm/huggingface_text_gen.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/llm/langchain.py` & `pandasai-2.1a1/pandasai/llm/langchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 from __future__ import annotations
 
+try:
+    from langchain_core.language_models import BaseLanguageModel
+    from langchain_core.language_models.chat_models import BaseChatModel
+
+except ImportError:
+    from unittest.mock import Mock
+
+    # Fallback definitions if langchain_core is not installed
+    BaseLanguageModel = BaseChatModel = Mock
+
 from typing import TYPE_CHECKING
 
 from pandasai.prompts.base import BasePrompt
 
 from .base import LLM
 
 if TYPE_CHECKING:
@@ -15,32 +25,36 @@
 
 Example:
     Use below example to call LLM
     >>> from pandasai.llm.langchain import LangchainLLm
 """
 
 
+def is_langchain_llm(llm) -> bool:
+    return isinstance(llm, BaseLanguageModel)
+
+
 class LangchainLLM(LLM):
     """
     Class to wrap Langchain LLMs and make PandasAI interoperable
     with LangChain.
     """
 
-    langchain_llm = None
+    langchain_llm: BaseLanguageModel
 
-    def __init__(self, langchain_llm):
+    def __init__(self, langchain_llm: BaseLanguageModel):
         self.langchain_llm = langchain_llm
 
-    def call(self, instruction: BasePrompt, context: PipelineContext = None) -> str:
-        prompt = instruction.to_string()
+    def call(
+        self, instruction: BasePrompt, context: PipelineContext = None, suffix: str = ""
+    ) -> str:
+        prompt = instruction.to_string() + suffix
         memory = context.memory if context else None
         prompt = self.prepend_system_prompt(prompt, memory)
         self.last_prompt = prompt
-        return self.langchain_llm.predict(prompt)
 
-    @staticmethod
-    def is_langchain_llm(llm: LLM) -> bool:
-        return hasattr(llm, "_llm_type")
+        res = self.langchain_llm.invoke(prompt)
+        return res.content if isinstance(self.langchain_llm, BaseChatModel) else res
 
     @property
     def type(self) -> str:
         return f"langchain_{self.langchain_llm._llm_type}"
```

### Comparing `pandasai-2.0a9/pandasai/llm/openai.py` & `pandasai-2.1a1/pandasai/llm/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
         "gpt-4",
         "gpt-4-0125-preview",
         "gpt-4-1106-preview",
         "gpt-4-0613",
         "gpt-4-32k",
         "gpt-4-32k-0613",
         "gpt-4-turbo-preview",
+        "gpt-4o",
+        "gpt-4o-2024-05-13",
     ]
     _supported_completion_models = ["gpt-3.5-turbo-instruct"]
 
     model: str = "gpt-3.5-turbo"
 
     def __init__(
         self,
@@ -66,14 +68,17 @@
 
         """
         self.api_token = api_token or os.getenv("OPENAI_API_KEY") or None
 
         if not self.api_token:
             raise APIKeyNotFoundError("OpenAI API key is required")
 
+        self.api_base = (
+            kwargs.get("api_base") or os.getenv("OPENAI_API_BASE") or self.api_base
+        )
         self.openai_proxy = kwargs.get("openai_proxy") or os.getenv("OPENAI_PROXY")
         if self.openai_proxy:
             openai.proxy = {"http": self.openai_proxy, "https": self.openai_proxy}
 
         self._set_params(**kwargs)
         # set the client
         model_name = self.model.split(":")[1] if "ft:" in self.model else self.model
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/base_logic_unit.py` & `pandasai-2.1a1/pandasai/pipelines/base_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/cache_lookup.py` & `pandasai-2.1a1/pandasai/pipelines/chat/cache_lookup.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/cache_population.py` & `pandasai-2.1a1/pandasai/pipelines/chat/cache_population.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/chat_pipeline_input.py` & `pandasai-2.1a1/pandasai/pipelines/chat/chat_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/code_generator.py` & `pandasai-2.1a1/pandasai/pipelines/chat/code_generator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 from pandasai.helpers.logger import Logger
 from pandasai.helpers.query_exec_tracker import QueryExecTracker
+from pandasai.pipelines.chat.code_cleaning import CodeCleaning
 from pandasai.pipelines.chat.code_generator import CodeGenerator
 from pandasai.pipelines.chat.error_correction_pipeline.error_correction_pipeline_input import (
     ErrorCorrectionPipelineInput,
 )
 from pandasai.pipelines.chat.error_correction_pipeline.error_prompt_generation import (
     ErrorPromptGeneration,
 )
@@ -23,22 +24,24 @@
 
     def __init__(
         self,
         context: Optional[PipelineContext] = None,
         logger: Optional[Logger] = None,
         query_exec_tracker: QueryExecTracker = None,
         on_prompt_generation=None,
+        on_code_generation=None,
     ):
         self.pipeline = Pipeline(
             context=context,
             logger=logger,
             query_exec_tracker=query_exec_tracker,
             steps=[
                 ErrorPromptGeneration(on_prompt_generation=on_prompt_generation),
-                CodeGenerator(),
+                CodeGenerator(on_execution=on_code_generation),
+                CodeCleaning(),
             ],
         )
         self._context = context
         self._logger = logger
 
     def run(self, input: ErrorCorrectionPipelineInput):
         self._logger.log(f"Executing Pipeline: {self.__class__.__name__}")
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py` & `pandasai-2.1a1/pandasai/ee/agents/semantic_agent/pipeline/error_correction_pipeline/error_prompt_generation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 from typing import Any, Callable
 
 from pandasai.exceptions import ExecuteSQLQueryNotUsed, InvalidLLMOutputType
 from pandasai.helpers.logger import Logger
 from pandasai.pipelines.base_logic_unit import BaseLogicUnit
 from pandasai.pipelines.chat.error_correction_pipeline.error_correction_pipeline_input import (
     ErrorCorrectionPipelineInput,
@@ -70,25 +71,28 @@
 
         Args:
             values (dict): The values to use for the prompt
 
         Returns:
             BasePrompt: The prompt
         """
+        traceback_errors = traceback.format_exc()
         return (
             CorrectOutputTypeErrorPrompt(
                 context=self.context,
                 code=code,
-                error=e,
+                error=traceback_errors,
                 output_type=self.context.get("output_type"),
             )
             if isinstance(e, InvalidLLMOutputType)
-            else CorrectExecuteSQLQueryUsageErrorPrompt(
-                context=self.context, code=code, error=e
-            )
-            if isinstance(e, ExecuteSQLQueryNotUsed)
-            else CorrectErrorPrompt(
-                context=self.context,
-                code=code,
-                error=e,
+            else (
+                CorrectExecuteSQLQueryUsageErrorPrompt(
+                    context=self.context, code=code, error=traceback_errors
+                )
+                if isinstance(e, ExecuteSQLQueryNotUsed)
+                else CorrectErrorPrompt(
+                    context=self.context,
+                    code=code,
+                    error=traceback_errors,
+                )
             )
         )
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/generate_chat_pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/chat/generate_chat_pipeline.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from typing import Optional
 
 from pandasai.helpers.query_exec_tracker import QueryExecTracker
 from pandasai.pipelines.chat.chat_pipeline_input import (
     ChatPipelineInput,
 )
+from pandasai.pipelines.chat.code_execution_pipeline_input import (
+    CodeExecutionPipelineInput,
+)
 from pandasai.pipelines.chat.error_correction_pipeline.error_correction_pipeline import (
     ErrorCorrectionPipeline,
 )
 from pandasai.pipelines.chat.error_correction_pipeline.error_correction_pipeline_input import (
     ErrorCorrectionPipelineInput,
 )
 from pandasai.pipelines.chat.validate_pipeline_input import (
@@ -15,41 +18,43 @@
 )
 
 from ...helpers.logger import Logger
 from ..pipeline import Pipeline
 from ..pipeline_context import PipelineContext
 from .cache_lookup import CacheLookup
 from .cache_population import CachePopulation
+from .code_cleaning import CodeCleaning
 from .code_execution import CodeExecution
 from .code_generator import CodeGenerator
 from .prompt_generation import PromptGeneration
 from .result_parsing import ResultParsing
 from .result_validation import ResultValidation
 
 
 class GenerateChatPipeline:
-    pipeline: Pipeline
+    code_generation_pipeline = Pipeline
+    code_execution_pipeline = Pipeline
     context: PipelineContext
     _logger: Logger
     last_error: str
 
     def __init__(
         self,
         context: Optional[PipelineContext] = None,
         logger: Optional[Logger] = None,
         on_prompt_generation=None,
         on_code_generation=None,
-        on_code_execution=None,
+        before_code_execution=None,
         on_result=None,
     ):
         self.query_exec_tracker = QueryExecTracker(
             server_config=context.config.log_server
         )
 
-        self.pipeline = Pipeline(
+        self.code_generation_pipeline = Pipeline(
             context=context,
             logger=logger,
             query_exec_tracker=self.query_exec_tracker,
             steps=[
                 ValidatePipelineInput(),
                 CacheLookup(),
                 PromptGeneration(
@@ -57,30 +62,44 @@
                     on_execution=on_prompt_generation,
                 ),
                 CodeGenerator(
                     skip_if=self.is_cached,
                     on_execution=on_code_generation,
                 ),
                 CachePopulation(skip_if=self.is_cached),
+                CodeCleaning(
+                    skip_if=self.no_code,
+                    on_failure=self.on_code_cleaning_failure,
+                    on_retry=self.on_code_retry,
+                ),
+            ],
+        )
+
+        self.code_execution_pipeline = Pipeline(
+            context=context,
+            logger=logger,
+            query_exec_tracker=self.query_exec_tracker,
+            steps=[
                 CodeExecution(
-                    before_execution=on_code_execution,
+                    before_execution=before_code_execution,
                     on_failure=self.on_code_execution_failure,
                     on_retry=self.on_code_retry,
                 ),
                 ResultValidation(),
                 ResultParsing(
                     before_execution=on_result,
                 ),
             ],
         )
 
         self.code_exec_error_pipeline = ErrorCorrectionPipeline(
             context=context,
             logger=logger,
             query_exec_tracker=self.query_exec_tracker,
+            on_code_generation=on_code_generation,
             on_prompt_generation=on_prompt_generation,
         )
 
         self.context = context
         self._logger = logger
         self.last_error = None
 
@@ -105,24 +124,157 @@
                     "content_type": "code",
                     "value": code,
                     "exception": errors,
                 },
             }
         )
 
+    def on_code_cleaning_failure(self, code, errors):
+        # Add information about the code failure in the query tracker for debug
+        self.query_exec_tracker.add_step(
+            {
+                "type": "CodeCleaning",
+                "success": False,
+                "message": "Failed to clean code",
+                "execution_time": None,
+                "data": {
+                    "content_type": "code",
+                    "value": code,
+                    "exception": errors,
+                },
+            }
+        )
+
     def on_code_retry(self, code: str, exception: Exception):
         correction_input = ErrorCorrectionPipelineInput(code, exception)
         return self.code_exec_error_pipeline.run(correction_input)
 
+    def no_code(self, context: PipelineContext):
+        return context.get("last_code_generated") is None
+
     def is_cached(self, context: PipelineContext):
         return context.get("found_in_cache")
 
     def get_last_track_log_id(self):
         return self.query_exec_tracker.last_log_id
 
+    def run_generate_code(self, input: ChatPipelineInput) -> dict:
+        """
+        Executes the code generation pipeline with user input and return the result
+        Args:
+            input (ChatPipelineInput): _description_
+
+        Returns:
+            The `output` dictionary is expected to have the following keys:
+            - 'type': The type of the output.
+            - 'value': The value of the output.
+        """
+        self._logger.log(f"Executing Pipeline: {self.__class__.__name__}")
+
+        # Reset intermediate values
+        self.context.reset_intermediate_values()
+
+        # Start New Tracking for Query
+        self.query_exec_tracker.start_new_track(input)
+
+        self.query_exec_tracker.add_skills(self.context)
+
+        self.query_exec_tracker.add_dataframes(self.context.dfs)
+
+        # Add Query to memory
+        self.context.memory.add(input.query, True)
+
+        self.context.add_many(
+            {
+                "output_type": input.output_type,
+                "last_prompt_id": input.prompt_id,
+            }
+        )
+        try:
+            output = self.code_generation_pipeline.run(input)
+
+            self.query_exec_tracker.success = True
+
+            self.query_exec_tracker.publish()
+
+            return output
+
+        except Exception as e:
+            # Show the full traceback
+            import traceback
+
+            traceback.print_exc()
+
+            self.last_error = str(e)
+            self.query_exec_tracker.success = False
+            self.query_exec_tracker.publish()
+
+            return (
+                "Unfortunately, I was not able to answer your question, "
+                "because of the following error:\n"
+                f"\n{e}\n"
+            )
+
+    def run_execute_code(self, input: CodeExecutionPipelineInput) -> dict:
+        """
+        Executes the chat pipeline with user input and return the result
+        Args:
+            input (CodeExecutionPipelineInput): _description_
+
+        Returns:
+            The `output` dictionary is expected to have the following keys:
+            - 'type': The type of the output.
+            - 'value': The value of the output.
+        """
+        self._logger.log(f"Executing Pipeline: {self.__class__.__name__}")
+
+        # Reset intermediate values
+        self.context.reset_intermediate_values()
+
+        # Start New Tracking for Query
+        self.query_exec_tracker.start_new_track(input)
+
+        self.query_exec_tracker.add_skills(self.context)
+
+        self.query_exec_tracker.add_dataframes(self.context.dfs)
+
+        # Add Query to memory
+        self.context.memory.add(input.code, True)
+
+        self.context.add_many(
+            {
+                "output_type": input.output_type,
+                "last_prompt_id": input.prompt_id,
+            }
+        )
+        try:
+            output = self.code_execution_pipeline.run(input.code)
+
+            self.query_exec_tracker.success = True
+
+            self.query_exec_tracker.publish()
+
+            return output
+
+        except Exception as e:
+            # Show the full traceback
+            import traceback
+
+            traceback.print_exc()
+
+            self.last_error = str(e)
+            self.query_exec_tracker.success = False
+            self.query_exec_tracker.publish()
+
+            return (
+                "Unfortunately, I was not able to answer your question, "
+                "because of the following error:\n"
+                f"\n{e}\n"
+            )
+
     def run(self, input: ChatPipelineInput) -> dict:
         """
         Executes the chat pipeline with user input and return the result
         Args:
             input (ChatPipelineInput): _description_
 
         Returns:
@@ -148,15 +300,20 @@
         self.context.add_many(
             {
                 "output_type": input.output_type,
                 "last_prompt_id": input.prompt_id,
             }
         )
         try:
-            output = self.pipeline.run(input)
+            if self.code_execution_pipeline:
+                output = (
+                    self.code_generation_pipeline | self.code_execution_pipeline
+                ).run(input)
+            else:
+                output = self.code_generation_pipeline.run(input)
 
             self.query_exec_tracker.success = True
 
             self.query_exec_tracker.publish()
 
             return output
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/prompt_generation.py` & `pandasai-2.1a1/pandasai/pipelines/chat/prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/result_parsing.py` & `pandasai-2.1a1/pandasai/pipelines/chat/result_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,12 @@
             result (dict): The result to add to the memory
             context (PipelineContext) : Pipeline Context
         """
         if result is None:
             return
 
         if result["type"] in ["string", "number"]:
-            context.memory.add(result["value"], False)
+            context.memory.add(str(result["value"]), False)
         elif result["type"] == "dataframe":
             context.memory.add("Check it out: <dataframe>", False)
         elif result["type"] == "plot":
             context.memory.add("Check it out: <plot>", False)
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/result_validation.py` & `pandasai-2.1a1/pandasai/pipelines/chat/result_validation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/chat/validate_pipeline_input.py` & `pandasai-2.1a1/pandasai/pipelines/chat/validate_pipeline_input.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, List
 
+from pandasai.connectors.pandas import PandasConnector
 from pandasai.connectors.sql import SQLConnector
 from pandasai.exceptions import InvalidConfigError
 from pandasai.pipelines.logic_unit_output import LogicUnitOutput
 
 from ...connectors import BaseConnector
 from ..base_logic_unit import BaseLogicUnit
 from ..pipeline_context import PipelineContext
@@ -23,19 +24,21 @@
             dfs (List[BaseConnector]): list of BaseConnectors
 
         Raises:
             InvalidConfigError: Raise Error in case of config is set but criteria is not met
         """
 
         if self.context.config.direct_sql:
-            if all((isinstance(df, SQLConnector) and df.equals(dfs[0])) for df in dfs):
+            if all(
+                (isinstance(df, SQLConnector) and df.equals(dfs[0])) for df in dfs
+            ) or all((isinstance(df, PandasConnector) and df.sql_enabed) for df in dfs):
                 return True
             else:
                 raise InvalidConfigError(
-                    "Direct requires all SQLConnector and they belong to same datasource "
+                    "Direct requires all Connector and they belong to same datasource "
                     "and have same credentials"
                 )
         return False
 
     def execute(self, input: Any, **kwargs) -> Any:
         """
         This method validates pipeline context and configs
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/logic_unit_output.py` & `pandasai-2.1a1/pandasai/pipelines/logic_unit_output.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/logic_units/output_logic_unit.py` & `pandasai-2.1a1/pandasai/pipelines/logic_units/output_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/pipelines/pipeline.py` & `pandasai-2.1a1/pandasai/pipelines/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import time
 from typing import Any, List, Optional, Union
 
 from pandasai.config import load_config_from_json
-from pandasai.exceptions import UnSupportedLogicUnit
+from pandasai.exceptions import PipelineConcatenationError, UnSupportedLogicUnit
 from pandasai.helpers.logger import Logger
 from pandasai.helpers.query_exec_tracker import QueryExecTracker
 from pandasai.pipelines.base_logic_unit import BaseLogicUnit
 from pandasai.pipelines.logic_unit_output import LogicUnitOutput
 from pandasai.pipelines.pipeline_context import PipelineContext
 
 from ..connectors import BaseConnector
@@ -133,7 +133,37 @@
                     logic.on_execution(data)
 
         except Exception as e:
             self._logger.log(f"Pipeline failed on step {index}: {e}", logging.ERROR)
             raise e
 
         return data
+
+    def __or__(self, pipeline: "Pipeline") -> Any:
+        """
+        This functions is responsible to pipe two pipelines
+        Args:
+            pipeline (Pipeline): Second Pipeline which will be Piped to the self.
+            data (Any, optional): Input Data to run the pipeline. Defaults to None.
+
+        Returns:
+            Any: Depends on the type can return anything
+        """
+
+        if not isinstance(pipeline, Pipeline):
+            raise PipelineConcatenationError(
+                "Pipeline can be concatenated with Pipeline class only!"
+            )
+
+        combined_pipeline = Pipeline(
+            context=self._context,
+            logger=self._logger,
+            query_exec_tracker=self._query_exec_tracker,
+        )
+
+        for step in self._steps:
+            combined_pipeline.add_step(step)
+
+        for step in pipeline._steps:
+            combined_pipeline.add_step(step)
+
+        return combined_pipeline
```

### Comparing `pandasai-2.0a9/pandasai/pipelines/pipeline_context.py` & `pandasai-2.1a1/pandasai/pipelines/pipeline_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,17 +41,19 @@
         self.intermediate_values = initial_values or {}
 
         self.vectorstore = vectorstore
 
         self._initial_values = initial_values
 
     def reset_intermediate_values(self):
+        print(self._initial_values)
         self.intermediate_values = self._initial_values or {}
+        print(self.intermediate_values)
 
     def add(self, key: str, value: Any):
         self.intermediate_values[key] = value
 
     def add_many(self, values: dict):
         self.intermediate_values.update(values)
 
-    def get(self, key: str):
-        return self.intermediate_values.get(key, "")
+    def get(self, key: str, default: Any = ""):
+        return self.intermediate_values.get(key, default)
```

### Comparing `pandasai-2.0a9/pandasai/prompts/base.py` & `pandasai-2.1a1/pandasai/prompts/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ Base class to implement a new Prompt
 In order to better handle the instructions, this prompt module is written.
 """
+
 import os
 import re
 from pathlib import Path
 from typing import Optional
 
 from jinja2 import Environment, FileSystemLoader
 
@@ -56,8 +57,19 @@
     def validate(self, output: str) -> bool:
         return isinstance(output, str)
 
     def to_json(self):
         """
         Return Json Prompt
         """
-        raise NotImplementedError("Implementation required")
+        if "context" not in self.props:
+            return {"prompt": self.to_string()}
+
+        context = self.props["context"]
+        memory = context.memory
+        conversations = memory.to_json()
+        system_prompt = memory.get_system_prompt()
+        return {
+            "conversation": conversations,
+            "system_prompt": system_prompt,
+            "prompt": self.to_string(),
+        }
```

### Comparing `pandasai-2.0a9/pandasai/prompts/clarification_questions_prompt.py` & `pandasai-2.1a1/pandasai/prompts/clarification_questions_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/correct_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/correct_output_type_error_prompt.py` & `pandasai-2.1a1/pandasai/prompts/correct_output_type_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/direct_sql_prompt.py` & `pandasai-2.1a1/pandasai/prompts/direct_sql_prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Prompt to explain code generation by the LLM"""
+import pandasai.pandas as pd
 from pandasai.helpers.dataframe_serializer import (
     DataframeSerializer,
     DataframeSerializerType,
 )
 
 from .generate_python_code import (
     CurrentCodePrompt,
@@ -44,11 +45,11 @@
             "code_description",
             kwargs.pop("code_description", "Update this initial code:"),
         )
         self.set_var("last_message", kwargs.pop("last_message", ""))
         self.set_var("prev_conversation", kwargs.pop("prev_conversation", ""))
 
     def on_prompt_generation(self) -> None:
-        default_import = "import pandas as pd"
+        default_import = f"import {pd.__name__} as pd"
 
         self.set_var("default_import", default_import)
         self.set_var("reasoning", SimpleReasoningPrompt())
```

### Comparing `pandasai-2.0a9/pandasai/prompts/file_based_prompt.py` & `pandasai-2.1a1/pandasai/prompts/file_based_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/generate_python_code.py` & `pandasai-2.1a1/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/templates/clarification_questions_prompt.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/clarification_questions_prompt.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/templates/generate_python_code.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/generate_python_code.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/templates/generate_python_code_with_sql.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/generate_python_code_with_sql.tmpl`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,82 @@
 00000000: 3c74 6162 6c65 733e 0a7b 2520 666f 7220  <tables>.{% for 
 00000010: 6466 2069 6e20 636f 6e74 6578 742e 6466  df in context.df
-00000020: 7320 257d 3c74 6162 6c65 3e0a 7b25 2073  s %}<table>.{% s
-00000030: 6574 2069 6e64 6578 203d 206c 6f6f 702e  et index = loop.
-00000040: 696e 6465 7820 257d 7b25 2069 6e63 6c75  index %}{% inclu
-00000050: 6465 2027 7368 6172 6564 2f64 6174 6166  de 'shared/dataf
-00000060: 7261 6d65 2e74 6d70 6c27 2077 6974 6820  rame.tmpl' with 
-00000070: 636f 6e74 6578 7420 257d 0a3c 2f74 6162  context %}.</tab
-00000080: 6c65 3e7b 2520 656e 6466 6f72 2025 7d0a  le>{% endfor %}.
-00000090: 3c2f 7461 626c 6573 3e0a 0a7b 2520 6966  </tables>..{% if
-000000a0: 2063 6f6e 7465 7874 2e73 6b69 6c6c 735f   context.skills_
-000000b0: 6d61 6e61 6765 722e 6861 735f 736b 696c  manager.has_skil
-000000c0: 6c73 2829 2025 7d0a 7b7b 636f 6e74 6578  ls() %}.{{contex
-000000d0: 742e 736b 696c 6c73 5f6d 616e 6167 6572  t.skills_manager
-000000e0: 2e70 726f 6d70 745f 6469 7370 6c61 7928  .prompt_display(
-000000f0: 297d 7d0a 7b25 2065 6c73 6520 257d 0a59  )}}.{% else %}.Y
-00000100: 6f75 2063 616e 2063 616c 6c20 7468 6520  ou can call the 
-00000110: 666f 6c6c 6f77 696e 6720 6675 6e63 7469  following functi
-00000120: 6f6e 7320 7468 6174 2068 6176 6520 6265  ons that have be
-00000130: 656e 2070 7265 2d64 6566 696e 6564 2066  en pre-defined f
-00000140: 6f72 2079 6f75 3a0a 7b25 2065 6e64 6966  or you:.{% endif
-00000150: 2025 7d0a 3c66 756e 6374 696f 6e3e 0a64   %}.<function>.d
-00000160: 6566 2065 7865 6375 7465 5f73 716c 5f71  ef execute_sql_q
-00000170: 7565 7279 2873 716c 5f71 7565 7279 3a20  uery(sql_query: 
-00000180: 7374 7229 202d 3e20 7064 2e44 6174 6166  str) -> pd.Dataf
-00000190: 7261 6d65 0a20 2020 2022 2222 5468 6973  rame.    """This
-000001a0: 206d 6574 686f 6420 636f 6e6e 6563 7473   method connects
-000001b0: 2074 6f20 7468 6520 6461 7461 6261 7365   to the database
-000001c0: 2c20 6578 6563 7574 6573 2074 6865 2073  , executes the s
-000001d0: 716c 2071 7565 7279 2061 6e64 2072 6574  ql query and ret
-000001e0: 7572 6e73 2074 6865 2064 6174 6166 7261  urns the datafra
-000001f0: 6d65 2222 220a 3c2f 6675 6e63 7469 6f6e  me""".</function
-00000200: 3e0a 0a7b 2520 6966 206c 6173 745f 636f  >..{% if last_co
-00000210: 6465 5f67 656e 6572 6174 6564 2021 3d20  de_generated != 
-00000220: 2222 2061 6e64 2063 6f6e 7465 7874 2e6d  "" and context.m
-00000230: 656d 6f72 792e 636f 756e 7428 2920 3e20  emory.count() > 
-00000240: 3020 257d 0a7b 7b20 6c61 7374 5f63 6f64  0 %}.{{ last_cod
-00000250: 655f 6765 6e65 7261 7465 6420 7d7d 0a7b  e_generated }}.{
-00000260: 2520 656c 7365 2025 7d0a 5570 6461 7465  % else %}.Update
-00000270: 2074 6869 7320 696e 6974 6961 6c20 636f   this initial co
-00000280: 6465 3a0a 6060 6070 7974 686f 6e0a 2320  de:.```python.# 
-00000290: 544f 444f 3a20 696d 706f 7274 2074 6865  TODO: import the
-000002a0: 2072 6571 7569 7265 6420 6465 7065 6e64   required depend
-000002b0: 656e 6369 6573 0a69 6d70 6f72 7420 7061  encies.import pa
-000002c0: 6e64 6173 2061 7320 7064 0a0a 2320 5772  ndas as pd..# Wr
-000002d0: 6974 6520 636f 6465 2068 6572 650a 0a23  ite code here..#
-000002e0: 2044 6563 6c61 7265 2072 6573 756c 7420   Declare result 
-000002f0: 7661 723a 207b 2520 696e 636c 7564 6520  var: {% include 
-00000300: 2773 6861 7265 642f 6f75 7470 7574 5f74  'shared/output_t
-00000310: 7970 655f 7465 6d70 6c61 7465 2e74 6d70  ype_template.tmp
-00000320: 6c27 2077 6974 6820 636f 6e74 6578 7420  l' with context 
-00000330: 257d 0a60 6060 0a7b 2520 656e 6469 6620  %}.```.{% endif 
-00000340: 257d 0a7b 2520 696e 636c 7564 6520 2773  %}.{% include 's
-00000350: 6861 7265 642f 7665 6374 6f72 6462 5f64  hared/vectordb_d
-00000360: 6f63 732e 746d 706c 2720 7769 7468 2063  ocs.tmpl' with c
-00000370: 6f6e 7465 7874 2025 7d0a 7b7b 2063 6f6e  ontext %}.{{ con
-00000380: 7465 7874 2e6d 656d 6f72 792e 6765 745f  text.memory.get_
-00000390: 6c61 7374 5f6d 6573 7361 6765 2829 207d  last_message() }
-000003a0: 7d0a 5661 7269 6162 6c65 2060 6466 733a  }.Variable `dfs:
-000003b0: 206c 6973 745b 7064 2e44 6174 6146 7261   list[pd.DataFra
-000003c0: 6d65 5d60 2069 7320 616c 7265 6164 7920  me]` is already 
-000003d0: 6465 636c 6172 6564 2e0a 0a41 7420 7468  declared...At th
-000003e0: 6520 656e 642c 2064 6563 6c61 7265 2022  e end, declare "
-000003f0: 7265 7375 6c74 2220 7661 7269 6162 6c65  result" variable
-00000400: 2061 7320 6120 6469 6374 696f 6e61 7279   as a dictionary
-00000410: 206f 6620 7479 7065 2061 6e64 2076 616c   of type and val
-00000420: 7565 2e0a 7b25 2069 6620 7669 7a5f 6c69  ue..{% if viz_li
-00000430: 6220 257d 0a49 6620 796f 7520 6172 6520  b %}.If you are 
-00000440: 6173 6b65 6420 746f 2070 6c6f 7420 6120  asked to plot a 
-00000450: 6368 6172 742c 2075 7365 2022 7b7b 7669  chart, use "{{vi
-00000460: 7a5f 6c69 627d 7d22 2066 6f72 2063 6861  z_lib}}" for cha
-00000470: 7274 732c 2073 6176 6520 6173 2070 6e67  rts, save as png
-00000480: 2e0a 7b25 2065 6e64 6966 2025 7d0a 0a47  ..{% endif %}..G
-00000490: 656e 6572 6174 6520 7079 7468 6f6e 2063  enerate python c
-000004a0: 6f64 6520 616e 6420 7265 7475 726e 2066  ode and return f
-000004b0: 756c 6c20 7570 6461 7465 6420 636f 6465  ull updated code
-000004c0: 3a0a 0a23 2323 204e 6f74 653a 2055 7365  :..### Note: Use
-000004d0: 206f 6e6c 7920 7265 6c65 7661 6e74 2074   only relevant t
-000004e0: 6162 6c65 2066 6f72 2071 7565 7279 2061  able for query a
-000004f0: 6e64 2064 6f20 6167 6772 6567 6174 696f  nd do aggregatio
-00000500: 6e2c 2073 6f72 7469 6e67 2c20 6a6f 696e  n, sorting, join
-00000510: 7320 616e 6420 6772 6f75 6279 2074 6872  s and grouby thr
-00000520: 6f75 6768 2073 716c 2071 7565 7279       ough sql query
+00000020: 7320 257d 0a7b 2520 7365 7420 696e 6465  s %}.{% set inde
+00000030: 7820 3d20 6c6f 6f70 2e69 6e64 6578 2025  x = loop.index %
+00000040: 7d7b 2520 696e 636c 7564 6520 2773 6861  }{% include 'sha
+00000050: 7265 642f 6461 7461 6672 616d 652e 746d  red/dataframe.tm
+00000060: 706c 2720 7769 7468 2063 6f6e 7465 7874  pl' with context
+00000070: 2025 7d0a 7b25 2065 6e64 666f 7220 257d   %}.{% endfor %}
+00000080: 0a3c 2f74 6162 6c65 733e 0a0a 7b25 2069  .</tables>..{% i
+00000090: 6620 636f 6e74 6578 742e 736b 696c 6c73  f context.skills
+000000a0: 5f6d 616e 6167 6572 2e68 6173 5f73 6b69  _manager.has_ski
+000000b0: 6c6c 7328 2920 257d 0a7b 7b63 6f6e 7465  lls() %}.{{conte
+000000c0: 7874 2e73 6b69 6c6c 735f 6d61 6e61 6765  xt.skills_manage
+000000d0: 722e 7072 6f6d 7074 5f64 6973 706c 6179  r.prompt_display
+000000e0: 2829 7d7d 0a7b 2520 656c 7365 2025 7d0a  ()}}.{% else %}.
+000000f0: 596f 7520 6172 6520 616c 7265 6164 7920  You are already 
+00000100: 7072 6f76 6964 6564 2077 6974 6820 7468  provided with th
+00000110: 6520 666f 6c6c 6f77 696e 6720 6675 6e63  e following func
+00000120: 7469 6f6e 7320 7468 6174 2079 6f75 2063  tions that you c
+00000130: 616e 2063 616c 6c3a 0a7b 2520 656e 6469  an call:.{% endi
+00000140: 6620 257d 0a3c 6675 6e63 7469 6f6e 3e0a  f %}.<function>.
+00000150: 6465 6620 6578 6563 7574 655f 7371 6c5f  def execute_sql_
+00000160: 7175 6572 7928 7371 6c5f 7175 6572 793a  query(sql_query:
+00000170: 2073 7472 2920 2d3e 2070 642e 4461 7461   str) -> pd.Data
+00000180: 6672 616d 650a 2020 2020 2222 2254 6869  frame.    """Thi
+00000190: 7320 6d65 7468 6f64 2063 6f6e 6e65 6374  s method connect
+000001a0: 7320 746f 2074 6865 2064 6174 6162 6173  s to the databas
+000001b0: 652c 2065 7865 6375 7465 7320 7468 6520  e, executes the 
+000001c0: 7371 6c20 7175 6572 7920 616e 6420 7265  sql query and re
+000001d0: 7475 726e 7320 7468 6520 6461 7461 6672  turns the datafr
+000001e0: 616d 6522 2222 0a3c 2f66 756e 6374 696f  ame""".</functio
+000001f0: 6e3e 0a0a 7b25 2069 6620 6c61 7374 5f63  n>..{% if last_c
+00000200: 6f64 655f 6765 6e65 7261 7465 6420 213d  ode_generated !=
+00000210: 2022 2220 616e 6420 636f 6e74 6578 742e   "" and context.
+00000220: 6d65 6d6f 7279 2e63 6f75 6e74 2829 203e  memory.count() >
+00000230: 2030 2025 7d0a 7b7b 206c 6173 745f 636f   0 %}.{{ last_co
+00000240: 6465 5f67 656e 6572 6174 6564 207d 7d0a  de_generated }}.
+00000250: 7b25 2065 6c73 6520 257d 0a55 7064 6174  {% else %}.Updat
+00000260: 6520 7468 6973 2069 6e69 7469 616c 2063  e this initial c
+00000270: 6f64 653a 0a60 6060 7079 7468 6f6e 0a23  ode:.```python.#
+00000280: 2054 4f44 4f3a 2069 6d70 6f72 7420 7468   TODO: import th
+00000290: 6520 7265 7175 6972 6564 2064 6570 656e  e required depen
+000002a0: 6465 6e63 6965 730a 696d 706f 7274 2070  dencies.import p
+000002b0: 616e 6461 7320 6173 2070 640a 0a23 2057  andas as pd..# W
+000002c0: 7269 7465 2063 6f64 6520 6865 7265 0a0a  rite code here..
+000002d0: 2320 4465 636c 6172 6520 7265 7375 6c74  # Declare result
+000002e0: 2076 6172 3a20 7b25 2069 6e63 6c75 6465   var: {% include
+000002f0: 2027 7368 6172 6564 2f6f 7574 7075 745f   'shared/output_
+00000300: 7479 7065 5f74 656d 706c 6174 652e 746d  type_template.tm
+00000310: 706c 2720 7769 7468 2063 6f6e 7465 7874  pl' with context
+00000320: 2025 7d0a 6060 600a 7b25 2065 6e64 6966   %}.```.{% endif
+00000330: 2025 7d0a 7b25 2069 6e63 6c75 6465 2027   %}.{% include '
+00000340: 7368 6172 6564 2f76 6563 746f 7264 625f  shared/vectordb_
+00000350: 646f 6373 2e74 6d70 6c27 2077 6974 6820  docs.tmpl' with 
+00000360: 636f 6e74 6578 7420 257d 0a7b 7b20 636f  context %}.{{ co
+00000370: 6e74 6578 742e 6d65 6d6f 7279 2e67 6574  ntext.memory.get
+00000380: 5f6c 6173 745f 6d65 7373 6167 6528 2920  _last_message() 
+00000390: 7d7d 0a56 6172 6961 626c 6520 6064 6673  }}.Variable `dfs
+000003a0: 3a20 6c69 7374 5b70 642e 4461 7461 4672  : list[pd.DataFr
+000003b0: 616d 655d 6020 6973 2061 6c72 6561 6479  ame]` is already
+000003c0: 2064 6563 6c61 7265 642e 0a0a 4174 2074   declared...At t
+000003d0: 6865 2065 6e64 2c20 6465 636c 6172 6520  he end, declare 
+000003e0: 2272 6573 756c 7422 2076 6172 6961 626c  "result" variabl
+000003f0: 6520 6173 2061 2064 6963 7469 6f6e 6172  e as a dictionar
+00000400: 7920 6f66 2074 7970 6520 616e 6420 7661  y of type and va
+00000410: 6c75 652e 0a7b 2520 6966 2076 697a 5f6c  lue..{% if viz_l
+00000420: 6962 2025 7d0a 4966 2079 6f75 2061 7265  ib %}.If you are
+00000430: 2061 736b 6564 2074 6f20 706c 6f74 2061   asked to plot a
+00000440: 2063 6861 7274 2c20 7573 6520 227b 7b76   chart, use "{{v
+00000450: 697a 5f6c 6962 7d7d 2220 666f 7220 6368  iz_lib}}" for ch
+00000460: 6172 7473 2c20 7361 7665 2061 7320 706e  arts, save as pn
+00000470: 672e 0a7b 2520 656e 6469 6620 257d 0a0a  g..{% endif %}..
+00000480: 4765 6e65 7261 7465 2070 7974 686f 6e20  Generate python 
+00000490: 636f 6465 2061 6e64 2072 6574 7572 6e20  code and return 
+000004a0: 6675 6c6c 2075 7064 6174 6564 2063 6f64  full updated cod
+000004b0: 653a 0a0a 2323 2320 4e6f 7465 3a20 5573  e:..### Note: Us
+000004c0: 6520 6f6e 6c79 2072 656c 6576 616e 7420  e only relevant 
+000004d0: 7461 626c 6520 666f 7220 7175 6572 7920  table for query 
+000004e0: 616e 6420 646f 2061 6767 7265 6761 7469  and do aggregati
+000004f0: 6f6e 2c20 736f 7274 696e 672c 206a 6f69  on, sorting, joi
+00000500: 6e73 2061 6e64 2067 726f 7562 7920 7468  ns and grouby th
+00000510: 726f 7567 6820 7371 6c20 7175 6572 79    rough sql query
```

### Comparing `pandasai-2.0a9/pandasai/prompts/templates/shared/output_type_template.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/shared/output_type_template.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/prompts/templates/shared/vectordb_docs.tmpl` & `pandasai-2.1a1/pandasai/prompts/templates/shared/vectordb_docs.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/responses/context.py` & `pandasai-2.1a1/pandasai/responses/context.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/responses/response_parser.py` & `pandasai-2.1a1/pandasai/responses/response_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,12 +61,16 @@
         If `open_charts` option set to `False`, the chart won't be displayed.
 
         Args:
             result (dict): result contains type and value
         Returns:
             Any: Returns depending on the user input
         """
-        if self._context._config.open_charts:
+        if (
+            self._context._config.open_charts
+            and isinstance(result["value"], str)
+            and "data:image/png;base64" not in result["value"]
+        ):
             with Image.open(result["value"]) as img:
                 img.show()
 
         return result["value"]
```

### Comparing `pandasai-2.0a9/pandasai/responses/response_serializer.py` & `pandasai-2.1a1/pandasai/responses/response_serializer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import base64
 import json
 
-import pandas as pd
-
+import pandasai.pandas as pd
 from pandasai.responses.response_type import ResponseType
 
 
 class ResponseSerializer:
     @staticmethod
     def serialize_dataframe(df: pd.DataFrame):
         json_data = json.loads(df.to_json(orient="split", date_format="iso"))
@@ -19,18 +18,24 @@
         Args:
             result (ResponseType): response returned after execution
 
         Returns:
             ResponseType: formatted response output
         """
         if result["type"] == "dataframe":
+            if isinstance(result["value"], pd.Series):
+                result["value"] = result["value"].to_frame()
             df_dict = ResponseSerializer.serialize_dataframe(result["value"])
             return {"type": result["type"], "value": df_dict}
 
-        elif result["type"] == "plot":
+        elif result["type"] == "plot" and isinstance(result["value"], str):
+            # check if already in base64 str return
+            if "data:image/png;base64" in result["value"]:
+                return result
+
             with open(result["value"], "rb") as image_file:
                 image_data = image_file.read()
             # Encode the image data to Base64
             base64_image = (
                 f"data:image/png;base64,{base64.b64encode(image_data).decode()}"
             )
             return {
```

### Comparing `pandasai-2.0a9/pandasai/responses/streamlit_response.py` & `pandasai-2.1a1/pandasai/responses/streamlit_response.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pandasai/schemas/df_config.py` & `pandasai-2.1a1/pandasai/schemas/df_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from typing import Any, List, Optional, TypedDict
 
-from pydantic import BaseModel, Field, validator
-
 from pandasai.constants import DEFAULT_CHART_DIRECTORY
 from pandasai.helpers.dataframe_serializer import DataframeSerializerType
+from pandasai.pydantic import BaseModel, Field, validator
 
-from ..exceptions import LLMNotFoundError
-from ..llm import LLM, LangchainLLM
+from ..llm import LLM, BambooLLM, LangchainLLM
 
 
 class LogServerConfig(TypedDict):
     server_url: str
     api_key: str
 
 
@@ -23,21 +21,21 @@
     open_charts: bool = True
     save_charts: bool = False
     save_charts_path: str = DEFAULT_CHART_DIRECTORY
     custom_whitelisted_dependencies: List[str] = Field(default_factory=list)
     max_retries: int = 3
     lazy_load_connector: bool = True
     response_parser: Any = None
-    llm: Any = None
+    llm: LLM = None
     data_viz_library: Optional[str] = ""
     log_server: LogServerConfig = None
     direct_sql: bool = False
-    dataframe_serializer: DataframeSerializerType = DataframeSerializerType.YML
+    dataframe_serializer: DataframeSerializerType = DataframeSerializerType.CSV
 
     class Config:
         arbitrary_types_allowed = True
 
-    @validator("llm")
-    def validate_llm(cls, llm):
-        if llm is None or not isinstance(llm, LLM or LangchainLLM):
-            raise LLMNotFoundError("LLM is required")
+    @validator("llm", always=True)
+    def validate_llm(cls, llm) -> LLM:
+        if not isinstance(llm, (LLM, LangchainLLM)):  # also covers llm is None
+            return BambooLLM()
         return llm
```

### Comparing `pandasai-2.0a9/pandasai/skills/__init__.py` & `pandasai-2.1a1/pandasai/skills/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 from typing import Any, Callable, Optional, Union
 
-from pydantic import BaseModel, PrivateAttr
+from pandasai.pydantic import BaseModel, PrivateAttr
 
 
 class Skill(BaseModel):
     """Skill that takes a function usable by pandasai"""
 
     func: Callable[..., Any]
     description: Optional[str] = None
```

### Comparing `pandasai-2.0a9/pandasai/smart_dataframe/__init__.py` & `pandasai-2.1a1/pandasai/smart_dataframe/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 
     df = SmartDataframe(df, config={"llm": llm})
     response = df.chat("What is the average loan amount?")
     print(response)
     # The average loan amount is $15,000.
     ```
 """
+
 import uuid
 from functools import cached_property
 from io import StringIO
 from typing import Any, List, Optional, Union
 
-import pydantic
-
 import pandasai.pandas as pd
-from pandasai.agent.base import Agent
+from pandasai.agent import Agent
 from pandasai.connectors.pandas import PandasConnector
 from pandasai.helpers.df_validator import DfValidator
+from pandasai.pydantic import BaseModel
 
 from ..connectors.base import BaseConnector
 from ..helpers.df_info import DataFrameType
 from ..helpers.logger import Logger
 from ..schemas.df_config import Config
 from ..skills import Skill
 
@@ -45,24 +45,22 @@
     def __init__(
         self,
         df: Union[DataFrameType, BaseConnector],
         name: str = None,
         description: str = None,
         custom_head: pd.DataFrame = None,
         config: Config = None,
-        logger: Logger = None,
     ):
         """
         Args:
             df: A supported dataframe type, or a pandasai Connector
             name (str, optional): Name of the dataframe. Defaults to None.
             description (str, optional): Description of the dataframe. Defaults to "".
             custom_head (pd.DataFrame, optional): Sample head of the dataframe.
             config (Config, optional): Config to be used. Defaults to None.
-            logger (Logger, optional): Logger to be used. Defaults to None.
         """
         self._original_import = df
 
         self._agent = Agent([df], config=config)
 
         self.dataframe = self._agent.context.dfs[0]
 
@@ -128,15 +126,15 @@
                         as a response object
 
         Raises:
             ValueError: If the query is empty
         """
         return self._agent.chat(query, output_type)
 
-    def validate(self, schema: pydantic.BaseModel):
+    def validate(self, schema: BaseModel):
         """
         Validates Dataframe rows on the basis Pydantic schema input
         (Args):
             schema: Pydantic schema class
             verbose: Print Errors
         """
         df_validator = DfValidator(self.dataframe)
```

### Comparing `pandasai-2.0a9/pandasai/smart_datalake/__init__.py` & `pandasai-2.1a1/pandasai/smart_datalake/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
     df = SmartDataframe(df, config={"llm": llm})
     response = df.chat("What is the average loan amount?")
     print(response)
     # The average loan amount is $15,000.
     ```
 """
+
 import uuid
 from typing import Any, List, Optional, Union
 
-from pandasai.agent.base import Agent
+from pandasai.agent import Agent
 from pandasai.skills import Skill
 
 from ..helpers.cache import Cache
 from ..helpers.df_info import DataFrameType
 from ..schemas.df_config import Config
 
 
@@ -34,15 +35,14 @@
         dfs: List[Union[DataFrameType, Any]],
         config: Optional[Union[Config, dict]] = None,
     ):
         """
         Args:
             dfs (List[Union[DataFrameType, Any]]): List of dataframes to be used
             config (Union[Config, dict], optional): Config to be used. Defaults to None.
-            logger (Logger, optional): Logger to be used. Defaults to None.
         """
         self._agent = Agent(dfs, config=config)
 
     def add_skills(self, *skills: Skill):
         """
         Add Skills to PandasAI
         """
```

### Comparing `pandasai-2.0a9/pandasai/vectorstores/bamboo_vectorstore.py` & `pandasai-2.1a1/pandasai/vectorstores/bamboo_vectorstore.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,26 +49,35 @@
         return True
 
     def get_relevant_qa_documents(self, question: str, k: int = None) -> List[dict]:
         """
         Returns relevant question answers based on search
         """
         k = k or self._max_samples
-        docs = self._session.get(
-            "/training-data/qa/relevant-qa", params={"query": question, "count": k}
-        )
-        return docs["docs"]
+
+        try:
+            docs = self._session.get(
+                "/training-data/qa/relevant-qa", params={"query": question, "count": k}
+            )
+            return docs["docs"]
+        except Exception:
+            self._logger.log("Querying without using training data.")
+            return []
 
     def get_relevant_docs_documents(
         self, question: str, k: Union[int, None] = 3
     ) -> List[str]:
         """
         Returns relevant question answers documents only
         Args:
             question (_type_): list of documents
         """
         k = k or self._max_samples
-
-        docs = self._session.get(
-            "/training-docs/docs/relevant-docs", params={"query": question, "count": k}
-        )
-        return docs["docs"]
+        try:
+            docs = self._session.get(
+                "/training-docs/docs/relevant-docs",
+                params={"query": question, "count": k},
+            )
+            return docs["docs"]
+        except Exception:
+            self._logger.log("Querying without using training docs.")
+            return []
```

### Comparing `pandasai-2.0a9/pandasai/vectorstores/chroma.py` & `pandasai-2.1a1/pandasai/ee/vectorstores/chroma.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pandasai.helpers.logger import Logger
 from pandasai.helpers.path import find_project_root
 from pandasai.vectorstores.vectorstore import VectorStore
 
 DEFAULT_EMBEDDING_FUNCTION = embedding_functions.DefaultEmbeddingFunction()
 
 
-class Chroma(VectorStore):
+class ChromaDB(VectorStore):
     """
     Implementation of ChromeDB vector store
     """
 
     _logger: Logger
 
     def __init__(
```

### Comparing `pandasai-2.0a9/pandasai/vectorstores/vectorstore.py` & `pandasai-2.1a1/pandasai/vectorstores/vectorstore.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a9/pyproject.toml` & `pandasai-2.1a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 [tool.poetry]
 name = "pandasai"
-version = "2.0a9"
-description = "PandasAI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
+version = "2.1a1"
+description = "Chat with your database (SQL, CSV, pandas, polars, mongodb, noSQL, etc). PandasAI makes data analysis conversational using LLMs (GPT 3.5 / 4, Anthropic, VertexAI) and RAG."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.9.7 || >3.9.7,<3.13"
+python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 python-dotenv = "^1.0.0"
 pandas = "1.5.3"
 astor = "^0.8.1"
 openai = "<2"
-ipython = "^8.13.1"
 matplotlib = "^3.7.1"
-pydantic = "^1"
+pydantic = ">=1,<3"
 sqlalchemy = ">=1.4,<3"
-duckdb = "^0.9.2"
+duckdb = "<1"
 faker = "^19.12.0"
 pillow = "^10.1.0"
 requests = "^2.31.0"
 jinja2 = "^3.1.3"
 modin = {version = "0.18.1", optional = true, extras=["ray"]}
 beautifulsoup4 = {version="^4.12.2", optional = true}
 google-generativeai = {version = "^0.3.2", optional = true}
 google-cloud-aiplatform = {version = "^1.26.1", optional = true}
-langchain = {version = "^0.0.199", optional = true}
+langchain = {version = "^0.1.0", optional = true}
 polars = {version = "^0.18.15", optional = true}
 statsmodels = {version = "^0.14.0", optional = true}
 scikit-learn = {version = "^1.2.2", optional = true}
 seaborn = {version = "^0.12.2", optional = true}
 plotly = {version = "^5.15.0", optional = true}
 kaleido = {version = "0.2.0", optional = true}
 ggplot = {version = "^0.11.5", optional = true}
 numpy = {version = "^1.17", optional = true}
 scipy = {version = "^1.9.0", optional = true}
 streamlit = {version = "^1.23.1", optional = true}
 text-generation = { version = ">=0.6.0", optional = true }
 openpyxl = { version = "^3.0.7", optional = true }
 pymysql = { version = "^1.1.0", optional = true }
-psycopg2 = { version = "^2.9.7", optional = true }
+psycopg2-binary = { version = "^2.9.7", optional = true }
 yfinance = { version = "^0.2.28", optional = true }
 sqlalchemy-databricks = { version = "^0.2.0", optional = true }
 snowflake-sqlalchemy = { version = "^1.5.0", optional = true }
 flask = { version = "^3.0.2", optional = true }
-sqlalchemy-bigquery = { version = "^1.8.0", optional = true }
+sqlalchemy-cockroachdb = { version = "^2.0.2", optional = true }
+sqlalchemy-bigquery = {version = "^1.8.0", optional = true, markers = "python_version >= '3.8' and python_version < '3.13'"}
 chromadb = {version = "^0.4.22", optional = true}
+boto3 = { version = ">=1.34.59", optional = true }
+qdrant-client = {version = "^1.8.0", extras = ["fastembed"], optional = true }
+ibm-watsonx-ai = { version = "^0.2.3", optional = true , markers = "python_version >= '3.10'"}
+cx-Oracle = { version = "^8.3.0", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
@@ -61,31 +65,35 @@
 pytest-env = "^0.8.1"
 click = "^8.1.3"
 coverage = "^7.2.7"
 sourcery = "^1.11.0"
 
 
 [tool.poetry.extras]
-connectors = [ "pymysql", "psycopg2",  "sqlalchemy-databricks", "sqlalchemy-bigquery", "snowflake-sqlalchemy"]
+connectors = [ "pymysql", "psycopg2-binary", "sqlalchemy-cockroachdb", "sqlalchemy-databricks", "sqlalchemy-bigquery", "snowflake-sqlalchemy", "cx-Oracle"]
 google-ai = ["google-generativeai", "google-cloud-aiplatform"]
 google-sheets = ["beautifulsoup4"]
 excel = ["openpyxl"]
 polars = ["polars"]
-langchain = ["langchain"]
+langchain = ["langchain", "langchain_openai", "langchain_community"]
 numpy = ["numpy"]
 ggplot = ["ggplot"]
 seaborn = ["seaborn"]
 plotly = ["plotly", "kaleido"]
 statsmodels = ["statsmodels"]
 scikit-learn = ["scikit-learn"]
 streamlit = ["streamlit"]
 text-generation = ["fsspec", "huggingface-hub", "text-generation"]
 yfinance = ["yfinance"]
 modin = ["modin", "ray"]
 chromadb = ["chromadb"]
+bedrock = ["boto3"]
+flask = ["flask"]
+qdrant = ["qdrant-client"]
+ibm-watsonx-ai = ["ibm-watsonx-ai"]
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "1.5.3"
 mkdocstrings-python = "1.7.2"
```

### Comparing `pandasai-2.0a9/PKG-INFO` & `pandasai-2.1a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,188 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 2.0a9
-Summary: PandasAI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
+Version: 2.1a1
+Summary: Chat with your database (SQL, CSV, pandas, polars, mongodb, noSQL, etc). PandasAI makes data analysis conversational using LLMs (GPT 3.5 / 4, Anthropic, VertexAI) and RAG.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: bedrock
 Provides-Extra: chromadb
 Provides-Extra: connectors
 Provides-Extra: excel
+Provides-Extra: flask
 Provides-Extra: ggplot
 Provides-Extra: google-ai
 Provides-Extra: google-sheets
+Provides-Extra: ibm-watsonx-ai
 Provides-Extra: langchain
 Provides-Extra: modin
 Provides-Extra: numpy
 Provides-Extra: plotly
 Provides-Extra: polars
+Provides-Extra: qdrant
 Provides-Extra: scikit-learn
 Provides-Extra: seaborn
 Provides-Extra: statsmodels
 Provides-Extra: streamlit
 Provides-Extra: text-generation
 Provides-Extra: yfinance
 Requires-Dist: astor (>=0.8.1,<0.9.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) ; extra == "google-sheets"
+Requires-Dist: boto3 (>=1.34.59) ; extra == "bedrock"
 Requires-Dist: chromadb (>=0.4.22,<0.5.0) ; extra == "chromadb"
-Requires-Dist: duckdb (>=0.9.2,<0.10.0)
+Requires-Dist: cx-Oracle (>=8.3.0,<9.0.0) ; extra == "connectors"
+Requires-Dist: duckdb (<1)
 Requires-Dist: faker (>=19.12.0,<20.0.0)
-Requires-Dist: flask (>=3.0.2,<4.0.0)
+Requires-Dist: flask (>=3.0.2,<4.0.0) ; extra == "flask"
 Requires-Dist: ggplot (>=0.11.5,<0.12.0) ; extra == "ggplot"
 Requires-Dist: google-cloud-aiplatform (>=1.26.1,<2.0.0) ; extra == "google-ai"
 Requires-Dist: google-generativeai (>=0.3.2,<0.4.0) ; extra == "google-ai"
-Requires-Dist: ipython (>=8.13.1,<9.0.0)
+Requires-Dist: ibm-watsonx-ai (>=0.2.3,<0.3.0) ; (python_version >= "3.10") and (extra == "ibm-watsonx-ai")
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
 Requires-Dist: kaleido (==0.2.0) ; extra == "plotly"
-Requires-Dist: langchain (>=0.0.199,<0.0.200) ; extra == "langchain"
+Requires-Dist: langchain (>=0.1.0,<0.2.0) ; extra == "langchain"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: modin[ray] (==0.18.1) ; extra == "modin"
 Requires-Dist: numpy (>=1.17,<2.0) ; extra == "numpy"
 Requires-Dist: openai (<2)
 Requires-Dist: openpyxl (>=3.0.7,<4.0.0) ; extra == "excel"
 Requires-Dist: pandas (==1.5.3)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0) ; extra == "plotly"
 Requires-Dist: polars (>=0.18.15,<0.19.0) ; extra == "polars"
-Requires-Dist: psycopg2 (>=2.9.7,<3.0.0) ; extra == "connectors"
-Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: psycopg2-binary (>=2.9.7,<3.0.0) ; extra == "connectors"
+Requires-Dist: pydantic (>=1,<3)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0) ; extra == "connectors"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: qdrant-client[fastembed] (>=1.8.0,<2.0.0) ; extra == "qdrant"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0) ; extra == "scikit-learn"
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "seaborn"
 Requires-Dist: snowflake-sqlalchemy (>=1.5.0,<2.0.0) ; extra == "connectors"
 Requires-Dist: sqlalchemy (>=1.4,<3)
-Requires-Dist: sqlalchemy-bigquery (>=1.8.0,<2.0.0) ; extra == "connectors"
+Requires-Dist: sqlalchemy-bigquery (>=1.8.0,<2.0.0) ; (python_version >= "3.8" and python_version < "3.13") and (extra == "connectors")
+Requires-Dist: sqlalchemy-cockroachdb (>=2.0.2,<3.0.0) ; extra == "connectors"
 Requires-Dist: sqlalchemy-databricks (>=0.2.0,<0.3.0) ; extra == "connectors"
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0) ; extra == "statsmodels"
 Requires-Dist: streamlit (>=1.23.1,<2.0.0) ; extra == "streamlit"
 Requires-Dist: text-generation (>=0.6.0) ; extra == "text-generation"
 Requires-Dist: yfinance (>=0.2.28,<0.3.0) ; extra == "yfinance"
 Description-Content-Type: text/markdown
 
-# PandasAI 🐼
+# ![PandasAI](images/logo.png)
 
 [![Release](https://img.shields.io/pypi/v/pandasai?label=Release&style=flat-square)](https://pypi.org/project/pandasai/)
 [![CI](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/ci.yml/badge.svg)
 [![CD](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)](https://github.com/gventuri/pandas-ai/actions/workflows/cd.yml/badge.svg)
 [![Coverage](https://codecov.io/gh/gventuri/pandas-ai/branch/main/graph/badge.svg)](https://codecov.io/gh/gventuri/pandas-ai)
-[![Documentation Status](https://readthedocs.org/projects/pandas-ai/badge/?version=latest)](https://pandas-ai.readthedocs.io/en/latest/?badge=latest)
 [![Discord](https://dcbadge.vercel.app/api/server/kF7FqH2FwS?style=flat&compact=true)](https://discord.gg/kF7FqH2FwS)
 [![Downloads](https://static.pepy.tech/badge/pandasai)](https://pepy.tech/project/pandasai) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
 
-PandasAI is a Python library that adds Generative AI capabilities to [pandas](https://github.com/pandas-dev/pandas), the popular data analysis and manipulation tool. It is designed to be used in conjunction with pandas, and is not a replacement for it.
+PandasAI is a Python library that makes it easy to ask questions to your data in natural language. It helps you to explore, clean, and analyze your data using generative AI.
 
-<!-- Add images/pandas-ai.png -->
+# 🔧 Getting started
 
-![PandasAI](images/pandas-ai.png?raw=true)
+The documentation for PandasAI to use it with specific LLMs, vector stores and connectors, can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
 
-## 🔧 Quick install
+## 📦 Installation
+
+With pip:
 
 ```bash
 pip install pandasai
 ```
 
-## 🔍 Demo
+With poetry:
 
-Try out PandasAI in your browser:
+```bash
+poetry add pandasai
+```
 
-[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
+## 🔍 Demo
 
-## 📖 Documentation
+Try out PandasAI yourself in your browser:
 
-The documentation for PandasAI can be found [here](https://pandas-ai.readthedocs.io/en/latest/).
+[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1ZnO-njhL7TBOYPZaqvMvGtsjckZKrv2E?usp=sharing)
 
-## 💻 Usage
+# 🚀 Deploying PandasAI
 
-> Disclaimer: GDP data was collected from [this source](https://ourworldindata.org/grapher/gross-domestic-product?tab=table), published by World Development Indicators - World Bank (2022.05.26) and collected at National accounts data - World Bank / OECD. It relates to the year of 2020. Happiness indexes were extracted from [the World Happiness Report](https://ftnnews.com/images/stories/documents/2020/WHR20.pdf). Another useful [link](https://data.world/makeovermonday/2020w19-world-happiness-report-2020).
+PandasAI can be deployed in a variety of ways. You can easily use it in your Jupyter notebooks or streamlit apps, or you can deploy it as a REST API such as with FastAPI or Flask.
 
-PandasAI is designed to be used in conjunction with pandas. It makes pandas conversational, allowing you to ask questions to your data in natural language.
+If you are interested in managed PandasAI Cloud or self-hosted Enterprise Offering, take a look at [our website](https://pandas-ai.com) or [book a meeting with us](https://zcal.co/gventuri/pandas-ai-demo).
 
-### Queries
+## 💻 Usage
 
-For example, you can ask PandasAI to find all the rows in a DataFrame where the value of a column is greater than 5, and it will return a DataFrame containing only those rows:
+### Ask questions
 
 ```python
+import os
 import pandas as pd
-from pandasai import SmartDataframe
+from pandasai import Agent
 
 # Sample DataFrame
-df = pd.DataFrame({
+sales_by_country = pd.DataFrame({
     "country": ["United States", "United Kingdom", "France", "Germany", "Italy", "Spain", "Canada", "Australia", "Japan", "China"],
-    "gdp": [19294482071552, 2891615567872, 2411255037952, 3435817336832, 1745433788416, 1181205135360, 1607402389504, 1490967855104, 4380756541440, 14631844184064],
-    "happiness_index": [6.94, 7.16, 6.66, 7.07, 6.38, 6.4, 7.23, 7.22, 5.87, 5.12]
+    "sales": [5000, 3200, 2900, 4100, 2300, 2100, 2500, 2600, 4500, 7000]
 })
 
-# Instantiate a LLM
-from pandasai.llm import OpenAI
-llm = OpenAI(api_token="YOUR_API_TOKEN")
+# By default, unless you choose a different LLM, it will use BambooLLM.
+# You can get your free API key signing up at https://pandabi.ai (you can also configure it in your .env file)
+os.environ["PANDASAI_API_KEY"] = "YOUR_API_KEY"
 
-df = SmartDataframe(df, config={"llm": llm})
-df.chat('Which are the 5 happiest countries?')
+agent = Agent(sales_by_country)
+agent.chat('Which are the top 5 countries by sales?')
 ```
 
-The above code will return the following:
-
 ```
-6            Canada
-7         Australia
-1    United Kingdom
-3           Germany
-0     United States
-Name: country, dtype: object
+China, United States, Japan, Germany, Australia
 ```
 
-Of course, you can also ask PandasAI to perform more complex queries. For example, you can ask PandasAI to find the sum of the GDPs of the 2 unhappiest countries:
+---
+
+Or you can ask more complex questions:
 
 ```python
-df.chat('What is the sum of the GDPs of the 2 unhappiest countries?')
+agent.chat(
+    "What is the total sales for the top 3 countries by sales?"
+)
 ```
 
-The above code will return the following:
-
 ```
-19012600725504
+The total sales for the top 3 countries by sales is 16500.
 ```
 
-### Charts
+### Visualize charts
 
-You can also ask PandasAI to draw a graph:
+You can also ask PandasAI to generate charts for you:
 
 ```python
-df.chat(
+agent.chat(
     "Plot the histogram of countries showing for each the gdp, using different colors for each bar",
 )
 ```
 
 ![Chart](images/histogram-chart.png?raw=true)
 
-You can save any charts generated by PandasAI by setting the `save_charts` parameter to `True` in the `PandasAI` constructor. For example, `PandasAI(llm, save_charts=True)`. Charts are saved in `./pandasai/exports/charts` .
-
 ### Multiple DataFrames
 
-Additionally, you can also pass in multiple dataframes to PandasAI and ask questions relating them.
+You can also pass in multiple dataframes to PandasAI and ask questions relating them.
 
 ```python
+import os
 import pandas as pd
-from pandasai import SmartDatalake
-from pandasai.llm import OpenAI
+from pandasai import Agent
 
 employees_data = {
     'EmployeeID': [1, 2, 3, 4, 5],
     'Name': ['John', 'Emma', 'Liam', 'Olivia', 'William'],
     'Department': ['HR', 'Sales', 'IT', 'Marketing', 'Finance']
 }
 
@@ -186,71 +190,48 @@
     'EmployeeID': [1, 2, 3, 4, 5],
     'Salary': [5000, 6000, 4500, 7000, 5500]
 }
 
 employees_df = pd.DataFrame(employees_data)
 salaries_df = pd.DataFrame(salaries_data)
 
+# By default, unless you choose a different LLM, it will use BambooLLM.
+# You can get your free API key signing up at https://pandabi.ai (you can also configure it in your .env file)
+os.environ["PANDASAI_API_KEY"] = "YOUR_API_KEY"
 
-llm = OpenAI()
-dl = SmartDatalake([employees_df, salaries_df], config={"llm": llm})
-dl.chat("Who gets paid the most?")
+agent = Agent([employees_df, salaries_df])
+agent.chat("Who gets paid the most?")
 ```
 
-The above code will return the following:
-
 ```
-Oh, Olivia gets paid the most.
+Olivia gets paid the most.
 ```
 
 You can find more examples in the [examples](examples) directory.
 
-### ⚡️ Shortcuts
-
-PandasAI also provides a number of shortcuts (beta) to make it easier to ask questions to your data. For example, you can ask PandasAI to `clean_data`, `impute_missing_values`, `generate_features`, `plot_histogram`, and many many more.
-
-```python
-# Clean data
-df.clean_data()
+## 🔒 Privacy & Security
 
-# Impute missing values
-df.impute_missing_values()
+In order to generate the Python code to run, we take some random samples from the dataframe, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the randomized head to the LLM.
 
-# Generate features
-df.generate_features()
+If you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
 
-# Plot histogram
-df.plot_histogram(column="gdp")
-```
+## 📜 License
 
-Learn more about the shortcuts [here](https://pandas-ai.readthedocs.io/en/latest/shortcuts/).
+PandasAI is available under the MIT expat license, except for the `pandasai/ee` directory (which has it's [license here](https://github.com/Sinaptik-AI/pandas-ai/blob/master/pandasai/ee/LICENSE) if applicable.
 
-## 🔒 Privacy & Security
+If you are interested in managed PandasAI Cloud or self-hosted Enterprise Offering, take a look at [our website](https://pandas-ai.com) or [book a meeting with us](https://zcal.co/gventuri/pandas-ai-demo).
 
-In order to generate the Python code to run, we take the dataframe head, we randomize it (using random generation for sensitive data and shuffling for non-sensitive data) and send just the head.
+## Resources
 
-Also, if you want to enforce further your privacy you can instantiate PandasAI with `enforce_privacy = True` which will not send the head (but just column names) to the LLM.
+- [Docs](https://pandas-ai.readthedocs.io/en/latest/) for comprehensive documentation
+- [Examples](examples) for example notebooks
+- [Discord](https://discord.gg/kF7FqH2FwS) for discussion with the community and PandasAI team
 
 ## 🤝 Contributing
 
-Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
-For more information, please see the [contributing guidelines](CONTRIBUTING.md).
+Contributions are welcome! Please check the outstanding issues and feel free to open a pull request.
+For more information, please check out the [contributing guidelines](CONTRIBUTING.md).
 
-After installing the virtual environment, please remember to install `pre-commit` to be compliant with our standards:
-
-```bash
-pre-commit install
-```
-
-## Contributors
+### Thank you!
 
 [![Contributors](https://contrib.rocks/image?repo=gventuri/pandas-ai)](https://github.com/gventuri/pandas-ai/graphs/contributors)
 
-## 📜 License
-
-PandasAI is licensed under the MIT License. See the LICENSE file for more details.
-
-## Acknowledgements
-
-- This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
-- This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
-
```

