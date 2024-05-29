# Comparing `tmp/clear_skies_aws-1.9.1.tar.gz` & `tmp/clear_skies_aws-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clear_skies_aws-1.9.1.tar", max compression
+gzip compressed data, was "clear_skies_aws-1.9.2.tar", max compression
```

## Comparing `clear_skies_aws-1.9.1.tar` & `clear_skies_aws-1.9.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0     1053 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/LICENSE
--rw-r--r--   0        0        0     7780 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/README.md
--rw-r--r--   0        0        0      789 2024-05-04 23:48:02.059008 clear_skies_aws-1.9.1/pyproject.toml
--rw-r--r--   0        0        0      134 2023-12-30 16:33:38.123814 clear_skies_aws-1.9.1/src/clearskies_aws/__init__.py
--rw-r--r--   0        0        0     2865 2024-02-28 23:50:28.351377 clear_skies_aws-1.9.1/src/clearskies_aws/actions/__init__.py
--rw-r--r--   0        0        0     3877 2024-03-20 10:13:37.291200 clear_skies_aws-1.9.1/src/clearskies_aws/actions/action_aws.py
--rw-r--r--   0        0        0     4085 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role.py
--rw-r--r--   0        0        0     2450 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role_test.py
--rw-r--r--   0        0        0     7886 2024-05-04 23:47:53.230973 clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses.py
--rw-r--r--   0        0        0     3076 2024-05-04 23:45:51.234501 clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses_test.py
--rw-r--r--   0        0        0     2197 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns.py
--rw-r--r--   0        0        0     2306 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns_test.py
--rw-r--r--   0        0        0     2340 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs.py
--rw-r--r--   0        0        0     2346 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs_test.py
--rw-r--r--   0        0        0     2363 2024-03-08 14:32:55.873530 clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function.py
--rw-r--r--   0        0        0     2742 2024-03-08 14:32:45.065230 clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function_test.py
--rw-r--r--   0        0        0       83 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/__init__.py
--rw-r--r--   0        0        0    29126 2024-04-19 11:51:58.524701 clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend.py
--rw-r--r--   0        0        0    13150 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend_test.py
--rw-r--r--   0        0        0     2726 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend.py
--rw-r--r--   0        0        0     1138 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend_test.py
--rw-r--r--   0        0        0      472 2024-01-06 13:06:05.318595 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__init__.py
--rw-r--r--   0        0        0     1305 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1276 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     1251 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      506 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli.py
--rw-r--r--   0        0        0     1085 2024-01-06 13:10:52.693804 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli_websocket_mock.py
--rw-r--r--   0        0        0     1002 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway.py
--rw-r--r--   0        0        0     1067 2023-12-18 00:15:49.555696 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py
--rw-r--r--   0        0        0      952 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_elb.py
--rw-r--r--   0        0        0     1009 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_http_gateway.py
--rw-r--r--   0        0        0     1336 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_invocation.py
--rw-r--r--   0        0        0     1317 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sns.py
--rw-r--r--   0        0        0     1685 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
--rw-r--r--   0        0        0     1999 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
--rw-r--r--   0        0        0      510 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/contexts/wsgi.py
--rw-r--r--   0        0        0       56 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/di/__init__.py
--rw-r--r--   0        0        0      775 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/di/standard_dependencies.py
--rw-r--r--   0        0        0      112 2024-03-29 18:03:20.842321 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/__init__.py
--rw-r--r--   0        0        0     7471 2024-03-29 18:02:23.674537 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/secrets_manager_rotation.py
--rw-r--r--   0        0        0     1449 2024-01-06 12:49:14.731820 clear_skies_aws-1.9.1/src/clearskies_aws/handlers/simple_body_routing.py
--rw-r--r--   0        0        0      385 2024-01-06 13:10:44.713712 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__init__.py
--rw-r--r--   0        0        0      943 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     3710 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
--rw-r--r--   0        0        0     2761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
--rw-r--r--   0        0        0      901 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
--rw-r--r--   0        0        0      434 2024-01-06 13:10:39.925657 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/cli_websocket_mock.py
--rw-r--r--   0        0        0     3401 2024-03-02 21:11:37.111733 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py
--rw-r--r--   0        0        0     2845 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
--rw-r--r--   0        0        0      308 2023-12-18 00:15:15.884654 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_web_socket.py
--rw-r--r--   0        0        0      750 2024-03-02 21:10:37.703292 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_elb.py
--rw-r--r--   0        0        0      692 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py
--rw-r--r--   0        0        0      928 2023-10-20 10:10:52.408121 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_invocation.py
--rw-r--r--   0        0        0     2163 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sns.py
--rw-r--r--   0        0        0     2082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
--rw-r--r--   0        0        0       22 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/__init__.py
--rw-r--r--   0        0        0       21 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/__init__.py
--rw-r--r--   0        0        0      937 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/ses.py
--rw-r--r--   0        0        0      326 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/__init__.py
--rw-r--r--   0        0        0     1919 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/__init__.py
--rw-r--r--   0        0        0     1082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
--rw-r--r--   0        0        0     3467 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
--rw-r--r--   0        0        0     3776 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
--rw-r--r--   0        0        0     6444 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
--rw-r--r--   0        0        0     1443 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
--rw-r--r--   0        0        0     1810 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store.py
--rw-r--r--   0        0        0      761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store_test.py
--rw-r--r--   0        0        0     3056 2024-03-01 17:17:16.849026 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager.py
--rw-r--r--   0        0        0      786 2023-10-19 20:17:08.669304 clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager_test.py
--rw-r--r--   0        0        0     1776 2023-12-30 17:11:03.525609 clear_skies_aws-1.9.1/src/clearskies_aws/web_socket_connection_model.py
--rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/LICENSE
+-rw-r--r--   0        0        0     7780 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/README.md
+-rw-r--r--   0        0        0      876 2024-05-29 12:50:12.740905 clear_skies_aws-1.9.2/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-12-30 16:33:38.123814 clear_skies_aws-1.9.2/src/clearskies_aws/__init__.py
+-rw-r--r--   0        0        0     2865 2024-02-28 23:50:28.351377 clear_skies_aws-1.9.2/src/clearskies_aws/actions/__init__.py
+-rw-r--r--   0        0        0     3877 2024-03-20 10:13:37.291200 clear_skies_aws-1.9.2/src/clearskies_aws/actions/action_aws.py
+-rw-r--r--   0        0        0     4085 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/assume_role.py
+-rw-r--r--   0        0        0     2450 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/assume_role_test.py
+-rw-r--r--   0        0        0     7886 2024-05-04 23:47:53.230973 clear_skies_aws-1.9.2/src/clearskies_aws/actions/ses.py
+-rw-r--r--   0        0        0     3076 2024-05-04 23:45:51.234501 clear_skies_aws-1.9.2/src/clearskies_aws/actions/ses_test.py
+-rw-r--r--   0        0        0     2197 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/sns.py
+-rw-r--r--   0        0        0     2306 2023-10-19 20:17:08.661303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/sns_test.py
+-rw-r--r--   0        0        0     2340 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/sqs.py
+-rw-r--r--   0        0        0     2346 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/actions/sqs_test.py
+-rw-r--r--   0        0        0     2363 2024-03-08 14:32:55.873530 clear_skies_aws-1.9.2/src/clearskies_aws/actions/step_function.py
+-rw-r--r--   0        0        0     2742 2024-03-08 14:32:45.065230 clear_skies_aws-1.9.2/src/clearskies_aws/actions/step_function_test.py
+-rw-r--r--   0        0        0       83 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/backends/__init__.py
+-rw-r--r--   0        0        0    29126 2024-04-19 11:51:58.524701 clear_skies_aws-1.9.2/src/clearskies_aws/backends/dynamo_db_backend.py
+-rw-r--r--   0        0        0    13150 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/backends/dynamo_db_backend_test.py
+-rw-r--r--   0        0        0     2726 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/backends/sqs_backend.py
+-rw-r--r--   0        0        0     1138 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/backends/sqs_backend_test.py
+-rw-r--r--   0        0        0      472 2024-01-06 13:06:05.318595 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__init__.py
+-rw-r--r--   0        0        0     1305 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1276 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     1251 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      506 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/cli.py
+-rw-r--r--   0        0        0     1085 2024-01-06 13:10:52.693804 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/cli_websocket_mock.py
+-rw-r--r--   0        0        0     1002 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_api_gateway.py
+-rw-r--r--   0        0        0     1067 2023-12-18 00:15:49.555696 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py
+-rw-r--r--   0        0        0      952 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_elb.py
+-rw-r--r--   0        0        0     1009 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_http_gateway.py
+-rw-r--r--   0        0        0     1336 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_invocation.py
+-rw-r--r--   0        0        0     1317 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sns.py
+-rw-r--r--   0        0        0     1685 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py
+-rw-r--r--   0        0        0     1999 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py
+-rw-r--r--   0        0        0      510 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/contexts/wsgi.py
+-rw-r--r--   0        0        0       56 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/di/__init__.py
+-rw-r--r--   0        0        0      775 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/di/standard_dependencies.py
+-rw-r--r--   0        0        0      112 2024-03-29 18:03:20.842321 clear_skies_aws-1.9.2/src/clearskies_aws/handlers/__init__.py
+-rw-r--r--   0        0        0     7471 2024-03-29 18:02:23.674537 clear_skies_aws-1.9.2/src/clearskies_aws/handlers/secrets_manager_rotation.py
+-rw-r--r--   0        0        0     1449 2024-01-06 12:49:14.731820 clear_skies_aws-1.9.2/src/clearskies_aws/handlers/simple_body_routing.py
+-rw-r--r--   0        0        0      385 2024-01-06 13:10:44.713712 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__init__.py
+-rw-r--r--   0        0        0      943 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     3710 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc
+-rw-r--r--   0        0        0     2761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc
+-rw-r--r--   0        0        0      901 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc
+-rw-r--r--   0        0        0      434 2024-01-06 13:10:39.925657 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/cli_websocket_mock.py
+-rw-r--r--   0        0        0     3401 2024-03-02 21:11:37.111733 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py
+-rw-r--r--   0        0        0     2845 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py
+-rw-r--r--   0        0        0      308 2023-12-18 00:15:15.884654 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_api_gateway_web_socket.py
+-rw-r--r--   0        0        0      750 2024-03-02 21:10:37.703292 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_elb.py
+-rw-r--r--   0        0        0      692 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py
+-rw-r--r--   0        0        0      928 2023-10-20 10:10:52.408121 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_invocation.py
+-rw-r--r--   0        0        0     2163 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_sns.py
+-rw-r--r--   0        0        0     2082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py
+-rw-r--r--   0        0        0       22 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/mocks/__init__.py
+-rw-r--r--   0        0        0       21 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/mocks/actions/__init__.py
+-rw-r--r--   0        0        0      937 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/mocks/actions/ses.py
+-rw-r--r--   0        0        0      326 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/__init__.py
+-rw-r--r--   0        0        0     1919 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/__init__.py
+-rw-r--r--   0        0        0     1082 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py
+-rw-r--r--   0        0        0     3467 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py
+-rw-r--r--   0        0        0     3776 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py
+-rw-r--r--   0        0        0     6444 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py
+-rw-r--r--   0        0        0     1443 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py
+-rw-r--r--   0        0        0     1810 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/parameter_store.py
+-rw-r--r--   0        0        0      761 2023-10-19 20:17:08.665303 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/parameter_store_test.py
+-rw-r--r--   0        0        0     3056 2024-03-01 17:17:16.849026 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/secrets_manager.py
+-rw-r--r--   0        0        0      786 2023-10-19 20:17:08.669304 clear_skies_aws-1.9.2/src/clearskies_aws/secrets/secrets_manager_test.py
+-rw-r--r--   0        0        0     1776 2023-12-30 17:11:03.525609 clear_skies_aws-1.9.2/src/clearskies_aws/web_socket_connection_model.py
+-rw-r--r--   0        0        0     8579 1970-01-01 00:00:00.000000 clear_skies_aws-1.9.2/PKG-INFO
```

### Comparing `clear_skies_aws-1.9.1/LICENSE` & `clear_skies_aws-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/README.md` & `clear_skies_aws-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/pyproject.toml` & `clear_skies_aws-1.9.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
 [tool.poetry]
 name = "clear-skies-aws"
