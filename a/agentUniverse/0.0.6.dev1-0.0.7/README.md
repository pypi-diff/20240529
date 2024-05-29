# Comparing `tmp/agentuniverse-0.0.6.dev1.tar.gz` & `tmp/agentuniverse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentuniverse-0.0.6.dev1.tar", max compression
+gzip compressed data, was "agentuniverse-0.0.7.tar", max compression
```

## Comparing `agentuniverse-0.0.6.dev1.tar` & `agentuniverse-0.0.7.tar`

### file list

```diff
@@ -1,185 +1,196 @@
--rw-r--r--   0        0        0    11335 2024-04-02 12:08:01.834225 agentuniverse-0.0.6.dev1/LICENSE
--rw-r--r--   0        0        0     1527 2024-04-19 04:40:08.243214 agentuniverse-0.0.6.dev1/README_PYPI.md
--rw-r--r--   0        0        0      164 2024-04-02 03:12:13.474920 agentuniverse-0.0.6.dev1/agentuniverse/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.835519 agentuniverse-0.0.6.dev1/agentuniverse/agent/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835723 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835932 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.836127 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/__init__.py
--rw-r--r--   0        0        0      972 2024-05-24 05:33:08.351840 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/embedding.py
--rw-r--r--   0        0        0     4270 2024-05-24 05:33:08.352083 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
--rw-r--r--   0        0        0     3097 2024-04-26 03:46:54.112257 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge.py
--rw-r--r--   0        0        0      655 2024-04-26 03:46:54.140111 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge_manager.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837041 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837386 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/__init__.py
--rw-r--r--   0        0        0     1160 2024-04-26 03:46:54.147189 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
--rw-r--r--   0        0        0     1651 2024-05-24 05:33:08.352329 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
--rw-r--r--   0        0        0     1568 2024-04-26 03:46:54.126577 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
--rw-r--r--   0        0        0     1460 2024-04-26 03:46:54.173810 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
--rw-r--r--   0        0        0     1478 2024-05-24 05:33:08.352566 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
--rw-r--r--   0        0        0      552 2024-04-26 03:46:54.132260 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/reader.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.838782 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/__init__.py
--rw-r--r--   0        0        0     5872 2024-05-24 05:33:08.352856 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/chroma_store.py
--rw-r--r--   0        0        0     2206 2024-05-24 05:33:08.353136 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/document.py
--rw-r--r--   0        0        0      662 2024-04-02 12:08:01.839355 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/query.py
--rw-r--r--   0        0        0     3842 2024-05-07 11:44:48.809881 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/store.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.839707 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/__init__.py
--rw-r--r--   0        0        0      276 2024-04-02 12:08:01.839872 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/enum.py
--rw-r--r--   0        0        0     3868 2024-05-24 05:33:08.353396 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool.py
--rw-r--r--   0        0        0      626 2024-04-26 03:46:54.149120 agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool_manager.py
--rw-r--r--   0        0        0     5806 2024-05-21 09:31:45.014048 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent.py
--rw-r--r--   0        0        0      639 2024-04-26 03:44:12.686183 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_manager.py
--rw-r--r--   0        0        0      526 2024-04-02 12:08:01.840672 agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_model.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.840834 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/__init__.py
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.006641 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/__init__.py
--rw-r--r--   0        0        0     1257 2024-05-09 06:23:55.006784 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1446 2024-05-09 06:23:55.006896 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     3123 2024-05-21 09:31:45.014435 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/executing_agent.py
--rw-r--r--   0        0        0      367 2024-05-09 06:23:55.007062 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/executing_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.007720 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/__init__.py
--rw-r--r--   0        0        0     1499 2024-05-09 06:23:55.007805 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1866 2024-05-09 06:23:55.007888 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     2094 2024-05-21 09:31:45.014618 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.py
--rw-r--r--   0        0        0      365 2024-05-09 06:23:55.008036 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008209 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/__init__.py
--rw-r--r--   0        0        0     1353 2024-05-21 09:31:45.014795 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.py
--rw-r--r--   0        0        0      374 2024-05-09 06:23:55.008415 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008732 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-09 06:23:55.008817 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1613 2024-05-09 06:23:55.008890 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     1687 2024-05-21 09:31:45.014972 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.py
--rw-r--r--   0        0        0      353 2024-05-09 06:23:55.009031 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009190 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/__init__.py
--rw-r--r--   0        0        0      769 2024-05-09 06:23:55.009270 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0      884 2024-05-09 06:23:55.009355 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     1377 2024-05-21 09:31:45.015159 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.py
--rw-r--r--   0        0        0      276 2024-05-09 06:23:55.009511 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.yaml
--rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009871 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/__init__.py
--rw-r--r--   0        0        0     1222 2024-05-09 06:23:55.009950 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
--rw-r--r--   0        0        0     1412 2024-05-09 06:23:55.010031 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
--rw-r--r--   0        0        0     2011 2024-05-21 09:31:45.015355 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
--rw-r--r--   0        0        0      359 2024-05-09 06:23:55.010255 agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
--rw-r--r--   0        0        0      657 2024-04-02 12:08:01.841347 agentuniverse-0.0.6.dev1/agentuniverse/agent/input_object.py
--rw-r--r--   0        0        0      173 2024-04-09 07:08:39.103227 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/__init__.py
--rw-r--r--   0        0        0     3907 2024-05-24 05:33:08.353668 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/chat_memory.py
--rw-r--r--   0        0        0      174 2024-04-26 09:03:49.031587 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/__init__.py
--rw-r--r--   0        0        0      845 2024-04-26 09:03:49.032072 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.py
--rw-r--r--   0        0        0      321 2024-04-26 09:03:49.032468 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.yaml
--rw-r--r--   0        0        0      402 2024-04-01 06:19:56.174000 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/enum.py
--rw-r--r--   0        0        0     7689 2024-04-26 09:03:49.032798 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/langchain_instance.py
--rw-r--r--   0        0        0     3054 2024-05-24 05:33:08.353951 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory.py
--rw-r--r--   0        0        0      635 2024-04-26 03:46:54.130633 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory_manager.py
--rw-r--r--   0        0        0     2005 2024-05-24 05:33:08.354185 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/message.py
--rw-r--r--   0        0        0      754 2024-04-26 09:03:49.033037 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
--rw-r--r--   0        0        0      896 2024-04-26 09:03:49.033338 agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_en_prompt.yaml
--rw-r--r--   0        0        0      572 2024-04-02 12:08:01.842690 agentuniverse-0.0.6.dev1/agentuniverse/agent/output_object.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842823 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/__init__.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842962 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/__init__.py
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.142958 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/__init__.py
--rw-r--r--   0        0        0     3691 2024-05-21 09:31:45.017893 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
--rw-r--r--   0        0        0      195 2024-04-26 03:46:54.158656 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.144134 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
--rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018077 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
--rw-r--r--   0        0        0      200 2024-04-26 03:46:54.188023 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
--rw-r--r--   0        0        0      158 2024-04-09 16:15:17.145177 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/__init__.py
--rw-r--r--   0        0        0     8940 2024-05-21 09:31:45.018315 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
--rw-r--r--   0        0        0      170 2024-04-26 03:46:54.113707 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
--rw-r--r--   0        0        0     6449 2024-05-21 09:31:45.018505 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner.py
--rw-r--r--   0        0        0      659 2024-04-26 03:46:54.185023 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner_manager.py
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.145969 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/__init__.py
--rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018670 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
--rw-r--r--   0        0        0      190 2024-04-26 03:46:54.166967 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-02 12:08:01.843408 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/__init__.py
--rw-r--r--   0        0        0     3680 2024-05-21 09:31:45.018865 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
--rw-r--r--   0        0        0      165 2024-04-26 03:46:54.135943 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
--rw-r--r--   0        0        0      157 2024-04-09 16:15:17.147020 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
--rw-r--r--   0        0        0     3626 2024-05-21 09:31:45.019044 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
--rw-r--r--   0        0        0      195 2024-04-26 03:46:54.178755 agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
--rw-r--r--   0        0        0        0 2024-04-02 12:08:01.843939 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/__init__.py
--rw-r--r--   0        0        0     1944 2024-04-02 12:08:01.844114 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service.py
--rw-r--r--   0        0        0     3152 2024-04-26 03:46:54.144088 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_configer.py
--rw-r--r--   0        0        0     1161 2024-04-02 12:08:01.844424 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_instance.py
--rw-r--r--   0        0        0      402 2024-04-02 12:08:01.844558 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_manager.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844690 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844823 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.845006 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/__init__.py
--rw-r--r--   0        0        0     1075 2024-04-02 12:08:01.845143 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/request_do.py
--rw-r--r--   0        0        0     5602 2024-05-24 05:33:08.366607 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/request_library.py
--rw-r--r--   0        0        0     5019 2024-05-15 03:58:25.722266 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/flask_server.py
--rw-r--r--   0        0        0     2351 2024-04-26 15:29:30.265783 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/gunicorn_server.py
--rw-r--r--   0        0        0     9311 2024-04-26 09:03:49.038432 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/request_task.py
--rw-r--r--   0        0        0      164 2024-04-26 09:03:49.038779 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/__init__.py
--rw-r--r--   0        0        0      164 2024-05-15 03:58:25.722567 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/__init__.py
--rw-r--r--   0        0        0      617 2024-05-15 03:58:25.722726 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto
--rw-r--r--   0        0        0     2092 2024-05-15 03:58:25.722866 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py
--rw-r--r--   0        0        0     5979 2024-05-15 03:58:25.723032 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py
--rw-r--r--   0        0        0     5033 2024-05-15 03:58:25.723168 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py
--rw-r--r--   0        0        0     3307 2024-05-15 03:58:25.723368 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/rpc_server.py
--rw-r--r--   0        0        0     1146 2024-04-02 12:08:01.845635 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/thread_with_result.py
--rw-r--r--   0        0        0      822 2024-04-26 15:29:30.266263 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_booster.py
--rw-r--r--   0        0        0     2679 2024-04-26 15:29:30.266639 agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846346 agentuniverse-0.0.6.dev1/agentuniverse/base/__init__.py
--rw-r--r--   0        0        0    11557 2024-05-15 03:58:25.723582 agentuniverse-0.0.6.dev1/agentuniverse/base/agentuniverse.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846609 agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/__init__.py
--rw-r--r--   0        0        0      515 2024-04-02 12:08:01.846840 agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/singleton.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.847286 agentuniverse-0.0.6.dev1/agentuniverse/base/component/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-26 03:46:54.108902 agentuniverse-0.0.6.dev1/agentuniverse/base/component/application_component_manager.py
--rw-r--r--   0        0        0     1264 2024-04-26 03:46:54.107724 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_base.py
--rw-r--r--   0        0        0     4380 2024-04-26 09:03:49.040235 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_configer_util.py
--rw-r--r--   0        0        0      626 2024-04-26 09:03:49.040545 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_enum.py
--rw-r--r--   0        0        0     2576 2024-04-26 03:46:54.137220 agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_manager_base.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.848825 agentuniverse-0.0.6.dev1/agentuniverse/base/config/__init__.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.849235 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/__init__.py
--rw-r--r--   0        0        0     4173 2024-04-26 09:03:49.040952 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/app_configer.py
--rw-r--r--   0        0        0     1006 2024-04-26 03:46:54.105041 agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/application_config_manager.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850062 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/__init__.py
--rw-r--r--   0        0        0     2811 2024-04-26 09:03:49.041321 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/component_configer.py
--rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850500 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/__init__.py
--rw-r--r--   0        0        0     2599 2024-04-26 03:46:54.162861 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/agent_configer.py
--rw-r--r--   0        0        0     2053 2024-04-26 03:46:54.189422 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
--rw-r--r--   0        0        0     3272 2024-04-26 03:46:54.100009 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/llm_configer.py
--rw-r--r--   0        0        0     2540 2024-04-26 03:46:54.198928 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/memory_configer.py
--rw-r--r--   0        0        0     2392 2024-04-26 03:46:54.181023 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/planner_configer.py
--rw-r--r--   0        0        0     1889 2024-04-26 09:03:49.041670 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/prompt_configer.py
--rw-r--r--   0        0        0     2192 2024-04-26 03:46:54.165777 agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/tool_configer.py
--rw-r--r--   0        0        0      423 2024-04-02 12:08:01.852070 agentuniverse-0.0.6.dev1/agentuniverse/base/config/config_type_enum.py
--rw-r--r--   0        0        0     4846 2024-04-26 15:29:30.267459 agentuniverse-0.0.6.dev1/agentuniverse/base/config/configer.py
--rw-r--r--   0        0        0      163 2024-04-02 12:08:01.852534 agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/__init__.py
--rw-r--r--   0        0        0      707 2024-04-26 03:55:12.618569 agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/custom_key_configer.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.852949 agentuniverse-0.0.6.dev1/agentuniverse/base/context/__init__.py
--rw-r--r--   0        0        0     1447 2024-04-26 03:46:54.182246 agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context.py
--rw-r--r--   0        0        0     2768 2024-04-26 03:46:54.110018 agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context_manager.py
--rw-r--r--   0        0        0      174 2024-04-26 09:03:49.042097 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/__init__.py
--rw-r--r--   0        0        0      286 2024-04-26 09:03:49.042363 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/combine_cn_prompt.yaml
--rw-r--r--   0        0        0      318 2024-04-26 09:03:49.042631 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/combine_en_prompt.yaml
--rw-r--r--   0        0        0      253 2024-04-26 09:03:49.042893 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/summary_cn_prompt.yaml
--rw-r--r--   0        0        0      272 2024-04-26 09:03:49.043156 agentuniverse-0.0.6.dev1/agentuniverse/base/prompt/summary_en_prompt.yaml
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.853924 agentuniverse-0.0.6.dev1/agentuniverse/base/util/__init__.py
--rw-r--r--   0        0        0      307 2024-04-02 12:08:01.854131 agentuniverse-0.0.6.dev1/agentuniverse/base/util/env_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.854373 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/__init__.py
--rw-r--r--   0        0        0     6600 2024-04-26 03:42:29.579851 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/general_logger.py
--rw-r--r--   0        0        0     5132 2024-04-02 12:08:01.854819 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_config.py
--rw-r--r--   0        0        0     6395 2024-04-26 03:42:21.826133 agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_util.py
--rw-r--r--   0        0        0      502 2024-04-26 03:42:41.042298 agentuniverse-0.0.6.dev1/agentuniverse/base/util/memory_util.py
--rw-r--r--   0        0        0     7465 2024-05-21 09:31:45.019227 agentuniverse-0.0.6.dev1/agentuniverse/base/util/prompt_util.py
--rw-r--r--   0        0        0      715 2024-04-02 12:08:01.855496 agentuniverse-0.0.6.dev1/agentuniverse/base/util/system_util.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.855704 agentuniverse-0.0.6.dev1/agentuniverse/llm/__init__.py
--rw-r--r--   0        0        0      173 2024-04-02 12:08:01.855856 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/__init__.py
--rw-r--r--   0        0        0     1352 2024-04-26 09:03:49.043837 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/default_openai_llm.py
--rw-r--r--   0        0        0      223 2024-04-26 09:03:49.044133 agentuniverse-0.0.6.dev1/agentuniverse/llm/default/default_openai_llm.yaml
--rw-r--r--   0        0        0     5625 2024-05-24 05:33:08.354446 agentuniverse-0.0.6.dev1/agentuniverse/llm/langchain_instance.py
--rw-r--r--   0        0        0     5601 2024-05-16 08:48:01.873337 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm.py
--rw-r--r--   0        0        0      619 2024-04-26 03:46:54.138842 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_manager.py
--rw-r--r--   0        0        0      408 2024-04-26 09:03:49.045322 agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_output.py
--rw-r--r--   0        0        0     8294 2024-05-24 05:33:08.354632 agentuniverse-0.0.6.dev1/agentuniverse/llm/openai_llm.py
--rw-r--r--   0        0        0      156 2024-04-02 12:08:01.856945 agentuniverse-0.0.6.dev1/agentuniverse/prompt/__init__.py
--rw-r--r--   0        0        0     3351 2024-05-21 09:31:45.020660 agentuniverse-0.0.6.dev1/agentuniverse/prompt/chat_prompt.py
--rw-r--r--   0        0        0      548 2024-04-26 07:36:14.033265 agentuniverse-0.0.6.dev1/agentuniverse/prompt/enum.py
--rw-r--r--   0        0        0     2863 2024-05-21 09:31:45.020823 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt.py
--rw-r--r--   0        0        0      741 2024-04-26 09:03:49.046141 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_manager.py
--rw-r--r--   0        0        0     1882 2024-05-21 09:31:45.020988 agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_model.py
--rw-r--r--   0        0        0      164 2024-04-02 03:12:13.477398 agentuniverse-0.0.6.dev1/agentuniverse_connector/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 03:13:12.638584 agentuniverse-0.0.6.dev1/agentuniverse_extension/__init__.py
--rw-r--r--   0        0        0      164 2024-04-02 12:08:01.857428 agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/__init__.py
--rw-r--r--   0        0        0     7321 2024-04-02 12:08:01.857588 agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/sls_sink.py
--rw-r--r--   0        0        0     2586 2024-05-24 05:33:38.652207 agentuniverse-0.0.6.dev1/pyproject.toml
--rw-r--r--   0        0        0     3078 1970-01-01 00:00:00.000000 agentuniverse-0.0.6.dev1/PKG-INFO
+-rw-r--r--   0        0        0    11335 2024-04-02 12:08:01.834225 agentuniverse-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1527 2024-04-19 04:40:08.243214 agentuniverse-0.0.7/README_PYPI.md
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.474920 agentuniverse-0.0.7/agentuniverse/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.835519 agentuniverse-0.0.7/agentuniverse/agent/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835723 agentuniverse-0.0.7/agentuniverse/agent/action/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.835932 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.836127 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/embedding/__init__.py
+-rw-r--r--   0        0        0      972 2024-05-24 21:45:34.046778 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/embedding/embedding.py
+-rw-r--r--   0        0        0     4270 2024-05-24 21:45:34.047061 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py
+-rw-r--r--   0        0        0     3097 2024-04-26 03:46:54.112257 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/knowledge.py
+-rw-r--r--   0        0        0      655 2024-04-26 03:46:54.140111 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/knowledge_manager.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837041 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.837386 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/__init__.py
+-rw-r--r--   0        0        0     1160 2024-04-26 03:46:54.147189 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py
+-rw-r--r--   0        0        0     1651 2024-05-24 21:45:34.047302 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/file_reader.py
+-rw-r--r--   0        0        0     1568 2024-04-26 03:46:54.126577 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py
+-rw-r--r--   0        0        0     1460 2024-04-26 03:46:54.173810 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py
+-rw-r--r--   0        0        0     1478 2024-05-24 21:45:34.047531 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py
+-rw-r--r--   0        0        0      552 2024-04-26 03:46:54.132260 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/reader.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.838782 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/__init__.py
+-rw-r--r--   0        0        0     5872 2024-05-24 21:45:34.047763 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/chroma_store.py
+-rw-r--r--   0        0        0     2206 2024-05-24 21:45:34.047972 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/document.py
+-rw-r--r--   0        0        0      662 2024-04-02 12:08:01.839355 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/query.py
+-rw-r--r--   0        0        0     3842 2024-05-07 11:44:48.809881 agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/store.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.839707 agentuniverse-0.0.7/agentuniverse/agent/action/tool/__init__.py
+-rw-r--r--   0        0        0      276 2024-04-02 12:08:01.839872 agentuniverse-0.0.7/agentuniverse/agent/action/tool/enum.py
+-rw-r--r--   0        0        0     3868 2024-05-24 21:45:34.048195 agentuniverse-0.0.7/agentuniverse/agent/action/tool/tool.py
+-rw-r--r--   0        0        0      626 2024-04-26 03:46:54.149120 agentuniverse-0.0.7/agentuniverse/agent/action/tool/tool_manager.py
+-rw-r--r--   0        0        0     5806 2024-05-21 09:31:45.014048 agentuniverse-0.0.7/agentuniverse/agent/agent.py
+-rw-r--r--   0        0        0      639 2024-04-26 03:44:12.686183 agentuniverse-0.0.7/agentuniverse/agent/agent_manager.py
+-rw-r--r--   0        0        0      526 2024-04-02 12:08:01.840672 agentuniverse-0.0.7/agentuniverse/agent/agent_model.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.840834 agentuniverse-0.0.7/agentuniverse/agent/default/__init__.py
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.006641 agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-09 06:23:55.006784 agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1446 2024-05-09 06:23:55.006896 agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     3123 2024-05-21 09:31:45.014435 agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/executing_agent.py
+-rw-r--r--   0        0        0      367 2024-05-09 06:23:55.007062 agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/executing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.007720 agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/__init__.py
+-rw-r--r--   0        0        0     1499 2024-05-09 06:23:55.007805 agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1866 2024-05-09 06:23:55.007888 agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     2094 2024-05-21 09:31:45.014618 agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/expressing_agent.py
+-rw-r--r--   0        0        0      365 2024-05-09 06:23:55.008036 agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/expressing_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008209 agentuniverse-0.0.7/agentuniverse/agent/default/peer_agent/__init__.py
+-rw-r--r--   0        0        0     1353 2024-05-21 09:31:45.014795 agentuniverse-0.0.7/agentuniverse/agent/default/peer_agent/peer_agent.py
+-rw-r--r--   0        0        0      374 2024-05-27 07:31:21.494476 agentuniverse-0.0.7/agentuniverse/agent/default/peer_agent/peer_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.008732 agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-09 06:23:55.008817 agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1613 2024-05-09 06:23:55.008890 agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1687 2024-05-21 09:31:45.014972 agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/planning_agent.py
+-rw-r--r--   0        0        0      353 2024-05-09 06:23:55.009031 agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/planning_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009190 agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-09 06:23:55.009270 agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0      884 2024-05-09 06:23:55.009355 agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     1377 2024-05-21 09:31:45.015159 agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/rag_agent.py
+-rw-r--r--   0        0        0      277 2024-05-29 07:48:13.263777 agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/rag_agent.yaml
+-rw-r--r--   0        0        0      173 2024-05-09 06:23:55.009871 agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/__init__.py
+-rw-r--r--   0        0        0     1222 2024-05-09 06:23:55.009950 agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml
+-rw-r--r--   0        0        0     1412 2024-05-09 06:23:55.010031 agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml
+-rw-r--r--   0        0        0     2011 2024-05-21 09:31:45.015355 agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py
+-rw-r--r--   0        0        0      359 2024-05-09 06:23:55.010255 agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/reviewing_agent.yaml
+-rw-r--r--   0        0        0      657 2024-04-02 12:08:01.841347 agentuniverse-0.0.7/agentuniverse/agent/input_object.py
+-rw-r--r--   0        0        0      173 2024-04-09 07:08:39.103227 agentuniverse-0.0.7/agentuniverse/agent/memory/__init__.py
+-rw-r--r--   0        0        0     4048 2024-05-29 07:48:13.264662 agentuniverse-0.0.7/agentuniverse/agent/memory/chat_memory.py
+-rw-r--r--   0        0        0      174 2024-04-26 09:03:49.031587 agentuniverse-0.0.7/agentuniverse/agent/memory/default/__init__.py
+-rw-r--r--   0        0        0      845 2024-04-26 09:03:49.032072 agentuniverse-0.0.7/agentuniverse/agent/memory/default/default_memory.py
+-rw-r--r--   0        0        0      321 2024-04-26 09:03:49.032468 agentuniverse-0.0.7/agentuniverse/agent/memory/default/default_memory.yaml
+-rw-r--r--   0        0        0      402 2024-04-01 06:19:56.174000 agentuniverse-0.0.7/agentuniverse/agent/memory/enum.py
+-rw-r--r--   0        0        0     7689 2024-04-26 09:03:49.032798 agentuniverse-0.0.7/agentuniverse/agent/memory/langchain_instance.py
+-rw-r--r--   0        0        0     3054 2024-05-24 21:45:34.048580 agentuniverse-0.0.7/agentuniverse/agent/memory/memory.py
+-rw-r--r--   0        0        0      635 2024-04-26 03:46:54.130633 agentuniverse-0.0.7/agentuniverse/agent/memory/memory_manager.py
+-rw-r--r--   0        0        0     2005 2024-05-24 21:45:34.048799 agentuniverse-0.0.7/agentuniverse/agent/memory/message.py
+-rw-r--r--   0        0        0      754 2024-04-26 09:03:49.033037 agentuniverse-0.0.7/agentuniverse/agent/memory/summarizer_cn_prompt.yaml
+-rw-r--r--   0        0        0      896 2024-04-26 09:03:49.033338 agentuniverse-0.0.7/agentuniverse/agent/memory/summarizer_en_prompt.yaml
+-rw-r--r--   0        0        0      572 2024-04-02 12:08:01.842690 agentuniverse-0.0.7/agentuniverse/agent/output_object.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842823 agentuniverse-0.0.7/agentuniverse/agent/plan/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.842962 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.142958 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/executing_planner/__init__.py
+-rw-r--r--   0        0        0     3691 2024-05-21 09:31:45.017893 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.158656 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/executing_planner/executing_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.144134 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/expressing_planner/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018077 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py
+-rw-r--r--   0        0        0      200 2024-04-26 03:46:54.188023 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.yaml
+-rw-r--r--   0        0        0      158 2024-04-09 16:15:17.145177 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/peer_planner/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-27 07:53:03.277263 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py
+-rw-r--r--   0        0        0      170 2024-04-26 03:46:54.113707 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/peer_planner/peer_planner.yaml
+-rw-r--r--   0        0        0     6449 2024-05-21 09:31:45.018505 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planner.py
+-rw-r--r--   0        0        0      659 2024-04-26 03:46:54.185023 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planner_manager.py
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.145969 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planning_planner/__init__.py
+-rw-r--r--   0        0        0     3620 2024-05-21 09:31:45.018670 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py
+-rw-r--r--   0        0        0      190 2024-04-26 03:46:54.166967 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planning_planner/planning_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-02 12:08:01.843408 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/rag_planner/__init__.py
+-rw-r--r--   0        0        0     3679 2024-05-29 07:48:13.265628 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py
+-rw-r--r--   0        0        0      165 2024-04-26 03:46:54.135943 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/rag_planner/rag_planner.yaml
+-rw-r--r--   0        0        0      157 2024-04-09 16:15:17.147020 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/reviewing_planner/__init__.py
+-rw-r--r--   0        0        0     3626 2024-05-21 09:31:45.019044 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py
+-rw-r--r--   0        0        0      195 2024-04-26 03:46:54.178755 agentuniverse-0.0.7/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.yaml
+-rw-r--r--   0        0        0        0 2024-04-02 12:08:01.843939 agentuniverse-0.0.7/agentuniverse/agent_serve/__init__.py
+-rw-r--r--   0        0        0     1944 2024-04-02 12:08:01.844114 agentuniverse-0.0.7/agentuniverse/agent_serve/service.py
+-rw-r--r--   0        0        0     3152 2024-04-26 03:46:54.144088 agentuniverse-0.0.7/agentuniverse/agent_serve/service_configer.py
+-rw-r--r--   0        0        0     1161 2024-04-02 12:08:01.844424 agentuniverse-0.0.7/agentuniverse/agent_serve/service_instance.py
+-rw-r--r--   0        0        0      402 2024-04-02 12:08:01.844558 agentuniverse-0.0.7/agentuniverse/agent_serve/service_manager.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844690 agentuniverse-0.0.7/agentuniverse/agent_serve/web/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.844823 agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.845006 agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/entity/__init__.py
+-rw-r--r--   0        0        0     1075 2024-04-02 12:08:01.845143 agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/entity/request_do.py
+-rw-r--r--   0        0        0     5602 2024-05-24 21:45:34.056389 agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/request_library.py
+-rw-r--r--   0        0        0     5019 2024-05-15 03:58:25.722266 agentuniverse-0.0.7/agentuniverse/agent_serve/web/flask_server.py
+-rw-r--r--   0        0        0     2351 2024-04-26 15:29:30.265783 agentuniverse-0.0.7/agentuniverse/agent_serve/web/gunicorn_server.py
+-rw-r--r--   0        0        0     9311 2024-04-26 09:03:49.038432 agentuniverse-0.0.7/agentuniverse/agent_serve/web/request_task.py
+-rw-r--r--   0        0        0      164 2024-04-26 09:03:49.038779 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-15 03:58:25.722567 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/__init__.py
+-rw-r--r--   0        0        0      617 2024-05-15 03:58:25.722726 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto
+-rw-r--r--   0        0        0     2092 2024-05-15 03:58:25.722866 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py
+-rw-r--r--   0        0        0     5979 2024-05-15 03:58:25.723032 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5033 2024-05-15 03:58:25.723168 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py
+-rw-r--r--   0        0        0     3307 2024-05-15 03:58:25.723368 agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/rpc_server.py
+-rw-r--r--   0        0        0     1146 2024-04-02 12:08:01.845635 agentuniverse-0.0.7/agentuniverse/agent_serve/web/thread_with_result.py
+-rw-r--r--   0        0        0      822 2024-04-26 15:29:30.266263 agentuniverse-0.0.7/agentuniverse/agent_serve/web/web_booster.py
+-rw-r--r--   0        0        0     2679 2024-04-26 15:29:30.266639 agentuniverse-0.0.7/agentuniverse/agent_serve/web/web_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846346 agentuniverse-0.0.7/agentuniverse/base/__init__.py
+-rw-r--r--   0        0        0    11555 2024-05-29 07:48:13.266425 agentuniverse-0.0.7/agentuniverse/base/agentuniverse.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.846609 agentuniverse-0.0.7/agentuniverse/base/annotation/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-02 12:08:01.846840 agentuniverse-0.0.7/agentuniverse/base/annotation/singleton.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.847286 agentuniverse-0.0.7/agentuniverse/base/component/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-26 03:46:54.108902 agentuniverse-0.0.7/agentuniverse/base/component/application_component_manager.py
+-rw-r--r--   0        0        0     1374 2024-05-29 07:48:13.267156 agentuniverse-0.0.7/agentuniverse/base/component/component_base.py
+-rw-r--r--   0        0        0     4380 2024-04-26 09:03:49.040235 agentuniverse-0.0.7/agentuniverse/base/component/component_configer_util.py
+-rw-r--r--   0        0        0      626 2024-04-26 09:03:49.040545 agentuniverse-0.0.7/agentuniverse/base/component/component_enum.py
+-rw-r--r--   0        0        0     2576 2024-04-26 03:46:54.137220 agentuniverse-0.0.7/agentuniverse/base/component/component_manager_base.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.848825 agentuniverse-0.0.7/agentuniverse/base/config/__init__.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.849235 agentuniverse-0.0.7/agentuniverse/base/config/application_configer/__init__.py
+-rw-r--r--   0        0        0     4173 2024-04-26 09:03:49.040952 agentuniverse-0.0.7/agentuniverse/base/config/application_configer/app_configer.py
+-rw-r--r--   0        0        0     1006 2024-04-26 03:46:54.105041 agentuniverse-0.0.7/agentuniverse/base/config/application_configer/application_config_manager.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850062 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-26 09:03:49.041321 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/component_configer.py
+-rw-r--r--   0        0        0      165 2024-04-02 12:08:01.850500 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/__init__.py
+-rw-r--r--   0        0        0     2599 2024-04-26 03:46:54.162861 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/agent_configer.py
+-rw-r--r--   0        0        0     2053 2024-04-26 03:46:54.189422 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/knowledge_configer.py
+-rw-r--r--   0        0        0     3516 2024-05-29 07:48:13.267421 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/llm_configer.py
+-rw-r--r--   0        0        0     2540 2024-04-26 03:46:54.198928 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/memory_configer.py
+-rw-r--r--   0        0        0     2392 2024-04-26 03:46:54.181023 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/planner_configer.py
+-rw-r--r--   0        0        0     1889 2024-04-26 09:03:49.041670 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/prompt_configer.py
+-rw-r--r--   0        0        0     2192 2024-04-26 03:46:54.165777 agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/tool_configer.py
+-rw-r--r--   0        0        0      423 2024-04-02 12:08:01.852070 agentuniverse-0.0.7/agentuniverse/base/config/config_type_enum.py
+-rw-r--r--   0        0        0     4846 2024-04-26 15:29:30.267459 agentuniverse-0.0.7/agentuniverse/base/config/configer.py
+-rw-r--r--   0        0        0      163 2024-04-02 12:08:01.852534 agentuniverse-0.0.7/agentuniverse/base/config/custom_configer/__init__.py
+-rw-r--r--   0        0        0      707 2024-04-26 03:55:12.618569 agentuniverse-0.0.7/agentuniverse/base/config/custom_configer/custom_key_configer.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.852949 agentuniverse-0.0.7/agentuniverse/base/context/__init__.py
+-rw-r--r--   0        0        0     1447 2024-04-26 03:46:54.182246 agentuniverse-0.0.7/agentuniverse/base/context/framework_context.py
+-rw-r--r--   0        0        0     2768 2024-04-26 03:46:54.110018 agentuniverse-0.0.7/agentuniverse/base/context/framework_context_manager.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.853924 agentuniverse-0.0.7/agentuniverse/base/util/__init__.py
+-rw-r--r--   0        0        0      307 2024-04-02 12:08:01.854131 agentuniverse-0.0.7/agentuniverse/base/util/env_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.854373 agentuniverse-0.0.7/agentuniverse/base/util/logging/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-26 03:42:29.579851 agentuniverse-0.0.7/agentuniverse/base/util/logging/general_logger.py
+-rw-r--r--   0        0        0     5132 2024-04-02 12:08:01.854819 agentuniverse-0.0.7/agentuniverse/base/util/logging/logging_config.py
+-rw-r--r--   0        0        0     6395 2024-04-26 03:42:21.826133 agentuniverse-0.0.7/agentuniverse/base/util/logging/logging_util.py
+-rw-r--r--   0        0        0      502 2024-04-26 03:42:41.042298 agentuniverse-0.0.7/agentuniverse/base/util/memory_util.py
+-rw-r--r--   0        0        0      174 2024-05-29 07:48:13.267764 agentuniverse-0.0.7/agentuniverse/base/util/prompt/__init__.py
+-rw-r--r--   0        0        0      286 2024-05-29 07:48:13.268142 agentuniverse-0.0.7/agentuniverse/base/util/prompt/combine_cn_prompt.yaml
+-rw-r--r--   0        0        0      318 2024-05-29 07:48:13.268525 agentuniverse-0.0.7/agentuniverse/base/util/prompt/combine_en_prompt.yaml
+-rw-r--r--   0        0        0      253 2024-05-29 07:48:13.268796 agentuniverse-0.0.7/agentuniverse/base/util/prompt/summary_cn_prompt.yaml
+-rw-r--r--   0        0        0      272 2024-05-29 07:48:13.269073 agentuniverse-0.0.7/agentuniverse/base/util/prompt/summary_en_prompt.yaml
+-rw-r--r--   0        0        0     7990 2024-05-29 07:48:13.269301 agentuniverse-0.0.7/agentuniverse/base/util/prompt_util.py
+-rw-r--r--   0        0        0      715 2024-04-02 12:08:01.855496 agentuniverse-0.0.7/agentuniverse/base/util/system_util.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.855704 agentuniverse-0.0.7/agentuniverse/llm/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-02 12:08:01.855856 agentuniverse-0.0.7/agentuniverse/llm/default/__init__.py
+-rw-r--r--   0        0        0     1497 2024-05-29 07:48:13.269591 agentuniverse-0.0.7/agentuniverse/llm/default/baichuan_openai_style_llm.py
+-rw-r--r--   0        0        0      310 2024-05-29 07:48:13.269709 agentuniverse-0.0.7/agentuniverse/llm/default/baichuan_openai_style_llm.yaml
+-rw-r--r--   0        0        0     2658 2024-05-29 12:52:08.219303 agentuniverse-0.0.7/agentuniverse/llm/default/default_openai_llm.py
+-rw-r--r--   0        0        0      223 2024-04-26 09:03:49.044133 agentuniverse-0.0.7/agentuniverse/llm/default/default_openai_llm.yaml
+-rw-r--r--   0        0        0     1787 2024-05-29 07:48:13.270292 agentuniverse-0.0.7/agentuniverse/llm/default/kimi_openai_style_llm.py
+-rw-r--r--   0        0        0      225 2024-05-29 07:48:13.270401 agentuniverse-0.0.7/agentuniverse/llm/default/kimi_openai_style_llm.yaml
+-rw-r--r--   0        0        0     1591 2024-05-29 07:48:13.270544 agentuniverse-0.0.7/agentuniverse/llm/default/qwen_openai_style_llm.py
+-rw-r--r--   0        0        0      223 2024-05-29 07:48:13.270659 agentuniverse-0.0.7/agentuniverse/llm/default/qwen_openai_style_llm.yaml
+-rw-r--r--   0        0        0     5168 2024-05-29 07:48:13.270796 agentuniverse-0.0.7/agentuniverse/llm/default/wenxin_llm.py
+-rw-r--r--   0        0        0      223 2024-05-29 07:48:13.270906 agentuniverse-0.0.7/agentuniverse/llm/default/wenxin_llm.yaml
+-rw-r--r--   0        0        0     5625 2024-05-24 21:45:34.049034 agentuniverse-0.0.7/agentuniverse/llm/langchain_instance.py
+-rw-r--r--   0        0        0     5868 2024-05-29 07:48:13.271935 agentuniverse-0.0.7/agentuniverse/llm/llm.py
+-rw-r--r--   0        0        0      619 2024-04-26 03:46:54.138842 agentuniverse-0.0.7/agentuniverse/llm/llm_manager.py
+-rw-r--r--   0        0        0      408 2024-04-26 09:03:49.045322 agentuniverse-0.0.7/agentuniverse/llm/llm_output.py
+-rw-r--r--   0        0        0     8196 2024-05-29 07:48:13.272571 agentuniverse-0.0.7/agentuniverse/llm/openai_llm.py
+-rw-r--r--   0        0        0     5623 2024-05-29 07:48:13.272725 agentuniverse-0.0.7/agentuniverse/llm/openai_style_langchain_instance.py
+-rw-r--r--   0        0        0     7170 2024-05-29 07:48:13.272875 agentuniverse-0.0.7/agentuniverse/llm/openai_style_llm.py
+-rw-r--r--   0        0        0     8206 2024-05-29 07:48:13.273014 agentuniverse-0.0.7/agentuniverse/llm/wenxin_langchain_instance.py
+-rw-r--r--   0        0        0      156 2024-04-02 12:08:01.856945 agentuniverse-0.0.7/agentuniverse/prompt/__init__.py
+-rw-r--r--   0        0        0     3351 2024-05-21 09:31:45.020660 agentuniverse-0.0.7/agentuniverse/prompt/chat_prompt.py
+-rw-r--r--   0        0        0      548 2024-04-26 07:36:14.033265 agentuniverse-0.0.7/agentuniverse/prompt/enum.py
+-rw-r--r--   0        0        0     2863 2024-05-21 09:31:45.020823 agentuniverse-0.0.7/agentuniverse/prompt/prompt.py
+-rw-r--r--   0        0        0      741 2024-04-26 09:03:49.046141 agentuniverse-0.0.7/agentuniverse/prompt/prompt_manager.py
+-rw-r--r--   0        0        0     1882 2024-05-21 09:31:45.020988 agentuniverse-0.0.7/agentuniverse/prompt/prompt_model.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:12:13.477398 agentuniverse-0.0.7/agentuniverse_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 03:13:12.638584 agentuniverse-0.0.7/agentuniverse_extension/__init__.py
+-rw-r--r--   0        0        0      164 2024-04-02 12:08:01.857428 agentuniverse-0.0.7/agentuniverse_extension/logger/__init__.py
+-rw-r--r--   0        0        0     7321 2024-04-02 12:08:01.857588 agentuniverse-0.0.7/agentuniverse_extension/logger/sls_sink.py
+-rw-r--r--   0        0        0     2645 2024-05-29 14:02:02.754677 agentuniverse-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3201 1970-01-01 00:00:00.000000 agentuniverse-0.0.7/PKG-INFO
```

### Comparing `agentuniverse-0.0.6.dev1/LICENSE` & `agentuniverse-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/README_PYPI.md` & `agentuniverse-0.0.7/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/embedding.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/embedding/openai_embedding.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/knowledge.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/knowledge_manager.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/knowledge_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/docx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/file_reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/file_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/pptx_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/file/web_pdf_reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/reader/reader.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/reader/reader.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/chroma_store.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/chroma_store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/document.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/document.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/query.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/query.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/knowledge/store/store.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/knowledge/store/store.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/tool/tool.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/action/tool/tool_manager.py` & `agentuniverse-0.0.7/agentuniverse/agent/action/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_manager.py` & `agentuniverse-0.0.7/agentuniverse/agent/agent_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/agent_model.py` & `agentuniverse-0.0.7/agentuniverse/agent/agent_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/executing_agent/executing_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/executing_agent/executing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/expressing_agent/expressing_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/expressing_agent/expressing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/peer_agent/peer_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/peer_agent/peer_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/planning_agent/planning_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/planning_agent/planning_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/rag_agent/rag_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/rag_agent/rag_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/default_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/default_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py` & `agentuniverse-0.0.7/agentuniverse/agent/default/reviewing_agent/reviewing_agent.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/input_object.py` & `agentuniverse-0.0.7/agentuniverse/agent/input_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/chat_memory.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/chat_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,14 @@
         """Initialize the chat memory by the ComponentConfiger object.
         Args:
             component_configer(MemoryConfiger): the ComponentConfiger object
         Returns:
             ChatMemory: the ChatMemory object
         """
         super().initialize_by_component_configer(component_configer)
