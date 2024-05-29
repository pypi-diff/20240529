# Comparing `tmp/apache_skywalking_onepiece-1.1.1.tar.gz` & `tmp/apache_skywalking_onepiece-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_skywalking_onepiece-1.1.1.tar", max compression
+gzip compressed data, was "apache_skywalking_onepiece-1.1.2.tar", max compression
```

## Comparing `apache_skywalking_onepiece-1.1.1.tar` & `apache_skywalking_onepiece-1.1.2.tar`

### file list

```diff
@@ -1,183 +1,183 @@
--rwxr-xr-x   0        0        0    11357 2023-04-25 16:02:57.380283 apache_skywalking_onepiece-1.1.1/LICENSE
--rwxr-xr-x   0        0        0     3188 2023-04-25 16:02:57.386283 apache_skywalking_onepiece-1.1.1/README.md
--rwxr-xr-x   0        0        0     4102 2024-05-29 06:43:27.994272 apache_skywalking_onepiece-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-29 06:36:24.055065 apache_skywalking_onepiece-1.1.1/skywalking/.DS_Store
--rwxr-xr-x   0        0        0     2158 2023-04-25 16:02:57.620123 apache_skywalking_onepiece-1.1.1/skywalking/__init__.py
--rwxr-xr-x   0        0        0    17297 2023-04-25 16:02:57.628116 apache_skywalking_onepiece-1.1.1/skywalking/agent/__init__.py
--rwxr-xr-x   0        0        0     1629 2023-04-25 16:02:57.639114 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/__init__.py
--rwxr-xr-x   0        0        0    10328 2023-04-25 16:02:57.646115 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/grpc.py
--rwxr-xr-x   0        0        0     4103 2023-04-25 16:02:57.651123 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/http.py
--rwxr-xr-x   0        0        0     3186 2023-04-25 16:02:57.658116 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/interceptors.py
--rwxr-xr-x   0        0        0     7071 2023-04-25 16:02:57.663120 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/kafka.py
--rwxr-xr-x   0        0        0     1441 2023-04-25 16:02:57.671121 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/__init__.py
--rwxr-xr-x   0        0        0      895 2023-04-25 16:02:57.681660 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/__init__.py
--rwxr-xr-x   0        0        0     4119 2023-04-25 16:02:57.688661 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/sw_python.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.701659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/__init__.py
--rwxr-xr-x   0        0        0     6133 2023-04-25 16:02:57.709659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/runner.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.720660 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/__init__.py
--rwxr-xr-x   0        0        0     2558 2023-04-25 16:02:57.727659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/uwsgi_hook.py
--rwxr-xr-x   0        0        0     1002 2023-04-25 16:02:57.738659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/__init__.py
--rwxr-xr-x   0        0        0     9252 2023-04-25 16:02:57.746653 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/sitecustomize.py
--rwxr-xr-x   0        0        0     4594 2023-04-25 16:02:57.754661 apache_skywalking_onepiece-1.1.1/skywalking/client/__init__.py
--rwxr-xr-x   0        0        0     4522 2023-04-25 16:02:57.759675 apache_skywalking_onepiece-1.1.1/skywalking/client/grpc.py
--rwxr-xr-x   0        0        0     5455 2023-04-25 16:02:57.764672 apache_skywalking_onepiece-1.1.1/skywalking/client/http.py
--rwxr-xr-x   0        0        0     5168 2023-04-25 16:02:57.770667 apache_skywalking_onepiece-1.1.1/skywalking/client/kafka.py
--rwxr-xr-x   0        0        0      884 2023-04-25 16:02:57.782210 apache_skywalking_onepiece-1.1.1/skywalking/command/__init__.py
--rwxr-xr-x   0        0        0     1008 2023-04-25 16:02:57.791209 apache_skywalking_onepiece-1.1.1/skywalking/command/base_command.py
--rwxr-xr-x   0        0        0     4436 2023-04-25 16:02:57.799205 apache_skywalking_onepiece-1.1.1/skywalking/command/command_service.py
--rwxr-xr-x   0        0        0      925 2023-04-25 16:02:57.813213 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/__init__.py
--rwxr-xr-x   0        0        0      878 2023-04-25 16:02:57.823215 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/command_executor.py
--rwxr-xr-x   0        0        0     1058 2023-04-25 16:02:57.830204 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/noop_command_executor.py
--rwxr-xr-x   0        0        0     1783 2023-04-25 16:02:57.838216 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/profile_task_command_executor.py
--rwxr-xr-x   0        0        0     3483 2023-04-25 16:02:57.845214 apache_skywalking_onepiece-1.1.1/skywalking/command/profile_task_command.py
--rwxr-xr-x   0        0        0    19613 2023-04-25 16:02:57.851205 apache_skywalking_onepiece-1.1.1/skywalking/config.py
--rwxr-xr-x   0        0        0     2922 2023-04-25 16:02:57.856206 apache_skywalking_onepiece-1.1.1/skywalking/decorators.py
--rwxr-xr-x   0        0        0     1206 2023-04-25 16:02:57.865245 apache_skywalking_onepiece-1.1.1/skywalking/log/__init__.py
--rwxr-xr-x   0        0        0     1736 2023-04-25 16:02:57.872235 apache_skywalking_onepiece-1.1.1/skywalking/log/formatter.py
--rwxr-xr-x   0        0        0     4907 2024-05-29 06:38:52.521523 apache_skywalking_onepiece-1.1.1/skywalking/log/sw_logging.py
--rwxr-xr-x   0        0        0     1462 2023-04-25 16:02:57.881760 apache_skywalking_onepiece-1.1.1/skywalking/loggings.py
--rwxr-xr-x   0        0        0     1181 2023-04-25 16:02:57.891761 apache_skywalking_onepiece-1.1.1/skywalking/meter/__init__.py
--rwxr-xr-x   0        0        0     3314 2023-04-25 16:02:57.898768 apache_skywalking_onepiece-1.1.1/skywalking/meter/counter.py
--rwxr-xr-x   0        0        0     1592 2023-04-25 16:02:57.903771 apache_skywalking_onepiece-1.1.1/skywalking/meter/gauge.py
--rwxr-xr-x   0        0        0     4111 2023-04-25 16:02:57.909769 apache_skywalking_onepiece-1.1.1/skywalking/meter/histogram.py
--rwxr-xr-x   0        0        0     3619 2023-04-25 16:02:57.915760 apache_skywalking_onepiece-1.1.1/skywalking/meter/meter.py
--rwxr-xr-x   0        0        0     2049 2023-04-25 16:02:57.921768 apache_skywalking_onepiece-1.1.1/skywalking/meter/meter_service.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.933768 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/__init__.py
--rwxr-xr-x   0        0        0     1194 2023-04-25 16:02:57.943761 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/cpu_usage.py
--rwxr-xr-x   0        0        0     1074 2023-04-25 16:02:57.950773 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/data_source.py
--rwxr-xr-x   0        0        0     1625 2023-04-25 16:02:57.957768 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/gc_data.py
--rwxr-xr-x   0        0        0     1241 2023-04-25 16:02:57.964790 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/mem_usage.py
--rwxr-xr-x   0        0        0     1273 2023-04-25 16:02:57.971785 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/thread_data.py
--rwxr-xr-x   0        0        0     4351 2023-04-25 16:02:57.981939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/__init__.py
--rwxr-xr-x   0        0        0     3965 2023-04-25 16:02:57.988935 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiohttp.py
--rwxr-xr-x   0        0        0     2079 2023-04-25 16:02:57.994936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aioredis.py
--rwxr-xr-x   0        0        0     3888 2023-04-25 16:02:58.000938 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiormq.py
--rwxr-xr-x   0        0        0     3831 2023-04-25 16:02:58.005936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_amqp.py
--rwxr-xr-x   0        0        0     4832 2023-04-25 16:02:58.011935 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_asyncpg.py
--rwxr-xr-x   0        0        0     3162 2023-04-25 16:02:58.017939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_bottle.py
--rwxr-xr-x   0        0        0     4666 2023-04-25 16:02:58.023936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_celery.py
--rwxr-xr-x   0        0        0     5229 2023-04-25 16:02:58.028937 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_confluent_kafka.py
--rwxr-xr-x   0        0        0     3784 2023-04-25 16:02:58.034936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_django.py
--rwxr-xr-x   0        0        0     1986 2023-04-25 16:02:58.039928 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_elasticsearch.py
--rwxr-xr-x   0        0        0     3255 2023-04-25 16:02:58.044936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_falcon.py
--rwxr-xr-x   0        0        0     4067 2023-04-25 16:02:58.051928 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_fastapi.py
--rwxr-xr-x   0        0        0     3593 2023-04-25 16:02:58.056937 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_flask.py
--rwxr-xr-x   0        0        0     4734 2023-04-25 16:02:58.062945 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_happybase.py
--rwxr-xr-x   0        0        0     5562 2023-04-25 16:02:58.068939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_http_server.py
--rwxr-xr-x   0        0        0     3849 2023-04-25 16:02:58.074471 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_httpx.py
--rwxr-xr-x   0        0        0     4086 2023-04-25 16:02:58.080478 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_kafka.py
--rwxr-xr-x   0        0        0     4171 2023-04-25 16:02:58.085477 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_loguru.py
--rwxr-xr-x   0        0        0     3077 2023-04-25 16:02:58.090485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_mysqlclient.py
--rwxr-xr-x   0        0        0    10581 2023-04-25 16:02:58.096486 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg.py
--rwxr-xr-x   0        0        0     6447 2023-04-25 16:02:58.102484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg2.py
--rwxr-xr-x   0        0        0     5706 2023-04-25 16:02:58.107488 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymongo.py
--rwxr-xr-x   0        0        0     2142 2023-04-25 16:02:58.113484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymysql.py
--rwxr-xr-x   0        0        0     2269 2023-04-25 16:02:58.118479 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pyramid.py
--rwxr-xr-x   0        0        0     7145 2023-04-25 16:02:58.124477 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_rabbitmq.py
--rwxr-xr-x   0        0        0     3372 2023-04-25 16:02:58.129475 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_redis.py
--rwxr-xr-x   0        0        0     3095 2023-04-25 16:02:58.134485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_requests.py
--rwxr-xr-x   0        0        0     4200 2023-04-25 16:02:58.140488 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_sanic.py
--rwxr-xr-x   0        0        0     4910 2023-04-25 16:02:58.147484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_tornado.py
--rwxr-xr-x   0        0        0     2346 2023-04-25 16:02:58.153487 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib3.py
--rwxr-xr-x   0        0        0     2717 2023-04-25 16:02:58.158485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib_request.py
--rwxr-xr-x   0        0        0     4021 2023-04-25 16:02:58.163492 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_websockets.py
--rwxr-xr-x   0        0        0     1082 2023-04-25 16:02:58.172501 apache_skywalking_onepiece-1.1.1/skywalking/profile/__init__.py
--rwxr-xr-x   0        0        0     1183 2023-04-25 16:02:58.179027 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_constants.py
--rwxr-xr-x   0        0        0    14758 2023-04-25 16:02:58.185027 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_context.py
--rwxr-xr-x   0        0        0     9316 2023-04-25 16:02:58.190026 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_service.py
--rwxr-xr-x   0        0        0     1539 2023-04-25 16:02:58.195035 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_status.py
--rwxr-xr-x   0        0        0     1820 2023-04-25 16:02:58.199036 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_task.py
--rwxr-xr-x   0        0        0     1610 2023-04-25 16:02:58.204034 apache_skywalking_onepiece-1.1.1/skywalking/profile/snapshot.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.165192 apache_skywalking_onepiece-1.1.1/skywalking/protocol/__init__.py
--rwxr-xr-x   0        0        0     1832 2023-04-29 19:50:32.982585 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2.py
--rwxr-xr-x   0        0        0      238 2023-04-29 19:50:32.543551 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2.pyi
--rwxr-xr-x   0        0        0     4248 2023-04-29 19:50:32.991585 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     3434 2023-04-29 19:50:32.999764 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.py
--rwxr-xr-x   0        0        0     4060 2023-04-29 19:50:32.564635 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.pyi
--rwxr-xr-x   0        0        0     4318 2023-04-29 19:50:33.009694 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.976019 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/__init__.py
--rwxr-xr-x   0        0        0     1631 2023-04-29 19:50:33.024771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.py
--rwxr-xr-x   0        0        0     1052 2023-04-29 19:50:32.585752 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.pyi
--rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.032771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2_grpc.py
--rwxr-xr-x   0        0        0     1988 2023-04-29 19:50:33.047772 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.py
--rwxr-xr-x   0        0        0     1463 2023-04-29 19:50:32.610341 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.pyi
--rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.058771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.016771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/__init__.py
--rwxr-xr-x   0        0        0     2592 2023-04-29 19:50:33.073954 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.py
--rwxr-xr-x   0        0        0     2298 2023-04-29 19:50:32.632968 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.pyi
--rwxr-xr-x   0        0        0     2916 2023-04-29 19:50:33.082968 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.066772 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/__init__.py
--rwxr-xr-x   0        0        0     1743 2023-04-29 19:50:33.096049 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2.py
--rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.652977 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2.pyi
--rwxr-xr-x   0        0        0     2659 2023-04-29 19:50:33.105289 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:33.114301 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.py
--rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:32.672480 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.pyi
--rwxr-xr-x   0        0        0     2701 2023-04-29 19:50:33.122302 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2_grpc.py
--rwxr-xr-x   0        0        0     1881 2023-04-29 19:50:33.133291 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.py
--rwxr-xr-x   0        0        0      545 2023-04-29 19:50:32.692232 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.pyi
--rwxr-xr-x   0        0        0     3563 2023-04-29 19:50:33.142286 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2_grpc.py
--rwxr-xr-x   0        0        0     1740 2023-04-29 19:50:33.151864 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2.py
--rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.712371 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2.pyi
--rwxr-xr-x   0        0        0     2620 2023-04-29 19:50:33.162209 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     4336 2023-04-29 19:50:33.171210 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.py
--rwxr-xr-x   0        0        0     5568 2023-04-29 19:50:32.742081 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.pyi
--rwxr-xr-x   0        0        0     2662 2023-04-29 19:50:33.181212 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2_grpc.py
--rwxr-xr-x   0        0        0     1701 2023-04-29 19:50:33.191024 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2.py
--rwxr-xr-x   0        0        0      233 2023-04-29 19:50:32.762005 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2.pyi
--rwxr-xr-x   0        0        0     2692 2023-04-29 19:50:33.200273 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     3036 2023-04-29 19:50:33.210276 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.py
--rwxr-xr-x   0        0        0     3101 2023-04-29 19:50:32.780009 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.pyi
--rwxr-xr-x   0        0        0     4696 2023-04-29 19:50:33.220471 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2_grpc.py
--rwxr-xr-x   0        0        0     1845 2023-04-29 19:50:33.232472 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2.py
--rwxr-xr-x   0        0        0      237 2023-04-29 19:50:32.799943 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2.pyi
--rwxr-xr-x   0        0        0     5037 2023-04-29 19:50:33.243973 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     5861 2023-04-29 19:50:33.251964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.py
--rwxr-xr-x   0        0        0     7713 2023-04-29 19:50:32.819120 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.pyi
--rwxr-xr-x   0        0        0     8576 2023-04-29 19:50:33.262964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.090548 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/__init__.py
--rwxr-xr-x   0        0        0     3150 2023-04-29 19:50:33.276964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.py
--rwxr-xr-x   0        0        0     3202 2023-04-29 19:50:32.841120 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.pyi
--rwxr-xr-x   0        0        0     2769 2023-04-29 19:50:33.285980 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.269964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/__init__.py
--rwxr-xr-x   0        0        0     1805 2023-04-29 19:50:33.300596 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2.py
--rwxr-xr-x   0        0        0      239 2023-04-29 19:50:32.869202 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2.pyi
--rwxr-xr-x   0        0        0     4469 2023-04-29 19:50:33.310752 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     2260 2023-04-29 19:50:33.319756 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.py
--rwxr-xr-x   0        0        0     1503 2023-04-29 19:50:32.891552 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.pyi
--rwxr-xr-x   0        0        0     4539 2023-04-29 19:50:33.327952 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.294980 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/__init__.py
--rwxr-xr-x   0        0        0     1900 2023-04-29 19:50:33.340963 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2.py
--rwxr-xr-x   0        0        0      230 2023-04-29 19:50:32.912940 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2.pyi
--rwxr-xr-x   0        0        0     5824 2023-04-29 19:50:33.350571 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2_grpc.py
--rwxr-xr-x   0        0        0     2725 2023-04-29 19:50:33.358571 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.py
--rwxr-xr-x   0        0        0     2183 2023-04-29 19:50:32.930949 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.pyi
--rwxr-xr-x   0        0        0     5922 2023-04-29 19:50:33.369147 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2_grpc.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.335964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/__init__.py
--rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.377153 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/__init__.py
--rwxr-xr-x   0        0        0     4632 2023-04-29 19:50:33.385164 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.py
--rwxr-xr-x   0        0        0     6980 2023-04-29 19:50:32.954545 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.pyi
--rwxr-xr-x   0        0        0     3043 2023-04-29 19:50:33.395161 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2_grpc.py
--rwxr-xr-x   0        0        0     1053 2023-04-25 16:02:58.211034 apache_skywalking_onepiece-1.1.1/skywalking/trace/__init__.py
--rwxr-xr-x   0        0        0     4860 2023-04-25 16:02:58.217035 apache_skywalking_onepiece-1.1.1/skywalking/trace/carrier.py
--rwxr-xr-x   0        0        0    10585 2023-04-25 16:02:58.221050 apache_skywalking_onepiece-1.1.1/skywalking/trace/context.py
--rwxr-xr-x   0        0        0     3250 2023-04-25 16:02:58.226034 apache_skywalking_onepiece-1.1.1/skywalking/trace/segment.py
--rwxr-xr-x   0        0        0     1673 2023-04-25 16:02:58.230027 apache_skywalking_onepiece-1.1.1/skywalking/trace/snapshot.py
--rwxr-xr-x   0        0        0     6714 2023-04-25 16:02:58.235027 apache_skywalking_onepiece-1.1.1/skywalking/trace/span.py
--rwxr-xr-x   0        0        0     1935 2023-04-25 16:02:58.239037 apache_skywalking_onepiece-1.1.1/skywalking/trace/tags.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.247035 apache_skywalking_onepiece-1.1.1/skywalking/utils/__init__.py
--rwxr-xr-x   0        0        0     2179 2023-04-25 16:02:58.253027 apache_skywalking_onepiece-1.1.1/skywalking/utils/array.py
--rwxr-xr-x   0        0        0     1511 2023-04-25 16:02:58.257035 apache_skywalking_onepiece-1.1.1/skywalking/utils/atomic_ref.py
--rwxr-xr-x   0        0        0     1029 2023-04-25 16:02:58.263043 apache_skywalking_onepiece-1.1.1/skywalking/utils/comparator.py
--rwxr-xr-x   0        0        0     1213 2023-04-25 16:02:58.268052 apache_skywalking_onepiece-1.1.1/skywalking/utils/counter.py
--rwxr-xr-x   0        0        0     1016 2023-04-25 16:02:58.273043 apache_skywalking_onepiece-1.1.1/skywalking/utils/exception.py
--rwxr-xr-x   0        0        0     1627 2023-04-25 16:02:58.277588 apache_skywalking_onepiece-1.1.1/skywalking/utils/filter.py
--rwxr-xr-x   0        0        0     1220 2023-04-25 16:02:58.281579 apache_skywalking_onepiece-1.1.1/skywalking/utils/integer.py
--rwxr-xr-x   0        0        0     1187 2023-04-25 16:02:58.285587 apache_skywalking_onepiece-1.1.1/skywalking/utils/lang.py
--rwxr-xr-x   0        0        0     1370 2023-04-25 16:02:58.289586 apache_skywalking_onepiece-1.1.1/skywalking/utils/singleton.py
--rwxr-xr-x   0        0        0      863 2023-04-25 16:02:58.294587 apache_skywalking_onepiece-1.1.1/skywalking/utils/time.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.299578 apache_skywalking_onepiece-1.1.1/sw_python/__init__.py
--rwxr-xr-x   0        0        0      837 2023-04-25 16:02:58.304586 apache_skywalking_onepiece-1.1.1/sw_python/__main__.py
--rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.313580 apache_skywalking_onepiece-1.1.1/sw_python/src/__init__.py
--rwxr-xr-x   0        0        0     1019 2023-04-25 16:02:58.319587 apache_skywalking_onepiece-1.1.1/sw_python/src/sw_python.py
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.1/setup.py
--rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2023-04-25 16:02:57.380283 apache_skywalking_onepiece-1.1.2/LICENSE
+-rwxr-xr-x   0        0        0     3188 2023-04-25 16:02:57.386283 apache_skywalking_onepiece-1.1.2/README.md
+-rwxr-xr-x   0        0        0     4102 2024-05-29 07:10:25.032441 apache_skywalking_onepiece-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-29 06:36:24.055065 apache_skywalking_onepiece-1.1.2/skywalking/.DS_Store
+-rwxr-xr-x   0        0        0     2158 2023-04-25 16:02:57.620123 apache_skywalking_onepiece-1.1.2/skywalking/__init__.py
+-rwxr-xr-x   0        0        0    17297 2023-04-25 16:02:57.628116 apache_skywalking_onepiece-1.1.2/skywalking/agent/__init__.py
+-rwxr-xr-x   0        0        0     1629 2023-04-25 16:02:57.639114 apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/__init__.py
+-rwxr-xr-x   0        0        0    10328 2023-04-25 16:02:57.646115 apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/grpc.py
+-rwxr-xr-x   0        0        0     4103 2023-04-25 16:02:57.651123 apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/http.py
+-rwxr-xr-x   0        0        0     3186 2023-04-25 16:02:57.658116 apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/interceptors.py
+-rwxr-xr-x   0        0        0     7071 2023-04-25 16:02:57.663120 apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/kafka.py
+-rwxr-xr-x   0        0        0     1441 2023-04-25 16:02:57.671121 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/__init__.py
+-rwxr-xr-x   0        0        0      895 2023-04-25 16:02:57.681660 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/__init__.py
+-rwxr-xr-x   0        0        0     4119 2023-04-25 16:02:57.688661 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/sw_python.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.701659 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/utility/__init__.py
+-rwxr-xr-x   0        0        0     6133 2023-04-25 16:02:57.709659 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/utility/runner.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.720660 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/hooks/__init__.py
+-rwxr-xr-x   0        0        0     2558 2023-04-25 16:02:57.727659 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/hooks/uwsgi_hook.py
+-rwxr-xr-x   0        0        0     1002 2023-04-25 16:02:57.738659 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/loader/__init__.py
+-rwxr-xr-x   0        0        0     9252 2023-04-25 16:02:57.746653 apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/loader/sitecustomize.py
+-rwxr-xr-x   0        0        0     4594 2023-04-25 16:02:57.754661 apache_skywalking_onepiece-1.1.2/skywalking/client/__init__.py
+-rwxr-xr-x   0        0        0     4522 2023-04-25 16:02:57.759675 apache_skywalking_onepiece-1.1.2/skywalking/client/grpc.py
+-rwxr-xr-x   0        0        0     5455 2023-04-25 16:02:57.764672 apache_skywalking_onepiece-1.1.2/skywalking/client/http.py
+-rwxr-xr-x   0        0        0     5168 2023-04-25 16:02:57.770667 apache_skywalking_onepiece-1.1.2/skywalking/client/kafka.py
+-rwxr-xr-x   0        0        0      884 2023-04-25 16:02:57.782210 apache_skywalking_onepiece-1.1.2/skywalking/command/__init__.py
+-rwxr-xr-x   0        0        0     1008 2023-04-25 16:02:57.791209 apache_skywalking_onepiece-1.1.2/skywalking/command/base_command.py
+-rwxr-xr-x   0        0        0     4436 2023-04-25 16:02:57.799205 apache_skywalking_onepiece-1.1.2/skywalking/command/command_service.py
+-rwxr-xr-x   0        0        0      925 2023-04-25 16:02:57.813213 apache_skywalking_onepiece-1.1.2/skywalking/command/executors/__init__.py
+-rwxr-xr-x   0        0        0      878 2023-04-25 16:02:57.823215 apache_skywalking_onepiece-1.1.2/skywalking/command/executors/command_executor.py
+-rwxr-xr-x   0        0        0     1058 2023-04-25 16:02:57.830204 apache_skywalking_onepiece-1.1.2/skywalking/command/executors/noop_command_executor.py
+-rwxr-xr-x   0        0        0     1783 2023-04-25 16:02:57.838216 apache_skywalking_onepiece-1.1.2/skywalking/command/executors/profile_task_command_executor.py
+-rwxr-xr-x   0        0        0     3483 2023-04-25 16:02:57.845214 apache_skywalking_onepiece-1.1.2/skywalking/command/profile_task_command.py
+-rwxr-xr-x   0        0        0    19613 2023-04-25 16:02:57.851205 apache_skywalking_onepiece-1.1.2/skywalking/config.py
+-rwxr-xr-x   0        0        0     2922 2023-04-25 16:02:57.856206 apache_skywalking_onepiece-1.1.2/skywalking/decorators.py
+-rwxr-xr-x   0        0        0     1206 2023-04-25 16:02:57.865245 apache_skywalking_onepiece-1.1.2/skywalking/log/__init__.py
+-rwxr-xr-x   0        0        0     1736 2023-04-25 16:02:57.872235 apache_skywalking_onepiece-1.1.2/skywalking/log/formatter.py
+-rwxr-xr-x   0        0        0     4906 2024-05-29 07:09:54.517949 apache_skywalking_onepiece-1.1.2/skywalking/log/sw_logging.py
+-rwxr-xr-x   0        0        0     1462 2023-04-25 16:02:57.881760 apache_skywalking_onepiece-1.1.2/skywalking/loggings.py
+-rwxr-xr-x   0        0        0     1181 2023-04-25 16:02:57.891761 apache_skywalking_onepiece-1.1.2/skywalking/meter/__init__.py
+-rwxr-xr-x   0        0        0     3314 2023-04-25 16:02:57.898768 apache_skywalking_onepiece-1.1.2/skywalking/meter/counter.py
+-rwxr-xr-x   0        0        0     1592 2023-04-25 16:02:57.903771 apache_skywalking_onepiece-1.1.2/skywalking/meter/gauge.py
+-rwxr-xr-x   0        0        0     4111 2023-04-25 16:02:57.909769 apache_skywalking_onepiece-1.1.2/skywalking/meter/histogram.py
+-rwxr-xr-x   0        0        0     3619 2023-04-25 16:02:57.915760 apache_skywalking_onepiece-1.1.2/skywalking/meter/meter.py
+-rwxr-xr-x   0        0        0     2049 2023-04-25 16:02:57.921768 apache_skywalking_onepiece-1.1.2/skywalking/meter/meter_service.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.933768 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/__init__.py
+-rwxr-xr-x   0        0        0     1194 2023-04-25 16:02:57.943761 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/cpu_usage.py
+-rwxr-xr-x   0        0        0     1074 2023-04-25 16:02:57.950773 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/data_source.py
+-rwxr-xr-x   0        0        0     1625 2023-04-25 16:02:57.957768 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/gc_data.py
+-rwxr-xr-x   0        0        0     1241 2023-04-25 16:02:57.964790 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/mem_usage.py
+-rwxr-xr-x   0        0        0     1273 2023-04-25 16:02:57.971785 apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/thread_data.py
+-rwxr-xr-x   0        0        0     4351 2023-04-25 16:02:57.981939 apache_skywalking_onepiece-1.1.2/skywalking/plugins/__init__.py
+-rwxr-xr-x   0        0        0     3965 2023-04-25 16:02:57.988935 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aiohttp.py
+-rwxr-xr-x   0        0        0     2079 2023-04-25 16:02:57.994936 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aioredis.py
+-rwxr-xr-x   0        0        0     3888 2023-04-25 16:02:58.000938 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aiormq.py
+-rwxr-xr-x   0        0        0     3831 2023-04-25 16:02:58.005936 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_amqp.py
+-rwxr-xr-x   0        0        0     4832 2023-04-25 16:02:58.011935 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_asyncpg.py
+-rwxr-xr-x   0        0        0     3162 2023-04-25 16:02:58.017939 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_bottle.py
+-rwxr-xr-x   0        0        0     4666 2023-04-25 16:02:58.023936 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_celery.py
+-rwxr-xr-x   0        0        0     5229 2023-04-25 16:02:58.028937 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_confluent_kafka.py
+-rwxr-xr-x   0        0        0     3784 2023-04-25 16:02:58.034936 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_django.py
+-rwxr-xr-x   0        0        0     1986 2023-04-25 16:02:58.039928 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_elasticsearch.py
+-rwxr-xr-x   0        0        0     3255 2023-04-25 16:02:58.044936 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_falcon.py
+-rwxr-xr-x   0        0        0     4067 2023-04-25 16:02:58.051928 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_fastapi.py
+-rwxr-xr-x   0        0        0     3593 2023-04-25 16:02:58.056937 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_flask.py
+-rwxr-xr-x   0        0        0     4734 2023-04-25 16:02:58.062945 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_happybase.py
+-rwxr-xr-x   0        0        0     5562 2023-04-25 16:02:58.068939 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_http_server.py
+-rwxr-xr-x   0        0        0     3849 2023-04-25 16:02:58.074471 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_httpx.py
+-rwxr-xr-x   0        0        0     4086 2023-04-25 16:02:58.080478 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_kafka.py
+-rwxr-xr-x   0        0        0     4171 2023-04-25 16:02:58.085477 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_loguru.py
+-rwxr-xr-x   0        0        0     3077 2023-04-25 16:02:58.090485 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_mysqlclient.py
+-rwxr-xr-x   0        0        0    10581 2023-04-25 16:02:58.096486 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_psycopg.py
+-rwxr-xr-x   0        0        0     6447 2023-04-25 16:02:58.102484 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_psycopg2.py
+-rwxr-xr-x   0        0        0     5706 2023-04-25 16:02:58.107488 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pymongo.py
+-rwxr-xr-x   0        0        0     2142 2023-04-25 16:02:58.113484 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pymysql.py
+-rwxr-xr-x   0        0        0     2269 2023-04-25 16:02:58.118479 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pyramid.py
+-rwxr-xr-x   0        0        0     7145 2023-04-25 16:02:58.124477 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_rabbitmq.py
+-rwxr-xr-x   0        0        0     3372 2023-04-25 16:02:58.129475 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_redis.py
+-rwxr-xr-x   0        0        0     3095 2023-04-25 16:02:58.134485 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_requests.py
+-rwxr-xr-x   0        0        0     4200 2023-04-25 16:02:58.140488 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_sanic.py
+-rwxr-xr-x   0        0        0     4910 2023-04-25 16:02:58.147484 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_tornado.py
+-rwxr-xr-x   0        0        0     2346 2023-04-25 16:02:58.153487 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_urllib3.py
+-rwxr-xr-x   0        0        0     2717 2023-04-25 16:02:58.158485 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_urllib_request.py
+-rwxr-xr-x   0        0        0     4021 2023-04-25 16:02:58.163492 apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_websockets.py
+-rwxr-xr-x   0        0        0     1082 2023-04-25 16:02:58.172501 apache_skywalking_onepiece-1.1.2/skywalking/profile/__init__.py
+-rwxr-xr-x   0        0        0     1183 2023-04-25 16:02:58.179027 apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_constants.py
+-rwxr-xr-x   0        0        0    14758 2023-04-25 16:02:58.185027 apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_context.py
+-rwxr-xr-x   0        0        0     9316 2023-04-25 16:02:58.190026 apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_service.py
+-rwxr-xr-x   0        0        0     1539 2023-04-25 16:02:58.195035 apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_status.py
+-rwxr-xr-x   0        0        0     1820 2023-04-25 16:02:58.199036 apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_task.py
+-rwxr-xr-x   0        0        0     1610 2023-04-25 16:02:58.204034 apache_skywalking_onepiece-1.1.2/skywalking/profile/snapshot.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.165192 apache_skywalking_onepiece-1.1.2/skywalking/protocol/__init__.py
+-rwxr-xr-x   0        0        0     1832 2023-04-29 19:50:32.982585 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerfCompat_pb2.py
+-rwxr-xr-x   0        0        0      238 2023-04-29 19:50:32.543551 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerfCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     4248 2023-04-29 19:50:32.991585 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerfCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     3434 2023-04-29 19:50:32.999764 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2.py
+-rwxr-xr-x   0        0        0     4060 2023-04-29 19:50:32.564635 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2.pyi
+-rwxr-xr-x   0        0        0     4318 2023-04-29 19:50:33.009694 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.976019 apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/__init__.py
+-rwxr-xr-x   0        0        0     1631 2023-04-29 19:50:33.024771 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Command_pb2.py
+-rwxr-xr-x   0        0        0     1052 2023-04-29 19:50:32.585752 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Command_pb2.pyi
+-rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.032771 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Command_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1988 2023-04-29 19:50:33.047772 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Common_pb2.py
+-rwxr-xr-x   0        0        0     1463 2023-04-29 19:50:32.610341 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Common_pb2.pyi
+-rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.058771 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Common_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.016771 apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/__init__.py
+-rwxr-xr-x   0        0        0     2592 2023-04-29 19:50:33.073954 apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2.py
+-rwxr-xr-x   0        0        0     2298 2023-04-29 19:50:32.632968 apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2.pyi
+-rwxr-xr-x   0        0        0     2916 2023-04-29 19:50:33.082968 apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.066772 apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/__init__.py
+-rwxr-xr-x   0        0        0     1743 2023-04-29 19:50:33.096049 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetricCompat_pb2.py
+-rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.652977 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetricCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2659 2023-04-29 19:50:33.105289 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetricCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:33.114301 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2.py
+-rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:32.672480 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2.pyi
+-rwxr-xr-x   0        0        0     2701 2023-04-29 19:50:33.122302 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1881 2023-04-29 19:50:33.133291 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.py
+-rwxr-xr-x   0        0        0      545 2023-04-29 19:50:32.692232 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.pyi
+-rwxr-xr-x   0        0        0     3563 2023-04-29 19:50:33.142286 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1740 2023-04-29 19:50:33.151864 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetricCompat_pb2.py
+-rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.712371 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetricCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2620 2023-04-29 19:50:33.162209 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetricCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     4336 2023-04-29 19:50:33.171210 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2.py
+-rwxr-xr-x   0        0        0     5568 2023-04-29 19:50:32.742081 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2.pyi
+-rwxr-xr-x   0        0        0     2662 2023-04-29 19:50:33.181212 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1701 2023-04-29 19:50:33.191024 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/MeterCompat_pb2.py
+-rwxr-xr-x   0        0        0      233 2023-04-29 19:50:32.762005 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/MeterCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2692 2023-04-29 19:50:33.200273 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/MeterCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     3036 2023-04-29 19:50:33.210276 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2.py
+-rwxr-xr-x   0        0        0     3101 2023-04-29 19:50:32.780009 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2.pyi
+-rwxr-xr-x   0        0        0     4696 2023-04-29 19:50:33.220471 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1845 2023-04-29 19:50:33.232472 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/TracingCompat_pb2.py
+-rwxr-xr-x   0        0        0      237 2023-04-29 19:50:32.799943 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/TracingCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     5037 2023-04-29 19:50:33.243973 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/TracingCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     5861 2023-04-29 19:50:33.251964 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2.py
+-rwxr-xr-x   0        0        0     7713 2023-04-29 19:50:32.819120 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2.pyi
+-rwxr-xr-x   0        0        0     8576 2023-04-29 19:50:33.262964 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.090548 apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/__init__.py
+-rwxr-xr-x   0        0        0     3150 2023-04-29 19:50:33.276964 apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2.py
+-rwxr-xr-x   0        0        0     3202 2023-04-29 19:50:32.841120 apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2.pyi
+-rwxr-xr-x   0        0        0     2769 2023-04-29 19:50:33.285980 apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.269964 apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/__init__.py
+-rwxr-xr-x   0        0        0     1805 2023-04-29 19:50:33.300596 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/ManagementCompat_pb2.py
+-rwxr-xr-x   0        0        0      239 2023-04-29 19:50:32.869202 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/ManagementCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     4469 2023-04-29 19:50:33.310752 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/ManagementCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2260 2023-04-29 19:50:33.319756 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2.py
+-rwxr-xr-x   0        0        0     1503 2023-04-29 19:50:32.891552 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2.pyi
+-rwxr-xr-x   0        0        0     4539 2023-04-29 19:50:33.327952 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.294980 apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/__init__.py
+-rwxr-xr-x   0        0        0     1900 2023-04-29 19:50:33.340963 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/ProfileCompat_pb2.py
+-rwxr-xr-x   0        0        0      230 2023-04-29 19:50:32.912940 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/ProfileCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     5824 2023-04-29 19:50:33.350571 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/ProfileCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2725 2023-04-29 19:50:33.358571 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2.py
+-rwxr-xr-x   0        0        0     2183 2023-04-29 19:50:32.930949 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2.pyi
+-rwxr-xr-x   0        0        0     5922 2023-04-29 19:50:33.369147 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.335964 apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.377153 apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/__init__.py
+-rwxr-xr-x   0        0        0     4632 2023-04-29 19:50:33.385164 apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2.py
+-rwxr-xr-x   0        0        0     6980 2023-04-29 19:50:32.954545 apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2.pyi
+-rwxr-xr-x   0        0        0     3043 2023-04-29 19:50:33.395161 apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1053 2023-04-25 16:02:58.211034 apache_skywalking_onepiece-1.1.2/skywalking/trace/__init__.py
+-rwxr-xr-x   0        0        0     4860 2023-04-25 16:02:58.217035 apache_skywalking_onepiece-1.1.2/skywalking/trace/carrier.py
+-rwxr-xr-x   0        0        0    10585 2023-04-25 16:02:58.221050 apache_skywalking_onepiece-1.1.2/skywalking/trace/context.py
+-rwxr-xr-x   0        0        0     3250 2023-04-25 16:02:58.226034 apache_skywalking_onepiece-1.1.2/skywalking/trace/segment.py
+-rwxr-xr-x   0        0        0     1673 2023-04-25 16:02:58.230027 apache_skywalking_onepiece-1.1.2/skywalking/trace/snapshot.py
+-rwxr-xr-x   0        0        0     6714 2023-04-25 16:02:58.235027 apache_skywalking_onepiece-1.1.2/skywalking/trace/span.py
+-rwxr-xr-x   0        0        0     1935 2023-04-25 16:02:58.239037 apache_skywalking_onepiece-1.1.2/skywalking/trace/tags.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.247035 apache_skywalking_onepiece-1.1.2/skywalking/utils/__init__.py
+-rwxr-xr-x   0        0        0     2179 2023-04-25 16:02:58.253027 apache_skywalking_onepiece-1.1.2/skywalking/utils/array.py
+-rwxr-xr-x   0        0        0     1511 2023-04-25 16:02:58.257035 apache_skywalking_onepiece-1.1.2/skywalking/utils/atomic_ref.py
+-rwxr-xr-x   0        0        0     1029 2023-04-25 16:02:58.263043 apache_skywalking_onepiece-1.1.2/skywalking/utils/comparator.py
+-rwxr-xr-x   0        0        0     1213 2023-04-25 16:02:58.268052 apache_skywalking_onepiece-1.1.2/skywalking/utils/counter.py
+-rwxr-xr-x   0        0        0     1016 2023-04-25 16:02:58.273043 apache_skywalking_onepiece-1.1.2/skywalking/utils/exception.py
+-rwxr-xr-x   0        0        0     1627 2023-04-25 16:02:58.277588 apache_skywalking_onepiece-1.1.2/skywalking/utils/filter.py
+-rwxr-xr-x   0        0        0     1220 2023-04-25 16:02:58.281579 apache_skywalking_onepiece-1.1.2/skywalking/utils/integer.py
+-rwxr-xr-x   0        0        0     1187 2023-04-25 16:02:58.285587 apache_skywalking_onepiece-1.1.2/skywalking/utils/lang.py
+-rwxr-xr-x   0        0        0     1370 2023-04-25 16:02:58.289586 apache_skywalking_onepiece-1.1.2/skywalking/utils/singleton.py
+-rwxr-xr-x   0        0        0      863 2023-04-25 16:02:58.294587 apache_skywalking_onepiece-1.1.2/skywalking/utils/time.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.299578 apache_skywalking_onepiece-1.1.2/sw_python/__init__.py
+-rwxr-xr-x   0        0        0      837 2023-04-25 16:02:58.304586 apache_skywalking_onepiece-1.1.2/sw_python/__main__.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.313580 apache_skywalking_onepiece-1.1.2/sw_python/src/__init__.py
+-rwxr-xr-x   0        0        0     1019 2023-04-25 16:02:58.319587 apache_skywalking_onepiece-1.1.2/sw_python/src/sw_python.py
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.2/setup.py
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.2/PKG-INFO
```

### Comparing `apache_skywalking_onepiece-1.1.1/LICENSE` & `apache_skywalking_onepiece-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/README.md` & `apache_skywalking_onepiece-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/pyproject.toml` & `apache_skywalking_onepiece-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "apache-skywalking-onepiece"
-version = "1.1.1"
+version = "1.1.2"
 description = "The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects."
 license = "Apache-2.0"
 authors = ["Apache Software Foundation <dev@skywalking.apache.org>"]
 maintainers = ["Apache SkyWalking Community <dev@skywalking.apache.org>"]
 readme = "README.md"
 homepage = "https://skywalking.apache.org/"
 repository = "https://github.com/apache/skywalking-python"
