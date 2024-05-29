# Comparing `tmp/forestadmin_agent_toolkit-1.8.2.tar.gz` & `tmp/forestadmin_agent_toolkit-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_toolkit-1.8.2.tar", max compression
+gzip compressed data, was "forestadmin_agent_toolkit-1.8.3.tar", max compression
```

## Comparing `forestadmin_agent_toolkit-1.8.2.tar` & `forestadmin_agent_toolkit-1.8.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/__init__.py
--rw-r--r--   0        0        0     9526 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/agent.py
--rw-r--r--   0        0        0      135 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/exceptions.py
--rw-r--r--   0        0        0     2477 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/forest_logger.py
--rw-r--r--   0        0        0     4152 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/options.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/__init__.py
--rw-r--r--   0        0        0     2305 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/requests.py
--rw-r--r--   0        0        0     9544 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/resources.py
--rw-r--r--   0        0        0      464 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/base.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/__init__.py
--rw-r--r--   0        0        0     1055 2024-05-23 09:47:35.808490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
--rw-r--r--   0        0        0     2780 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_collection.py
--rw-r--r--   0        0        0     1912 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
--rw-r--r--   0        0        0    17490 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud.py
--rw-r--r--   0        0        0    22065 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud_related.py
--rw-r--r--   0        0        0     4348 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/decorators.py
--rw-r--r--   0        0        0      148 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/exceptions.py
--rw-r--r--   0        0        0    13206 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/filter.py
--rw-r--r--   0        0        0     5509 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/requests.py
--rw-r--r--   0        0        0    12193 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/stats.py
--rw-r--r--   0        0        0      935 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/__init__.py
--rw-r--r--   0        0        0      427 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/exceptions.py
--rw-r--r--   0        0        0     4696 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/resources.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/__init__.py
--rw-r--r--   0        0        0     1695 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
--rw-r--r--   0        0        0      176 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/options.py
--rw-r--r--   0        0        0     9001 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permission_service.py
--rw-r--r--   0        0        0     3261 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
--rw-r--r--   0        0        0      406 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_types.py
--rw-r--r--   0        0        0     5276 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
--rw-r--r--   0        0        0     3200 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
--rw-r--r--   0        0        0     1010 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/__init__.py
--rw-r--r--   0        0        0    10346 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/json_api.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     3663 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/authentication.py
--rw-r--r--   0        0        0     4554 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context.py
--rw-r--r--   0        0        0     1252 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_injector.py
--rw-r--r--   0        0        0      655 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
--rw-r--r--   0        0        0     1230 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variables.py
--rw-r--r--   0        0        0     1661 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/csv.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
--rw-r--r--   0        0        0     6276 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
--rw-r--r--   0        0        0     4229 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
--rw-r--r--   0        0        0     2298 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
--rw-r--r--   0        0        0     5069 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
--rw-r--r--   0        0        0    13958 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
--rw-r--r--   0        0        0     2461 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
--rw-r--r--   0        0        0     8646 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
--rw-r--r--   0        0        0      506 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
--rw-r--r--   0        0        0     9931 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/type.py
--rw-r--r--   0        0        0     1281 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/validation.py
--rw-r--r--   0        0        0     7303 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/http.py
--rw-r--r--   0        0        0     1774 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/id.py
--rw-r--r--   0        0        0     1889 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
--rw-r--r--   0        0        0      513 2024-05-23 09:47:35.812490 forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/token.py
--rw-r--r--   0        0        0     1776 2024-05-23 09:47:50.548705 forestadmin_agent_toolkit-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.056268 forestadmin_agent_toolkit-1.8.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/__init__.py
+-rw-r--r--   0        0        0     9526 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/agent.py
+-rw-r--r--   0        0        0      135 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/exceptions.py
+-rw-r--r--   0        0        0     2477 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/forest_logger.py
+-rw-r--r--   0        0        0     4152 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/options.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/actions/__init__.py
+-rw-r--r--   0        0        0     2305 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/actions/requests.py
+-rw-r--r--   0        0        0     9544 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/actions/resources.py
+-rw-r--r--   0        0        0      464 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/base.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1055 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py
+-rw-r--r--   0        0        0     2780 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/charts_collection.py
+-rw-r--r--   0        0        0     1912 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py
+-rw-r--r--   0        0        0    17490 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/crud.py
+-rw-r--r--   0        0        0    22065 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/crud_related.py
+-rw-r--r--   0        0        0     4348 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/decorators.py
+-rw-r--r--   0        0        0      148 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/exceptions.py
+-rw-r--r--   0        0        0    13206 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/filter.py
+-rw-r--r--   0        0        0     5509 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/requests.py
+-rw-r--r--   0        0        0    12193 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/stats.py
+-rw-r--r--   0        0        0      935 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/ip_white_list_resource.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/security/__init__.py
+-rw-r--r--   0        0        0      427 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/security/exceptions.py
+-rw-r--r--   0        0        0     4696 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/security/resources.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py
+-rw-r--r--   0        0        0      176 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/options.py
+-rw-r--r--   0        0        0     8943 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/permission_service.py
+-rw-r--r--   0        0        0     3261 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/permissions_functions.py
+-rw-r--r--   0        0        0      406 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/permissions_types.py
+-rw-r--r--   0        0        0     5276 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py
+-rw-r--r--   0        0        0     3200 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py
+-rw-r--r--   0        0        0     1010 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/serializers/__init__.py
+-rw-r--r--   0        0        0    10346 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/serializers/json_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     3663 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/authentication.py
+-rw-r--r--   0        0        0     4554 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context.py
+-rw-r--r--   0        0        0     1252 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variable_injector.py
+-rw-r--r--   0        0        0      655 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variable_instantiator.py
+-rw-r--r--   0        0        0     1230 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variables.py
+-rw-r--r--   0        0        0     1661 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/csv.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/__init__.py
+-rw-r--r--   0        0        0     5746 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/action_fields.py
+-rw-r--r--   0        0        0     6276 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py
+-rw-r--r--   0        0        0     4229 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py
+-rw-r--r--   0        0        0     2298 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py
+-rw-r--r--   0        0        0     5032 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py
+-rw-r--r--   0        0        0    14186 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py
+-rw-r--r--   0        0        0     2294 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py
+-rw-r--r--   0        0        0     8549 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py
+-rw-r--r--   0        0        0      506 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_segment.py
+-rw-r--r--   0        0        0     9587 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/type.py
+-rw-r--r--   0        0        0     1281 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/validation.py
+-rw-r--r--   0        0        0     7303 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/http.py
+-rw-r--r--   0        0        0     1774 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/id.py
+-rw-r--r--   0        0        0     1889 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/ip_whitelist_util.py
+-rw-r--r--   0        0        0      513 2024-05-29 07:53:14.060268 forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/token.py
+-rw-r--r--   0        0        0     1776 2024-05-29 07:53:28.852288 forestadmin_agent_toolkit-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 forestadmin_agent_toolkit-1.8.3/PKG-INFO
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/agent.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/forest_logger.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/forest_logger.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/options.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/options.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/requests.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/actions/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/actions/resources.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/actions/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/base_collection_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_collection.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/charts_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/charts_datasource.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/charts_datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/crud_related.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/decorators.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/decorators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/filter.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/filter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/requests.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/collections/stats.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/collections/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/ip_white_list_resource.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/ip_white_list_resource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/resources/security/resources.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/resources/security/resources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/ip_whitelist_service.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permission_service.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/permission_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,10 +193,9 @@
         if len(actions) == 0:
             return None
 
         actions = [
             action
             for action in actions
             if action["id"] == f"{collection.name}-{get_params['action_name']}-{get_params['slug']}"
-            and http_method.value == action["httpMethod"]
         ]
         return actions[0] if len(actions) > 0 else None
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/permissions_functions.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/permissions_functions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/smart_actions_checker.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/permissions/sse_cache_invalidation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/__init__.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/services/serializers/json_api.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/services/serializers/json_api.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/authentication.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_injector.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variable_injector.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variable_instantiator.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variable_instantiator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/context_variables.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/context_variables.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/csv.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/csv.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/action_values.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/action_values.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/emitter.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/emitter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/filterable.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/filterable.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union, cast
+from typing import List, Literal, Union, cast
 
 from forestadmin.agent_toolkit.utils.forest_schema.action_values import ForestValueConverter
 from forestadmin.agent_toolkit.utils.forest_schema.generator_action_field_widget import GeneratorActionFieldWidget
 from forestadmin.agent_toolkit.utils.forest_schema.generator_field import SchemaFieldGenerator
 from forestadmin.agent_toolkit.utils.forest_schema.type import ForestServerAction, ForestServerActionField
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
@@ -21,33 +21,30 @@
             defaultValue="Form is loading",
             value=None,
             description="",
             enums=None,
             hook=None,
             isRequired=False,
             reference=None,
