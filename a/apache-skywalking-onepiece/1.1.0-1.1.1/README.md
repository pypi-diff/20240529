# Comparing `tmp/apache_skywalking_onepiece-1.1.0.tar.gz` & `tmp/apache_skywalking_onepiece-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_skywalking_onepiece-1.1.0.tar", max compression
+gzip compressed data, was "apache_skywalking_onepiece-1.1.1.tar", max compression
```

## Comparing `apache_skywalking_onepiece-1.1.0.tar` & `apache_skywalking_onepiece-1.1.1.tar`

### file list

```diff
@@ -1,122 +1,183 @@
--rw-r--r--   0        0        0    11357 2024-03-04 13:56:56.376612 apache_skywalking_onepiece-1.1.0/LICENSE
--rw-r--r--   0        0        0      171 2024-03-04 13:56:56.376777 apache_skywalking_onepiece-1.1.0/NOTICE
--rwxr-xr-x   0        0        0     3298 2024-03-04 13:56:56.376863 apache_skywalking_onepiece-1.1.0/README.md
--rw-r--r--   0        0        0     4511 2024-05-29 03:13:54.051605 apache_skywalking_onepiece-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2174 2024-03-04 13:56:56.383667 apache_skywalking_onepiece-1.1.0/skywalking/__init__.py
--rw-r--r--   0        0        0    30179 2024-03-04 13:56:56.383899 apache_skywalking_onepiece-1.1.0/skywalking/agent/__init__.py
--rw-r--r--   0        0        0     2439 2024-03-04 13:56:56.384035 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/__init__.py
--rw-r--r--   0        0        0    10337 2024-03-04 13:56:56.384172 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/grpc.py
--rw-r--r--   0        0        0     8978 2024-03-04 13:56:56.384318 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/grpc_aio.py
--rw-r--r--   0        0        0     4103 2024-03-04 13:56:56.384409 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/http.py
--rw-r--r--   0        0        0     3499 2024-03-04 13:56:56.384484 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/http_aio.py
--rw-r--r--   0        0        0     3186 2024-03-04 13:56:56.384558 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/interceptors.py
--rw-r--r--   0        0        0     3420 2024-03-04 13:56:56.384633 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/interceptors_aio.py
--rw-r--r--   0        0        0     7071 2024-03-04 13:56:56.384749 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/kafka.py
--rw-r--r--   0        0        0     6182 2024-03-04 13:56:56.384859 apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/kafka_aio.py
--rw-r--r--   0        0        0     1441 2024-03-04 13:56:56.385004 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/__init__.py
--rw-r--r--   0        0        0      895 2024-03-04 13:56:56.385123 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/__init__.py
--rw-r--r--   0        0        0     4119 2024-03-04 13:56:56.385235 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/sw_python.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.385347 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/utility/__init__.py
--rw-r--r--   0        0        0     6133 2024-03-04 13:56:56.385448 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/utility/runner.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.385552 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/hooks/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-04 13:56:56.385632 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/hooks/uwsgi_hook.py
--rw-r--r--   0        0        0     1002 2024-03-04 13:56:56.385750 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/loader/__init__.py
--rw-r--r--   0        0        0     9284 2024-03-04 13:56:56.385874 apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/loader/sitecustomize.py
--rw-r--r--   0        0        0     8300 2024-03-04 13:56:56.386008 apache_skywalking_onepiece-1.1.0/skywalking/client/__init__.py
--rw-r--r--   0        0        0     4522 2024-03-04 13:56:56.386111 apache_skywalking_onepiece-1.1.0/skywalking/client/grpc.py
--rw-r--r--   0        0        0     4859 2024-03-04 13:56:56.386201 apache_skywalking_onepiece-1.1.0/skywalking/client/grpc_aio.py
--rw-r--r--   0        0        0     5455 2024-03-04 13:56:56.386289 apache_skywalking_onepiece-1.1.0/skywalking/client/http.py
--rw-r--r--   0        0        0     6058 2024-03-04 13:56:56.386375 apache_skywalking_onepiece-1.1.0/skywalking/client/http_aio.py
--rw-r--r--   0        0        0     5168 2024-03-04 13:56:56.386477 apache_skywalking_onepiece-1.1.0/skywalking/client/kafka.py
--rw-r--r--   0        0        0     6944 2024-03-04 13:56:56.386574 apache_skywalking_onepiece-1.1.0/skywalking/client/kafka_aio.py
--rw-r--r--   0        0        0      951 2024-03-04 13:56:56.386693 apache_skywalking_onepiece-1.1.0/skywalking/command/__init__.py
--rw-r--r--   0        0        0     1008 2024-03-04 13:56:56.386770 apache_skywalking_onepiece-1.1.0/skywalking/command/base_command.py
--rw-r--r--   0        0        0     6220 2024-03-04 13:56:56.386861 apache_skywalking_onepiece-1.1.0/skywalking/command/command_service.py
--rw-r--r--   0        0        0      925 2024-03-04 13:56:56.386978 apache_skywalking_onepiece-1.1.0/skywalking/command/executors/__init__.py
--rw-r--r--   0        0        0      878 2024-03-04 13:56:56.387060 apache_skywalking_onepiece-1.1.0/skywalking/command/executors/command_executor.py
--rw-r--r--   0        0        0     1058 2024-03-04 13:56:56.387129 apache_skywalking_onepiece-1.1.0/skywalking/command/executors/noop_command_executor.py
--rw-r--r--   0        0        0     1783 2024-03-04 13:56:56.387199 apache_skywalking_onepiece-1.1.0/skywalking/command/executors/profile_task_command_executor.py
--rw-r--r--   0        0        0     3483 2024-03-04 13:56:56.387280 apache_skywalking_onepiece-1.1.0/skywalking/command/profile_task_command.py
--rw-r--r--   0        0        0    19852 2024-03-04 13:56:56.387516 apache_skywalking_onepiece-1.1.0/skywalking/config.py
--rw-r--r--   0        0        0     2922 2024-03-04 13:56:56.387591 apache_skywalking_onepiece-1.1.0/skywalking/decorators.py
--rw-r--r--   0        0        0     1206 2024-03-04 13:56:56.387716 apache_skywalking_onepiece-1.1.0/skywalking/log/__init__.py
--rw-r--r--   0        0        0     1736 2024-03-04 13:56:56.387792 apache_skywalking_onepiece-1.1.0/skywalking/log/formatter.py
--rw-r--r--   0        0        0     5107 2024-03-04 13:56:56.387883 apache_skywalking_onepiece-1.1.0/skywalking/log/sw_logging.py
--rw-r--r--   0        0        0     1462 2024-03-04 13:56:56.387957 apache_skywalking_onepiece-1.1.0/skywalking/loggings.py
--rw-r--r--   0        0        0     1547 2024-03-04 13:56:56.388057 apache_skywalking_onepiece-1.1.0/skywalking/meter/__init__.py
--rw-r--r--   0        0        0     3314 2024-03-04 13:56:56.388140 apache_skywalking_onepiece-1.1.0/skywalking/meter/counter.py
--rw-r--r--   0        0        0     1592 2024-03-04 13:56:56.388216 apache_skywalking_onepiece-1.1.0/skywalking/meter/gauge.py
--rw-r--r--   0        0        0     4111 2024-03-04 13:56:56.388307 apache_skywalking_onepiece-1.1.0/skywalking/meter/histogram.py
--rw-r--r--   0        0        0     3619 2024-03-04 13:56:56.388379 apache_skywalking_onepiece-1.1.0/skywalking/meter/meter.py
--rw-r--r--   0        0        0     3182 2024-03-04 13:56:56.388450 apache_skywalking_onepiece-1.1.0/skywalking/meter/meter_service.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.388544 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/__init__.py
--rw-r--r--   0        0        0     1194 2024-03-04 13:56:56.388620 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/cpu_usage.py
--rw-r--r--   0        0        0     1074 2024-03-04 13:56:56.388694 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/data_source.py
--rw-r--r--   0        0        0     1625 2024-03-04 13:56:56.388767 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/gc_data.py
--rw-r--r--   0        0        0     1241 2024-03-04 13:56:56.388831 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/mem_usage.py
--rw-r--r--   0        0        0     1273 2024-03-04 13:56:56.388893 apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/thread_data.py
--rw-r--r--   0        0        0     4727 2024-03-04 13:56:56.389020 apache_skywalking_onepiece-1.1.0/skywalking/plugins/__init__.py
--rw-r--r--   0        0        0     4418 2024-03-04 13:56:56.389106 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aiohttp.py
--rw-r--r--   0        0        0     2079 2024-03-04 13:56:56.389207 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aioredis.py
--rw-r--r--   0        0        0     3888 2024-03-04 13:56:56.389299 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aiormq.py
--rw-r--r--   0        0        0     3831 2024-03-04 13:56:56.389381 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_amqp.py
--rw-r--r--   0        0        0     4832 2024-03-04 13:56:56.389470 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_asyncpg.py
--rw-r--r--   0        0        0     3162 2024-03-04 13:56:56.389547 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_bottle.py
--rw-r--r--   0        0        0     4666 2024-03-04 13:56:56.389635 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_celery.py
--rw-r--r--   0        0        0     5229 2024-03-04 13:56:56.389719 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_confluent_kafka.py
--rw-r--r--   0        0        0     3784 2024-03-04 13:56:56.389788 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_django.py
--rw-r--r--   0        0        0     1986 2024-03-04 13:56:56.389876 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_elasticsearch.py
--rw-r--r--   0        0        0     3255 2024-03-04 13:56:56.389962 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_falcon.py
--rw-r--r--   0        0        0     4067 2024-03-04 13:56:56.390032 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_fastapi.py
--rw-r--r--   0        0        0     3593 2024-03-04 13:56:56.390127 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_flask.py
--rw-r--r--   0        0        0     4734 2024-03-04 13:56:56.390201 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_happybase.py
--rw-r--r--   0        0        0     5562 2024-03-04 13:56:56.390287 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_http_server.py
--rw-r--r--   0        0        0     3849 2024-03-04 13:56:56.390358 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_httpx.py
--rw-r--r--   0        0        0     4086 2024-03-04 13:56:56.390440 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_kafka.py
--rw-r--r--   0        0        0     4371 2024-03-04 13:56:56.390541 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_loguru.py
--rw-r--r--   0        0        0     3077 2024-03-04 13:56:56.390626 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_mysqlclient.py
--rw-r--r--   0        0        0     4202 2024-03-04 13:56:56.390719 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_neo4j.py
--rw-r--r--   0        0        0    10581 2024-03-04 13:56:56.390827 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_psycopg.py
--rw-r--r--   0        0        0     6447 2024-03-04 13:56:56.390909 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_psycopg2.py
--rw-r--r--   0        0        0     5706 2024-03-04 13:56:56.390992 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pymongo.py
--rw-r--r--   0        0        0     2142 2024-03-04 13:56:56.391080 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pymysql.py
--rw-r--r--   0        0        0     2269 2024-03-04 13:56:56.391153 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pyramid.py
--rw-r--r--   0        0        0     7145 2024-03-04 13:56:56.391232 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_rabbitmq.py
--rw-r--r--   0        0        0     3372 2024-03-04 13:56:56.391335 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_redis.py
--rw-r--r--   0        0        0     3095 2024-03-04 13:56:56.391420 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_requests.py
--rw-r--r--   0        0        0     4200 2024-03-04 13:56:56.391514 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_sanic.py
--rw-r--r--   0        0        0     4910 2024-03-04 13:56:56.391618 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_tornado.py
--rw-r--r--   0        0        0     2346 2024-03-04 13:56:56.391699 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_urllib3.py
--rw-r--r--   0        0        0     2717 2024-03-04 13:56:56.391787 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_urllib_request.py
--rw-r--r--   0        0        0     4021 2024-03-04 13:56:56.391856 apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_websockets.py
--rw-r--r--   0        0        0     1082 2024-03-04 13:56:56.391985 apache_skywalking_onepiece-1.1.0/skywalking/profile/__init__.py
--rw-r--r--   0        0        0     1183 2024-03-04 13:56:56.392073 apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_constants.py
--rw-r--r--   0        0        0    14529 2024-03-04 13:56:56.392187 apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_context.py
--rw-r--r--   0        0        0     9316 2024-03-04 13:56:56.392308 apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_service.py
--rw-r--r--   0        0        0     1539 2024-03-04 13:56:56.392384 apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_status.py
--rw-r--r--   0        0        0     1820 2024-03-04 13:56:56.392450 apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_task.py
--rw-r--r--   0        0        0     1610 2024-03-04 13:56:56.392529 apache_skywalking_onepiece-1.1.0/skywalking/profile/snapshot.py
--rw-r--r--   0        0        0     1053 2024-03-04 13:56:56.392650 apache_skywalking_onepiece-1.1.0/skywalking/trace/__init__.py
--rw-r--r--   0        0        0     4860 2024-03-04 13:56:56.392737 apache_skywalking_onepiece-1.1.0/skywalking/trace/carrier.py
--rw-r--r--   0        0        0    10652 2024-03-04 13:56:56.392850 apache_skywalking_onepiece-1.1.0/skywalking/trace/context.py
--rw-r--r--   0        0        0     3250 2024-03-04 13:56:56.392920 apache_skywalking_onepiece-1.1.0/skywalking/trace/segment.py
--rw-r--r--   0        0        0     1673 2024-03-04 13:56:56.393010 apache_skywalking_onepiece-1.1.0/skywalking/trace/snapshot.py
--rw-r--r--   0        0        0     6714 2024-03-04 13:56:56.393101 apache_skywalking_onepiece-1.1.0/skywalking/trace/span.py
--rw-r--r--   0        0        0     1935 2024-03-04 13:56:56.393189 apache_skywalking_onepiece-1.1.0/skywalking/trace/tags.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.393284 apache_skywalking_onepiece-1.1.0/skywalking/utils/__init__.py
--rw-r--r--   0        0        0     2179 2024-03-04 13:56:56.393350 apache_skywalking_onepiece-1.1.0/skywalking/utils/array.py
--rw-r--r--   0        0        0     1511 2024-03-04 13:56:56.393426 apache_skywalking_onepiece-1.1.0/skywalking/utils/atomic_ref.py
--rw-r--r--   0        0        0     1029 2024-03-04 13:56:56.393503 apache_skywalking_onepiece-1.1.0/skywalking/utils/comparator.py
--rw-r--r--   0        0        0     1213 2024-03-04 13:56:56.393572 apache_skywalking_onepiece-1.1.0/skywalking/utils/counter.py
--rw-r--r--   0        0        0     1016 2024-03-04 13:56:56.393656 apache_skywalking_onepiece-1.1.0/skywalking/utils/exception.py
--rw-r--r--   0        0        0     1627 2024-03-04 13:56:56.393725 apache_skywalking_onepiece-1.1.0/skywalking/utils/filter.py
--rw-r--r--   0        0        0     1220 2024-03-04 13:56:56.393789 apache_skywalking_onepiece-1.1.0/skywalking/utils/integer.py
--rw-r--r--   0        0        0     1187 2024-03-04 13:56:56.393865 apache_skywalking_onepiece-1.1.0/skywalking/utils/lang.py
--rw-r--r--   0        0        0     1370 2024-03-04 13:56:56.393942 apache_skywalking_onepiece-1.1.0/skywalking/utils/singleton.py
--rw-r--r--   0        0        0      863 2024-03-04 13:56:56.394010 apache_skywalking_onepiece-1.1.0/skywalking/utils/time.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.394098 apache_skywalking_onepiece-1.1.0/sw_python/__init__.py
--rw-r--r--   0        0        0      837 2024-03-04 13:56:56.394166 apache_skywalking_onepiece-1.1.0/sw_python/__main__.py
--rw-r--r--   0        0        0      785 2024-03-04 13:56:56.394258 apache_skywalking_onepiece-1.1.0/sw_python/src/__init__.py
--rw-r--r--   0        0        0     1019 2024-03-04 13:56:56.394331 apache_skywalking_onepiece-1.1.0/sw_python/src/sw_python.py
--rw-r--r--   0        0        0     5391 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.0/setup.py
--rw-r--r--   0        0        0     5462 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2023-04-25 16:02:57.380283 apache_skywalking_onepiece-1.1.1/LICENSE
+-rwxr-xr-x   0        0        0     3188 2023-04-25 16:02:57.386283 apache_skywalking_onepiece-1.1.1/README.md
+-rwxr-xr-x   0        0        0     4102 2024-05-29 06:43:27.994272 apache_skywalking_onepiece-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-29 06:36:24.055065 apache_skywalking_onepiece-1.1.1/skywalking/.DS_Store
+-rwxr-xr-x   0        0        0     2158 2023-04-25 16:02:57.620123 apache_skywalking_onepiece-1.1.1/skywalking/__init__.py
+-rwxr-xr-x   0        0        0    17297 2023-04-25 16:02:57.628116 apache_skywalking_onepiece-1.1.1/skywalking/agent/__init__.py
+-rwxr-xr-x   0        0        0     1629 2023-04-25 16:02:57.639114 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/__init__.py
+-rwxr-xr-x   0        0        0    10328 2023-04-25 16:02:57.646115 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/grpc.py
+-rwxr-xr-x   0        0        0     4103 2023-04-25 16:02:57.651123 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/http.py
+-rwxr-xr-x   0        0        0     3186 2023-04-25 16:02:57.658116 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/interceptors.py
+-rwxr-xr-x   0        0        0     7071 2023-04-25 16:02:57.663120 apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/kafka.py
+-rwxr-xr-x   0        0        0     1441 2023-04-25 16:02:57.671121 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/__init__.py
+-rwxr-xr-x   0        0        0      895 2023-04-25 16:02:57.681660 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/__init__.py
+-rwxr-xr-x   0        0        0     4119 2023-04-25 16:02:57.688661 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/sw_python.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.701659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/__init__.py
+-rwxr-xr-x   0        0        0     6133 2023-04-25 16:02:57.709659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/runner.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.720660 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/__init__.py
+-rwxr-xr-x   0        0        0     2558 2023-04-25 16:02:57.727659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/uwsgi_hook.py
+-rwxr-xr-x   0        0        0     1002 2023-04-25 16:02:57.738659 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/__init__.py
+-rwxr-xr-x   0        0        0     9252 2023-04-25 16:02:57.746653 apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/sitecustomize.py
+-rwxr-xr-x   0        0        0     4594 2023-04-25 16:02:57.754661 apache_skywalking_onepiece-1.1.1/skywalking/client/__init__.py
+-rwxr-xr-x   0        0        0     4522 2023-04-25 16:02:57.759675 apache_skywalking_onepiece-1.1.1/skywalking/client/grpc.py
+-rwxr-xr-x   0        0        0     5455 2023-04-25 16:02:57.764672 apache_skywalking_onepiece-1.1.1/skywalking/client/http.py
+-rwxr-xr-x   0        0        0     5168 2023-04-25 16:02:57.770667 apache_skywalking_onepiece-1.1.1/skywalking/client/kafka.py
+-rwxr-xr-x   0        0        0      884 2023-04-25 16:02:57.782210 apache_skywalking_onepiece-1.1.1/skywalking/command/__init__.py
+-rwxr-xr-x   0        0        0     1008 2023-04-25 16:02:57.791209 apache_skywalking_onepiece-1.1.1/skywalking/command/base_command.py
+-rwxr-xr-x   0        0        0     4436 2023-04-25 16:02:57.799205 apache_skywalking_onepiece-1.1.1/skywalking/command/command_service.py
+-rwxr-xr-x   0        0        0      925 2023-04-25 16:02:57.813213 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/__init__.py
+-rwxr-xr-x   0        0        0      878 2023-04-25 16:02:57.823215 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/command_executor.py
+-rwxr-xr-x   0        0        0     1058 2023-04-25 16:02:57.830204 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/noop_command_executor.py
+-rwxr-xr-x   0        0        0     1783 2023-04-25 16:02:57.838216 apache_skywalking_onepiece-1.1.1/skywalking/command/executors/profile_task_command_executor.py
+-rwxr-xr-x   0        0        0     3483 2023-04-25 16:02:57.845214 apache_skywalking_onepiece-1.1.1/skywalking/command/profile_task_command.py
+-rwxr-xr-x   0        0        0    19613 2023-04-25 16:02:57.851205 apache_skywalking_onepiece-1.1.1/skywalking/config.py
+-rwxr-xr-x   0        0        0     2922 2023-04-25 16:02:57.856206 apache_skywalking_onepiece-1.1.1/skywalking/decorators.py
+-rwxr-xr-x   0        0        0     1206 2023-04-25 16:02:57.865245 apache_skywalking_onepiece-1.1.1/skywalking/log/__init__.py
+-rwxr-xr-x   0        0        0     1736 2023-04-25 16:02:57.872235 apache_skywalking_onepiece-1.1.1/skywalking/log/formatter.py
+-rwxr-xr-x   0        0        0     4907 2024-05-29 06:38:52.521523 apache_skywalking_onepiece-1.1.1/skywalking/log/sw_logging.py
+-rwxr-xr-x   0        0        0     1462 2023-04-25 16:02:57.881760 apache_skywalking_onepiece-1.1.1/skywalking/loggings.py
+-rwxr-xr-x   0        0        0     1181 2023-04-25 16:02:57.891761 apache_skywalking_onepiece-1.1.1/skywalking/meter/__init__.py
+-rwxr-xr-x   0        0        0     3314 2023-04-25 16:02:57.898768 apache_skywalking_onepiece-1.1.1/skywalking/meter/counter.py
+-rwxr-xr-x   0        0        0     1592 2023-04-25 16:02:57.903771 apache_skywalking_onepiece-1.1.1/skywalking/meter/gauge.py
+-rwxr-xr-x   0        0        0     4111 2023-04-25 16:02:57.909769 apache_skywalking_onepiece-1.1.1/skywalking/meter/histogram.py
+-rwxr-xr-x   0        0        0     3619 2023-04-25 16:02:57.915760 apache_skywalking_onepiece-1.1.1/skywalking/meter/meter.py
+-rwxr-xr-x   0        0        0     2049 2023-04-25 16:02:57.921768 apache_skywalking_onepiece-1.1.1/skywalking/meter/meter_service.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:57.933768 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/__init__.py
+-rwxr-xr-x   0        0        0     1194 2023-04-25 16:02:57.943761 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/cpu_usage.py
+-rwxr-xr-x   0        0        0     1074 2023-04-25 16:02:57.950773 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/data_source.py
+-rwxr-xr-x   0        0        0     1625 2023-04-25 16:02:57.957768 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/gc_data.py
+-rwxr-xr-x   0        0        0     1241 2023-04-25 16:02:57.964790 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/mem_usage.py
+-rwxr-xr-x   0        0        0     1273 2023-04-25 16:02:57.971785 apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/thread_data.py
+-rwxr-xr-x   0        0        0     4351 2023-04-25 16:02:57.981939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/__init__.py
+-rwxr-xr-x   0        0        0     3965 2023-04-25 16:02:57.988935 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiohttp.py
+-rwxr-xr-x   0        0        0     2079 2023-04-25 16:02:57.994936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aioredis.py
+-rwxr-xr-x   0        0        0     3888 2023-04-25 16:02:58.000938 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiormq.py
+-rwxr-xr-x   0        0        0     3831 2023-04-25 16:02:58.005936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_amqp.py
+-rwxr-xr-x   0        0        0     4832 2023-04-25 16:02:58.011935 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_asyncpg.py
+-rwxr-xr-x   0        0        0     3162 2023-04-25 16:02:58.017939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_bottle.py
+-rwxr-xr-x   0        0        0     4666 2023-04-25 16:02:58.023936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_celery.py
+-rwxr-xr-x   0        0        0     5229 2023-04-25 16:02:58.028937 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_confluent_kafka.py
+-rwxr-xr-x   0        0        0     3784 2023-04-25 16:02:58.034936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_django.py
+-rwxr-xr-x   0        0        0     1986 2023-04-25 16:02:58.039928 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_elasticsearch.py
+-rwxr-xr-x   0        0        0     3255 2023-04-25 16:02:58.044936 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_falcon.py
+-rwxr-xr-x   0        0        0     4067 2023-04-25 16:02:58.051928 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_fastapi.py
+-rwxr-xr-x   0        0        0     3593 2023-04-25 16:02:58.056937 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_flask.py
+-rwxr-xr-x   0        0        0     4734 2023-04-25 16:02:58.062945 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_happybase.py
+-rwxr-xr-x   0        0        0     5562 2023-04-25 16:02:58.068939 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_http_server.py
+-rwxr-xr-x   0        0        0     3849 2023-04-25 16:02:58.074471 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_httpx.py
+-rwxr-xr-x   0        0        0     4086 2023-04-25 16:02:58.080478 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_kafka.py
+-rwxr-xr-x   0        0        0     4171 2023-04-25 16:02:58.085477 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_loguru.py
+-rwxr-xr-x   0        0        0     3077 2023-04-25 16:02:58.090485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_mysqlclient.py
+-rwxr-xr-x   0        0        0    10581 2023-04-25 16:02:58.096486 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg.py
+-rwxr-xr-x   0        0        0     6447 2023-04-25 16:02:58.102484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg2.py
+-rwxr-xr-x   0        0        0     5706 2023-04-25 16:02:58.107488 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymongo.py
+-rwxr-xr-x   0        0        0     2142 2023-04-25 16:02:58.113484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymysql.py
+-rwxr-xr-x   0        0        0     2269 2023-04-25 16:02:58.118479 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pyramid.py
+-rwxr-xr-x   0        0        0     7145 2023-04-25 16:02:58.124477 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_rabbitmq.py
+-rwxr-xr-x   0        0        0     3372 2023-04-25 16:02:58.129475 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_redis.py
+-rwxr-xr-x   0        0        0     3095 2023-04-25 16:02:58.134485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_requests.py
+-rwxr-xr-x   0        0        0     4200 2023-04-25 16:02:58.140488 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_sanic.py
+-rwxr-xr-x   0        0        0     4910 2023-04-25 16:02:58.147484 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_tornado.py
+-rwxr-xr-x   0        0        0     2346 2023-04-25 16:02:58.153487 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib3.py
+-rwxr-xr-x   0        0        0     2717 2023-04-25 16:02:58.158485 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib_request.py
+-rwxr-xr-x   0        0        0     4021 2023-04-25 16:02:58.163492 apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_websockets.py
+-rwxr-xr-x   0        0        0     1082 2023-04-25 16:02:58.172501 apache_skywalking_onepiece-1.1.1/skywalking/profile/__init__.py
+-rwxr-xr-x   0        0        0     1183 2023-04-25 16:02:58.179027 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_constants.py
+-rwxr-xr-x   0        0        0    14758 2023-04-25 16:02:58.185027 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_context.py
+-rwxr-xr-x   0        0        0     9316 2023-04-25 16:02:58.190026 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_service.py
+-rwxr-xr-x   0        0        0     1539 2023-04-25 16:02:58.195035 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_status.py
+-rwxr-xr-x   0        0        0     1820 2023-04-25 16:02:58.199036 apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_task.py
+-rwxr-xr-x   0        0        0     1610 2023-04-25 16:02:58.204034 apache_skywalking_onepiece-1.1.1/skywalking/profile/snapshot.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.165192 apache_skywalking_onepiece-1.1.1/skywalking/protocol/__init__.py
+-rwxr-xr-x   0        0        0     1832 2023-04-29 19:50:32.982585 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2.py
+-rwxr-xr-x   0        0        0      238 2023-04-29 19:50:32.543551 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     4248 2023-04-29 19:50:32.991585 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerfCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     3434 2023-04-29 19:50:32.999764 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.py
+-rwxr-xr-x   0        0        0     4060 2023-04-29 19:50:32.564635 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2.pyi
+-rwxr-xr-x   0        0        0     4318 2023-04-29 19:50:33.009694 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/BrowserPerf_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:32.976019 apache_skywalking_onepiece-1.1.1/skywalking/protocol/browser/__init__.py
+-rwxr-xr-x   0        0        0     1631 2023-04-29 19:50:33.024771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.py
+-rwxr-xr-x   0        0        0     1052 2023-04-29 19:50:32.585752 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2.pyi
+-rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.032771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Command_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1988 2023-04-29 19:50:33.047772 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.py
+-rwxr-xr-x   0        0        0     1463 2023-04-29 19:50:32.610341 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2.pyi
+-rwxr-xr-x   0        0        0      159 2023-04-29 19:50:33.058771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/Common_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.016771 apache_skywalking_onepiece-1.1.1/skywalking/protocol/common/__init__.py
+-rwxr-xr-x   0        0        0     2592 2023-04-29 19:50:33.073954 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.py
+-rwxr-xr-x   0        0        0     2298 2023-04-29 19:50:32.632968 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2.pyi
+-rwxr-xr-x   0        0        0     2916 2023-04-29 19:50:33.082968 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/Event_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.066772 apache_skywalking_onepiece-1.1.1/skywalking/protocol/event/__init__.py
+-rwxr-xr-x   0        0        0     1743 2023-04-29 19:50:33.096049 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2.py
+-rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.652977 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2659 2023-04-29 19:50:33.105289 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetricCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:33.114301 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.py
+-rwxr-xr-x   0        0        0     2820 2023-04-29 19:50:32.672480 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2.pyi
+-rwxr-xr-x   0        0        0     2701 2023-04-29 19:50:33.122302 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/CLRMetric_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1881 2023-04-29 19:50:33.133291 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.py
+-rwxr-xr-x   0        0        0      545 2023-04-29 19:50:32.692232 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2.pyi
+-rwxr-xr-x   0        0        0     3563 2023-04-29 19:50:33.142286 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/ConfigurationDiscoveryService_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1740 2023-04-29 19:50:33.151864 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2.py
+-rwxr-xr-x   0        0        0      241 2023-04-29 19:50:32.712371 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2620 2023-04-29 19:50:33.162209 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetricCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     4336 2023-04-29 19:50:33.171210 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.py
+-rwxr-xr-x   0        0        0     5568 2023-04-29 19:50:32.742081 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2.pyi
+-rwxr-xr-x   0        0        0     2662 2023-04-29 19:50:33.181212 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/JVMMetric_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1701 2023-04-29 19:50:33.191024 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2.py
+-rwxr-xr-x   0        0        0      233 2023-04-29 19:50:32.762005 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     2692 2023-04-29 19:50:33.200273 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/MeterCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     3036 2023-04-29 19:50:33.210276 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.py
+-rwxr-xr-x   0        0        0     3101 2023-04-29 19:50:32.780009 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2.pyi
+-rwxr-xr-x   0        0        0     4696 2023-04-29 19:50:33.220471 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Meter_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1845 2023-04-29 19:50:33.232472 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2.py
+-rwxr-xr-x   0        0        0      237 2023-04-29 19:50:32.799943 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     5037 2023-04-29 19:50:33.243973 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/TracingCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     5861 2023-04-29 19:50:33.251964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.py
+-rwxr-xr-x   0        0        0     7713 2023-04-29 19:50:32.819120 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2.pyi
+-rwxr-xr-x   0        0        0     8576 2023-04-29 19:50:33.262964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/Tracing_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.090548 apache_skywalking_onepiece-1.1.1/skywalking/protocol/language_agent/__init__.py
+-rwxr-xr-x   0        0        0     3150 2023-04-29 19:50:33.276964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.py
+-rwxr-xr-x   0        0        0     3202 2023-04-29 19:50:32.841120 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2.pyi
+-rwxr-xr-x   0        0        0     2769 2023-04-29 19:50:33.285980 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/Logging_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.269964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/logging/__init__.py
+-rwxr-xr-x   0        0        0     1805 2023-04-29 19:50:33.300596 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2.py
+-rwxr-xr-x   0        0        0      239 2023-04-29 19:50:32.869202 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     4469 2023-04-29 19:50:33.310752 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/ManagementCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2260 2023-04-29 19:50:33.319756 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.py
+-rwxr-xr-x   0        0        0     1503 2023-04-29 19:50:32.891552 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2.pyi
+-rwxr-xr-x   0        0        0     4539 2023-04-29 19:50:33.327952 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/Management_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.294980 apache_skywalking_onepiece-1.1.1/skywalking/protocol/management/__init__.py
+-rwxr-xr-x   0        0        0     1900 2023-04-29 19:50:33.340963 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2.py
+-rwxr-xr-x   0        0        0      230 2023-04-29 19:50:32.912940 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2.pyi
+-rwxr-xr-x   0        0        0     5824 2023-04-29 19:50:33.350571 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/ProfileCompat_pb2_grpc.py
+-rwxr-xr-x   0        0        0     2725 2023-04-29 19:50:33.358571 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.py
+-rwxr-xr-x   0        0        0     2183 2023-04-29 19:50:32.930949 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2.pyi
+-rwxr-xr-x   0        0        0     5922 2023-04-29 19:50:33.369147 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/Profile_pb2_grpc.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.335964 apache_skywalking_onepiece-1.1.1/skywalking/protocol/profile/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-04-29 19:50:33.377153 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/__init__.py
+-rwxr-xr-x   0        0        0     4632 2023-04-29 19:50:33.385164 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.py
+-rwxr-xr-x   0        0        0     6980 2023-04-29 19:50:32.954545 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2.pyi
+-rwxr-xr-x   0        0        0     3043 2023-04-29 19:50:33.395161 apache_skywalking_onepiece-1.1.1/skywalking/protocol/service_mesh_probe/service_mesh_pb2_grpc.py
+-rwxr-xr-x   0        0        0     1053 2023-04-25 16:02:58.211034 apache_skywalking_onepiece-1.1.1/skywalking/trace/__init__.py
+-rwxr-xr-x   0        0        0     4860 2023-04-25 16:02:58.217035 apache_skywalking_onepiece-1.1.1/skywalking/trace/carrier.py
+-rwxr-xr-x   0        0        0    10585 2023-04-25 16:02:58.221050 apache_skywalking_onepiece-1.1.1/skywalking/trace/context.py
+-rwxr-xr-x   0        0        0     3250 2023-04-25 16:02:58.226034 apache_skywalking_onepiece-1.1.1/skywalking/trace/segment.py
+-rwxr-xr-x   0        0        0     1673 2023-04-25 16:02:58.230027 apache_skywalking_onepiece-1.1.1/skywalking/trace/snapshot.py
+-rwxr-xr-x   0        0        0     6714 2023-04-25 16:02:58.235027 apache_skywalking_onepiece-1.1.1/skywalking/trace/span.py
+-rwxr-xr-x   0        0        0     1935 2023-04-25 16:02:58.239037 apache_skywalking_onepiece-1.1.1/skywalking/trace/tags.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.247035 apache_skywalking_onepiece-1.1.1/skywalking/utils/__init__.py
+-rwxr-xr-x   0        0        0     2179 2023-04-25 16:02:58.253027 apache_skywalking_onepiece-1.1.1/skywalking/utils/array.py
+-rwxr-xr-x   0        0        0     1511 2023-04-25 16:02:58.257035 apache_skywalking_onepiece-1.1.1/skywalking/utils/atomic_ref.py
+-rwxr-xr-x   0        0        0     1029 2023-04-25 16:02:58.263043 apache_skywalking_onepiece-1.1.1/skywalking/utils/comparator.py
+-rwxr-xr-x   0        0        0     1213 2023-04-25 16:02:58.268052 apache_skywalking_onepiece-1.1.1/skywalking/utils/counter.py
+-rwxr-xr-x   0        0        0     1016 2023-04-25 16:02:58.273043 apache_skywalking_onepiece-1.1.1/skywalking/utils/exception.py
+-rwxr-xr-x   0        0        0     1627 2023-04-25 16:02:58.277588 apache_skywalking_onepiece-1.1.1/skywalking/utils/filter.py
+-rwxr-xr-x   0        0        0     1220 2023-04-25 16:02:58.281579 apache_skywalking_onepiece-1.1.1/skywalking/utils/integer.py
+-rwxr-xr-x   0        0        0     1187 2023-04-25 16:02:58.285587 apache_skywalking_onepiece-1.1.1/skywalking/utils/lang.py
+-rwxr-xr-x   0        0        0     1370 2023-04-25 16:02:58.289586 apache_skywalking_onepiece-1.1.1/skywalking/utils/singleton.py
+-rwxr-xr-x   0        0        0      863 2023-04-25 16:02:58.294587 apache_skywalking_onepiece-1.1.1/skywalking/utils/time.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.299578 apache_skywalking_onepiece-1.1.1/sw_python/__init__.py
+-rwxr-xr-x   0        0        0      837 2023-04-25 16:02:58.304586 apache_skywalking_onepiece-1.1.1/sw_python/__main__.py
+-rwxr-xr-x   0        0        0      785 2023-04-25 16:02:58.313580 apache_skywalking_onepiece-1.1.1/sw_python/src/__init__.py
+-rwxr-xr-x   0        0        0     1019 2023-04-25 16:02:58.319587 apache_skywalking_onepiece-1.1.1/sw_python/src/sw_python.py
+-rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.1/setup.py
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 apache_skywalking_onepiece-1.1.1/PKG-INFO
```

### Comparing `apache_skywalking_onepiece-1.1.0/LICENSE` & `apache_skywalking_onepiece-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/README.md` & `apache_skywalking_onepiece-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 
 Before submitting a pull request or pushing a commit, please read our [contributing](CONTRIBUTING.md) and [developer guide](docs/en/contribution/Developer.md).
 
 ## Contact Us
 * Mail list: **dev@skywalking.apache.org**. Mail to `dev-subscribe@skywalking.apache.org`, follow the reply to subscribe the mail list.
 * Send `Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.
 * Twitter, [ASFSkyWalking](https://twitter.com/AsfSkyWalking)
-* For Chinese speaker, send `[CN] Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.
+* QQ Group: 901167865, 392443393
 * [bilibili B站 视频](https://space.bilibili.com/390683219)
 
 ## License
 Apache 2.0
```

### Comparing `apache_skywalking_onepiece-1.1.0/pyproject.toml` & `apache_skywalking_onepiece-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "apache-skywalking-onepiece"
-version = "1.1.0"
+version = "1.1.1"
 description = "The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects."
 license = "Apache-2.0"
 authors = ["Apache Software Foundation <dev@skywalking.apache.org>"]
 maintainers = ["Apache SkyWalking Community <dev@skywalking.apache.org>"]
 readme = "README.md"
 homepage = "https://skywalking.apache.org/"
 repository = "https://github.com/apache/skywalking-python"
@@ -45,15 +45,15 @@
 
     'Topic :: System :: Monitoring',
     'Topic :: Software Development',
 ]
 
 packages = [
     { include = "skywalking" },
-    { include = "sw_python" },
+    { include = "sw_python" }
 ]
 
 # poetry will ignore generated files as .gitignore, but we need them in package
 include = ['skywalking/protocol/**/*']
 exclude = ['tests']
 
 [tool.poetry.build]
