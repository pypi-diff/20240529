# Comparing `tmp/flwr_nightly-1.9.0.dev20240524.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240527.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240524.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240527.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240524.tar` & `flwr_nightly-1.9.0.dev20240527.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0    11358 2024-05-24 23:05:22.683554 flwr_nightly-1.9.0.dev20240524/LICENSE
--rw-r--r--   0        0        0    13010 2024-05-24 23:05:22.683554 flwr_nightly-1.9.0.dev20240524/README.md
--rw-r--r--   0        0        0     5813 2024-05-24 23:05:41.599603 flwr_nightly-1.9.0.dev20240524/pyproject.toml
--rw-r--r--   0        0        0      937 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1141 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5064 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/build.py
--rw-r--r--   0        0        0     4277 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     6223 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0     1450 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
--rw-r--r--   0        0        0     1434 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl
--rw-r--r--   0        0        0     2113 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
--rw-r--r--   0        0        0      521 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1280 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      338 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
--rw-r--r--   0        0        0      246 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.jax.py.tpl
--rw-r--r--   0        0        0      272 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
--rw-r--r--   0        0        0      248 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      579 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     2857 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
--rw-r--r--   0        0        0     1519 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl
--rw-r--r--   0        0        0     2598 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
--rw-r--r--   0        0        0     3684 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0     1044 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
--rw-r--r--   0        0        0      759 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
--rw-r--r--   0        0        0      568 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl
--rw-r--r--   0        0        0      668 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
--rw-r--r--   0        0        0      606 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      675 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      655 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      654 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2687 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4903 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5415 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2624 2024-05-24 23:05:23.103555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4982 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9915 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     7107 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    13896 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4838 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     5056 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    14009 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4173 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-05-24 23:05:23.107555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1716 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    29973 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     3421 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      886 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     6490 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/inmemory_driver.py
--rw-r--r--   0        0        0     5063 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17821 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17406 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12853 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-05-24 23:05:23.111555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4791 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     7691 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6722 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12456 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    12750 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    28528 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7989 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    14003 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1348 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    14380 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15098 2024-05-24 23:05:23.115555 flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15398 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240524/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-27 23:05:17.278325 flwr_nightly-1.9.0.dev20240527/LICENSE
+-rw-r--r--   0        0        0    13010 2024-05-27 23:05:17.278325 flwr_nightly-1.9.0.dev20240527/README.md
+-rw-r--r--   0        0        0     5801 2024-05-27 23:05:35.462298 flwr_nightly-1.9.0.dev20240527/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5064 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/build.py
+-rw-r--r--   0        0        0     4277 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     6223 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0     1450 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
+-rw-r--r--   0        0        0     1434 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl
+-rw-r--r--   0        0        0     2113 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
+-rw-r--r--   0        0        0      521 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1280 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      338 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
+-rw-r--r--   0        0        0      246 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.jax.py.tpl
+-rw-r--r--   0        0        0      272 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
+-rw-r--r--   0        0        0      248 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      579 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     2857 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
+-rw-r--r--   0        0        0     1519 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl
+-rw-r--r--   0        0        0     2598 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
+-rw-r--r--   0        0        0     3684 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0     1044 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
+-rw-r--r--   0        0        0      759 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
+-rw-r--r--   0        0        0      568 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl
+-rw-r--r--   0        0        0      668 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
+-rw-r--r--   0        0        0      606 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      675 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      655 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      654 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2687 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-27 23:05:17.702324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2624 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4982 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9915 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     7107 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    13896 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4838 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     5056 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    14009 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-05-27 23:05:17.706324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4173 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1716 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    27481 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     3421 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      886 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     6490 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/inmemory_driver.py
+-rw-r--r--   0        0        0     5063 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17821 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17406 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12853 2024-05-27 23:05:17.710324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4791 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     7691 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6722 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12456 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    12750 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    28528 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7989 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    14003 2024-05-27 23:05:17.714324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1348 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15098 2024-05-27 23:05:17.718324 flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15398 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240527/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240524/LICENSE` & `flwr_nightly-1.9.0.dev20240527/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/README.md` & `flwr_nightly-1.9.0.dev20240527/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/pyproject.toml` & `flwr_nightly-1.9.0.dev20240527/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240524"
+version = "1.9.0.dev20240527"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
@@ -77,15 +77,15 @@
 ray = { version = "==2.10.0", optional = true, python = ">=3.8,<3.12" }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.31.0", optional = true }
 starlette = { version = "^0.31.0", optional = true }
 uvicorn = { version = "^0.23.0", extras = ["standard"], optional = true }
 
 [tool.poetry.extras]
-simulation = ["ray", "pydantic"]
+simulation = ["ray"]
 rest = ["requests", "starlette", "uvicorn"]
 
 [tool.poetry.group.dev.dependencies]
 types-dataclasses = "==0.6.6"
 types-protobuf = "==3.19.18"
 types-requests = "==2.31.0.20240125"
 types-setuptools = "==69.0.0.20240125"