-        if component_configer.input_key:
+        if hasattr(component_configer, 'input_key') and component_configer.input_key:
             self.input_key = component_configer.input_key
-        if component_configer.output_key:
+        if hasattr(component_configer, 'output_key') and component_configer.output_key:
             self.output_key = component_configer.output_key
-        if component_configer.prompt_version:
+        if hasattr(component_configer, 'prompt_version') and component_configer.prompt_version:
             self.prompt_version = component_configer.prompt_version
         return self
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/default/default_memory.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/default/default_memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/langchain_instance.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/memory_manager.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/memory_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/message.py` & `agentuniverse-0.0.7/agentuniverse/agent/memory/message.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_cn_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/memory/summarizer_cn_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/memory/summarizer_en_prompt.yaml` & `agentuniverse-0.0.7/agentuniverse/agent/memory/summarizer_en_prompt.yaml`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/output_object.py` & `agentuniverse-0.0.7/agentuniverse/agent/output_object.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/executing_planner/executing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/expressing_planner/expressing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/peer_planner/peer_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planner_manager.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planner_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/planning_planner/planning_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/rag_planner/rag_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
         self.handle_all_actions(agent_model, planner_input, input_object)
 
         llm: LLM = self.handle_llm(agent_model)
 
         prompt: ChatPrompt = self.handle_prompt(agent_model, planner_input)
         process_llm_token(llm, prompt.as_langchain(), agent_model.profile, planner_input)
-
         llm_chain = LLMChain(llm=llm.as_langchain(),
                              prompt=prompt.as_langchain(),
                              output_key=self.output_key, memory=memory)
 
         return asyncio.run(llm_chain.acall(inputs=planner_input))
 
     def handle_prompt(self, agent_model: AgentModel, planner_input: dict) -> ChatPrompt:
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py` & `agentuniverse-0.0.7/agentuniverse/agent/plan/planner/reviewing_planner/reviewing_planner.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/service.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_configer.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/service_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/service_instance.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/service_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/entity/request_do.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/entity/request_do.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/dal/request_library.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/dal/request_library.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/flask_server.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/flask_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/gunicorn_server.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/gunicorn_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/request_task.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/request_task.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service.proto`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/agentuniverse_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/grpc/grpc_server_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/rpc/rpc_server.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/rpc/rpc_server.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/thread_with_result.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/thread_with_result.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_booster.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/web_booster.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/agent_serve/web/web_util.py` & `agentuniverse-0.0.7/agentuniverse/agent_serve/web/web_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/agentuniverse.py` & `agentuniverse-0.0.7/agentuniverse/base/agentuniverse.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def __init__(self):
         self.__application_container = ApplicationComponentManager()
         self.__config_container: ApplicationConfigManager = ApplicationConfigManager()
         self.__system_default_agent_package = ['agentuniverse.agent.default']
         self.__system_default_llm_package = ['agentuniverse.llm.default']
         self.__system_default_planner_package = ['agentuniverse.agent.plan.planner']
         self.__system_default_memory_package = ['agentuniverse.agent.memory.default']
