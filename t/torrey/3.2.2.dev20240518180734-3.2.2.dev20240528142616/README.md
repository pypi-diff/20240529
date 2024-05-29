# Comparing `tmp/torrey-3.2.2.dev20240518180734.tar.gz` & `tmp/torrey-3.2.2.dev20240528142616.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torrey-3.2.2.dev20240518180734.tar", max compression
+gzip compressed data, was "torrey-3.2.2.dev20240528142616.tar", max compression
```

## Comparing `torrey-3.2.2.dev20240518180734.tar` & `torrey-3.2.2.dev20240528142616.tar`

### file list

```diff
@@ -1,120 +1,116 @@
--rw-r--r--   0        0        0    11356 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/LICENSE.txt
--rw-r--r--   0        0        0       21 2024-05-18 18:07:35.906473 torrey-3.2.2.dev20240518180734/README.md
--rw-r--r--   0        0        0      454 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/__init__.py
--rw-r--r--   0        0        0        5 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/__version__
--rw-r--r--   0        0        0      199 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/config/__init__.py
--rw-r--r--   0        0        0     3228 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/config/config.py
--rw-r--r--   0        0        0     4258 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/config/openapi.py
--rw-r--r--   0        0        0      934 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/config/pinecone_config.py
--rw-r--r--   0        0        0       30 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/control/__init__.py
--rw-r--r--   0        0        0     1786 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/control/index_host_store.py
--rw-r--r--   0        0        0    26249 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/control/pinecone.py
--rw-r--r--   0        0        0        0 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/__init__.py
--rw-r--r--   0        0        0      912 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/__init__.py
--rw-r--r--   0        0        0      226 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/api/__init__.py
--rw-r--r--   0        0        0    44181 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/api/data_plane_api.py
--rw-r--r--   0        0        0     5335 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/api/inference_api.py
--rw-r--r--   0        0        0    42855 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/api/manage_indexes_api.py
--rw-r--r--   0        0        0    37047 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/api_client.py
--rw-r--r--   0        0        0     1037 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/apis/__init__.py
--rw-r--r--   0        0        0    17126 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/configuration.py
--rw-r--r--   0        0        0     5275 2024-05-18 17:58:18.151089 torrey-3.2.2.dev20240518180734/pinecone/core/client/exceptions.py
--rw-r--r--   0        0        0      348 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/__init__.py
--rw-r--r--   0        0        0    11438 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/collection_list.py
--rw-r--r--   0        0        0    13037 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/collection_model.py
--rw-r--r--   0        0        0    11532 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request.py
--rw-r--r--   0        0        0    11555 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request_spec.py
--rw-r--r--   0        0        0    12268 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request_spec_pod.py
--rw-r--r--   0        0        0    12068 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0        0        0    13960 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/create_index_request.py
--rw-r--r--   0        0        0    12890 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/delete_request.py
--rw-r--r--   0        0        0    11727 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0        0        0    12928 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0        0        0    11474 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embedding.py
--rw-r--r--   0        0        0    11176 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_inputs.py
--rw-r--r--   0        0        0    11918 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_list.py
--rw-r--r--   0        0        0    11225 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_list_usage.py
--rw-r--r--   0        0        0    11962 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_parameters.py
--rw-r--r--   0        0        0    11779 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/error_response.py
--rw-r--r--   0        0        0    11913 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0        0        0    11368 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_list.py
--rw-r--r--   0        0        0    14023 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model.py
--rw-r--r--   0        0        0    11700 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model_spec.py
--rw-r--r--   0        0        0    11830 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model_status.py
--rw-r--r--   0        0        0    12075 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_object.py
--rw-r--r--   0        0        0    11791 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_response400.py
--rw-r--r--   0        0        0    12846 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_response400_error.py
--rw-r--r--   0        0        0    11140 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/list_item.py
--rw-r--r--   0        0        0    12236 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/list_response.py
--rw-r--r--   0        0        0    11545 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0        0        0    11156 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pagination.py
--rw-r--r--   0        0        0    14771 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pod_spec.py
--rw-r--r--   0        0        0    11500 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pod_spec_metadata_config.py
--rw-r--r--   0        0        0    11361 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0        0        0    12278 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0        0        0    15454 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_request.py
--rw-r--r--   0        0        0    12556 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_response.py
--rw-r--r--   0        0        0    13173 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_vector.py
--rw-r--r--   0        0        0    11744 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0        0        0    12977 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0        0        0    12098 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/serverless_spec.py
--rw-r--r--   0        0        0    11734 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0        0        0    11536 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0        0        0    12781 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/update_request.py
--rw-r--r--   0        0        0    11921 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0        0        0    11283 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0        0        0    11278 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/usage.py
--rw-r--r--   0        0        0    12592 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model/vector.py
--rw-r--r--   0        0        0    80542 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/model_utils.py
--rw-r--r--   0        0        0     4002 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/models/__init__.py
--rw-r--r--   0        0        0    14209 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/client/rest.py
--rw-r--r--   0        0        0    76084 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0        0        0    24258 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2.pyi
--rw-r--r--   0        0        0    14276 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0        0        0      291 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/data/__init__.py
--rw-r--r--   0        0        0     2125 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/data/errors.py
--rw-r--r--   0        0        0    27458 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/data/index.py
--rw-r--r--   0        0        0     1730 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/data/sparse_vector_factory.py
--rw-r--r--   0        0        0     2815 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/data/vector_factory.py
--rw-r--r--   0        0        0     4027 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/deprecation_warnings.py
--rw-r--r--   0        0        0     1033 2024-05-18 17:58:18.155089 torrey-3.2.2.dev20240518180734/pinecone/exceptions.py
--rw-r--r--   0        0        0     1300 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/__init__.py
--rw-r--r--   0        0        0     5875 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/base.py
--rw-r--r--   0        0        0     1728 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/config.py
--rw-r--r--   0        0        0      961 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/future.py
--rw-r--r--   0        0        0    28020 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/index_grpc.py
--rw-r--r--   0        0        0     4166 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/pinecone.py
--rw-r--r--   0        0        0     3193 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/retry.py
--rw-r--r--   0        0        0     2000 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/sparse_values_factory.py
--rw-r--r--   0        0        0     2996 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/utils.py
--rw-r--r--   0        0        0     3841 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/grpc/vector_factory_grpc.py
--rw-r--r--   0        0        0       76 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/inference/__init__.py
--rw-r--r--   0        0        0      839 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/inference/build_parameters_dict_for_inference.py
--rw-r--r--   0        0        0     3612 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/inference/embeddings.py
--rw-r--r--   0        0        0     1875 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/inference/repl_overrides.py
--rw-r--r--   0        0        0       87 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/interfaces/__init__.py
--rw-r--r--   0        0        0      143 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/interfaces/installables.py
--rw-r--r--   0        0        0      294 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/interfaces/pinecone_plugin.py
--rw-r--r--   0        0        0      600 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/__init__.py
--rw-r--r--   0        0        0      277 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/collection_description.py
--rw-r--r--   0        0        0      852 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/collection_list.py
--rw-r--r--   0        0        0      765 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/embeddings_list.py
--rw-r--r--   0        0        0     1330 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/index_description.py
--rw-r--r--   0        0        0      718 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/index_list.py
--rw-r--r--   0        0        0      198 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/list_response.py
--rw-r--r--   0        0        0     2189 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/pod_spec.py
--rw-r--r--   0        0        0      164 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/models/serverless_spec.py
--rw-r--r--   0        0        0      379 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/plugins/example_plugin/__init__.py
--rw-r--r--   0        0        0      375 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/__init__.py
--rw-r--r--   0        0        0      288 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/check_kwargs.py
--rw-r--r--   0        0        0      722 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/constants.py
--rw-r--r--   0        0        0      785 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/convert_to_list.py
--rw-r--r--   0        0        0      263 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/deprecation_notice.py
--rw-r--r--   0        0        0      750 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/error_handling.py
--rw-r--r--   0        0        0      193 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/fix_tuple_length.py
--rw-r--r--   0        0        0      206 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/normalize_host.py
--rw-r--r--   0        0        0      752 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/setup_openapi_client.py
--rw-r--r--   0        0        0     1011 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/user_agent.py
--rw-r--r--   0        0        0      157 2024-05-18 17:58:18.159089 torrey-3.2.2.dev20240518180734/pinecone/utils/version.py
--rw-r--r--   0        0        0     3295 2024-05-18 18:07:35.942473 torrey-3.2.2.dev20240518180734/pyproject.toml
--rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 torrey-3.2.2.dev20240518180734/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/LICENSE.txt
+-rw-r--r--   0        0        0       21 2024-05-28 14:26:17.976384 torrey-3.2.2.dev20240528142616/README.md
+-rw-r--r--   0        0        0      394 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/__init__.py
+-rw-r--r--   0        0        0        5 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/__version__
+-rw-r--r--   0        0        0      199 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/config/__init__.py
+-rw-r--r--   0        0        0     3228 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/config/config.py
+-rw-r--r--   0        0        0     4258 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/config/openapi.py
+-rw-r--r--   0        0        0      934 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/config/pinecone_config.py
+-rw-r--r--   0        0        0       30 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/control/__init__.py
+-rw-r--r--   0        0        0     1786 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/control/index_host_store.py
+-rw-r--r--   0        0        0    24940 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/control/pinecone.py
+-rw-r--r--   0        0        0        0 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/__init__.py
+-rw-r--r--   0        0        0      912 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/client/__init__.py
+-rw-r--r--   0        0        0      226 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/client/api/__init__.py
+-rw-r--r--   0        0        0    44181 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/client/api/data_plane_api.py
+-rw-r--r--   0        0        0     5335 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/client/api/inference_api.py
+-rw-r--r--   0        0        0    42855 2024-05-28 14:16:34.861048 torrey-3.2.2.dev20240528142616/pinecone/core/client/api/manage_indexes_api.py
+-rw-r--r--   0        0        0    37047 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/api_client.py
+-rw-r--r--   0        0        0     1037 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/apis/__init__.py
+-rw-r--r--   0        0        0    17126 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/configuration.py
+-rw-r--r--   0        0        0     5275 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/exceptions.py
+-rw-r--r--   0        0        0      348 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/__init__.py
+-rw-r--r--   0        0        0    11438 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/collection_list.py
+-rw-r--r--   0        0        0    13037 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/collection_model.py
+-rw-r--r--   0        0        0    11532 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request.py
+-rw-r--r--   0        0        0    11555 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request_spec.py
+-rw-r--r--   0        0        0    12268 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request_spec_pod.py
+-rw-r--r--   0        0        0    12068 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/create_collection_request.py
+-rw-r--r--   0        0        0    13960 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/create_index_request.py
+-rw-r--r--   0        0        0    12890 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/delete_request.py
+-rw-r--r--   0        0        0    11727 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/describe_index_stats_request.py
+-rw-r--r--   0        0        0    12928 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/describe_index_stats_response.py
+-rw-r--r--   0        0        0    11474 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embedding.py
+-rw-r--r--   0        0        0    11176 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_inputs.py
+-rw-r--r--   0        0        0    11918 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_list.py
+-rw-r--r--   0        0        0    11225 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_list_usage.py
+-rw-r--r--   0        0        0    11962 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_parameters.py
+-rw-r--r--   0        0        0    11779 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/error_response.py
+-rw-r--r--   0        0        0    11913 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/fetch_response.py
+-rw-r--r--   0        0        0    11368 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_list.py
+-rw-r--r--   0        0        0    14023 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model.py
+-rw-r--r--   0        0        0    11700 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model_spec.py
+-rw-r--r--   0        0        0    11830 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model_status.py
+-rw-r--r--   0        0        0    12075 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_object.py
+-rw-r--r--   0        0        0    11791 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_response400.py
+-rw-r--r--   0        0        0    12846 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_response400_error.py
+-rw-r--r--   0        0        0    11140 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/list_item.py
+-rw-r--r--   0        0        0    12236 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/list_response.py
+-rw-r--r--   0        0        0    11545 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/namespace_summary.py
+-rw-r--r--   0        0        0    11156 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pagination.py
+-rw-r--r--   0        0        0    14771 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pod_spec.py
+-rw-r--r--   0        0        0    11500 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pod_spec_metadata_config.py
+-rw-r--r--   0        0        0    11361 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/protobuf_any.py
+-rw-r--r--   0        0        0    12278 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/protobuf_null_value.py
+-rw-r--r--   0        0        0    15454 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_request.py
+-rw-r--r--   0        0        0    12556 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_response.py
+-rw-r--r--   0        0        0    13173 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_vector.py
+-rw-r--r--   0        0        0    11744 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/rpc_status.py
+-rw-r--r--   0        0        0    12977 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/scored_vector.py
+-rw-r--r--   0        0        0    12098 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/serverless_spec.py
+-rw-r--r--   0        0        0    11734 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/single_query_results.py
+-rw-r--r--   0        0        0    11536 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/sparse_values.py
+-rw-r--r--   0        0        0    12781 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/update_request.py
+-rw-r--r--   0        0        0    11921 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/upsert_request.py
+-rw-r--r--   0        0        0    11283 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/upsert_response.py
+-rw-r--r--   0        0        0    11278 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/usage.py
+-rw-r--r--   0        0        0    12592 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model/vector.py
+-rw-r--r--   0        0        0    80542 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/model_utils.py
+-rw-r--r--   0        0        0     4002 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/models/__init__.py
+-rw-r--r--   0        0        0    14209 2024-05-28 14:16:34.865049 torrey-3.2.2.dev20240528142616/pinecone/core/client/rest.py
+-rw-r--r--   0        0        0    76084 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2.py
+-rw-r--r--   0        0        0    24258 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2.pyi
+-rw-r--r--   0        0        0    14276 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
+-rw-r--r--   0        0        0      291 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/data/__init__.py
+-rw-r--r--   0        0        0     2125 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/data/errors.py
+-rw-r--r--   0        0        0    27458 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/data/index.py
+-rw-r--r--   0        0        0     1730 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/data/sparse_vector_factory.py
+-rw-r--r--   0        0        0     2815 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/data/vector_factory.py
+-rw-r--r--   0        0        0     4027 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/deprecation_warnings.py
+-rw-r--r--   0        0        0     1033 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/exceptions.py
+-rw-r--r--   0        0        0     1300 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/__init__.py
+-rw-r--r--   0        0        0     5875 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/base.py
+-rw-r--r--   0        0        0     1728 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/config.py
+-rw-r--r--   0        0        0      961 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/future.py
+-rw-r--r--   0        0        0    28020 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/index_grpc.py
+-rw-r--r--   0        0        0     4166 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/pinecone.py
+-rw-r--r--   0        0        0     3193 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/retry.py
+-rw-r--r--   0        0        0     2000 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/sparse_values_factory.py
+-rw-r--r--   0        0        0     2996 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/utils.py
+-rw-r--r--   0        0        0     3841 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/grpc/vector_factory_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/inference/__init__.py
+-rw-r--r--   0        0        0      839 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/inference/build_parameters_dict_for_inference.py
+-rw-r--r--   0        0        0     3726 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/inference/embeddings.py
+-rw-r--r--   0        0        0     1875 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/inference/repl_overrides.py
+-rw-r--r--   0        0        0      600 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/__init__.py
+-rw-r--r--   0        0        0      277 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/collection_description.py
+-rw-r--r--   0        0        0      852 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/collection_list.py
+-rw-r--r--   0        0        0      765 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/embeddings_list.py
+-rw-r--r--   0        0        0     1330 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/index_description.py
+-rw-r--r--   0        0        0      718 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/index_list.py
+-rw-r--r--   0        0        0      198 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/list_response.py
+-rw-r--r--   0        0        0     2189 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/pod_spec.py
+-rw-r--r--   0        0        0      164 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/models/serverless_spec.py
+-rw-r--r--   0        0        0      375 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/__init__.py
+-rw-r--r--   0        0        0      288 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/check_kwargs.py
+-rw-r--r--   0        0        0      722 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/constants.py
+-rw-r--r--   0        0        0      785 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/convert_to_list.py
+-rw-r--r--   0        0        0      263 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/deprecation_notice.py
+-rw-r--r--   0        0        0      750 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/error_handling.py
+-rw-r--r--   0        0        0      193 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/fix_tuple_length.py
+-rw-r--r--   0        0        0      206 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/normalize_host.py
+-rw-r--r--   0        0        0      894 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/setup_openapi_client.py
+-rw-r--r--   0        0        0     1011 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/user_agent.py
+-rw-r--r--   0        0        0      157 2024-05-28 14:16:34.869048 torrey-3.2.2.dev20240528142616/pinecone/utils/version.py
+-rw-r--r--   0        0        0     3332 2024-05-28 14:26:18.000383 torrey-3.2.2.dev20240528142616/pyproject.toml
+-rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 torrey-3.2.2.dev20240528142616/PKG-INFO
```

### Comparing `torrey-3.2.2.dev20240518180734/LICENSE.txt` & `torrey-3.2.2.dev20240528142616/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/config/config.py` & `torrey-3.2.2.dev20240528142616/pinecone/config/config.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/config/openapi.py` & `torrey-3.2.2.dev20240528142616/pinecone/config/openapi.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/config/pinecone_config.py` & `torrey-3.2.2.dev20240528142616/pinecone/config/pinecone_config.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/control/index_host_store.py` & `torrey-3.2.2.dev20240528142616/pinecone/control/index_host_store.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/control/pinecone.py` & `torrey-3.2.2.dev20240528142616/pinecone/control/pinecone.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,18 @@
     CreateIndexRequest,
     ConfigureIndexRequest,
     ConfigureIndexRequestSpec,
     ConfigureIndexRequestSpecPod
 )
 from pinecone.models import ServerlessSpec, PodSpec, IndexList, CollectionList
 
