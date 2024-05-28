# Comparing `tmp/lionagi-0.1.2.tar.gz` & `tmp/lionagi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lionagi-0.1.2.tar", last modified: Tue Apr 30 11:58:02 2024, max compression
+gzip compressed data, was "lionagi-0.2.0.tar", last modified: Tue May 28 22:45:41 2024, max compression
```

## Comparing `lionagi-0.1.2.tar` & `lionagi-0.2.0.tar`

### file list

```diff
@@ -1,263 +1,305 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-30 11:57:47.000000 lionagi-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-30 11:58:02.500678 lionagi-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-30 11:57:47.000000 lionagi-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-30 11:57:47.000000 lionagi-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.460678 lionagi-0.1.2/lionagi/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.460678 lionagi-0.1.2/lionagi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/agent/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18010 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/executable_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/flow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/branch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.464678 lionagi-0.1.2/lionagi/core/direct/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/cot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/react.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/direct/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/base_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/branch_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/instruction_map_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/neo4j_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/execute/structure_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/baseflow.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/mono_chat_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/monoflow/
--rw-r--r--   0 runner    (1001) docker     (127)     9637 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/ReAct.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/chat_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8938 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/monoflow/followup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/flow/polyflow/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/polyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/flow/polyflow/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.468678 lionagi-0.1.2/lionagi/core/form/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/action_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/form/scored_form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    17247 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/generic/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/mail/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/messages/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38111 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.472678 lionagi-0.1.2/lionagi/core/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/core/tool/tool_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/evaluator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/ast_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/base_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/sandbox_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/evaluator/script_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/directive/template_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/template_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/directive/template_/base_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/report/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.476678 lionagi-0.1.2/lionagi/experimental/tool/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/function_calling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/manual.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/tool_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/tool/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/validator/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/validator/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/work/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/async_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/work_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/experimental/work2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13320 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/form.py
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/report.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/util.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/work.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/work_function.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/experimental/work2/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/autogen_/autogen_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.480678 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/langchain_/langchain_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/get_index.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_pack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/textnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/bridge/transformers_/install_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/chunker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/chunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/chunker/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/config/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/mlx_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/oai_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/ollama_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/config/openrouter_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.484678 lionagi-0.1.2/lionagi/integrations/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/loader/load_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.488678 lionagi-0.1.2/lionagi/integrations/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/litellm.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/mistralai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/mlx_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/provider/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.488678 lionagi-0.1.2/lionagi/integrations/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25785 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)    10600 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/storage_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12145 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/structure_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/to_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/integrations/storage/to_excel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_knowledge_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/ln_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/libs/sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/coder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/add_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/base_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/coder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/coder/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/researcher/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/lions/researcher/data_source/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/finhub_.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/google_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/wiki_.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/lions/researcher/data_source/yfinance_.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.492678 lionagi-0.1.2/lionagi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/libs/test_sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.496678 lionagi-0.1.2/lionagi/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/lionagi/tests/test_core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/generic/test_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_base_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_chat_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_session_base_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/tests/test_core/test_tool_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 11:57:47.000000 lionagi-0.1.2/lionagi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 11:58:02.500678 lionagi-0.1.2/lionagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7834 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-30 11:58:02.000000 lionagi-0.1.2/lionagi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-30 11:57:47.000000 lionagi-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 11:58:02.500678 lionagi-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-30 11:57:47.000000 lionagi-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.092661 lionagi-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11288 2024-05-28 22:45:26.000000 lionagi-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-05-28 22:45:41.092661 lionagi-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-28 22:45:26.000000 lionagi-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-28 22:45:26.000000 lionagi-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.052661 lionagi-0.2.0/lionagi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.052661 lionagi-0.2.0/lionagi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/_setting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/_setting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/_setting/_setting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/action/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11753 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/action/tool_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/agent/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/eval/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/eval/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/agent/learn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/learn/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/agent/plan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/plan/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/agent/plan/unit_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.056661 lionagi-0.2.0/lionagi/core/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12104 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.060661 lionagi-0.2.0/lionagi/core/collections/abc/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/abc/concepts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/abc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/abc/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14846 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29444 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/progression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/collections/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.060661 lionagi-0.2.0/lionagi/core/director/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/director/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10111 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/director/direct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/director/director.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.060661 lionagi-0.2.0/lionagi/core/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12187 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/engine/branch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/engine/instruction_map_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/engine/sandbox_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/engine/script_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.060661 lionagi-0.2.0/lionagi/core/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/executor/base_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/executor/graph_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/executor/neo4j_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.060661 lionagi-0.2.0/lionagi/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/edge_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7265 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/hyperedge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/generic/tree_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.064661 lionagi-0.2.0/lionagi/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/mail/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/mail/mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/mail/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/mail/start_mail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.064661 lionagi-0.2.0/lionagi/core/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/action_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/action_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/assistant_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8419 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9764 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/message/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.064661 lionagi-0.2.0/lionagi/core/report/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/report/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7891 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/report/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/report/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/rule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7515 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/choice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/rulebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/rule/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14761 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/session/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/session/directive_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11012 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/structure/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/structure/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/structure/forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/structure/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/structure/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9332 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/parallel_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/unit/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/template/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12986 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/unit_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39312 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/unit_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/unit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.068661 lionagi-0.2.0/lionagi/core/validator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12012 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/validator/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/core/work/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/work_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/work_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6030 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/core/work/worklog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/compressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/compressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/compressor/llm_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/compressor/llm_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/compressor/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/directive/
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/directive/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10758 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/parser/base_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/directive/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/template/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/template/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/directive/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/evaluator/ast_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/evaluator/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.072661 lionagi-0.2.0/lionagi/experimental/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/knowledge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/knowledge/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/knowledge/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/experimental/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/memory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/experimental/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/experimental/strategies/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/autogen_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/autogen_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/autogen_/autogen_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/langchain_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/langchain_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4938 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/langchain_/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/llama_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/node_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/textnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/pydantic_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/pydantic_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/bridge/transformers_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/transformers_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/bridge/transformers_/install_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.076661 lionagi-0.2.0/lionagi/integrations/chunker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/chunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/chunker/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.080661 lionagi-0.2.0/lionagi/integrations/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/config/mlx_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/config/oai_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/config/ollama_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/config/openrouter_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.080661 lionagi-0.2.0/lionagi/integrations/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/loader/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/loader/load_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.080661 lionagi-0.2.0/lionagi/integrations/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/litellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/mistralai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/mlx_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/provider/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.080661 lionagi-0.2.0/lionagi/integrations/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25705 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10671 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/storage_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/structure_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/integrations/storage/to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.084661 lionagi-0.2.0/lionagi/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36870 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23883 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50382 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_knowledge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30183 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27226 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8963 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/ln_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/special_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19776 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/libs/sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.084661 lionagi-0.2.0/lionagi/lions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.084661 lionagi-0.2.0/lionagi/lions/coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/add_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/code_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/coder/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.084661 lionagi-0.2.0/lionagi/lions/researcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/lions/researcher/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/data_source/finhub_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/data_source/google_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/data_source/wiki_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/lions/researcher/data_source/yfinance_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20843 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13527 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/libs/test_sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.088661 lionagi-0.2.0/lionagi/tests/test_core/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8653 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/test_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/test_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/test_pile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/collections/test_progression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.092661 lionagi-0.2.0/lionagi/tests/test_core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/generic/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/generic/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/generic/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/generic/test_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/tests/test_core/test_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 22:45:26.000000 lionagi-0.2.0/lionagi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:45:41.092661 lionagi-0.2.0/lionagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-05-28 22:45:41.000000 lionagi-0.2.0/lionagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-05-28 22:45:41.000000 lionagi-0.2.0/lionagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:45:41.000000 lionagi-0.2.0/lionagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-28 22:45:41.000000 lionagi-0.2.0/lionagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 22:45:41.000000 lionagi-0.2.0/lionagi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 22:45:26.000000 lionagi-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:45:41.092661 lionagi-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-28 22:45:26.000000 lionagi-0.2.0/setup.py
```

### Comparing `lionagi-0.1.2/lionagi/core/direct/score.py` & `lionagi-0.2.0/lionagi/core/session/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,279 +1,311 @@
 """
-This module contains the ScoreTemplate class and related functions for scoring a given context using a language model.
+Copyright 2024 HaiyangLi
 
-The ScoreTemplate class is a subclass of ScoredTemplate and provides functionality for scoring a given context
-based on specified instructions, score range, and other parameters. It includes fields for the input sentence,
-score range, inclusive flag, number of digits, confidence score, and reason for the score.
-
-The module also includes functions for scoring a single instance or multiple instances of the context using the
-ScoreTemplate class and a language model.
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
-from pydantic import Field
-import numpy as np
-from lionagi.libs import func_call, convert
-from lionagi.core.form.scored_form import ScoredForm
-from lionagi.core.branch.branch import Branch
+from lionagi.core.collections import (
+    Pile,
+    Progression,
+    progression,
+    pile,
+    iModel,
+)
+from lionagi.core.message import System
+from typing import Any
+from lionagi.core.action.tool_manager import ToolManager
+
+from lionagi.libs import SysUtil
+from lionagi.core.session.branch import Branch
+from lionagi.core.collections import pile, Pile, Exchange
+from lionagi.core.collections.abc import get_lion_id
+from lionagi.core.collections.util import to_list_type
+from lionagi.core.mail.mail_manager import MailManager
 
 
-class ScoreTemplate(ScoredForm):
+class Session:
     """
-    A class for scoring a given context using a language model.
+    A session for managing branches, mail transfer, and interactions with a model.
 
     Attributes:
-        template_name (str): The name of the score template (default: "default_score").
-        sentence (str | list | dict): The given context to score.
-        answer (float): The numeric score for the context.
-        signature (str): The signature indicating the input and output fields (default: "sentence -> answer").
-
-    Methods:
-        __init__(self, sentence=None, instruction=None, score_range=(1, 10), inclusive=True, num_digit=0,
-                 confidence_score=False, reason=False, **kwargs):
-            Initializes a new instance of the ScoreTemplate class.
+        ln_id (str): The unique identifier for the session.
+        timestamp (str): The timestamp when the session was created.
+        system (System): The default system message for the session.
+        system_sender (str): The sender of the system message.
+        branches (Pile[Branch]): The pile of branches in the session.
+        mail_transfer (Exchange): The exchange for managing mail transfer.
+        mail_manager (MailManager): The manager for handling mail.
+        imodel (iModel): The model associated with the session.
+        user (str): The user associated with the session.
+        default_branch (Branch): The default branch of the session.
     """
 
-    template_name: str = "default_score"
-    sentence: str | list | dict = Field(
-        default_factory=str, description="the given context to score"
-    )
-    answer: float = Field(default_factory=float, description=f"a numeric score")
-    signature: str = "sentence -> answer"
-
     def __init__(
         self,
-        sentence=None,
-        instruction=None,
-        score_range=(1, 10),
-        inclusive=True,
-        num_digit=0,
-        confidence_score=False,
-        reason=False,
-        **kwargs,
+        system=None,  # the default system message for the session
+        branches: Any | None = None,
+        system_sender: str | None = None,
+        user: str | None = None,
+        imodel=None,
+        tools=None,
     ):
-        super().__init__(**kwargs)
-
-        self.sentence = sentence
-
-        return_precision = ""
-        if num_digit == 0:
-            return_precision = "integer"
+        self.ln_id = SysUtil.create_id()
+        self.timestamp = SysUtil.get_timestamp(sep=None)[:-6]
+        system = system or "You are a helpful assistant, let's think step by step"
+        self.system = System(system=system, sender=system_sender)
+        self.system_sender = system_sender
+        self.branches: Pile[Branch] = self._validate_branches(branches)
+        self.mail_transfer = Exchange()
+        self.mail_manager = MailManager([self.mail_transfer])
+        self.imodel = imodel or iModel()
+        self.user = user
+        self.default_branch = None
+        if self.branches.size() == 0:
+            self.new_branch(system=self.system.clone())
         else:
-            return_precision = f"num:{convert.to_str(num_digit)}f"
-
-        self.task = f"""
-score context according to the following constraints
-1. objective, {convert.to_str(instruction)}
-2. score range, {convert.to_str(score_range)}
-3. include_endpoints, {"yes" if inclusive else "no"}
-4. format the score in {return_precision}
-"""
-
-        if reason:
-            self.output_fields.append("reason")
-
-        if confidence_score:
-            self.output_fields.append("confidence_score")
-
-        self.out_validation_kwargs["answer"] = {
-            "upper_bound": score_range[1],
-            "lower_bound": score_range[0],
-            "num_type": int if num_digit == 0 else float,
-            "precision": num_digit if num_digit != 0 else None,
-        }
-
-
-async def _score(
-    sentence,
-    instruction=None,
-    score_range=(1, 10),
-    inclusive=True,
-    num_digit=0,
-    confidence_score=False,
-    reason=False,
-    retries=2,
-    delay=0.5,
-    backoff_factor=2,
-    default_value=None,
-    timeout=None,
-    branch_name=None,
-    system=None,
-    messages=None,
-    service=None,
-    sender=None,
-    llmconfig=None,
-    tools=None,
-    datalogger=None,
-    persist_path=None,
-    tool_manager=None,
-    **kwargs,
-):
-    """
-    Scores a given context using a language model.
-
-    Args:
-        sentence (str | list | dict): The given context to score.
-        instruction (Optional[str]): The instruction for scoring the context.
-        score_range (tuple): The range of valid scores (default: (1, 10)).
-        inclusive (bool): Whether to include the endpoints of the score range (default: True).
-        num_digit (int): The number of digits after the decimal point for the score (default: 0).
-        confidence_score (bool): Whether to include the confidence score in the output (default: False).
-        reason (bool): Whether to include the reason for the score in the output (default: False).
-        retries (int): The number of retries for the API call (default: 2).
-        delay (float): The initial delay between retries in seconds (default: 0.5).
-        backoff_factor (float): The backoff factor for exponential delay between retries (default: 2).
-        default_value (Optional[Any]): The default value to return if the API call fails (default: None).
-        timeout (Optional[float]): The timeout for the API call in seconds (default: None).
-        branch_name (Optional[str]): The name of the branch to use for scoring.
-        system (Optional[Any]): The system configuration for the branch.
-        messages (Optional[Any]): The messages to initialize the branch with.
-        service (Optional[Any]): The service to use for scoring.
-        sender (Optional[str]): The sender of the scoring request.
-        llmconfig (Optional[Any]): The configuration for the language model.
-        tools (Optional[Any]): The tools to use for scoring.
-        datalogger (Optional[Any]): The data logger for the branch.
-        persist_path (Optional[str]): The path to persist the branch data.
-        tool_manager (Optional[Any]): The tool manager for the branch.
-        **kwargs: Additional keyword arguments for the API call.
-
-    Returns:
-        ScoreTemplate: The score template with the scored context.
-    """
-
-    if "temperature" not in kwargs:
-        kwargs["temperature"] = 0.1
-
-    instruction = instruction or ""
-
-    branch = Branch(
-        name=branch_name,
-        system=system,
-        messages=messages,
-        service=service,
-        sender=sender,
-        llmconfig=llmconfig,
-        tools=tools,
-        datalogger=datalogger,
-        persist_path=persist_path,
-        tool_manager=tool_manager,
-    )
-
-    _template = ScoreTemplate(
-        sentence=sentence,
-        instruction=instruction,
-        score_range=score_range,
-        inclusive=inclusive,
-        num_digit=num_digit,
-        confidence_score=confidence_score,
-        reason=reason,
-    )
-
-    await func_call.rcall(
-        branch.chat,
-        form=_template,
-        retries=retries,
-        delay=delay,
-        backoff_factor=backoff_factor,
-        default=default_value,
-        timeout=timeout,
-        **kwargs,
-    )
-
-    return _template
-
-
-async def score(
-    sentence,
-    *,
-    num_instances=1,
-    instruction=None,
-    score_range=(1, 10),
-    inclusive=True,
-    num_digit=0,
-    confidence_score=False,
-    reason=False,
-    retries=2,
-    delay=0.5,
-    backoff_factor=2,
-    default_value=None,
-    timeout=None,
-    branch_name=None,
-    system=None,
-    messages=None,
-    service=None,
-    sender=None,
-    llmconfig=None,
-    tools=None,
-    datalogger=None,
-    persist_path=None,
-    tool_manager=None,
-    return_template=True,
-    **kwargs,
-) -> ScoreTemplate | float:
-    """
-    Scores a given context using a language model, with the option to score multiple instances.
-
-    Args:
-        sentence (str | list | dict): The given context to score.
-        num_instances (int): The number of instances to score (default: 1).
-        instruction (Optional[str]): The instruction for scoring the context.
-        score_range (tuple): The range of valid scores (default: (1, 10)).
-        inclusive (bool): Whether to include the endpoints of the score range (default: True).
-        num_digit (int): The number of digits after the decimal point for the score (default: 0).
-        confidence_score (bool): Whether to include the confidence score in the output (default: False).
-        reason (bool): Whether to include the reason for the score in the output (default: False).
-        retries (int): The number of retries for the API call (default: 2).
-        delay (float): The initial delay between retries in seconds (default: 0.5).
-        backoff_factor (float): The backoff factor for exponential delay between retries (default: 2).
-        default_value (Optional[Any]): The default value to return if the API call fails (default: None).
-        timeout (Optional[float]): The timeout for the API call in seconds (default: None).
-        branch_name (Optional[str]): The name of the branch to use for scoring.
-        system (Optional[Any]): The system configuration for the branch.
-        messages (Optional[Any]): The messages to initialize the branch with.
-        service (Optional[Any]): The service to use for scoring.
-        sender (Optional[str]): The sender of the scoring request.
-        llmconfig (Optional[Any]): The configuration for the language model.
-        tools (Optional[Any]): The tools to use for scoring.
-        datalogger (Optional[Any]): The data logger for the branch.
-        persist_path (Optional[str]): The path to persist the branch data.
-        tool_manager (Optional[Any]): The tool manager for the branch.
-        return_template (bool): Whether to return the score template or only the score (default: True).
-        **kwargs: Additional keyword arguments for the API call.
+            self.default_branch = self.branches[0]
+        if tools:
+            self.default_branch.tool_manager.register_tools(tools)
+
+    def _validate_branches(self, value):
+        """
+        Validates and converts the branches input to a Pile of Branch objects.
+
+        Args:
+            value (Any): The input value to validate and convert.
+
+        Returns:
+            Pile[Branch]: A pile of validated branches.
+
+        Raises:
+            ValueError: If the input value contains non-Branch objects.
+        """
+        if isinstance(value, Pile):
+            for branch in value:
+                if not isinstance(branch, Branch):
+                    raise ValueError("The branches pile contains non-Branch object")
+            return value
+        else:
+            try:
+                value = pile(items=value, item_type=Branch)
+                return value
+            except Exception as e:
+                raise ValueError(f"Invalid branches value. Error:{e}")
 
-    Returns:
-        ScoreTemplate | float: The score template with the scored context or the average score if `return_template` is False.
-    """
+    # ---- branch manipulation ---- #
+    def new_branch(
+        self,
+        system: System | None = None,
+        system_sender: str | None = None,
+        user: str | None = None,
+        messages: Pile = None,
+        progress: Progression = None,
+        tool_manager: ToolManager = None,
+        tools: Any = None,
+        imodel=None,
+    ):
+        """
+        Creates a new branch and adds it to the session.
 
-    async def _inner(i=0):
-        return await _score(
-            sentence=sentence,
-            instruction=instruction,
-            score_range=score_range,
-            inclusive=inclusive,
-            num_digit=num_digit,
-            confidence_score=confidence_score,
-            reason=reason,
-            retries=retries,
-            delay=delay,
-            backoff_factor=backoff_factor,
-            default_value=default_value,
-            timeout=timeout,
-            branch_name=branch_name,
+        Args:
+            system (System, optional): The system message for the branch.
+            system_sender (str, optional): The sender of the system message.
+            user (str, optional): The user associated with the branch.
+            messages (Pile, optional): The pile of messages for the branch.
+            progress (Progression, optional): The progression of messages.
+            tool_manager (ToolManager, optional): The tool manager for the branch.
+            tools (Any, optional): The tools to register with the tool manager.
+            imodel (iModel, optional): The model associated with the branch.
+
+        Returns:
+            Branch: The created branch.
+        """
+        if system is None:
+            system = self.system.clone()
+            system.sender = self.ln_id
+            system_sender = self.ln_id
+        branch = Branch(
             system=system,
+            system_sender=system_sender,
+            user=user,
             messages=messages,
-            service=service,
-            sender=sender,
-            llmconfig=llmconfig,
-            tools=tools,
-            datalogger=datalogger,
-            persist_path=persist_path,
+            progress=progress,
             tool_manager=tool_manager,
-            **kwargs,
+            tools=tools,
+            imodel=imodel or self.imodel,
         )
-
-    if num_instances == 1:
-        _out = await _inner()
-        return _out if return_template else _out.answer
-
-    elif num_instances > 1:
-        _outs = await func_call.alcall(range(num_instances), _inner)
-        return _outs if return_template else np.mean([i.answer for i in _outs])
+        self.branches.append(branch)
+        self.mail_manager.add_sources(branch)
+        if self.default_branch is None:
+            self.default_branch = branch
+        return branch
+
+    def delete_branch(self, branch):
+        """
+        Deletes a branch from the session.
+
+        Args:
+            branch (Branch | str): The branch or its ID to delete.
+        """
+        branch_id = get_lion_id(branch)
+        self.branches.pop(branch_id)
+        self.mail_manager.delete_source(branch_id)
+
+        if self.default_branch == branch:
+            if self.branches.size() == 0:
+                self.default_branch = None
+            else:
+                self.default_branch = self.branches[0]
+
+    def split_branch(self, branch):
+        """
+        Splits a branch, creating a new branch with the same messages and tools.
+
+        Args:
+            branch (Branch | str): The branch or its ID to split.
+
+        Returns:
+            Branch: The newly created branch.
+        """
+        branch = self.branches[branch]
+        system = branch.system.clone() if branch.system else None
+        if system:
+            system.sender = branch.ln_id
+        progress = progression()
+        messages = pile()
+
+        for id_ in branch.progress:
+            clone_message = branch.messages[id_].clone()
+            progress.append(clone_message.ln_id)
+            messages.append(clone_message)
+
+        tools = (
+            list(branch.tool_manager.registry.values())
+            if branch.tool_manager.registry
+            else None
+        )
+        branch_clone = Branch(
+            system=system,
+            system_sender=branch.ln_id,
+            user=branch.user,
+            progress=progress,
+            messages=messages,
+            tools=tools,
+        )
+        for message in branch_clone.messages:
+            message.sender = branch.ln_id
+            message.recipient = branch_clone.ln_id
+        self.branches.append(branch_clone)
+        self.mail_manager.add_sources(branch_clone)
+        return branch_clone
+
+    def change_default_branch(self, branch):
+        """
+        Changes the default branch of the session.
+
+        Args:
+            branch (Branch | str): The branch or its ID to set as the default.
+        """
+        branch = self.branches[branch]
+        self.default_branch = branch
+
+    def collect(self, from_: Branch | str | Pile[Branch] | None = None):
+        """
+        Collects mail from specified branches.
+
+        Args:
+            from_ (Branch | str | Pile[Branch], optional): The branches to collect mail from.
+                If None, collects mail from all branches.
+        """
+        if from_ is None:
+            self.mail_manager.collect_all()
+        else:
+            try:
+                sources = to_list_type(from_)
+                for source in sources:
+                    self.mail_manager.collect(get_lion_id(source))
+            except Exception as e:
+                raise ValueError(f"Failed to collect mail. Error: {e}")
+
+    def send(self, to_: Branch | str | Pile[Branch] | None = None):
+        """
+        Sends mail to specified branches.
+
+        Args:
+            to_ (Branch | str | Pile[Branch], optional): The branches to send mail to.
+                If None, sends mail to all branches.
+        """
+        if to_ is None:
+            self.mail_manager.send_all()
+        else:
+            try:
+                sources = to_list_type(to_)
+                for source in sources:
+                    self.mail_manager.send(get_lion_id(source))
+            except Exception as e:
+                raise ValueError(f"Failed to send mail. Error: {e}")
+
+    def collect_send_all(self, receive_all=False):
+        """
+        Collects and sends mail for all branches, optionally receiving all mail.
+
+        Args:
+            receive_all (bool, optional): Whether to receive all mail for all branches.
+        """
+        self.collect()
+        self.send()
+        if receive_all:
+            for branch in self.branches:
+                branch.receive_all()
+
+    async def chat(self, *args, branch=None, **kwargs):
+        """
+        Initiates a chat interaction with a branch.
+
+        Args:
+            *args: Positional arguments to pass to the chat method.
+            branch (Branch, optional): The branch to chat with. Defaults to the default branch.
+            **kwargs: Keyword arguments to pass to the chat method.
+
+        Returns:
+            Any: The result of the chat interaction.
+
+        Raises:
+            ValueError: If the specified branch is not found in the session branches.
+        """
+        if branch is None:
+            branch = self.default_branch
+        if branch not in self.branches:
+            raise ValueError("Branch not found in session branches")
+        return await self.branches[branch].chat(*args, **kwargs)
+
+    async def direct(self, *args, branch=None, **kwargs):
+        """
+        Initiates a direct interaction with a branch.
+
+        Args:
+            *args: Positional arguments to pass to the direct method.
+            branch (Branch, optional): The branch to interact with. Defaults to the default branch.
+            **kwargs: Keyword arguments to pass to the direct method.
+
+        Returns:
+            Any: The result of the direct interaction.
+
+        Raises:
+            ValueError: If the specified branch is not found in the session branches.
+        """
+        if branch is None:
+            branch = self.default_branch
+        if branch not in self.branches:
+            raise ValueError("Branch not found in session branches")
+        return await self.branches[branch].direct(*args, **kwargs)
```

### Comparing `lionagi-0.1.2/lionagi/core/execute/branch_executor.py` & `lionagi-0.2.0/lionagi/core/engine/branch_engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,134 +1,163 @@
 import contextlib
 from lionagi.libs import convert, AsyncUtil, ParseUtil
-from lionagi.core.generic import ActionNode, Edge
-from lionagi.core.mail.schema import BaseMail
-from lionagi.core.messages.schema import System, Instruction
+from lionagi.core.generic.edge import Edge
+from lionagi.core.action import ActionNode
+from lionagi.core.mail.mail import Mail
+from lionagi.core.message import System, Instruction
+from lionagi.core.collections import Pile, Progression
 
-from lionagi.core.branch.branch import Branch
-from lionagi.core.execute.base_executor import BaseExecutor
+from lionagi.core.session.branch import Branch
+from lionagi.core.executor.base_executor import BaseExecutor
 
 
 class BranchExecutor(Branch, BaseExecutor):
 
+    def __init__(
+        self,
+        context=None,
+        verbose=True,
+        system=None,
+        user=None,
+        messages=None,
+        progress=None,
+        tool_manager=None,
+        tools=None,
+        imodel=None,
+        **kwargs,
+    ):
+        super().__init__(
+            system=system,
+            user=user,
+            messages=messages,
+            progress=progress,
+            tool_manager=tool_manager,
+            tools=tools,
+            imodel=imodel,
+            **kwargs,
+        )
+        self.context = context
+        self.verbose = verbose
+
     async def forward(self) -> None:
         """
         Forwards the execution by processing all pending incoming mails in each branch. Depending on the category of the mail,
         it processes starts, nodes, node lists, conditions, or ends, accordingly executing different functions.
         """
-        for key in list(self.pending_ins.keys()):
-            while self.pending_ins[key]:
-                mail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile.pop(mail_id)
                 if mail.category == "start":
                     self._process_start(mail)
                 elif mail.category == "node":
                     await self._process_node(mail)
                 elif mail.category == "node_list":
                     self._process_node_list(mail)
                 elif mail.category == "condition":
-                    self._process_condition(mail)
+                    await self._process_condition(mail)
                 elif mail.category == "end":
                     self._process_end(mail)
+            if self.mailbox.pending_ins[key].size() == 0:
+                self.mailbox.pending_ins.pop(key)
 
     async def execute(self, refresh_time=1) -> None:
         """
         Executes the forward process repeatedly at specified time intervals until execution is instructed to stop.
 
         Args:
             refresh_time (int): The interval, in seconds, at which the forward method is called repeatedly.
         """
         while not self.execute_stop:
             await self.forward()
             await AsyncUtil.sleep(refresh_time)
 
-    async def _process_node(self, mail: BaseMail):
+    async def _process_node(self, mail: Mail):
         """
         Processes a single node based on the node type specified in the mail's package. It handles different types of nodes such as System,
         Instruction, ActionNode, and generic nodes through separate processes.
 
         Args:
-            mail (BaseMail): The mail containing the node to be processed along with associated details.
+            mail (Mail): The mail containing the node to be processed along with associated details.
 
         Raises:
             ValueError: If an invalid mail is encountered or the process encounters errors.
         """
-        if isinstance(mail.package["package"], System):
-            self._system_process(mail.package["package"], verbose=self.verbose)
+        node = mail.package.package
+        if isinstance(node, System):
+            self._system_process(node, verbose=self.verbose)
             self.send(
-                mail.sender_id,
-                "node_id",
-                {"request_source": self.id_, "package": mail.package["package"].id_},
+                recipient=mail.sender,
+                category="node_id",
+                package=node.ln_id,
+                request_source=self.ln_id,
             )
 
-        elif isinstance(mail.package["package"], Instruction):
-            await self._instruction_process(
-                mail.package["package"], verbose=self.verbose
-            )
+        elif isinstance(node, Instruction):
+            await self._instruction_process(node, verbose=self.verbose)
             self.send(
-                mail.sender_id,
-                "node_id",
-                {"request_source": self.id_, "package": mail.package["package"].id_},
+                recipient=mail.sender,
+                category="node_id",
+                package=node.ln_id,
+                request_source=self.ln_id,
             )
 
-        elif isinstance(mail.package["package"], ActionNode):
-            await self._action_process(mail.package["package"], verbose=self.verbose)
+        elif isinstance(node, ActionNode):
+            await self._action_process(node, verbose=self.verbose)
             self.send(
-                mail.sender_id,
-                "node_id",
-                {
-                    "request_source": self.id_,
-                    "package": mail.package["package"].instruction.id_,
-                },
+                recipient=mail.sender,
+                category="node_id",
+                package=node.instruction.ln_id,
+                request_source=self.ln_id,
             )
         else:
             try:
-                await self._agent_process(mail.package["package"], verbose=self.verbose)
+                await self._agent_process(node, verbose=self.verbose)
                 self.send(
-                    mail.sender_id,
-                    "node_id",
-                    {
-                        "request_source": self.id_,
-                        "package": mail.package["package"].id_,
-                    },
+                    recipient=mail.sender,
+                    category="node_id",
+                    package=node.ln_id,
+                    request_source=self.ln_id,
                 )
             except:
                 raise ValueError(f"Invalid mail to process. Mail:{mail}")
 
-    def _process_node_list(self, mail: BaseMail):
+    def _process_node_list(self, mail: Mail):
         """
         Processes a list of nodes provided in the mail, but currently only sends an end signal as multiple path selection is not supported.
 
         Args:
             mail (BaseMail): The mail containing a list of nodes to be processed.
 
         Raises:
             ValueError: When trying to process multiple paths which is currently unsupported.
         """
-        self.send(mail.sender_id, "end", {"request_source": self.id_, "package": "end"})
+        self.send(mail.sender, category="end", package="end", request_source=self.ln_id)
         self.execute_stop = True
-        raise ValueError("Multiple path selection is currently not supported")
+        raise ValueError("Multiple path selection is not supported in BranchExecutor")
 
-    def _process_condition(self, mail: BaseMail):
+    async def _process_condition(self, mail: Mail):
         """
         Processes a condition associated with an edge based on the mail's package, setting up the result of the condition check.
 
         Args:
             mail (BaseMail): The mail containing the condition to be processed.
         """
-        relationship: Edge = mail.package["package"]
-        check_result = relationship.condition(self)
+        edge: Edge = mail.package.package
+        check_result = await edge.check_condition(self)
         back_mail = {
-            "from": self.id_,
-            "edge_id": mail.package["package"].id_,
+            "from": self.ln_id,
+            "edge_id": edge.ln_id,
             "check_result": check_result,
         }
         self.send(
-            mail.sender_id,
-            "condition",
-            {"request_source": self.id_, "package": back_mail},
+            recipient=mail.sender,
+            category="condition",
+            package=back_mail,
+            request_source=self.ln_id,
         )
 
     def _system_process(self, system: System, verbose=True, context_verbose=False):
         """
         Processes a system node, possibly displaying its content and context if verbose is enabled.
 
         Args:
@@ -173,29 +202,30 @@
             display(
                 Markdown(
                     f"{instruction.sender}: {convert.to_str(instruction.instruct)}"
                 )
             )
 
         if self.context:
-            instruction.content.update({"context": self.context})
-            self.context_log.append(self.context)
+            result = await self.chat(
+                instruction=instruction.instruct, context=self.context, **kwargs
+            )
             self.context = None
+        else:
+            result = await self.chat(instruction=instruction.instruct, **kwargs)
+            # instruction._add_context(context=self.context)
+            # self.context_log.append(self.context)
+            # self.context = None
 
-        result = await self.chat(instruction, **kwargs)
         with contextlib.suppress(Exception):
             result = ParseUtil.fuzzy_parse_json(result)
-            if "response" in result.keys():
-                result = result["response"]
-        if verbose and len(self.assistant_responses) != 0:
-            display(
-                Markdown(
-                    f"{self.last_assistant_response.sender}: {convert.to_str(result)}"
-                )
-            )
+            if "assistant_response" in result.keys():
+                result = result["assistant_response"]
+        if verbose:
+            display(Markdown(f"assistant {self.ln_id}: {convert.to_str(result)}"))
             print("-----------------------------------------------------")
 
         self.execution_responses.append(result)
 
     async def _action_process(self, action: ActionNode, verbose=True):
         """
         Processes an action node, executing the defined action along with any tools specified within the node.
@@ -205,92 +235,99 @@
             verbose (bool): Flag to enable verbose output of the action results.
         """
         from lionagi.libs import SysUtil
 
         SysUtil.check_import("IPython")
         from IPython.display import Markdown, display
 
-        try:
-            func = getattr(self, action.action)
-        except:
-            raise ValueError(f"{action.action} is not a valid action")
+        # try:
+        #     func = getattr(self, action.action)
+        # except:
+        #     raise ValueError(f"{action.action} is not a valid action")
 
         if verbose:
             display(
                 Markdown(
                     f"{action.instruction.sender}: {convert.to_str(action.instruction.instruct)}"
                 )
             )
 
-        if action.tools:
-            self.register_tools(action.tools)
-        if self.context:
-            result = await func(
-                action.instruction.content["instruction"],
-                context=self.context,
-                tools=action.tools,
-                **action.action_kwargs,
-            )
-            self.context = None
-        else:
-            result = await func(
-                action.instruction.content, tools=action.tools, **action.action_kwargs
-            )
+        # if action.tools:
+        #     self.register_tools(action.tools)
+        # if self.context:
+        # result = await self.direct(
+        #     action.directive,
+        #     instruction=action.instruction.instruct,
+        #     context=self.context,
+        #     tools=action.tools,
+        #     **action.directive_kwargs,
+        # )
+        result = await action.invoke(branch=self, context=self.context)
+        self.context = None
+        # else:
+        #     result = await self.direct(
+        #         action.directive,
+        #         instruction=action.instruction.content,
+        #         tools=action.tools,
+        #         **action.directive_kwargs
+        #     )
 
-        if verbose and len(self.assistant_responses) != 0:
-            display(
-                Markdown(
-                    f"{self.last_assistant_response.sender}: {convert.to_str(result)}"
-                )
-            )
+        if verbose:
+            if action.directive == "chat":
+                display(Markdown(f"assistant {self.ln_id}: {convert.to_str(result)}"))
+            else:
+                display(Markdown(f"assistant {self.ln_id}:\n"))
+                for k, v in result.work_fields.items():
+                    display(Markdown(f"{k}: \n{v}\n"))
             print("-----------------------------------------------------")
 
         self.execution_responses.append(result)
 
     async def _agent_process(self, agent, verbose=True):
         """
         Processes an agent.
 
         Args:
             agent: The agent to process.
             verbose (bool): A flag indicating whether to provide verbose output (default: True).
         """
-        context = list(self.messages["content"])
+        context = [msg["content"] for msg in self.to_chat_messages()]
         if verbose:
             print("*****************************************************")
         result = await agent.execute(context)
 
         if verbose:
             print("*****************************************************")
 
-        from pandas import DataFrame
-
-        if isinstance(result, DataFrame):
-            self.context = list(result["content"])
-        else:
-            self.context = result
+        self.context = result
         self.execution_responses.append(result)
 
     def _process_start(self, mail):
         """
         Processes a start mail.
 
         Args:
             mail (BaseMail): The start mail to process.
         """
-        start_mail_content = mail.package
+        start_mail_content = mail.package.package
         self.context = start_mail_content["context"]
         self.send(
-            start_mail_content["structure_id"],
-            "start",
-            {"request_source": self.id_, "package": "start"},
+            recipient=start_mail_content["structure_id"],
+            category="start",
+            package="start",
+            request_source=self.ln_id,
         )
 
-    def _process_end(self, mail: BaseMail):
+    def _process_end(self, mail: Mail):
         """
         Processes an end mail.
 
         Args:
             mail (BaseMail): The end mail to process.
         """
         self.execute_stop = True
-        self.send(mail.sender_id, "end", {"request_source": self.id_, "package": "end"})
+        self.send(
+            recipient=mail.sender,
+            category="end",
+            package="end",
+            request_source=self.ln_id,
+        )
```

### Comparing `lionagi-0.1.2/lionagi/core/execute/instruction_map_executor.py` & `lionagi-0.2.0/lionagi/core/engine/instruction_map_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import asyncio
 from pydantic import Field
 
-from lionagi.libs import AsyncUtil
-
-from lionagi.core.mail.schema import BaseMail, MailTransfer
+from lionagi.core.mail.mail import Mail, Package
+from lionagi.core.collections import Exchange
 from lionagi.core.mail.mail_manager import MailManager
-from lionagi.core.execute.base_executor import BaseExecutor
-from lionagi.core.execute.branch_executor import BranchExecutor
+from lionagi.core.executor.base_executor import BaseExecutor
+from lionagi.core.engine.branch_engine import BranchExecutor
+from lionagi.core.collections import progression, pile, Pile
 
 
-class InstructionMapExecutor(BaseExecutor):
+class InstructionMapEngine(BaseExecutor):
     """
     Manages the execution of a mapped set of instructions across multiple branches within an executable structure.
 
     Attributes:
         branches (dict[str, BranchExecutor]): A dictionary of branch executors managing individual instruction flows.
         structure_id (str): The identifier for the structure within which these branches operate.
-        mail_transfer (MailTransfer): Handles the transfer of mail between branches and other components.
+        mail_transfer (Exchange): Handles the transfer of mail between branches and other components.
         branch_kwargs (dict): Keyword arguments used for initializing branches.
         num_end_branches (int): Tracks the number of branches that have completed execution.
         mail_manager (MailManager): Manages the distribution and collection of mails across branches.
     """
 
-    branches: dict[str, BranchExecutor] = Field(
+    branches: Pile[BranchExecutor] = Field(
         default_factory=dict, description="The branches of the instruction mapping."
     )
     structure_id: str = Field("", description="The ID of the executable structure.")
-    mail_transfer: MailTransfer = Field(
-        default_factory=MailTransfer, description="The mail transfer."
+    mail_transfer: Exchange = Field(
+        default_factory=Exchange, description="The mail transfer."
     )
     branch_kwargs: dict = Field(
         default_factory=dict,
         description="The keyword arguments for the initializing the branches.",
     )
     num_end_branches: int = Field(0, description="The number of end branches.")
     mail_manager: MailManager = Field(
@@ -49,124 +49,149 @@
         self.mail_manager = MailManager([self.mail_transfer])
 
     def transfer_ins(self):
         """
         Processes incoming mails, directing them appropriately based on their categories, and handles the initial setup
         of branches or the routing of node and condition mails.
         """
-        for key in list(self.pending_ins.keys()):
-            while self.pending_ins[key]:
-                mail: BaseMail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile.pop(mail_id)
                 if mail.category == "start":
                     self._process_start(mail)
                 elif mail.category == "node_list":
                     self._process_node_list(mail)
                 elif (
                     (mail.category == "node")
                     or (mail.category == "condition")
                     or (mail.category == "end")
                 ):
-                    mail.sender_id = self.mail_transfer.id_
-                    mail.recipient_id = mail.package["request_source"]
-                    self.mail_transfer.pending_outs.append(mail)
+                    mail.sender = self.mail_transfer.ln_id
+                    mail.recipient = mail.package.request_source
+                    self.mail_transfer.include(mail, "out")
 
     def transfer_outs(self):
         """
         Processes outgoing mails from the central mail transfer, handling end-of-execution notifications and routing
         other mails to appropriate recipients.
         """
         for key in list(self.mail_transfer.pending_ins.keys()):
-            while self.mail_transfer.pending_ins[key]:
-                mail: BaseMail = self.mail_transfer.pending_ins[key].popleft()
+            while self.mail_transfer.pending_ins[key].size() > 0:
+                mail_id = self.mail_transfer.pending_ins[key].popleft()
+                mail = self.mail_transfer.pile.pop(mail_id)
                 if mail.category == "end":
                     self.num_end_branches += 1
                     if self.num_end_branches == len(
                         self.branches
                     ):  # tell when structure should stop
-                        mail.sender_id = self.id_
-                        mail.recipient_id = self.structure_id
-                        self.pending_outs.append(mail)
+                        mail.sender = self.ln_id
+                        mail.recipient = self.structure_id
+                        self.mailbox.include(mail, "out")
                         self.execute_stop = True
                 else:
-                    mail.sender_id = self.id_
-                    mail.recipient_id = self.structure_id
-                    self.pending_outs.append(mail)
+                    mail.sender = self.ln_id
+                    mail.recipient = self.structure_id
+                    self.mailbox.include(mail, "out")
 
-    def _process_start(self, start_mail: BaseMail):
+    def _process_start(self, start_mail: Mail):
         """
         Processes a start mail to initialize a new branch executor and configures it based on the mail's package content.
 
         Args:
             start_mail (BaseMail): The mail initiating the start of a new branch execution.
         """
         branch = BranchExecutor(verbose=self.verbose, **self.branch_kwargs)
-        branch.context = start_mail.package["context"]
-        self.branches[branch.id_] = branch
+        branch.context = start_mail.package.package["context"]
+        self.branches[branch.ln_id] = branch
         self.mail_manager.add_sources([branch])
-        self.structure_id = start_mail.package["structure_id"]
-        mail = BaseMail(
-            sender_id=self.id_,
-            recipient_id=self.structure_id,
-            category="start",
-            package={"request_source": branch.id_, "package": "start"},
+        self.structure_id = start_mail.package.package["structure_id"]
+
+        pack = Package(category="start", package="start", request_source=branch.ln_id)
+        mail = Mail(
+            sender=self.ln_id,
+            recipient=self.structure_id,
+            package=pack,
         )
-        self.pending_outs.append(mail)
+        self.mailbox.include(mail, "out")
 
-    def _process_node_list(self, nl_mail: BaseMail):
+    def _process_node_list(self, nl_mail: Mail):
         """
         Processes a node list mail, setting up new branches or propagating the execution context based on the node list
         provided in the mail.
 
         Args:
             nl_mail (BaseMail): The mail containing a list of nodes to be processed in subsequent branches.
         """
-        source_branch_id = nl_mail.package["request_source"]
-        node_list = nl_mail.package["package"]
+        source_branch_id = nl_mail.package.request_source
+        node_list = nl_mail.package.package
         shared_context = self.branches[source_branch_id].context
         shared_context_log = self.branches[source_branch_id].context_log
         base_branch = self.branches[source_branch_id]
 
-        first_node_mail = BaseMail(
-            sender_id=self.mail_transfer.id_,
-            recipient_id=source_branch_id,
-            category="node",
-            package={"request_source": source_branch_id, "package": node_list[0]},
+        pack = Package(
+            category="node", package=node_list[0], request_source=source_branch_id
+        )
+        mail = Mail(
+            sender=self.mail_transfer.ln_id,
+            recipient=source_branch_id,
+            package=pack,
         )
-        self.mail_transfer.pending_outs.append(first_node_mail)
+        self.mail_transfer.include(mail, "out")
 
         for i in range(1, len(node_list)):
+            system = base_branch.system.clone() if base_branch.system else None
+            if system:
+                system.sender = base_branch.ln_id
+            progress = progression()
+            messages = pile()
+
+            for id_ in base_branch.progress:
+                clone_message = base_branch.messages[id_].clone()
+                progress.append(clone_message.ln_id)
+                messages.append(clone_message)
+
             branch = BranchExecutor(
                 verbose=self.verbose,
-                messages=base_branch.messages.copy(),
-                service=base_branch.service,
-                llmconfig=base_branch.llmconfig,
-                datalogger=base_branch.datalogger,
+                messages=messages,
+                user=base_branch.user,
+                system=base_branch.system.clone(),
+                progress=progress,
+                imodel=base_branch.imodel,
             )
+            for message in branch.messages:
+                message.sender = base_branch.ln_id
+                message.recipient = branch.ln_id
+
             branch.context = shared_context
             branch.context_log = shared_context_log
-            self.branches[branch.id_] = branch
+            self.branches[branch.ln_id] = branch
             self.mail_manager.add_sources([branch])
-            node_mail = BaseMail(
-                sender_id=self.mail_transfer.id_,
-                recipient_id=branch.id_,
-                category="node",
-                package={"request_source": source_branch_id, "package": node_list[i]},
+            node_pacakge = Package(
+                category="node", package=node_list[i], request_source=source_branch_id
+            )
+            node_mail = Mail(
+                sender=self.mail_transfer.ln_id,
+                recipient=branch.ln_id,
+                package=node_pacakge,
             )
-            self.mail_transfer.pending_outs.append(node_mail)
+            self.mail_transfer.include(node_mail, "out")
 
     async def forward(self):
         """
         Forwards the execution by processing all incoming and outgoing mails and advancing the state of all active branches.
         """
         self.transfer_ins()
         self.transfer_outs()
         self.mail_manager.collect_all()
         self.mail_manager.send_all()
         tasks = [
-            branch.forward() for branch in self.branches.values() if branch.pending_ins
+            branch.forward()
+            for branch in self.branches.values()
+            if branch.mailbox.pending_ins
         ]
         await asyncio.gather(*tasks)
         return
 
     async def execute(self, refresh_time=1):
         """
         Continuously executes the forward process at specified intervals until instructed to stop.
```

### Comparing `lionagi-0.1.2/lionagi/core/execute/neo4j_executor.py` & `lionagi-0.2.0/lionagi/core/executor/neo4j_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from collections import deque
 import json
 from typing import Callable
 
-from lionagi.core.execute.base_executor import BaseExecutor
+from lionagi.core.executor.base_executor import BaseExecutor
 from lionagi.integrations.storage.neo4j import Neo4j
 from lionagi.integrations.storage.storage_util import ParseNode
-from lionagi.core.generic import ActionNode
 from lionagi.core.agent.base_agent import BaseAgent
-from lionagi.core.execute.instruction_map_executor import InstructionMapExecutor
+from lionagi.core.engine.instruction_map_engine import InstructionMapEngine
 
-from lionagi.core.mail.schema import BaseMail
-from lionagi.core.tool import Tool
-from lionagi.core.generic import ActionSelection, Edge
+from lionagi.core.mail import Mail
+from lionagi.core.action import Tool, DirectiveSelection, ActionNode
+from lionagi.core.generic.edge import Edge
+from lionagi.core.collections.progression import progression
 
 from lionagi.libs import AsyncUtil
 
 
 class Neo4jExecutor(BaseExecutor):
     """
     Executes tasks within a Neo4j graph database, handling dynamic instruction flows and conditional logic across various nodes and agents.
@@ -29,17 +29,20 @@
         condition_check_result (bool | None): Result of the last condition check performed during execution.
     """
 
     driver: Neo4j | None
     structure_id: str = None
     structure_name: str = None
     middle_agents: list | None = None
-    default_agent_executable: BaseExecutor = InstructionMapExecutor()
+    default_agent_executable: BaseExecutor = InstructionMapEngine()
     condition_check_result: bool | None = None
 
+    class Config:
+        arbitrary_types_allowed = True
+
     async def check_edge_condition(
         self, condition, executable_id, request_source, head, tail
     ):
         """
         Evaluates the condition associated with an edge in the graph, determining if execution should proceed along that edge.
 
         Args:
@@ -48,42 +51,42 @@
             request_source (str): Origin of the request prompting this check.
             head (str): ID of the head node in the edge.
             tail (str): ID of the tail node in the edge.
 
         Returns:
             bool: Result of the condition check.
         """
-        if condition.source_type == "structure":
-            return condition(self)
-        elif condition.source_type == "executable":
+        if condition.source == "structure":
+            return condition.applies(self)
+        elif condition.source == "executable":
             return await self._check_executable_condition(
                 condition, executable_id, head, tail, request_source
             )
 
     def _process_edge_condition(self, edge_id):
         """
         Process the condition of a edge.
 
         Args:
             edge_id (str): The ID of the edge.
         """
-        for key in list(self.pending_ins.keys()):
-            skipped_requests = deque()
-            while self.pending_ins[key]:
-                mail: BaseMail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            skipped_requests = progression()
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile[mail_id]
                 if (
                     mail.category == "condition"
-                    and mail.package["package"]["edge_id"] == edge_id
+                    and mail.package.package["edge_id"] == edge_id
                 ):
-                    self.condition_check_result = mail.package["package"][
-                        "check_result"
-                    ]
+                    self.mailbox.pile.pop(mail_id)
+                    self.condition_check_result = mail.package.package["check_result"]
                 else:
                     skipped_requests.append(mail)
-            self.pending_ins[key] = skipped_requests
+            self.mailbox.pending_ins[key] = skipped_requests
 
     async def _check_executable_condition(
         self, condition, executable_id, head, tail, request_source
     ):
         """
         Sends a condition to be checked by an external executable and awaits the result.
 
@@ -95,21 +98,22 @@
             request_source (str): Source of the request for condition evaluation.
 
         Returns:
             bool: The result of the condition check.
         """
         edge = Edge(head=head, tail=tail, condition=condition)
         self.send(
-            recipient_id=executable_id,
+            recipient=executable_id,
             category="condition",
-            package={"request_source": request_source, "package": edge},
+            package=edge,
+            request_source=request_source,
         )
         while self.condition_check_result is None:
             await AsyncUtil.sleep(0.1)
-            self._process_edge_condition(edge.id_)
+            self._process_edge_condition(edge.ln_id)
             continue
         check_result = self.condition_check_result
         self.condition_check_result = None
         return check_result
 
     @staticmethod
     def parse_bundled_to_action(instruction, bundle_list):
@@ -122,61 +126,65 @@
 
         Returns:
             ActionNode: A node representing a composite action constructed from the bundled nodes.
         """
         bundled_nodes = deque()
         for node_labels, node_properties in bundle_list:
             try:
-                if "ActionSelection" in node_labels:
-                    node = ParseNode.parse_actionSelection(node_properties)
+                if "DirectiveSelection" in node_labels:
+                    node = ParseNode.parse_directiveSelection(node_properties)
                     bundled_nodes.append(node)
                 elif "Tool" in node_labels:
                     node = ParseNode.parse_tool(node_properties)
                     bundled_nodes.append(node)
                 else:
                     raise ValueError(
-                        f"Invalid bundle node {node_properties.id}. Valid nodes are ActionSelection or Tool"
+                        f"Invalid bundle node {node_properties.ln_id}. Valid nodes are ActionSelection or Tool"
                     )
             except Exception as e:
                 raise ValueError(
-                    f"Failed to parse ActionSelection or Tool node {node_properties.id}. Error: {e}"
+                    f"Failed to parse ActionSelection or Tool node {node_properties.ln_id}. Error: {e}"
                 )
 
         action_node = ActionNode(instruction=instruction)
         while bundled_nodes:
             node = bundled_nodes.popleft()
-            if isinstance(node, ActionSelection):
-                action_node.action = node.action
-                action_node.action_kwargs = node.action_kwargs
+            if isinstance(node, DirectiveSelection):
+                action_node.directive = node.directive
+                action_node.directive_kwargs = node.directive_kwargs
             elif isinstance(node, Tool):
                 action_node.tools.append(node)
         return action_node
 
     def parse_agent(self, node_properties):
         """
         Parses agent properties and creates an agent executor.
 
         Args:
             node_properties (dict): Properties defining the agent.
 
         Returns:
             BaseAgent: An agent executor configured with the given properties.
         """
-        output_parser = ParseNode.convert_to_def(node_properties["outputParser"])
+        output_parser = (
+            ParseNode.convert_to_def(node_properties["outputParser"])
+            if "outputParser" in node_properties
+            else None
+        )
 
         structure = Neo4jExecutor(
             driver=self.driver, structure_id=node_properties["structureId"]
         )
         agent = BaseAgent(
             structure=structure,
             executable=self.default_agent_executable,
             output_parser=output_parser,
+            ln_id=node_properties["ln_id"],
+            timestamp=node_properties["timestamp"],
         )
-        agent.id_ = node_properties["id"]
-        agent.timestamp = node_properties["timestamp"]
         return agent
 
     async def _next_node(
         self, query_list, node_id=None, executable_id=None, request_source=None
     ):
         """
         Processes the next set of nodes based on the results of a query list, applying conditions and preparing nodes
@@ -198,43 +206,43 @@
                     condition = json.loads(edge_properties["condition"])
                     condition_cls = await self.driver.get_condition_cls_code(
                         condition["class"]
                     )
                     condition_obj = ParseNode.parse_condition(condition, condition_cls)
 
                     head = node_id
-                    tail = node_properties["id"]
+                    tail = node_properties["ln_id"]
                     check = await self.check_edge_condition(
                         condition_obj, executable_id, request_source, head, tail
                     )
                     if not check:
                         continue
                 except Exception as e:
                     raise ValueError(
-                        f"Failed to use condition {edge_properties['condition']} from {node_id} to {node_properties['id']}, Error: {e}"
+                        f"Failed to use condition {edge_properties['condition']} from {node_id} to {node_properties['ln_id']}, Error: {e}"
                     )
 
             try:
                 if "System" in node_labels:
                     node = ParseNode.parse_system(node_properties)
                 elif "Instruction" in node_labels:
                     node = ParseNode.parse_instruction(node_properties)
                 elif "Agent" in node_labels:
                     node = self.parse_agent(node_properties)
 
                 else:
                     raise ValueError(
-                        f"Invalid start node {node_properties.id}. Valid nodes are System or Instruction"
+                        f"Invalid start node {node_properties.ln_id}. Valid nodes are System or Instruction"
                     )
             except Exception as e:
                 raise ValueError(
-                    f"Failed to parse System or Instruction node {node_properties.id}. Error: {e}"
+                    f"Failed to parse System or Instruction node {node_properties.ln_id}. Error: {e}"
                 )
 
-            bundle_list = await self.driver.get_bundle(node.id_)
+            bundle_list = await self.driver.get_bundle(node.ln_id)
 
             if bundle_list and "System" in node_labels:
                 raise ValueError("System node does not support bundle edge")
             if bundle_list:
                 node = self.parse_bundled_to_action(node, bundle_list)
             next_nodes.append(node)
         return next_nodes
@@ -243,18 +251,18 @@
         """
         Handles the start of execution, fetching and processing head nodes from the structure.
 
         Raises:
             ValueError: If there is an issue with finding or starting the structure.
         """
         try:
-            id, head_list = await self.driver.get_heads(
+            id_, head_list = await self.driver.get_heads(
                 self.structure_name, self.structure_id
             )
-            self.structure_id = id
+            self.structure_id = id_
             return await self._next_node(head_list)
         except Exception as e:
             raise ValueError(f"Error in searching for structure in Neo4j. Error: {e}")
 
     async def _handle_node_id(self, node_id, executable_id, request_source):
         """
         Handles the processing of a specific node ID, fetching its forward connections and conditions.
@@ -269,20 +277,20 @@
         """
         check = await self.driver.node_exist(node_id)
         if not check:
             raise ValueError(f"Node {node_id} if not found in the database")
         node_list = await self.driver.get_forwards(node_id)
         return await self._next_node(node_list, node_id, executable_id, request_source)
 
-    async def _handle_mail(self, mail: BaseMail):
+    async def _handle_mail(self, mail: Mail):
         """
         Processes incoming mail, determining the next action based on the mail's category and content.
 
         Args:
-            mail (BaseMail): The incoming mail to be processed.
+            mail (Mail): The incoming mail to be processed.
 
         Raises:
             ValueError: If there is an error processing the mail.
         """
         if mail.category == "start":
             try:
                 return await self._handle_start()
@@ -291,79 +299,74 @@
 
         elif mail.category == "end":
             self.execute_stop = True
             return None
 
         elif mail.category == "node_id":
             try:
-                node_id = mail.package["package"]
-                executable_id = mail.sender_id
-                request_source = mail.package["request_source"]
+                node_id = mail.package.package
+                executable_id = mail.sender
+                request_source = mail.package.request_source
                 return await self._handle_node_id(
                     node_id, executable_id, request_source
                 )
             except Exception as e:
                 raise ValueError(f"Error in handling node_id: {e}")
         elif mail.category == "node":
             try:
-                node_id = mail.package["package"].id_
-                executable_id = mail.sender_id
-                request_source = mail.package["request_source"]
+                node_id = mail.package.package.ln_id
+                executable_id = mail.sender
+                request_source = mail.package.request_source
                 return await self._handle_node_id(
                     node_id, executable_id, request_source
                 )
             except Exception as e:
                 raise ValueError(f"Error in handling node: {e}")
         else:
             raise ValueError(f"Invalid mail type for structure")
 
-    def _send_mail(self, next_nodes: list | None, mail: BaseMail):
+    def _send_mail(self, next_nodes: list | None, mail: Mail):
         """
         Sends out mail to the next nodes or marks the execution as ended if there are no next nodes.
 
         Args:
             next_nodes (list | None): List of next nodes to which mail should be sent.
-            mail (BaseMail): The current mail being processed.
+            mail (Mail): The current mail being processed.
         """
         if not next_nodes:  # tail
             self.send(
-                recipient_id=mail.sender_id,
+                recipient=mail.sender,
                 category="end",
-                package={
-                    "request_source": mail.package["request_source"],
-                    "package": "end",
-                },
+                package="end",
+                request_source=mail.package.request_source,
             )
         else:
             if len(next_nodes) == 1:
                 self.send(
-                    recipient_id=mail.sender_id,
+                    recipient=mail.sender,
                     category="node",
-                    package={
-                        "request_source": mail.package["request_source"],
-                        "package": next_nodes[0],
-                    },
+                    package=next_nodes[0],
+                    request_source=mail.package.request_source,
                 )
             else:
                 self.send(
-                    recipient_id=mail.sender_id,
+                    recipient=mail.sender,
                     category="node_list",
-                    package={
-                        "request_source": mail.package["request_source"],
-                        "package": next_nodes,
-                    },
+                    package=next_nodes,
+                    request_source=mail.package.request_source,
                 )
 
     async def forward(self) -> None:
         """
         Forwards execution by processing all pending mails and advancing to next nodes or actions.
         """
-        for key in list(self.pending_ins.keys()):
-            while self.pending_ins[key]:
-                mail: BaseMail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile.pop(mail_id)
                 try:
                     if mail == "end":
                         self.execute_stop = True
                         return
                     next_nodes = await self._handle_mail(mail)
                     self._send_mail(next_nodes, mail)
                 except Exception as e:
```

### Comparing `lionagi-0.1.2/lionagi/core/execute/structure_executor.py` & `lionagi-0.2.0/lionagi/core/executor/graph_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from typing import overload
-
-from abc import ABC
 from collections import deque
 
 from lionagi.libs import AsyncUtil, convert
 
-from lionagi.core.generic import BaseNode, ActionNode, ActionSelection, Edge
-from lionagi.core.tool import Tool
-from lionagi.core.mail.schema import BaseMail
-from lionagi.core.execute.base_executor import BaseExecutor
+from lionagi.core.generic.node import Node
+from lionagi.core.generic.edge import Edge
+from lionagi.core.executor.base_executor import BaseExecutor
 
-from lionagi.libs import AsyncUtil
-from lionagi.core.generic import Node, ActionSelection, Edge
-from lionagi.core.tool import Tool
+from lionagi.core.action import Tool, DirectiveSelection, ActionNode
 
-from lionagi.core.mail.schema import BaseMail
-from lionagi.core.graph.graph import Graph
+from lionagi.core.mail import Mail
+from lionagi.core.generic.graph import Graph
+from lionagi.core.collections.progression import progression
 
 
-class StructureExecutor(BaseExecutor, Graph):
+class GraphExecutor(BaseExecutor, Graph):
     """
     Executes tasks within a graph structure, handling dynamic node flows and conditional edge logic.
 
     Attributes:
         condition_check_result (bool | None): Result of the last condition check performed during execution,
             used to control flow based on dynamic conditions.
     """
@@ -41,46 +36,48 @@
 
         Returns:
             bool: Result of the condition evaluation.
 
         Raises:
             ValueError: If the source_type of the condition is invalid.
         """
-        if edge.condition.source_type == "structure":
-            return edge.condition(self)
+        if edge.condition.source == "structure" or isinstance(
+            edge.condition.source, Node
+        ):
+            return await edge.check_condition(self)
 
-        elif edge.condition.source_type == "executable":
+        elif edge.condition.source == "executable":
             return await self._check_executable_condition(
                 edge, executable_id, request_source
             )
 
         else:
             raise ValueError("Invalid source_type.")
 
     def _process_edge_condition(self, edge_id):
         """
         Process the condition of a edge.
 
         Args:
             edge_id (str): The ID of the edge.
         """
-        for key in list(self.pending_ins.keys()):
-            skipped_requests = deque()
-            while self.pending_ins[key]:
-                mail: BaseMail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            skipped_requests = progression()
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile[mail_id]
                 if (
                     mail.category == "condition"
-                    and mail.package["package"]["edge_id"] == edge_id
+                    and mail.package.package["edge_id"] == edge_id
                 ):
-                    self.condition_check_result = mail.package["package"][
-                        "check_result"
-                    ]
+                    self.mailbox.pile.pop(mail_id)
+                    self.condition_check_result = mail.package.package["check_result"]
                 else:
                     skipped_requests.append(mail)
-            self.pending_ins[key] = skipped_requests
+            self.mailbox.pending_ins[key] = skipped_requests
 
     async def _check_executable_condition(
         self, edge: Edge, executable_id, request_source
     ):
         """
         Sends the edge's condition to an external executable for evaluation and waits for the result.
 
@@ -89,66 +86,67 @@
             executable_id (str): ID of the executable that will evaluate the condition.
             request_source (str): Source of the request for condition evaluation.
 
         Returns:
             bool: The result of the condition check.
         """
         self.send(
-            recipient_id=executable_id,
+            recipient=executable_id,
             category="condition",
-            package={"request_source": request_source, "package": edge},
+            package=edge,
+            request_source=request_source,
         )
         while self.condition_check_result is None:
             await AsyncUtil.sleep(0.1)
-            self._process_edge_condition(edge.id_)
+            self._process_edge_condition(edge.ln_id)
             continue
         check_result = self.condition_check_result
         self.condition_check_result = None
         return check_result
 
-    async def _handle_node_id(self, mail: BaseMail):
+    async def _handle_node_id(self, mail: Mail):
         """
         Processes the node identified by its ID in the mail's package, ensuring it exists and retrieving the next set of
         nodes based on the current node.
 
         Args:
             mail (BaseMail): The mail containing the node ID and related execution details.
 
         Raises:
             ValueError: If the node does not exist within the structure.
         """
-        if mail.package["package"] not in self.internal_nodes:
+        if mail.package.package not in self.internal_nodes:
             raise ValueError(
-                f"Node {mail.package} does not exist in the structure {self.id_}"
+                f"Node {mail.package.package}: Node does not exist in the structure {self.ln_id}"
             )
         return await self._next_node(
-            self.internal_nodes[mail.package["package"]],
-            mail.sender_id,
-            mail.package["request_source"],
+            self.internal_nodes[mail.package.package],
+            mail.sender,
+            mail.package.request_source,
         )
 
-    async def _handle_node(self, mail: BaseMail):
+    async def _handle_node(self, mail: Mail):
         """
         Processes the node specified in the mail's package, ensuring it exists within the structure.
 
         Args:
             mail (BaseMail): The mail containing the node details to be processed.
 
         Raises:
             ValueError: If the node does not exist within the structure.
         """
-        if not self.node_exist(mail.package["package"]):
+        if not self.node_exist(mail.package.package):
             raise ValueError(
-                f"Node {mail.package} does not exist in the structure {self.id_}"
+                f"Node {mail.package.package.ln_id}: does not exist in the structure {self.ln_id}"
             )
         return await self._next_node(
-            mail.package["package"], mail.sender_id, mail.package["request_source"]
+            mail.package.package, mail.sender, mail.package.request_source
         )
 
-    async def _handle_mail(self, mail: BaseMail):
+    async def _handle_mail(self, mail: Mail):
         """
         Processes incoming mail based on its category, initiating node execution or structure operations accordingly.
 
         Args:
             mail (BaseMail): The mail to be processed, containing category and package information.
 
         Raises:
@@ -161,17 +159,17 @@
             self.execute_stop = True
             return None
 
         elif mail.category == "node_id":
             try:
                 return await self._handle_node_id(mail)
             except Exception as e:
-                raise ValueError(f"Error handling node id: {e}") from e
+                raise ValueError(f"Error handling node_id: {e}") from e
 
-        elif mail.category == "node" and isinstance(mail.package["package"], BaseNode):
+        elif mail.category == "node" and isinstance(mail.package.package, Node):
             try:
                 return await self._handle_node(mail)
             except Exception as e:
                 raise ValueError(f"Error handling node: {e}") from e
 
         else:
             raise ValueError(f"Invalid mail type for structure")
@@ -184,70 +182,64 @@
             current_node (Node): The current node.
             executable_id (str): The ID of the executable.
 
         Returns:
             list[Node]: The next step nodes.
         """
         next_nodes = []
-        next_edges = self.get_node_edges(current_node, node_as="out")
+        next_edges = self.get_node_edges(current_node, direction="out")
         for edge in convert.to_list(list(next_edges.values())):
             if edge.bundle:
                 continue
             if edge.condition:
                 check = await self.check_edge_condition(
                     edge, executable_id, request_source
                 )
                 if not check:
                     continue
             node = self.internal_nodes[edge.tail]
-            further_edges = self.get_node_edges(node, node_as="out")
+            further_edges = self.get_node_edges(node, direction="out")
             bundled_nodes = deque()
             for f_edge in convert.to_list(list(further_edges.values())):
                 if f_edge.bundle:
                     bundled_nodes.append(self.internal_nodes[f_edge.tail])
             if bundled_nodes:
                 node = self.parse_bundled_to_action(node, bundled_nodes)
             next_nodes.append(node)
         return next_nodes
 
-    def _send_mail(self, next_nodes: list | None, mail: BaseMail):
+    def _send_mail(self, next_nodes: list | None, mail: Mail):
         """
         Sends mails to the next nodes or signals the end of execution if no next nodes exist.
 
         Args:
             next_nodes (list | None): List of next nodes to process or None if no further nodes are available.
             mail (BaseMail): The base mail used for sending follow-up actions.
         """
         if not next_nodes:  # tail
             self.send(
-                recipient_id=mail.sender_id,
+                recipient=mail.sender,
                 category="end",
-                package={
-                    "request_source": mail.package["request_source"],
-                    "package": "end",
-                },
+                package="end",
+                request_source=mail.package.request_source,
             )
         else:
             if len(next_nodes) == 1:
                 self.send(
-                    recipient_id=mail.sender_id,
+                    recipient=mail.sender,
                     category="node",
-                    package={
-                        "request_source": mail.package["request_source"],
-                        "package": next_nodes[0],
-                    },
+                    package=next_nodes[0],
+                    request_source=mail.package.request_source,
                 )
             else:
                 self.send(
-                    recipient_id=mail.sender_id,
+                    recipient=mail.sender,
                     category="node_list",
-                    package={
-                        "request_source": mail.package["request_source"],
-                        "package": next_nodes,
-                    },
+                    package=next_nodes,
+                    request_source=mail.package.request_source,
                 )
 
     @staticmethod
     def parse_bundled_to_action(instruction: Node, bundled_nodes: deque):
         """
         Constructs an action node from a bundle of nodes, combining various types of nodes like ActionSelection or Tool
         into a single actionable unit.
@@ -267,50 +259,53 @@
         Raises:
             ValueError: If an unrecognized node type is encountered within the bundled nodes. Only `ActionSelection` and
                 `Tool` nodes are valid for bundling into an `ActionNode`.
         """
         action_node = ActionNode(instruction=instruction)
         while bundled_nodes:
             node = bundled_nodes.popleft()
-            if isinstance(node, ActionSelection):
-                action_node.action = node.action
-                action_node.action_kwargs = node.action_kwargs
+            if isinstance(node, DirectiveSelection):
+                action_node.directive = node.directive
+                action_node.directive_kwargs = node.directive_kwargs
             elif isinstance(node, Tool):
                 action_node.tools.append(node)
             else:
                 raise ValueError("Invalid bundles nodes")
         return action_node
 
     async def forward(self) -> None:
         """
         Process the pending incoming mails and perform the corresponding actions.
         """
-        for key in list(self.pending_ins.keys()):
-            while self.pending_ins[key]:
-                mail: BaseMail = self.pending_ins[key].popleft()
+        for key in list(self.mailbox.pending_ins.keys()):
+            while self.mailbox.pending_ins[key].size() > 0:
+                mail_id = self.mailbox.pending_ins[key].popleft()
+                mail = self.mailbox.pile.pop(mail_id)
                 try:
                     if mail.category == "end":
                         self.execute_stop = True
                         return
                     next_nodes = await self._handle_mail(mail)
                     self._send_mail(next_nodes, mail)
                 except Exception as e:
                     raise ValueError(f"Error handling mail: {e}") from e
+            if self.mailbox.pending_ins[key].size() == 0:
+                self.mailbox.pending_ins.pop(key)
 
     async def execute(self, refresh_time=1):
         """
         Executes the forward processing loop, checking conditions and processing nodes at defined intervals.
 
         Args:
             refresh_time (int): The delay between execution cycles, allowing for asynchronous operations to complete.
 
         Raises:
             ValueError: If the graph structure is found to be cyclic, which is unsupported.
         """
-        if not self.acyclic:
+        if not self.is_acyclic():
             raise ValueError("Structure is not acyclic")
 
         while not self.execute_stop:
             await self.forward()
             await AsyncUtil.sleep(refresh_time)
 
     def to_excel(self, structure_name, dir="structure_storage"):
@@ -327,8 +322,9 @@
             dir (str, optional): The directory where the Excel file will be saved. Defaults to "structure_storage".
 
         Raises:
             Exception: Propagates any exceptions raised by the `to_excel` function, which might occur during
                        the file writing process or data formatting.
         """
         from lionagi.integrations.storage.to_excel import to_excel
+
         to_excel(self, structure_name, dir)
```

### Comparing `lionagi-0.1.2/lionagi/core/flow/monoflow/chat_mixin.py` & `lionagi-0.2.0/lionagi/core/report/form.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,253 +1,231 @@
 """
-This module contains mixins for configuring and invoking chatbots.
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
-from abc import ABC
-from typing import Any
+"""
+This module extends the BaseForm class to implement the Form class, which
+dynamically manages form operations based on specific assignments. It provides
+functionalities for initializing fields, filling forms with data, and
+validating the readiness of forms for further processing.
+"""
 
-import re
-from lionagi.libs import nested, func_call, convert, StringMatch, ParseUtil
-from lionagi.core.tool.tool import TOOL_TYPE
-from lionagi.core.messages.schema import Instruction
+from typing import Dict, Any
+from lionagi.libs.ln_convert import to_readable_dict
+from lionagi.core.collections.abc import SYSTEM_FIELDS
+from lionagi.core.report.util import get_input_output_fields
+from lionagi.core.report.base import BaseForm
 
 
-class MonoChatConfigMixin(ABC):
+class Form(BaseForm):
     """
-    Mixin class for configuring chatbots.
+    A specialized implementation of BaseForm designed to manage form fields
+    dynamically based on specified assignments. Supports initialization and
+    management of input and requested fields, handles form filling operations,
+    and ensures forms are properly configured for use.
 
-    Methods:
-        _create_chat_config(self, instruction=None, context=None, sender=None, system=None,
-        output_fields=None, form=None, tools=False, **kwargs) -> Any:
-        Creates a chat configuration based on the provided parameters.
+    Attributes:
+        input_fields (List[str]): Fields required to carry out the objective of the form.
+        requested_fields (List[str]): Fields requested to be filled by the user.
     """
 
-    def _create_chat_config(
-        self,
-        instruction: Instruction | str | dict[str, Any] = None,
-        context: Any | None = None,
-        sender: str | None = None,
-        system: str | dict[str, Any] | None = None,
-        output_fields=None,
-        form=None,
-        tools: TOOL_TYPE = False,
-        **kwargs,
-    ) -> Any:
+    def __init__(self, **kwargs):
         """
-        Creates a chat configuration based on the provided parameters.
+        Initializes a new instance of the Form, setting up input and requested
+        fields based on the form's assignment.
+        """
+        super().__init__(**kwargs)
+        self.input_fields, self.requested_fields = get_input_output_fields(
+            self.assignment
+        )
 
-        Args:
-            instruction (Instruction | str | dict[str, Any]): The instruction for the chatbot (optional).
-            context (Any): The context for the chatbot (optional).
-            sender (str): The sender of the message (optional).
-            system (str | dict[str, Any]): The system message for the chatbot (optional).
-            output_fields: The output fields for the chatbot (optional).
-            form: The prompt template for the chatbot (optional).
-            tools (TOOL_TYPE): The tools for the chatbot (default: False).
-            **kwargs: Additional keyword arguments for the chat configuration.
+        for i in self.input_fields:
+            self.append_to_input(i)
 
-        Returns:
-            Any: The chat configuration.
+        for i in self.input_fields + self.requested_fields:
+            if i not in self._all_fields:
+                self._add_field(i, value=None)
+
+    def append_to_request(self, field: str, value=None):
         """
-        if system:
-            self.branch.change_first_system_message(system)
+        Appends a field to the requested fields.
 
-        if not form:
-            self.branch.add_message(
-                instruction=instruction,
-                context=context,
-                sender=sender,
-                output_fields=output_fields,
-            )
-        else:
-            instruct_ = Instruction.from_form(form)
-            self.branch.add_message(instruction=instruct_)
-
-        if "tool_parsed" in kwargs:
-            kwargs.pop("tool_parsed")
-            tool_kwarg = {"tools": tools}
-            kwargs = tool_kwarg | kwargs
-        elif tools and self.branch.has_tools:
-            kwargs = self.branch.tool_manager.parse_tool(tools=tools, **kwargs)
-
-        config = {**self.branch.llmconfig, **kwargs}
-        if sender is not None:
-            config["sender"] = sender
+        Args:
+            field (str): The name of the field to be requested.
+            value (optional): The value to be assigned to the field. Defaults to None.
+        """
+        if "," in field:
+            field = field.split(",")
+        if not isinstance(field, list):
+            field = [field]
 
-        return config
+        for i in field:
+            i = i.strip()
+            if i not in self._all_fields:
+                self._add_field(i, value=value)
 
+            if i not in self.requested_fields:
+                self.requested_fields.append(i)
+                self.validation_kwargs[i] = self._get_field_attr(
+                    i, "validation_kwargs", {}
+                )
 
-class MonoChatInvokeMixin(ABC):
-    """
-    Mixin class for invoking chatbots.
+    def append_to_input(self, field: str, value=None):
+        """
+        Appends a field to the input fields.
 
-    Methods:
-        async _output(self, invoke, out, output_fields, func_calls_=None, form=None,
-                    return_template=True):
-            Processes the output of the chatbot.
+        Args:
+            field (str): The name of the field to be added to input.
+            value (optional): The value to be assigned to the field. Defaults to None.
+        """
+        if "," in field:
+            field = field.split(",")
+        if not isinstance(field, list):
+            field = [field]
 
-        _return_response(content_, output_fields) -> Any:
-            Returns the response from the chatbot.
+        for i in field:
+            i = i.strip()
+            if i not in self._all_fields:
+                self._add_field(i, value=value)
 
-        async _invoke_tools(self, content_=None, func_calls_=None):
-            Invokes the tools associated with the chatbot.
+            if i not in self.input_fields:
+                self.input_fields.append(i)
+                self.validation_kwargs[i] = self._get_field_attr(
+                    i, "validation_kwargs", {}
+                )
 
-        _process_chatcompletion(self, payload, completion, sender):
-            Processes the chat completion.
+    @property
+    def work_fields(self) -> Dict[str, Any]:
+        """
+        Retrieves a dictionary of the fields relevant to the current task,
+        excluding any SYSTEM_FIELDS and including only the input and requested
+        fields.
 
-        async _call_chatcompletion(self, sender=None, with_sender=False, **kwargs):
-            Calls the chat completion API.
-    """
+        Returns:
+            Dict[str, Any]: The relevant fields for the current task.
+        """
+        dict_ = self.to_dict()
+        return {
+            k: v
+            for k, v in dict_.items()
+            if k not in SYSTEM_FIELDS and k in self.input_fields + self.requested_fields
+        }
 
-    async def _output(
-        self,
-        invoke,
-        out,
-        output_fields,
-        func_calls_=None,
-        form=None,
-        return_template=True,
-    ):
+    def fill(self, form: "Form" = None, strict: bool = True, **kwargs) -> None:
         """
-        Processes the output of the chatbot.
+        Fills the form from another form instance or provided keyword arguments.
+        Raises an error if the form is already filled.
 
         Args:
-            invoke: Flag indicating whether to invoke the tools.
-            out: Flag indicating whether to return the output.
-            output_fields: The output fields for the chatbot.
-            func_calls_: The function calls for invoking the tools (optional).
-            form: The prompt template for the chatbot (optional).
-            return_template (bool): Flag indicating whether to return the prompt template (default: True).
+            form (Form, optional): The form to fill from.
+            strict (bool, optional): Whether to enforce strict filling. Defaults to True.
+            **kwargs: Additional fields to fill.
         """
+        if self.filled:
+            if strict:
+                raise ValueError("Form is filled, cannot be worked on again")
 
-        content_ = self.branch.last_message_content
+        all_fields = self._get_all_fields(form, **kwargs)
 
-        if invoke:
-            try:
-                await self._invoke_tools(content_, func_calls_=func_calls_)
-            except Exception:
-                pass
+        for k, v in all_fields.items():
+            if (
+                k in self.work_fields
+                and v is not None
+                and getattr(self, k, None) is None
+            ):
+                setattr(self, k, v)
 
-        response_ = self._return_response(content_, output_fields)
-
-        if form:
-            form._process_response(response_)
-            return form if return_template else form.outputs
-
-        if out:
-            return response_
-
-    @staticmethod
-    def _return_response(content_, output_fields):
+    def is_workable(self) -> bool:
         """
-        Returns the response from the chatbot.
-
-        Args:
-            content_: The content of the last message.
-            output_fields: The output fields for the chatbot.
+        Determines if the form is ready for processing. Checks if all required
+        fields are filled and raises an error if the form is already filled or
+        if any required field is missing.
 
         Returns:
-            Any: The response from the chatbot.
+            bool: True if the form is workable, otherwise raises ValueError.
         """
-        out_ = ""
+        if self.filled:
+            raise ValueError("Form is already filled, cannot be worked on again")
 
-        if len(content_.items()) == 1 and len(nested.get_flattened_keys(content_)) == 1:
-            key = nested.get_flattened_keys(content_)[0]
-            out_ = content_[key]
-
-        if output_fields:
-            try:
-                return StringMatch.force_validate_dict(
-                    out_, keys=list(output_fields.keys())
-                )
-            except Exception:
-                pass
-
-        if isinstance(out_, str):
-            try:
-                match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
-                if match:
-                    out_ = ParseUtil.fuzzy_parse_json(match.group(1))
-            except Exception:
-                pass
+        for i in self.input_fields:
+            if not getattr(self, i, None):
+                raise ValueError(f"Required field {i} is not provided")
 
-        return out_
+        return True
 
-    async def _invoke_tools(self, content_=None, func_calls_=None):
+    @property
+    def _instruction_context(self) -> str:
         """
-        Invokes the tools associated with the chatbot.
-
-        Args:
-            content_: The content of the last message (optional).
-            func_calls_: The function calls for invoking the tools (optional).
+        Generates a detailed description of the input fields, including their
+        current values and descriptions.
 
         Returns:
-            list: The results of invoking the tools.
+            str: A detailed description of the input fields.
+        """
+        return "".join(
+            f"""
+        ## input: {i}:
+        - description: {getattr(self._all_fields[i], "description", "N/A")}
+        - value: {str(self.__getattribute__(self.input_fields[idx]))}
         """
-        if func_calls_ is None and content_ is not None:
-            tool_uses = content_
-            func_calls_ = func_call.lcall(
-                [convert.to_dict(i) for i in tool_uses["action_request"]],
-                self.branch.tool_manager.get_function_call,
-            )
-
-        outs = await func_call.alcall(func_calls_, self.branch.tool_manager.invoke)
-        outs = convert.to_list(outs, flatten=True)
-
-        a = []
-        for out_, f in zip(outs, func_calls_):
-            res = {
-                "function": f[0],
-                "arguments": f[1],
-                "output": out_,
-            }
-            self.branch.add_message(response=res)
-            a.append(res)
+            for idx, i in enumerate(self.input_fields)
+        )
 
-        return a
+    @property
+    def _instruction_prompt(self) -> str:
+        return f"""
+        ## Task Instructions
+        Please follow prompts to complete the task:
+        1. Your task is: {self.task}
+        2. The provided input fields are: {', '.join(self.input_fields)}
+        3. The requested output fields are: {', '.join(self.requested_fields)}
+        4. Provide your response in the specified JSON format.
+        """
 
-    def _process_chatcompletion(self, payload, completion, sender):
+    @property
+    def _instruction_requested_fields(self) -> Dict[str, str]:
         """
-        Processes the chat completion.
+        Provides a dictionary mapping requested field names to their
+        descriptions.
 
-        Args:
-            payload: The payload for the chat completion.
-            completion: The completed chat response.
-            sender: The sender of the message.
-        """
-        if "choices" in completion:
-            add_msg_config = {"response": completion["choices"][0]}
-            if sender is not None:
-                add_msg_config["sender"] = sender
-
-            self.branch.datalogger.append(input_data=payload, output_data=completion)
-            self.branch.add_message(**add_msg_config)
-            self.branch.status_tracker.num_tasks_succeeded += 1
-        else:
-            self.branch.status_tracker.num_tasks_failed += 1
+        Returns:
+            Dict[str, str]: A dictionary of requested field descriptions.
+        """
+        return {
+            i: getattr(self._all_fields[i], "description", "N/A")
+            for i in self.requested_fields
+        }
 
-    async def _call_chatcompletion(self, sender=None, with_sender=False, **kwargs):
+    def display(self, fields=None):
         """
-        Calls the chat completion API.
+        Displays the form fields using IPython display.
 
         Args:
-            sender: The sender of the message (optional).
-            with_sender (bool): Flag indicating whether to include the sender in the chat messages (default: False).
-            **kwargs: Additional keyword arguments for the chat completion API.
-        """
-        messages = (
-            self.branch.chat_messages_with_sender
-            if with_sender
-            else self.branch.chat_messages
-        )
-        payload, completion = await self.branch.service.serve_chat(
-            messages=messages, **kwargs
-        )
-        self._process_chatcompletion(payload, completion, sender)
+            fields (optional): Specific fields to display. Defaults to None.
+        """
+        from IPython.display import display, Markdown
 
+        fields = fields or self.work_fields
 
-class MonoChatMixin(MonoChatConfigMixin, MonoChatInvokeMixin, ABC):
-    """
-    Mixin class that combines MonoChatConfigMixin and MonoChatInvokeMixin.
-    """
+        if "answer" in fields:
+            answer = fields.pop("answer")
+            fields["answer"] = answer
 
-    pass
+        for k, v in fields.items():
+            if isinstance(v, dict):
+                v = to_readable_dict(v)
+            if len(str(v)) > 50:
+                display(Markdown(f"**{k}**: \n {v}"))
+            else:
+                display(Markdown(f"**{k}**: {v}"))
```

### Comparing `lionagi-0.1.2/lionagi/core/flow/polyflow/chat.py` & `lionagi-0.2.0/lionagi/core/director/direct.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,251 +1,314 @@
 """
-This module contains the PolyChat class for performing parallel chat conversations with multiple branches.
+Copyright 2024 HaiyangLi
 
-The PolyChat class allows for conducting parallel chat conversations with multiple branches, each processing
-instructions and context independently. It provides methods for parallel chat execution and manages the
-created branches within the session.
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
-from typing import Any
+from lionagi.core.unit.unit import Unit
+from lionagi.core.session.branch import Branch
 
-from lionagi.libs import convert, AsyncUtil
-from lionagi.core.messages.schema import Instruction
-from lionagi.core.branch.branch import Branch
-from lionagi.core.flow.baseflow import BasePolyFlow
-
-
-class PolyChat(BasePolyFlow):
-    """
-    A class for performing parallel chat conversations with multiple branches.
-
-    Methods:
-        __init__(self, session: Any) -> None:
-            Initializes the PolyChat instance.
-
-        async parallel_chat(self, instruction: Union[Instruction, str], num_instances: int = 1,
-                             context: Optional[Any] = None, sender: Optional[str] = None,
-                             branch_system: Optional[Any] = None, messages: Optional[Any] = None,
-                             tools: bool = False, out: bool = True, invoke: bool = True,
-                             output_fields: Optional[Any] = None, persist_path: Optional[str] = None,
-                             branch_config: Optional[dict] = None, explode: bool = False, **kwargs) -> Any:
-            Performs parallel chat conversations with multiple branches.
-
-        async _parallel_chat(self, instruction: Union[Instruction, str], num_instances: int = 1,
-                              context: Optional[Any] = None, sender: Optional[str] = None,
-                              messages: Optional[Any] = None, tools: bool = False, out: bool = True,
-                              invoke: bool = True, output_fields: Optional[Any] = None,
-                              persist_path: Optional[str] = None, branch_config: dict = {},
-                              explode: bool = False, include_mapping: bool = True, default_key: str = "response",
-                              **kwargs) -> Any:
-            Internal method for performing parallel chat conversations with multiple branches.
-    """
-
-    def __init__(self, session) -> None:
-        """
-        Initializes the PolyChat instance.
-
-        Args:
-            session: The session object.
-        """
-        super().__init__(session)
-
-    async def parallel_chat(
-        self,
-        instruction: Instruction | str,
-        num_instances=1,
-        context=None,
-        sender=None,
-        branch_system=None,
-        messages=None,
-        tools=False,
-        out=True,
-        invoke: bool = True,
-        output_fields=None,
-        persist_path=None,
-        branch_config=None,
-        explode=False,
-        **kwargs,
-    ) -> Any:
-        """
-        Performs parallel chat conversations with multiple branches.
-
-        Args:
-            instruction (Instruction | str): The instruction for the chat conversation.
-            num_instances (int): The number of branch instances to create (default: 1).
-            context (Optional[Any]): Additional context for the chat conversation.
-            sender (Optional[str]): The sender of the chat message.
-            branch_system (Optional[Any]): The system configuration for the branches.
-            messages (Optional[Any]): Messages to initialize the branches with.
-            tools (bool): Flag indicating whether to use tools in the chat conversation (default: False).
-            out (bool): Flag indicating whether to return the output of the chat conversation (default: True).
-            invoke (bool): Flag indicating whether to invoke tools during the chat conversation (default: True).
-            output_fields (Optional[Any]): The output fields for the chat conversation.
-            persist_path (Optional[str]): The path to persist the branch data.
-            branch_config (Optional[dict]): Additional configuration for the branches.
-            explode (bool): Flag indicating whether to explode the instruction and context combinations (default: False).
-            **kwargs: Additional keyword arguments for the chat conversation.
-
-        Returns:
-            Any: The result of the parallel chat conversation.
-        """
-        if branch_config is None:
-            branch_config = {}
-        return await self._parallel_chat(
-            instruction,
-            num_instances=num_instances,
-            context=context,
-            sender=sender,
-            branch_system=branch_system,
-            messages=messages,
-            tools=tools,
-            out=out,
-            invoke=invoke,
-            output_fields=output_fields,
-            persist_path=persist_path,
-            branch_config=branch_config,
-            explode=explode,
-            **kwargs,
-        )
-
-    async def _parallel_chat(
-        self,
-        instruction: Instruction | str,
-        num_instances=1,
-        context=None,
-        sender=None,
-        messages=None,
-        tools=False,
-        out=True,
-        invoke: bool = True,
-        output_fields=None,
-        persist_path=None,
-        branch_config={},
-        explode=False,
-        include_mapping=True,
-        default_key="response",
-        **kwargs,
-    ) -> Any:
-        """
-        Internal method for performing parallel chat conversations with multiple branches.
-
-        Args:
-            instruction (Instruction | str): The instruction for the chat conversation.
-            num_instances (int): The number of branch instances to create (default: 1).
-            context (Optional[Any]): Additional context for the chat conversation.
-            sender (Optional[str]): The sender of the chat message.
-            messages (Optional[Any]): Messages to initialize the branches with.
-            tools (bool): Flag indicating whether to use tools in the chat conversation (default: False).
-            out (bool): Flag indicating whether to return the output of the chat conversation (default: True).
-            invoke (bool): Flag indicating whether to invoke tools during the chat conversation (default: True).
-            output_fields (Optional[Any]): The output fields for the chat conversation.
-            persist_path (Optional[str]): The path to persist the branch data.
-            branch_config (dict): Additional configuration for the branches (default: {}).
-            explode (bool): Flag indicating whether to explode the instruction and context combinations (default: False).
-            include_mapping (bool): Flag indicating whether to include mapping information in the output (default: True).
-            default_key (str): The default key for the output mapping (default: "response").
-            **kwargs: Additional keyword arguments for the chat conversation.
-
-        Returns:
-            Any: The result of the parallel chat conversation.
-        """
-
-        branches = {}
-
-        async def _inner(i, ins_, cxt_):
-
-            branch_ = Branch(
-                messages=messages,
-                service=self.session.default_branch.service,
-                llmconfig=self.session.default_branch.llmconfig,
-                persist_path=persist_path,
-                **branch_config,
-            )
-
-            branch_.branch_name = branch_.id_
-
-            if tools:
-                branch_.tool_manager = self.session.default_branch.tool_manager
-
-            res_ = await branch_.chat(
-                instruction=ins_ or instruction,
-                context=cxt_ or context,
-                sender=sender,
-                tools=tools,
-                invoke=invoke,
-                out=out,
-                output_fields=output_fields,
-                **kwargs,
-            )
-
-            branches[branch_.id_] = branch_
-            if include_mapping:
-                return {
-                    "instruction": ins_ or instruction,
-                    "context": cxt_ or context,
-                    "branch_id": branch_.id_,
-                    default_key: res_,
-                }
-
-            else:
-                return res_
-
-        async def _inner_2(i, ins_=None, cxt_=None):
-            """returns num_instances of branches performing for same task/context"""
-            tasks = [_inner(i, ins_, cxt_) for _ in range(num_instances)]
-            ress = await AsyncUtil.execute_tasks(*tasks)
-            return convert.to_list(ress)
-
-        async def _inner_3(i):
-            """different instructions but same context"""
-            tasks = [_inner_2(i, ins_=ins_) for ins_ in convert.to_list(instruction)]
-            ress = await AsyncUtil.execute_tasks(*tasks)
-            return convert.to_list(ress)
-
-        async def _inner_3_b(i):
-            """different context but same instruction"""
-            tasks = [_inner_2(i, cxt_=cxt_) for cxt_ in convert.to_list(context)]
-            ress = await AsyncUtil.execute_tasks(*tasks)
-            return convert.to_list(ress)
-
-        async def _inner_4(i):
-            """different instructions and different context"""
-
-            tasks = []
-            if explode:
-                tasks = [
-                    _inner_2(i, ins_=ins_, cxt_=cxt_)
-                    for ins_ in convert.to_list(instruction)
-                    for cxt_ in convert.to_list(context)
-                ]
-            else:
-                tasks = [
-                    _inner_2(i, ins_=ins_, cxt_=cxt_)
-                    for ins_, cxt_ in zip(
-                        convert.to_list(instruction), convert.to_list(context)
-                    )
-                ]
-
-            ress = await AsyncUtil.execute_tasks(*tasks)
-            return convert.to_list(ress)
-
-        if len(convert.to_list(instruction)) == 1:
-            if len(convert.to_list(context)) == 1:
-                out_ = await _inner_2(0)
-                self.session.branches.update(branches)
-                return out_
-
-            elif len(convert.to_list(context)) > 1:
-                out_ = await _inner_3_b(0)
-                self.session.branches.update(branches)
-                return out_
-
-        elif len(convert.to_list(instruction)) > 1:
-            if len(convert.to_list(context)) == 1:
-                out_ = await _inner_3(0)
-                self.session.branches.update(branches)
-                return out_
-
-            elif len(convert.to_list(context)) > 1:
-                out_ = await _inner_4(0)
-                self.session.branches.update(branches)
-                return out_
+
+async def chat(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    **kwargs,
+):
+    """
+    Performs a chat operation using the specified parameters.
+
+    Args:
+        instruction (str, optional): The instruction for the chat.
+        context (Any, optional): The context to perform the instruction on.
+        system (Any, optional): The system context for the chat.
+        sender (str, optional): The sender of the instruction.
+        recipient (str, optional): The recipient of the instruction.
+        branch (Branch, optional): The branch to use for the chat.
+        form (Any, optional): The form to create instruction from.
+        confidence_score (float, optional): The confidence score for the operation.
+        reason (bool, optional): Whether to include a reason for the operation.
+        **kwargs: Additional keyword arguments for the chat operation.
+
+    Returns:
+        Any: The result of the chat operation.
+    """
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.chat(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        branch=branch,
+        **kwargs,
+    )
+
+
+async def select(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    choices=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    **kwargs,
+):
+    """
+    Performs a select operation using the specified parameters.
+
+    Args:
+        instruction (str, optional): The instruction for the selection.
+        context (Any, optional): The context to perform the instruction on.
+        system (Any, optional): The system context for the selection.
+        sender (str, optional): The sender of the instruction.
+        recipient (str, optional): The recipient of the instruction.
+        choices (list, optional): The choices for the selection.
+        branch (Branch, optional): The branch to use for the selection.
+        form (Any, optional): The form to create instruction from.
+        confidence_score (float, optional): The confidence score for the operation.
+        reason (bool, optional): Whether to include a reason for the operation.
+        **kwargs: Additional keyword arguments for the selection operation.
+
+    Returns:
+        Any: The result of the selection operation.
+    """
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.select(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        choices=choices,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        **kwargs,
+    )
+
+
+async def predict(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    num_sentences=1,
+    **kwargs,
+):
+    """
+    Performs a predict operation using the specified parameters.
+
+    Args:
+        instruction (str, optional): The instruction for the prediction.
+        context (Any, optional): The context to perform the instruction on.
+        system (Any, optional): The system context for the prediction.
+        sender (str, optional): The sender of the instruction.
+        recipient (str, optional): The recipient of the instruction.
+        branch (Branch, optional): The branch to use for the prediction.
+        form (Any, optional): The form to create instruction from.
+        confidence_score (float, optional): The confidence score for the operation.
+        reason (bool, optional): Whether to include a reason for the operation.
+        **kwargs: Additional keyword arguments for the prediction operation.
+
+    Returns:
+        Any: The result of the prediction operation.
+    """
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.predict(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        num_sentences=num_sentences,
+        **kwargs,
+    )
+
+
+async def act(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    **kwargs,
+):
+    """
+    Performs an act operation using the specified parameters.
+
+    Args:
+        instruction (str, optional): The instruction for the action.
+        context (Any, optional): The context to perform the instruction on.
+        system (Any, optional): The system context for the action.
+        sender (str, optional): The sender of the instruction.
+        recipient (str, optional): The recipient of the instruction.
+        branch (Branch, optional): The branch to use for the action.
+        form (Any, optional): The form to create instruction from.
+        confidence_score (float, optional): The confidence score for the operation.
+        reason (bool, optional): Whether to include a reason for the operation.
+        **kwargs: Additional keyword arguments for the act operation.
+
+    Returns:
+        Any: The result of the act operation.
+    """
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.act(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        **kwargs,
+    )
+
+
+async def score(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    score_range=None,
+    include_endpoints=None,
+    num_digit=None,
+    **kwargs,
+):
+    """
+    Asynchronously performs a scoring task within a given context.
+
+    Args:
+        instruction (str, optional): Additional instruction for the scoring task.
+        context (Any, optional): Context to perform the scoring task on.
+        system (str, optional): System message to use for the scoring task.
+        sender (str, optional): Sender of the instruction. Defaults to None.
+        recipient (str, optional): Recipient of the instruction. Defaults to None.
+        branch (Branch, optional): Branch to perform the task within. Defaults to a new Branch.
+        form (Form, optional): Form to create the instruction from. Defaults to None.
+        confidence_score (bool, optional): Flag to include a confidence score. Defaults to None.
+        reason (bool, optional): Flag to include a reason for the scoring. Defaults to False.
+        score_range (tuple, optional): Range for the score. Defaults to None.
+        include_endpoints (bool, optional): Flag to include endpoints in the score range. Defaults to None.
+        num_digit (int, optional): Number of decimal places for the score. Defaults to None.
+        **kwargs: Additional keyword arguments for further customization.
+
+    Returns:
+        Any: The result of the scoring task.
+    """
+
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.score(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        score_range=score_range,
+        include_endpoints=include_endpoints,
+        num_digit=num_digit,
+        **kwargs,
+    )
+
+
+async def plan(
+    instruction=None,
+    context=None,
+    system=None,
+    sender=None,
+    recipient=None,
+    branch=None,
+    form=None,
+    confidence_score=None,
+    reason=False,
+    num_step=3,
+    **kwargs,
+):
+    """
+    Asynchronously generates a step-by-step plan within a given context.
+
+    Args:
+        instruction (str, optional): Additional instruction for the planning task.
+        context (Any, optional): Context to perform the planning task on.
+        system (str, optional): System message to use for the planning task.
+        sender (str, optional): Sender of the instruction. Defaults to None.
+        recipient (str, optional): Recipient of the instruction. Defaults to None.
+        branch (Branch, optional): Branch to perform the task within. Defaults to a new Branch.
+        form (Form, optional): Form to create the instruction from. Defaults to None.
+        confidence_score (bool, optional): Flag to include a confidence score. Defaults to None.
+        reason (bool, optional): Flag to include a reason for the plan. Defaults to False.
+        num_step (int, optional): Number of steps in the plan. Defaults to 3.
+        **kwargs: Additional keyword arguments for further customization.
+
+    Returns:
+        Any: The result of the planning task.
+    """
+
+    branch = branch or Branch()
+    unit = Unit(branch)
+
+    return await unit.plan(
+        instruction=instruction,
+        context=context,
+        system=system,
+        sender=sender,
+        recipient=recipient,
+        form=form,
+        confidence_score=confidence_score,
+        reason=reason,
+        num_step=num_step,
+        **kwargs,
+    )
```

### Comparing `lionagi-0.1.2/lionagi/core/form/field_validator.py` & `lionagi-0.2.0/lionagi/libs/ln_validate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,51 @@
 """
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+"""
 This module provides functions for validating and fixing field values based on their data types.
 
 The module defines several functions for checking and fixing field values of different data types,
 including numeric, boolean, string, and enum. It also provides a dictionary `validation_funcs` that
 maps data types to their corresponding validation functions.
 """
 
-from lionagi.libs import convert, StringMatch, ParseUtil
+from .ln_convert import to_str, is_same_dtype, to_list, to_dict, to_num, strip_lower
+from .ln_parse import StringMatch, ParseUtil
 
 
 def check_dict_field(x, keys: list[str] | dict, fix_=True, **kwargs):
     if isinstance(x, dict):
         return x
     if fix_:
         try:
-            x = convert.to_str(x)
+            x = to_str(x)
             return StringMatch.force_validate_dict(x, keys=keys, **kwargs)
         except Exception as e:
             raise ValueError("Invalid dict field type.") from e
     raise ValueError(f"Default value for DICT must be a dict, got {type(x).__name__}")
 
 
 def check_action_field(x, fix_=True, **kwargs):
     if (
         isinstance(x, list)
-        and convert.is_same_dtype(x, dict)
+        and is_same_dtype(x, dict)
         and all(_has_action_keys(y) for y in x)
     ):
         return x
     try:
         x = _fix_action_field(x, fix_)
         return x
     except Exception as e:
@@ -131,15 +148,15 @@
 
     Returns:
         The original value if it's valid, or the fixed value if `fix_` is True.
 
     Raises:
         ValueError: If the value is not a valid enum field and cannot be fixed.
     """
-    same_dtype, dtype_ = convert.is_same_dtype(choices, return_dtype=True)
+    same_dtype, dtype_ = is_same_dtype(choices, return_dtype=True)
     if not same_dtype:
         raise ValueError(
             f"Field type ENUM requires all choices to be of the same type, got {choices}"
         )
 
     if not isinstance(x, dtype_):
         raise ValueError(
@@ -165,18 +182,18 @@
 
 def _fix_action_field(x, discard_=True):
     corrected = []
     if isinstance(x, str):
         x = ParseUtil.fuzzy_parse_json(x)
 
     try:
-        x = convert.to_list(x)
+        x = to_list(x)
 
         for i in x:
-            i = convert.to_dict(i)
+            i = to_dict(i)
             if _has_action_keys(i):
                 corrected.append(i)
             elif not discard_:
                 raise ValueError(f"Invalid action field: {i}")
     except Exception as e:
         raise ValueError(f"Invalid action field: {e}") from e
 
@@ -195,15 +212,15 @@
     Returns:
         The fixed numeric value.
 
     Raises:
         ValueError: If the value cannot be converted into a valid numeric value.
     """
     try:
-        x = convert.to_num(x, *args, **kwargs)
+        x = to_num(x, *args, **kwargs)
         if isinstance(x, (int, float)):
             return x
         raise ValueError(f"Failed to convert {x} into a numeric value")
     except Exception as e:
         raise ValueError(f"Failed to convert {x} into a numeric value") from e
 
 
@@ -217,15 +234,15 @@
     Returns:
         The fixed boolean value.
 
     Raises:
         ValueError: If the value cannot be converted into a valid boolean value.
     """
     try:
-        x = convert.strip_lower(convert.to_str(x))
+        x = strip_lower(to_str(x))
         if x in ["true", "1", "correct", "yes"]:
             return True
 
         elif x in ["false", "0", "incorrect", "no", "none", "n/a"]:
             return False
 
         raise ValueError(f"Failed to convert {x} into a boolean value")
@@ -243,15 +260,15 @@
     Returns:
         The fixed string value.
 
     Raises:
         ValueError: If the value cannot be converted into a valid string value.
     """
     try:
-        x = convert.to_str(x)
+        x = to_str(x)
         if isinstance(x, str):
             return x
         raise ValueError(f"Failed to convert {x} into a string value")
     except Exception as e:
         raise ValueError(f"Failed to convert {x} into a string value") from e
 
 
@@ -267,15 +284,15 @@
     Returns:
         The fixed enum value.
 
     Raises:
         ValueError: If the value cannot be converted into a valid enum value.
     """
     try:
-        x = convert.to_str(x)
+        x = to_str(x)
         return StringMatch.choose_most_similar(x, choices, **kwargs)
     except Exception as e:
         raise ValueError(f"Failed to convert {x} into one of the choices") from e
 
 
 validation_funcs = {
     "number": check_number_field,
```

### Comparing `lionagi-0.1.2/lionagi/core/generic/data_logger.py` & `lionagi-0.2.0/lionagi/core/collections/_logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import atexit
 import contextlib
 import logging
 from collections import deque
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List
@@ -10,32 +26,31 @@
 
 
 # TODO: there should be a global data logger, under setting
 
 
 @dataclass
 class DLog:
-    """
-    Defines a log entry structure for data processing operations.
+    """Defines a log entry structure for data processing operations.
 
-    This class encapsulates both the input to and output from a data processing operation,
-    along with an automatically generated timestamp indicating when the log entry was
-    created. It aims to standardize logging across applications for easier analysis
-    and debugging.
+    This class encapsulates both the input to and output from a data processing
+    operation, along with an automatically generated timestamp indicating when
+    the log entry was created. It aims to standardize logging across applications
+    for easier analysis and debugging.
 
     Attributes:
         input_data: The data input to the operation. Can be of any type.
         output_data: The data output by the operation. Can be of any type.
     """
 
     input_data: Any
     output_data: Any
 
     def serialize(self, *, flatten_: bool = True, sep: str = "[^_^]") -> dict[str, Any]:
-        """Serializes the DLog instance into a dictionary with an added timestamp.
+        """Serialize the DLog instance into a dictionary with an added timestamp.
 
         Args:
             flatten_ (bool): If True, flattens dictionary inputs for serialization.
             sep (str): Separator used in flattening nested dictionaries.
 
         Returns:
             A dictionary representation of the DLog instance, including 'input_data',
@@ -44,22 +59,20 @@
         log_dict = {}
 
         def _process_data(data, field):
             try:
                 data = convert.to_str(data)
                 if "{" not in data:
                     log_dict[field] = convert.to_str(data)
-
                 else:
                     with contextlib.suppress(Exception):
                         data = convert.to_dict(data)
 
                     if isinstance(self.input_data, dict) and flatten_:
                         log_dict[field] = convert.to_str(nested.flatten(data, sep=sep))
-
                     else:
                         log_dict[field] = convert.to_str(data)
 
             except Exception as e:
                 log_dict[field] = data
                 logging.error(f"Error in processing {field} to str: {e}")
 
@@ -75,93 +88,91 @@
         cls,
         *,
         input_str: str,
         output_str: str,
         unflatten_: bool = True,
         sep: str = "[^_^]",
     ) -> "DLog":
-        """Deserializes log entries from string representations of input and output data.
+        """Deserialize log entries from string representations.
 
-        This method reconstructs a DLog instance from serialized string data, optionally
-        unflattening nested dictionary structures if they were flattened during the
-        serialization process. The method is particularly useful for reading logs from
-        storage formats like JSON or CSV where data is represented as strings.
+        This method reconstructs a DLog instance from serialized string data,
+        optionally unflattening nested dictionary structures if they were
+        flattened during the serialization process. The method is particularly
+        useful for reading logs from storage formats like JSON or CSV where
+        data is represented as strings.
 
         Note:
-            The separator '[^_^]' is reserved and should not be used within dictionary
-            keys to ensure proper structure preservation during unflattening.
+            The separator '[^_^]' is reserved and should not be used within
+            dictionary keys to ensure proper structure preservation during
+            unflattening.
 
         Args:
             input_str: String representation of the input data.
             output_str: String representation of the output data.
-            unflatten_ (bool): Indicates whether to unflatten the string data back into
-                               nested dictionaries.
+            unflatten_ (bool): Indicates whether to unflatten the string data
+                               back into nested dictionaries.
             sep (str): Separator used if unflattening is performed.
 
         Returns:
             An instance of DLog reconstructed from the provided string data.
 
         Raises:
-            ValueError: If deserialization or unflattening fails due to incorrect data
-                        format or separator issues.
+            ValueError: If deserialization or unflattening fails due to incorrect
+                        data format or separator issues.
         """
 
         def _process_data(data):
             if unflatten_:
                 try:
                     return nested.unflatten(convert.to_dict(data), sep=sep)
-                except:
+                except Exception:
                     return data
             else:
                 return data
 
         input_data = _process_data(input_str)
         output_data = _process_data(output_str)
 
         return cls(input_data=input_data, output_data=output_data)
 
 
 class DataLogger:
-    """
-    Manages logging for data processing activities within an application.
+    """Manages logging for data processing activities within an application.
 
-    This class handles the accumulation,
-    structuring, and persistence of log entries.
-    It supports exporting logs to disk in both CSV and JSON formats,
-    with features for
+    This class handles the accumulation, structuring, and persistence of log entries.
+    It supports exporting logs to disk in both CSV and JSON formats, with features for
     automatic log saving at program exit and customizable file naming.
 
     Attributes:
         persist_path: Path to the directory for saving log files.
         log: Container for log entries.
         filename: Base name for log files.
     """
 
     def __init__(
         self,
         persist_path: str | Path | None = None,
         log: List[Dict] | None = None,
         filename: str | None = None,
     ) -> None:
-        """
-        Initializes the DataLogger with optional custom settings for log storage.
+        """Initialize the DataLogger with optional custom settings for log storage.
 
         Args:
-            persist_path: The file system path for storing log files. Defaults to 'data/logs/'.
+            persist_path: The file system path for storing log files.
+                          Defaults to 'data/logs/'.
             log: Initial log entries.
             filename: Base name for exported log files.
         """
         self.persist_path = Path(persist_path) if persist_path else Path("data/logs/")
         self.log = deque(log) if log else deque()
         self.filename = filename or "log"
         atexit.register(self.save_at_exit)
 
     def extend(self, logs) -> None:
-        """
-        Extends the log deque with multiple log entries.
+        """Extend the log deque with multiple log entries.
 
         This method allows for bulk addition of log entries, which can be useful for
         importing logs from external sources or consolidating logs from different parts
         of an application.
 
         Args:
             logs: A list of log entries, each as a dictionary conforming to the log
@@ -169,16 +180,15 @@
         """
         if len(logs) > 0:
             log1 = convert.to_list(self.log)
             log1.extend(convert.to_list(logs))
             self.log = deque(log1)
 
     def append(self, *, input_data: Any, output_data: Any) -> None:
-        """
-        Appends a new log entry from provided input and output data.
+        """Append a new log entry from provided input and output data.
 
         Args:
             input_data: Input data to the operation.
             output_data: Output data from the operation.
         """
         log_entry = DLog(input_data=input_data, output_data=output_data)
         self.log.append(log_entry)
@@ -188,35 +198,35 @@
         filename: str = "log.csv",
         *,
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
-        flatten_=True,
-        sep="[^_^]",
-        index=False,
-        random_hash_digits=3,
+        flatten_: bool = True,
+        sep: str = "[^_^]",
+        index: bool = False,
+        random_hash_digits: int = 3,
         **kwargs,
     ) -> None:
-        """Exports log entries to a CSV file with customizable options.
+        """Export log entries to a CSV file with customizable options.
 
         Args:
             filename: Filename for the exported CSV. Defaults to 'log.csv'.
             dir_exist_ok: If True, allows writing to an existing directory.
             timestamp: If True, appends a timestamp to the filename.
             time_prefix: If True, places the timestamp prefix before the filename.
             verbose: If True, prints a message upon successful save.
             clear: If True, clears the log deque after saving.
             flatten_: If True, flattens dictionary data for serialization.
             sep: Separator for flattening nested dictionaries.
             index: If True, includes an index column in the CSV.
+            random_hash_digits: Number of random hash digits to add to the filename.
             **kwargs: Additional arguments for DataFrame.to_csv().
         """
-
         if not filename.endswith(".csv"):
             filename += ".csv"
 
         filepath = SysUtil.create_path(
             self.persist_path,
             filename,
             timestamp=timestamp,
@@ -240,32 +250,33 @@
         filename: str = "log.json",
         *,
         dir_exist_ok: bool = True,
         timestamp: bool = True,
         time_prefix: bool = False,
         verbose: bool = True,
         clear: bool = True,
-        flatten_=True,
-        sep="[^_^]",
-        index=False,
-        random_hash_digits=3,
+        flatten_: bool = True,
+        sep: str = "[^_^]",
+        index: bool = False,
+        random_hash_digits: int = 3,
         **kwargs,
     ) -> None:
-        """Exports log entries to a JSON file with customizable options.
+        """Export log entries to a JSON file with customizable options.
 
         Args:
             filename: Filename for the exported JSON. Defaults to 'log.json'.
             dir_exist_ok: If True, allows writing to an existing directory.
             timestamp: If True, appends a timestamp to the filename.
             time_prefix: If True, places the timestamp prefix before the filename.
             verbose: If True, prints a message upon successful save.
             clear: If True, clears the log deque after saving.
             flatten_: If True, flattens dictionary data for serialization.
             sep: Separator for flattening nested dictionaries.
             index: If True, includes an index in the JSON.
+            random_hash_digits: Number of random hash digits to add to the filename.
             **kwargs: Additional arguments for DataFrame.to_json().
         """
         if not filename.endswith(".json"):
             filename += ".json"
 
         filepath = SysUtil.create_path(
             self.persist_path,
@@ -281,25 +292,28 @@
             df = convert.to_df(convert.to_list(logs, flatten=True))
             df.to_json(filepath, index=index, **kwargs)
             if verbose:
                 print(f"{len(self.log)} logs saved to {filepath}")
             if clear:
                 self.log.clear()
         except Exception as e:
-            raise ValueError(f"Error in saving to csv: {e}") from e
+            raise ValueError(f"Error in saving to json: {e}") from e
 
     def save_at_exit(self):
-        """
-        Registers an at-exit handler to ensure that any unsaved logs are automatically
-        persisted to a file upon program termination. This safeguard helps prevent the
-        loss of log data due to unexpected shutdowns or program exits.
+        """Save any unsaved logs automatically upon program termination.
+
+        This method is registered as an at-exit handler to ensure that any unsaved
+        logs are automatically persisted to a file upon program termination. This
+        safeguard helps prevent the loss of log data due to unexpected shutdowns
+        or program exits.
 
         The method is configured to save the logs to a CSV file, named
-        'unsaved_logs.csv', which is stored in the designated persisting directory. This
-        automatic save operation is triggered only if there are unsaved logs present at
-        the time of program exit.
+        'unsaved_logs.csv', which is stored in the designated persisting directory.
+        This automatic save operation is triggered only if there are unsaved logs
+        present at the time of program exit.
 
-        Note: This method does not clear the logs after saving, allowing for the
-        possibility of manual.py review or recovery after the program has terminated.
+        Note:
+            This method does not clear the logs after saving, allowing for the
+            possibility of manual review or recovery after the program has terminated.
         """
         if self.log:
             self.to_csv_file("unsaved_logs.csv", clear=False)
```

### Comparing `lionagi-0.1.2/lionagi/core/generic/node.py` & `lionagi-0.2.0/lionagi/core/generic/node.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,285 +1,220 @@
-from typing import Any, Type
+"""
+This module defines the Node class, representing a node in a graph-like
+structure within LionAGI. Nodes can form relationships with other nodes
+through directed edges, enabling construction and manipulation of complex
+relational networks.
+
+Includes functionality for managing relationships, such as adding,
+modifying, and removing edges, and querying related nodes and connections.
+"""
+
 from pydantic import Field
-from lionagi.integrations.bridge import LlamaIndexBridge, LangchainBridge
+from pandas import Series
+
+from lionagi.libs.ln_convert import to_list
 
-from lionagi.core.generic.component import BaseNode
-from lionagi.core.generic.condition import Condition
+from lionagi.core.collections.abc import (
+    Component,
+    Condition,
+    Relatable,
+    RelationError,
+    get_lion_id,
+)
+from lionagi.core.collections import pile, Pile
 from lionagi.core.generic.edge import Edge
-from lionagi.core.generic.relation import Relations
-from lionagi.core.generic.mailbox import MailBox
 
 
-class Node(BaseNode):
+class Node(Component, Relatable):
     """
-    Represents a node with relations to other nodes.
-
-    Attributes:
-        relations (Relations): The relations of the node, managed through a
-            `Relations` instance.
+    Node in a graph structure, can connect to other nodes via edges.
 
-    Properties:
-        related_nodes: A set of IDs representing nodes related to this node.
-        edges: A dictionary of all edges connected to this node.
-        node_relations: A dictionary categorizing preceding and succeeding
-            relations to this node.
-        precedessors: A list of node IDs that precede this node.
-        successors: A list of node IDs that succeed this node.
-
-    Methods:
-        relate(node, self_as, condition, **kwargs): Relates this node to
-            another node with an edge.
-        unrelate(node, edge): Removes one or all relations between this node
-            and another.
-        to_llama_index(node_type, **kwargs): Serializes this node for
-            LlamaIndex.
-        to_langchain(**kwargs): Serializes this node for Langchain.
-        from_llama_index(llama_node, **kwargs): Deserializes a node from
-            LlamaIndex data.
-        from_langchain(lc_doc): Deserializes a node from Langchain data.
-        __str__(): String representation of the node.
+    Extends `Component` by incorporating relational capabilities, allowing
+    nodes to connect through 'in' and 'out' directed edges, representing
+    incoming and outgoing relationships.
 
-    Raises:
-        ValueError: When invalid parameters are provided to methods.
+    Attributes:
+        relations (dict[str, Pile]): Dictionary holding 'Pile' instances
+            for incoming ('in') and outgoing ('out') edges.
     """
 
-    relations: Relations = Field(
-        default_factory=Relations,
+    relations: dict[str, Pile] = Field(
+        default_factory=lambda: {"in": pile(), "out": pile()},
         description="The relations of the node.",
-        alias="node_relations",
     )
 
-    mailbox: MailBox = Field(
-        default_factory=MailBox,
-        description="The mailbox for incoming and outgoing mails.",
-    )
+    @property
+    def edges(self) -> Pile[Edge]:
+        """
+        Get unified view of all incoming and outgoing edges.
+
+        Returns:
+            Combined pile of all edges connected to this node.
+        """
+        return self.relations["in"] + self.relations["out"]
 
     @property
     def related_nodes(self) -> list[str]:
-        """Returns a set of node IDs related to this node, excluding itself."""
-        nodes = set(self.relations.all_nodes)
-        nodes.discard(self.id_)
-        return list(nodes)
+        """
+        Get list of all unique node IDs directly related to this node.
 
-    @property
-    def edges(self) -> dict[str, Edge]:
-        """Returns a dictionary of all edges connected to this node."""
-        return self.relations.all_edges
+        Returns:
+            List of node IDs related to this node.
+        """
+        all_nodes = set(
+            to_list([[i.head, i.tail] for i in self.edges], flatten=True, dropna=True)
+        )
+        all_nodes.discard(self.ln_id)
+        return list(all_nodes)
 
     @property
     def node_relations(self) -> dict:
-        """Categorizes preceding and succeeding relations to this node."""
+        """
+        Get categorized view of direct relationships into groups.
 
-        points_to_nodes = {}
-        for edge in self.relations.points_to.values():
-            for i in self.related_nodes:
-                if edge.tail == i:
-                    if i in points_to_nodes:
-                        points_to_nodes[i].append(edge)
-                    else:
-                        points_to_nodes[i] = [edge]
-
-        pointed_by_nodes = {}
-        for edge in self.relations.pointed_by.values():
-            for i in self.related_nodes:
-                if edge.head == i:
-                    if i in pointed_by_nodes:
-                        pointed_by_nodes[i].append(edge)
-                    else:
-                        pointed_by_nodes[i] = [edge]
+        Returns:
+            Dict with keys 'in' and 'out', each containing a mapping of
+            related node IDs to lists of edges representing relationships.
+        """
+        out_node_edges = {}
+        if not self.relations["out"].is_empty():
+            for edge in self.relations["out"]:
+                for node_id in self.related_nodes:
+                    if edge.tail == node_id:
+                        out_node_edges.setdefault(node_id, []).append(edge)
+
+        in_node_edges = {}
+        if not self.relations["in"].is_empty():
+            for edge in self.relations["in"]:
+                for node_id in self.related_nodes:
+                    if edge.head == node_id:
+                        in_node_edges.setdefault(node_id, []).append(edge)
 
-        return {"points_to": points_to_nodes, "pointed_by": pointed_by_nodes}
+        return {"out": out_node_edges, "in": in_node_edges}
 
     @property
-    def precedessors(self) -> list[str]:
-        """return a list of nodes id that precede this node"""
-        return [k for k, v in self.node_relations["pointed_by"].items() if len(v) > 0]
+    def predecessors(self) -> list[str]:
+        """
+        Get list of IDs of nodes with direct incoming relation to this.
+
+        Returns:
+            List of node IDs that precede this node.
+        """
+        return [
+            node_id for node_id, edges in self.node_relations["in"].items() if edges
+        ]
 
     @property
     def successors(self) -> list[str]:
-        """return a list of nodes id that succeed this node"""
-        return [k for k, v in self.node_relations["points_to"].items() if len(v) > 0]
+        """
+        Get list of IDs of nodes with direct outgoing relation from this.
+
+        Returns:
+            List of node IDs that succeed this node.
+        """
+        return [
+            node_id for node_id, edges in self.node_relations["out"].items() if edges
+        ]
 
     def relate(
         self,
         node: "Node",
-        node_as: str = "head",
+        direction: str = "out",
         condition: Condition | None = None,
         label: str | None = None,
-        bundle=False,
+        bundle: bool = False,
     ) -> None:
-        """Relates this node to another node with an edge.
+        """
+        Establish directed relationship from this node to another.
 
         Args:
-            node (Node): The node to relate to.
-            self_as (str): Specifies whether this node is the 'head' or 'tail'
-                of the relation. Defaults to "head".
-            condition (Condition | None): The condition associated with the
-                edge, if any. Defaults to None.
-            **kwargs: Additional keyword arguments for edge creation.
+            node: Target node to relate to.
+            direction: Direction of edge ('in' or 'out'). Default 'out'.
+            condition: Optional condition to associate with edge.
+            label: Optional label for edge.
+            bundle: Whether to bundle edge with others. Default False.
 
         Raises:
-            ValueError: If `self_as` is not 'head' or 'tail'.
+            ValueError: If direction is neither 'in' nor 'out'.
         """
-        if node_as == "head":
-            edge = Edge(
-                head=self, tail=node, condition=condition, bundle=bundle, label=label
+        if direction not in ["in", "out"]:
+            raise ValueError(
+                f"Invalid value for direction: {direction}, " "must be 'in' or 'out'"
             )
-            self.relations.points_to[edge.id_] = edge
-            node.relations.pointed_by[edge.id_] = edge
 
-        elif node_as == "tail":
-            edge = Edge(
-                head=node, tail=self, condition=condition, label=label, bundle=bundle
-            )
-            self.relations.pointed_by[edge.id_] = edge
-            node.relations.points_to[edge.id_] = edge
+        edge = Edge(
+            head=self if direction == "out" else node,
+            tail=node if direction == "out" else self,
+            condition=condition,
+            bundle=bundle,
+            label=label,
+        )
 
-        else:
-            raise ValueError(
-                f"Invalid value for self_as: {node_as}, must be 'head' or 'tail'"
-            )
+        self.relations[direction].include(edge)
+        node.relations["in" if direction == "out" else "out"].include(edge)
 
     def remove_edge(self, node: "Node", edge: Edge | str) -> bool:
-        if node.id_ not in self.related_nodes:
-            raise ValueError(f"Node {self.id_} is not related to node {node.id_}.")
+        """
+        Remove specified edge or all edges between this and another node.
 
-        edge_id = edge.id_ if isinstance(edge, Edge) else edge
+        Args:
+            node: Other node involved in edge.
+            edge: Specific edge to remove or 'all' to remove all edges.
 
-        if (
-            edge_id not in self.relations.all_edges
-            or edge_id not in node.relations.all_edges
-        ):
-            raise ValueError(
-                f"Edge {edge_id} does not exist between nodes {self.id_} and "
-                f"{node.id_}."
-            )
+        Returns:
+            True if edge(s) successfully removed, False otherwise.
 
-        all_dicts = [
-            self.relations.points_to,
-            self.relations.pointed_by,
-            node.relations.points_to,
-            node.relations.pointed_by,
+        Raises:
+            RelationError: If removal fails or edge does not exist.
+        """
+        edge_piles = [
+            self.relations["in"],
+            self.relations["out"],
+            node.relations["in"],
+            node.relations["out"],
         ]
-        try:
-            for _dict in all_dicts:
-                edge_id = edge.id_ if isinstance(edge, Edge) else edge
-                _dict.pop(edge_id, None)
-            return True
 
-        except Exception as e:
-            raise ValueError(
-                f"Failed to remove edge between nodes {self.id_} and " f"{node.id_}."
-            ) from e
+        if not all(pile.exclude(edge) for pile in edge_piles):
+            raise RelationError(f"Failed to remove edge between nodes.")
+        return True
 
     def unrelate(self, node: "Node", edge: Edge | str = "all") -> bool:
         """
-        Removes one or all relations between this node and another.
+        Remove all or specific relationships between this and another node.
 
         Args:
-            node (Node): The node to unrelate from.
-            edge (Edge | str): Specific edge or 'all' to remove all relations.
-                Defaults to "all".
+            node: Other node to unrelate from.
+            edge: Specific edge to remove or 'all' for all. Default 'all'.
 
         Returns:
-            bool: True if the operation is successful, False otherwise.
+            True if relationships successfully removed, False otherwise.
 
         Raises:
-            ValueError: If the node is not related or the edge does not exist.
+            RelationError: If operation fails to unrelate nodes.
         """
         if edge == "all":
-            edge = self.node_relations["points_to"].get(
-                node.id_, []
-            ) + self.node_relations["pointed_by"].get(node.id_, [])
+            edges = self.node_relations["out"].get(
+                node.ln_id, []
+            ) + self.node_relations["in"].get(node.ln_id, [])
         else:
-            edge = [edge.id_] if isinstance(edge, Edge) else [edge]
+            edges = [get_lion_id(edge)]
 
-        if len(edge) == 0:
-            raise ValueError(f"Node {self.id_} is not related to node {node.id_}.")
+        if not edges:
+            raise RelationError(f"Node is not related to {node.ln_id}.")
 
         try:
-            for edge_id in edge:
+            for edge_id in edges:
                 self.remove_edge(node, edge_id)
             return True
-        except Exception as e:
-            raise ValueError(
-                f"Failed to remove edge between nodes {self.id_} and " f"{node.id_}."
-            ) from e
+        except RelationError as e:
+            raise e
 
-    def to_llama_index(self, node_type: Type | str | Any = None, **kwargs) -> Any:
-        """
-        Serializes this node for LlamaIndex.
-
-        Args:
-            node_type (Type | str | Any): The type of node in LlamaIndex.
-                Defaults to None.
-            **kwargs: Additional keyword arguments for serialization.
-
-        Returns:
-            Any: The serialized node for LlamaIndex.
-        """
-        return LlamaIndexBridge.to_llama_index_node(self, node_type=node_type, **kwargs)
-
-    def to_langchain(self, **kwargs) -> Any:
-        """
-        Serializes this node for Langchain.
-
-        Args:
-            **kwargs: Additional keyword arguments for serialization.
-
-        Returns:
-            Any: The serialized node for Langchain.
-        """
-        return LangchainBridge.to_langchain_document(self, **kwargs)
-
-    @classmethod
-    def from_llama_index(cls, llama_node: Any, **kwargs) -> "Node":
-        """
-        Deserializes a node from LlamaIndex data.
-
-        Args:
-            llama_node (Any): The LlamaIndex node data.
-            **kwargs: Additional keyword arguments for deserialization.
-
-        Returns:
-            Node: The deserialized node.
-        """
-        llama_dict = llama_node.to_dict(**kwargs)
-        return cls.from_obj(llama_dict)
-
-    @classmethod
-    def from_langchain(cls, lc_doc: Any) -> "Node":
-        """Deserializes a node from Langchain data.
-
-        Args:
-            lc_doc (Any): The Langchain document data.
-
-        Returns:
-            Node: The deserialized node.
-        """
-        langchain_json = lc_doc.to_json()
-        langchain_dict = {"lc_id": langchain_json["id"], **langchain_json["kwargs"]}
-        return cls.from_obj(langchain_dict)
-
-    def __str__(self) -> str:
-        """
-        Provides a string representation of the node.
+    def __str__(self):
+        _dict = self.to_dict()
+        _dict["relations"] = [
+            len(self.relations["in"]),
+            len(self.relations["out"]),
+        ]
+        return Series(_dict).__str__()
 
-        Returns:
-            str: The string representation of the node.
-        """
-        timestamp = f" ({self.timestamp})" if self.timestamp else ""
-        if self.content:
-            content_preview = (
-                f"{self.content[:50]}..." if len(self.content) > 50 else self.content
-            )
-        else:
-            content_preview = ""
-        meta_preview = (
-            f"{str(self.metadata)[:50]}..."
-            if len(str(self.metadata)) > 50
-            else str(self.metadata)
-        )
-        return (
-            f"{self.class_name()}({self.id_}, {content_preview}, {meta_preview},"
-            f"{timestamp})"
-        )
+    def __repr__(self):
+        return self.__str__()
```

### Comparing `lionagi-0.1.2/lionagi/core/session/session.py` & `lionagi-0.2.0/lionagi/core/unit/unit_mixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,985 +1,1168 @@
-from collections import deque
-from typing import Tuple
+"""
+Copyright 2024 HaiyangLi
 
-from pathlib import Path
-from lionagi.libs import BaseService, convert, dataframe
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+"""
+The base directive module.
+"""
+
+import asyncio
+import contextlib
+import re
+from abc import ABC
+
+from typing import Any, Optional
+
+from lionagi.libs import ParseUtil, StringMatch, to_list
+from lionagi.libs.ln_nested import nmerge
+from lionagi.core.collections.abc import ActionError
+from lionagi.core.message import ActionRequest, ActionResponse, Instruction
+from lionagi.core.message.util import _parse_action_request
+from lionagi.core.report.form import Form
+from lionagi.core.unit.util import process_tools
+from lionagi.core.validator.validator import Validator
 
-from lionagi.core.generic import DataLogger
-from lionagi.core.tool import ToolManager, Tool, TOOL_TYPE
-from lionagi.core.mail.mail_manager import MailManager
-from lionagi.core.messages.schema import System, Instruction
-from lionagi.core.branch.branch import Branch
-from lionagi.core.flow.polyflow import PolyChat
 
-
-class Session:
+class DirectiveMixin(ABC):
     """
-    Represents a session for managing conversations and branches.
-
-    A `Session` encapsulates the state and behavior for managing conversations and their branches.
-    It provides functionality for initializing and managing conversation sessions, including setting up default
-    branches, configuring language learning models, managing tools, and handling session data logging.
-
-    Attributes:
-            branches (dict[str, Branch]): A dictionary of branch instances associated with the session.
-            service (BaseService]): The external service instance associated with the | Nonesession.
-            mail_manager (BranchManager): The manager for handling branches within the session.
-            datalogger (Optional[Any]): The datalogger instance for session data logging.
+    DirectiveMixin is a class for handling chat operations and
+    processing responses.
     """
 
-    def __init__(
+    def _create_chat_config(
         self,
-        system: dict | list | System | None = None,
-        sender: str | None = None,
-        llmconfig: dict[str, str | int | dict] | None = None,
-        service: BaseService | None = None,
-        branches: dict[str, Branch] | None = None,
-        default_branch: Branch | None = None,
-        default_branch_name: str | None = None,
-        tools: TOOL_TYPE | None = None,
-        # instruction_sets: Optional[List[Instruction]] = None,
-        tool_manager: ToolManager | None = None,
-        messages: dataframe.ln_DataFrame | None = None,
-        datalogger: None | DataLogger = None,
-        persist_path: Path | str | None = None,
-    ):
-        """Initialize a new session with optional configuration for managing conversations.
+        system: Optional[str] = None,
+        instruction: Optional[str] = None,
+        context: Optional[str] = None,
+        images: Optional[str] = None,
+        sender: Optional[str] = None,
+        recipient: Optional[str] = None,
+        requested_fields: Optional[list] = None,
+        form: Form = None,
+        tools: bool = False,
+        branch: Optional[Any] = None,
+        **kwargs,
+    ) -> Any:
+        """
+        Create the chat configuration based on the provided parameters.
 
         Args:
-                system (Optional[Union[str, System]]): The system message.
-                sender (str | None): the default sender name for default branch
-                llmconfig (dict[str, Any] | None): Configuration for language learning models.
-                service (BaseService]): External service  | Nonenstance.
-                branches (dict[str, Branch] | None): dictionary of branch instances.
-                default_branch (Branch | None): The default branch for the session.
-                default_branch_name (str | None): The name of the default branch.
-                tools (TOOL_TYPE | None): List of tools available for the session.
-                instruction_sets (Optional[List[Instruction]]): List of instruction sets.
-                tool_manager (Optional[Any]): Manager for handling tools.
-                messages (Optional[List[dict[str, Any]]]): Initial list of messages.
-                datalogger (Optional[Any]): Logger instance for the session.
-                persist_path (str | None): Directory path for saving session data.
-
-        Examples:
-                >>> session = Session(system="you are a helpful assistant", sender="researcher")
-        """
-        self.branches = branches if isinstance(branches, dict) else {}
-        self.service = service
-        self.setup_default_branch(
-            system=system,
-            sender=sender,
-            default_branch=default_branch,
-            default_branch_name=default_branch_name,
-            messages=messages,
-            # instruction_sets=instruction_sets,
-            tool_manager=tool_manager,
-            service=service,
-            llmconfig=llmconfig,
-            tools=tools,
-            persist_path=persist_path,
-            datalogger=datalogger,
-        )
-        self.mail_manager = MailManager(self.branches)
-        self.datalogger = self.default_branch.datalogger
-        for key, branch in self.branches.items():
-            branch.name = key
-
-    # --- default branch methods ---- #
-
-    @property
-    def messages(self):
-        return self.default_branch.messages
-
-    @property
-    def messages_describe(self):
-        """
-        Provides a descriptive summary of all messages in the branch.
+            system: System message.
+            instruction: Instruction message.
+            context: Context message.
+            sender: Sender identifier.
+            recipient: Recipient identifier.
+            requested_fields: Fields requested in the response.
+            form: Form data.
+            tools: Flag indicating if tools should be used.
+            branch: Branch instance.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                dict[str, Any]: A dictionary containing summaries of messages by role and sender, total message count,
-                instruction sets, registered tools, and message details.
-
-        Examples:
-                >>> session.messages_describe
-                {'total_messages': 100, 'by_sender': {'User123': 60, 'Bot': 40}}
+            dict: The chat configuration.
         """
-        return self.default_branch.messages_describe
+        branch = branch or self.branch
 
-    @property
-    def has_tools(self) -> bool:
-        """
-        Checks if there are any tools registered in the tool manager.
+        if system:
+            branch.add_message(system=system)
 
-        Returns:
-                bool: True if there are tools registered, False otherwise.
+        if not form:
+            if recipient == "branch.ln_id":
+                recipient = branch.ln_id
+
+            branch.add_message(
+                instruction=instruction,
+                context=context,
+                sender=sender,
+                recipient=recipient,
+                requested_fields=requested_fields,
+                images=images,
+            )
+        else:
+            instruct_ = Instruction.from_form(form)
+            branch.add_message(instruction=instruct_)
 
-        Examples:
-                >>> session.has_tools
-                True
+        if "tool_parsed" in kwargs:
+            kwargs.pop("tool_parsed")
+            tool_kwarg = {"tools": tools}
+            kwargs = tool_kwarg | kwargs
+        elif tools and branch.has_tools:
+            kwargs = branch.tool_manager.parse_tool(tools=tools, **kwargs)
+
+        config = {**self.imodel.config, **kwargs}
+        if sender is not None:
+            config["sender"] = sender
+
+        return config
+
+    async def _call_chatcompletion(
+        self, imodel: Optional[Any] = None, branch: Optional[Any] = None, **kwargs
+    ) -> Any:
         """
-        return self.default_branch.has_tools
+        Calls the chat completion model.
 
-    @property
-    def last_message(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves the last message from the conversation.
+        Args:
+            imodel: The model instance.
+            branch: The branch instance.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                pd.Series: The last message as a pandas Series.
-        """
-        return self.default_branch.last_message
-
-    @property
-    def first_system(self) -> dataframe.ln_DataFrame:
+            Any: The chat completion result.
         """
-        Retrieves the first system message from the conversation.
+        imodel = imodel or self.imodel
+        branch = branch or self.branch
+        return await imodel.call_chat_completion(branch.to_chat_messages(), **kwargs)
 
-        Returns:
-                pd.Series: The first system message as a pandas Series.
+    async def _process_chatcompletion(
+        self,
+        payload: dict,
+        completion: dict,
+        sender: str,
+        invoke_tool: bool = True,
+        branch: Optional[Any] = None,
+        action_request: Optional[Any] = None,
+        costs=None,
+    ) -> Any:
         """
-        return self.default_branch.first_system
+        Processes the chat completion response.
+        Currently only support last message for function calling
 
-    @property
-    def last_response(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves the last response message from the conversation.
+        Args:
+            payload: The payload data.
+            completion: The completion data.
+            sender: The sender identifier.
+            invoke_tool: Flag indicating if tools should be invoked.
+            branch: The branch instance.
+            action_request: The action request instance.
 
         Returns:
-                pd.Series: The last response message as a pandas Series.
+            Any: The processed result.
         """
-        return self.default_branch.last_response
+        branch = branch or self.branch
+        _msg = None
 
-    @property
-    def last_response_content(self) -> dict:
-        """
-        Retrieves the content of the last response message from the conversation.
-
-        Returns:
-                dict: The content of the last response message as a dictionary
-        """
-        return self.default_branch.last_response_content
+        if "choices" in completion:
+            payload.pop("messages", None)
+            branch.update_last_instruction_meta(payload)
+            _choices = completion.pop("choices", None)
+
+            def process_completion_choice(choice, price=None):
+                if isinstance(choice, dict):
+                    msg = choice.pop("message", None)
+                    _completion = completion.copy()
+                    _completion.update(choice)
+                    branch.add_message(
+                        assistant_response=msg,
+                        metadata=_completion,
+                        sender=sender,
+                    )
 
-    @property
-    def tool_request(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves all tool request messages from the conversation.
+                a = branch.messages[-1]._meta_get(
+                    ["extra", "usage", "prompt_tokens"], 0
+                )
+                b = branch.messages[-1]._meta_get(
+                    ["extra", "usage", "completion_tokens"], 0
+                )
+                m = completion.get("model", None)
+                if m:
+                    ttl = (a * price[0] + b * price[1]) / 1000000
+                    branch.messages[-1]._meta_insert(["extra", "usage", "expense"], ttl)
+                return msg
+
+            if _choices and not isinstance(_choices, list):
+                _choices = [_choices]
+
+            if _choices and isinstance(_choices, list):
+                for _choice in _choices:
+                    _msg = process_completion_choice(_choice, price=costs)
 
-        Returns:
-                dataframe.ln_DataFrame: A DataFrame containing all tool request messages.
-        """
-        return self.default_branch.tool_request
+            branch.imodel.status_tracker.num_tasks_succeeded += 1
+        else:
+            branch.imodel.status_tracker.num_tasks_failed += 1
 
-    @property
-    def tool_response(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves all tool response messages from the conversation.
+        return await self._process_action_request(
+            _msg=_msg,
+            branch=branch,
+            invoke_tool=invoke_tool,
+            action_request=action_request,
+        )
 
-        Returns:
-                dataframe.ln_DataFrame: A DataFrame containing all tool response messages.
+    async def _process_action_request(
+        self,
+        _msg: Optional[dict] = None,
+        branch: Optional[Any] = None,
+        invoke_tool: bool = True,
+        action_request: Optional[Any] = None,
+    ) -> Any:
         """
-        return self.default_branch.tool_response
+        Processes an action request from the assistant response.
 
-    @property
-    def responses(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves all response messages from the conversation.
+        Args:
+            _msg: The message data.
+            branch: The branch instance.
+            invoke_tool: Flag indicating if tools should be invoked.
+            action_request: The action request instance.
 
         Returns:
-                dataframe.ln_DataFrame: A DataFrame containing all response messages.
+            Any: The processed result.
         """
-        return self.default_branch.responses
+        action_request = action_request or _parse_action_request(_msg)
+        if action_request is None:
+            return _msg if _msg else False
+
+        if action_request:
+            for i in action_request:
+                if i.function in branch.tool_manager.registry:
+                    i.recipient = branch.tool_manager.registry[i.function].ln_id
+                else:
+                    raise ActionError(f"Tool {i.function} not found in registry")
+                branch.add_message(action_request=i, recipient=i.recipient)
+
+        if invoke_tool:
+            tasks = []
+            for i in action_request:
+                tool = branch.tool_manager.registry[i.function]
+                tasks.append(asyncio.create_task(tool.invoke(i.arguments)))
+            results = await asyncio.gather(*tasks)
+
+            for idx, item in enumerate(results):
+                if item is not None:
+                    branch.add_message(
+                        action_request=action_request[idx],
+                        func_outputs=item,
+                        sender=action_request[idx].recipient,
+                        recipient=action_request[idx].sender,
+                    )
 
-    @property
-    def assistant_responses(self) -> dataframe.ln_DataFrame:
-        """
-        Retrieves all assistant responses from the conversation, excluding tool requests and responses.
+        return None
 
-        Returns:
-                dataframe.ln_DataFrame: A DataFrame containing assistant responses excluding tool requests and responses.
+    async def _output(
+        self,
+        payload: dict,
+        completion: dict,
+        sender: str,
+        invoke_tool: bool,
+        requested_fields: dict,
+        form: Form = None,
+        return_form: bool = True,
+        strict: bool = False,
+        rulebook: Any = None,
+        use_annotation: bool = True,
+        template_name: str = None,
+        costs=None,
+    ) -> Any:
         """
-        return self.default_branch.assistant_responses
+        Outputs the final processed response.
 
-    @property
-    def info(self) -> dict[str, int]:
-        """
-        Get a summary of the conversation messages categorized by role.
+        Args:
+            payload: The payload data.
+            completion: The completion data.
+            sender: The sender identifier.
+            invoke_tool: Flag indicating if tools should be invoked.
+            requested_fields: Fields requested in the response.
+            form: Form data.
+            return_form: Flag indicating if form should be returned.
+            strict: Flag indicating if strict validation should be applied.
+            rulebook: Rulebook instance for validation.
+            use_annotation: Flag indicating if annotations should be used.
+            template_name: Template name for form.
 
         Returns:
-                dict[str, int]: A dictionary with keys as message roles and values as counts.
+            Any: The processed response.
         """
+        _msg = await self._process_chatcompletion(
+            payload=payload,
+            completion=completion,
+            sender=sender,
+            invoke_tool=invoke_tool,
+            costs=costs,
+        )
 
-        return self.default_branch.info
+        if _msg is None:
+            return None
 
-    @property
-    def sender_info(self) -> dict[str, int]:
-        """
-        Provides a descriptive summary of the conversation, including total message count and summary by sender.
+        response_ = self._process_model_response(_msg, requested_fields)
 
-        Returns:
-                dict[str, Any]: A dictionary containing the total number of messages and a summary categorized by sender.
-        """
-        return self.default_branch.sender_info
+        if form:
+            validator = Validator(rulebook=rulebook) if rulebook else self.validator
+            form = await validator.validate_response(
+                form=form,
+                response=response_,
+                strict=strict,
+                use_annotation=use_annotation,
+            )
+            if template_name:
+                form.template_name = template_name
+
+            return (
+                form
+                if return_form
+                else {
+                    i: form.work_fields[i]
+                    for i in form.requested_fields
+                    if form.work_fields[i] is not None
+                }
+            )
 
-    def register_tools(self, tools):
-        self.default_branch.register_tools(tools)
+        return response_
 
-    @classmethod
-    def from_csv(
-        cls,
-        filepath: Path | str,
-        system: dict | list | System | None = None,
-        sender: str | None = None,
-        llmconfig: dict[str, str | int | dict] | None = None,
-        service: BaseService = None,
-        default_branch_name: str = "main",
-        tools: TOOL_TYPE = False,  # instruction_sets=None,
-        tool_manager=None,
+    async def _base_chat(
+        self,
+        instruction: Any = None,
+        *,
+        system: Any = None,
+        context: Any = None,
+        sender: Any = None,
+        recipient: Any = None,
+        requested_fields: dict = None,
+        form: Form = None,
+        tools: Any = False,
+        images: Optional[str] = None,
+        invoke_tool: bool = True,
+        return_form: bool = True,
+        strict: bool = False,
+        rulebook: Any = None,
+        imodel: Any = None,
+        use_annotation: bool = True,
+        branch: Any = None,
+        clear_messages: bool = False,
+        return_branch: bool = False,
         **kwargs,
-    ) -> "Session":
+    ) -> Any:
         """
-        Creates a Session instance from a CSV file containing messages.
+        Handles the base chat operation by configuring the chat and
+        processing the response.
 
         Args:
-                filepath (str): Path to the CSV file.
-                name (str | None): Name of the branch, default is None.
-                instruction_sets (Optional[dict[str, InstructionSet]]): Instruction sets, default is None.
-                tool_manager (Optional[ToolManager]): Tool manager for the branch, default is None.
-                service (BaseService]): External service for the branch, default | Noneis None.
-                llmconfig (Optional[dict]): Configuration for language learning models, default is None.
-                tools (TOOL_TYPE | None): Initial list of tools to register, default is None.
-                **kwargs: Additional keyword arguments for pd.read_csv().
+            instruction: Instruction message.
+            system: System message.
+            context: Context message.
+            sender: Sender identifier.
+            recipient: Recipient identifier.
+            requested_fields: Fields requested in the response.
+            form: Form data.
+            tools: Flag indicating if tools should be used.
+            invoke_tool: Flag indicating if tools should be invoked.
+            return_form: Flag indicating if form should be returned.
+            strict: Flag indicating if strict validation should be applied.
+            rulebook: Rulebook instance for validation.
+            imodel: Model instance.
+            use_annotation: Flag indicating if annotations should be used.
+            branch: Branch instance.
+            clear_messages: Flag indicating if messages should be cleared.
+            return_branch: Flag indicating if branch should be returned.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                Branch: A new Branch instance created from the CSV data.
-
-        Examples:
-                >>> branch = Branch.from_csv("path/to/messages.csv", name="ImportedBranch")
+            Any: The processed response and branch.
         """
-        df = dataframe.read_csv(filepath, **kwargs)
+        branch = branch or self.branch
+        if clear_messages:
+            branch.clear()
+            branch.set_system(system)
 
-        return cls(
+        config = self._create_chat_config(
             system=system,
+            instruction=instruction,
+            context=context,
             sender=sender,
-            llmconfig=llmconfig,
-            service=service,
-            default_branch_name=default_branch_name,
+            recipient=recipient,
+            requested_fields=requested_fields,
+            form=form,
             tools=tools,
-            tool_manager=tool_manager,
-            messages=df,
+            branch=branch,
+            images=images,
             **kwargs,
         )
 
-    @classmethod
-    def from_json(
-        cls,
-        filepath: Path | str,
-        system: dict | list | System | None = None,
-        sender: str | None = None,
-        llmconfig: dict[str, str | int | dict] | None = None,
-        service: BaseService = None,
-        default_branch_name: str = "main",
-        tools: TOOL_TYPE = False,  # instruction_sets=None,
-        tool_manager=None,
+        payload, completion = await self._call_chatcompletion(
+            imodel=imodel, branch=branch, **config
+        )
+
+        imodel = imodel or self.imodel
+        out_ = await self._output(
+            payload=payload,
+            completion=completion,
+            sender=sender,
+            invoke_tool=invoke_tool,
+            requested_fields=requested_fields,
+            form=form,
+            return_form=return_form,
+            strict=strict,
+            rulebook=rulebook,
+            use_annotation=use_annotation,
+            costs=imodel.costs,
+        )
+
+        return out_, branch if return_branch else out_
+
+    async def _chat(
+        self,
+        instruction=None,
+        context=None,
+        system=None,
+        sender=None,
+        recipient=None,
+        branch=None,
+        requested_fields=None,
+        form: Form = None,
+        tools=False,
+        invoke_tool=True,
+        return_form=True,
+        strict=False,
+        rulebook=None,
+        imodel=None,
+        images: Optional[str] = None,
+        clear_messages=False,
+        use_annotation=True,
+        timeout: float = None,
+        return_branch=False,
         **kwargs,
-    ) -> "Session":
+    ):
         """
-        Creates a Branch instance from a JSON file containing messages.
+        Handles the chat operation.
 
         Args:
-                filepath (str): Path to the JSON file.
-                name (str | None): Name of the branch, default is None.
-                instruction_sets (Optional[dict[str, InstructionSet]]): Instruction sets, default is None.
-                tool_manager (Optional[ToolManager]): Tool manager for the branch, default is None.
-                service (BaseService]): External service for the branch, default | Noneis None.
-                llmconfig (Optional[dict]): Configuration for language learning models, default is None.
-                **kwargs: Additional keyword arguments for pd.read_json().
+            instruction: Instruction message.
+            context: Context message.
+            system: System message.
+            sender: Sender identifier.
+            recipient: Recipient identifier.
+            branch: Branch instance.
+            requested_fields: Fields requested in the response.
+            form: Form data.
+            tools: Flag indicating if tools should be used.
+            invoke_tool: Flag indicating if tools should be invoked.
+            return_form: Flag indicating if form should be returned.
+            strict: Flag indicating if strict validation should be applied.
+            rulebook: Rulebook instance for validation.
+            imodel: Model instance.
+            clear_messages: Flag indicating if messages should be cleared.
+            use_annotation: Flag indicating if annotations should be used.
+            timeout: Timeout value.
+            return_branch: Flag indicating if branch should be returned.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                Branch: A new Branch instance created from the JSON data.
-
-        Examples:
-                >>> branch = Branch.from_json_string("path/to/messages.json", name="JSONBranch")
+            Any: The processed response.
         """
-        df = dataframe.read_json(filepath, **kwargs)
-        return cls(
+        a = await self._base_chat(
+            context=context,
+            instruction=instruction,
             system=system,
             sender=sender,
-            llmconfig=llmconfig,
-            service=service,
-            default_branch_name=default_branch_name,
-            tools=tools,  # instruction_sets=instruction_sets,
-            tool_manager=tool_manager,
-            messages=df,
+            recipient=recipient,
+            requested_fields=requested_fields,
+            form=form,
+            tools=tools,
+            images=images,
+            invoke_tool=invoke_tool,
+            return_form=return_form,
+            strict=strict,
+            rulebook=rulebook,
+            imodel=imodel,
+            use_annotation=use_annotation,
+            timeout=timeout,
+            branch=branch,
+            clear_messages=clear_messages,
+            return_branch=return_branch,
             **kwargs,
         )
 
-    def to_csv_file(
-        self,
-        filename: str = "messages.csv",
-        dir_exist_ok: bool = True,
-        timestamp: bool = True,
-        time_prefix: bool = False,
-        verbose: bool = True,
-        clear: bool = True,
-        **kwargs,
-    ):
-        """
-        Saves the branch's messages to a CSV file.
+        if isinstance(a, str):
+            return a
 
-        Args:
-                filename (str): The name of the output CSV file, default is 'messages.csv'.
-                dir_exist_ok (bool): If True, does not raise an error if the directory already exists, default is True.
-                timestamp (bool): If True, appends a timestamp to the filename, default is True.
-                time_prefix (bool): If True, adds a timestamp prefix to the filename, default is False.
-                verbose (bool): If True, prints a message upon successful save, default is True.
-                clear (bool): If True, clears the messages after saving, default is True.
-                **kwargs: Additional keyword arguments for DataFrame.to_csv().
-
-        Examples:
-                >>> branch.to_csv_file("exported_messages.csv")
-                >>> branch.to_csv_file("timed_export.csv", timestamp=True, time_prefix=True)
-        """
-        for name, branch in self.branches.items():
-            f_name = f"{name}_{filename}"
-            branch.to_csv_file(
-                filename=f_name,
-                dir_exist_ok=dir_exist_ok,
-                timestamp=timestamp,
-                time_prefix=time_prefix,
-                verbose=verbose,
-                clear=clear,
-                **kwargs,
-            )
+        a = list(a)
 
-    def to_json_file(
+        if len(a) == 2 and a[0] == a[1]:
+            return a[0] if not isinstance(a[0], tuple) else a[0][0]
+        if len(a) == 2 and a[0] != a[1]:
+            return a[0], a[1]
+        if len(a) == 1 and isinstance(a[0], tuple):
+            return a[0][0]
+        if len(a) == 1 and not isinstance(a[0], tuple):
+            return a[0]
+
+    async def _direct(
         self,
-        filename: str = "messages.json",
-        dir_exist_ok: bool = False,
-        timestamp: bool = True,
-        time_prefix: bool = False,
-        verbose: bool = True,
-        clear: bool = True,
+        instruction=None,
+        context=None,
+        form: Form = None,
+        branch=None,
+        tools=None,
+        reason: bool = None,
+        predict: bool = None,
+        score: bool = None,
+        select: bool = None,
+        plan: bool = None,
+        allow_action: bool = None,
+        allow_extension: bool = None,
+        confidence: bool = None,
+        max_extension: int = None,
+        score_num_digits=None,
+        score_range=None,
+        select_choices=None,
+        plan_num_step=None,
+        predict_num_sentences=None,
+        clear_messages=False,
+        return_branch=False,
+        images: Optional[str] = None,
+        verbose=None,
         **kwargs,
     ):
         """
-        Saves the branch's messages to a JSON file.
+        Directs the operation based on the provided parameters.
 
         Args:
-                filename (str): The name of the output JSON file, default is 'messages.json'.
-                dir_exist_ok (bool): If True, does not raise an error if the directory already exists, default is True.
-                timestamp (bool): If True, appends a timestamp to the filename, default is True.
-                time_prefix (bool): If True, adds a timestamp prefix to the filename, default is False.
-                verbose (bool): If True, prints a message upon successful save, default is True.
-                clear (bool): If True, clears the messages after saving, default is True.
-                **kwargs: Additional keyword arguments for DataFrame.to_json().
-
-        Examples:
-                >>> branch.to_json_file("exported_messages.json")
-                >>> branch.to_json_file("timed_export.json", timestamp=True, time_prefix=True)
-        """
-
-        for name, branch in self.branches.items():
-            f_name = f"{name}_{filename}"
-            branch.to_json_file(
-                filename=f_name,
-                dir_exist_ok=dir_exist_ok,
-                timestamp=timestamp,
-                time_prefix=time_prefix,
-                verbose=verbose,
-                clear=clear,
-                **kwargs,
-            )
+            instruction: Instruction message.
+            context: Context message.
+            form: Form data.
+            branch: Branch instance.
+            tools: Tools data.
+            reason: Flag indicating if reason should be included.
+            predict: Flag indicating if prediction should be included.
+            score: Flag indicating if score should be included.
+            select: Flag indicating if selection should be included.
+            plan: Flag indicating if plan should be included.
+            allow_action: Flag indicating if action should be allowed.
+            allow_extension: Flag indicating if extension should be allowed.
+            confidence: Flag indicating if confidence should be included.
+            max_extension: Maximum extension value.
+            score_num_digits: Number of digits for score.
+            score_range: Range for score.
+            select_choices: Choices for selection.
+            plan_num_step: Number of steps for plan.
+            predict_num_sentences: Number of sentences for prediction.
+            clear_messages: Flag indicating if messages should be cleared.
+            return_branch: Flag indicating if branch should be returned.
+            kwargs: Additional keyword arguments.
 
-    def log_to_csv(
-        self,
-        filename: str = "log.csv",
-        dir_exist_ok: bool = True,
-        timestamp: bool = True,
-        time_prefix: bool = False,
-        verbose: bool = True,
-        clear: bool = True,
-        **kwargs,
-    ):
+        Returns:
+            Any: The processed response and branch.
         """
-        Saves the branch's log data to a CSV file.
+        a = await self._base_direct(
+            instruction=instruction,
+            context=context,
+            form=form,
+            branch=branch,
+            tools=tools,
+            reason=reason,
+            predict=predict,
+            score=score,
+            select=select,
+            images=images,
+            plan=plan,
+            allow_action=allow_action,
+            allow_extension=allow_extension,
+            confidence=confidence,
+            max_extension=max_extension,
+            score_num_digits=score_num_digits,
+            score_range=score_range,
+            select_choices=select_choices,
+            plan_num_step=plan_num_step,
+            predict_num_sentences=predict_num_sentences,
+            clear_messages=clear_messages,
+            return_branch=return_branch,
+            verbose=verbose,
+            **kwargs,
+        )
 
-        This method is designed to export log data, potentially including operations and intertools,
-        to a CSV file for analysis or record-keeping.
+        a = list(a)
+        if len(a) == 2 and a[0] == a[1]:
+            return a[0] if not isinstance(a[0], tuple) else a[0][0]
 
-        Args:
-                filename (str): The name of the output CSV file. Defaults to 'log.csv'.
-                dir_exist_ok (bool): If True, will not raise an error if the directory already exists. Defaults to True.
-                timestamp (bool): If True, appends a timestamp to the filename for uniqueness. Defaults to True.
-                time_prefix (bool): If True, adds a timestamp prefix to the filename. Defaults to False.
-                verbose (bool): If True, prints a success message upon completion. Defaults to True.
-                clear (bool): If True, clears the log after saving. Defaults to True.
-                **kwargs: Additional keyword arguments for `DataFrame.to_csv()`.
-
-        Examples:
-                >>> branch.log_to_csv("branch_log.csv")
-                >>> branch.log_to_csv("detailed_branch_log.csv", timestamp=True, verbose=True)
-        """
-        for name, branch in self.branches.items():
-            f_name = f"{name}_{filename}"
-            branch.log_to_csv(
-                filename=f_name,
-                dir_exist_ok=dir_exist_ok,
-                timestamp=timestamp,
-                time_prefix=time_prefix,
-                verbose=verbose,
-                clear=clear,
-                **kwargs,
-            )
+        return a[0], a[1]
 
-    def log_to_json(
+    async def _base_direct(
         self,
-        filename: str = "log.json",
-        dir_exist_ok: bool = True,
-        timestamp: bool = True,
-        time_prefix: bool = False,
-        verbose: bool = True,
-        clear: bool = True,
+        instruction=None,
+        *,
+        context=None,
+        form: Form = None,
+        branch=None,
+        tools=None,
+        reason: bool = None,
+        predict: bool = None,
+        score: bool = None,
+        select: bool = None,
+        plan: bool = None,
+        allow_action: bool = None,
+        allow_extension: bool = None,
+        confidence: bool = None,
+        max_extension: int = None,
+        score_num_digits=None,
+        score_range=None,
+        select_choices=None,
+        plan_num_step=None,
+        predict_num_sentences=None,
+        clear_messages=False,
+        return_branch=False,
+        images: Optional[str] = None,
+        verbose=None,
         **kwargs,
     ):
         """
-        Saves the branch's log data to a JSON file.
-
-        Useful for exporting log data in JSON format, allowing for easy integration with web applications
-        and services that consume JSON.
+        Handles the base direct operation.
 
         Args:
-                filename (str): The name of the output JSON file. Defaults to 'log.json'.
-                dir_exist_ok (bool): If directory existence should not raise an error. Defaults to True.
-                timestamp (bool): If True, appends a timestamp to the filename. Defaults to True.
-                time_prefix (bool): If True, adds a timestamp prefix to the filename. Defaults to False.
-                verbose (bool): If True, prints a success message upon completion. Defaults to True.
-                clear (bool): If True, clears the log after saving. Defaults to True.
-                **kwargs: Additional keyword arguments for `DataFrame.to_json()`.
-
-        Examples:
-                >>> branch.log_to_json("branch_log.json")
-                >>> branch.log_to_json("detailed_branch_log.json", verbose=True, timestamp=True)
-        """
-        for name, branch in self.branches.items():
-            f_name = f"{name}_{filename}"
-            branch.log_to_json(
-                filename=f_name,
-                dir_exist_ok=dir_exist_ok,
-                timestamp=timestamp,
-                time_prefix=time_prefix,
-                verbose=verbose,
-                clear=clear,
-                **kwargs,
-            )
+            instruction: Instruction message.
+            context: Context message.
+            form: Form data.
+            branch: Branch instance.
+            tools: Tools data.
+            reason: Flag indicating if reason should be included.
+            predict: Flag indicating if prediction should be included.
+            score: Flag indicating if score should be included.
+            select: Flag indicating if selection should be included.
+            plan: Flag indicating if plan should be included.
+            allow_action: Flag indicating if action should be allowed.
+            allow_extension: Flag indicating if extension should be allowed.
+            confidence: Flag indicating if confidence should be included.
+            max_extension: Maximum extension value.
+            score_num_digits: Number of digits for score.
+            score_range: Range for score.
+            select_choices: Choices for selection.
+            plan_num_step: Number of steps for plan.
+            predict_num_sentences: Number of sentences for prediction.
+            clear_messages: Flag indicating if messages should be cleared.
+            return_branch: Flag indicating if branch should be returned.
+            kwargs: Additional keyword arguments.
 
-    @property
-    def all_messages(self) -> dataframe.ln_DataFrame:
-        """
-        return all messages across branches
-        """
-        dfs = deque()
-        for _, v in self.branches.items():
-            dfs.append(convert.to_df(v.messages))
-        return convert.to_df(convert.to_list(dfs, flatten=True, dropna=True))
-
-    # ----- chatflow ----#
-    async def call_chatcompletion(
-        self,
-        branch: Branch | str | None = None,
-        sender: str | None = None,
-        with_sender=False,
-        **kwargs,
-    ):
+        Returns:
+            Any: The processed response and branch.
         """
-        Asynchronously calls the chat completion service with the current message queue.
+        # Ensure branch is initialized
+        branch = branch or self.branch
+        if clear_messages:
+            branch.clear()
+
+        # Set a default max_extension if allow_extension is True and max_extension is None
+        if allow_extension and not max_extension:
+            max_extension = 3  # Set a default limit for recursion
+
+        # Process tools if provided
+        if tools:
+            process_tools(tools, branch)
+
+        if allow_action and not tools:
+            tools = True
+
+        tool_schema=None
+        if tools:
+            tool_schema = branch.tool_manager.get_tool_schema(tools)
+
+        if not form:
+            form = self.default_template(
+                instruction=instruction,
+                context=context,
+                reason=reason,
+                predict=predict,
+                score=score,
+                select=select,
+                plan=plan,
+                tool_schema=tool_schema,
+                allow_action=allow_action,
+                allow_extension=allow_extension,
+                max_extension=max_extension,
+                confidence=confidence,
+                score_num_digits=score_num_digits,
+                score_range=score_range,
+                select_choices=select_choices,
+                plan_num_step=plan_num_step,
+                predict_num_sentences=predict_num_sentences,
+            )
 
-        This method prepares the messages for chat completion, sends the request to the configured service, and handles the response. The method supports additional keyword arguments that are passed directly to the service.
+        elif form and "tool_schema" not in form._all_fields:
+            form.append_to_input("tool_schema")
+            form.tool_schema = tool_schema
 
-        Args:
-                sender (str | None): The name of the sender to be included in the chat completion request. Defaults to None.
-                with_sender (bool): If True, includes the sender's name in the messages. Defaults to False.
-                **kwargs: Arbitrary keyword arguments passed directly to the chat completion service.
+        else:
+            form.tool_schema = tool_schema
 
-        Examples:
-                >>> await branch.call_chatcompletion()
-        """
-        branch = self.get_branch(branch)
-        await branch.call_chatcompletion(
-            sender=sender,
-            with_sender=with_sender,
+        verbose = (
+            verbose
+            if verbose is not None and isinstance(verbose, bool)
+            else self.verbose
+        )
+        if verbose:
+            print("Chatting with model...")
+
+        # Call the base chat method
+        form = await self._chat(
+            form=form,
+            branch=branch,
+            images=images,
             **kwargs,
         )
 
-    async def chat(
-        self,
-        instruction: dict | list | Instruction | str,
-        branch: Branch | str | None = None,
-        context: dict | list | str = None,
-        sender: str | None = None,
-        system: dict | list | System | None = None,
-        tools: TOOL_TYPE = False,
-        out: bool = True,
-        invoke: bool = True,
-        output_fields=None,
-        **kwargs,
-    ) -> str | None:
-        """
-        a chat conversation with LLM, processing instructions and system messages, optionally invoking tools.
+        # Handle actions if allowed and required
+        if allow_action and getattr(form, "action_required", None):
+            actions = getattr(form, "actions", None)
+            if actions:
+                if verbose:
+                    print(
+                        "Found action requests in model response. Processing actions..."
+                    )
+                form = await self._act(form, branch, actions=actions)
+                if verbose:
+                    print("Actions processed!")
+
+        last_form = form
+
+        ctr = 1
+
+        # Handle extensions if allowed and required
+        extension_forms = []
+        max_extension = max_extension if isinstance(max_extension, int) else 3
+        while (
+            allow_extension
+            and max_extension > 0
+            and getattr(last_form, "extension_required", None)
+        ):
+            if getattr(last_form, "is_extension", None):
+                break
+            if verbose:
+                print(f"\nFound extension requests in model response.")
+                print(
+                    f"------------------- Processing extension No.{ctr} -------------------"
+                )
 
-        Args:
-                branch: The Branch instance to perform chat operations.
-                instruction (dict | list | Instruction | str): The instruction for the chat.
-                context (Optional[Any]): Additional context for the chat.
-                sender (str | None): The sender of the chat message.
-                system (Optional[Union[System, str, dict[str, Any]]]): System message to be processed.
-                tools (Union[bool, Tool, List[Tool], str, List[str]]): Specifies tools to be invoked.
-                out (bool): If True, outputs the chat response.
-                invoke (bool): If True, invokes tools as part of the chat.
-                **kwargs: Arbitrary keyword arguments for chat completion.
+            max_extension -= 1
 
-        Examples:
-                >>> await ChatFlow.chat(branch, "Ask about user preferences")
-        """
+            # new form cannot be extended, otherwise it will be an infinite loop
+            new_form = await self._extend(
+                tools=tools,
+                reason=reason,
+                predict=predict,
+                score=score,
+                select=select,
+                plan=getattr(last_form, "plan", None),
+                allow_action=allow_action,
+                confidence=confidence,
+                score_num_digits=score_num_digits,
+                score_range=score_range,
+                select_choices=select_choices,
+                predict_num_sentences=predict_num_sentences,
+                **kwargs,
+            )
 
-        branch = self.get_branch(branch)
-        return await branch.chat(
-            instruction=instruction,
-            context=context,
-            sender=sender,
-            system=system,
-            tools=tools,
-            out=out,
-            invoke=invoke,
-            output_fields=output_fields,
-            **kwargs,
-        )
+            if verbose:
+                print(f"------------------- Extension completed -------------------\n")
+
+            extension_forms.extend(new_form)
+            last_form = new_form[-1] if isinstance(new_form, list) else new_form
+            ctr += len(form)
+
+        if extension_forms:
+            if not getattr(form, "extension_forms", None):
+                form._add_field("extension_forms", list, None, [])
+            form.extension_forms.extend(extension_forms)
+            action_responses = [
+                i.action_response
+                for i in extension_forms
+                if getattr(i, "action_response", None) is not None
+            ]
+            if not hasattr(form, "action_response"):
+                form.add_field("action_response", {})
+
+            for action_response in action_responses:
+                nmerge([form.action_response, action_response])
+
+        if "PLEASE_ACTION" in form.answer:
+            if verbose:
+                print("Analyzing action responses and generating answer...")
+
+            answer = await self._chat(
+                "please provide final answer basing on the above"
+                " information, provide answer value as a string only"
+                " do not return as json, do not include other information",
+            )
 
-    async def ReAct(
+            if isinstance(answer, dict):
+                a = answer.get("answer", None)
+                if a is not None:
+                    answer = a
+
+            answer = str(answer).strip()
+            if answer.startswith("{") and answer.endswith("}"):
+                answer = answer[1:-1]
+                answer = answer.strip()
+            if '"answer":' in answer:
+                answer.replace('"answer":', "")
+                answer = answer.strip()
+            elif "'answer':" in answer:
+                answer.replace("'answer':", "")
+                answer = answer.strip()
+
+            form.answer = answer
+
+        return form, branch if return_branch else form
+
+    async def _extend(
         self,
-        instruction: dict | list | Instruction | str,
-        branch: Branch | str | None = None,
-        context=None,
-        sender=None,
-        system=None,
-        tools=None,
-        auto=False,
-        num_rounds: int = 1,
-        reason_prompt=None,
-        action_prompt=None,
-        output_prompt=None,
+        tools,
+        reason,
+        predict,
+        score,
+        select,
+        plan,
+        # image,
+        allow_action,
+        confidence,
+        score_num_digits,
+        score_range,
+        select_choices,
+        predict_num_sentences,
         **kwargs,
     ):
         """
-        Performs a reason-tool cycle with optional tool invocation over multiple rounds.
+        Handles the extension of the form based on the provided parameters.
 
         Args:
-                branch: The Branch instance to perform ReAct operations.
-                instruction (dict | list | Instruction | str): Initial instruction for the cycle.
-                context: Context relevant to the instruction.
-                sender (str | None): Identifier for the message sender.
-                system: Initial system message or configuration.
-                tools: Tools to be registered or used during the cycle.
-                num_rounds (int): Number of reason-tool cycles to perform.
-                **kwargs: Additional keyword arguments for customization.
+            form: Form data.
+            tools: Tools data.
+            reason: Flag indicating if reason should be included.
+            predict: Flag indicating if prediction should be included.
+            score: Flag indicating if score should be included.
+            select: Flag indicating if selection should be included.
+            plan: Flag indicating if plan should be included.
+            allow_action: Flag indicating if action should be allowed.
+            confidence: Flag indicating if confidence should be included.
+            score_num_digits: Number of digits for score.
+            score_range: Range for score.
+            select_choices: Choices for selection.
+            predict_num_sentences: Number of sentences for prediction.
+            allow_extension: Flag indicating if extension should be allowed.
+            max_extension: Maximum extension value.
+            kwargs: Additional keyword arguments.
 
-        Examples:
-                >>> await ChatFlow.ReAct(branch, "Analyze user feedback", num_rounds=2)
+        Returns:
+            list: The extended forms.
         """
-        branch = self.get_branch(branch)
+        extension_forms = []
 
-        return await branch.ReAct(
-            instruction=instruction,
-            context=context,
-            sender=sender,
-            system=system,
-            tools=tools,
-            auto=auto,
-            num_rounds=num_rounds,
-            reason_prompt=reason_prompt,
-            action_prompt=action_prompt,
-            output_prompt=output_prompt,
+        # Ensure the next step in the plan is handled
+        directive_kwargs = {
+            "tools": tools,
+            "reason": reason,
+            "predict": predict,
+            "score": score,
+            "select": select,
+            "allow_action": allow_action,
+            "confidence": confidence,
+            "score_num_digits": score_num_digits,
+            "score_range": score_range,
+            "select_choices": select_choices,
+            "predict_num_sentences": predict_num_sentences,
             **kwargs,
-        )
+        }
 
-    async def followup(
-        self,
-        instruction: dict | list | Instruction | str,
-        branch=None,
-        context=None,
-        sender=None,
-        system=None,
-        tools=None,
-        max_followup: int = 1,
-        auto=False,
-        followup_prompt=None,
-        output_prompt=None,
-        out=True,
-        **kwargs,
-    ):
+        if plan:
+            keys = [f"step_{i+1}" for i in range(len(plan))]
+            plan = StringMatch.force_validate_dict(plan, keys)
+
+            # If plan is provided, process each step
+            for i in keys:
+                directive_kwargs["instruction"] = plan[i]
+                last_form = await self._direct(**directive_kwargs)
+                last_form.is_extension = True
+                extension_forms.append(last_form)
+                directive_kwargs["max_extension"] -= 1
+                if not getattr(last_form, "extension_required", None):
+                    break
+
+        else:
+            # Handle single step extension
+            last_form = await self._direct(**directive_kwargs)
+            last_form.is_extension = True
+            extension_forms.append(last_form)
+
+        return extension_forms
+
+    async def _act(self, form, branch, actions=None):
         """
-        Automatically performs follow-up tools based on chat intertools and tool invocations.
+        Processes actions based on the provided form and actions.
 
         Args:
-                branch: The Branch instance to perform follow-up operations.
-                instruction (dict | list | Instruction | str): The initial instruction for follow-up.
-                context: Context relevant to the instruction.
-                sender (str | None): Identifier for the message sender.
-                system: Initial system message or configuration.
-                tools: Specifies tools to be considered for follow-up tools.
-                max_followup (int): Maximum number of follow-up chats allowed.
-                out (bool): If True, outputs the result of the follow-up tool.
-                **kwargs: Additional keyword arguments for follow-up customization.
+            form: Form data.
+            branch: Branch instance.
+            actions: Actions data.
 
-        Examples:
-                >>> await ChatFlow.auto_followup(branch, "Finalize report", max_followup=2)
+        Returns:
+            dict: The updated form.
         """
-        branch = self.get_branch(branch)
-        return await branch.followup(
-            instruction=instruction,
-            context=context,
-            sender=sender,
-            system=system,
-            tools=tools,
-            max_followup=max_followup,
-            auto=auto,
-            followup_prompt=followup_prompt,
-            output_prompt=output_prompt,
-            out=out,
-            **kwargs,
-        )
+        if getattr(form, "action_performed", None) is True:
+            return form
+
+        keys = [f"action_{i+1}" for i in range(len(actions))]
+        actions = StringMatch.force_validate_dict(actions, keys)
+
+        try:
+            requests = []
+            for k in keys:
+                _func = actions[k]["function"]
+                _func = _func.replace("functions.", "")
+                msg = ActionRequest(
+                    function=_func,
+                    arguments=actions[k]["arguments"],
+                    sender=branch.ln_id,
+                    recipient=branch.tool_manager.registry[_func].ln_id,
+                )
+                requests.append(msg)
+                branch.add_message(action_request=msg)
+
+            if requests:
+                out = await self._process_action_request(
+                    branch=branch, invoke_tool=True, action_request=requests
+                )
+
+                if out is False:
+                    raise ValueError("No requests found.")
 
-    async def parallel_chat(
+                len_actions = len(actions)
+                action_responses = [
+                    i
+                    for i in branch.messages[-len_actions:]
+                    if isinstance(i, ActionResponse)
+                ]
+
+                _action_responses = {}
+                for idx, item in enumerate(action_responses):
+                    _action_responses[f"action_{idx+1}"] = item._to_dict()
+
+                form.append_to_request("action_response")
+                if (a := getattr(form, "action_response", None)) is None:
+                    form.add_field("action_response", {})
+
+                len1 = len(form.action_response)
+                for k, v in _action_responses.items():
+                    while k in form.action_response:
+                        k = f"{k}_1"
+                    form.action_response[k] = v
+
+                if len(form.action_response) > len1:
+                    form.append_to_request("action_performed")
+                    form.action_performed = True
+                return form
+
+        except Exception as e:
+            raise ValueError(f"Error processing action request: {e}")
+
+    async def _select(
         self,
-        instruction: Instruction | str,
-        num_instances=1,
+        form=None,
+        choices=None,
+        reason=False,
+        confidence_score=None,
+        instruction=None,
+        template=None,
         context=None,
-        sender=None,
-        branch_system=None,
-        messages=None,
-        tools=False,
-        out=True,
-        invoke: bool = True,
-        output_fields=None,
-        persist_path=None,
-        branch_config=None,
-        explode=False,
-        include_mapping=False,
+        branch=None,
         **kwargs,
     ):
         """
-        parallel chat
-        """
+        Selects a response based on the provided parameters.
 
-        if branch_config is None:
-            branch_config = {}
-        flow = PolyChat(self)
+        Args:
+            form (Any, optional): Form to create instruction from.
+            choices (Any, optional): Choices for the selection.
+            reason (bool, optional): Whether to include a reason for the selection.
+            confidence_score (Any, optional): Confidence score for the selection.
+            instruction (Any, optional): Instruction for the selection.
+            template (Any, optional): Template for the selection.
+            context (Any, optional): Context to perform the selection on.
+            branch (Any, optional): Branch to use for the selection.
+            **kwargs: Additional arguments for the selection.
 
-        return await flow.parallel_chat(
-            instruction,
-            num_instances=num_instances,
-            context=context,
-            sender=sender,
-            branch_system=branch_system,
-            messages=messages,
-            tools=tools,
-            out=out,
-            invoke=invoke,
-            output_fields=output_fields,
-            persist_path=persist_path,
-            branch_config=branch_config,
-            explode=explode,
-            include_mapping=include_mapping,
-            **kwargs,
-        )
+        Returns:
+            Any: The selection response.
+        """
+        branch = branch or self.branch
 
-    # ---- branch manipulation ---- #
-    def new_branch(
-        self,
-        branch_name: str,
-        system: dict | list | System | None = None,
-        sender: str | None = None,
-        messages: dataframe.ln_DataFrame | None = None,
-        tool_manager=None,
-        service=None,
-        llmconfig=None,
-        tools: TOOL_TYPE = False,
-    ) -> None:
-        """Create a new branch with the specified configurations.
-
-        Args:
-                branch_name (str | None): Name of the new branch.
-                system (Optional[Union[System, str]]): System or context identifier for the new branch.
-                sender (str | None): Default sender identifier for the new branch.
-                messages (Optional[dataframe.ln_DataFrame]): Initial set of messages for the new branch.
-                instruction_sets (Optional[Any]): Instruction sets for the new branch.
-                tool_manager (Optional[Any]): Tool manager for handling tools in the new branch.
-                service (BaseService]): External service instance for the ne | None branch.
-                llmconfig (dict[str, Any] | None): Configuration for language learning models in the new branch.
-                tools (TOOL_TYPE | None): List of tools available for the new branch.
-
-        Raises:
-                ValueError: If the branch name already exists.
-
-        Examples:
-                >>> session.new_branch("new_branch_name")
-        """
-        if branch_name in self.branches.keys():
-            raise ValueError(
-                f"Invalid new branch name {branch_name}. Branch already existed."
+        if not form:
+            form = template(
+                choices=choices,
+                reason=reason,
+                confidence_score=confidence_score,
+                instruction=instruction,
+                context=context,
             )
-        if isinstance(tools, Tool):
-            tools = [tools]
-        new_branch = Branch(
-            name=branch_name,
-            messages=messages,
-            tool_manager=tool_manager,
-            service=service,
-            llmconfig=llmconfig,
-            tools=tools,
-        )
-        if system:
-            new_branch.add_message(system=system, sender=sender)
 
-        self.branches[branch_name] = new_branch
-        self.mail_manager.sources[branch_name] = new_branch
-        self.mail_manager.mails[branch_name] = {}
+        return await self._chat(form=form, return_form=True, branch=branch, **kwargs)
 
-    def get_branch(
-        self, branch: Branch | str | None = None, get_name: bool = False
-    ) -> Branch | Tuple[Branch, str]:
+    async def _predict(
+        self,
+        form=None,
+        num_sentences=None,
+        reason=False,
+        confidence_score=None,
+        instruction=None,
+        context=None,
+        branch=None,
+        template=None,
+        **kwargs,
+    ):
         """
-        Retrieve a branch by name or instance.
+        Predicts a response based on the provided parameters.
 
         Args:
-                branch (Optional[Branch | str]): The branch name or instance to retrieve.
-                get_name (bool): If True, returns a tuple of the branch instance and its name.
+            form: Form data.
+            num_sentences: Number of sentences for the prediction.
+            reason: Flag indicating if reason should be included.
+            confidence_score: Confidence score for the prediction.
+            instruction: Instruction for the prediction.
+            context: Context to perform the prediction on.
+            branch: Branch instance.
+            template: Template for the prediction.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                Union[Branch, Tuple[Branch, str]]: The branch instance or a tuple of the branch instance and its name.
-
-        Raises:
-                ValueError: If the branch name does not exist or the branch input is invalid.
-
-        Examples:
-                >>> branch_instance = session.get_branch("existing_branch_name")
-                >>> branch_instance, branch_name = session.get_branch("existing_branch_name", get_name=True)
+            Any: The prediction response.
         """
-        if isinstance(branch, str):
-            if branch not in self.branches.keys():
-                raise ValueError(f"Invalid branch name {branch}. Not exist.")
-            return (
-                (self.branches[branch], branch) if get_name else self.branches[branch]
-            )
-        elif isinstance(branch, Branch) and branch in self.branches.values():
-            return (branch, branch.name) if get_name else branch
-        elif branch is None:
-            if get_name:
-                return self.default_branch, self.default_branch_name
-            return self.default_branch
+        branch = branch or self.branch
 
-        else:
-            raise ValueError(f"Invalid branch input {branch}.")
-
-    def change_default_branch(self, branch: str | Branch) -> None:
-        """Change the default branch of the session.
+        if not form:
+            form = template(
+                instruction=instruction,
+                context=context,
+                num_sentences=num_sentences,
+                confidence_score=confidence_score,
+                reason=reason,
+            )
 
-        Args:
-                branch (str | Branch): The branch name or instance to set as the new default.
+        return await self._chat(form=form, return_form=True, branch=branch, **kwargs)
 
-        Examples:
-                >>> session.change_default_branch("new_default_branch")
+    async def _score(
+        self,
+        form=None,
+        score_range=None,
+        include_endpoints=None,
+        num_digit=None,
+        reason=False,
+        confidence_score=None,
+        instruction=None,
+        context=None,
+        branch=None,
+        template=None,
+        **kwargs,
+    ):
         """
-        branch_, name_ = self.get_branch(branch, get_name=True)
-        self.default_branch = branch_
-        self.default_branch_name = name_
-
-    def delete_branch(self, branch: Branch | str, verbose: bool = True) -> bool:
-        """Delete a branch from the session.
+        Scores a response based on the provided parameters.
 
         Args:
-                branch (Branch | str): The branch name or instance to delete.
-                verbose (bool): If True, prints a message upon deletion.
+            form: Form data.
+            score_range: Range for score.
+            include_endpoints: Flag indicating if endpoints should be included.
+            num_digit: Number of digits for score.
+            reason: Flag indicating if reason should be included.
+            confidence_score: Confidence score for the score.
+            instruction: Instruction for the score.
+            context: Context to perform the score on.
+            branch: Branch instance.
+            template: Template for the score.
+            kwargs: Additional keyword arguments.
 
         Returns:
-                bool: True if the branch was successfully deleted.
-
-        Raises:
-                ValueError: If attempting to delete the current default branch.
-
-        Examples:
-                >>> session.delete_branch("branch_to_delete")
+            Any: The score response.
         """
-        _, branch_name = self.get_branch(branch, get_name=True)
-
-        if branch_name == self.default_branch_name:
-            raise ValueError(
-                f"{branch_name} is the current default branch, please switch to another branch before delete it."
+        branch = branch or self.branch
+        if not form:
+            form = template(
+                score_range=score_range,
+                include_endpoints=include_endpoints,
+                num_digit=num_digit,
+                reason=reason,
+                confidence_score=confidence_score,
+                instruction=instruction,
+                context=context,
             )
-        self.branches.pop(branch_name)
-        # self.mail_manager.sources.pop(branch_name)
-        self.mail_manager.mails.pop(branch_name)
-        if verbose:
-            print(f"Branch {branch_name} is deleted.")
-        return True
 
-    def merge_branch(
+        return await self._chat(form=form, return_form=True, branch=branch, **kwargs)
+
+    async def _plan(
         self,
-        from_: str | Branch,
-        to_branch: str | Branch,
-        update: bool = True,
-        del_: bool = False,
-    ) -> None:
-        """Merge messages and settings from one branch to another.
+        form=None,
+        num_step=None,
+        reason=False,
+        confidence_score=None,
+        instruction=None,
+        context=None,
+        branch=None,
+        template=None,
+        **kwargs,
+    ):
+        """
+        Plans a response based on the provided parameters.
 
         Args:
-                from_ (str | Branch): The source branch name or instance.
-                to_branch (str | Branch): The target branch name or instance where the merge will happen.
-                update (bool): If True, updates the target branch with the source branch's settings.
-                del_ (bool): If True, deletes the source branch after merging.
+            form: Form data.
+            num_step: Number of steps for the plan.
+            reason: Flag indicating if reason should be included.
+            confidence_score: Confidence score for the plan.
+            instruction: Instruction for the plan.
+            context: Context to perform the plan on.
+            branch: Branch instance.
+            template: Template for the plan.
+            kwargs: Additional keyword arguments.
 
-        Examples:
-                >>> session.merge_branch("source_branch", "target_branch", del_=True)
+        Returns:
+            Any: The plan response.
         """
-        from_ = self.get_branch(branch=from_)
-        to_branch, to_name = self.get_branch(branch=to_branch, get_name=True)
-        to_branch.merge_branch(from_, update=update)
+        branch = branch or self.branch
+        template = template or self.default_template
 
-        if del_:
-            if from_ == self.default_branch:
-                self.default_branch_name = to_name
-                self.default_branch = to_branch
-            self.delete_branch(from_, verbose=False)
+        if not form:
+            form = template(
+                instruction=instruction,
+                context=context,
+                num_step=num_step,
+                reason=reason,
+                confidence_score=confidence_score,
+            )
 
-    def take_branch(self, branch):
-        self.branches[branch.branch_name] = branch
-        self.mail_manager.sources[branch.id_] = branch
-        self.mail_manager.mails[branch.id_] = {}
+        return await self._chat(form=form, **kwargs)
 
-    def collect(self, from_: str | Branch | list[str | Branch] | None = None):
+    @staticmethod
+    def _process_model_response(content_, requested_fields):
         """
-        Collects requests from specified branches or from all branches if none are specified.
-
-        This method is intended to aggregate data or requests from one or more branches for processing or analysis.
+        Processes the model response content.
 
         Args:
-                from_ (Optional[Union[str, Branch, List[str | Branch]]]): The branch(es) from which to collect requests.
-                        Can be a single branch name, a single branch instance, a list of branch names, a list of branch instances, or None.
-                        If None, requests are collected from all branches.
+            content_: The content data.
+            requested_fields: Fields requested in the response.
 
-        Examples:
-                >>> session.collect("branch_name")
-                >>> session.collect([branch_instance_1, "branch_name_2"])
-                >>> session.collect()  # Collects from all branches
+        Returns:
+            Any: The processed response.
         """
-        if from_ is None:
-            for branch in self.branches.values():
-                self.mail_manager.collect(branch.id_)
-        else:
-            if not isinstance(from_, list):
-                from_ = [from_]
-            for branch in from_:
-                if isinstance(branch, str):
-                    branch = self.branches[branch]
-                    self.mail_manager.collect(branch.id_)
-                elif isinstance(branch, Branch):
-                    self.mail_manager.collect(branch.id_)
-
-    def send(self, to_: str | Branch | list[str | Branch] | None = None):
-        """
-        Sends requests or data to specified branches or to all branches if none are specified.
-
-        This method facilitates the distribution of data or requests to one or more branches, potentially for further tool or processing.
-
-        Args:
-                to_ (Optional[Union[str, Branch, List[str | Branch]]]): The target branch(es) to which to send requests.
-                        Can be a single branch name, a single branch instance, a list of branch names, a list of branch instances, or None.
-                        If None, requests are sent to all branches.
-
-        Examples:
-                >>> session.send("target_branch")
-                >>> session.send([branch_instance_1, "target_branch_2"])
-                >>> session.send()  # Sends to all branches
-        """
-        if to_ is None:
-            for branch in self.branches.values():
-                self.mail_manager.send(branch.id_)
-        else:
-            if not isinstance(to_, list):
-                to_ = [to_]
-            for branch in to_:
-                if isinstance(branch, str):
-                    branch = self.branches[branch]
-                    self.mail_manager.send(branch.id_)
-                if isinstance(branch, Branch):
-                    self.mail_manager.send(branch.id_)
-
-    def collect_send_all(self, receive_all=False):
-        """
-        Collects and sends requests across all branches, optionally invoking a receive operation on each branch.
-
-        This method is a convenience function for performing a full cycle of collect and send operations across all branches,
-        useful in scenarios where data or requests need to be aggregated and then distributed uniformly.
-
-        Args:
-                receive_all (bool): If True, triggers a `receive_all` method on each branch after sending requests,
-                        which can be used to process or acknowledge the received data.
-
-        Examples:
-                >>> session.collect_send_all()
-                >>> session.collect_send_all(receive_all=True)
-        """
-        self.collect()
-        self.send()
-        if receive_all:
-            for branch in self.branches.values():
-                branch.receive_all()
-
-    def setup_default_branch(self, **kwargs):
-        self._setup_default_branch(**kwargs)
-        self._verify_default_branch()
-
-    def _verify_default_branch(self):
-        if self.branches:
-            if self.default_branch_name not in self.branches.keys():
-                raise ValueError("default branch name is not in imported branches")
-            if self.default_branch is not self.branches[self.default_branch_name]:
-                raise ValueError(
-                    f"default branch does not match Branch object under {self.default_branch_name}"
-                )
+        out_ = content_.get("content", "")
+        if out_ == "":
+            out_ = content_
 
-        if not self.branches:
-            self.branches[self.default_branch_name] = self.default_branch
+        if requested_fields:
+            with contextlib.suppress(Exception):
+                return StringMatch.force_validate_dict(out_, requested_fields)
 
-    def _setup_default_branch(
-        self,
-        system,
-        sender,
-        default_branch,
-        default_branch_name,
-        messages,  # instruction_sets,
-        tool_manager,
-        service,
-        llmconfig,
-        tools,
-        persist_path,
-        datalogger,
-    ):
+        if isinstance(out_, str):
+            with contextlib.suppress(Exception):
+                return ParseUtil.fuzzy_parse_json(out_)
 
-        branch = default_branch or Branch(
-            name=default_branch_name,
-            service=service,
-            llmconfig=llmconfig,
-            tools=tools,
-            tool_manager=tool_manager,
-            # instruction_sets=instruction_sets,
-            messages=messages,
-            persist_path=persist_path,
-            datalogger=datalogger,
-        )
+            with contextlib.suppress(Exception):
+                return ParseUtil.extract_json_block(out_)
 
-        self.default_branch = branch
-        self.default_branch_name = default_branch_name or "main"
-        if system:
-            self.default_branch.add_message(system=system, sender=sender)
+            with contextlib.suppress(Exception):
+                match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
+                if match:
+                    return ParseUtil.fuzzy_parse_json(match.group(1))
 
-        self.llmconfig = self.default_branch.llmconfig
+        return out_
```

### Comparing `lionagi-0.1.2/lionagi/core/tool/tool_manager.py` & `lionagi-0.2.0/lionagi/core/action/tool_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,283 +1,356 @@
-import asyncio
+"""
+Copyright 2024 HaiyangLi
 
-from typing import Tuple, Any, TypeVar, Callable
-from lionagi.libs import func_call, convert, ParseUtil
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
+"""
+This module contains the ToolManager class, which manages tools in the system.
+It allows registering, invoking, and retrieving schemas of tools. Tools can be
+registered individually or in batches, and invoked using function names, JSON
+strings, or specialized objects.
+"""
+
+import inspect
+from functools import singledispatchmethod
+from typing import Any, Callable, List, Union, Tuple
+from lionagi.libs import ParseUtil
+from lionagi.libs.ln_convert import to_list, to_dict
+from lionagi.libs.ln_func_call import lcall
+from lionagi.core.collections.abc import Actionable
+from lionagi.core.action.function_calling import FunctionCalling
+from lionagi.core.action.tool import Tool, TOOL_TYPE
 
-from lionagi.core.tool.tool import Tool, TOOL_TYPE
 
-T = TypeVar("T", bound=Tool)
-
-
-class ToolManager:
+class ToolManager(Actionable):
     """
-    A manager class for handling the registration and invocation of tools that are subclasses of Tool.
-
-    This class maintains a registry of tool instances, allowing for dynamic invocation based on
-    tool name and provided arguments. It supports both synchronous and asynchronous tool function
-    calls.
-
-    Attributes:
-        registry (dict[str, Tool]): A dictionary to hold registered tools, keyed by their names.
+    Manages tools in the system. Provides functionality to register tools,
+    invoke them based on various input formats, and retrieve tool schemas.
     """
 
-    registry: dict = {}
-
-    def name_existed(self, name: str) -> bool:
+    def __init__(self, registry: dict[str, Tool] = None) -> None:
         """
-        Checks if a tool name already exists in the registry.
+        Initializes a new instance of ToolManager.
 
         Args:
-            name (str): The name of the tool to check.
-
-        Returns:
-            bool: True if the name exists, False otherwise.
+            registry (dict[str, Tool], optional): A dictionary to store registered tools.
+                Defaults to an empty dictionary.
         """
-        return name in self.registry
+        self.registry = registry or {}
 
-    @property
-    def has_tools(self):
-        return self.registry != {}
+    def __contains__(self, tool) -> bool:
+        if isinstance(tool, Tool):
+            return tool.name in self.registry
+
+        elif isinstance(tool, str):
+            return tool in self.registry
+
+        elif inspect.isfunction(tool):
+            return tool.__name__ in self.registry
 
-    def _register_tool(self, tool: Tool | Callable) -> None:
+        return False
+
+    def _register_tool(self, tool: Tool | Callable, update: bool = False) -> bool:
         """
-        Registers a tool in the registry. Raises a TypeError if the object is not an instance of Tool.
+        Registers a single tool or multiple tools based on the input type.
 
         Args:
-            tool (Tool): The tool instance to register.
+            tool (Any): Can be a single Tool, a list of Tools, a callable, or other forms.
 
         Raises:
-            TypeError: If the provided object is not an instance of Tool.
+            TypeError: If the tools argument type is unsupported.
         """
+        if not update and tool in self:
+            raise ValueError(f"Function {tool.name} is already registered.")
         if isinstance(tool, Callable):
-            tool = func_to_tool(tool)[0]
+            tool = func_to_tool(tool)
+            tool = tool[0] if isinstance(tool, list) and len(tool) == 1 else tool
         if not isinstance(tool, Tool):
             raise TypeError("Please register a Tool object.")
-        name = tool.schema_["function"]["name"]
-        self.registry.update({name: tool})
+        self.registry[tool.name] = tool
+        return True
+
+    def update_tools(self, tools: list | Tool | Callable):
+        if isinstance(tools, Tool) or isinstance(tools, Callable):
+            return self._register_tool(tools, update=True)
+        else:
+            return all(lcall(tools, self._register_tool, update=True))
 
-    async def invoke(self, func_calls: Tuple[str, dict[str, Any]]) -> Any:
+    def register_tools(self, tools: list | Tool | Callable):
         """
-        Invokes a registered tool's function with the given arguments. Supports both coroutine and regular functions.
+        Registers multiple Tools.
 
         Args:
-            func_call (Tuple[str, Dict[str, Any]]): A tuple containing the function name and a dictionary of keyword arguments.
+            tools (list): The list of Tools to register.
+
+        Returns:
+            bool: True if all tools are successfully registered.
+        """
+        if isinstance(tools, Tool) or isinstance(tools, Callable):
+            return self._register_tool(tools)
+        else:
+            return all(lcall(tools, self._register_tool))
+
+    async def invoke(self, func_calling=None):
+        """
+        Invokes a function based on the provided function calling description.
+
+        Args:
+            func_calling (Any, optional): The function calling description, which can be:
+                - tuple: (name, kwargs)
+                - dict: {"function": name, "arguments": kwargs}
+                - str: JSON string of dict format
+                - ActionRequest object
+                - FunctionCalling object
 
         Returns:
             Any: The result of the function call.
 
         Raises:
-            ValueError: If the function name is not registered or if there's an error during function invocation.
+            ValueError: If func_calling is None or the function is not registered.
         """
-        name, kwargs = func_calls
-        if not self.name_existed(name):
-            raise ValueError(f"Function {name} is not registered.")
-        tool = self.registry[name]
-        func = tool.func
-        parser = tool.parser
-        try:
-            if func_call.is_coroutine_func(func):
-                tasks = [func_call.call_handler(func, **kwargs)]
-                out = await asyncio.gather(*tasks)
-                return parser(out[0]) if parser else out[0]
-            else:
-                out = func(**kwargs)
-                return parser(out) if parser else out
-        except Exception as e:
-            raise ValueError(
-                f"Error when invoking function {name} with arguments {kwargs} with error message {e}"
-            ) from e
+        if not func_calling:
+            raise ValueError("func_calling is required.")
 
-    @staticmethod
-    def get_function_call(response: dict) -> Tuple[str, dict]:
+        if not isinstance(func_calling, FunctionCalling):
+            func_calling = FunctionCalling.create(func_calling)
+
+        if func_calling.func_name in self.registry:
+            return await self.registry[func_calling.func_name].invoke(
+                func_calling=func_calling
+            )
+
+        raise ValueError(f"Function {func_calling.func_name} is not registered.")
+
+    @property
+    def _schema_list(self) -> list[dict[str, Any]]:
+        """
+        Lists all tool schemas currently registered in the ToolManager.
+
+        Returns:
+            list[dict[str, Any]]: A list of tool schemas.
+        """
+        return [tool.schema_ for tool in self.registry.values()]
+
+    def get_tool_schema(self, tools: TOOL_TYPE, **kwargs) -> dict:
         """
-        Extracts a function call and arguments from a response dictionary.
+        Retrieves the schema for a specific tool or all tools based on the input.
 
         Args:
-            response (dict): The response dictionary containing the function call information.
+            tools (TOOL_TYPE): Can be a boolean, specific tool name, Tool, or list of tools.
+            **kwargs: Additional keyword arguments to be merged with tool schema.
 
         Returns:
-            Tuple[str, dict]: A tuple containing the function name and a dictionary of arguments.
+            dict: Combined tool schema and kwargs.
+        """
+        if isinstance(tools, bool):
+            tool_kwarg = {"tools": self._schema_list}
+            return tool_kwarg | kwargs
+
+        else:
+            tool_kwarg = {"tools": self._get_tool_schema(tools)}
+            return tool_kwarg | kwargs
+
+    @singledispatchmethod
+    def _get_tool_schema(self, tool: Any) -> dict:
+        """
+        Retrieves the schema for a specific tool based on its type.
+
+        Args:
+            tool (Any): The tool descriptor, can be a dict, Tool, str, or list.
 
         Raises:
-            ValueError: If the response does not contain valid function call information.
+            TypeError: If the tool type is unsupported.
         """
-        try:
-            func = response["action"][7:]
-            args = convert.to_dict(response["arguments"])
-            return func, args
-        except Exception:
-            try:
-                func = response["recipient_name"].split(".")[-1]
-                args = response["parameters"]
-                return func, args
-            except:
-                raise ValueError("response is not a valid function call")
+        raise TypeError(f"Unsupported type {type(tool)}")
 
-    def register_tools(self, tools: list[Tool]) -> None:
+    @_get_tool_schema.register(dict)
+    def _(self, tool):
         """
-        Registers multiple tools in the registry.
+        Assumes that the tool is a schema and returns it.
 
         Args:
-            tools (list[Tool]): A list of tool instances to register.
+            tool (dict): The tool schema.
+
+        Returns:
+            dict: The tool schema.
         """
-        func_call.lcall(tools, self._register_tool)
+        return tool
 
-    def to_tool_schema_list(self) -> list[dict[str, Any]]:
+    @_get_tool_schema.register(Tool)
+    def _(self, tool):
         """
-        Generates a list of schemas for all registered tools.
+        Retrieves the schema for a Tool object.
+
+        Args:
+            tool (Tool): The Tool object.
 
         Returns:
-            list[dict[str, Any]]: A list of tool schemas.
+            dict: The tool schema.
 
+        Raises:
+            ValueError: If the Tool is not registered.
         """
-        return [tool.schema_ for tool in self.registry.values()]
+        if tool.name in self.registry:
+            return self.registry[tool.name].schema_
+        else:
+            err_msg = f"Function {tool.name} is not registered."
+            raise ValueError(err_msg)
 
-    def parse_tool(self, tools: TOOL_TYPE, **kwargs) -> dict:
+    @_get_tool_schema.register(str)
+    def _(self, tool):
         """
-        Parses tool information and generates a dictionary for tool invocation.
+        Assumes that the tool is a name and retrieves its schema.
 
         Args:
-            tools: Tool information which can be a single Tool instance, a list of Tool instances, a tool name, or a list of tool names.
-            **kwargs: Additional keyword arguments.
+            tool (str): The tool name.
 
         Returns:
-            dict: A dictionary containing tool schema information and any additional keyword arguments.
+            dict: The tool schema.
 
         Raises:
-            ValueError: If a tool name is provided that is not registered.
+            ValueError: If the tool name is not registered.
         """
+        if tool in self.registry:
+            return self.registry[tool].schema_
+        else:
+            err_msg = f"Function {tool} is not registered."
+            raise ValueError(err_msg)
 
-        def tool_check(tool):
-            if isinstance(tool, dict):
-                return tool
-            elif isinstance(tool, Tool):
-                return tool.schema_
-            elif isinstance(tool, str):
-                if self.name_existed(tool):
-                    tool: Tool = self.registry[tool]
-                    return tool.schema_
-                else:
-                    raise ValueError(f"Function {tool} is not registered.")
+    @_get_tool_schema.register(list)
+    def _(self, tools):
+        """
+        Retrieves the schema for a list of tools.
+
+        Args:
+            tools (list): The list of tools.
 
+        Returns:
+            list: A list of tool schemas.
+        """
+        return lcall(tools, self._get_tool_schema)
+
+    def parse_tool(self, tools: TOOL_TYPE, **kwargs) -> dict:
+        """
+        Parses and merges tool schemas based on the provided tool descriptors.
+
+        Args:
+            tools (TOOL_TYPE): The tools to parse, can be a single tool or list.
+            **kwargs: Additional keyword arguments to be merged with the tool schema.
+
+        Returns:
+            dict: The merged tool schema and additional arguments.
+        """
         if tools:
             if isinstance(tools, bool):
-                tool_kwarg = {"tools": self.to_tool_schema_list()}
+                tool_kwarg = {"tools": self._schema_list}
                 kwargs = tool_kwarg | kwargs
-
             else:
-                if not isinstance(tools, list):
-                    tools = [tools]
-                tool_kwarg = {"tools": func_call.lcall(tools, tool_check)}
+                tools = to_list(tools) if not isinstance(tools, list) else [tools]
+                tool_kwarg = {"tools": lcall(tools, self._get_tool_schema)}
                 kwargs = tool_kwarg | kwargs
 
         return kwargs
 
+    @staticmethod
+    def parse_tool_request(response: dict) -> Tuple[str, dict]:
+        """
+        Parses a tool request from a given response dictionary.
+
+        Args:
+            response (dict): The response data containing the tool request.
+
+        Returns:
+            Tuple[str, dict]: The function name and its arguments.
+
+        Raises:
+            ValueError: If the response is not a valid function call.
+        """
+        try:
+            func = response["action"][7:]
+            args = to_dict(response["arguments"])
+            return func, args
+        except Exception:
+            try:
+                func = response["recipient_name"].split(".")[-1]
+                args = response["parameters"]
+                return func, args
+            except:
+                raise ValueError("response is not a valid function call")
+
 
 def func_to_tool(
-    func_: Callable | list[Callable], parser=None, docstring_style="google"
-):
+    func_: Union[Callable, List[Callable]],
+    parser: Union[Callable, List[Callable]] = None,
+    docstring_style: str = "google",
+    **kwargs,
+) -> List[Tool]:
     """
-    Transforms a given function into a Tool object, equipped with a schema derived
-    from its docstring. This process involves parsing the function's docstring based
-    on a specified style ('google' or 'reST') to extract relevant metadata and
-    parameters, which are then used to construct a comprehensive schema for the Tool.
-    This schema facilitates the integration of the function with systems or
-    frameworks that rely on structured metadata for automation, documentation, or
-    interface generation purposes.
-
-    The function to be transformed can be any Callable that adheres to the
-    specified docstring conventions. The resulting Tool object encapsulates the
-    original function, allowing it to be utilized within environments that require
-    objects with structured metadata.
+    Converts functions to Tool objects, optionally associating parsers with each function
+    and applying a specified docstring parsing style to generate tool schemas.
 
     Args:
-        func_ (Callable): The function to be transformed into a Tool object. This
-            function should have a docstring that follows the
-            specified docstring style for accurate schema generation.
-        parser (Optional[Any]): An optional parser object associated with the Tool.
-                  This parameter is currently not utilized in the
-                  transformation process but is included for future
-                  compatibility and extension purposes.
-        docstring_style (str): The format of the docstring to be parsed, indicating
-                 the convention used in the function's docstring.
-                 Supports 'google' for Google-style docstrings and
-                 'reST' for reStructuredText-style docstrings. The
-                 chosen style affects how the docstring is parsed and
-                 how the schema is generated.
+        func_ (Callable | list[Callable]): The function(s) to convert into tool(s).
+        parser (Callable | list[Callable], optional): Parser(s) to associate with
+            the function(s). If a list is provided, it should match the length of func_.
+        docstring_style (str, optional): The style of the docstring parser to use when
+            generating tool schemas. Defaults to "google".
 
     Returns:
-        Tool: An object representing the original function wrapped as a Tool, along
-            with its generated schema. This Tool object can be used in systems that
-            require detailed metadata about functions, facilitating tasks such as
-            automatic documentation generation, user interface creation, or
-            integration with other software tools.
+        list[Tool]: A list of Tool objects created from the provided function(s).
+
+    Raises:
+        ValueError: If the length of the parsers does not match the length of the
+            functions when both are provided as lists.
 
     Examples:
-        >>> def example_function_google(param1: int, param2: str) -> bool:
-        ...     '''
-        ...     An example function using Google style docstrings.
-        ...
-        ...     Args:
-        ...         param1 (int): The first parameter, demonstrating an integer input_.
-        ...         param2 (str): The second parameter, demonstrating a string input_.
-        ...
-        ...     Returns:
-        ...         bool: A boolean value, illustrating the return type.
-        ...     '''
-        ...     return True
-        ...
-        >>> tool_google = func_to_tool(example_function_google, docstring_style='google')
-        >>> print(isinstance(tool_google, Tool))
-        True
-
-        >>> def example_function_reST(param1: int, param2: str) -> bool:
-        ...     '''
-        ...     An example function using reStructuredText (reST) style docstrings.
-        ...
-        ...     :param param1: The first parameter, demonstrating an integer input_.
-        ...     :type param1: int
-        ...     :param param2: The second parameter, demonstrating a string input_.
-        ...     :type param2: str
-        ...     :returns: A boolean value, illustrating the return type.
-        ...     :rtype: bool
-        ...     '''
-        ...     return True
-        ...
-        >>> tool_reST = func_to_tool(example_function_reST, docstring_style='reST')
-        >>> print(isinstance(tool_reST, Tool))
-        True
-
-    Note:
-        The transformation process relies heavily on the accuracy and completeness of
-        the function's docstring. Functions with incomplete or incorrectly formatted
-        docstrings may result in incomplete or inaccurate Tool schemas.
-    """
+        # Convert a single function with a custom parser
+        tools = func_to_tool(my_function, my_parser)
 
+        # Convert multiple functions without parsers
+        tools = func_to_tool([func_one, func_two])
+
+        # Convert multiple functions with multiple parsers
+        tools = func_to_tool([func_one, func_two], [parser_one, parser_two])
+    """
     fs = []
-    funcs = convert.to_list(func_, flatten=True, dropna=True)
-    parsers = convert.to_list(parser, flatten=True, dropna=True)
+    funcs = to_list(func_, flatten=True, dropna=True)
+    parsers = to_list(parser, flatten=True, dropna=True)
 
     if parser:
         if len(funcs) != len(parsers) != 1:
             raise ValueError(
                 "Length of parser must match length of func. Except if you only pass one"
             )
 
         for idx in range(len(funcs)):
             f_ = lambda _f: Tool(
-                func=_f,
+                function=_f,
                 schema_=ParseUtil._func_to_schema(_f, style=docstring_style),
                 parser=parsers[idx] if len(parsers) > 1 else parsers[0],
+                **kwargs,
             )
 
             fs.append(f_)
 
     else:
-        fs = func_call.lcall(
+        fs = lcall(
             funcs,
             lambda _f: Tool(
-                func=_f, schema_=ParseUtil._func_to_schema(_f, style=docstring_style)
+                function=_f,
+                schema_=ParseUtil._func_to_schema(_f, style=docstring_style),
+                **kwargs,
             ),
         )
 
     return fs
```

### Comparing `lionagi-0.1.2/lionagi/experimental/directive/evaluator/ast_evaluator.py` & `lionagi-0.2.0/lionagi/experimental/evaluator/ast_evaluator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import ast
 import operator
 
 
 class ASTEvaluator:
     """
     Safely evaluates expressions using AST parsing to prevent unsafe operations.
```

### Comparing `lionagi-0.1.2/lionagi/experimental/directive/evaluator/base_evaluator.py` & `lionagi-0.2.0/lionagi/experimental/evaluator/base_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import ast
 import operator
 from typing import Any, Dict, Tuple, Callable
 
 from lionagi.libs.ln_convert import to_dict
```

### Comparing `lionagi-0.1.2/lionagi/experimental/directive/evaluator/script_engine.py` & `lionagi-0.2.0/lionagi/core/engine/script_engine.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,27 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import ast
 from functools import lru_cache
 from lionagi.libs import AsyncUtil
-from .base_evaluator import BaseEvaluator
+from ..evaluator.base_evaluator import BaseEvaluator
 from .sandbox_ import SandboxTransformer
 
 
 class ScriptEngine:
     def __init__(self):
         self.variables = {}
         self.safe_evaluator = BaseEvaluator()
```

### Comparing `lionagi-0.1.2/lionagi/experimental/directive/schema.py` & `lionagi-0.2.0/lionagi/experimental/directive/template/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/experimental/report/util.py` & `lionagi-0.2.0/lionagi/core/collections/abc/util.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-from lionagi.libs import convert
+base_lion_fields = [
+    "ln_id",
+    "timestamp",
+    "metadata",
+    "extra_fields",
+    "content",
+    "created",
+    "embedding",
+]
 
-system_fields = [
+lc_meta_fields = ["lc", "type", "id", "langchain", "lc_type", "lc_id"]
+
+llama_meta_fields = [
     "id_",
-    "node_id",
-    "meta",
-    "metadata",
+    "embedding",
+    "excluded_embed_metadata_keys",
+    "excluded_llm_metadata_keys",
+    "relationships",
+    "start_char_idx",
+    "end_char_idx",
+    "class_name",
+    "text_template",
+    "metadata_template",
+    "metadata_seperator",
+]
+
+SYSTEM_FIELDS = [
+    "ln_id",
     "timestamp",
+    "metadata",
+    "meta",
+    "extra_fields",
     "content",
+    "created",
+    "form",
+    "report",
+    "work",
     "assignment",
     "assignments",
-    "task",
-    "template_name",
-    "version",
-    "description",
-    "in_validation_kwargs",
-    "out_validation_kwargs",
-    "fix_input",
-    "fix_output",
     "input_fields",
-    "output_fields",
-    "choices",
-    "prompt_fields",
-    "prompt_fields_annotation",
-    "instruction_context",
+    "requested_fields",
     "instruction",
-    "instruction_output_fields",
-    "inputs",
-    "outputs",
-    "process",
-    "_validate_field",
-    "_process_input",
-    "_process_response",
-    "_validate_field_choices",
-    "_validate_input_choices",
-    "_validate_output_choices",
+    "system",
+    "strict",
 ]
-
-
-def get_input_output_fields(str_: str) -> list[list[str]]:
-
-    inputs, outputs = str_.split("->")
-
-    input_fields = [convert.strip_lower(i) for i in inputs.split(",")]
-    output_fields = [convert.strip_lower(o) for o in outputs.split(",")]
-
-    return input_fields, output_fields
```

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/autogen_/autogen_.py` & `lionagi-0.2.0/lionagi/integrations/bridge/autogen_/autogen_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/langchain_/documents.py` & `lionagi-0.2.0/lionagi/integrations/bridge/langchain_/documents.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,18 @@
     SysUtil.check_import("langchain")
     from langchain.schema import Document as LangchainDocument
 
     dnode = datanode.to_dict()
     SysUtil.change_dict_key(dnode, old_key="content", new_key="page_content")
     SysUtil.change_dict_key(dnode, old_key="lc_id", new_key="id_")
     dnode = {**dnode, **kwargs}
+    dnode = {k: v for k, v in dnode.items() if v is not None}
+    if "page_content" not in dnode:
+        dnode["page_content"] = ""
+
     return LangchainDocument(**dnode)
 
 
 def langchain_loader(
     loader: Union[str, Callable],
     loader_args: List[Any] = [],
     loader_kwargs: Dict[str, Any] = {},
```

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/langchain_/langchain_bridge.py` & `lionagi-0.2.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py` & `lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,7 +96,13 @@
           TypeError: If the reader is neither a string nor a subclass of BasePydanticReader.
           ValueError: If the specified reader string does not correspond to a known reader.
           AttributeError: If there is an issue importing the specified reader.
         """
         from .reader import get_llama_index_reader
 
         return get_llama_index_reader(*args, **kwargs)
+
+    @staticmethod
+    def index(nodes, **kwargs):
+        from .index import LlamaIndex
+
+        return LlamaIndex.index(nodes, **kwargs)
```

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/llama_pack.py` & `lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/llama_pack.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/node_parser.py` & `lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/node_parser.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/reader.py` & `lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/reader.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/llamaindex_/textnode.py` & `lionagi-0.2.0/lionagi/integrations/bridge/llamaindex_/textnode.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/bridge/transformers_/install_.py` & `lionagi-0.2.0/lionagi/integrations/bridge/transformers_/install_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/config/openrouter_configs.py` & `lionagi-0.2.0/lionagi/integrations/config/openrouter_configs.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
+API_key_schema = ("OPENROUTER_API_KEY",)
+
 openrouter_chat_llmconfig = {
-    "model": "gpt-4-turbo",
+    "model": "gpt-4o",
     "frequency_penalty": 0,
     "max_tokens": None,
     "num": 1,
     "presence_penalty": 0,
     "response_format": {"type": "text"},
     "seed": None,
     "stop": None,
     "stream": False,
-    "temperature": 0.7,
+    "temperature": 0.1,
     "top_p": 1,
     "tools": None,
     "tool_choice": "none",
     "user": None,
+    "logprobs": False,
+    "top_logprobs": None,
 }
 
 openrouter_chat_schema = {
     "required": [
         "model",
         "frequency_penalty",
         "num",
@@ -29,17 +33,24 @@
         "seed",
         "stop",
         "stream",
         "tools",
         "tool_choice",
         "user",
         "max_tokens",
+        "logprobs",
+        "top_logprobs",
     ],
     "input_": "messages",
     "config": openrouter_chat_llmconfig,
+    "token_encoding_name": "cl100k_base",
+    "token_limit": 128_000,
+    "interval_tokens": 10_000,
+    "interval_requests": 100,
+    "interval": 60,
 }
 
 openrouter_finetune_llmconfig = {
     "model": "gpt-3.5-turbo",
     "hyperparameters": {
         "batch_size": "auto",
         "learning_rate_multiplier": "auto",
@@ -55,8 +66,9 @@
     "input_": ["training_file"],
     "config": openrouter_finetune_llmconfig,
 }
 
 openrouter_schema = {
     "chat/completions": openrouter_chat_schema,
     "finetune": openrouter_finetune_schema,
+    "API_key_schema": API_key_schema,
 }
```

### Comparing `lionagi-0.1.2/lionagi/integrations/loader/load_util.py` & `lionagi-0.2.0/lionagi/integrations/loader/load_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # use utils and schema
-import math
 from enum import Enum
 from pathlib import Path
 from typing import List, Union, Dict, Any, Tuple
 
 from lionagi.libs import convert, func_call
+from lionagi.libs.ln_tokenize import TokenizeUtil
 from lionagi.core.generic import Node
 
 
 class ReaderType(str, Enum):
     PLAIN = "plain"
     LANGCHAIN = "langchain"
     LLAMAINDEX = "llama_index"
@@ -53,15 +53,15 @@
             func_call.lcall(ext, _dir_to_path, flatten=True), flatten=flatten
         )
     except:
         raise ValueError("Invalid directory or extension, please check the path")
 
 
 def dir_to_nodes(
-    dir: str,
+    dir_: str,
     ext: Union[List[str], str],
     recursive: bool = False,
     flatten: bool = True,
     clean_text: bool = True,
 ) -> List[Node]:
     """
     Converts directory contents into Node objects based on specified file extensions.
@@ -80,90 +80,19 @@
 
     Example:
         nodes = dir_to_nodes("/path/to/dir", ".txt", recursive=True)
         # This would read all .txt files in /path/to/dir and its subdirectories,
         # converting them into Node objects.
     """
 
-    path_list = dir_to_path(dir, ext, recursive, flatten)
+    path_list = dir_to_path(dir=dir_, ext=ext, recursive=recursive, flatten=flatten)
     files_info = func_call.lcall(path_list, read_text, clean=clean_text)
     return func_call.lcall(files_info, lambda x: Node(content=x[0], metadata=x[1]))
 
 
-def chunk_text(
-    input: str, chunk_size: int, overlap: float, threshold: int
-) -> List[Union[str, None]]:
-    """
-    Chunks the input text into smaller parts, with optional overlap and threshold for final chunk.
-
-    Parameters:
-        input (str): The input text to chunk.
-
-        chunk_size (int): The size of each chunk.
-
-        overlap (float): The amount of overlap between chunks.
-
-        threshold (int): The minimum size of the final chunk.
-
-    Returns:
-        List[Union[str, None]]: A list of text chunks.
-
-    Raises:
-        ValueError: If an error occurs during chunking.
-    """
-
-    def _chunk_n1():
-        return [input]
-
-    def _chunk_n2():
-        chunks = []
-        chunks.append(input[: chunk_size + overlap_size])
-
-        if len(input) - chunk_size > threshold:
-            chunks.append(input[chunk_size - overlap_size :])
-        else:
-            return _chunk_n1()
-
-        return chunks
-
-    def _chunk_n3():
-        chunks = []
-        chunks.append(input[: chunk_size + overlap_size])
-        for i in range(1, n_chunks - 1):
-            start_idx = chunk_size * i - overlap_size
-            end_idx = chunk_size * (i + 1) + overlap_size
-            chunks.append(input[start_idx:end_idx])
-
-        if len(input) - chunk_size * (n_chunks - 1) > threshold:
-            chunks.append(input[chunk_size * (n_chunks - 1) - overlap_size :])
-        else:
-            chunks[-1] += input[chunk_size * (n_chunks - 1) + overlap_size :]
-
-        return chunks
-
-    try:
-        if not isinstance(input, str):
-            input = convert.to_str(input)
-
-        n_chunks = math.ceil(len(input) / chunk_size)
-        overlap_size = int(overlap / 2)
-
-        if n_chunks == 1:
-            return _chunk_n1()
-
-        elif n_chunks == 2:
-            return _chunk_n2()
-
-        elif n_chunks > 2:
-            return _chunk_n3()
-
-    except Exception as e:
-        raise ValueError(f"An error occurred while chunking the text. {e}")
-
-
 def read_text(filepath: str, clean: bool = True) -> Tuple[str, dict]:
     """
     Reads text from a file and optionally cleans it, returning the content and metadata.
 
     Parameters:
         filepath (str): The path to the file to read.
 
@@ -198,17 +127,17 @@
         }
 
     try:
         with open(filepath, "r") as f:
             content = f.read()
             if clean:
                 # Define characters to replace and their replacements
-                replacements = {"\\": " ", "\n": " ", "\t": " ", "  ": " ", "'": " "}
+                replacements = {"\\": "", "\n\n": "\n"}
                 for old, new in replacements.items():
-                    content = content.replace(old, new)
+                    content = content.replace(old, new).strip()
             metadata = _get_metadata()
             return content, metadata
     except Exception as e:
         raise e
 
 
 def _file_to_chunks(
@@ -219,15 +148,15 @@
     threshold: int = 200,
 ) -> List[Dict[str, Any]]:
     try:
         out = {key: value for key, value in input.items() if key != field} | {
             "chunk_overlap": overlap,
             "chunk_threshold": threshold,
         }
-        chunks = chunk_text(
+        chunks = TokenizeUtil.chunk_by_chars(
             input[field], chunk_size=chunk_size, overlap=overlap, threshold=threshold
         )
         logs = []
         for i, chunk in enumerate(chunks):
             chunk_dict = out | {
                 "file_chunks": len(chunks),
                 "chunk_id": i + 1,
```

### Comparing `lionagi-0.1.2/lionagi/integrations/provider/litellm.py` & `lionagi-0.2.0/lionagi/integrations/provider/litellm.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,21 @@
         SysUtil.check_import("litellm")
 
         from litellm import acompletion
 
         self.acompletion = acompletion
         self.model = model
         self.kwargs = kwargs
+        self.allowed_kwargs = allowed_kwargs
 
     async def serve_chat(self, messages, **kwargs):
         payload = {"messages": messages}
         config = {}
         for k, v in kwargs.items():
-            if k in allowed_kwargs:
+            if k in self.allowed_kwargs:
                 config[k] = v
 
         kwargs = {**self.kwargs, **config}
 
         try:
             completion = await self.acompletion(
                 model=self.model, messages=messages, **kwargs
```

### Comparing `lionagi-0.1.2/lionagi/integrations/provider/mlx_service.py` & `lionagi-0.2.0/lionagi/integrations/provider/mlx_service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,54 @@
+import re
 from lionagi.libs.sys_util import SysUtil
 import lionagi.libs.ln_convert as convert
 from lionagi.libs.ln_api import BaseService
 from lionagi.integrations.config.mlx_configs import model
 
 
-class MlXService(BaseService):
+class MLXService(BaseService):
     def __init__(self, model=model, **kwargs):
 
         SysUtil.check_import("mlx_lm")
+        SysUtil.check_import("ipywidgets")
+
+        if model is not None and "olmo" in str(model).lower():
+            SysUtil.check_import("olmo", pip_name="ai2-olmo")
 
         from mlx_lm import load, generate
 
         super().__init__()
 
         model_, tokenizer = load(model, **kwargs)
 
         self.model_name = model
         self.model = model_
         self.tokenizer = tokenizer
         self.generate = generate
+        self.allowed_kwargs = []
 
     async def serve_chat(self, messages, **kwargs):
         if "verbose" not in kwargs.keys():
-            verbose = True
+            verbose = False
 
-        prompts = [
-            convert.to_dict(msg["content"])["instruction"]
-            for msg in messages
-            if msg["role"] == "user"
-        ]
+        prompts = [msg["content"] for msg in messages if msg["role"] == "user"]
 
         payload = {"messages": messages}
 
         try:
             response = self.generate(
                 self.model,
                 self.tokenizer,
                 prompt=f"{prompts[-1]} \nOutput: ",
                 verbose=verbose,
             )
-            completion = {"model": self.model_name, "choices": [{"message": response}]}
-
+            if "```" in response:
+                regex = re.compile(r"```[\s\S]*?```")
+                matches = regex.findall(response)
+                msg = matches[0].strip("```")
+                completion = {"choices": [{"message": {"content": msg}}]}
+            else:
+                completion = {"choices": [{"message": {"content": response}}]}
             return payload, completion
         except Exception as e:
             self.status_tracker.num_tasks_failed += 1
             raise e
```

### Comparing `lionagi-0.1.2/lionagi/integrations/provider/ollama.py` & `lionagi-0.2.0/lionagi/integrations/provider/ollama.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from lionagi.libs.ln_api import BaseService
 from lionagi.integrations.config.ollama_configs import model
 
 allowed_kwargs = [
     "model",
     "frequency_penalty",
-    "max_tokens",
+    # "max_tokens",
     "n",
     "presence_penalty",
     "response_format",
     "seed",
     "stop",
     "stream",
     # "temperature",
@@ -28,27 +28,28 @@
 
         SysUtil.check_import("ollama")
 
         import ollama
 
         self.ollama = ollama
         self.model = model
-        self.client = self.ollama.AsyncClient(**kwargs)
+        self.client = self.ollama.AsyncClient()
+        self.allowed_kwargs = allowed_kwargs
 
     async def serve_chat(self, messages, **kwargs):
         config = {}
         for k, v in kwargs.items():
             if k in allowed_kwargs:
                 config[k] = v
 
         self.ollama.pull(self.model)
         payload = {"messages": messages}
+        if "model" not in config:
+            config["model"] = self.model
 
         try:
-            completion = await self.client.chat(
-                model=self.model, messages=messages, **config
-            )
+            completion = await self.client.chat(messages=messages, **config)
             completion["choices"] = [{"message": completion.pop("message")}]
             return payload, completion
         except Exception as e:
             self.status_tracker.num_tasks_failed += 1
             raise e
```

### Comparing `lionagi-0.1.2/lionagi/integrations/provider/services.py` & `lionagi-0.2.0/lionagi/integrations/provider/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,10 +127,10 @@
         A provider to interact with MlX
 
         Attributes:
                 model (str): name of the model to use
                 kwargs (Optional[Any]): additional kwargs for calling the model
         """
 
-        from lionagi.integrations.provider.mlx_service import MlXService
+        from lionagi.integrations.provider.mlx_service import MLXService
 
-        return MlXService(**kwargs)
+        return MLXService(**kwargs)
```

### Comparing `lionagi-0.1.2/lionagi/integrations/provider/transformers.py` & `lionagi-0.2.0/lionagi/integrations/provider/transformers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from typing import Union, Dict, Any
 import subprocess
 
 from lionagi.libs.sys_util import SysUtil
 from lionagi.libs.ln_api import BaseService
 
 allowed_kwargs = [
-    "model",
+    # "model",
     "tokenizer",
     "modelcard",
     "framework",
     "task",
     "num_workers",
     "batch_size",
     "args_parser",
     "device",
     "torch_dtype",
     "min_length_for_response",
     "minimum_tokens",
+    "mask_token",
+    "max_length",
+    "max_new_tokens",
 ]
 
 
 def get_pytorch_install_command():
     cpu_arch = SysUtil.get_cpu_architecture()
 
     if cpu_arch == "apple_silicon":
@@ -48,34 +51,27 @@
         device="cpu",
         **kwargs,
     ):
         super().__init__()
         self.task = task
         self.model = model
         self.config = config
+        self.allowed_kwargs = allowed_kwargs
         try:
             from transformers import pipeline
 
             self.pipeline = pipeline
         except ImportError:
             try:
                 if not SysUtil.is_package_installed("torch"):
-                    in_ = input(
-                        "PyTorch is required for transformers. Would you like to install it now? (y/n): "
-                    )
-                    if in_ == "y":
-                        install_pytorch()
+                    install_pytorch()
                 if not SysUtil.is_package_installed("transformers"):
-                    in_ = input(
-                        "transformers is required. Would you like to install it now? (y/n): "
+                    SysUtil.install_import(
+                        package_name="transformers", import_name="pipeline"
                     )
-                    if in_ == "y":
-                        SysUtil.install_import(
-                            package_name="transformers", import_name="pipeline"
-                        )
                     from transformers import pipeline
 
                     self.pipeline = pipeline
             except Exception as e:
                 raise ImportError(
                     f"Unable to import required module from transformers. Please make sure that transformers is installed. Error: {e}"
                 )
@@ -88,23 +84,23 @@
         if self.task:
             if self.task != "conversational":
                 raise ValueError(f"Invalid transformers pipeline task: {self.task}.")
 
         payload = {"messages": messages}
         config = {}
         for k, v in kwargs.items():
+            if k == "max_tokens":
+                config["max_new_tokens"] = v
             if k in allowed_kwargs:
                 config[k] = v
 
-        conversation = self.pipe(str(messages), **config)
-
-        texts = conversation[-1]["generated_text"]
-        msgs = (
-            str(texts.split("]")[1:])
-            .replace("\\n", "")
-            .replace("['", "")
-            .replace("\\", "")
-        )
+        msg = "".join([i["content"] for i in messages if i["role"] == "user"])
+        conversation = ""
+        response = self.pipe(msg, **config)
+        try:
+            conversation = response[0]["generated_text"]
+        except:
+            conversation = response
 
-        completion = {"model": self.pipe.model, "choices": [{"message": msgs}]}
+        completion = {"choices": [{"message": {"content": conversation}}]}
 
         return payload, completion
```

### Comparing `lionagi-0.1.2/lionagi/integrations/storage/neo4j.py` & `lionagi-0.2.0/lionagi/integrations/storage/neo4j.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,194 +33,186 @@
     @staticmethod
     async def add_structure_node(tx, node, name):
         """
         Asynchronously adds a structure node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the node to be added, including 'id' and 'timestamp'.
+            node (dict): The properties of the node to be added, including 'ln_id' and 'timestamp'.
             name (str): The name of the structure, which is set on the node.
         """
         query = """
-            MERGE (n:Structure:LionNode {id:$id})
+            MERGE (n:Structure:LionNode {ln_id:$ln_id})
             SET n.timestamp = $timestamp
             SET n.name = $name
             """
-        await tx.run(query, id=node["id"], timestamp=node["timestamp"], name=name)
+        await tx.run(query, ln_id=node["ln_id"], timestamp=node["timestamp"], name=name)
         # heads=node['head_nodes'],
         # nodes=node['nodes'],
         # edges=node['edges'])
 
     @staticmethod
     async def add_system_node(tx, node):
         """
         Asynchronously adds a system node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the system node including 'id', 'timestamp', 'content', 'sender', and 'recipient'.
+            node (dict): The properties of the system node including 'ln_id', 'timestamp', 'content', 'sender', and 'recipient'.
         """
         query = """
-            MERGE (n:System:LionNode {id: $id})
+            MERGE (n:System:LionNode {ln_id: $ln_id})
             SET n.timestamp = $timestamp
             SET n.content = $content
-            SET n.sender = $sender
-            SET n.recipient = $recipient
             """
         await tx.run(
             query,
-            id=node["id"],
+            ln_id=node["ln_id"],
             timestamp=node["timestamp"],
             content=node["content"],
-            sender=node["sender"],
-            recipient=node["recipient"],
         )
 
     @staticmethod
     async def add_instruction_node(tx, node):
         """
         Asynchronously adds an instruction node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the instruction node including 'id', 'timestamp', 'content', 'sender', and 'recipient'.
+            node (dict): The properties of the instruction node including 'ln_id', 'timestamp', 'content', 'sender', and 'recipient'.
         """
         query = """
-            MERGE (n:Instruction:LionNode {id: $id})
+            MERGE (n:Instruction:LionNode {ln_id: $ln_id})
             SET n.timestamp = $timestamp
             SET n.content = $content
-            SET n.sender = $sender
-            SET n.recipient = $recipient
             """
         await tx.run(
             query,
-            id=node["id"],
+            ln_id=node["ln_id"],
             timestamp=node["timestamp"],
             content=node["content"],
-            sender=node["sender"],
-            recipient=node["recipient"],
         )
 
     # TODO: tool.manual
     @staticmethod
     async def add_tool_node(tx, node):
         """
         Asynchronously adds a tool node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the tool node including 'id', 'timestamp', 'function', and 'parser'.
+            node (dict): The properties of the tool node including 'ln_id', 'timestamp', 'function', and 'parser'.
         """
         query = """
-            MERGE (n:Tool:LionNode {id: $id})
+            MERGE (n:Tool:LionNode {ln_id: $ln_id})
             SET n.timestamp = $timestamp
             SET n.function = $function
             SET n.parser = $parser
             """
         await tx.run(
             query,
-            id=node["id"],
+            ln_id=node["ln_id"],
             timestamp=node["timestamp"],
             function=node["function"],
             parser=node["parser"],
         )
 
     @staticmethod
-    async def add_actionSelection_node(tx, node):
+    async def add_directiveSelection_node(tx, node):
         """
-        Asynchronously adds an action selection node to the graph.
+        Asynchronously adds an directive selection node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the action selection node including 'id', 'action', and 'actionKwargs'.
+            node (dict): The properties of the directive selection node including 'ln_id', 'directive', and 'directiveKwargs'.
         """
         query = """
-            MERGE (n:ActionSelection:LionNode {id: $id})
-            SET n.action = $action
-            SET n.actionKwargs = $actionKwargs
+            MERGE (n:DirectiveSelection:LionNode {ln_id: $ln_id})
+            SET n.directive = $directive
+            SET n.directiveKwargs = $directiveKwargs
             """
         await tx.run(
             query,
-            id=node["id"],
-            action=node["action"],
-            actionKwargs=node["action_kwargs"],
+            ln_id=node["ln_id"],
+            directive=node["directive"],
+            directiveKwargs=node["directive_kwargs"],
         )
 
     @staticmethod
     async def add_baseAgent_node(tx, node):
         """
         Asynchronously adds an agent node to the graph.
 
         Args:
             tx: The Neo4j transaction.
-            node (dict): The properties of the agent node including 'id', 'timestamp', 'structureId', and 'outputParser'.
+            node (dict): The properties of the agent node including 'ln_id', 'timestamp', 'structureId', and 'outputParser'.
         """
         query = """
-            MERGE (n:Agent:LionNode {id:$id})
+            MERGE (n:Agent:LionNode {ln_id:$ln_id})
             SET n.timestamp = $timestamp
             SET n.structureId = $structureId
             SET n.outputParser = $outputParser
             """
         await tx.run(
             query,
-            id=node["id"],
+            ln_id=node["ln_id"],
             timestamp=node["timestamp"],
             structureId=node["structure_id"],
             outputParser=node["output_parser"],
         )
 
     @staticmethod
     async def add_forward_edge(tx, edge):
         """
         Asynchronously adds a forward relationship between two nodes in the graph.
 
         Args:
             tx: The Neo4j transaction.
-            edge (dict): The properties of the edge including 'id', 'timestamp', 'head', 'tail', 'label', and 'condition'.
+            edge (dict): The properties of the edge including 'ln_id', 'timestamp', 'head', 'tail', 'label', and 'condition'.
         """
         query = """
-            MATCH (m:LionNode) WHERE m.id = $head
-            MATCH (n:LionNode) WHERE n.id = $tail
+            MATCH (m:LionNode) WHERE m.ln_id = $head
+            MATCH (n:LionNode) WHERE n.ln_id = $tail
             MERGE (m)-[r:FORWARD]->(n)
-            SET r.id = $id
+            SET r.ln_id = $ln_id
             SET r.timestamp = $timestamp
             SET r.label = $label
             SET r.condition = $condition
             """
         await tx.run(
             query,
-            id=edge["id"],
+            ln_id=edge["ln_id"],
             timestamp=edge["timestamp"],
             head=edge["head"],
             tail=edge["tail"],
             label=edge["label"],
             condition=edge["condition"],
         )
 
     @staticmethod
     async def add_bundle_edge(tx, edge):
         """
         Asynchronously adds a bundle relationship between two nodes in the graph.
 
         Args:
             tx: The Neo4j transaction.
-            edge (dict): The properties of the edge including 'id', 'timestamp', 'head', 'tail', 'label', and 'condition'.
+            edge (dict): The properties of the edge including 'ln_id', 'timestamp', 'head', 'tail', 'label', and 'condition'.
         """
         query = """
-            MATCH (m:LionNode) WHERE m.id = $head
-            MATCH (n:LionNode) WHERE n.id = $tail
+            MATCH (m:LionNode) WHERE m.ln_id = $head
+            MATCH (n:LionNode) WHERE n.ln_id = $tail
             MERGE (m)-[r:BUNDLE]->(n)
-            SET r.id = $id
+            SET r.ln_id = $ln_id
             SET r.timestamp = $timestamp
             SET r.label = $label
             SET r.condition = $condition
             """
         await tx.run(
             query,
-            id=edge["id"],
+            ln_id=edge["ln_id"],
             timestamp=edge["timestamp"],
             head=edge["head"],
             tail=edge["tail"],
             label=edge["label"],
             condition=edge["condition"],
         )
 
@@ -230,33 +222,33 @@
         Asynchronously adds head relationships from a structure node to its head nodes.
 
         Args:
             tx: The Neo4j transaction.
             structure: The structure node from which head relationships are established.
         """
         for head in structure.get_heads():
-            head_id = head.id_
+            head_id = head.ln_id
             query = """
-                MATCH (m:Structure) WHERE m.id = $structureId
-                MATCH (n:LionNode) WHERE n.id = $headId
+                MATCH (m:Structure) WHERE m.ln_id = $structureId
+                MATCH (n:LionNode) WHERE n.ln_id = $headId
                 MERGE (m)-[:HEAD]->(n)
                 """
-            await tx.run(query, structureId=structure.id_, headId=head_id)
+            await tx.run(query, structureId=structure.ln_id, headId=head_id)
 
     @staticmethod
     async def add_single_condition_cls(tx, condCls):
         """
         Asynchronously adds a condition class node to the graph.
 
         Args:
             tx: The Neo4j transaction.
             condCls (dict): The properties of the condition class node including 'className' and 'code'.
         """
         query = """
-            MERGE (n:Condition:LionNode {className: $className})
+            MERGE (n:EdgeCondition:LionNode {className: $className})
             SET n.code = $code
             """
         await tx.run(query, className=condCls["class_name"], code=condCls["class"])
 
     async def add_node(self, tx, node_dict, structure_name):
         """
         Asynchronously adds various types of nodes to the Neo4j graph based on the provided dictionary of node lists.
@@ -270,27 +262,27 @@
             structure_name (str): The name of the structure to which these nodes belong, used specifically for 'StructureExecutor' nodes.
 
         Raises:
             ValueError: If an unsupported node type is detected in the dictionary.
         """
         for node in node_dict:
             node_list = node_dict[node]
-            if node == "StructureExecutor":
+            if node == "GraphExecutor":
                 [
                     await self.add_structure_node(tx, i, structure_name)
                     for i in node_list
                 ]
             elif node == "System":
                 [await self.add_system_node(tx, i) for i in node_list]
             elif node == "Instruction":
                 [await self.add_instruction_node(tx, i) for i in node_list]
             elif node == "Tool":
                 [await self.add_tool_node(tx, i) for i in node_list]
-            elif node == "ActionSelection":
-                [await self.add_actionSelection_node(tx, i) for i in node_list]
+            elif node == "DirectiveSelection":
+                [await self.add_directiveSelection_node(tx, i) for i in node_list]
             elif node == "BaseAgent":
                 [await self.add_baseAgent_node(tx, i) for i in node_list]
             else:
                 raise ValueError("Not supported node type detected")
 
     async def add_edge(self, tx, edge_list):
         """
@@ -331,24 +323,24 @@
         """
         for cls in edge_cls_list:
             await self.add_single_condition_cls(tx, cls)
 
     @staticmethod
     async def check_id_constraint(tx):
         """
-        Asynchronously applies a unique constraint on the 'id' attribute for all nodes of type 'LionNode' in the graph.
+        Asynchronously applies a unique constraint on the 'ln_id' attribute for all nodes of type 'LionNode' in the graph.
 
         This constraint ensures that each node in the graph has a unique identifier.
 
         Args:
             tx: The Neo4j transaction.
         """
         query = """
             CREATE CONSTRAINT node_id IF NOT EXISTS
-            FOR (n:LionNode) REQUIRE (n.id) IS UNIQUE
+            FOR (n:LionNode) REQUIRE (n.ln_id) IS UNIQUE
             """
         await tx.run(query)
 
     @staticmethod
     async def check_structure_name_constraint(tx):
         """
         Asynchronously applies a unique constraint on the 'name' attribute for all nodes of type 'Structure' in the graph.
@@ -417,18 +409,18 @@
             tx: The Neo4j transaction.
             node_id (str): The unique identifier of the node to retrieve.
 
         Returns:
             A dictionary containing the properties of the node if found, otherwise None.
         """
         query = """
-            MATCH (n:LionNode) WHERE n.id = $id
+            MATCH (n:LionNode) WHERE n.ln_id = $ln_id
             RETURN labels(n), n{.*}
             """
-        result = await tx.run(query, id=node_id)
+        result = await tx.run(query, ln_id=node_id)
         result = [record.values() async for record in result]
         if result:
             return result[0]
         else:
             return None
 
     @staticmethod
@@ -441,15 +433,15 @@
             name (str): The name of the structure to retrieve the identifier for.
 
         Returns:
             A list containing the identifier(s) of the matching structure(s).
         """
         query = """
             MATCH (n:Structure) WHERE n.name = $name
-            RETURN n.id
+            RETURN n.ln_id
             """
         result = await tx.run(query, name=name)
         result = [record.values() async for record in result]
         result = sum(result, [])
         return result
 
     @staticmethod
@@ -461,15 +453,15 @@
             tx: The Neo4j transaction.
             node_id (str): The identifier of the structure node whose head nodes are to be retrieved.
 
         Returns:
             A list of dictionaries representing the properties and labels of each head node connected to the structure.
         """
         query = """
-            MATCH (n:Structure)-[r:HEAD]->(m) WHERE n.id = $nodeId
+            MATCH (n:Structure)-[r:HEAD]->(m) WHERE n.ln_id = $nodeId
             RETURN r{.*}, labels(m), m{.*}
             """
         result = await tx.run(query, nodeId=node_id)
         result = [record.values() async for record in result]
         return result
 
     @staticmethod
@@ -481,15 +473,15 @@
             tx: The Neo4j transaction.
             node_id (str): The identifier of the node from which to retrieve forward relationships.
 
         Returns:
             A list of dictionaries representing the properties and labels of each node connected by a forward relationship.
         """
         query = """
-            MATCH (n:LionNode)-[r:FORWARD]->(m) WHERE n.id = $nodeId
+            MATCH (n:LionNode)-[r:FORWARD]->(m) WHERE n.ln_id = $nodeId
             RETURN r{.*}, labels(m), m{.*}
             """
         result = await tx.run(query, nodeId=node_id)
         result = [record.values() async for record in result]
         return result
 
     @staticmethod
@@ -501,15 +493,15 @@
             tx: The Neo4j transaction.
             node_id (str): The identifier of the node from which to retrieve bundle relationships.
 
         Returns:
             A list of dictionaries representing the properties and labels of each node connected by a bundle relationship.
         """
         query = """
-            MATCH (n:LionNode)-[r:BUNDLE]->(m) WHERE n.id = $nodeId
+            MATCH (n:LionNode)-[r:BUNDLE]->(m) WHERE n.ln_id = $nodeId
             RETURN labels(m), m{.*}
             """
         result = await tx.run(query, nodeId=node_id)
         result = [record.values() async for record in result]
         return result
 
     @staticmethod
@@ -521,15 +513,15 @@
             tx: The Neo4j transaction.
             name (str): The class name of the condition to retrieve the code for.
 
         Returns:
             The code of the condition class if found, otherwise None.
         """
         query = """
-            MATCH (n:Condition) WHERE n.className = $name
+            MATCH (n:EdgeCondition) WHERE n.className = $name
             RETURN n.code
             """
         result = await tx.run(query, name=name)
         result = [record.values() async for record in result]
         if result:
             return result[0][0]
         else:
@@ -553,15 +545,15 @@
             str: The identifier of the located structure.
 
         Raises:
             ValueError: If neither structure name nor ID is provided, or if the provided name or ID does not correspond
                 to any existing structure.
         """
         if not structure_name and not structure_id:
-            raise ValueError("Please provide the structure name or id")
+            raise ValueError("Please provide the structure name or ln_id")
         if structure_name:
             id = await self.match_structure_id(tx, structure_name)
             if not id:
                 raise ValueError(f"Structure: {structure_name} is not found")
             elif structure_id is not None and structure_id not in id:
                 raise ValueError(
                     f"{structure_name} and id {structure_id} does not match"
```

### Comparing `lionagi-0.1.2/lionagi/integrations/storage/storage_util.py` & `lionagi-0.2.0/lionagi/integrations/storage/storage_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import json
 import inspect
 import re
 
-from lionagi.core import System, Instruction
-from lionagi.core.tool import Tool
-from lionagi.core.generic.action import ActionSelection
+from lionagi.core.message import System, Instruction, RoledMessage
+from lionagi.core.action import Tool, DirectiveSelection, func_to_tool
+from lionagi.core.action import DirectiveSelection
 from lionagi.core.agent.base_agent import BaseAgent
-from lionagi.core.generic.condition import Condition
-
-from lionagi.core import func_to_tool
+from lionagi.core.generic.edge_condition import EdgeCondition
 
 
 def output_node_list(structure):
     """
     Processes a structure object to extract and format all associated nodes into a summary list and detailed output dictionary.
 
     This function traverses a structure, extracting key properties of nodes and organizing them by type into a dictionary for easy access and manipulation.
@@ -23,46 +21,50 @@
     Returns:
         tuple: A tuple containing a summary list of all nodes and a dictionary categorizing nodes by type.
     """
     summary_list = []
     output = {}
 
     structure_output = {
-        "id": structure.id_,
+        "ln_id": structure.ln_id,
         "timestamp": structure.timestamp,
         "type": structure.class_name,
     }
     summary_list.append(structure_output.copy())
-    structure_output["head_nodes"] = json.dumps([i.id_ for i in structure.get_heads()])
+    structure_output["head_nodes"] = json.dumps(
+        [i.ln_id for i in structure.get_heads()]
+    )
     # structure_output['nodes'] = json.dumps([i for i in structure.internal_nodes.keys()])
     # structure_output['edges'] = json.dumps([i for i in structure.internal_edges.keys()])
     output[structure_output["type"]] = [structure_output]
     for node in structure.internal_nodes.values():
         node_output = {
-            "id": node.id_,
+            "ln_id": node.ln_id,
             "timestamp": node.timestamp,
             "type": node.class_name,
         }
         summary_list.append(node_output.copy())
         if isinstance(node, System) or isinstance(node, Instruction):
             node_output["content"] = json.dumps(node.content)
-            node_output["sender"] = node.sender
-            node_output["recipient"] = node.recipient
+            # node_output["sender"] = node.sender
+            # node_output["recipient"] = node.recipient
         elif isinstance(node, Tool):
-            node_output["function"] = inspect.getsource(node.func)
+            node_output["function"] = inspect.getsource(node.function)
             # node_output['manual'] = node.manual
             node_output["parser"] = (
                 inspect.getsource(node.parser) if node.parser else None
             )
-        elif isinstance(node, ActionSelection):
-            node_output["action"] = node.action
-            node_output["action_kwargs"] = json.dumps(node.action_kwargs)
+        elif isinstance(node, DirectiveSelection):
+            node_output["directive"] = node.directive
+            node_output["directive_kwargs"] = json.dumps(node.directive_kwargs)
         elif isinstance(node, BaseAgent):
-            node_output["structure_id"] = node.structure.id_
-            node_output["output_parser"] = inspect.getsource(node.output_parser)
+            node_output["structure_id"] = node.structure.ln_id
+            node_output["output_parser"] = (
+                inspect.getsource(node.output_parser) if node.output_parser else None
+            )
         else:
             raise ValueError("Not supported node type detected")
         if node_output["type"] not in output:
             output[node_output["type"]] = []
         output[node_output["type"]].append(node_output)
 
     return summary_list, output
@@ -80,15 +82,15 @@
     Returns:
         tuple: A tuple containing a list of all edges with their details and a list of unique condition classes.
     """
     edge_list = []
     edge_cls_dict = {}
     for edge in structure.internal_edges.values():
         edge_output = {
-            "id": edge.id_,
+            "ln_id": edge.ln_id,
             "timestamp": edge.timestamp,
             "head": edge.head,
             "tail": edge.tail,
             "label": edge.label,
             "bundle": str(edge.bundle),
         }
         if edge.condition:
@@ -179,61 +181,52 @@
 
         Args:
             info_dict (dict): A dictionary containing properties of a system node.
 
         Returns:
             System: An instantiated System node filled with properties from info_dict.
         """
-        node = System(" ")
-        node.id_ = info_dict["id"]
-        node.timestamp = info_dict["timestamp"]
-        node.content = json.loads(info_dict["content"])
-        node.sender = info_dict["sender"]
-        node.recipient = info_dict["recipient"]
+        info_dict["system"] = json.loads(info_dict.pop("content"))["system_info"]
+        node = System.from_obj(info_dict)
         return node
 
     @staticmethod
     def parse_instruction(info_dict):
         """
         Parses dictionary information into an Instruction node object.
 
         Args:
             info_dict (dict): A dictionary containing properties of an instruction node.
 
         Returns:
             Instruction: An instantiated Instruction node filled with properties from info_dict.
         """
-        node = Instruction(" ")
-        node.id_ = info_dict["id"]
-        node.timestamp = info_dict["timestamp"]
-        node.content = json.loads(info_dict["content"])
-        node.sender = info_dict["sender"]
-        node.recipient = info_dict["recipient"]
+        info_dict["instruction"] = json.loads(info_dict.pop("content"))["instruction"]
+        node = Instruction.from_obj(info_dict)
         return node
 
     @staticmethod
-    def parse_actionSelection(info_dict):
+    def parse_directiveSelection(info_dict):
         """
-        Parses dictionary information into an ActionSelection node object.
+        Parses dictionary information into an DirectiveSelection node object.
 
         Args:
             info_dict (dict): A dictionary containing properties of an action selection node.
 
         Returns:
             ActionSelection: An instantiated ActionSelection node filled with properties from info_dict.
         """
-        node = ActionSelection()
-        node.id_ = info_dict["id"]
-        node.action = info_dict["action"]
-        if "action_kwargs" in info_dict:
-            if info_dict["action_kwargs"]:
-                node.action_kwargs = json.loads(info_dict["action_kwargs"])
-        elif "actionKwargs" in info_dict:
-            if info_dict["actionKwargs"]:
-                node.action_kwargs = json.loads(info_dict["actionKwargs"])
+        node = DirectiveSelection(ln_id=info_dict["ln_id"])
+        node.directive = info_dict["directive"]
+        if "directive_kwargs" in info_dict:
+            if info_dict["directive_kwargs"]:
+                node.directive_kwargs = json.loads(info_dict["directive_kwargs"])
+        elif "directiveKwargs" in info_dict:
+            if info_dict["directiveKwargs"]:
+                node.directive_kwargs = json.loads(info_dict["directiveKwargs"])
         return node
 
     @staticmethod
     def parse_tool(info_dict):
         """
         Parses dictionary information into a Tool node object, converting associated function code into a callable.
 
@@ -249,22 +242,27 @@
         func_code = info_dict["function"]
         if "import os" in func_code or "__" in func_code or "import sys" in func_code:
             raise ValueError(
                 "Unsafe code detected in Tool function. Please double check or implement explicitly"
             )
 
         func = ParseNode.convert_to_def(func_code)
-        tool = func_to_tool(func)
+        tool = func_to_tool(
+            func, ln_id=info_dict["ln_id"], timestamp=info_dict["timestamp"]
+        )
         if func.__doc__:
             if re.search(r":param \w+:", func.__doc__):
-                tool = func_to_tool(func, docstring_style="reST")
+                tool = func_to_tool(
+                    func,
+                    docstring_style="reST",
+                    ln_id=info_dict["ln_id"],
+                    timestamp=info_dict["timestamp"],
+                )
 
         tool = tool[0]
-        tool.id_ = info_dict["id"]
-        tool.timestamp = info_dict["timestamp"]
         return tool
 
     @staticmethod
     def parse_condition(condition, cls_code):
         """
         Parses a condition dictionary and corresponding class code into a class instance representing the condition.
 
@@ -282,8 +280,8 @@
         cls = ParseNode.convert_to_class(cls_code)
 
         init_params = {}
         for key in inspect.signature(cls.__init__).parameters.keys():
             if key == "self":
                 continue
             init_params[key] = args[key]
-        return cls(**init_params)
+        return cls(**init_params)
```

### Comparing `lionagi-0.1.2/lionagi/integrations/storage/structure_excel.py` & `lionagi-0.2.0/lionagi/integrations/storage/structure_excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pandas as pd
 import json
 from pathlib import Path
 
 from lionagi.integrations.storage.storage_util import ParseNode
-from lionagi.core.execute.structure_executor import StructureExecutor
+from lionagi.core.executor.graph_executor import GraphExecutor
 from lionagi.core.agent.base_agent import BaseAgent
-from lionagi.core.execute.base_executor import BaseExecutor
-from lionagi.core.execute.instruction_map_executor import InstructionMapExecutor
+from lionagi.core.executor.base_executor import BaseExecutor
+from lionagi.core.engine.instruction_map_engine import InstructionMapEngine
 
 
 def excel_reload(structure_name=None, structure_id=None, dir="structure_storage"):
     """
     Loads a structure from an Excel file into a StructureExecutor instance.
 
     This function uses the StructureExcel class to handle the reloading process. It identifies the
@@ -48,18 +48,21 @@
         get_heads(): Retrieves the head nodes of the loaded structure.
         parse_node(info_dict): Parses a node from the structure based on the provided dictionary.
         get_next(node_id): Gets the next nodes connected by outgoing edges from a given node.
         relate(parent_node, node): Relates two nodes within the structure based on the edge definitions.
         parse(node_list, parent_node=None): Recursively parses nodes and their relationships from the structure.
         reload(): Reloads the structure from the Excel file based on the initially provided parameters.
     """
-    structure: StructureExecutor = StructureExecutor()
-    default_agent_executable: BaseExecutor = InstructionMapExecutor()
 
-    def __init__(self, structure_name=None, structure_id=None, file_path="structure_storage"):
+    structure: GraphExecutor = GraphExecutor()
+    default_agent_executable: BaseExecutor = InstructionMapEngine()
+
+    def __init__(
+        self, structure_name=None, structure_id=None, file_path="structure_storage"
+    ):
         """
         Initializes the StructureExcel class with specified parameters.
 
         This method sets up the paths and reads the Excel file, preparing the internal dataframes used for
         structure parsing.
 
         Args:
@@ -87,39 +90,41 @@
                     name = name.rsplit("_", 1)[0]
                     if name == structure_name:
                         filename.append(file.name)
                 except:
                     continue
             if len(filename) > 1:
                 raise ValueError(
-                    f"Multiple files starting with the same structure name {structure_name} has found, please specify the structure id")
+                    f"Multiple files starting with the same structure name {structure_name} has found, please specify the structure id"
+                )
             self.filename = f"{file_path}/{filename[0]}"
             self.file = pd.read_excel(self.filename, sheet_name=None)
         elif structure_id and not structure_name:
             dir_path = Path(file_path)
             files = list(dir_path.glob(f"*{structure_id}.xlsx"))
             filename = [file.name for file in files]
             if len(filename) > 1:
                 raise ValueError(
-                    f"Multiple files with the same structure id {structure_id} has found, please double check the stored structure")
+                    f"Multiple files with the same structure id {structure_id} has found, please double check the stored structure"
+                )
             self.filename = f"{file_path}/{filename[0]}"
             self.file = pd.read_excel(self.filename, sheet_name=None)
         self.nodes = self.file["Nodes"]
         self.edges = self.file["Edges"]
 
     def get_heads(self):
         """
         Retrieves the list of head node identifiers from the loaded structure data.
 
         This method parses the 'StructureExecutor' sheet in the loaded Excel file to extract the list of head nodes.
 
         Returns:
             list: A list of identifiers for the head nodes in the structure.
         """
-        structure_df = self.file["StructureExecutor"]
+        structure_df = self.file["GraphExecutor"]
         head_list = json.loads(structure_df["head_nodes"].iloc[0])
         return head_list
 
     def _reload_info_dict(self, node_id):
         """
         Retrieves detailed information about a specific node from the Excel file based on its identifier.
 
@@ -128,17 +133,17 @@
 
         Args:
             node_id (str): The identifier of the node to look up.
 
         Returns:
             dict: A dictionary containing the properties and values for the specified node.
         """
-        node_type = self.nodes[self.nodes["id"] == node_id]["type"].iloc[0]
+        node_type = self.nodes[self.nodes["ln_id"] == node_id]["type"].iloc[0]
         node_file = self.file[node_type]
-        row = node_file[node_file["id"] == node_id].iloc[0]
+        row = node_file[node_file["ln_id"] == node_id].iloc[0]
         info_dict = row.to_dict()
         return info_dict
 
     def parse_agent(self, info_dict):
         """
         Parses an agent node from the structure using the agent's specific details provided in a dictionary.
 
@@ -150,20 +155,26 @@
                               and output parser code.
 
         Returns:
             BaseAgent: An initialized agent object.
         """
         output_parser = ParseNode.convert_to_def(info_dict["output_parser"])
 
-        structure_excel = StructureExcel(structure_id=info_dict["structure_id"], file_path=self.file_path)
+        structure_excel = StructureExcel(
+            structure_id=info_dict["structure_id"], file_path=self.file_path
+        )
         structure_excel.reload()
         structure = structure_excel.structure
-        agent = BaseAgent(structure=structure, executable=self.default_agent_executable, output_parser=output_parser)
-        agent.id_ = info_dict["id"]
-        agent.timestamp = info_dict["timestamp"]
+        agent = BaseAgent(
+            structure=structure,
+            executable=self.default_agent_executable,
+            output_parser=output_parser,
+            ln_id=info_dict["ln_id"],
+            timestamp=info_dict["timestamp"],
+        )
         return agent
 
     def parse_node(self, info_dict):
         """
         Parses a node from its dictionary representation into a specific node type like System, Instruction, etc.
 
         This method determines the type of node from the info dictionary and uses the appropriate parsing method
@@ -177,16 +188,16 @@
         """
         if info_dict["type"] == "System":
             return ParseNode.parse_system(info_dict)
         elif info_dict["type"] == "Instruction":
             return ParseNode.parse_instruction(info_dict)
         elif info_dict["type"] == "Tool":
             return ParseNode.parse_tool(info_dict)
-        elif info_dict["type"] == "ActionSelection":
-            return ParseNode.parse_actionSelection(info_dict)
+        elif info_dict["type"] == "DirectiveSelection":
+            return ParseNode.parse_directiveSelection(info_dict)
         elif info_dict["type"] == "BaseAgent":
             return self.parse_agent(info_dict)
 
     def get_next(self, node_id):
         """
         Retrieves the list of identifiers for nodes that are directly connected via outgoing edges from the specified node.
 
@@ -213,27 +224,33 @@
             node (Node): The child node in the relationship.
 
         Raises:
             ValueError: If there are issues with the edge data such as multiple undefined edges.
         """
         if not parent_node:
             return
-        row = self.edges[(self.edges["head"] == parent_node.id_) & (self.edges["tail"] == node.id_)]
+        row = self.edges[
+            (self.edges["head"] == parent_node.ln_id)
+            & (self.edges["tail"] == node.ln_id)
+        ]
         if len(row) > 1:
             raise ValueError(
-                f"currently does not support handle multiple edges between two nodes, Error node: from {parent_node.id_} to {node.id_}")
-        if row['condition'].isna().any():
-            self.structure.relate_nodes(parent_node, node)
+                f"currently does not support handle multiple edges between two nodes, Error node: from {parent_node.ln_id} to {node.ln_id}"
+            )
+        if row["condition"].isna().any():
+            self.structure.add_edge(parent_node, node)
         else:
             cond = json.loads(row["condition"].iloc[0])
             cond_cls = cond["class"]
-            cond_row = self.file["EdgesCondClass"][self.file["EdgesCondClass"]["class_name"] == cond_cls]
+            cond_row = self.file["EdgesCondClass"][
+                self.file["EdgesCondClass"]["class_name"] == cond_cls
+            ]
             cond_code = cond_row["class"].iloc[0]
             condition = ParseNode.parse_condition(cond, cond_code)
-            self.structure.relate_nodes(parent_node, node, condition=condition)
+            self.structure.add_edge(parent_node, node, condition=condition)
 
     def parse(self, node_list, parent_node=None):
         """
         Recursively parses a list of nodes and establishes their interconnections based on the Excel data.
 
         This method processes each node ID in the list, parsing individual nodes and relating them according
         to their connections defined in the Excel file.
@@ -245,24 +262,24 @@
         Raises:
             ValueError: If an error occurs during parsing or relating nodes.
         """
         for node_id in node_list:
             info_dict = self._reload_info_dict(node_id)
             node = self.parse_node(info_dict)
 
-            if node.id_ not in self.structure.internal_nodes:
+            if node.ln_id not in self.structure.internal_nodes:
                 self.structure.add_node(node)
             self.relate(parent_node, node)
 
             next_node_list = self.get_next(node_id)
             self.parse(next_node_list, node)
 
     def reload(self):
         """
         Reloads the entire structure from the Excel file.
 
         This method initializes a new StructureExecutor and uses the Excel data to rebuild the entire structure,
         starting from the head nodes and recursively parsing and connecting all nodes defined within.
         """
-        self.structure = StructureExecutor()
+        self.structure = GraphExecutor()
         heads = self.get_heads()
-        self.parse(heads)
+        self.parse(heads)
```

### Comparing `lionagi-0.1.2/lionagi/integrations/storage/to_csv.py` & `lionagi-0.2.0/lionagi/integrations/storage/to_csv.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/integrations/storage/to_excel.py` & `lionagi-0.2.0/lionagi/integrations/storage/to_excel.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import pandas as pd
 from lionagi.libs import SysUtil
 
 from lionagi.integrations.storage.storage_util import output_node_list, output_edge_list
 
 
-def _output_excel(node_list, node_dict, edge_list, edge_cls_list, structure_name, dir="structure_storage"):
+def _output_excel(
+    node_list,
+    node_dict,
+    edge_list,
+    edge_cls_list,
+    structure_name,
+    dir="structure_storage",
+):
     """
     Writes provided node and edge data into multiple sheets of a single Excel workbook.
 
     This helper function takes lists and dictionaries of nodes and edges, converts them into pandas DataFrames,
     and then writes each DataFrame to a distinct sheet in an Excel workbook. This includes a separate sheet
     for each type of node and edge, as well as edge conditions if they exist.
 
@@ -31,21 +38,22 @@
 
     structure_id = ""
 
     tables = {"Nodes": pd.DataFrame(node_list), "Edges": pd.DataFrame(edge_list)}
     if edge_cls_list:
         tables["EdgesCondClass"] = pd.DataFrame(edge_cls_list)
     for i in node_dict:
-        if i == "StructureExecutor":
+        if i == "GraphExecutor":
             structure_node = node_dict[i][0]
             structure_node["name"] = structure_name
-            structure_id = structure_node["id"]
+            structure_id = structure_node["ln_id"]
         tables[i] = pd.DataFrame(node_dict[i])
 
     import os
+
     filepath = os.path.join(dir, f"{structure_name}_{structure_id}.xlsx")
 
     if not os.path.exists(dir):
         os.makedirs(dir)
 
     with pd.ExcelWriter(filepath) as writer:
         for i in tables:
@@ -69,8 +77,7 @@
     Returns:
         None: This function does not return a value but outputs an Excel workbook with multiple sheets.
     """
     node_list, node_dict = output_node_list(structure)
     edge_list, edge_cls_list = output_edge_list(structure)
 
     _output_excel(node_list, node_dict, edge_list, edge_cls_list, structure_name, dir)
-
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_api.py` & `lionagi-0.2.0/lionagi/libs/ln_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,40 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from collections.abc import Sequence, Mapping
 
 from abc import ABC
 from dataclasses import dataclass
 
+import contextlib
 import logging
 import re
 import asyncio
 import aiohttp
 
 from typing import Any, NoReturn, Type, Callable
 
 from lionagi.libs.ln_async import AsyncUtil
-import lionagi.libs.ln_convert as convert
-import lionagi.libs.ln_nested as nested
+from lionagi.libs.ln_convert import to_dict, strip_lower, to_str
 import lionagi.libs.ln_func_call as func_call
+from lionagi.libs.ln_nested import nget
 
 
 class APIUtil:
     """
     A utility class for assisting with common API usage patterns.
     """
 
@@ -171,15 +188,15 @@
     @staticmethod
     def get_cache_key(url: str, params: Mapping[str, Any] | None) -> str:
         """
         Creates a unique cache key based on the URL and parameters.
         """
         import hashlib
 
-        param_str = convert.to_str(params, sort_keys=True) if params else ""
+        param_str = to_str(params, sort_keys=True) if params else ""
         return hashlib.md5((url + param_str).encode("utf-8")).hexdigest()
 
     @staticmethod
     async def retry_api_call(
         http_session: aiohttp.ClientSession,
         url: str,
         retries: int = 3,
@@ -351,33 +368,56 @@
         Example:
                 >>> rate_limiter = OpenAIRateLimiter(100, 200)
                 >>> payload = {'prompt': 'Translate the following text:', 'max_tokens': 50}
                 >>> rate_limiter.calculate_num_token(payload, 'completions')
                 # Expected token calculation for the given payload and endpoint.
         """
         import tiktoken
+        from .ln_image import ImageUtil
 
+        token_encoding_name = token_encoding_name or "cl100k_base"
         encoding = tiktoken.get_encoding(token_encoding_name)
         if api_endpoint.endswith("completions"):
             max_tokens = payload.get("max_tokens", 15)
             n = payload.get("n", 1)
             completion_tokens = n * max_tokens
-
-            # chat completions
             if api_endpoint.startswith("chat/"):
                 num_tokens = 0
+
                 for message in payload["messages"]:
                     num_tokens += 4  # every message follows <im_start>{role/name}\n{content}<im_end>\n
-                    for key, value in message.items():
-                        num_tokens += len(encoding.encode(value))
-                        if key == "name":  # if there's a name, the role is omitted
-                            num_tokens -= (
-                                1
-                                # role is always required and always 1 token
-                            )
+
+                    _content = message.get("content")
+                    if isinstance(_content, str):
+                        num_tokens += len(encoding.encode(_content))
+
+                    elif isinstance(_content, list):
+                        for item in _content:
+                            if isinstance(item, dict):
+                                if "text" in item:
+                                    num_tokens += len(
+                                        encoding.encode(to_str(item["text"]))
+                                    )
+                                elif "image_url" in item:
+                                    a: str = item["image_url"]["url"]
+                                    if "data:image/jpeg;base64," in a:
+                                        a = a.split("data:image/jpeg;base64,")[
+                                            1
+                                        ].strip()
+                                    num_tokens += ImageUtil.calculate_image_token_usage_from_base64(
+                                        a, item.get("detail", "low")
+                                    )
+                                    num_tokens += (
+                                        20  # for every image we add 20 tokens buffer
+                                    )
+                            elif isinstance(item, str):
+                                num_tokens += len(encoding.encode(item))
+                            else:
+                                num_tokens += len(encoding.encode(str(item)))
+
                 num_tokens += 2  # every reply is primed with <im_start>assistant
                 return num_tokens + completion_tokens
             else:
                 prompt = payload["format_prompt"]
                 if isinstance(prompt, str):  # single format_prompt
                     prompt_tokens = len(encoding.encode(prompt))
                     return prompt_tokens + completion_tokens
@@ -408,15 +448,15 @@
         config = {**config, **kwargs}
         payload = {input_key: input_}
 
         for key in required_:
             payload[key] = config[key]
 
         for key in optional_:
-            if bool(config[key]) and convert.strip_lower(config[key]) != "none":
+            if bool(config[key]) and strip_lower(config[key]) != "none":
                 payload[key] = config[key]
 
         return payload
 
 
 @dataclass
 class StatusTracker:
@@ -523,14 +563,15 @@
         http_session,
         endpoint: str,
         base_url: str,
         api_key: str,
         max_attempts: int = 3,
         method: str = "post",
         payload: Mapping[str, any] = None,
+        required_tokens: int = None,
         **kwargs,
     ) -> Mapping[str, any] | None:
         """
         Makes an API call to the specified endpoint using the provided HTTP session.
 
         Args:
                 http_session: The aiohttp client session to use for the API call.
@@ -548,17 +589,19 @@
         while True:
             if (
                 self.available_request_capacity < 1
                 or self.available_token_capacity < 10
             ):  # Minimum token count
                 await AsyncUtil.sleep(1)  # Wait for capacity
                 continue
-            required_tokens = APIUtil.calculate_num_token(
-                payload, endpoint, self.token_encoding_name, **kwargs
-            )
+
+            if not required_tokens:
+                required_tokens = APIUtil.calculate_num_token(
+                    payload, endpoint, self.token_encoding_name, **kwargs
+                )
 
             if await self.request_permission(required_tokens):
                 request_headers = {"Authorization": f"Bearer {api_key}"}
                 attempts_left = max_attempts
 
                 while attempts_left > 0:
                     try:
@@ -744,15 +787,15 @@
             for ep in endpoint_:
                 if ep not in self.available_endpoints:
                     raise ValueError(
                         f"Endpoint {ep} not available for service {self.__class__.__name__}"
                     )
 
                 if ep not in self.endpoints:
-                    endpoint_config = nested.nget(self.schema, [ep, "config"])
+                    endpoint_config = nget(self.schema, [ep, "config"])
                     self.schema.get(ep, {})
                     if isinstance(ep, EndPoint):
                         self.endpoints[ep.endpoint] = ep
                     elif ep == "chat/completions":
                         self.endpoints[ep] = EndPoint(
                             max_requests=self.chat_config_rate_limit.get(
                                 "max_requests", 1000
@@ -788,29 +831,29 @@
                         )
 
                 if not self.endpoints[ep]._has_initialized:
                     await self.endpoints[ep].init_rate_limiter()
 
         else:
             for ep in self.available_endpoints:
-                endpoint_config = nested.nget(self.schema, [ep, "config"])
+                endpoint_config = nget(self.schema, [ep, "config"])
                 self.schema.get(ep, {})
                 if ep not in self.endpoints:
                     self.endpoints[ep] = EndPoint(
                         max_requests=endpoint_config.get("max_requests", 1000),
                         max_tokens=endpoint_config.get("max_tokens", 100000),
                         interval=endpoint_config.get("interval", 60),
                         endpoint_=ep,
                         token_encoding_name=self.token_encoding_name,
                         config=endpoint_config,
                     )
                 if not self.endpoints[ep]._has_initialized:
                     await self.endpoints[ep].init_rate_limiter()
 
-    async def call_api(self, payload, endpoint, method, **kwargs):
+    async def call_api(self, payload, endpoint, method, required_tokens=None, **kwargs):
         """
         Calls the specified API endpoint with the given payload and method.
 
         Args:
                 payload: The payload to send with the API call.
                 endpoint: The endpoint to call.
                 method: The HTTP method to use for the call.
@@ -827,21 +870,33 @@
             return await self.endpoints[endpoint].rate_limiter._call_api(
                 http_session=http_session,
                 endpoint=endpoint,
                 base_url=self.base_url,
                 api_key=self.api_key,
                 method=method,
                 payload=payload,
+                required_tokens=required_tokens,
                 **kwargs,
             )
 
 
 class PayloadPackage:
 
     @classmethod
+    def embeddings(cls, embed_str, llmconfig, schema, **kwargs):
+        return APIUtil.create_payload(
+            input_=embed_str,
+            config=llmconfig,
+            required_=schema["required"],
+            optional_=schema["optional"],
+            input_key="input",
+            **kwargs,
+        )
+
+    @classmethod
     def chat_completion(cls, messages, llmconfig, schema, **kwargs):
         """
         Creates a payload for the chat completion operation.
 
         Args:
                 messages: The messages to include in the chat completion.
                 llmconfig: Configuration for the language model.
@@ -870,15 +925,15 @@
                 llmconfig: Configuration for the language model.
                 schema: The schema describing required and optional fields.
                 **kwargs: Additional keyword arguments.
 
         Returns:
                 The constructed payload.
         """
-        return APIUtil._create_payload(
+        return APIUtil.create_payload(
             input_=training_file,
             config=llmconfig,
             required_=schema["required"],
             optional_=schema["optional"],
             input_key="training_file",
             **kwargs,
         )
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_async.py` & `lionagi-0.2.0/lionagi/libs/ln_async.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/libs/ln_convert.py` & `lionagi-0.2.0/lionagi/libs/ln_convert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import json
 import re
 from functools import singledispatch
 
 from typing import Any, Type, Iterable, Generator
 
 import pandas as pd
@@ -357,14 +373,16 @@
     /,
     *,
     how: str = "all",
     drop_kwargs: dict | None = None,
     reset_index: bool = True,
     **kwargs,
 ) -> pd.DataFrame:
+    if not input_:
+        return pd.DataFrame()
     if not isinstance(input_[0], (pd.DataFrame, pd.Series, pd.core.generic.NDFrame)):
         if drop_kwargs is None:
             drop_kwargs = {}
         try:
             dfs = pd.DataFrame(input_, **kwargs)
             dfs = dfs.dropna(**(drop_kwargs | {"how": how}))
             return dfs.reset_index(drop=True) if reset_index else dfs
@@ -396,15 +414,15 @@
 
 def to_num(
     input_: Any,
     /,
     *,
     upper_bound: int | float | None = None,
     lower_bound: int | float | None = None,
-    num_type: Type[int | float] = int,
+    num_type: Type[int | float] = float,
     precision: int | None = None,
 ) -> int | float:
     """
     Converts the input to a numeric value of specified type, with optional bounds and precision.
 
     Args:
             input_ (Any): The input value to convert. Can be of any type that `to_str` can handle.
@@ -419,23 +437,17 @@
     Raises:
             ValueError: If the input cannot be converted to a number, or if it violates the specified bounds.
     """
     str_ = to_str(input_)
     return _str_to_num(str_, upper_bound, lower_bound, num_type, precision)
 
 
-def to_readable_dict(input_: Any | list[Any]) -> str | list[Any]:
+def to_readable_dict(input_: Any) -> str:
     """
-    Converts a given input to a readable dictionary format, either as a string or a list of dictionaries.
-
-    Args:
-            input_ (Any | list[Any]): The input to convert to a readable dictionary format.
-
-    Returns:
-            str | list[str]: The readable dictionary format of the input.
+    Converts a given input to a readable dictionary format
     """
 
     try:
         dict_ = to_dict(input_)
         return json.dumps(dict_, indent=4) if isinstance(input_, dict) else input_
     except Exception as e:
         raise ValueError(f"Could not convert given input to readable dict: {e}") from e
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_dataframe.py` & `lionagi-0.2.0/lionagi/libs/ln_dataframe.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/libs/ln_func_call.py` & `lionagi-0.2.0/lionagi/libs/ln_func_call.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from __future__ import annotations
 
 import functools
 import asyncio
 import logging
 from concurrent.futures import ThreadPoolExecutor
 
@@ -111,27 +127,32 @@
             >>> async def square(x): return x * x
             >>> await alcall([1, 2, 3], square)
             [1, 4, 9]
     """
     tasks = []
     if input_ is not None:
         lst = to_list(input_)
-        tasks = [AsyncUtil.handle_async_sync(func, i, **kwargs) for i in lst]
+        tasks = [call_handler(func, i, **kwargs) for i in lst]
 
     else:
-        tasks = [AsyncUtil.handle_async_sync(func, **kwargs)]
+        tasks = [call_handler(func, **kwargs)]
 
-    outs = await AsyncUtil.execute_tasks(*tasks)
+    outs = await asyncio.gather(*tasks)
     outs_ = []
     for i in outs:
         outs_.append(await i if isinstance(i, (Coroutine, asyncio.Future)) else i)
 
     return to_list(outs_, flatten=flatten, dropna=dropna)
 
 
+async def pcall(funcs):
+    task = [call_handler(func) for func in funcs]
+    return await asyncio.gather(*task)
+
+
 async def mcall(
     input_: Any, /, func: Any, *, explode: bool = False, **kwargs
 ) -> tuple[Any]:
     """
     asynchronously map a function or functions over an input_ or inputs.
 
     Args:
@@ -286,18 +307,20 @@
     return await async_call() if AsyncUtil.is_coroutine_func(func) else sync_call()
 
 
 async def rcall(
     func: Callable,
     *args,
     retries: int = 0,
-    delay: float = 1.0,
-    backoff_factor: float = 2.0,
+    delay: float = 0.1,
+    backoff_factor: float = 2,
     default: Any = None,
     timeout: float | None = None,
+    timing: bool = False,
+    verbose: bool = True,
     **kwargs,
 ) -> Any:
     """
     asynchronously retries a function call with exponential backoff.
 
     designed for resilience, this function attempts to call an asynchronous function
     multiple times with increasing delays between attempts. this is particularly
@@ -335,28 +358,42 @@
             ...     raise Exception("temporary error")
             >>> await rcall(fetch_data, retries=3, delay=2, default="default value")
             'default value'
     """
     last_exception = None
     result = None
 
+    start = SysUtil.get_now(datetime_=False)
     for attempt in range(retries + 1) if retries == 0 else range(retries):
         try:
+            err_msg = f"Attempt {attempt + 1}/{retries}: " if retries > 0 else None
+            if timing:
+                return (
+                    await _tcall(
+                        func, *args, err_msg=err_msg, timeout=timeout, **kwargs
+                    ),
+                    SysUtil.get_now(datetime_=False) - start,
+                )
+
             return await _tcall(func, *args, timeout=timeout, **kwargs)
         except Exception as e:
             last_exception = e
             if attempt < retries:
-                await AsyncUtil.sleep(delay)
+                if verbose:
+                    print(f"Attempt {attempt + 1}/{retries} failed: {e}, retrying...")
+                await asyncio.sleep(delay)
                 delay *= backoff_factor
             else:
                 break
     if result is None and default is not None:
         return default
     elif last_exception is not None:
-        raise last_exception
+        raise RuntimeError(
+            f"Operation failed after {retries+1} attempts: {last_exception}"
+        ) from last_exception
     else:
         raise RuntimeError("rcall failed without catching an exception")
 
 
 def _dropna(lst_: list[Any]) -> list[Any]:
     """
     Remove None values from a list.
@@ -391,16 +428,16 @@
 
     examples:
             >>> async def square(x): return x * x
             >>> asyncio.run(alcall([1, 2, 3], square))
             [1, 4, 9]
     """
     lst = to_list(input_)
-    tasks = [AsyncUtil.handle_async_sync(func, i, **kwargs) for i in lst]
-    outs = await AsyncUtil.execute_tasks(*tasks)
+    tasks = [call_handler(func, i, **kwargs) for i in lst]
+    outs = await asyncio.gather(*tasks)
     return to_list(outs, flatten=flatten)
 
 
 async def _tcall(
     func: Callable,
     *args,
     delay: float = 0,
@@ -431,49 +468,47 @@
     examples:
             >>> async def example_func(x): return x
             >>> asyncio.run(tcall(example_func, 5, timing=True))
             (5, duration)
     """
     start_time = SysUtil.get_now(datetime_=False)
     try:
-        await AsyncUtil.sleep(delay)
+        await asyncio.sleep(delay)
         # Apply timeout to the function call
         if timeout is not None:
             coro = ""
-            if AsyncUtil.is_coroutine_func(func):
+            if is_coroutine_func(func):
                 coro = func(*args, **kwargs)
             else:
 
                 async def coro_():
                     return func(*args, **kwargs)
 
                 coro = coro_()
 
             result = await asyncio.wait_for(coro, timeout)
 
         else:
-            if AsyncUtil.is_coroutine_func(func):
+            if is_coroutine_func(func):
                 return await func(*args, **kwargs)
             return func(*args, **kwargs)
         duration = SysUtil.get_now(datetime_=False) - start_time
         return (result, duration) if timing else result
     except asyncio.TimeoutError as e:
-        err_msg = f"{err_msg} Error: {e}" if err_msg else f"An error occurred: {e}"
-        print(err_msg)
+        err_msg = f"{err_msg or ''}Timeout {timeout} seconds exceeded"
         if ignore_err:
             return (
                 (default, SysUtil.get_now(datetime_=False) - start_time)
                 if timing
                 else default
             )
         else:
-            raise e  # Re-raise the timeout exception
+            raise asyncio.TimeoutError(err_msg)  # Re-raise the timeout exception
     except Exception as e:
         err_msg = f"{err_msg} Error: {e}" if err_msg else f"An error occurred: {e}"
-        print(err_msg)
         if ignore_err:
             return (
                 (default, SysUtil.get_now(datetime_=False) - start_time)
                 if timing
                 else default
             )
         else:
@@ -533,15 +568,19 @@
 
             return wrapper
 
         return decorator
 
     @staticmethod
     def retry(
-        retries: int = 3, delay: float = 2.0, backoff_factor: float = 2.0
+        retries: int = 3,
+        delay: float = 2.0,
+        backoff_factor: float = 2.0,
+        default=...,
+        verbose=True,
     ) -> Callable:
         """
         Decorates an asynchronous function to automatically retry on failure,
         with configurable retries, delay, and exponential backoff.
 
         This decorator is useful for handling operations that may fail due to transient
         issues, such as network connectivity problems or temporary provider
@@ -577,14 +616,16 @@
             async def wrapper(*args, **kwargs) -> Any:
                 return await rcall(
                     func,
                     *args,
                     retries=retries,
                     delay=delay,
                     backoff_factor=backoff_factor,
+                    default=default,
+                    verbose=verbose,
                     **kwargs,
                 )
 
             return wrapper
 
         return decorator
 
@@ -686,15 +727,15 @@
                 ... async def get_names():
                 ...     # Asynchronously fetches a list of names
                 ...     return ["alice", "bob", "charlie"]
                 ... # `get_names` now returns ["ALICE", "BOB", "CHARLIE"]
         """
 
         def decorator(func: Callable[..., list[Any]]) -> Callable:
-            if AsyncUtil.is_coroutine_func(func):
+            if is_coroutine_func(func):
 
                 @functools.wraps(func)
                 async def async_wrapper(*args, **kwargs) -> list[Any]:
                     values = await func(*args, **kwargs)
                     return [function(value) for value in values]
 
                 return async_wrapper
@@ -744,30 +785,30 @@
                 ... def start_value(x):
                 ...     return x
                 >>> start_value(3)
                 7  # The value is doubled to 6, then incremented to 7
         """
 
         def decorator(func: Callable) -> Callable:
-            if not any(AsyncUtil.is_coroutine_func(f) for f in functions):
+            if not any(is_coroutine_func(f) for f in functions):
 
                 @functools.wraps(func)
                 def sync_wrapper(*args, **kwargs):
                     value = func(*args, **kwargs)
                     for function in functions:
                         try:
                             value = function(value)
                         except Exception as e:
                             raise ValueError(
                                 f"Error in function {function.__name__}: {e}"
                             )
                     return value
 
                 return sync_wrapper
-            elif all(AsyncUtil.is_coroutine_func(f) for f in functions):
+            elif all(is_coroutine_func(f) for f in functions):
 
                 @functools.wraps(func)
                 async def async_wrapper(*args, **kwargs):
                     value = func(*args, **kwargs)
                     for function in functions:
                         try:
                             value = await function(value)
@@ -823,15 +864,15 @@
                 ... async def process_value(x):
                 ...     return x + 2
                 >>> asyncio.run(process_value(5))
                 12  # Input 5 is preprocessed to 4, processed to 6, and postprocessed to 12
         """
 
         def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
-            if AsyncUtil.is_coroutine_func(func):
+            if is_coroutine_func(func):
 
                 @functools.wraps(func)
                 async def async_wrapper(*args, **kwargs) -> Any:
                     preprocessed_args = [
                         preprocess(arg, *preprocess_args, **preprocess_kwargs)
                         for arg in args
                     ]
@@ -885,15 +926,15 @@
                 ... async def fetch_data(key):
                 ...     # Simulate a database fetch
                 ...     return "data for " + key
                 ... # Subsequent calls to `fetch_data` with the same `key` within 10 seconds
                 ... # will return the cached result without re-executing the function body.
         """
 
-        if AsyncUtil.is_coroutine_func(func):
+        if is_coroutine_func(func):
             # Asynchronous function handling
             @AsyncUtil.cached(ttl=ttl)
             async def cached_async(*args, **kwargs) -> Any:
                 return await func(*args, **kwargs)
 
             @functools.wraps(func)
             async def async_wrapper(*args, **kwargs) -> Any:
@@ -989,15 +1030,15 @@
                 ...     return [1, 2, 3, 4]
                 >>> asyncio.run(sum_numbers())
                 10
                 ... # The numbers in the list are summed, resulting in a single value.
         """
 
         def decorator(func: Callable[..., list[Any]]) -> Callable:
-            if AsyncUtil.is_coroutine_func(func):
+            if is_coroutine_func(func):
 
                 @functools.wraps(func)
                 async def async_wrapper(*args, **kwargs) -> Any:
                     values = await func(*args, **kwargs)
                     return functools.reduce(function, values, initial)
 
                 return async_wrapper
@@ -1035,19 +1076,19 @@
                 ... async def process_data(input_):
                 ...     # Asynchronous processing logic here
                 ...     pass
                 ... # No more than 3 instances of `process_data` will run concurrently.
         """
 
         def decorator(func: Callable) -> Callable:
-            if not AsyncUtil.is_coroutine_func(func):
+            if not is_coroutine_func(func):
                 raise TypeError(
                     "max_concurrency decorator can only be used with async functions."
                 )
-            semaphore = AsyncUtil.semaphore(limit)
+            semaphore = asyncio.Semaphore(limit)
 
             @functools.wraps(func)
             async def wrapper(*args, **kwargs):
                 async with semaphore:
                     return await func(*args, **kwargs)
 
             return wrapper
@@ -1085,15 +1126,15 @@
     @staticmethod
     def force_async(fn):
         pool = ThreadPoolExecutor()
 
         @functools.wraps(fn)
         def wrapper(*args, **kwargs):
             future = pool.submit(fn, *args, **kwargs)
-            return AsyncUtil.wrap_future(future)  # make it awaitable
+            return asyncio.wrap_future(future)  # make it awaitable
 
         return wrapper
 
 
 class Throttle:
     """
     A class that provides a throttling mechanism for function calls.
@@ -1229,16 +1270,16 @@
 
         if loop.is_running():
             return await func(*args, **kwargs)
 
     except Exception as e:
         if error_map:
             _custom_error_handler(e, error_map)
-        else:
-            logging.error(f"Error in call_handler: {e}")
+        # else:
+        #     logging.error(f"Error in call_handler: {e}")
         raise
 
 
 @functools.lru_cache(maxsize=None)
 def is_coroutine_func(func: Callable) -> bool:
     """
     checks if the specified function is an asyncio coroutine function.
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_knowledge_graph.py` & `lionagi-0.2.0/lionagi/libs/ln_knowledge_graph.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/libs/ln_nested.py` & `lionagi-0.2.0/lionagi/libs/ln_nested.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from collections import defaultdict
 from itertools import chain
 from typing import Any, Generator, Callable
 
 from lionagi.libs.sys_util import SysUtil
 import lionagi.libs.ln_convert as convert
 
@@ -48,15 +64,15 @@
     else:
         raise TypeError("Cannot set value on non-list/dict element")
 
 
 def nget(
     nested_structure: dict | list,
     indices: list[int | str],
-    default: Any | None = None,
+    default=...,
 ) -> Any:
     """
     retrieves a value from a nested list or dictionary structure, with an option to
     specify a default value.
 
     navigates through the nested structure using the specified indices and
     retrieves the value at the target location. the indices can be integers for
@@ -94,33 +110,33 @@
             and isinstance(last_index, int)
             and last_index < len(target_container)
         ):
 
             return target_container[last_index]
         elif isinstance(target_container, dict) and last_index in target_container:
             return target_container[last_index]
-        elif default is not None:
+        elif default is not ...:
             return default
         else:
             raise LookupError("Target not found and no default value provided.")
     except (IndexError, KeyError, TypeError):
-        if default is not None:
+        if default is not ...:
             return default
         else:
             raise LookupError("Target not found and no default value provided.")
 
 
 # nested merge
 def nmerge(
     nested_structure: list[dict | list],
     /,
     *,
     overwrite: bool = False,
     dict_sequence: bool = False,
-    sequence_separator: str = "_",
+    sequence_separator: str = "[^_^]",
     sort_list: bool = False,
     custom_sort: Callable[[Any], Any] | None = None,
 ) -> dict | list:
     """
     merges multiple dictionaries, lists, or sequences into a unified structure.
 
     this method intelligently merges a nested_structure of iterable objects (
@@ -172,15 +188,15 @@
 
 # flatten dictionary
 def flatten(
     nested_structure: Any,
     /,
     *,
     parent_key: str = "",
-    sep: str = "_",
+    sep: str = "[^_^]",
     max_depth: int | None = None,
     inplace: bool = False,
     dict_only: bool = False,
 ) -> dict | None:
     """
     flattens a nested structure into a dictionary with composite keys.
 
@@ -234,15 +250,15 @@
 
 
 # unflatten dictionary
 def unflatten(
     flat_dict: dict[str, Any],
     /,
     *,
-    sep: str = "_",
+    sep: str = "[^_^]",
     custom_logic: Callable[[str], Any] | None = None,
     max_depth: int | None = None,
 ) -> dict | list:
     """
     reconstructs a nested structure from a flat dictionary with composite keys.
 
     given a flat dictionary with keys representing paths, this method rebuilds the
@@ -326,15 +342,15 @@
 
 def ninsert(
     nested_structure: dict | list,
     /,
     indices: list[str | int],
     value: Any,
     *,
-    sep: str = "_",
+    sep: str = "[^_^]",
     max_depth: int | None = None,
     current_depth: int = 0,
 ) -> None:
     """
     inserts a value into a nested structure at a specified path.
 
     navigates a nested dictionary or list based on a sequence of indices or keys (
@@ -389,20 +405,19 @@
         _handle_list_insert(nested_structure, last_part, value)
     elif isinstance(nested_structure, list):
         nested_structure.append({last_part: value})
     else:
         nested_structure[last_part] = value
 
 
-# noinspection PyDecorator
 def get_flattened_keys(
     nested_structure: Any,
     /,
     *,
-    sep: str = "_",
+    sep: str = "[^_^]",
     max_depth: int | None = None,
     dict_only: bool = False,
     inplace: bool = False,
 ) -> list[str]:
     """
     retrieves keys from a nested structure after flattening.
 
@@ -444,15 +459,15 @@
 
 
 def _dynamic_flatten_in_place(
     nested_structure: Any,
     /,
     *,
     parent_key: str = "",
-    sep: str = "_",
+    sep: str = "[^_^]",
     max_depth: int | None = None,
     current_depth: int = 0,
     dict_only: bool = False,
 ) -> None:
     """
     Flattens a nested structure in place up to a specified depth.
 
@@ -577,15 +592,15 @@
             original[key] = value
     return original
 
 
 def _dynamic_flatten_generator(
     nested_structure: Any,
     parent_key: tuple[str, ...],
-    sep: str = "_",
+    sep: str = "[^_^]",
     max_depth: int | None = None,
     current_depth: int = 0,
     dict_only: bool = False,
 ) -> Generator[tuple[str, Any], None, None]:
     """
     Generates flattened key-value pairs from a nested structure.
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_parse.py` & `lionagi-0.2.0/lionagi/libs/ln_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,27 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 from collections.abc import Callable
 import re
 import inspect
 import itertools
-import contextlib
-from functools import singledispatchmethod
 from typing import Any
 import numpy as np
 import lionagi.libs.ln_convert as convert
 
 
 md_json_char_map = {"\n": "\\n", "\r": "\\r", "\t": "\\t", '"': '\\"'}
 
@@ -99,20 +113,20 @@
 
         # Match any of the special characters to be escaped.
         return re.sub(r'[\n\r\t"]', replacement, value)
 
     # inspired by langchain_core.output_parsers.json (MIT License)
     # https://github.com/langchain-ai/langchain/blob/master/libs/core/langchain_core/output_parsers/json.py
     @staticmethod
-    def extract_code_block(
+    def extract_json_block(
         str_to_parse: str,
         language: str | None = None,
         regex_pattern: str | None = None,
         *,
-        parser: Callable[[str], Any],
+        parser: Callable[[str], Any] = None,
     ) -> Any:
         """
         Extracts and parses a code block from Markdown content.
 
         This method searches for a code block in the given Markdown string, optionally
         filtered by language. If a code block is found, it is parsed using the provided parser function.
 
@@ -144,18 +158,46 @@
         code_str = ""
         if match:
             code_str = match[1].strip()
         else:
             raise ValueError(
                 f"No {language or 'specified'} code block found in the Markdown content."
             )
+        if not match:
+            str_to_parse = str_to_parse.strip()
+            if str_to_parse.startswith("```json\n") and str_to_parse.endswith("\n```"):
+                str_to_parse = str_to_parse[8:-4].strip()
 
+        parser = parser or ParseUtil.fuzzy_parse_json
         return parser(code_str)
 
     @staticmethod
+    def extract_code_blocks(code):
+        code_blocks = []
+        lines = code.split("\n")
+        inside_code_block = False
+        current_block = []
+
+        for line in lines:
+            if line.startswith("```"):
+                if inside_code_block:
+                    code_blocks.append("\n".join(current_block))
+                    current_block = []
+                    inside_code_block = False
+                else:
+                    inside_code_block = True
+            elif inside_code_block:
+                current_block.append(line)
+
+        if current_block:
+            code_blocks.append("\n".join(current_block))
+
+        return "\n\n".join(code_blocks)
+
+    @staticmethod
     def md_to_json(
         str_to_parse: str,
         *,
         expected_keys: list[str] | None = None,
         parser: Callable[[str], Any] | None = None,
     ) -> Any:
         """
@@ -177,15 +219,15 @@
                 ValueError: If the JSON code block is missing, or if any of the expected keys are missing
                         from the parsed JSON object.
 
         Examples:
                 >>> md_to_json('```json\\n{"key": "value"}\\n```', expected_keys=['key'])
                 {'key': 'value'}
         """
-        json_obj = ParseUtil.extract_code_block(
+        json_obj = ParseUtil.extract_json_block(
             str_to_parse, language="json", parser=parser or ParseUtil.fuzzy_parse_json
         )
 
         if expected_keys:
             if missing_keys := [key for key in expected_keys if key not in json_obj]:
                 raise ValueError(
                     f"Missing expected keys in JSON object: {', '.join(missing_keys)}"
@@ -381,15 +423,17 @@
             "tuple": "array",
             "bool": "boolean",
             "dict": "object",
         }
         return type_mapping.get(py_type, "object")
 
     @staticmethod
-    def _func_to_schema(func, style="google"):
+    def _func_to_schema(
+        func, style="google", func_description=None, params_description=None
+    ):
         """
         Generates a schema description for a given function, using typing hints and
         docstrings. The schema includes the function's name, description, and parameters.
 
         Args:
                 func (Callable): The function to generate a schema for.
                 style (str): The docstring format ('google' or 'reST').
@@ -408,17 +452,19 @@
                 ...     return True
                 >>> schema = _func_to_schema(example_function)
                 >>> schema['function']['name']
                 'example_function'
         """
         # Extracting function name and docstring details
         func_name = func.__name__
-        func_description, params_description = ParseUtil._extract_docstring_details(
-            func, style
-        )
+
+        if not func_description:
+            func_description, _ = ParseUtil._extract_docstring_details(func, style)
+        if not params_description:
+            _, params_description = ParseUtil._extract_docstring_details(func, style)
 
         # Extracting parameters with typing hints
         sig = inspect.signature(func)
         parameters = {
             "type": "object",
             "properties": {},
             "required": [],
@@ -630,47 +676,60 @@
 
         if score_func is None:
             score_func = StringMatch.jaro_winkler_similarity
 
         # Calculate Jaro-Winkler similarity scores for each potential match
         scores = np.array(
             [
-                score_func(convert.to_str(word), correct_word)
+                score_func(str(word), str(correct_word))
                 for correct_word in correct_words_list
             ]
         )
         # Find the index of the highest score
         max_score_index = np.argmax(scores)
         return correct_words_list[max_score_index]
 
     @staticmethod
     def force_validate_dict(x, keys: dict | list[str]) -> dict:
         out_ = x
 
         if isinstance(out_, str):
             # first try to parse it straight as a fuzzy json
+            
             try:
                 out_ = ParseUtil.fuzzy_parse_json(out_)
-            except Exception:
+                return StringMatch.correct_dict_keys(keys, out_)
+            
+            except:
                 try:
-                    # if failed we try to extract the json block and parse it
                     out_ = ParseUtil.md_to_json(out_)
+                    return StringMatch.correct_dict_keys(keys, out_)
+
                 except Exception:
-                    # if still failed we try to extract the json block using re and parse it again
-                    match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
-                    if match:
-                        out_ = match.group(1)
-                        try:
-                            out_ = ParseUtil.fuzzy_parse_json(out_)
-                        except:
+                    try:
+                        # if failed we try to extract the json block and parse it
+                        out_ = ParseUtil.md_to_json(out_)
+                        return StringMatch.correct_dict_keys(keys, out_)
+
+                    except Exception:
+                        # if still failed we try to extract the json block using re and parse it again
+                        match = re.search(r"```json\n({.*?})\n```", out_, re.DOTALL)
+                        if match:
+                            out_ = match.group(1)
                             try:
-                                out_ = ParseUtil.fuzzy_parse_json(
-                                    out_.replace("'", '"')
-                                )
+                                out_ = ParseUtil.fuzzy_parse_json(out_)
+                                return StringMatch.correct_dict_keys(keys, out_)
+
                             except:
-                                pass
+                                try:
+                                    out_ = ParseUtil.fuzzy_parse_json(
+                                        out_.replace("'", '"')
+                                    )
+                                    return StringMatch.correct_dict_keys(keys, out_)
+                                except:
+                                    pass
 
         if isinstance(out_, dict):
             try:
                 return StringMatch.correct_dict_keys(keys, out_)
             except Exception as e:
                 raise ValueError(f"Failed to force_validate_dict for input: {x}") from e
```

### Comparing `lionagi-0.1.2/lionagi/libs/ln_tokenizer.py` & `lionagi-0.2.0/lionagi/experimental/directive/tokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+"""
+Copyright 2024 HaiyangLi
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
+"""
+
 import re
 
 
 class BaseToken:
     def __init__(self, type_, value):
         self.type = type_
         self.value = value
```

### Comparing `lionagi-0.1.2/lionagi/libs/sys_util.py` & `lionagi-0.2.0/lionagi/libs/sys_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 """
-MIT License
+Copyright 2024 HaiyangLi
 
-Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
-
-Permission is hereby granted, free of charge, to any person 
-obtaining a copy of this software and associated documentation 
-files (the "Software"), to deal in the Software without 
-restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or 
-sell copies of the Software, and to permit persons to whom 
-the Software is furnished to do so, subject to the following 
-conditions:
-
-The above copyright notice and this permission notice shall be 
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, 
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES 
-OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND 
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS 
-BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN 
-ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN 
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-SOFTWARE.
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 
 import copy
 import importlib
 import logging
 import os
 import platform
@@ -426,34 +415,116 @@
         full_path = directory / full_filename
         full_path.parent.mkdir(parents=True, exist_ok=dir_exist_ok)
 
         return full_path
 
     @staticmethod
     def list_files(dir_path: Path | str, extension: str = None) -> list[Path]:
+        """
+        Lists all files in a specified directory with an optional filter for file extensions.
+
+        Args:
+            dir_path (Path | str): The directory path where files are listed.
+            extension (str, optional): Filter files by extension. Default is None, which lists all files.
+
+        Returns:
+            list[Path]: A list of Path objects representing files in the directory.
+
+        Raises:
+            NotADirectoryError: If the provided dir_path is not a directory.
+        """
         dir_path = Path(dir_path)
         if not dir_path.is_dir():
             raise NotADirectoryError(f"{dir_path} is not a directory.")
         if extension:
             return list(dir_path.glob(f"*.{extension}"))
         else:
             return list(dir_path.glob("*"))
 
     @staticmethod
     def copy_file(src: Path | str, dest: Path | str) -> None:
+        """
+        Copies a file from a source path to a destination path.
+
+        Args:
+            src (Path | str): The source file path.
+            dest (Path | str): The destination file path.
+
+        Raises:
+            FileNotFoundError: If the source file does not exist or is not a file.
+        """
         from shutil import copy2
 
         src, dest = Path(src), Path(dest)
         if not src.is_file():
             raise FileNotFoundError(f"{src} does not exist or is not a file.")
         dest.parent.mkdir(parents=True, exist_ok=True)
         copy2(src, dest)
 
     @staticmethod
     def get_size(path: Path | str) -> int:
+        """
+        Gets the size of a file or total size of files in a directory.
+
+        Args:
+            path (Path | str): The file or directory path.
+
+        Returns:
+            int: The size in bytes.
+
+        Raises:
+            FileNotFoundError: If the path does not exist.
+        """
         path = Path(path)
         if path.is_file():
             return path.stat().st_size
         elif path.is_dir():
             return sum(f.stat().st_size for f in path.glob("**/*") if f.is_file())
         else:
             raise FileNotFoundError(f"{path} does not exist.")
+
+    @staticmethod
+    def save_to_file(
+        text,
+        directory: Path | str,
+        filename: str,
+        timestamp: bool = True,
+        dir_exist_ok: bool = True,
+        time_prefix: bool = False,
+        custom_timestamp_format: str | None = None,
+        random_hash_digits=0,
+        verbose=True,
+    ):
+        """
+        Saves text to a file within a specified directory, optionally adding a timestamp, hash, and verbose logging.
+
+        Args:
+            text (str): The text to save.
+            directory (Path | str): The directory path to save the file.
+            filename (str): The filename for the saved text.
+            timestamp (bool): If True, append a timestamp to the filename. Default is True.
+            dir_exist_ok (bool): If True, creates the directory if it does not exist. Default is True.
+            time_prefix (bool): If True, prepend the timestamp instead of appending. Default is False.
+            custom_timestamp_format (str | None): A custom format for the timestamp, if None uses default format. Default is None.
+            random_hash_digits (int): Number of random hash digits to append to filename. Default is 0.
+            verbose (bool): If True, prints the file path after saving. Default is True.
+
+        Returns:
+            bool: True if the text was successfully saved.
+        """
+        file_path = SysUtil.create_path(
+            directory=directory,
+            filename=filename,
+            timestamp=timestamp,
+            dir_exist_ok=dir_exist_ok,
+            time_prefix=time_prefix,
+            custom_timestamp_format=custom_timestamp_format,
+            random_hash_digits=random_hash_digits,
+        )
+
+        with open(file_path, "w") as file:
+            file.write(text)
+
+        if verbose:
+            print(f"Text saved to: {file_path}")
+
+        return True
```

### Comparing `lionagi-0.1.2/lionagi/lions/coder/add_feature.py` & `lionagi-0.2.0/lionagi/lions/coder/add_feature.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/lions/coder/coder.py` & `lionagi-0.2.0/lionagi/lions/coder/coder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,53 @@
 import asyncio
+from pathlib import Path
+
+from lionagi import logging as _logging
 from lionagi.core import Session
+from lionagi.libs import ParseUtil
 
 from .base_prompts import CODER_PROMPTS
-from .util import extract_code_blocks, install_missing_dependencies, set_up_interpreter
+from .util import install_missing_dependencies, set_up_interpreter, save_code_file
 
 
 class Coder:
+
     def __init__(
-        self, prompts=None, session=None, session_kwargs=None, required_libraries=None
+        self,
+        prompts: dict = None,
+        session: Session = None,
+        session_kwargs: dict = None,
+        required_libraries: list = None,
+        work_dir: Path | str = None,
+    ) -> None:
+
+        self.prompts = prompts or CODER_PROMPTS
+        self.session = session or self._create_session(session_kwargs)
+        self.required_libraries = required_libraries or ["lionagi"]
+        self.work_dir = work_dir or Path.cwd() / "coder" / "code_files"
+
+    def _create_session(self, session_kwargs: dict = None) -> Session:
+        session_kwargs = session_kwargs or {}
+        return Session(system=self.prompts["system"], **session_kwargs)
+
+
+class Coder:
+    def __init__(
+        self,
+        prompts=None,
+        session=None,
+        session_kwargs=None,
+        required_libraries=None,
+        work_dir=None,
     ):
         print("Initializing Coder...")
         self.prompts = prompts or CODER_PROMPTS
         self.session = session or self._create_session(session_kwargs)
         self.required_libraries = required_libraries or ["lionagi"]
+        self.work_dir = work_dir or Path.cwd() / "coder" / "code_files"
         print("Coder initialized.")
 
     def _create_session(self, session_kwargs=None):
         print("Creating session...")
         session_kwargs = session_kwargs or {}
         session = Session(system=self.prompts["system"], **session_kwargs)
         print("Session created.")
@@ -28,15 +59,15 @@
         print("Code planning completed.")
         return plans
 
     async def _write_code(self, context=None):
         print("Writing code...")
         code = await self.session.chat(self.prompts["write_code"], context=context)
         print("Code writing completed.")
-        return extract_code_blocks(code)
+        return ParseUtil.extract_code_blocks(code)
 
     async def _review_code(self, context=None):
         print("Reviewing code...")
         code = await self.session.chat(self.prompts["review_code"], context=context)
         print("Code review completed.")
         return code
 
@@ -74,14 +105,30 @@
             )
             if error == "try again":
                 print("Retrying code execution...")
                 execution = sandbox.notebook.exec_cell(code, **kwargs)
             print("Code execution completed.")
             return execution
 
+    def _save_code_file(self, code, **kwargs):
+        print("Saving code...")
+        save_code_file(code, self.work_dir, **kwargs)
+        print("Code saved.")
+
+    @staticmethod
+    def _load_code_file(file_path):
+        print("Loading code...")
+        try:
+            with open(file_path, "r") as file:
+                print("Code loaded.")
+                return file.read()
+        except FileNotFoundError:
+            _logging.error(f"File not found: {file_path}")
+            return None
+
 
 async def main():
     print("Starting main function...")
     coder = Coder()
 
     code_prompt = """
     write a pure python function that takes a list of integers and returns the sum of all the integers in the list. write a couple tests as well
```

### Comparing `lionagi-0.1.2/lionagi/lions/coder/util.py` & `lionagi-0.2.0/lionagi/lions/coder/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from typing import Any
+from pathlib import Path
+
 E2B_key_scheme = "E2B_API_KEY"
 
 
 def set_up_interpreter(interpreter_provider="e2b", key_scheme=E2B_key_scheme):
 
     if interpreter_provider == "e2b":
         from dotenv import load_dotenv
@@ -17,39 +20,14 @@
 
         return CodeInterpreter(api_key=getenv(key_scheme))
 
     else:
         raise ValueError("Invalid interpreter provider")
 
 
-def extract_code_blocks(code):
-    print("Extracting code blocks...")
-    code_blocks = []
-    lines = code.split("\n")
-    inside_code_block = False
-    current_block = []
-
-    for line in lines:
-        if line.startswith("```"):
-            if inside_code_block:
-                code_blocks.append("\n".join(current_block))
-                current_block = []
-                inside_code_block = False
-            else:
-                inside_code_block = True
-        elif inside_code_block:
-            current_block.append(line)
-
-    if current_block:
-        code_blocks.append("\n".join(current_block))
-
-    print(f"Extracted {len(code_blocks)} code block(s).")
-    return "\n\n".join(code_blocks)
-
-
 def install_missing_dependencies(required_libraries):
     print("Checking for missing dependencies...")
     missing_libraries = [
         library for library in required_libraries if not is_library_installed(library)
     ]
 
     if missing_libraries:
@@ -85,7 +63,34 @@
         print(f"Error occurred while installing {library}: {str(e)}")
         print(
             "Please check the error message and ensure you have the necessary permissions to install packages."
         )
         print(
             "You may need to run the script with administrative privileges or use a virtual environment."
         )
+
+
+def save_code_file(
+    code: Any,
+    directory: Path | str = None,
+    filename: str = "code.py",
+    timestamp: bool = True,
+    dir_exist_ok: bool = True,
+    time_prefix: bool = False,
+    custom_timestamp_format: str | None = None,
+    random_hash_digits: int = 3,
+    verbose: bool = True,
+):
+
+    from lionagi.libs import SysUtil
+
+    return SysUtil.save_to_file(
+        text=code,
+        directory=directory,
+        filename=filename,
+        timestamp=timestamp,
+        dir_exist_ok=dir_exist_ok,
+        time_prefix=time_prefix,
+        custom_timestamp_format=custom_timestamp_format,
+        random_hash_digits=random_hash_digits,
+        verbose=verbose,
+    )
```

### Comparing `lionagi-0.1.2/lionagi/lions/researcher/data_source/finhub_.py` & `lionagi-0.2.0/lionagi/lions/researcher/data_source/finhub_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/lions/researcher/data_source/google_.py` & `lionagi-0.2.0/lionagi/lions/researcher/data_source/google_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/lions/researcher/data_source/wiki_.py` & `lionagi-0.2.0/lionagi/lions/researcher/data_source/wiki_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/lions/researcher/data_source/yfinance_.py` & `lionagi-0.2.0/lionagi/lions/researcher/data_source/yfinance_.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_api.py` & `lionagi-0.2.0/lionagi/tests/libs/test_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_convert.py` & `lionagi-0.2.0/lionagi/tests/libs/test_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_field_validators.py` & `lionagi-0.2.0/lionagi/tests/libs/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_func_call.py` & `lionagi-0.2.0/lionagi/tests/libs/test_func_call.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,41 +292,41 @@
         self.assertEqual(result, 10)
 
     async def test_timeout(self):
         async def async_func(x):
             await asyncio.sleep(2)
             return x
 
-        with self.assertRaises(asyncio.TimeoutError):
-            await rcall(async_func, 5, timeout=1)
+        with self.assertRaises(RuntimeError):
+            await rcall(async_func, 5, timeout=0.1)
 
     async def test_retry_mechanism(self):
         attempt_count = 0
 
         def sync_func(x):
             nonlocal attempt_count
             attempt_count += 1
             raise ValueError("Test Error")
 
-        with self.assertRaises(ValueError):
-            await rcall(sync_func, 5, retries=3)
+        with self.assertRaises(RuntimeError):
+            await rcall(sync_func, 5, retries=3, delay=0.1, backoff_factor=1.1)
         self.assertEqual(attempt_count, 3)  # Initial call + 3 retries
 
     async def test_default_value_on_exception(self):
         def sync_func(x):
             raise ValueError("Test Error")
 
-        result = await rcall(sync_func, 5, default=10)
+        result = await rcall(sync_func, 5, default=10, delay=0)
         self.assertEqual(result, 10)
 
     async def test_exception_propagation(self):
         def sync_func(x):
             raise ValueError("Test Error")
 
-        with self.assertRaises(ValueError):
+        with self.assertRaises(RuntimeError):
             await rcall(sync_func, 5)
 
 
 class TestCallDecorator(unittest.IsolatedAsyncioTestCase):
 
     def test_cache_decorator_sync(self):
         @CallDecorator.cache
@@ -577,123 +577,125 @@
         results = await asyncio.gather(*(test_func(i) for i in range(5)))
         self.assertEqual(results, [0, 1, 2, 3, 4])
 
 
 class TestThrottleClass(unittest.TestCase):
 
     def test_throttling_behavior_sync(self):
-        throttle_decorator = Throttle(2)  # 2 seconds throttle period
+        throttle_decorator = Throttle(0.1)  # 2 seconds throttle period
 
         @throttle_decorator
         def test_func():
             return time.time()
 
         first_call_time = test_func()
-        time.sleep(1)  # Sleep less than the throttle period
+        time.sleep(0.1)  # Sleep less than the throttle period
         second_call_time = test_func()
 
         self.assertGreaterEqual(
-            second_call_time - first_call_time, 2
+            second_call_time - first_call_time, 0.1
         )  # Second call should be throttled
 
     def test_throttling_behavior_async(self):
-        throttle_decorator = Throttle(2)  # 2 seconds throttle period
+        throttle_decorator = Throttle(1)  # 2 seconds throttle period
 
         @throttle_decorator
         async def test_func():
             return time.time()
 
         async def async_test():
             first_call_time = await test_func()
-            await asyncio.sleep(1)  # Sleep less than the throttle period
+            await asyncio.sleep(0.1)  # Sleep less than the throttle period
             second_call_time = await test_func()
 
             self.assertGreaterEqual(
-                second_call_time - first_call_time, 2
+                second_call_time - first_call_time, 1
             )  # Second call should be throttled
 
         asyncio.run(async_test())
 
     def test_successive_calls_with_sufficient_delay(self):
-        throttle_decorator = Throttle(1)  # 1 second throttle period
+        throttle_decorator = Throttle(0.1)  # 1 second throttle period
 
         @throttle_decorator
         def test_func():
             return time.time()
 
         first_call_time = test_func()
-        time.sleep(1.1)  # Sleep more than the throttle period
+        time.sleep(0.12)  # Sleep more than the throttle period
         second_call_time = test_func()
 
         self.assertLess(
-            second_call_time - first_call_time, 1.5
+            second_call_time - first_call_time, 0.2
         )  # Second call should not be throttled
 
 
 class TestAsyncRetryDecorator(unittest.IsolatedAsyncioTestCase):
     async def test_successful_retry(self):
         attempt = 0
 
-        @CallDecorator.retry(retries=3, delay=1, backoff_factor=2)
+        @CallDecorator.retry(retries=3, delay=0.1, backoff_factor=2)
         async def test_func():
             nonlocal attempt
             attempt += 1
             if attempt < 3:
                 raise ValueError("Test failure")
             return "Success"
 
         result = await test_func()
         self.assertEqual(result, "Success")
         self.assertEqual(attempt, 3)
 
     async def test_retry_limit(self):
         attempt = 0
 
-        @CallDecorator.retry(retries=2, delay=1, backoff_factor=2)
+        @CallDecorator.retry(retries=2, delay=0.1, backoff_factor=2)
         async def test_func():
             nonlocal attempt
             attempt += 1
             raise ValueError("Test failure")
 
-        with self.assertRaises(ValueError):
+        try:
             await test_func()
+        except:
+            pass
         self.assertEqual(attempt, 2)
 
     async def test_immediate_success(self):
         attempt = 0
 
-        @CallDecorator.retry(retries=3, delay=1, backoff_factor=2)
+        @CallDecorator.retry(retries=3, delay=0.1, backoff_factor=2)
         async def test_func():
             nonlocal attempt
             attempt += 1
             return "Success"
 
         result = await test_func()
         self.assertEqual(result, "Success")
         self.assertEqual(attempt, 1)
 
     async def test_retry_with_delays(self):
         attempt = 0
         start_time = time.time()
 
-        @CallDecorator.retry(retries=3, delay=1, backoff_factor=2)
+        @CallDecorator.retry(retries=3, delay=0.1, backoff_factor=2)
         async def test_func():
             nonlocal attempt
             attempt += 1
             if attempt < 3:
                 raise ValueError("Test failure")
             return "Success"
 
         result = await test_func()
         end_time = time.time()
         elapsed_time = end_time - start_time
 
         self.assertEqual(result, "Success")
         # Note: The actual delay might be slightly longer than expected due to asyncio's event loop scheduling.
         self.assertTrue(
-            elapsed_time >= 3, f"Elapsed time was {elapsed_time}, expected >= 3"
+            elapsed_time >= 0.3, f"Elapsed time was {elapsed_time}, expected >= 3"
         )
         self.assertEqual(attempt, 3)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_nested.py` & `lionagi-0.2.0/lionagi/tests/libs/test_nested.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         with self.assertRaises(LookupError):
             nget({"a": 1}, ["b"])
 
     def test_flatten_and_unflatten_dict(self):
         """Test flattening and then unflattening a nested dictionary."""
         original = {"a": {"b": {"c": 1}}}
         flattened = flatten(original)
-        self.assertEqual(flattened, {"a_b_c": 1})
+        self.assertEqual(flattened, {"a[^_^]b[^_^]c": 1})
         unflattened = unflatten(flattened)
         self.assertEqual(original, unflattened)
 
     def test_nfilter_dict(self):
         """Test filtering items in a dictionary."""
         data = {"a": 1, "b": 2, "c": 3}
         filtered = nfilter(data, lambda x: x[1] > 1)
@@ -221,84 +221,93 @@
 
 
 class TestFlatten(unittest.TestCase):
 
     def test_flatten_nested_dict(self):
         nested_dict = {"a": {"b": 1, "c": {"d": 2}}}
         result = flatten(nested_dict)
-        self.assertEqual(result, {"a_b": 1, "a_c_d": 2})
+        self.assertEqual(result, {"a[^_^]b": 1, "a[^_^]c[^_^]d": 2})
 
     def test_flatten_nested_list(self):
         nested_list = [[1, 2], [3, [4, 5]]]
         result = flatten(nested_list)
-        self.assertEqual(result, {"0_0": 1, "0_1": 2, "1_0": 3, "1_1_0": 4, "1_1_1": 5})
+        self.assertEqual(
+            result,
+            {
+                "0[^_^]0": 1,
+                "0[^_^]1": 2,
+                "1[^_^]0": 3,
+                "1[^_^]1[^_^]0": 4,
+                "1[^_^]1[^_^]1": 5,
+            },
+        )
 
     def test_flatten_with_max_depth(self):
         nested_dict = {"a": {"b": {"c": 1}}}
         result = flatten(nested_dict, max_depth=1)
-        self.assertEqual(result, {"a_b": {"c": 1}})
+        self.assertEqual(result, {"a[^_^]b": {"c": 1}})
 
     def test_flatten_dict_only(self):
         nested_mix = {"a": [1, 2], "b": {"c": 3}}
         result = flatten(nested_mix, dict_only=True)
-        self.assertEqual(result, {"a": [1, 2], "b_c": 3})
+        self.assertEqual(result, {"a": [1, 2], "b[^_^]c": 3})
 
     def test_flatten_inplace(self):
         nested_dict = {"a": {"b": 1}}
         flatten(nested_dict, inplace=True)
-        self.assertEqual(nested_dict, {"a_b": 1})
+        self.assertEqual(nested_dict, {"a[^_^]b": 1})
 
     def test_flatten_empty_structure(self):
         self.assertEqual(flatten({}), {})
         self.assertEqual(flatten([]), {})
 
     def test_flatten_deeply_nested_structure(self):
         deeply_nested = {"a": {"b": {"c": {"d": 1}}}}
         result = flatten(deeply_nested)
-        self.assertEqual(result, {"a_b_c_d": 1})
+        self.assertEqual(result, {"a[^_^]b[^_^]c[^_^]d": 1})
 
 
 class TestUnflatten(unittest.TestCase):
 
     def test_unflatten_to_nested_dict(self):
-        flat_dict = {"a_b": 1, "a_c_d": 2}
+        flat_dict = {"a[^_^]b": 1, "a[^_^]c[^_^]d": 2}
         result = unflatten(flat_dict)
         self.assertEqual(result, {"a": {"b": 1, "c": {"d": 2}}})
 
     def test_unflatten_to_nested_list(self):
-        flat_dict = {"0_0": 1, "0_1": 2, "1": [3, 4]}
+        flat_dict = {"0[^_^]0": 1, "0[^_^]1": 2, "1": [3, 4]}
         result = unflatten(flat_dict)
         self.assertEqual(result, [[1, 2], [3, 4]])
 
     def test_unflatten_with_custom_separator(self):
         flat_dict = {"a-b": 1, "a-c-d": 2}
         result = unflatten(flat_dict, sep="-")
         self.assertEqual(result, {"a": {"b": 1, "c": {"d": 2}}})
 
     def test_unflatten_with_custom_logic(self):
-        flat_dict = {"a_1": "one", "a_2": "two"}
+        flat_dict = {"a[^_^]1": "one", "a[^_^]2": "two"}
         custom_logic = lambda key: int(key) if key.isdigit() else key
         result = unflatten(flat_dict, custom_logic=custom_logic)
         self.assertEqual(result, {"a": [None, "one", "two"]})
 
     def test_unflatten_with_max_depth(self):
-        flat_dict = {"a_b_c": 1, "a_b_d": 2}
+        flat_dict = {"a[^_^]b[^_^]c": 1, "a[^_^]b[^_^]d": 2}
         result = unflatten(flat_dict, max_depth=1)
-        self.assertEqual(result, {"a": {"b_c": 1, "b_d": 2}})
+        self.assertEqual(result, {"a": {"b[^_^]c": 1, "b[^_^]d": 2}})
 
     def test_unflatten_with_max_depth_int(self):
-        flat_dict = {"0_0_0": 1, "0_1_0": 2}
+        flat_dict = {"0[^_^]0[^_^]0": 1, "0[^_^]1[^_^]0": 2}
         result = unflatten(flat_dict, max_depth=1)
-        self.assertEqual(result, [[{"0_0": 1}, {"1_0": 2}]])
+        self.assertEqual(result, [[{"0[^_^]0": 1}, {"1[^_^]0": 2}]])
 
     def test_unflatten_empty_flat_dict(self):
         self.assertEqual(unflatten({}), [])
 
     def test_unflatten_to_mixed_structure(self):
-        flat_dict = {"0_0": 1, "1_key": 2}
+        flat_dict = {"0[^_^]0": 1, "1[^_^]key": 2}
         result = unflatten(flat_dict)
         self.assertEqual(result, [[1], {"key": 2}])
 
 
 class TestNInsert(unittest.TestCase):
 
     def test_insert_into_nested_dict(self):
@@ -315,52 +324,58 @@
         obj = {"a": [{}]}
         ninsert(obj, ["a", 0, "b"], 2)
         self.assertEqual(obj, {"a": [{"b": 2}]})
 
     def test_insert_with_max_depth(self):
         obj = {}
         ninsert(obj, ["a", "b", "c"], "value", max_depth=1)
-        self.assertEqual(obj, {"a": {"b_c": "value"}})
+        self.assertEqual(obj, {"a": {"b[^_^]c": "value"}})
 
     def test_insert_into_empty_structure(self):
         obj = {}
         ninsert(obj, ["a"], 1)
         self.assertEqual(obj, {"a": 1})
 
 
 class TestGetFlattenedKeys(unittest.TestCase):
 
     def test_get_keys_from_nested_dict(self):
         nested_dict = {"a": {"b": 1, "c": {"d": 2}}}
-        expected_keys = ["a_b", "a_c_d"]
+        expected_keys = ["a[^_^]b", "a[^_^]c[^_^]d"]
         self.assertEqual(set(get_flattened_keys(nested_dict)), set(expected_keys))
 
     def test_get_keys_from_nested_list(self):
         nested_list = [[1, 2], [3, [4, 5]]]
-        expected_keys = ["0_0", "0_1", "1_0", "1_1_0", "1_1_1"]
+        expected_keys = [
+            "0[^_^]0",
+            "0[^_^]1",
+            "1[^_^]0",
+            "1[^_^]1[^_^]0",
+            "1[^_^]1[^_^]1",
+        ]
         self.assertEqual(set(get_flattened_keys(nested_list)), set(expected_keys))
 
     def test_get_keys_with_max_depth(self):
         nested_dict = {"a": {"b": {"c": 1}}}
-        expected_keys = ["a_b"]
+        expected_keys = ["a[^_^]b"]
         self.assertEqual(
             set(get_flattened_keys(nested_dict, max_depth=1)), set(expected_keys)
         )
 
     def test_get_keys_dict_only(self):
         nested_mix = {"a": [1, 2], "b": {"c": 3}}
-        expected_keys = ["a", "b_c"]
+        expected_keys = ["a", "b[^_^]c"]
         self.assertEqual(
             set(get_flattened_keys(nested_mix, dict_only=True)), set(expected_keys)
         )
 
     def test_get_keys_from_empty_structure(self):
         self.assertEqual(get_flattened_keys({}), [])
 
     def test_keys_from_deeply_nested_structure(self):
         deeply_nested = {"a": {"b": {"c": {"d": 1}}}}
-        expected_keys = ["a_b_c_d"]
+        expected_keys = ["a[^_^]b[^_^]c[^_^]d"]
         self.assertEqual(set(get_flattened_keys(deeply_nested)), set(expected_keys))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_parse.py` & `lionagi-0.2.0/lionagi/tests/libs/test_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             ParseUtil.escape_chars_in_json("Line 1\nLine 2"), "Line 1\\nLine 2"
         )
         self.assertEqual(ParseUtil.escape_chars_in_json('Quote: "'), 'Quote: \\"')
 
     def test_extract_code_block(self):
         """Test extracting and parsing code blocks from Markdown."""
         markdown = '```python\nprint("Hello, world!")\n```'
-        result = ParseUtil.extract_code_block(
+        result = ParseUtil.extract_json_block(
             markdown, language="python", parser=lambda x: x
         )
         self.assertEqual(result, 'print("Hello, world!")')
 
     def test_md_to_json(self):
         """Test extracting and validating JSON from Markdown content."""
         markdown = '```json\n{"key": "value"}\n```'
```

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_queue.py` & `lionagi-0.2.0/lionagi/tests/libs/test_queue.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi/tests/libs/test_sys_util.py` & `lionagi-0.2.0/lionagi/tests/libs/test_sys_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/lionagi.egg-info/SOURCES.txt` & `lionagi-0.2.0/lionagi.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -7,129 +7,154 @@
 lionagi/version.py
 lionagi.egg-info/PKG-INFO
 lionagi.egg-info/SOURCES.txt
 lionagi.egg-info/dependency_links.txt
 lionagi.egg-info/requires.txt
 lionagi.egg-info/top_level.txt
 lionagi/core/__init__.py
+lionagi/core/_setting/__init__.py
+lionagi/core/_setting/_setting.py
+lionagi/core/action/__init__.py
+lionagi/core/action/function_calling.py
+lionagi/core/action/manual.py
+lionagi/core/action/node.py
+lionagi/core/action/tool.py
+lionagi/core/action/tool_manager.py
 lionagi/core/agent/__init__.py
 lionagi/core/agent/base_agent.py
-lionagi/core/branch/__init__.py
-lionagi/core/branch/base.py
-lionagi/core/branch/branch.py
-lionagi/core/branch/executable_branch.py
-lionagi/core/branch/flow_mixin.py
-lionagi/core/branch/util.py
-lionagi/core/direct/__init__.py
-lionagi/core/direct/cot.py
-lionagi/core/direct/plan.py
-lionagi/core/direct/predict.py
-lionagi/core/direct/react.py
-lionagi/core/direct/score.py
-lionagi/core/direct/select.py
-lionagi/core/direct/sentiment.py
-lionagi/core/direct/utils.py
-lionagi/core/direct/vote.py
-lionagi/core/execute/__init__.py
-lionagi/core/execute/base_executor.py
-lionagi/core/execute/branch_executor.py
-lionagi/core/execute/instruction_map_executor.py
-lionagi/core/execute/neo4j_executor.py
-lionagi/core/execute/structure_executor.py
-lionagi/core/flow/__init__.py
-lionagi/core/flow/baseflow.py
-lionagi/core/flow/mono_chat_mixin.py
-lionagi/core/flow/monoflow/ReAct.py
-lionagi/core/flow/monoflow/__init__.py
-lionagi/core/flow/monoflow/chat.py
-lionagi/core/flow/monoflow/chat_mixin.py
-lionagi/core/flow/monoflow/followup.py
-lionagi/core/flow/polyflow/__init__.py
-lionagi/core/flow/polyflow/chat.py
-lionagi/core/form/__init__.py
-lionagi/core/form/action_form.py
-lionagi/core/form/field_validator.py
-lionagi/core/form/form.py
-lionagi/core/form/mixin.py
-lionagi/core/form/scored_form.py
+lionagi/core/agent/eval/__init__.py
+lionagi/core/agent/eval/evaluator.py
+lionagi/core/agent/eval/vote.py
+lionagi/core/agent/learn/__init__.py
+lionagi/core/agent/learn/learner.py
+lionagi/core/agent/plan/__init__.py
+lionagi/core/agent/plan/plan.py
+lionagi/core/agent/plan/unit_template.py
+lionagi/core/collections/__init__.py
+lionagi/core/collections/_logger.py
+lionagi/core/collections/exchange.py
+lionagi/core/collections/flow.py
+lionagi/core/collections/model.py
+lionagi/core/collections/pile.py
+lionagi/core/collections/progression.py
+lionagi/core/collections/util.py
+lionagi/core/collections/abc/__init__.py
+lionagi/core/collections/abc/component.py
+lionagi/core/collections/abc/concepts.py
+lionagi/core/collections/abc/exceptions.py
+lionagi/core/collections/abc/util.py
+lionagi/core/director/__init__.py
+lionagi/core/director/direct.py
+lionagi/core/director/director.py
+lionagi/core/engine/__init__.py
+lionagi/core/engine/branch_engine.py
+lionagi/core/engine/instruction_map_engine.py
+lionagi/core/engine/sandbox_.py
+lionagi/core/engine/script_engine.py
+lionagi/core/executor/__init__.py
+lionagi/core/executor/base_executor.py
+lionagi/core/executor/graph_executor.py
+lionagi/core/executor/neo4j_executor.py
 lionagi/core/generic/__init__.py
-lionagi/core/generic/action.py
-lionagi/core/generic/component.py
-lionagi/core/generic/condition.py
-lionagi/core/generic/data_logger.py
 lionagi/core/generic/edge.py
-lionagi/core/generic/mail.py
-lionagi/core/generic/mailbox.py
+lionagi/core/generic/edge_condition.py
+lionagi/core/generic/graph.py
+lionagi/core/generic/hyperedge.py
 lionagi/core/generic/node.py
-lionagi/core/generic/relation.py
-lionagi/core/generic/signal.py
-lionagi/core/generic/structure.py
-lionagi/core/generic/transfer.py
-lionagi/core/generic/work.py
-lionagi/core/graph/__init__.py
-lionagi/core/graph/graph.py
-lionagi/core/graph/tree.py
+lionagi/core/generic/tree.py
+lionagi/core/generic/tree_node.py
 lionagi/core/mail/__init__.py
+lionagi/core/mail/mail.py
 lionagi/core/mail/mail_manager.py
-lionagi/core/mail/schema.py
-lionagi/core/messages/__init__.py
-lionagi/core/messages/schema.py
+lionagi/core/mail/package.py
+lionagi/core/mail/start_mail.py
+lionagi/core/message/__init__.py
+lionagi/core/message/action_request.py
+lionagi/core/message/action_response.py
+lionagi/core/message/assistant_response.py
+lionagi/core/message/instruction.py
+lionagi/core/message/message.py
+lionagi/core/message/system.py
+lionagi/core/message/util.py
+lionagi/core/report/__init__.py
+lionagi/core/report/base.py
+lionagi/core/report/form.py
+lionagi/core/report/report.py
+lionagi/core/report/util.py
+lionagi/core/rule/__init__.py
+lionagi/core/rule/_default.py
+lionagi/core/rule/action.py
+lionagi/core/rule/base.py
+lionagi/core/rule/boolean.py
+lionagi/core/rule/choice.py
+lionagi/core/rule/mapping.py
+lionagi/core/rule/number.py
+lionagi/core/rule/rulebook.py
+lionagi/core/rule/string.py
+lionagi/core/rule/util.py
 lionagi/core/session/__init__.py
+lionagi/core/session/branch.py
+lionagi/core/session/directive_mixin.py
 lionagi/core/session/session.py
-lionagi/core/tool/__init__.py
-lionagi/core/tool/tool.py
-lionagi/core/tool/tool_manager.py
+lionagi/core/structure/__init__.py
+lionagi/core/structure/chain.py
+lionagi/core/structure/forest.py
+lionagi/core/structure/graph.py
+lionagi/core/structure/tree.py
+lionagi/core/unit/__init__.py
+lionagi/core/unit/parallel_unit.py
+lionagi/core/unit/unit.py
+lionagi/core/unit/unit_form.py
+lionagi/core/unit/unit_mixin.py
+lionagi/core/unit/util.py
+lionagi/core/unit/template/__init__.py
+lionagi/core/unit/template/action.py
+lionagi/core/unit/template/base.py
+lionagi/core/unit/template/plan.py
+lionagi/core/unit/template/predict.py
+lionagi/core/unit/template/score.py
+lionagi/core/unit/template/select.py
+lionagi/core/validator/__init__.py
+lionagi/core/validator/validator.py
+lionagi/core/work/__init__.py
+lionagi/core/work/work.py
+lionagi/core/work/work_function.py
+lionagi/core/work/work_queue.py
+lionagi/core/work/worker.py
+lionagi/core/work/worklog.py
 lionagi/experimental/__init__.py
+lionagi/experimental/compressor/__init__.py
+lionagi/experimental/compressor/base.py
+lionagi/experimental/compressor/llm_compressor.py
+lionagi/experimental/compressor/llm_summarizer.py
+lionagi/experimental/compressor/util.py
 lionagi/experimental/directive/__init__.py
-lionagi/experimental/directive/schema.py
-lionagi/experimental/directive/evaluator/__init__.py
-lionagi/experimental/directive/evaluator/ast_evaluator.py
-lionagi/experimental/directive/evaluator/base_evaluator.py
-lionagi/experimental/directive/evaluator/sandbox_.py
-lionagi/experimental/directive/evaluator/script_engine.py
+lionagi/experimental/directive/tokenizer.py
 lionagi/experimental/directive/parser/__init__.py
 lionagi/experimental/directive/parser/base_parser.py
-lionagi/experimental/directive/template_/__init__.py
-lionagi/experimental/directive/template_/base_template.py
-lionagi/experimental/report/__init__.py
-lionagi/experimental/report/form.py
-lionagi/experimental/report/report.py
-lionagi/experimental/report/util.py
-lionagi/experimental/tool/__init__.py
-lionagi/experimental/tool/function_calling.py
-lionagi/experimental/tool/manual.py
-lionagi/experimental/tool/schema.py
-lionagi/experimental/tool/tool_manager.py
-lionagi/experimental/tool/util.py
-lionagi/experimental/validator/__init__.py
-lionagi/experimental/validator/rule.py
-lionagi/experimental/validator/validator.py
-lionagi/experimental/work/__init__.py
-lionagi/experimental/work/async_queue.py
-lionagi/experimental/work/schema.py
-lionagi/experimental/work/work_function.py
-lionagi/experimental/work/worker.py
-lionagi/experimental/work2/__init__.py
-lionagi/experimental/work2/form.py
-lionagi/experimental/work2/report.py
-lionagi/experimental/work2/schema.py
-lionagi/experimental/work2/tests.py
-lionagi/experimental/work2/util.py
-lionagi/experimental/work2/work.py
-lionagi/experimental/work2/work_function.py
-lionagi/experimental/work2/worker.py
+lionagi/experimental/directive/template/__init__.py
+lionagi/experimental/directive/template/base_template.py
+lionagi/experimental/directive/template/schema.py
+lionagi/experimental/evaluator/__init__.py
+lionagi/experimental/evaluator/ast_evaluator.py
+lionagi/experimental/evaluator/base_evaluator.py
+lionagi/experimental/knowledge/__init__.py
+lionagi/experimental/knowledge/base.py
+lionagi/experimental/knowledge/graph.py
+lionagi/experimental/memory/__init__.py
+lionagi/experimental/strategies/__init__.py
+lionagi/experimental/strategies/base.py
 lionagi/integrations/__init__.py
 lionagi/integrations/bridge/__init__.py
 lionagi/integrations/bridge/autogen_/__init__.py
 lionagi/integrations/bridge/autogen_/autogen_.py
 lionagi/integrations/bridge/langchain_/__init__.py
 lionagi/integrations/bridge/langchain_/documents.py
 lionagi/integrations/bridge/langchain_/langchain_bridge.py
 lionagi/integrations/bridge/llamaindex_/__init__.py
-lionagi/integrations/bridge/llamaindex_/get_index.py
 lionagi/integrations/bridge/llamaindex_/index.py
 lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
 lionagi/integrations/bridge/llamaindex_/llama_pack.py
 lionagi/integrations/bridge/llamaindex_/node_parser.py
 lionagi/integrations/bridge/llamaindex_/reader.py
 lionagi/integrations/bridge/llamaindex_/textnode.py
 lionagi/integrations/bridge/pydantic_/__init__.py
@@ -143,14 +168,15 @@
 lionagi/integrations/config/oai_configs.py
 lionagi/integrations/config/ollama_configs.py
 lionagi/integrations/config/openrouter_configs.py
 lionagi/integrations/loader/__init__.py
 lionagi/integrations/loader/load.py
 lionagi/integrations/loader/load_util.py
 lionagi/integrations/provider/__init__.py
+lionagi/integrations/provider/_mapping.py
 lionagi/integrations/provider/litellm.py
 lionagi/integrations/provider/mistralai.py
 lionagi/integrations/provider/mlx_service.py
 lionagi/integrations/provider/oai.py
 lionagi/integrations/provider/ollama.py
 lionagi/integrations/provider/openrouter.py
 lionagi/integrations/provider/services.py
@@ -160,52 +186,60 @@
 lionagi/integrations/storage/storage_util.py
 lionagi/integrations/storage/structure_excel.py
 lionagi/integrations/storage/to_csv.py
 lionagi/integrations/storage/to_excel.py
 lionagi/libs/__init__.py
 lionagi/libs/ln_api.py
 lionagi/libs/ln_async.py
+lionagi/libs/ln_context.py
 lionagi/libs/ln_convert.py
 lionagi/libs/ln_dataframe.py
 lionagi/libs/ln_func_call.py
+lionagi/libs/ln_image.py
 lionagi/libs/ln_knowledge_graph.py
 lionagi/libs/ln_nested.py
 lionagi/libs/ln_parse.py
 lionagi/libs/ln_queue.py
-lionagi/libs/ln_tokenizer.py
+lionagi/libs/ln_tokenize.py
 lionagi/libs/ln_validate.py
+lionagi/libs/special_tokens.py
 lionagi/libs/sys_util.py
 lionagi/lions/__init__.py
 lionagi/lions/coder/__init__.py
 lionagi/lions/coder/add_feature.py
 lionagi/lions/coder/base_prompts.py
+lionagi/lions/coder/code_form.py
 lionagi/lions/coder/coder.py
 lionagi/lions/coder/util.py
 lionagi/lions/researcher/__init__.py
 lionagi/lions/researcher/data_source/__init__.py
 lionagi/lions/researcher/data_source/finhub_.py
 lionagi/lions/researcher/data_source/google_.py
 lionagi/lions/researcher/data_source/wiki_.py
 lionagi/lions/researcher/data_source/yfinance_.py
 lionagi/tests/__init__.py
 lionagi/tests/integrations/__init__.py
 lionagi/tests/libs/__init__.py
 lionagi/tests/libs/test_api.py
-lionagi/tests/libs/test_async.py
 lionagi/tests/libs/test_convert.py
 lionagi/tests/libs/test_field_validators.py
 lionagi/tests/libs/test_func_call.py
 lionagi/tests/libs/test_nested.py
 lionagi/tests/libs/test_parse.py
 lionagi/tests/libs/test_queue.py
 lionagi/tests/libs/test_sys_util.py
 lionagi/tests/test_core/__init__.py
-lionagi/tests/test_core/test_base_branch.py
 lionagi/tests/test_core/test_branch.py
-lionagi/tests/test_core/test_chat_flow.py
-lionagi/tests/test_core/test_mail_manager.py
-lionagi/tests/test_core/test_prompts.py
-lionagi/tests/test_core/test_session.py
-lionagi/tests/test_core/test_session_base_util.py
-lionagi/tests/test_core/test_tool_manager.py
+lionagi/tests/test_core/test_form.py
+lionagi/tests/test_core/test_report.py
+lionagi/tests/test_core/test_validator.py
+lionagi/tests/test_core/collections/__init__.py
+lionagi/tests/test_core/collections/test_component.py
+lionagi/tests/test_core/collections/test_exchange.py
+lionagi/tests/test_core/collections/test_flow.py
+lionagi/tests/test_core/collections/test_pile.py
+lionagi/tests/test_core/collections/test_progression.py
 lionagi/tests/test_core/generic/__init__.py
-lionagi/tests/test_core/generic/test_component.py
+lionagi/tests/test_core/generic/test_edge.py
+lionagi/tests/test_core/generic/test_graph.py
+lionagi/tests/test_core/generic/test_node.py
+lionagi/tests/test_core/generic/test_tree_node.py
```

### Comparing `lionagi-0.1.2/pyproject.toml` & `lionagi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.2/setup.py` & `lionagi-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "pandas",
 ]
 
 setuptools.setup(
     name="lionagi",
     version=__version__,
     author="HaiyangLi",
-    author_email="ocean@lionagi.ai",
+    author_email="quantocean.li@gmail.com",
     description="Towards automated general intelligence.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=["lionagi*"]),
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python :: 3",
```