-            widget=None,
+            widgetEdit=None,
         )
     ]
 
     @classmethod
     async def build(
         cls, prefix: str, collection: Union[Collection, CollectionCustomizer], name: str
     ) -> ForestServerAction:
         schema = collection.schema["actions"][name]
         idx = list(collection.schema["actions"].keys()).index(name)
         slug = name.lower().replace(r"[^a-z0-9-]+", "-")
         return ForestServerAction(
             id=f"{collection.name}-{idx}-{slug}",
             name=name,
-            type=schema.scope.value.lower(),
-            baseUrl=None,
+            type=cast(Literal["single", "bulk", "global"], schema.scope.value.lower()),
             endpoint=f"/forest/_actions/{collection.name}/{idx}/{slug}",
-            httpMethod="POST",
-            redirect=None,
             download=bool(schema.generate_file),
             fields=await cls.build_fields(collection, schema, name),
             # Always registering the change hook has no consequences, even if we don't use it.
             hooks={"load": not schema.static_form, "change": ["changeHook"]},
         )
 
     @classmethod
@@ -58,23 +55,22 @@
         default_value = ForestValueConverter.value_to_forest(field, field["default_value"])
         output: ForestServerActionField = {
             "field": field["label"],
             "value": value,
             # When sending to server, we need to rename 'value' into 'defaultValue'
             # otherwise, it does not gets applied 🤷‍♂️
             "defaultValue": default_value,
-            "description": field["description"],
+            "description": field.get("description"),
             "enums": None,
             "hook": None,
             "isReadOnly": field.get("is_read_only", False),
             "isRequired": field.get("is_required", True),
             "reference": None,
             "type": PrimitiveType.STRING,
-            "widget": None,
-            "widgetEdit": GeneratorActionFieldWidget.build_widget_options(field),
+            "widgetEdit": GeneratorActionFieldWidget.build_widget_options(field),  # type:ignore
         }
         if field["type"] == ActionFieldType.COLLECTION:
             collection: Collection = datasource.get_collection(field["collection_name"])  # type: ignore
             pk = SchemaUtils.get_primary_keys(collection.schema)[0]
             pk_schema = cast(Column, collection.get_field(pk))
             output["type"] = SchemaFieldGenerator.build_column_type(pk_schema["column_type"])  # type: ignore
             output["reference"] = f"{collection.name}.{pk}"
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_action_field_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from datetime import date
 from typing import Literal, Union
 
 from forestadmin.agent_toolkit.utils.forest_schema.action_fields import ActionFields
 from forestadmin.agent_toolkit.utils.forest_schema.type import (
+    ForestServerActionFieldAddressAutocompleteEditorOptions,
     ForestServerActionFieldCheckboxGroupOptions,
     ForestServerActionFieldCheckboxOptions,
     ForestServerActionFieldColorPickerOptions,
     ForestServerActionFieldCurrencyInputEditorOptions,
     ForestServerActionFieldDatePickerOptions,
     ForestServerActionFieldDropdownOptions,
     ForestServerActionFieldFilePickerEditorOptions,
@@ -126,15 +127,15 @@
     def build_text_area_widget_edit(
         field: PlainStringDynamicFieldTextAreaWidget,
     ) -> ForestServerActionFieldTextAreaEditorOptions:
         return {
             "name": "text area editor",
             "parameters": {
                 "placeholder": field.get("placeholder"),
-                "rows": int(field["rows"]) if field.get("rows") else None,
+                "rows": int(field["rows"]) if field.get("rows") is not None else None,
             },
         }
 
     @staticmethod
     def build_rich_text_widget_edit(
         field: PlainStringDynamicFieldRichTextWidget,
     ) -> ForestServerActionFieldRichTextEditorOptions:
@@ -144,15 +145,15 @@
                 "placeholder": field.get("placeholder"),
             },
         }
 
     @staticmethod
     def build_address_autocomplete_widget_edit(
         field: PlainStringDynamicFieldAddressAutocompleteWidget,
-    ) -> ForestServerActionFieldRichTextEditorOptions:
+    ) -> ForestServerActionFieldAddressAutocompleteEditorOptions:
         return {
             "name": "address editor",
             "parameters": {
                 "placeholder": field.get("placeholder"),
             },
         }
 