-        self.__system_default_prompt_package = ['agentuniverse.agent', 'agentuniverse.base.prompt']
+        self.__system_default_prompt_package = ['agentuniverse.agent', 'agentuniverse.base.util']
 
     def start(self, config_path: str = None):
         """Start the agentUniverse framework."""
         # get default config path
         project_root_path = get_project_root_path()
         sys.path.append(str(project_root_path.parent))
         app_path = project_root_path / 'app'
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/annotation/singleton.py` & `agentuniverse-0.0.7/agentuniverse/base/annotation/singleton.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/component/application_component_manager.py` & `agentuniverse-0.0.7/agentuniverse/base/component/application_component_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_base.py` & `agentuniverse-0.0.7/agentuniverse/base/component/component_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 # @Time    : 2024/3/14 15:35
 # @Author  : jerry.zzw 
 # @Email   : jerry.zzw@antgroup.com
 # @FileName: component_base.py
 from abc import ABC
 
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 
 from agentuniverse.base.component.component_enum import ComponentEnum
 from agentuniverse.base.config.application_configer.application_config_manager import ApplicationConfigManager
 from agentuniverse.base.config.component_configer.component_configer import ComponentConfiger
 
 
 class ComponentBase(BaseModel):
     """The ComponentBase class, which is used to define the base class of the component."""
 
     component_type: ComponentEnum
