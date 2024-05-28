# Comparing `tmp/altmindpy-0.1.0.tar.gz` & `tmp/altmindpy-0.2.0.tar.gz`

## Comparing `altmindpy-0.1.0.tar` & `altmindpy-0.2.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/__init__.py
--rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_base_client.py
--rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_constants.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_files.py
--rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_qs.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_resource.py
--rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_response.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_streaming.py
--rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_types.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/__init__.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/lib/.keep
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/__init__.py
--rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/assistants.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/experimental.py
--rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/login.py
--rw-r--r--   0        0        0    19508 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/runs.py
--rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/threads.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/__init__.py
--rw-r--r--   0        0        0    20387 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/messages.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/messages/thread.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/__init__.py
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/open.py
--rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/users.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/__init__.py
--rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/me.py
--rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/resources/users/me/password.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_create_params.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_delete.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_list_params.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_response.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistant_update_params.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/assistants_response.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/experimental_stream_params.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/login_access_token_params.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_create_params.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_delete.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_list_params.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_response.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/message_update_params.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_create_params.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_list_params.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_response.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/run_update_params.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/runs_response.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_create_params.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_delete.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_list_params.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_response.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/thread_update_params.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/threads_response.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/token.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_create_params.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_list_params.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/user_update_params.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users_out.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/messages/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/messages/thread_list_params.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/messages_response.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/response_message.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/shared/user_out.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/__init__.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me_update_params.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/open_create_params.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me/__init__.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 altmindpy-0.1.0/src/altmind/types/users/me/password_update_params.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.1.0/.gitignore
--rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 altmindpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    11943 2020-02-02 00:00:00.000000 altmindpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/__init__.py
+-rw-r--r--   0        0        0    64415 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_base_client.py
+-rw-r--r--   0        0        0    18167 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_constants.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_qs.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_resource.py
+-rw-r--r--   0        0        0    28381 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_response.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_streaming.py
+-rw-r--r--   0        0        0     6128 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_types.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/__init__.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_typing.py
+-rw-r--r--   0        0        0    11447 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/lib/.keep
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/__init__.py
+-rw-r--r--   0        0        0    20337 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/assistants.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/experimental.py
+-rw-r--r--   0        0        0     8122 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/login.py
+-rw-r--r--   0        0        0    19942 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/runs.py
+-rw-r--r--   0        0        0    17588 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/threads.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/messages/__init__.py
+-rw-r--r--   0        0        0    20534 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/messages/messages.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/messages/thread.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/__init__.py
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/open.py
+-rw-r--r--   0        0        0    20279 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/users.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/me/__init__.py
+-rw-r--r--   0        0        0     8170 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/me/me.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/resources/users/me/password.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistant_create_params.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistant_delete.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistant_list_params.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistant_response.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistant_update_params.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/assistants_response.py
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/experimental_stream_params.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/login_access_token_params.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/message_create_params.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/message_delete.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/message_list_params.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/message_response.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/message_update_params.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/run_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/run_list_params.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/run_response.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/run_update_params.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/runs_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/thread_create_params.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/thread_delete.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/thread_list_params.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/thread_response.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/thread_update_params.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/threads_response.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/token.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/user_create_params.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/user_list_params.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/user_update_params.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users_out.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/messages/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/messages/thread_list_params.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/shared/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/shared/messages_response.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/shared/response_message.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/shared/user_out.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users/__init__.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users/me_update_params.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users/open_create_params.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users/me/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 altmindpy-0.2.0/src/altmind/types/users/me/password_update_params.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 altmindpy-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11337 2020-02-02 00:00:00.000000 altmindpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 altmindpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    12032 2020-02-02 00:00:00.000000 altmindpy-0.2.0/PKG-INFO
```

### Comparing `altmindpy-0.1.0/src/altmind/__init__.py` & `altmindpy-0.2.0/src/altmind/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_base_client.py` & `altmindpy-0.2.0/src/altmind/_base_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_client.py` & `altmindpy-0.2.0/src/altmind/_client.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_compat.py` & `altmindpy-0.2.0/src/altmind/_compat.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_exceptions.py` & `altmindpy-0.2.0/src/altmind/_exceptions.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_files.py` & `altmindpy-0.2.0/src/altmind/_files.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_models.py` & `altmindpy-0.2.0/src/altmind/_models.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_qs.py` & `altmindpy-0.2.0/src/altmind/_qs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_resource.py` & `altmindpy-0.2.0/src/altmind/_resource.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_response.py` & `altmindpy-0.2.0/src/altmind/_response.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_streaming.py` & `altmindpy-0.2.0/src/altmind/_streaming.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_types.py` & `altmindpy-0.2.0/src/altmind/_types.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/__init__.py` & `altmindpy-0.2.0/src/altmind/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_logs.py` & `altmindpy-0.2.0/src/altmind/_utils/_logs.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_proxy.py` & `altmindpy-0.2.0/src/altmind/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_sync.py` & `altmindpy-0.2.0/src/altmind/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_transform.py` & `altmindpy-0.2.0/src/altmind/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_typing.py` & `altmindpy-0.2.0/src/altmind/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/_utils/_utils.py` & `altmindpy-0.2.0/src/altmind/_utils/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     overload,
 )
 from pathlib import Path
 from typing_extensions import TypeGuard
 
 import sniffio
 