@@ -160,29 +161,29 @@
     def build_number_input_widget_edit(
         field: PlainNumberDynamicFieldNumberInputWidget,
     ) -> ForestServerActionFieldNumberInputEditorOptions:
         return {
             "name": "number input",
             "parameters": {
                 "placeholder": field.get("placeholder"),
-                "min": field.get("min"),
-                "max": field.get("max"),
-                "step": field.get("step"),
+                "min": field.get("min"),  #  type:ignore
+                "max": field.get("max"),  #  type:ignore
+                "step": field.get("step"),  #  type:ignore
             },
         }
 
     @staticmethod
     def build_currency_input_widget_edit(
         field: PlainNumberDynamicFieldCurrencyInputWidget,
     ) -> ForestServerActionFieldCurrencyInputEditorOptions:
         return {
             "name": "price editor",
             "parameters": {
                 "placeholder": field.get("placeholder"),
-                "min": field.get("min"),
+                "min": field.get("min"),  #  type:ignore
                 "max": field.get("max"),
                 "step": field.get("step"),
                 "currency": (
                     field["currency"]
                     if isinstance(field.get("currency"), str) and len(field["currency"]) == 3
                     else None
                 ),
@@ -206,15 +207,15 @@
     def build_number_input_list_widget_edit(
         field: PlainListNumberDynamicFieldNumberInputListWidget,
     ) -> ForestServerActionFieldNumberInputListEditorOptions:
         return {
             "name": "input array",
             "parameters": {
                 "placeholder": field.get("placeholder"),
-                "min": field.get("min"),
+                "min": field.get("min"),  # type: ignore
                 "max": field.get("max"),
                 "step": field.get("step"),
                 "allowDuplicate": field.get("allow_duplicates", False),
                 "enableReorder": field.get("enable_reorder", True),
             },
         }
 
@@ -227,29 +228,29 @@
     @staticmethod
     def build_file_picker_widget_edit(
         field: Union[PlainFileDynamicFieldFilePickerWidget, PlainFileListDynamicFieldFilePickerWidget],
     ) -> ForestServerActionFieldFilePickerEditorOptions:
         return {
             "name": "file picker",
             "parameters": {
-                "prefix": None,
+                "prefix": None,  # type:ignore
                 "filesExtensions": field.get("extensions", None),
                 "filesCountLimit": field.get("max_count"),
                 "filesSizeLimit": field.get("max_size_mb"),
             },
         }
 
     @staticmethod
     def build_date_picker_widget_edit(
         field: Union[PlainDateDynamicFieldDatePickerWidget, PlainDateOnlyDynamicFieldDatePickerWidget],
     ) -> ForestServerActionFieldDatePickerOptions:
         return {
             "name": "date editor",
             "parameters": {
-                "format": field.get("format"),
+                "format": field.get("format"),  # type:ignore
                 "placeholder": field.get("placeholder"),
                 "minDate": field["min"].isoformat() if isinstance(field.get("min"), date) else None,
                 "maxDate": field["max"].isoformat() if isinstance(field.get("max"), date) else None,
             },
         }
 
     @staticmethod
@@ -279,15 +280,15 @@
         ForestServerActionFieldRadioGroupOptions[int],
         ForestServerActionFieldRadioGroupOptions[float],
         ForestServerActionFieldRadioGroupOptions[str],
     ]:
         return {
             "name": "radio button",
             "parameters": {
-                "static": {
+                "static": {  # type:ignore
                     "options": field.get("options", []),
                 },
             },
         }
 
     @staticmethod
     def build_checkbox_group_widget_edit(
@@ -298,15 +299,15 @@
         ForestServerActionFieldCheckboxGroupOptions[int],
         ForestServerActionFieldCheckboxGroupOptions[float],
         ForestServerActionFieldCheckboxGroupOptions[str],
     ]:
         return {
             "name": "checkboxes",
             "parameters": {
-                "static": {
+                "static": {  # type:ignore
                     "options": field.get("options", []),
                 },
             },
         }
 
     @staticmethod
     def build_dropdown_widget_edit(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_collection.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,24 +21,19 @@
                 # ignore foreign key because we have relationships, except when the fk is pk
                 continue
             fields.append(SchemaFieldGenerator.build(collection, field_name))
         fields = sorted(fields, key=lambda field: field["field"])
 
         return {
             "name": collection.name,
-            "isVirtual": False,
-            "icon": None,
             "isReadOnly": all(
                 [f["type"] == FieldType.COLUMN and f["is_read_only"] for f in collection.schema["fields"].values()]
             ),
-            "integration": None,
             "isSearchable": collection.schema["searchable"],
-            "onlyForRelationships": False,
             "paginationType": "page",
-            "searchField": None,
             "actions": sorted(
                 [
                     await SchemaActionGenerator.build(prefix, collection, name)
                     for name in collection.schema["actions"].keys()
                 ],
                 key=lambda action: action["id"],
             ),
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/generator_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,25 +80,23 @@
 
         res = {
             "field": name,
             "type": cls.build_column_type(column["column_type"]),
             "validations": FrontendValidationUtils.convert_validation_list(column["validations"]),
             "defaultValue": column["default_value"],
             "enums": sorted(column["enum_values"]) if column.get("enum_values") is not None else None,
-            "integration": None,
             "inverseOf": None,
             "isFilterable": FrontendFilterableUtils.is_filterable(column["column_type"], column["filter_operators"]),
             "isPrimaryKey": bool(column["is_primary_key"]),
             "isSortable": bool(column["is_sortable"]),
             # When a column is a foreign key, it is readonly.
             # This may sound counter-intuitive: it is so that the user don't have two fields which
             # allow updating the same foreign key in the detail-view form (fk + many to one)
             "isReadOnly": is_foreign_key or bool(column["is_read_only"]),
             "isRequired": any([v["operator"] == Operator.PRESENT for v in validations]),
-            "isVirtual": False,
             "reference": None,
         }
         return ForestServerField(**res)
 
     @staticmethod
     def is_foreign_collection_filterable(foreign_collection: Collection) -> bool:
         res = False
@@ -186,15 +184,14 @@
         cls, collection: Union[Collection, CollectionCustomizer], field_name: str, field_schema: RelationAlias
     ) -> ForestServerField:
         foreign_collection = collection.datasource.get_collection(field_schema["foreign_collection"])
         relation_schema: ForestServerField = {
             "field": field_name,
             "enums": None,
             "isReadOnly": False,
-            "isVirtual": False,
             "inverseOf": CollectionUtils.get_inverse_relation(cast(Collection, collection), field_name),
             "relationship": cls.RELATION_MAPPING[field_schema["type"]],
         }
         if is_many_to_many(field_schema) or is_one_to_many(field_schema):
             res = cls.build_to_many_relation_schema(field_schema, collection, foreign_collection, relation_schema)
         elif is_one_to_one(field_schema):
             res = cls.build_one_to_one_schema(field_schema, collection, foreign_collection, relation_schema)
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/type.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import enum
 from typing import Any, Dict, Generic, List, Literal, Optional, TypeVar, Union
 
 from forestadmin.datasource_toolkit.interfaces.fields import ColumnAlias
-from typing_extensions import NotRequired, TypedDict
+from typing_extensions import TypedDict
 
 Number = Union[int, float]
 TValue = TypeVar("TValue")
 TName = TypeVar("TName")
 
 
 class ValidationType(enum.Enum):
@@ -49,21 +49,19 @@
 
 
 class ForestServerField(TypedDict, total=False):
     field: str
     type: ColumnAlias
     defaultValue: Any
     enums: Optional[List[str]]
-    integration: None
     isFilterable: bool
     isPrimaryKey: bool
     isReadOnly: bool
     isRequired: bool
     isSortable: bool
-    isVirtual: bool
     reference: Optional[str]
     inverseOf: Optional[str]
     relationship: RelationServer
     validations: List[ServerValidationType]
 
 
 LiteralPage = Literal["page"]
@@ -108,15 +106,15 @@
     name: Literal["input array"]
     parameters: ForestServerActionFieldTextListEditorOptionsParameters
 
 
 # text area
 class ForestServerActionFieldTextAreaEditorOptionsParameters(TypedDict):
     placeholder: Optional[str]
-    rows: NotRequired[str]
+    rows: Optional[int]
 
 
 class ForestServerActionFieldTextAreaEditorOptions(TypedDict):
     name: Literal["text area editor"]
     parameters: ForestServerActionFieldTextAreaEditorOptionsParameters
 
 
@@ -138,21 +136,22 @@
 class ForestServerActionFieldAddressAutocompleteEditorOptions(TypedDict):
     name: Literal["address editor"]
     parameters: ForestServerActionFieldAddressAutocompleteEditorOptionsParameters
 
 
 # number
 class ForestServerActionFieldNumberInputEditorOptionsParameters(TypedDict):
+    placeholder: Optional[str]
     min: Optional[Number]
     max: Optional[Number]
     step: Optional[Number]
 
 
 class ForestServerActionFieldNumberInputEditorOptions(TypedDict):
-    name: Literal["address editor"]
+    name: Literal["number input"]
     parameters: ForestServerActionFieldNumberInputEditorOptionsParameters
 
 
 # number list
 class ForestServerActionFieldNumberInputListEditorOptionsParameters(TypedDict):
     min: Optional[Number]
     max: Optional[Number]
@@ -160,15 +159,15 @@
     placeholder: Optional[str]
     allowDuplicate: bool
     allowEmptyValue: bool
     enableReorder: bool
 
 
 class ForestServerActionFieldNumberInputListEditorOptions(TypedDict):
-    name: Literal["address editor"]
+    name: Literal["input array"]
     parameters: ForestServerActionFieldNumberInputListEditorOptionsParameters
 
 
 # currency
 class ForestServerActionFieldCurrencyInputEditorOptionsParameters(TypedDict):
     placeholder: Optional[str]
     min: Optional[Number]
@@ -305,48 +304,38 @@
     enums: Optional[List[str]]
     field: str
     hook: Optional[str]
     isReadOnly: bool
     isRequired: bool
     reference: Optional[str]
     type: Union[ColumnAlias, Literal["File"]]
-    widget: Optional[Literal["belongsto select", "file picker"]]
     widgetEdit: Optional[WidgetEditConfiguration]
-    searchValue: Optional[str]
 
 
 class ForestServerAction(TypedDict):
     id: str
     name: str
     type: Literal["single", "bulk", "global"]
-    baseUrl: Optional[str]
     endpoint: str
-    httpMethod: Literal["POST"]
-    redirect: Any
     download: bool
     fields: List[ForestServerActionField]
     hooks: ForestServerActionHooks
-    searchField: Optional[str]
 
 
 class ForestServerSegment(TypedDict):
     id: str
     name: str
 
 
 class ForestServerCollection(TypedDict):
     name: str
-    icon: None
-    integration: None
     isReadOnly: bool
     isSearchable: bool
-    isVirtual: bool
-    onlyForRelationships: bool
     paginationType: LiteralPage
-    actions: Optional[List[ForestServerAction]]
+    actions: List[ForestServerAction]
     fields: List[ForestServerField]
-    segments: Optional[List[ForestServerSegment]]
+    segments: List[ForestServerSegment]
 
 
 class ForestSchema(TypedDict):
     data: List[ForestServerCollection]
     meta: AgentMeta
```

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/forest_schema/validation.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/forest_schema/validation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/http.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/http.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/id.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/id.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/ip_whitelist_util.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/ip_whitelist_util.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/forestadmin/agent_toolkit/utils/token.py` & `forestadmin_agent_toolkit-1.8.3/forestadmin/agent_toolkit/utils/token.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_toolkit-1.8.2/pyproject.toml` & `forestadmin_agent_toolkit-1.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-toolkit"
 description = "agent toolkit for forestadmin python agent"
-version = "1.8.2"
+version = "1.8.3"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
@@ -19,15 +19,15 @@
 typing-extensions = ">=4.2.0, <5.0"
 aiohttp = "~=3.9"
 oic = "~=1.4"
 pyjwt = "^2"
 cachetools = "~=5.2"
 marshmallow-jsonapi = ">=0.24.0, <1.0"
 sseclient-py = "^1.5"
-forestadmin-datasource-toolkit = "1.8.2"
+forestadmin-datasource-toolkit = "1.8.3"
 [[tool.poetry.dependencies.pandas]]
 version = ">=1.4.0"
 python = ">=3.8"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
 version = "~0.2.1"
 python = "<3.9"
```

### Comparing `forestadmin_agent_toolkit-1.8.2/PKG-INFO` & `forestadmin_agent_toolkit-1.8.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-toolkit
-Version: 1.8.2
+Version: 1.8.3
 Summary: agent toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9,<4.0)
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: cachetools (>=5.2,<6.0)
-Requires-Dist: forestadmin-datasource-toolkit (==1.8.2)
+Requires-Dist: forestadmin-datasource-toolkit (==1.8.3)
 Requires-Dist: marshmallow-jsonapi (>=0.24.0,<1.0)
 Requires-Dist: oic (>=1.4,<2.0)
 Requires-Dist: pandas (>=1.4.0) ; python_version >= "3.8"
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: sseclient-py (>=1.5,<2.0)
 Requires-Dist: typing-extensions (>=4.2.0,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
```