-version = "1.9.1"
+version = "1.9.2"
 description = "clearskies bindings for working in AWS"
 authors = [
     "Conor Mancone <cmancone@gmail.com>",
     "tnijboer"
 ]
 repository = "https://github.com/cmancone/clearskies-aws"
 license = "MIT"
@@ -22,17 +22,17 @@
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
-akeyless = "^3.3.6"
-akeyless-cloud-id = "^0.2.0"
-jinja2 = "^3.1.2"
+jinja2 = {version = "^3.1.2", optional = true}
+akeyless = {version = "^4.0.0", optional = true}
+akeyless-cloud-id = {version = "^0.2.3", optional = true}
 
 [tool.poetry.extras]
 akeyless = ["akeyless-cloud-id", "akeyless"]
 ses = ["jinja2"]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/__init__.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/action_aws.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/action_aws.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/assume_role.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/assume_role_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/assume_role_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/ses_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/ses_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sns_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/sns_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/sqs.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/sqs_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/sqs_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/step_function.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/actions/step_function_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/actions/step_function_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/backends/dynamo_db_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/backends/dynamo_db_backend_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/backends/dynamo_db_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/backends/sqs_backend.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/backends/sqs_backend_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/backends/sqs_backend_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/cli_websocket_mock.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/cli_websocket_mock.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_api_gateway_web_socket.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_elb.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_http_gateway.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_invocation.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sns.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/contexts/lambda_sqs_standard_partial_batch_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/di/standard_dependencies.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/di/standard_dependencies.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/handlers/secrets_manager_rotation.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/handlers/secrets_manager_rotation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/handlers/simple_body_routing.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/handlers/simple_body_routing.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_http_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_api_gateway_test.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/__pycache__/aws_lambda_elb.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_api_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_api_gateway_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_elb.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_elb.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_http_gateway.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_http_gateway.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_invocation.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_invocation.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sns.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_sns.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/input_outputs/lambda_sqs_standard.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/input_outputs/lambda_sqs_standard.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/mocks/actions/ses.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/mocks/actions/ses.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/__init__.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/iam_db_auth_with_ssm.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssh_cert_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/additional_configs/mysql_connection_dynamic_producer_via_ssm_bastion.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/akeyless_with_ssm_cache.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/parameter_store.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/parameter_store_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/parameter_store_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/secrets/secrets_manager_test.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/secrets/secrets_manager_test.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/src/clearskies_aws/web_socket_connection_model.py` & `clear_skies_aws-1.9.2/src/clearskies_aws/web_socket_connection_model.py`

 * *Files identical despite different names*

### Comparing `clear_skies_aws-1.9.1/PKG-INFO` & `clear_skies_aws-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clear-skies-aws
-Version: 1.9.1
+Version: 1.9.2
 Summary: clearskies bindings for working in AWS
 Home-page: https://github.com/cmancone/clearskies-aws
 License: MIT
 Author: Conor Mancone
 Author-email: cmancone@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