@@ -68,52 +68,29 @@
 
 [tool.poetry.dependencies]
 python = ">=3.7, <3.12"
 grpcio = '*'
 grpcio-tools = '*'
 packaging = '*'
 wrapt = '*'
-psutil = '<=5.9.5'
+psutil = '*'
 requests = { version = ">=2.26.0", optional = true }
 kafka-python = { version = "*", optional = true }
-uvloop = { version = "^0.17.0", optional = true }
-aiokafka = { version = "^0.8.0", optional = true }
-aiohttp = { version = "^3.7.4", optional = true }
 
 [tool.poetry.extras]
 all=[
     'requests',
     'kafka-python',
-    'uvloop',
-    'aiokafka',
-    'aiohttp',
-]
-sync=[
-    'requests',
-    'kafka-python',
 ]
 http= [
     'requests',
 ]
 kafka=[
     'kafka-python',
 ]
-async=[
-    'uvloop',
-    'aiokafka',
-    'aiohttp',
-]
-asynchttp=[
-    'uvloop',
-    'aiohttp',
-]
-asynckafka=[
-    'uvloop',
-    'aiokafka',
-]
 
 [tool.poetry.group.dev.dependencies]
 pkginfo = "^1.8.3"
 testcontainers = "*"
 pyyaml = "*"
 pytest = "*"
 uwsgi = "*"