+    # pydantic protected_namespaces config
+    model_config = ConfigDict(protected_namespaces=())
 
     def get_instance_code(self) -> str:
         """Return the full name of the component."""
         appname = ApplicationConfigManager().app_configer.base_info_appname
         return f'{appname}.{self.component_type.value.lower()}.{self.name}'
 
     def initialize_by_component_configer(self, component_configer: ComponentConfiger) -> 'ComponentBase':
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_configer_util.py` & `agentuniverse-0.0.7/agentuniverse/base/component/component_configer_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_enum.py` & `agentuniverse-0.0.7/agentuniverse/base/component/component_enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/component/component_manager_base.py` & `agentuniverse-0.0.7/agentuniverse/base/component/component_manager_base.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/app_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/application_configer/app_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/application_configer/application_config_manager.py` & `agentuniverse-0.0.7/agentuniverse/base/config/application_configer/application_config_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/component_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/component_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/agent_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/agent_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/knowledge_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/knowledge_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/llm_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/llm_configer.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         self.__model_name: Optional[str] = None
         self.__temperature: Optional[float] = None
         self.__request_timeout: Optional[int] = None
         self.__max_tokens: Optional[int] = None
         self.__max_retries: Optional[int] = None
         self.__streaming: Optional[bool] = None
         self.__ext_info: Optional[dict] = None