-from .._types import Headers, NotGiven, FileTypes, NotGivenOr, HeadersLike
+from .._types import NotGiven, FileTypes, NotGivenOr, HeadersLike
 from .._compat import parse_date as parse_date, parse_datetime as parse_datetime
 
 _T = TypeVar("_T")
 _TupleT = TypeVar("_TupleT", bound=Tuple[object, ...])
 _MappingT = TypeVar("_MappingT", bound=Mapping[str, object])
 _SequenceT = TypeVar("_SequenceT", bound=Sequence[object])
 CallableT = TypeVar("CallableT", bound=Callable[..., Any])
@@ -366,15 +366,14 @@
     file_name = os.path.basename(path)
     return (file_name, contents)
 
 
 def get_required_header(headers: HeadersLike, header: str) -> str:
     lower_header = header.lower()
     if isinstance(headers, Mapping):
-        headers = cast(Headers, headers)
         for k, v in headers.items():
             if k.lower() == lower_header and isinstance(v, str):
                 return v
 
     """ to deal with the case where the header looks like Stainless-Event-Id """
     intercaps_header = re.sub(r"([^\w])(\w)", lambda pat: pat.group(1) + pat.group(2).upper(), header.capitalize())
```

### Comparing `altmindpy-0.1.0/src/altmind/resources/__init__.py` & `altmindpy-0.2.0/src/altmind/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/assistants.py` & `altmindpy-0.2.0/src/altmind/resources/assistants.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/experimental.py` & `altmindpy-0.2.0/src/altmind/resources/experimental.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/login.py` & `altmindpy-0.2.0/src/altmind/resources/login.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/runs.py` & `altmindpy-0.2.0/src/altmind/resources/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
 from ..types import run_list_params, run_create_params, run_update_params
 from .._types import NOT_GIVEN, Body, Query, Headers, NotGiven
 from .._utils import (
@@ -45,14 +45,16 @@
         assistant_id: Optional[int],
         thread_id: Optional[int],
         stream: bool | NotGiven = NOT_GIVEN,
         additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         model: Optional[str] | NotGiven = NOT_GIVEN,
         run_metadata: object | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[object] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         type: Literal["default", "analysis", "execution"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
@@ -81,14 +83,16 @@
                 {
                     "assistant_id": assistant_id,
                     "thread_id": thread_id,
                     "additional_instructions": additional_instructions,
                     "instructions": instructions,
                     "model": model,
                     "run_metadata": run_metadata,
+                    "tool_choice": tool_choice,
+                    "tools": tools,
                     "type": type,
                 },
                 run_create_params.RunCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
@@ -258,14 +262,16 @@
         assistant_id: Optional[int],
         thread_id: Optional[int],
         stream: bool | NotGiven = NOT_GIVEN,
         additional_instructions: Optional[str] | NotGiven = NOT_GIVEN,
         instructions: Optional[str] | NotGiven = NOT_GIVEN,
         model: Optional[str] | NotGiven = NOT_GIVEN,
         run_metadata: object | NotGiven = NOT_GIVEN,
+        tool_choice: Optional[object] | NotGiven = NOT_GIVEN,
+        tools: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         type: Literal["default", "analysis", "execution"] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
@@ -294,14 +300,16 @@
                 {
                     "assistant_id": assistant_id,
                     "thread_id": thread_id,
                     "additional_instructions": additional_instructions,
                     "instructions": instructions,
                     "model": model,
                     "run_metadata": run_metadata,
+                    "tool_choice": tool_choice,
+                    "tools": tools,
                     "type": type,
                 },
                 run_create_params.RunCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers,
                 extra_query=extra_query,
```

### Comparing `altmindpy-0.1.0/src/altmind/resources/threads.py` & `altmindpy-0.2.0/src/altmind/resources/threads.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/messages/__init__.py` & `altmindpy-0.2.0/src/altmind/resources/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/messages/messages.py` & `altmindpy-0.2.0/src/altmind/resources/messages/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Iterable, Optional
+from typing import Union, Iterable, Optional
 from typing_extensions import Literal
 
 import httpx
 
 from .thread import (
     ThreadResource,
     AsyncThreadResource,
@@ -51,20 +51,20 @@
     @cached_property
     def with_streaming_response(self) -> MessagesResourceWithStreamingResponse:
         return MessagesResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
-        content: Iterable[message_create_params.Content],
-        tool_calls: Optional[Iterable[object]],
+        content: Union[str, Iterable[message_create_params.ContentUnionMember1]],
         message_metadata: object | NotGiven = NOT_GIVEN,
         original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         thread_id: Optional[int] | NotGiven = NOT_GIVEN,
+        tool_calls: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> MessageResponse:
@@ -81,19 +81,19 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._post(
             "/api/v1/messages/",
             body=maybe_transform(
                 {
                     "content": content,
-                    "tool_calls": tool_calls,
                     "message_metadata": message_metadata,
                     "original_role": original_role,
                     "role": role,
                     "thread_id": thread_id,
+                    "tool_calls": tool_calls,
                 },
                 message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=MessageResponse,
@@ -130,18 +130,18 @@
             cast_to=MessageResponse,
         )
 
     def update(
         self,
         message_id: int,
         *,
-        tool_calls: Optional[Iterable[object]],
         content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
         message_metadata: object | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        tool_calls: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> MessageResponse:
@@ -157,18 +157,18 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return self._patch(
             f"/api/v1/messages/{message_id}",
             body=maybe_transform(
                 {
-                    "tool_calls": tool_calls,
                     "content": content,
                     "message_metadata": message_metadata,
                     "role": role,
+                    "tool_calls": tool_calls,
                 },
                 message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=MessageResponse,
@@ -260,20 +260,20 @@
     @cached_property
     def with_streaming_response(self) -> AsyncMessagesResourceWithStreamingResponse:
         return AsyncMessagesResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
-        content: Iterable[message_create_params.Content],
-        tool_calls: Optional[Iterable[object]],
+        content: Union[str, Iterable[message_create_params.ContentUnionMember1]],
         message_metadata: object | NotGiven = NOT_GIVEN,
         original_role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
         thread_id: Optional[int] | NotGiven = NOT_GIVEN,
+        tool_calls: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> MessageResponse:
@@ -290,19 +290,19 @@
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._post(
             "/api/v1/messages/",
             body=await async_maybe_transform(
                 {
                     "content": content,
-                    "tool_calls": tool_calls,
                     "message_metadata": message_metadata,
                     "original_role": original_role,
                     "role": role,
                     "thread_id": thread_id,
+                    "tool_calls": tool_calls,
                 },
                 message_create_params.MessageCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=MessageResponse,
@@ -339,18 +339,18 @@
             cast_to=MessageResponse,
         )
 
     async def update(
         self,
         message_id: int,
         *,
-        tool_calls: Optional[Iterable[object]],
         content: Optional[Iterable[message_update_params.Content]] | NotGiven = NOT_GIVEN,
         message_metadata: object | NotGiven = NOT_GIVEN,
         role: Optional[Literal["user", "assistant", "system", "tool"]] | NotGiven = NOT_GIVEN,
+        tool_calls: Optional[Iterable[object]] | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
     ) -> MessageResponse:
@@ -366,18 +366,18 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         return await self._patch(
             f"/api/v1/messages/{message_id}",
             body=await async_maybe_transform(
                 {
-                    "tool_calls": tool_calls,
                     "content": content,
                     "message_metadata": message_metadata,
                     "role": role,
+                    "tool_calls": tool_calls,
                 },
                 message_update_params.MessageUpdateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
             cast_to=MessageResponse,
```

### Comparing `altmindpy-0.1.0/src/altmind/resources/messages/thread.py` & `altmindpy-0.2.0/src/altmind/resources/messages/thread.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/__init__.py` & `altmindpy-0.2.0/src/altmind/resources/users/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/open.py` & `altmindpy-0.2.0/src/altmind/resources/users/open.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/users.py` & `altmindpy-0.2.0/src/altmind/resources/users/users.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/me/__init__.py` & `altmindpy-0.2.0/src/altmind/resources/users/me/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/me/me.py` & `altmindpy-0.2.0/src/altmind/resources/users/me/me.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/resources/users/me/password.py` & `altmindpy-0.2.0/src/altmind/resources/users/me/password.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/types/__init__.py` & `altmindpy-0.2.0/src/altmind/types/__init__.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/types/assistant_response.py` & `altmindpy-0.2.0/src/altmind/types/assistant_response.py`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/src/altmind/types/message_create_params.py` & `altmindpy-0.2.0/src/altmind/types/message_update_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 
 from __future__ import annotations
 
 from typing import Union, Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = [
-    "MessageCreateParams",
+    "MessageUpdateParams",
     "Content",
     "ContentTextContent",
     "ContentTextContentText",
     "ContentImageFileContent",
     "ContentImageFileContentImageFile",
     "ContentToolContent",
     "ContentToolContentTool",
 ]
 
 
-class MessageCreateParams(TypedDict, total=False):
-    content: Required[Iterable[Content]]
-
-    tool_calls: Required[Optional[Iterable[object]]]
+class MessageUpdateParams(TypedDict, total=False):
+    content: Optional[Iterable[Content]]
 
     message_metadata: object
 
-    original_role: Optional[Literal["user", "assistant", "system", "tool"]]
-
     role: Optional[Literal["user", "assistant", "system", "tool"]]
 
-    thread_id: Optional[int]
+    tool_calls: Optional[Iterable[object]]
 
 
 class ContentTextContentText(TypedDict, total=False):
     value: Required[str]
 
 
 class ContentTextContent(TypedDict, total=False):
@@ -58,11 +54,11 @@
 
     tool_call_id: Optional[str]
 
 
 class ContentToolContent(TypedDict, total=False):
     tool: Required[ContentToolContentTool]
 
-    type: Literal["tool_output"]
+    type: Literal["tool"]
 
 
 Content = Union[ContentTextContent, ContentImageFileContent, ContentToolContent]
```

### Comparing `altmindpy-0.1.0/src/altmind/types/message_response.py` & `altmindpy-0.2.0/src/altmind/types/message_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
+import builtins
 from typing import List, Union, Optional
 from typing_extensions import Literal
 
 from .._models import BaseModel
 
 __all__ = [
     "MessageResponse",
@@ -44,31 +45,31 @@
 
     tool_call_id: Optional[str] = None
 
 
 class ContentToolContent(BaseModel):
     tool: ContentToolContentTool
 
-    type: Optional[Literal["tool_output"]] = None
+    type: Optional[Literal["tool"]] = None
 
 
 Content = Union[ContentTextContent, ContentImageFileContent, ContentToolContent]
 
 
 class MessageResponse(BaseModel):
     id: int
 
     content: List[Content]
 
     created_at: int
 
     original_role: Optional[Literal["user", "assistant", "system", "tool"]] = None
 
-    tool_calls: Optional[List[object]] = None
-
     message_metadata: Optional[object] = None
 
     object: Optional[Literal["message"]] = None
 
     role: Optional[Literal["user", "assistant", "system", "tool"]] = None
 
     thread_id: Optional[int] = None
+
+    tool_calls: Optional[List[builtins.object]] = None
```

### Comparing `altmindpy-0.1.0/src/altmind/types/run_create_params.py` & `altmindpy-0.2.0/src/altmind/types/run_create_params.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
-from typing import Optional
+from typing import Iterable, Optional
 from typing_extensions import Literal, Required, TypedDict
 
 __all__ = ["RunCreateParams"]
 
 
 class RunCreateParams(TypedDict, total=False):
     assistant_id: Required[Optional[int]]
@@ -22,8 +22,12 @@
     """Override the assistant instructions for this run"""
 
     model: Optional[str]
     """Override the assistant model for this run"""
 
     run_metadata: object
 
+    tool_choice: Optional[object]
+
+    tools: Optional[Iterable[object]]
+
     type: Literal["default", "analysis", "execution"]
```

### Comparing `altmindpy-0.1.0/src/altmind/types/run_response.py` & `altmindpy-0.2.0/src/altmind/types/run_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,7 +33,9 @@
     usage: Optional[Dict[str, int]] = None
 
     model: Optional[str] = None
 
     object: Optional[Literal["run"]] = None
 
     run_metadata: Optional[builtins.object] = None
+
+    tool_choice: Optional[builtins.object] = None
```

### Comparing `altmindpy-0.1.0/LICENSE` & `altmindpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altmindpy-0.1.0/pyproject.toml` & `altmindpy-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "altmindpy"
-version = "0.1.0"
+version = "0.2.0"
 description = "The official Python library for the altmind API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Altmind", email = "azzi.leonardo@gmail.com" },
 ]
 dependencies = [
```

### Comparing `altmindpy-0.1.0/PKG-INFO` & `altmindpy-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altmindpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: The official Python library for the altmind API
 Project-URL: Homepage, https://github.com/AltermindLabs/altmind-python
 Project-URL: Repository, https://github.com/AltermindLabs/altmind-python
 Author-email: Altmind <azzi.leonardo@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -60,19 +60,19 @@
 ```python
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
 
-user_out = client.users.create(
-    email="string",
+token = client.login.access_token(
     password="string",
+    username="string",
 )
-print(user_out.id)
+print(token.access_token)
 ```
 
 ## Async usage
 
 Simply import `AsyncAltmind` instead of `Altmind` and use `await` with each API call:
 
 ```python
@@ -81,19 +81,19 @@
 
 client = AsyncAltmind(
     access_token="My Access Token",
 )
 
 
 async def main() -> None:
-    user_out = await client.users.create(
-        email="string",
+    token = await client.login.access_token(
         password="string",
+        username="string",
     )
-    print(user_out.id)
+    print(token.access_token)
 
 
 asyncio.run(main())
 ```
 
 Functionality between the synchronous and asynchronous clients is otherwise identical.
 
@@ -120,17 +120,17 @@
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
 
 try:
-    client.users.create(
-        email="string",
+    client.login.access_token(
         password="string",
+        username="string",
     )
 except altmind.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
 except altmind.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
 except altmind.APIStatusError as e:
@@ -167,17 +167,17 @@
 client = Altmind(
     # default is 2
     max_retries=0,
     access_token="My Access Token",
 )
 
 # Or, configure per-request:
-client.with_options(max_retries=5).users.create(
-    email="string",
+client.with_options(max_retries=5).login.access_token(
     password="string",
+    username="string",
 )
 ```
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
@@ -195,17 +195,17 @@
 # More granular control:
 client = Altmind(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
     access_token="My Access Token",
 )
 
 # Override per-request:
-client.with_options(timeout=5.0).users.create(
-    email="string",
+client.with_options(timeout=5.0).login.access_token(
     password="string",
+    username="string",
 )
 ```
 
 On timeout, an `APITimeoutError` is thrown.
 
 Note that requests that time out are [retried twice by default](https://github.com/AltermindLabs/altmind-python/tree/main/#retries).
 
@@ -239,38 +239,38 @@
 
 ```py
 from altmind import Altmind
 
 client = Altmind(
     access_token="My Access Token",
 )
-response = client.users.with_raw_response.create(
-    email="string",
+response = client.login.with_raw_response.access_token(
     password="string",
+    username="string",
 )
 print(response.headers.get('X-My-Header'))
 
-user = response.parse()  # get the object that `users.create()` would have returned
-print(user.id)
+login = response.parse()  # get the object that `login.access_token()` would have returned
+print(login.access_token)
 ```
 
 These methods return an [`APIResponse`](https://github.com/AltermindLabs/altmind-python/tree/main/src/altmind/_response.py) object.
 
 The async client returns an [`AsyncAPIResponse`](https://github.com/AltermindLabs/altmind-python/tree/main/src/altmind/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
 ```python
-with client.users.with_streaming_response.create(
-    email="string",
+with client.login.with_streaming_response.access_token(
     password="string",
+    username="string",
 ) as response:
     print(response.headers.get("X-My-Header"))
 
     for line in response.iter_lines():
         print(line)
 ```
```