@@ -125,15 +102,15 @@
 [tool.poetry.group.plugins.dependencies]
 urllib3 = "1.26.7"
 aiohttp = "3.7.4"
 celery = "5.1.2"
 django = "3.2.8"
 elasticsearch = "7.15.1"
 flask = "2.0.2"
-gevent = "22.10.2"
+gevent = "22.8.0"
 hug = "2.6.1"
 pika = "1.2.0"
 psycopg = {extras = ["binary"], version = "^3.1.7"}
 psycopg2-binary = "^2.9"
 pymongo = "3.12.0"
 pymysql = "1.0.2"
 mysqlclient = "^2.1.1"
@@ -151,15 +128,14 @@
 aiormq = "^6.4.2"
 asyncpg = "^0.27.0"
 happybase = "1.2.0"
 websockets = "^10.4"
 loguru = "^0.6.0"
 httpx = "^0.23.3"
 confluent-kafka = "^2.0.2"
-neo4j = "^5.9.0"
 
 [tool.poetry.group.lint.dependencies]
 pylint = '2.13.9'
 flake8 = "^5.0.4"
 # isort = "^5.10.1"
 unify = "^0.5"
 flynt = "^0.76"
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     PostgreSQL = 22
     KafkaProducer = 40
     KafkaConsumer = 41
     RabbitmqProducer = 52
     RabbitmqConsumer = 53
     Elasticsearch = 47
     HBase = 94