+        self.__max_context_length: Optional[int] = None
 
     @property
     def name(self) -> Optional[str]:
         """Return the name of the LLM."""
         return self.__name
 
     @property
@@ -61,14 +62,18 @@
     def streaming(self) -> Optional[bool]:
         return self.__streaming
 
     @property
     def ext_info(self) -> Optional[dict]:
         return self.__ext_info
 
+    @property
+    def max_content_length(self) -> Optional[int]:
+        return self.__max_context_length
+
     def load(self) -> 'LLMConfiger':
         """Load the configuration by the Configer object.
         Returns:
             LLMConfiger: the LLMConfiger object
         """
         return self.load_by_configer(self.__configer)
 
@@ -87,10 +92,11 @@
             self.__model_name = configer.value.get('model_name')
             self.__temperature = configer.value.get('temperature')
             self.__request_timeout = configer.value.get('request_timeout')
             self.__max_tokens = configer.value.get('max_tokens')
             self.__max_retries = configer.value.get('max_retries')
             self.__streaming = configer.value.get('streaming')
             self.__ext_info = configer.value.get('ext_info')
+            self.__max_context_length = configer.value.get('max_context_length')
         except Exception as e:
             raise Exception(f"Failed to parse the LLM configuration: {e}")
         return self
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/memory_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/memory_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/planner_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/planner_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/prompt_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/prompt_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/component_configer/configers/tool_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/component_configer/configers/tool_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/config/custom_configer/custom_key_configer.py` & `agentuniverse-0.0.7/agentuniverse/base/config/custom_configer/custom_key_configer.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context.py` & `agentuniverse-0.0.7/agentuniverse/base/context/framework_context.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/context/framework_context_manager.py` & `agentuniverse-0.0.7/agentuniverse/base/context/framework_context_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/general_logger.py` & `agentuniverse-0.0.7/agentuniverse/base/util/logging/general_logger.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_config.py` & `agentuniverse-0.0.7/agentuniverse/base/util/logging/logging_config.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/util/logging/logging_util.py` & `agentuniverse-0.0.7/agentuniverse/base/util/logging/logging_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/util/prompt_util.py` & `agentuniverse-0.0.7/agentuniverse/base/util/prompt_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @Email   : wangchongshi.wcs@antgroup.com
 # @FileName: prompt_util.py
 from typing import List
 
 from langchain.chains.summarize import load_summarize_chain
 from langchain_core.documents import Document
 