-from pinecone.interfaces import InstallablePlugin
-import importlib
-import pkgutil
-
 from pinecone.data import Index
 
+from pinecone_plugin_interface import load_and_install as install_plugins
+
 class Pinecone:
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         host: Optional[str] = None,
         proxy_url: Optional[str] = None,
@@ -199,55 +197,31 @@
 
         if kwargs.get("openapi_config", None):
             warnings.warn("Passing openapi_config is deprecated and will be removed in a future release. Please pass settings such as proxy_url, proxy_headers, ssl_ca_certs, and ssl_verify directly to the Pinecone constructor as keyword arguments. See the README at https://github.com/pinecone-io/pinecone-python-client for examples.", DeprecationWarning)
 
         self.openapi_config = ConfigBuilder.build_openapi_config(self.config, **kwargs)
         self.pool_threads = pool_threads
 
-        self.discover_and_install_plugins()
-
-        # TODO: Remove after successful plugin migration
         self.embeddings = Embeddings(
-            build_plugin_setup_client(self.config, self.openapi_config, self.pool_threads),
             config=self.config,
+            openapi_config=self.openapi_config,
+            pool_threads=self.pool_threads,
         )
 
+        openapi_client_builder = build_plugin_setup_client(self.config, self.openapi_config, self.pool_threads)
+        install_plugins(self, openapi_client_builder)
+
         if index_api:
             self.index_api = index_api
         else:
             self.index_api = setup_openapi_client(ManageIndexesApi, self.config, self.openapi_config, pool_threads)
 
         self.index_host_store = IndexHostStore()
         """ @private """
 