-    Neo4j = 112
     Urllib3 = 7006
     Sanic = 7007
     AioHttp = 7008
     Pyramid = 7009
     Psycopg = 7010
     Celery = 7011
     Falcon = 7012
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/agent/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/agent/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,39 +15,34 @@
 # limitations under the License.
 #
 
 import atexit
 import functools
 import os
 import sys
-import asyncio
 from queue import Queue, Full
 from threading import Thread, Event
 from typing import TYPE_CHECKING, Optional
 
 from skywalking import config, plugins
 from skywalking import loggings
 from skywalking import meter
 from skywalking import profile
-from skywalking.agent.protocol import Protocol, ProtocolAsync
-from skywalking.command import command_service, command_service_async
+from skywalking.agent.protocol import Protocol
+from skywalking.command import command_service
 from skywalking.loggings import logger
 from skywalking.profile.profile_task import ProfileTask
 from skywalking.profile.snapshot import TracingThreadSnapshot
 from skywalking.protocol.language_agent.Meter_pb2 import MeterData
 from skywalking.protocol.logging.Logging_pb2 import LogData
 from skywalking.utils.singleton import Singleton
 
 if TYPE_CHECKING:
     from skywalking.trace.context import Segment
 
-if config.agent_asyncio_enhancement:
-    import uvloop
-    uvloop.install()
-
 
 def report_with_backoff(reporter_name, init_wait):
     """
     An exponential backoff for retrying reporters.
     """
 
     def backoff_decorator(func):
@@ -68,41 +63,14 @@
             logger.info('finished reporter thread')
 
         return backoff_wrapper
 
     return backoff_decorator
 
 
-def report_with_backoff_async(reporter_name, init_wait):
-    """
-    An exponential async backoff for retrying reporters.
-    """
-
-    def backoff_decorator(func):
-        @functools.wraps(func)
-        async def backoff_wrapper(self, *args, **kwargs):
-            wait = base = init_wait
-            while not self._finished.is_set():
-                try:
-                    flag = await func(self, *args, **kwargs)
-                    # for segment/log reporter, if the queue not empty(return True), we should keep reporter working
-                    # for other cases(return false or None), reset to base wait time on success
-                    wait = 0 if flag else base
-                except Exception:  # noqa
-                    wait = min(60, wait * 2 or 1)  # double wait time with each consecutive error up to a maximum
-                    logger.exception(f'Exception in {reporter_name} service in pid {os.getpid()}, '
-                                     f'retry in {wait} seconds')
-                await asyncio.sleep(wait)
-            logger.info('finished reporter coroutine')
-
-        return backoff_wrapper
-
-    return backoff_decorator
-
-
 class SkyWalkingAgent(Singleton):
     """
     The main singleton class and entrypoint of SkyWalking Python Agent.
     Upon fork(), original instance rebuild everything (queues, threads, instrumentation) by
     calling the fork handlers in the class instance.
     """
     __started: bool = False  # shared by all instances