+from agentuniverse.agent.memory.enum import ChatMessageEnum
 from agentuniverse.agent.memory.message import Message
 from agentuniverse.llm.llm import LLM
 from agentuniverse.llm.llm_manager import LLMManager
 from agentuniverse.prompt.prompt_manager import PromptManager
 from agentuniverse.prompt.prompt_model import AgentPromptModel
 from agentuniverse.prompt.enum import PromptProcessEnum
 
@@ -116,14 +117,20 @@
     """
     message_list = []
     for attr in prompt_assemble_order:
         value = getattr(agent_prompt_model, attr, None)
         if value is not None:
             message_list.append(
                 Message(type=agent_prompt_model.get_message_type(attr), content=value))
+    if message_list:
+        # Integrate the system messages and put them in the first of the message list.
+        system_messages = '\n'.join(msg.content for msg in message_list if msg.type == ChatMessageEnum.SYSTEM.value)
+        if system_messages:
+            message_list = list(filter(lambda msg: msg.type != ChatMessageEnum.SYSTEM.value, message_list))
+            message_list.insert(0, Message(type=ChatMessageEnum.SYSTEM.value, content=system_messages))
     return message_list
 
 
 def process_llm_token(agent_llm: LLM, lc_prompt_template, profile: dict, planner_input: dict):
     """Process the prompt template based on the prompt processor.
 
     Args:
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/base/util/system_util.py` & `agentuniverse-0.0.7/agentuniverse/base/util/system_util.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/llm/langchain_instance.py` & `agentuniverse-0.0.7/agentuniverse/llm/langchain_instance.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/llm/llm.py` & `agentuniverse-0.0.7/agentuniverse/llm/llm.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     model_name: Optional[str] = None
     temperature: Optional[float] = 0.5
     request_timeout: Optional[int] = None
     max_tokens: Optional[int] = 1024
     max_retries: Optional[int] = 2
     streaming: Optional[bool] = False
     ext_info: Optional[dict] = None