-    def discover_and_install_plugins(self):
-        plugin_client_builder = build_plugin_setup_client(self.config, self.openapi_config, self.pool_threads)
-
-        plugin_sources = [p.name for p in pkgutil.iter_modules() if 'pinecone' in p.name and p.name != 'pinecone']
-
-        for package in plugin_sources:
-            print("Checking for plugins in: ", package)
-            try:
-                # Attempt to import the package under the assumed namespace
-                plugin_module = importlib.import_module(f"{package}.pinecone_plugins")
-                if not hasattr(plugin_module, '__installables__'):
-                    raise Exception(f"{package} does not have __installables__")
-                else:
-                    for plugin in plugin_module.__installables__:
-                        if not isinstance(plugin, InstallablePlugin):
-                            raise Exception(f"installable in {package} is not of type InstallablePlugin")
-                        else:
-                            if plugin.target_object == 'Pinecone':
-                                impl = plugin.implementation_class
-                                setattr(self, plugin.namespace, impl(plugin_client_builder, self.config))
-            except ModuleNotFoundError:
-                print(f"No plugins found in '{package}'")
-                continue
-            
-
     def create_index(
         self,
         name: str,
         dimension: int,
         spec: Union[Dict, ServerlessSpec, PodSpec],
         metric: Optional[str] = "cosine",
         timeout: Optional[int] = None,
```

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/__init__.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/__init__.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/api/data_plane_api.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/api/data_plane_api.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/api/inference_api.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/api/inference_api.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/api/manage_indexes_api.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/api/manage_indexes_api.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/api_client.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/api_client.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/apis/__init__.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/configuration.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/configuration.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/exceptions.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/collection_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/collection_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/collection_model.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/collection_model.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request_spec.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request_spec.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/configure_index_request_spec_pod.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/configure_index_request_spec_pod.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/create_collection_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/create_index_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/create_index_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/delete_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/delete_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/describe_index_stats_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/describe_index_stats_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/describe_index_stats_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/describe_index_stats_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embedding.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embedding.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_inputs.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_inputs.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_list_usage.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_list_usage.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/embeddings_parameters.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/embeddings_parameters.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/error_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/error_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/fetch_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/fetch_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model_spec.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model_spec.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/index_model_status.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/index_model_status.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_object.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_object.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_response400.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/inline_response400_error.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/inline_response400_error.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/list_item.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/list_item.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/list_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/list_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/namespace_summary.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/namespace_summary.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pagination.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pagination.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pod_spec.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pod_spec.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/pod_spec_metadata_config.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/pod_spec_metadata_config.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/protobuf_any.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/protobuf_null_value.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/query_vector.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/query_vector.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/rpc_status.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/rpc_status.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/scored_vector.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/scored_vector.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/serverless_spec.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/serverless_spec.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/single_query_results.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/single_query_results.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/sparse_values.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/sparse_values.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/update_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/update_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/upsert_request.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/upsert_request.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/upsert_response.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/upsert_response.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/usage.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/usage.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model/vector.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model/vector.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/model_utils.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/model_utils.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/models/__init__.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/client/rest.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/client/rest.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2.pyi` & `torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/core/grpc/protos/vector_service_pb2_grpc.py` & `torrey-3.2.2.dev20240528142616/pinecone/core/grpc/protos/vector_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/data/errors.py` & `torrey-3.2.2.dev20240528142616/pinecone/data/errors.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/data/index.py` & `torrey-3.2.2.dev20240528142616/pinecone/data/index.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/data/sparse_vector_factory.py` & `torrey-3.2.2.dev20240528142616/pinecone/data/sparse_vector_factory.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/data/vector_factory.py` & `torrey-3.2.2.dev20240528142616/pinecone/data/vector_factory.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/deprecation_warnings.py` & `torrey-3.2.2.dev20240528142616/pinecone/deprecation_warnings.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/exceptions.py` & `torrey-3.2.2.dev20240528142616/pinecone/exceptions.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/__init__.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/base.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/base.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/config.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/config.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/future.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/future.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/index_grpc.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/index_grpc.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/pinecone.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/pinecone.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/retry.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/retry.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/sparse_values_factory.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/sparse_values_factory.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/utils.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/utils.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/grpc/vector_factory_grpc.py` & `torrey-3.2.2.dev20240528142616/pinecone/grpc/vector_factory_grpc.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/inference/build_parameters_dict_for_inference.py` & `torrey-3.2.2.dev20240528142616/pinecone/inference/build_parameters_dict_for_inference.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/inference/embeddings.py` & `torrey-3.2.2.dev20240528142616/pinecone/inference/embeddings.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 from pinecone.core.client.model.embeddings_inputs import EmbeddingsInputs
 from pinecone.core.client.model.inline_object import InlineObject
 from pinecone.inference.build_parameters_dict_for_inference import build_parameters_dict_for_inference
 from pinecone.utils import setup_openapi_client
 
 from pinecone.models import EmbeddingsList 
 
-from pinecone.interfaces import PineconePlugin
 
-class Embeddings(PineconePlugin):
+class Embeddings:
     """
     The `Embeddings` class configures and utilizes the Pinecone Inference API to generate embeddings.
 
     :param config: A `pinecone.config.Config` object, configured and built in the Pinecone class.
     :type config: `pinecone.config.Config`, required
 
     :param openapi_config: A `pinecone.config.openapi.OpenApiConfiguration` object, configured and built in the
     Pinecone class.
     :type openapi_config: `pinecone.config.openapi.OpenApiConfiguration`, required
 
     :param pool_threads: Number of threads to use for the connection pool, as declared in the Pinecone class.
     :type pool_threads: int, required (but optional in the Pinecone class)
     """
 
-    def __init__(self, plugin_client_builder, config: Config):
+    def __init__(self, config: Config, openapi_config: OpenApiConfiguration, pool_threads: Optional[int]):
         self.config = config
-        self.inference_api = plugin_client_builder(InferenceApi)
+        self.openapi_config = openapi_config
+        self.pool_threads = pool_threads
+        self.inference_api = setup_openapi_client(InferenceApi, self.config, self.openapi_config, pool_threads)
 
     def create(
         self, model: str, inputs: List[str], parameters: Optional[Dict[str, str]] = None, async_req=False
     ) -> EmbeddingsList:
         """
         Generates embeddings for the provided inputs using the specified model and (optional) parameters.
```

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/inference/repl_overrides.py` & `torrey-3.2.2.dev20240528142616/pinecone/inference/repl_overrides.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/__init__.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/__init__.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/collection_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/collection_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/embeddings_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/embeddings_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/index_description.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/index_description.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/index_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/index_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/models/pod_spec.py` & `torrey-3.2.2.dev20240528142616/pinecone/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/utils/constants.py` & `torrey-3.2.2.dev20240528142616/pinecone/utils/constants.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/utils/convert_to_list.py` & `torrey-3.2.2.dev20240528142616/pinecone/utils/convert_to_list.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/utils/error_handling.py` & `torrey-3.2.2.dev20240528142616/pinecone/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/utils/setup_openapi_client.py` & `torrey-3.2.2.dev20240528142616/pinecone/utils/setup_openapi_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from pinecone.core.client.api_client import ApiClient
 from .user_agent import get_user_agent
 
-def setup_openapi_client(api_klass, config, openapi_config, pool_threads):
+def setup_openapi_client(api_klass, config, openapi_config, pool_threads, api_version=None):
     api_client = ApiClient(
         configuration=openapi_config, 
         pool_threads=pool_threads
     )
     api_client.user_agent = get_user_agent(config)
     extra_headers = config.additional_headers or {}
     for key, value in extra_headers.items():
         api_client.set_default_header(key, value)
+    if api_version:
+        api_client.set_default_header("X-Pinecone-Api-Version", api_version)
     client = api_klass(api_client)
     return client
 
 def build_plugin_setup_client(config, openapi_config, pool_threads):
-    def setup_plugin_client(api_klass):
-        return setup_openapi_client(api_klass, config, openapi_config, pool_threads)
-    return setup_plugin_client
+    def setup_plugin_client(api_klass, api_version):
+        return setup_openapi_client(api_klass, config, openapi_config, pool_threads, api_version)
+    return setup_plugin_client
```

### Comparing `torrey-3.2.2.dev20240518180734/pinecone/utils/user_agent.py` & `torrey-3.2.2.dev20240528142616/pinecone/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `torrey-3.2.2.dev20240518180734/pyproject.toml` & `torrey-3.2.2.dev20240528142616/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   | foo.py           # also separately exclude a file named foo.py in
                      # the root of the project
 )
 '''
 
 [tool.poetry]
 name = "torrey"
-version = "3.2.2.dev20240518180734"
+version = "3.2.2.dev20240528142616"
 packages = [
     { include="pinecone", from="." },
 ]
 description = "Torrey client and SDK"
 authors = ["Torrey Systems, Inc. <support@torrey.com>"]
 license = "Apache-2.0"
 readme = "README.md"
@@ -63,14 +63,15 @@
   { version = ">=1.44.0", optional = true, python = "^3.8,<3.11" },
   { version = ">=1.59.0", optional = true, python = "^3.11" }
 ]
 grpc-gateway-protoc-gen-openapiv2 = { version = "0.1.0", optional = true }
 googleapis-common-protos = { version = ">=1.53.0", optional = true }
 lz4 = { version = ">=3.1.3", optional = true }
 protobuf = { version = "~=3.20.0", optional = true }
+pinecone-plugin-interface = "^0.0.4"
 
 [tool.poetry.group.types]
 optional = true
 
 [tool.poetry.group.types.dependencies]
 mypy = "^1.6.1"
 types-urllib3 = "^1.26.25.14"
```

### Comparing `torrey-3.2.2.dev20240518180734/PKG-INFO` & `torrey-3.2.2.dev20240528142616/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torrey
-Version: 3.2.2.dev20240518180734
+Version: 3.2.2.dev20240528142616
 Summary: Torrey client and SDK
 Home-page: https://www.torrey.com
 License: Apache-2.0
 Keywords: Torrey,vector,database,cloud
 Author: Torrey Systems, Inc.
 Author-email: support@torrey.com
 Requires-Python: >=3.8,<4.0
@@ -29,14 +29,15 @@
 Provides-Extra: grpc
 Requires-Dist: certifi (>=2019.11.17)
 Requires-Dist: googleapis-common-protos (>=1.53.0) ; extra == "grpc"
 Requires-Dist: grpc-gateway-protoc-gen-openapiv2 (==0.1.0) ; extra == "grpc"
 Requires-Dist: grpcio (>=1.44.0) ; (python_version >= "3.8" and python_version < "3.11") and (extra == "grpc")
 Requires-Dist: grpcio (>=1.59.0) ; (python_version >= "3.11" and python_version < "4.0") and (extra == "grpc")
 Requires-Dist: lz4 (>=3.1.3) ; extra == "grpc"
+Requires-Dist: pinecone-plugin-interface (>=0.0.4,<0.0.5)
 Requires-Dist: protobuf (>=3.20.0,<3.21.0) ; extra == "grpc"
 Requires-Dist: tqdm (>=4.64.1)
 Requires-Dist: typing-extensions (>=3.7.4)
 Requires-Dist: urllib3 (>=1.26.0) ; python_version >= "3.8" and python_version < "3.12"
 Requires-Dist: urllib3 (>=1.26.5) ; python_version >= "3.12" and python_version < "4.0"
 Project-URL: Documentation, https://torrey.com/docs
 Description-Content-Type: text/markdown
```