@@ -261,17 +229,18 @@
             os.environ['GRPC_POLL_STRATEGY'] = 'poll'
 
         if not self.__started:
             # if not already started, start the agent
             config.finalize()  # Must be finalized exactly once
 
             self.__started = True
-            logger.info(f'SkyWalking sync agent instance {config.agent_instance_name} starting in pid-{os.getpid()}.')
+            logger.info(f'SkyWalking agent instance {config.agent_instance_name} starting in pid-{os.getpid()}.')
 
             # Install log reporter core
+            # TODO - Add support for printing traceID/ context in logs
             if config.agent_log_reporter_active:
                 from skywalking import log
                 log.install()
             # Here we install all other lib plugins on first time start (parent process)
             plugins.install()
         elif self.__started and os.getpid() == self.started_pid:
             # if already started, and this is the same process, raise an error
@@ -409,274 +378,11 @@
     def notify_profile_finish(self, task: ProfileTask):
         try:
             self.__protocol.notify_profile_task_finish(task)
         except Exception as e:
             logger.error(f'notify profile task finish to backend fail. {str(e)}')
 
 
-class SkyWalkingAgentAsync(Singleton):
-    __started: bool = False  # shared by all instances
-
-    def __init__(self):
-        """
-        ProtocolAsync is one of gRPC, HTTP and Kafka that
-        provides async clients to reporters to communicate with OAP backend.
-        """
-        self.started_pid = None
-        self.__protocol: Optional[ProtocolAsync] = None
-        self._finished: Optional[asyncio.Event] = None
-        # Initialize asyncio queues for segment, log, meter and profiling snapshots
-        self.__segment_queue: Optional[asyncio.Queue] = None
-        self.__log_queue: Optional[asyncio.Queue] = None
-        self.__meter_queue: Optional[asyncio.Queue] = None
-        self.__snapshot_queue: Optional[asyncio.Queue] = None
-
-        self.event_loop_thread: Optional[Thread] = None
-
-    def __bootstrap(self):
-        if config.agent_protocol == 'grpc':
-            from skywalking.agent.protocol.grpc_aio import GrpcProtocolAsync
-            self.__protocol = GrpcProtocolAsync()
-        elif config.agent_protocol == 'http':
-            from skywalking.agent.protocol.http_aio import HttpProtocolAsync
-            self.__protocol = HttpProtocolAsync()
-        elif config.agent_protocol == 'kafka':
-            from skywalking.agent.protocol.kafka_aio import KafkaProtocolAsync
-            self.__protocol = KafkaProtocolAsync()
-        else:
-            raise ValueError(f'Unsupported protocol: {config.agent_protocol}')
-        logger.info(f'You are using {config.agent_protocol} protocol to communicate with OAP backend')
-
-        # Start reporter's asyncio coroutines and register queues
-        self.__init_coroutine()
-
-    def __init_coroutine(self) -> None:
-        """
-        This method initializes all asyncio coroutines for the agent and reporters.
-
-        Heartbeat task is started by default.
-        Segment reporter task and segment queue is created by default.
-        All other queues and tasks depends on user configuration.
-        """
-
-        self.background_coroutines = set()
-
-        self.background_coroutines.add(self.__heartbeat())
-        self.background_coroutines.add(self.__report_segment())
-
-        if config.agent_meter_reporter_active:
-            self.background_coroutines.add(self.__report_meter())
-
-            if config.agent_pvm_meter_reporter_active:
-                from skywalking.meter.pvm.cpu_usage import CPUUsageDataSource
-                from skywalking.meter.pvm.gc_data import GCDataSource
-                from skywalking.meter.pvm.mem_usage import MEMUsageDataSource
-                from skywalking.meter.pvm.thread_data import ThreadDataSource
-
-                MEMUsageDataSource().register()
-                CPUUsageDataSource().register()
-                GCDataSource().register()
-                ThreadDataSource().register()
-
-        if config.agent_log_reporter_active:
-            self.background_coroutines.add(self.__report_log())
-
-        if config.agent_profile_active:
-            self.background_coroutines.add(self.__command_dispatch())
-            self.background_coroutines.add(self.__query_profile_command())
-            self.background_coroutines.add(self.__send_profile_snapshot())
-
-    async def __start_event_loop_async(self) -> None:
-        self.loop = asyncio.get_running_loop()  # always get the current running loop first
-        # asyncio Queue should be created after the creation of event loop
-        self.__segment_queue = asyncio.Queue(maxsize=config.agent_trace_reporter_max_buffer_size)
-        if config.agent_meter_reporter_active:
-            self.__meter_queue = asyncio.Queue(maxsize=config.agent_meter_reporter_max_buffer_size)
-        if config.agent_log_reporter_active:
-            self.__log_queue = asyncio.Queue(maxsize=config.agent_log_reporter_max_buffer_size)
-        if config.agent_profile_active:
-            self.__snapshot_queue = asyncio.Queue(maxsize=config.agent_profile_snapshot_transport_buffer_size)
-        # initialize background coroutines
-        self.background_coroutines = set()
-        self.background_tasks = set()
-        self._finished = asyncio.Event()
-
-        # Install log reporter core
-        if config.agent_log_reporter_active:
-            from skywalking import log
-            log.install()
-        if config.agent_meter_reporter_active:
-            # meter.init(force=True)
-            await meter.init_async()
-
-        self.__bootstrap()  # gather all coroutines
-
-        logger.debug('All background coroutines started')
-        await asyncio.gather(*self.background_coroutines)
-
-    def __start_event_loop(self) -> None:
-        try:
-            asyncio.run(self.__start_event_loop_async())
-        except asyncio.CancelledError:
-            logger.info('Python agent asyncio event loop is closed')
-        except Exception as e:
-            logger.error(f'Error in Python agent asyncio event loop: {e}')
-        finally:
-            if self._finished is not None:
-                self._finished.set()
-
-    def start(self) -> None:
-        loggings.init()
-
-        if sys.version_info < (3, 7):
-            # agent may or may not work for Python 3.6 and below
-            # since 3.6 is EOL, we will not officially support it
-            logger.warning('SkyWalking Python agent does not support Python 3.6 and below, '
-                           'please upgrade to Python 3.7 or above.')
-
-        if not self.__started:
-            # if not already started, start the agent
-            config.finalize()  # Must be finalized exactly once
-
-            self.__started = True
-            logger.info(f'SkyWalking async agent instance {config.agent_instance_name} starting in pid-{os.getpid()}.')
-
-            # Here we install all other lib plugins on first time start (parent process)
-            plugins.install()
-
-        elif self.__started and os.getpid() == self.started_pid:
-            # if already started, and this is the same process, raise an error
-            raise RuntimeError('SkyWalking Python agent has already been started in this process, '
-                               'did you call start more than once in your code + sw-python CLI? '
-                               'If you already use sw-python CLI, you should remove the manual start(), vice versa.')
-
-        self.started_pid = os.getpid()
-        atexit.register(self.__fini)
-
-        # still init profile here, since it is using threading rather than asyncio
-        if config.agent_profile_active:
-            profile.init()
-
-        self.event_loop_thread = Thread(name='event_loop_thread', target=self.__start_event_loop, daemon=True)
-        self.event_loop_thread.start()
-
-    async def __fini_async(self):
-        """
-        This method is called when the agent is shutting down.
-        Clean up all the queues and stop all the asyncio tasks.
-        """
-        if self._finished is not None:
-            self._finished.set()
-        queue_join_coroutine_list = [self.__segment_queue.join()]
-
-        if config.agent_log_reporter_active:
-            queue_join_coroutine_list.append(self.__log_queue.join())
-
-        if config.agent_profile_active:
-            queue_join_coroutine_list.append(self.__snapshot_queue.join())
-
-        if config.agent_meter_reporter_active:
-            queue_join_coroutine_list.append(self.__meter_queue.join())
-
-        await asyncio.gather(*queue_join_coroutine_list, return_exceptions=True)    # clean queues
-        # cancel all tasks
-        all_tasks = asyncio.all_tasks(self.loop)
-        for task in all_tasks:
-            task.cancel()
-
-    def __fini(self):
-        if not self.loop.is_closed():
-            asyncio.run_coroutine_threadsafe(self.__fini_async(), self.loop)
-        self.event_loop_thread.join()
-        logger.info('Finished Python agent event_loop thread')
-        # TODO: Unhandled error in sys.excepthook https://github.com/pytest-dev/execnet/issues/30
-
-    def stop(self) -> None:
-        """
-        Stops the agent and reset the started flag.
-        """
-        atexit.unregister(self.__fini)
-        self.__fini()
-        self.__started = False
-
-    @report_with_backoff_async(reporter_name='heartbeat', init_wait=config.agent_collector_heartbeat_period)
-    async def __heartbeat(self) -> None:
-        await self.__protocol.heartbeat()
-
-    @report_with_backoff_async(reporter_name='segment', init_wait=0.02)
-    async def __report_segment(self) -> bool:
-        """Returns True if the queue is not empty"""
-        queue_not_empty_flag = not self.__segment_queue.empty()
-        if queue_not_empty_flag:
-            await self.__protocol.report_segment(self.__segment_queue)
-        return queue_not_empty_flag
-
-    @report_with_backoff_async(reporter_name='log', init_wait=0.02)
-    async def __report_log(self) -> bool:
-        """Returns True if the queue is not empty"""
-        queue_not_empty_flag = not self.__log_queue.empty()
-        if queue_not_empty_flag:
-            await self.__protocol.report_log(self.__log_queue)
-        return queue_not_empty_flag
-
-    @report_with_backoff_async(reporter_name='meter', init_wait=config.agent_meter_reporter_period)
-    async def __report_meter(self) -> None:
-        if not self.__meter_queue.empty():
-            await self.__protocol.report_meter(self.__meter_queue)
-
-    @report_with_backoff_async(reporter_name='profile_snapshot', init_wait=0.5)
-    async def __send_profile_snapshot(self) -> None:
-        if not self.__snapshot_queue.empty():
-            await self.__protocol.report_snapshot(self.__snapshot_queue)
-
-    @report_with_backoff_async(
-        reporter_name='query_profile_command',
-        init_wait=config.agent_collector_get_profile_task_interval)
-    async def __query_profile_command(self) -> None:
-        await self.__protocol.query_profile_commands()
-
-    @staticmethod
-    async def __command_dispatch() -> None:
-        # command dispatch will stuck when there are no commands
-        await command_service_async.dispatch()
-
-    def __asyncio_queue_put_nowait(self, q: asyncio.Queue, queue_name: str, item):
-        try:
-            q.put_nowait(item)
-        except asyncio.QueueFull:
-            logger.warning(f'the {queue_name} queue is full, the item will be abandoned')
-
-    def is_segment_queue_full(self):
-        return self.__segment_queue.full()
-
-    def archive_segment(self, segment: 'Segment'):
-        if not self.loop.is_closed():
-            self.loop.call_soon_threadsafe(self.__asyncio_queue_put_nowait, self.__segment_queue, 'segment', segment)
-
-    def archive_log(self, log_data: 'LogData'):
-        if not self.loop.is_closed():
-            self.loop.call_soon_threadsafe(self.__asyncio_queue_put_nowait, self.__log_queue, 'log', log_data)
-
-    def archive_meter(self, meter_data: 'MeterData'):
-        if not self.loop.is_closed():
-            self.loop.call_soon_threadsafe(self.__asyncio_queue_put_nowait, self.__meter_queue, 'meter', meter_data)
-
-    async def archive_meter_async(self, meter_data: 'MeterData'):
-        try:
-            self.__meter_queue.put_nowait(meter_data)
-        except asyncio.QueueFull:
-            logger.warning('the meter queue is full, the item will be abandoned')
-
-    def add_profiling_snapshot(self, snapshot: TracingThreadSnapshot):
-        self.loop.call_soon_threadsafe(self.__asyncio_queue_put_nowait, self.__snapshot_queue, 'snapshot', snapshot)
-
-    def notify_profile_finish(self, task: ProfileTask):
-        try:
-            asyncio.run_coroutine_threadsafe(self.__protocol.notify_profile_task_finish(task), self.loop)
-        except Exception as e:
-            logger.error(f'notify profile task finish to backend fail. {e}')
-
-
 # Export for user (backwards compatibility)
 # so users still use `from skywalking import agent`