+    __max_context_length: Optional[int] = None
 
     def __init__(self, **kwargs):
         """Initialize the llm."""
         super().__init__(component_type=ComponentEnum.LLM, **kwargs)
 
     def _new_client(self):
         """Initialize the client."""
@@ -96,14 +97,15 @@
             self.max_tokens = component_configer.max_tokens
         if component_configer.max_retries:
             self.max_retries = component_configer.max_retries
         if component_configer.streaming:
             self.streaming = component_configer.streaming
         if component_configer.ext_info:
             self.ext_info = component_configer.ext_info
+
         return self
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the LLM model in the agent configuration."""
         if 'model_name' in kwargs and kwargs['model_name']:
             self.model_name = kwargs['model_name']
         if 'temperature' in kwargs and kwargs['temperature']:
@@ -112,27 +114,32 @@
             self.request_timeout = kwargs['request_timeout']
         if 'max_tokens' in kwargs and kwargs['max_tokens']:
             self.max_tokens = kwargs['max_tokens']
         if 'max_retries' in kwargs and kwargs['max_retries']:
             self.max_retries = kwargs['max_retries']
         if 'streaming' in kwargs and kwargs['streaming']:
             self.streaming = kwargs['streaming']
+        if 'max_context_length' in kwargs and kwargs['max_context_length']:
+            self.__max_context_length = kwargs['max_context_length']
 
-    @abstractmethod
     def max_context_length(self) -> int:
         """Max context length.
 
         The total length of input tokens and generated tokens is limited by the model's context length.
         """
+        return self.__max_context_length
 
     @abstractmethod
     def get_num_tokens(self, text: str) -> int:
         """Get the number of tokens present in the text.
 
         Useful for checking if an input will fit in a model's context window.
 
         Args:
             text: The string input to tokenize.
 
         Returns:
             The integer number of tokens in the text.
         """
+
+    class Config:
+        protected_namespaces = ()
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/llm/llm_manager.py` & `agentuniverse-0.0.7/agentuniverse/llm/llm_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/llm/openai_llm.py` & `agentuniverse-0.0.7/agentuniverse/llm/openai_llm.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,51 +89,51 @@
         """Run the OpenAI LLM.
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
         streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