```

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/.DS_Store` & `apache_skywalking_onepiece-1.1.2/skywalking/.DS_Store`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/http.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/http.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/interceptors.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/interceptors.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/kafka.py` & `apache_skywalking_onepiece-1.1.2/skywalking/agent/protocol/kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/sw_python.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/sw_python.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/runner.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/cli/utility/runner.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/uwsgi_hook.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/hooks/uwsgi_hook.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/sitecustomize.py` & `apache_skywalking_onepiece-1.1.2/skywalking/bootstrap/loader/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/client/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/client/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/client/grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/client/grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/client/http.py` & `apache_skywalking_onepiece-1.1.2/skywalking/client/http.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/client/kafka.py` & `apache_skywalking_onepiece-1.1.2/skywalking/client/kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/base_command.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/base_command.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/command_service.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/command_service.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/command_executor.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/executors/command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/noop_command_executor.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/executors/noop_command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/profile_task_command_executor.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/executors/profile_task_command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/command/profile_task_command.py` & `apache_skywalking_onepiece-1.1.2/skywalking/command/profile_task_command.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/config.py` & `apache_skywalking_onepiece-1.1.2/skywalking/config.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/decorators.py` & `apache_skywalking_onepiece-1.1.2/skywalking/decorators.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/log/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/log/formatter.py` & `apache_skywalking_onepiece-1.1.2/skywalking/log/formatter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/log/sw_logging.py` & `apache_skywalking_onepiece-1.1.2/skywalking/log/sw_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,18 @@
         from skywalking.log.formatter import SWFormatter
         sw_formatter = SWFormatter(fmt=layout, tb_limit=config.agent_cause_exception_depth)
 
     _handle = Logger.handle
     log_reporter_level = logging.getLevelName(config.agent_log_reporter_level)  # type: int
 
     def _sw_handle(self, record):