-agent = SkyWalkingAgentAsync() if config.agent_asyncio_enhancement else SkyWalkingAgent()
+agent = SkyWalkingAgent()
 start = agent.start
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/grpc.py` & `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import traceback
 from queue import Queue, Empty
 from time import time
 
 import grpc
 
 from skywalking import config
-from skywalking.agent.protocol import Protocol
+from skywalking.agent import Protocol
 from skywalking.agent.protocol.interceptors import header_adder_interceptor
 from skywalking.client.grpc import GrpcServiceManagementClient, GrpcTraceSegmentReportService, \
     GrpcProfileTaskChannelService, GrpcLogDataReportService, GrpcMeterReportService
 from skywalking.loggings import logger, logger_debug_enabled
 from skywalking.profile.profile_task import ProfileTask
 from skywalking.profile.snapshot import TracingThreadSnapshot
 from skywalking.protocol.common.Common_pb2 import KeyStringValuePair
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/http.py` & `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/http.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/interceptors.py` & `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/interceptors.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/agent/protocol/kafka.py` & `apache_skywalking_onepiece-1.1.1/skywalking/agent/protocol/kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/sw_python.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/sw_python.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/utility/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/cli/utility/runner.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/cli/utility/runner.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/hooks/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/hooks/uwsgi_hook.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/hooks/uwsgi_hook.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/loader/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/bootstrap/loader/sitecustomize.py` & `apache_skywalking_onepiece-1.1.1/skywalking/bootstrap/loader/sitecustomize.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,15 @@
                             'application are using the same Python executable. '
                             'Rerun with debug flag, `sw-python -d run <your_python_command>` for '
                             'some troubleshooting information.'
                             'use `which sw-python` to find out the invoked CLI location')
     os._exit(1)  # noqa: do not go further
 
 else:
-    from skywalking import config
-    from skywalking.agent import agent
+    from skywalking import agent, config
 
     _sw_loader_logger.info(f'Process-{os.getpid()}, running sitecustomize.py from {__file__}')
     # also override debug for skywalking agent itself
     if os.environ.get('SW_AGENT_SW_PYTHON_CLI_DEBUG_ENABLED') == 'True':  # set from the original CLI runner
         config.agent_logging_level = 'DEBUG'
 
     # Currently supports configs read from os.environ
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/client/grpc.py` & `apache_skywalking_onepiece-1.1.1/skywalking/client/grpc.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/client/http.py` & `apache_skywalking_onepiece-1.1.1/skywalking/client/http.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/client/kafka.py` & `apache_skywalking_onepiece-1.1.1/skywalking/client/kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,11 +11,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from skywalking.command.command_service import CommandService, CommandServiceAsync
+from skywalking.command.command_service import CommandService
 
 command_service = CommandService()
-command_service_async = CommandServiceAsync()
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/base_command.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/base_command.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/command_service.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/command_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import queue
-from asyncio import Queue as AsyncQueue, QueueFull as AsyncQueueFull
 from collections import deque
 
 from skywalking.protocol.common.Command_pb2 import Commands, Command
 
 from skywalking.command.base_command import BaseCommand
 from skywalking.command.executors import noop_command_executor_instance
 from skywalking.command.executors.profile_task_command_executor import ProfileTaskCommandExecutor
@@ -61,53 +60,14 @@
                 except queue.Full:
                     logger.warning('command[{%s}, {%s}] cannot add to command list. because the command list is full.',
                                    base_command.command, base_command.serial_number)
             except UnsupportedCommandException as e:
                 logger.warning('received unsupported command[{%s}].', e.command.command)
 
 
-class CommandServiceAsync:
-
-    def __init__(self):
-        self._commands = AsyncQueue()  # type: AsyncQueue
-        # don't execute same command twice
-        self._command_serial_number_cache = CommandSerialNumberCache()
-
-    async def dispatch(self):
-        while True:
-            # block until a command is available
-            command = await self._commands.get()  # type: BaseCommand
-            if not self.__is_command_executed(command):
-                command_executor_service.execute(command)
-                self._command_serial_number_cache.add(command.serial_number)
-
-    def __is_command_executed(self, command: BaseCommand):
-        return self._command_serial_number_cache.contains(command.serial_number)
-
-    def receive_command(self, commands: Commands):
-        for command in commands.commands:
-            try:
-                base_command = CommandDeserializer.deserialize(command)
-                logger.debug('received command [{%s} {%s}]', base_command.command, base_command.serial_number)
-
-                if self.__is_command_executed(base_command):
-                    logger.warning('command[{%s}] is executed, ignored.', base_command.command)
-                    continue
-
-                try:
-                    self._commands.put_nowait(base_command)
-                except AsyncQueueFull:
-                    logger.warning(
-                        'command[{%s}, {%s}] cannot add to command list. because the command list is full.',
-                        base_command.command,
-                        base_command.serial_number)
-            except UnsupportedCommandException as e:
-                logger.warning('received unsupported command[{%s}].', e.command.command)
-
-
 class CommandSerialNumberCache:
 
     def __init__(self, maxlen=64):
         self.queue = deque(maxlen=maxlen)
 
     def add(self, number: str):
         # Once a bounded length deque is full, when new items are added,
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/executors/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/executors/command_executor.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/executors/noop_command_executor.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/noop_command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/executors/profile_task_command_executor.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/executors/profile_task_command_executor.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/command/profile_task_command.py` & `apache_skywalking_onepiece-1.1.1/skywalking/command/profile_task_command.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/config.py` & `apache_skywalking_onepiece-1.1.1/skywalking/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,14 @@
 # in format of `service_instance-child(pid)`.
 # This feature may not work when a precise combination of gRPC + Python 3.7 + subprocess (not fork) is used together.
 # The agent will output a warning log when using on Python 3.7 for such a reason.
 agent_experimental_fork_support: bool = os.getenv('SW_AGENT_EXPERIMENTAL_FORK_SUPPORT', '').lower() == 'true'
 # DANGEROUS - This option controls the interval of each bulk report from telemetry data queues
 # Do not modify unless you have evaluated its impact given your service load.
 agent_queue_timeout: int = int(os.getenv('SW_AGENT_QUEUE_TIMEOUT', '1'))
-# Replace the threads to asyncio coroutines to report telemetry data to the OAP.
-# This option is experimental and may not work as expected.
-agent_asyncio_enhancement: bool = os.getenv('SW_AGENT_ASYNCIO_ENHANCEMENT', '').lower() == 'true'
 
 # BEGIN: SW_PYTHON Auto Instrumentation CLI
 # Special: can only be passed via environment. This config controls the child process agent bootstrap behavior in
 # `sw-python` CLI, if set to `False`, a valid child process will not boot up a SkyWalking Agent. Please refer to the
 # [CLI Guide](CLI.md) for details.
 agent_sw_python_bootstrap_propagate = os.getenv('SW_AGENT_SW_PYTHON_BOOTSTRAP_PROPAGATE', '').lower() == 'true'
 # Special: can only be passed via environment. This config controls the CLI and agent logging debug mode, if set to
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/decorators.py` & `apache_skywalking_onepiece-1.1.1/skywalking/decorators.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/log/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/log/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/log/formatter.py` & `apache_skywalking_onepiece-1.1.1/skywalking/log/formatter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/log/sw_logging.py` & `apache_skywalking_onepiece-1.1.1/skywalking/log/sw_logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,19 +82,16 @@
         primary_endpoint_name = ''
 
         try:
             # Try to extract active span, if user code/plugin code throws uncaught
             # exceptions before any span is even created, just ignore these fields and
             # avoid appending 'no active span' traceback that could be confusing.
             # Or simply the log is generated outside any span context.