-        self.client = self._new_client()
-        with self.client as client:
-            chat_completion = client.chat.completions.create(
-                messages=messages,
-                model=kwargs.pop('model', self.model_name),
-                temperature=kwargs.pop('temperature', self.temperature),
-                stream=kwargs.pop('stream', streaming),
-                max_tokens=kwargs.pop('max_tokens', self.max_tokens),
-                **kwargs,
-            )
-            if not streaming:
-                text = chat_completion.choices[0].message.content
-                return LLMOutput(text=text, raw=chat_completion.model_dump())
-            return self.generate_stream_result(chat_completion)
+        if self.client is None:
+            self.client = self._new_client()
+        chat_completion = self.client.chat.completions.create(
+            messages=messages,
+            model=kwargs.pop('model', self.model_name),
+            temperature=kwargs.pop('temperature', self.temperature),
+            stream=kwargs.pop('stream', streaming),
+            max_tokens=kwargs.pop('max_tokens', self.max_tokens),
+            **kwargs,
+        )
+        if not streaming:
+            text = chat_completion.choices[0].message.content
+            return LLMOutput(text=text, raw=chat_completion.model_dump())
+        return self.generate_stream_result(chat_completion)
 
     async def acall(self, messages: list, **kwargs: Any) -> Union[LLMOutput, AsyncIterator[LLMOutput]]:
         """Asynchronously run the OpenAI LLM.
 
         Args:
             messages (list): The messages to send to the LLM.
             **kwargs: Arbitrary keyword arguments.
         """
         streaming = kwargs.pop("streaming") if "streaming" in kwargs else self.streaming
-        self.async_client = self._new_async_client()
-        async with self.async_client as async_client:
-            chat_completion = await async_client.chat.completions.create(
-                messages=messages,
-                model=kwargs.pop('model', self.model_name),
-                temperature=kwargs.pop('temperature', self.temperature),
-                stream=kwargs.pop('stream', streaming),
-                max_tokens=kwargs.pop('max_tokens', self.max_tokens),
-                **kwargs,
-            )
-            if not streaming:
-                text = chat_completion.choices[0].message.content
-                return LLMOutput(text=text, raw=chat_completion.model_dump())
-            return self.agenerate_stream_result(chat_completion)
+        if self.async_client is None:
+            self.async_client = self._new_async_client()
+        chat_completion = await self.async_client.chat.completions.create(
+            messages=messages,
+            model=kwargs.pop('model', self.model_name),
+            temperature=kwargs.pop('temperature', self.temperature),
+            stream=kwargs.pop('stream', streaming),
+            max_tokens=kwargs.pop('max_tokens', self.max_tokens),
+            **kwargs,
+        )
+        if not streaming:
+            text = chat_completion.choices[0].message.content
+            return LLMOutput(text=text, raw=chat_completion.model_dump())
+        return self.agenerate_stream_result(chat_completion)
 
     def as_langchain(self) -> BaseLanguageModel:
         """Convert the agentUniverse(aU) openai llm class to the langchain openai llm class."""
         return LangchainOpenAI(self)
 
     def set_by_agent_model(self, **kwargs) -> None:
         """ Assign values of parameters to the OpenAILLM model in the agent configuration."""
```

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/prompt/chat_prompt.py` & `agentuniverse-0.0.7/agentuniverse/prompt/chat_prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/prompt/enum.py` & `agentuniverse-0.0.7/agentuniverse/prompt/enum.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt.py` & `agentuniverse-0.0.7/agentuniverse/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_manager.py` & `agentuniverse-0.0.7/agentuniverse/prompt/prompt_manager.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse/prompt/prompt_model.py` & `agentuniverse-0.0.7/agentuniverse/prompt/prompt_model.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/agentuniverse_extension/logger/sls_sink.py` & `agentuniverse-0.0.7/agentuniverse_extension/logger/sls_sink.py`

 * *Files identical despite different names*

### Comparing `agentuniverse-0.0.6.dev1/pyproject.toml` & `agentuniverse-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentUniverse"
-version = "0.0.6.dev1"
+version = "0.0.7"
 description = "agentUniverse is a framework for developing applications powered by multi-agent base on large language model."
 
 authors = ["AntGroup <jerry.zzw@antgroup.com>"]
 repository = "https://github.com/alipay/agentUniverse"
 readme = "README_PYPI.md"
 
 packages = [
@@ -37,14 +37,17 @@
 grpcio = "1.63.0"
 chromadb = "0.4.24"
 sphinx = "^7.2.6"
 sphinx-rtd-theme = "^2.0.0"
 aliyun-log-python-sdk = { version = "0.8.8", optional = true}
 googleapis-common-protos = "^1.63.0"
 myst-parser = "^2.0.0"
+qianfan = "^0.3.12"
+dashscope = "^1.19.1"
+anthropic = "^0.26.0"
 
 [tool.poetry.extras]
 log_ext = ["aliyun-log-python-sdk"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
```

### Comparing `agentuniverse-0.0.6.dev1/PKG-INFO` & `agentuniverse-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 Metadata-Version: 2.1
 Name: agentUniverse
-Version: 0.0.6.dev1
+Version: 0.0.7
 Summary: agentUniverse is a framework for developing applications powered by multi-agent base on large language model.
 Home-page: https://github.com/alipay/agentUniverse
 Author: AntGroup
 Author-email: jerry.zzw@antgroup.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: log-ext
 Requires-Dist: SQLAlchemy (==2.0.25)
 Requires-Dist: aliyun-log-python-sdk (==0.8.8) ; extra == "log-ext"
+Requires-Dist: anthropic (>=0.26.0,<0.27.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: chromadb (==0.4.24)
+Requires-Dist: dashscope (>=1.19.1,<2.0.0)
 Requires-Dist: flask (==2.2)
 Requires-Dist: flask_cors (==4.0.0)
 Requires-Dist: googleapis-common-protos (>=1.63.0,<2.0.0)
 Requires-Dist: grpcio (==1.63.0)
 Requires-Dist: gunicorn (==21.2.0)
 Requires-Dist: langchain (==0.0.352)
 Requires-Dist: langchain-core (==0.1.3)
 Requires-Dist: loguru (==0.7.2)
 Requires-Dist: myst-parser (>=2.0.0,<3.0.0)
 Requires-Dist: openai (==1.13.3)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
+Requires-Dist: qianfan (>=0.3.12,<0.4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sphinx (>=7.2.6,<8.0.0)
 Requires-Dist: sphinx-rtd-theme (>=2.0.0,<3.0.0)
 Requires-Dist: tiktoken (==0.5.2)
 Requires-Dist: werkzeug (==2.2.2)
 Project-URL: Repository, https://github.com/alipay/agentUniverse
 Description-Content-Type: text/markdown
```