+        context = get_context()
+        if '%(tid)s' in layout:
+            record.tid = str(context.segment.related_traces[0])
+
         _handle(self=self, record=record)
 
         if self.disabled:
             return
 
         if record.name in ['skywalking', 'skywalking-cli', 'skywalking-loader']:  # Ignore SkyWalking internal loggers
             return
@@ -69,19 +73,14 @@
 
             if record.exc_info:
                 l_tags.data.append(KeyStringValuePair(key='exception',
                                                       value=sw_traceback()
                                                       ))  # \n doesn't work in tags for UI
             return l_tags
 
-        context = get_context()
-
-        if '%(tid)s' in layout:
-            record.tid = str(context.segment.related_traces[0])
-
         active_span_id = -1
         primary_endpoint_name = ''
 
         try:
             # Try to extract active span, if user code/plugin code throws uncaught
             # exceptions before any span is even created, just ignore these fields and
             # avoid appending 'no active span' traceback that could be confusing.
```

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/loggings.py` & `apache_skywalking_onepiece-1.1.2/skywalking/loggings.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/counter.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/counter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/gauge.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/gauge.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/histogram.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/histogram.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/meter.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/meter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/meter_service.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/meter_service.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/cpu_usage.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/data_source.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/data_source.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/gc_data.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/gc_data.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/mem_usage.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/mem_usage.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/thread_data.py` & `apache_skywalking_onepiece-1.1.2/skywalking/meter/pvm/thread_data.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiohttp.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aiohttp.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aioredis.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aioredis.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiormq.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_aiormq.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_amqp.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_amqp.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_asyncpg.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_asyncpg.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_bottle.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_bottle.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_celery.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_celery.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_confluent_kafka.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_django.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_django.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_elasticsearch.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_falcon.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_falcon.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_fastapi.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_fastapi.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_flask.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_flask.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_happybase.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_happybase.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_http_server.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_http_server.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_httpx.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_httpx.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_kafka.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_loguru.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_loguru.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_mysqlclient.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_mysqlclient.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_psycopg.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_psycopg2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymongo.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pymongo.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymysql.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pymysql.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pyramid.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_pyramid.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_rabbitmq.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_redis.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_redis.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_requests.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_requests.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_sanic.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_sanic.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_tornado.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_tornado.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib3.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_urllib3.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib_request.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_urllib_request.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_websockets.py` & `apache_skywalking_onepiece-1.1.2/skywalking/plugins/sw_websockets.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_constants.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_constants.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_context.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_context.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_service.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_service.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_status.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_status.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_task.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/profile_task.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/profile/snapshot.py` & `apache_skywalking_onepiece-1.1.2/skywalking/profile/snapshot.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerfCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerfCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/browser/BrowserPerf_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Command_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/common/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/event/Event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetricCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetricCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/CLRMetric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetricCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetricCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/JVMMetric_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/MeterCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/MeterCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Meter_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/TracingCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/TracingCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/language_agent/Tracing_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/logging/Logging_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/ManagementCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/ManagementCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/management/Management_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/ProfileCompat_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/ProfileCompat_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/profile/Profile_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.pyi` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2_grpc.py` & `apache_skywalking_onepiece-1.1.2/skywalking/protocol/service_mesh_probe/service_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/carrier.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/carrier.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/context.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/context.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/segment.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/segment.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/snapshot.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/snapshot.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/span.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/span.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/trace/tags.py` & `apache_skywalking_onepiece-1.1.2/skywalking/trace/tags.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/__init__.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/array.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/array.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/atomic_ref.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/atomic_ref.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/comparator.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/comparator.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/counter.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/counter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/exception.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/exception.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/filter.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/filter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/integer.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/integer.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/lang.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/lang.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/singleton.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/skywalking/utils/time.py` & `apache_skywalking_onepiece-1.1.2/skywalking/utils/time.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/sw_python/__init__.py` & `apache_skywalking_onepiece-1.1.2/sw_python/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/sw_python/__main__.py` & `apache_skywalking_onepiece-1.1.2/sw_python/__main__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/sw_python/src/__init__.py` & `apache_skywalking_onepiece-1.1.2/sw_python/src/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/sw_python/src/sw_python.py` & `apache_skywalking_onepiece-1.1.2/sw_python/src/sw_python.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.1/setup.py` & `apache_skywalking_onepiece-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
  'kafka': ['kafka-python']}
 
 entry_points = \
 {'console_scripts': ['sw-python = skywalking.bootstrap.cli.sw_python:start']}
 
 setup_kwargs = {
     'name': 'apache-skywalking-onepiece',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects.',
     'long_description': '# SkyWalking Python Agent\n\n<img src="http://skywalking.apache.org/assets/logo.svg" alt="Sky Walking logo" height="90px" align="right" />\n\n**SkyWalking-Python**: The Python Agent for Apache SkyWalking provides the native tracing/metrics/logging/profiling abilities for Python projects.\n\n**[SkyWalking](https://github.com/apache/skywalking)**: Application performance monitor tool for distributed systems, especially designed for microservices, cloud native and container-based (Kubernetes) architectures.\n\n\n[![GitHub stars](https://img.shields.io/github/stars/apache/skywalking-python.svg?style=for-the-badge&label=Stars&logo=github)](https://github.com/apache/skywalking-python)\n[![Twitter Follow](https://img.shields.io/twitter/follow/asfskywalking.svg?style=for-the-badge&label=Follow&logo=twitter)](https://twitter.com/AsfSkyWalking)\n\n![Release](https://img.shields.io/pypi/v/apache-skywalking)\n![Version](https://img.shields.io/pypi/pyversions/apache-skywalking)\n![Build](https://github.com/apache/skywalking-python/actions/workflows/CI.yaml/badge.svg?event=push)\n\n## Documentation\n\n- [Official documentation](https://skywalking.apache.org/docs/#PythonAgent)\n- [Blog](https://skywalking.apache.org/blog/2021-09-12-skywalking-python-profiling/) about the Python Agent Profiling Feature\n\n## Capabilities\n\n| Reporter  | Supported?      | Details                                                    | \n|:----------|:----------------|:-----------------------------------------------------------|\n| Trace     | ✅ (default: ON) | Automatic instrumentation + Manual SDK                     |            \n| Log       | ✅ (default: ON) | Direct reporter only. (Tracing context in log planned)     |\n| Meter     | ✅ (default: ON) | Meter API + Automatic PVM metrics                          |\n| Event     | ❌ (Planned)     | Report lifecycle events of your awesome Python application |\n| Profiling | ✅ (default: ON) | Threading and Greenlet Profiler                            |\n\n## Installation Requirements\n\nSkyWalking Python Agent requires [Apache SkyWalking 8.0+](https://skywalking.apache.org/downloads/#SkyWalkingAPM) and Python 3.7+.\n\n> If you would like to try out the latest features that are not released yet, please refer to this [guide](docs/en/setup/faq/How-to-build-from-sources.md) to build from sources.\n\n## Live Demo\n- Find the [live demo](https://skywalking.apache.org/#demo) with Python agent on our website.\n- Follow the [showcase](https://skywalking.apache.org/docs/skywalking-showcase/next/readme/) to set up preview deployment quickly.\n\n## Contributing\n\nBefore submitting a pull request or pushing a commit, please read our [contributing](CONTRIBUTING.md) and [developer guide](docs/en/contribution/Developer.md).\n\n## Contact Us\n* Mail list: **dev@skywalking.apache.org**. Mail to `dev-subscribe@skywalking.apache.org`, follow the reply to subscribe the mail list.\n* Send `Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.\n* Twitter, [ASFSkyWalking](https://twitter.com/AsfSkyWalking)\n* QQ Group: 901167865, 392443393\n* [bilibili B站 视频](https://space.bilibili.com/390683219)\n\n## License\nApache 2.0\n',
     'author': 'Apache Software Foundation',
     'author_email': 'dev@skywalking.apache.org',
     'maintainer': 'Apache SkyWalking Community',
     'maintainer_email': 'dev@skywalking.apache.org',
     'url': 'https://skywalking.apache.org/',
```

### Comparing `apache_skywalking_onepiece-1.1.1/PKG-INFO` & `apache_skywalking_onepiece-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-skywalking-onepiece
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects.
 Home-page: https://skywalking.apache.org/
 License: Apache-2.0
 Keywords: skywalking,tracing,metrics,logging,profiling,observability,distributed-tracing,apm,python
 Author: Apache Software Foundation
 Author-email: dev@skywalking.apache.org
 Maintainer: Apache SkyWalking Community
```