-            # But actually NO need to raise and catch IllegalStateError here.
-            active_span = context.active_span
-            if active_span is not None:
-                active_span_id = active_span.sid
-                primary_endpoint_name = context.primary_endpoint.get_name() if context.primary_endpoint else ''
+            active_span_id = context.active_span.sid
+            primary_endpoint_name = context.primary_endpoint.get_name()
         except IllegalStateError:
             pass
 
         log_data = LogData(
             timestamp=round(record.created * 1000),
             service=config.agent_name,
             serviceInstance=config.agent_instance_name,
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/loggings.py` & `apache_skywalking_onepiece-1.1.1/skywalking/loggings.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-import asyncio
-
 _meter_service = None
 
 
 def init(force: bool = False):
     """
     If the meter service is not initialized, initialize it.
     if force, we are in a fork(), we force re-initialization
@@ -29,19 +27,7 @@
 
     global _meter_service
     if _meter_service and not force:
         return
 
     _meter_service = MeterService()
     _meter_service.start()
-
-
-async def init_async(async_event: asyncio.Event = None):
-    from skywalking.meter.meter_service import MeterServiceAsync
-
-    global _meter_service
-
-    _meter_service = MeterServiceAsync()
-    if async_event is not None:
-        async_event.set()
-    task = asyncio.create_task(_meter_service.start())
-    _meter_service.strong_ref_set.add(task)
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/counter.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/counter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/gauge.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/gauge.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/histogram.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/histogram.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/meter.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/meter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/meter_service.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/meter_service.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import time
-import asyncio
-
 from concurrent.futures import ThreadPoolExecutor
 from threading import Thread
 from skywalking import config
 from skywalking.agent import agent
 from skywalking.meter.meter import BaseMeter
 from skywalking.utils.time import current_milli_time
 from skywalking.loggings import logger
@@ -50,40 +48,7 @@
         with ThreadPoolExecutor(thread_name_prefix='meter_service_pool_worker', max_workers=1) as executor:
             executor.map(archive, self.meter_map.values())
 
     def run(self):
         while True:
             time.sleep(config.agent_meter_reporter_period)
             self.send()
-
-
-class MeterServiceAsync():
-    def __init__(self):
-        self.meter_map = {}
-        # strong reference to asyncio.Task to prevent garbage collection
-        self.strong_ref_set = set()
-
-    def register(self, meter: BaseMeter):
-        self.meter_map[meter.get_id().get_name()] = meter
-
-    def get_meter(self, name: str):
-        return self.meter_map.get(name)
-
-    async def send(self):
-
-        async def archive_async(meterdata):
-            meterdata = meterdata.transform()
-            meterdata.service = config.agent_name
-            meterdata.serviceInstance = config.agent_instance_name
-            meterdata.timestamp = current_milli_time()
-            await agent.archive_meter_async(meterdata)
-
-        for m in self.meter_map.values():
-            task = asyncio.create_task(archive_async(m))
-            self.strong_ref_set.add(task)
-            task.add_done_callback(self.strong_ref_set.discard)
-
-    async def start(self):
-        logger.debug('Started async meter service')
-        while True:
-            await asyncio.sleep(config.agent_meter_reporter_period)
-            await self.send()
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/cpu_usage.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/data_source.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/data_source.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/gc_data.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/gc_data.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/mem_usage.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/mem_usage.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/meter/pvm/thread_data.py` & `apache_skywalking_onepiece-1.1.1/skywalking/meter/pvm/thread_data.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,30 +16,15 @@
 #
 import inspect
 import logging
 import pkgutil
 import re
 import traceback
 
-import sys
-
-if sys.version_info < (3, 8):
-    import pkg_resources
-    PackageNotFoundException = pkg_resources.DistributionNotFound
-
-    def get_pkg_version(pkg_name):
-        return pkg_resources.get_distribution(pkg_name).version
-
-else:
-    import importlib.metadata
-    PackageNotFoundException = importlib.metadata.PackageNotFoundError
-
-    def get_pkg_version(pkg_name):
-        return importlib.metadata.version(pkg_name)
-
+import pkg_resources
 from packaging import version
 
 import skywalking
 from skywalking import config
 from skywalking.loggings import logger
 from skywalking.utils.comparator import operators
 from skywalking.utils.exception import VersionRuleException
@@ -89,16 +74,16 @@
     if not hasattr(plugin, 'version_rule'):
         return supported
 
     pkg_name = plugin.version_rule.get('name')
     rules = plugin.version_rule.get('rules')
 
     try:
-        current_pkg_version = get_pkg_version(pkg_name)
-    except PackageNotFoundException:
+        current_pkg_version = pkg_resources.get_distribution(pkg_name).version
+    except pkg_resources.DistributionNotFound:
         # when failed to get the version, we consider it as supported.
         return supported
 
     current_version = version.parse(current_pkg_version)
     # pass one rule in rules (OR)
     for rule in rules:
         if rule.find(' ') == -1:
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aiohttp.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiohttp.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,21 @@
 }
 note = """"""
 
 
 def install():
     from aiohttp import ClientSession
     from aiohttp.web_protocol import RequestHandler
-    from aiohttp.web_request import BaseRequest
     from multidict import CIMultiDict, MultiDict, MultiDictProxy
     from yarl import URL
 
-    _request = ClientSession._request
-
     async def _sw_request(self: ClientSession, method: str, str_or_url, **kwargs):
         url = URL(str_or_url).with_user(None).with_password(None)
         peer = f"{url.host or ''}:{url.port or ''}"
 
-        if config.agent_protocol == 'http' and config.agent_collector_backend_services.rstrip('/') \
-                .endswith(f'{url.host}:{url.port}'):
-            return _request
-
         span = NoopSpan(NoopContext()) if config.ignore_http_method_check(method) \
             else get_context().new_exit_span(op=url.path or '/', peer=peer, component=Component.AioHttp)
 
         with span:
             span.layer = Layer.Http
             span.tag(TagHttpMethod(method.upper()))  # pyre-ignore
             span.tag(TagHttpURL(str(url.with_password(None))))  # pyre-ignore
@@ -72,24 +65,18 @@
             span.tag(TagHttpStatusCode(res.status))
 
             if res.status >= 400:
                 span.error_occurred = True
 
             return res
 
+    _request = ClientSession._request
     ClientSession._request = _sw_request
 
-    _handle_request = RequestHandler._handle_request
-
-    async def _sw_handle_request(self, request: BaseRequest, start_time: float):
-
-        if config.agent_protocol == 'http' and config.agent_collector_backend_services.rstrip('/') \
-                .endswith(f'{request.url.host}:{request.url.port}'):
-            return _handle_request
-
+    async def _sw_handle_request(self, request, start_time: float):
         carrier = Carrier()
         method = request.method
 
         for item in carrier:
             val = request.headers.get(item.key)
 
             if val is not None:
@@ -115,8 +102,9 @@
             span.tag(TagHttpStatusCode(resp.status))
 
             if resp.status >= 400:
                 span.error_occurred = True
 
         return resp, reset
 
+    _handle_request = RequestHandler._handle_request
     RequestHandler._handle_request = _sw_handle_request
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aioredis.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aioredis.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_aiormq.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_aiormq.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_amqp.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_amqp.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_asyncpg.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_asyncpg.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_bottle.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_bottle.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_celery.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_celery.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_confluent_kafka.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_confluent_kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_django.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_django.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_elasticsearch.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_falcon.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_falcon.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_fastapi.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_fastapi.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_flask.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_flask.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_happybase.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_happybase.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_http_server.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_http_server.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_httpx.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_httpx.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_kafka.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_kafka.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_loguru.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_loguru.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,19 +75,16 @@
         primary_endpoint_name = ''
 
         try:
             # Try to extract active span, if user code/plugin code throws uncaught
             # exceptions before any span is even created, just ignore these fields and
             # avoid appending 'no active span' traceback that could be confusing.
             # Or simply the log is generated outside any span context.
-            # But actually NO need to raise and catch IllegalStateError here.
-            active_span = context.active_span
-            if active_span is not None:
-                active_span_id = active_span.sid
-                primary_endpoint_name = context.primary_endpoint.get_name() if context.primary_endpoint else ''
+            active_span_id = context.active_span.sid
+            primary_endpoint_name = context.primary_endpoint.get_name()
         except IllegalStateError:
             pass
 
         log_data = LogData(
             timestamp=round(record['time'].timestamp() * 1000),
             service=config.agent_name,
             serviceInstance=config.agent_instance_name,
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_mysqlclient.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_mysqlclient.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_psycopg.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_psycopg2.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_psycopg2.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pymongo.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymongo.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pymysql.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pymysql.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_pyramid.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_pyramid.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_rabbitmq.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_redis.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_redis.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_requests.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_requests.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_sanic.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_sanic.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_tornado.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_tornado.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_urllib3.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib3.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_urllib_request.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_urllib_request.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/plugins/sw_websockets.py` & `apache_skywalking_onepiece-1.1.1/skywalking/plugins/sw_websockets.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_constants.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_constants.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_context.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 # limitations under the License.
 #
 
 import sys
 import time
 import traceback
 
+from packaging import version
 from threading import Thread, Event, current_thread
 from typing import Optional
 
 from skywalking.agent import agent
 from skywalking import config
 from skywalking import profile
 from skywalking.loggings import logger
@@ -38,20 +39,23 @@
 THREAD_MODEL = 'thread'
 try:
     from gevent import monkey
     import greenlet
     from gevent.exceptions import BlockingSwitchOutError
 
     if monkey.is_module_patched('threading'):
-        THREAD_MODEL = 'greenlet'
-        logger.debug('Using greenlet model')
-    else:
-        logger.debug('Gevent monkey exists but does not patch threading, using threading model')
+        if version.parse(greenlet.__version__) <= version.parse('1.1.3.post0'):
+            # todo: greenlet will raise a segment fault with signal 11 when it upgrade to 2.0.0
+            # this issue may be caused by gevent's compatibility with greenlet
+            # we should do some tests when gevent release a new version to verify if this issue would be fixed
+            THREAD_MODEL = 'greenlet'
+        else:
+            logger.warn('greenlet profiler can not work with version >= 2.0.0')
 except ImportError:
-    logger.debug("Gevent does\'t exist, using threading model")
+    pass
 
 
 class ProfileTaskExecutionContext:
     def __init__(self, task: ProfileTask):
         self.task = task  # type: ProfileTask
         self._current_profiling_cnt = AtomicInteger(var=0)
         self._total_started_profiling_cnt = AtomicInteger(var=0)
@@ -318,15 +322,14 @@
             stack_list,
                     )
         self.dump_sequence += 1
         return snapshot
 
 
     def start_profiling(self, context: ProfileTaskExecutionContext):
-        logger.debug('GreenletProfiler::start_profiling')
         self._task_execution_context = context
         try:
             curr = self._profiling_thread
 
             def callback(event, args):
                 origin, target = args
                 if origin == curr or target == curr:
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_service.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_service.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_status.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_status.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/profile_task.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/profile_task.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/profile/snapshot.py` & `apache_skywalking_onepiece-1.1.1/skywalking/profile/snapshot.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/carrier.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/carrier.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/context.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -223,26 +223,24 @@
         if self._nspans == 0:
             agent.archive_segment(self.segment)
             return True
 
         return False
 
     @staticmethod
-    def peek(raise_if_none: bool = False) -> Optional[Span]:
+    def peek() -> Optional[Span]:
         spans = _spans()
-        if not spans:
-            if raise_if_none:
-                raise IllegalStateError('No active span')
-            else:
-                return None
-        return spans[-1]
+        return spans[-1] if spans else None
 
     @property
     def active_span(self):
-        return self.peek(raise_if_none=False)
+        active_span = self.peek()
+        if not active_span:
+            raise IllegalStateError('No active span')
+        return active_span
 
     def get_correlation(self, key):
         if key in self._correlation:
             return self._correlation[key]
         return None
 
     def put_correlation(self, key, value):
```

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/segment.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/segment.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/snapshot.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/snapshot.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/span.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/span.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/trace/tags.py` & `apache_skywalking_onepiece-1.1.1/skywalking/trace/tags.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/__init__.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/array.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/array.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/atomic_ref.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/atomic_ref.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/comparator.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/comparator.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/counter.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/counter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/exception.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/exception.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/filter.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/filter.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/integer.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/integer.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/lang.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/lang.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/singleton.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/skywalking/utils/time.py` & `apache_skywalking_onepiece-1.1.1/skywalking/utils/time.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/sw_python/__init__.py` & `apache_skywalking_onepiece-1.1.1/sw_python/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/sw_python/__main__.py` & `apache_skywalking_onepiece-1.1.1/sw_python/__main__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/sw_python/src/__init__.py` & `apache_skywalking_onepiece-1.1.1/sw_python/src/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/sw_python/src/sw_python.py` & `apache_skywalking_onepiece-1.1.1/sw_python/src/sw_python.py`

 * *Files identical despite different names*

### Comparing `apache_skywalking_onepiece-1.1.0/setup.py` & `apache_skywalking_onepiece-1.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,48 +14,47 @@
  'skywalking.command',
  'skywalking.command.executors',
  'skywalking.log',
  'skywalking.meter',
  'skywalking.meter.pvm',
  'skywalking.plugins',
  'skywalking.profile',
+ 'skywalking.protocol',
+ 'skywalking.protocol.browser',
+ 'skywalking.protocol.common',
+ 'skywalking.protocol.event',
+ 'skywalking.protocol.language_agent',
+ 'skywalking.protocol.logging',
+ 'skywalking.protocol.management',
+ 'skywalking.protocol.profile',
+ 'skywalking.protocol.service_mesh_probe',
  'skywalking.trace',
  'skywalking.utils',
  'sw_python',
  'sw_python.src']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['grpcio', 'grpcio-tools', 'packaging', 'psutil<=5.9.5', 'wrapt']
+['grpcio', 'grpcio-tools', 'packaging', 'psutil', 'wrapt']
 
 extras_require = \
-{'all': ['requests>=2.26.0',
-         'kafka-python',
-         'uvloop>=0.17.0,<0.18.0',
-         'aiokafka>=0.8.0,<0.9.0',
-         'aiohttp>=3.7.4,<4.0.0'],
- 'async': ['uvloop>=0.17.0,<0.18.0',
-           'aiokafka>=0.8.0,<0.9.0',
-           'aiohttp>=3.7.4,<4.0.0'],
- 'asynchttp': ['uvloop>=0.17.0,<0.18.0', 'aiohttp>=3.7.4,<4.0.0'],
- 'asynckafka': ['uvloop>=0.17.0,<0.18.0', 'aiokafka>=0.8.0,<0.9.0'],
+{'all': ['requests>=2.26.0', 'kafka-python'],
  'http': ['requests>=2.26.0'],
- 'kafka': ['kafka-python'],
- 'sync': ['requests>=2.26.0', 'kafka-python']}
+ 'kafka': ['kafka-python']}
 
 entry_points = \
 {'console_scripts': ['sw-python = skywalking.bootstrap.cli.sw_python:start']}
 
 setup_kwargs = {
     'name': 'apache-skywalking-onepiece',
-    'version': '1.1.0',
+    'version': '1.1.1',
     'description': 'The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects.',
-    'long_description': '# SkyWalking Python Agent\n\n<img src="http://skywalking.apache.org/assets/logo.svg" alt="Sky Walking logo" height="90px" align="right" />\n\n**SkyWalking-Python**: The Python Agent for Apache SkyWalking provides the native tracing/metrics/logging/profiling abilities for Python projects.\n\n**[SkyWalking](https://github.com/apache/skywalking)**: Application performance monitor tool for distributed systems, especially designed for microservices, cloud native and container-based (Kubernetes) architectures.\n\n\n[![GitHub stars](https://img.shields.io/github/stars/apache/skywalking-python.svg?style=for-the-badge&label=Stars&logo=github)](https://github.com/apache/skywalking-python)\n[![Twitter Follow](https://img.shields.io/twitter/follow/asfskywalking.svg?style=for-the-badge&label=Follow&logo=twitter)](https://twitter.com/AsfSkyWalking)\n\n![Release](https://img.shields.io/pypi/v/apache-skywalking)\n![Version](https://img.shields.io/pypi/pyversions/apache-skywalking)\n![Build](https://github.com/apache/skywalking-python/actions/workflows/CI.yaml/badge.svg?event=push)\n\n## Documentation\n\n- [Official documentation](https://skywalking.apache.org/docs/#PythonAgent)\n- [Blog](https://skywalking.apache.org/blog/2021-09-12-skywalking-python-profiling/) about the Python Agent Profiling Feature\n\n## Capabilities\n\n| Reporter  | Supported?      | Details                                                    | \n|:----------|:----------------|:-----------------------------------------------------------|\n| Trace     | ✅ (default: ON) | Automatic instrumentation + Manual SDK                     |            \n| Log       | ✅ (default: ON) | Direct reporter only. (Tracing context in log planned)     |\n| Meter     | ✅ (default: ON) | Meter API + Automatic PVM metrics                          |\n| Event     | ❌ (Planned)     | Report lifecycle events of your awesome Python application |\n| Profiling | ✅ (default: ON) | Threading and Greenlet Profiler                            |\n\n## Installation Requirements\n\nSkyWalking Python Agent requires [Apache SkyWalking 8.0+](https://skywalking.apache.org/downloads/#SkyWalkingAPM) and Python 3.7+.\n\n> If you would like to try out the latest features that are not released yet, please refer to this [guide](docs/en/setup/faq/How-to-build-from-sources.md) to build from sources.\n\n## Live Demo\n- Find the [live demo](https://skywalking.apache.org/#demo) with Python agent on our website.\n- Follow the [showcase](https://skywalking.apache.org/docs/skywalking-showcase/next/readme/) to set up preview deployment quickly.\n\n## Contributing\n\nBefore submitting a pull request or pushing a commit, please read our [contributing](CONTRIBUTING.md) and [developer guide](docs/en/contribution/Developer.md).\n\n## Contact Us\n* Mail list: **dev@skywalking.apache.org**. Mail to `dev-subscribe@skywalking.apache.org`, follow the reply to subscribe the mail list.\n* Send `Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.\n* Twitter, [ASFSkyWalking](https://twitter.com/AsfSkyWalking)\n* For Chinese speaker, send `[CN] Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.\n* [bilibili B站 视频](https://space.bilibili.com/390683219)\n\n## License\nApache 2.0\n',
+    'long_description': '# SkyWalking Python Agent\n\n<img src="http://skywalking.apache.org/assets/logo.svg" alt="Sky Walking logo" height="90px" align="right" />\n\n**SkyWalking-Python**: The Python Agent for Apache SkyWalking provides the native tracing/metrics/logging/profiling abilities for Python projects.\n\n**[SkyWalking](https://github.com/apache/skywalking)**: Application performance monitor tool for distributed systems, especially designed for microservices, cloud native and container-based (Kubernetes) architectures.\n\n\n[![GitHub stars](https://img.shields.io/github/stars/apache/skywalking-python.svg?style=for-the-badge&label=Stars&logo=github)](https://github.com/apache/skywalking-python)\n[![Twitter Follow](https://img.shields.io/twitter/follow/asfskywalking.svg?style=for-the-badge&label=Follow&logo=twitter)](https://twitter.com/AsfSkyWalking)\n\n![Release](https://img.shields.io/pypi/v/apache-skywalking)\n![Version](https://img.shields.io/pypi/pyversions/apache-skywalking)\n![Build](https://github.com/apache/skywalking-python/actions/workflows/CI.yaml/badge.svg?event=push)\n\n## Documentation\n\n- [Official documentation](https://skywalking.apache.org/docs/#PythonAgent)\n- [Blog](https://skywalking.apache.org/blog/2021-09-12-skywalking-python-profiling/) about the Python Agent Profiling Feature\n\n## Capabilities\n\n| Reporter  | Supported?      | Details                                                    | \n|:----------|:----------------|:-----------------------------------------------------------|\n| Trace     | ✅ (default: ON) | Automatic instrumentation + Manual SDK                     |            \n| Log       | ✅ (default: ON) | Direct reporter only. (Tracing context in log planned)     |\n| Meter     | ✅ (default: ON) | Meter API + Automatic PVM metrics                          |\n| Event     | ❌ (Planned)     | Report lifecycle events of your awesome Python application |\n| Profiling | ✅ (default: ON) | Threading and Greenlet Profiler                            |\n\n## Installation Requirements\n\nSkyWalking Python Agent requires [Apache SkyWalking 8.0+](https://skywalking.apache.org/downloads/#SkyWalkingAPM) and Python 3.7+.\n\n> If you would like to try out the latest features that are not released yet, please refer to this [guide](docs/en/setup/faq/How-to-build-from-sources.md) to build from sources.\n\n## Live Demo\n- Find the [live demo](https://skywalking.apache.org/#demo) with Python agent on our website.\n- Follow the [showcase](https://skywalking.apache.org/docs/skywalking-showcase/next/readme/) to set up preview deployment quickly.\n\n## Contributing\n\nBefore submitting a pull request or pushing a commit, please read our [contributing](CONTRIBUTING.md) and [developer guide](docs/en/contribution/Developer.md).\n\n## Contact Us\n* Mail list: **dev@skywalking.apache.org**. Mail to `dev-subscribe@skywalking.apache.org`, follow the reply to subscribe the mail list.\n* Send `Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.\n* Twitter, [ASFSkyWalking](https://twitter.com/AsfSkyWalking)\n* QQ Group: 901167865, 392443393\n* [bilibili B站 视频](https://space.bilibili.com/390683219)\n\n## License\nApache 2.0\n',
     'author': 'Apache Software Foundation',
     'author_email': 'dev@skywalking.apache.org',
     'maintainer': 'Apache SkyWalking Community',
     'maintainer_email': 'dev@skywalking.apache.org',
     'url': 'https://skywalking.apache.org/',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `apache_skywalking_onepiece-1.1.0/PKG-INFO` & `apache_skywalking_onepiece-1.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-skywalking-onepiece
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Python Agent for Apache SkyWalking, which provides the native tracing/metrics/logging/profiling abilities for Python projects.
 Home-page: https://skywalking.apache.org/
 License: Apache-2.0
 Keywords: skywalking,tracing,metrics,logging,profiling,observability,distributed-tracing,apm,python
 Author: Apache Software Foundation
 Author-email: dev@skywalking.apache.org
 Maintainer: Apache SkyWalking Community
@@ -18,29 +18,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: System :: Monitoring
 Provides-Extra: all
-Provides-Extra: async
-Provides-Extra: asynchttp
-Provides-Extra: asynckafka
 Provides-Extra: http
 Provides-Extra: kafka
-Provides-Extra: sync
-Requires-Dist: aiohttp (>=3.7.4,<4.0.0) ; extra == "all" or extra == "async" or extra == "asynchttp"
-Requires-Dist: aiokafka (>=0.8.0,<0.9.0) ; extra == "all" or extra == "async" or extra == "asynckafka"
 Requires-Dist: grpcio
 Requires-Dist: grpcio-tools
-Requires-Dist: kafka-python ; extra == "all" or extra == "sync" or extra == "kafka"
+Requires-Dist: kafka-python ; extra == "all" or extra == "kafka"
 Requires-Dist: packaging
-Requires-Dist: psutil (<=5.9.5)
-Requires-Dist: requests (>=2.26.0) ; extra == "all" or extra == "sync" or extra == "http"
-Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; extra == "all" or extra == "async" or extra == "asynchttp" or extra == "asynckafka"
+Requires-Dist: psutil
+Requires-Dist: requests (>=2.26.0) ; extra == "all" or extra == "http"
 Requires-Dist: wrapt
 Project-URL: Bug Tracker, https://github.com/apache/skywalking/issues
 Project-URL: Documentation, https://skywalking.apache.org/docs/skywalking-python/next/readme/
 Project-URL: Repository, https://github.com/apache/skywalking-python
 Description-Content-Type: text/markdown
 
 # SkyWalking Python Agent
@@ -88,13 +81,13 @@
 
 Before submitting a pull request or pushing a commit, please read our [contributing](CONTRIBUTING.md) and [developer guide](docs/en/contribution/Developer.md).
 
 ## Contact Us
 * Mail list: **dev@skywalking.apache.org**. Mail to `dev-subscribe@skywalking.apache.org`, follow the reply to subscribe the mail list.
 * Send `Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.
 * Twitter, [ASFSkyWalking](https://twitter.com/AsfSkyWalking)
-* For Chinese speaker, send `[CN] Request to join SkyWalking slack` mail to the mail list(`dev@skywalking.apache.org`), we will invite you in.
+* QQ Group: 901167865, 392443393
 * [bilibili B站 视频](https://space.bilibili.com/390683219)
 
 ## License
 Apache 2.0
```