```

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/build.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/build.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server app."""
 
 import argparse
-import asyncio
 import csv
 import importlib.util
 import sys
 import threading
 from logging import ERROR, INFO, WARN
 from os.path import isfile
 from pathlib import Path
@@ -35,15 +34,14 @@
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
-    TRANSPORT_TYPE_VCE,
 )
 from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
     private_key_to_bytes,
     public_key_to_bytes,
 )
@@ -59,15 +57,14 @@
 from .superlink.driver.driver_grpc import run_driver_api_grpc
 from .superlink.fleet.grpc_bidi.grpc_server import (
     generic_create_grpc_server,
     start_grpc_server,
 )
 from .superlink.fleet.grpc_rere.fleet_servicer import FleetServicer
 from .superlink.fleet.grpc_rere.server_interceptor import AuthenticateServerInterceptor
-from .superlink.fleet.vce import start_vce
 from .superlink.state import StateFactory
 
 ADDRESS_DRIVER_API = "0.0.0.0:9091"
 ADDRESS_FLEET_API_GRPC_RERE = "0.0.0.0:9092"
 ADDRESS_FLEET_API_GRPC_BIDI = "[::]:8080"  # IPv6 to keep start_server compatible
 ADDRESS_FLEET_API_REST = "0.0.0.0:9093"
 
@@ -397,25 +394,14 @@
         fleet_server = _run_fleet_api_grpc_rere(
             address=address,
             state_factory=state_factory,
             certificates=certificates,
             interceptors=interceptors,
         )
         grpc_servers.append(fleet_server)
-    elif args.fleet_api_type == TRANSPORT_TYPE_VCE:
-        f_stop = asyncio.Event()  # Does nothing
-        _run_fleet_api_vce(
-            num_supernodes=args.num_supernodes,
-            client_app_attr=args.client_app,
-            backend_name=args.backend,
-            backend_config_json_stream=args.backend_config,
-            app_dir=args.app_dir,
-            state_factory=state_factory,
-            f_stop=f_stop,
-        )
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
     register_exit_handlers(
         event_type=EventType.RUN_SUPERLINK_LEAVE,
         grpc_servers=grpc_servers,
@@ -565,37 +551,14 @@
 
     log(INFO, "Flower ECE: Starting Fleet API (gRPC-rere) on %s", address)
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
 
-# pylint: disable=too-many-arguments
-def _run_fleet_api_vce(
-    num_supernodes: int,
-    client_app_attr: str,
-    backend_name: str,
-    backend_config_json_stream: str,
-    app_dir: str,
-    state_factory: StateFactory,
-    f_stop: asyncio.Event,
-) -> None:
-    log(INFO, "Flower VCE: Starting Fleet API (VirtualClientEngine)")
-
-    start_vce(
-        num_supernodes=num_supernodes,
-        client_app_attr=client_app_attr,
-        backend_name=backend_name,
-        backend_config_json_stream=backend_config_json_stream,
-        state_factory=state_factory,
-        app_dir=app_dir,
-        f_stop=f_stop,
-    )
-
-
 # pylint: disable=import-outside-toplevel,too-many-arguments
 def _run_fleet_api_rest(
     host: str,
     port: int,
     ssl_keyfile: Optional[str],
     ssl_certfile: Optional[str],
     state_factory: StateFactory,
@@ -779,22 +742,14 @@
         "--rest",
         action="store_const",
         dest="fleet_api_type",
         const=TRANSPORT_TYPE_REST,
         help="Start a Fleet API server (REST, experimental)",
     )
 
-    ex_group.add_argument(
-        "--vce",
-        action="store_const",
-        dest="fleet_api_type",
-        const=TRANSPORT_TYPE_VCE,
-        help="Start a Fleet API server (VirtualClientEngine)",
-    )
-
     # Fleet API gRPC-rere options
     grpc_rere_group = parser.add_argument_group(
         "Fleet API (gRPC-rere) server options", ""
     )
     grpc_rere_group.add_argument(
         "--grpc-rere-fleet-api-address",
         help="Fleet API (gRPC-rere) server address (IPv4, IPv6, or a domain name)",
@@ -822,40 +777,7 @@
     )
     rest_group.add_argument(
         "--rest-fleet-api-workers",
         help="Set the number of concurrent workers for the Fleet API REST server.",
         type=int,
         default=1,
     )
-
-    # Fleet API VCE options
-    vce_group = parser.add_argument_group("Fleet API (VCE) server options", "")
-    vce_group.add_argument(
-        "--client-app",
-        help="For example: `client:app` or `project.package.module:wrapper.app`.",
-    )
-    vce_group.add_argument(
-        "--num-supernodes",
-        type=int,
-        help="Number of simulated SuperNodes.",
-    )
-    vce_group.add_argument(
-        "--backend",
-        default="ray",
-        type=str,
-        help="Simulation backend that executes the ClientApp.",
-    )
-    vce_group.add_argument(
-        "--backend-config",
-        type=str,
-        default='{"client_resources": {"num_cpus":1, "num_gpus":0.0}, "tensorflow": 0}',
-        help='A JSON formatted stream, e.g \'{"<keyA>":<value>, "<keyB>":<value>}\' to '
-        "configure a backend. Values supported in <value> are those included by "
-        "`flwr.common.typing.ConfigsRecordValues`. ",
-    )
-    parser.add_argument(
-        "--app-dir",
-        default="",
-        help="Add specified directory to the PYTHONPATH and load"
-        "ClientApp from there."
-        " Default: current working directory.",
-    )
```

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/driver/inmemory_driver.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/driver/inmemory_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240527/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240524/PKG-INFO` & `flwr_nightly-1.9.0.dev20240527/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240524
+Version: 1.9.0.dev20240527
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240524 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240527 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

