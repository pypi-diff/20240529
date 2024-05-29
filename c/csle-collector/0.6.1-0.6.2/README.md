# Comparing `tmp/csle_collector-0.6.1.tar.gz` & `tmp/csle_collector-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.6.1.tar", last modified: Thu May 23 18:35:03 2024, max compression
+gzip compressed data, was "csle_collector-0.6.2.tar", last modified: Tue May 28 16:30:10 2024, max compression
```

## Comparing `csle_collector-0.6.1.tar` & `csle_collector-0.6.2.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.347895 csle_collector-0.6.1/
--rw-r--r--   0 kim        (501) staff       (20)      793 2024-05-23 18:35:03.347970 csle_collector-0.6.1/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     6209 2024-02-13 12:24:16.000000 csle_collector-0.6.1/README.md
--rw-r--r--   0 kim        (501) staff       (20)      674 2023-08-15 10:44:03.000000 csle_collector-0.6.1/pyproject.toml
--rw-r--r--   0 kim        (501) staff       (20)     2012 2024-05-23 18:35:03.348250 csle_collector-0.6.1/setup.cfg
--rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_collector-0.6.1/setup.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.330188 csle_collector-0.6.1/src/
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.332292 csle_collector-0.6.1/src/csle_collector/
--rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-23 18:34:56.000000 csle_collector-0.6.1/src/csle_collector/__version__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.334231 csle_collector-0.6.1/src/csle_collector/client_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    11529 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/client_manager/client_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     5708 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)     8592 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     2179 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)     4905 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/client_manager/client_population_metrics.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.336004 csle_collector-0.6.1/src/csle_collector/client_manager/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     1538 2023-08-26 08:04:28.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)    10142 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/client.py
--rw-r--r--   0 kim        (501) staff       (20)      340 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/client_arrival_type.py
--rw-r--r--   0 kim        (501) staff       (20)     2646 2023-08-17 11:41:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/constant_arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3498 2023-08-17 11:41:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3333 2023-08-17 11:41:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3647 2023-08-17 11:41:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/sine_arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)     3037 2023-08-17 11:41:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/spiking_arrival_config.py
--rw-r--r--   0 kim        (501) staff       (20)     5442 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflow_markov_chain.py
--rw-r--r--   0 kim        (501) staff       (20)     5167 2023-08-26 12:43:42.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflow_service.py
--rw-r--r--   0 kim        (501) staff       (20)     5506 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflows_config.py
--rw-r--r--   0 kim        (501) staff       (20)     4274 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/query_clients.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.336605 csle_collector-0.6.1/src/csle_collector/client_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     7493 2023-09-20 12:38:50.000000 csle_collector-0.6.1/src/csle_collector/client_manager/threads/arrival_thread.py
--rw-r--r--   0 kim        (501) staff       (20)      972 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/threads/client_thread.py
--rw-r--r--   0 kim        (501) staff       (20)     2375 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/client_manager/threads/producer_thread.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.336920 csle_collector-0.6.1/src/csle_collector/constants/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/constants/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    36628 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/constants/constants.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.337773 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.338073 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 12:02:11.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    12998 2023-10-09 08:04:01.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/dao/docker_stats.py
--rw-r--r--   0 kim        (501) staff       (20)     8158 2023-08-17 14:42:06.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2578 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)     6193 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     8932 2023-08-17 12:02:53.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-r--r--   0 kim        (501) staff       (20)     4276 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.338316 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 11:58:45.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     6475 2023-08-17 12:02:53.000000 csle_collector-0.6.1/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.339026 csle_collector-0.6.1/src/csle_collector/elk_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    10740 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2642 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)    14300 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     1540 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)     6227 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/elk_manager/query_elk_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.339842 csle_collector-0.6.1/src/csle_collector/host_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.340318 csle_collector-0.6.1/src/csle_collector/host_manager/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2152 2023-10-10 07:26:51.000000 csle_collector-0.6.1/src/csle_collector/host_manager/dao/failed_login_attempt.py
--rw-r--r--   0 kim        (501) staff       (20)     8321 2023-10-10 15:35:12.000000 csle_collector-0.6.1/src/csle_collector/host_manager/dao/host_metrics.py
--rw-r--r--   0 kim        (501) staff       (20)     2697 2023-10-10 15:35:12.000000 csle_collector-0.6.1/src/csle_collector/host_manager/dao/successful_login.py
--rw-r--r--   0 kim        (501) staff       (20)    61864 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/host_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     6844 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)    28800 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)    34458 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)    17833 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/query_host_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.340539 csle_collector-0.6.1/src/csle_collector/host_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2684 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/host_manager/threads/host_monitor_thread.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.341257 csle_collector-0.6.1/src/csle_collector/kafka_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     6487 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2146 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)     8484 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     1726 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)     3501 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.342024 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.342350 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     3665 2023-10-10 15:35:12.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py
--rw-r--r--   0 kim        (501) staff       (20)    13966 2023-10-13 14:30:45.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py
--rw-r--r--   0 kim        (501) staff       (20)     9655 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     4448 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)    10801 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)    13730 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-r--r--   0 kim        (501) staff       (20)     5883 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.342571 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2108 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.343152 csle_collector-0.6.1/src/csle_collector/ryu_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     4241 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/query_ryu_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    15273 2023-08-17 13:01:17.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2414 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)     8367 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     2102 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.343339 csle_collector-0.6.1/src/csle_collector/ryu_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 12:58:31.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     3332 2023-08-17 14:41:06.000000 csle_collector-0.6.1/src/csle_collector/ryu_manager/threads/failure_detector.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.343978 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/__init__.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.344805 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)    11068 2023-10-11 07:23:20.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py
--rw-r--r--   0 kim        (501) staff       (20)    12629 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py
--rw-r--r--   0 kim        (501) staff       (20)     2520 2023-10-12 15:33:50.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py
--rw-r--r--   0 kim        (501) staff       (20)     9819 2023-10-12 15:33:50.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py
--rw-r--r--   0 kim        (501) staff       (20)     4903 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py
--rw-r--r--   0 kim        (501) staff       (20)     6293 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    10517 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     5252 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)    10801 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)    16968 2023-10-12 15:33:50.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.345086 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/threads/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/threads/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2839 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.345865 csle_collector-0.6.1/src/csle_collector/traffic_manager/
--rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/__init__.py
--rw-r--r--   0 kim        (501) staff       (20)     2753 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     7861 2024-02-13 12:24:16.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     1735 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-r--r--   0 kim        (501) staff       (20)     5596 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-r--r--   0 kim        (501) staff       (20)     1526 2023-08-15 10:44:03.000000 csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.333096 csle_collector-0.6.1/src/csle_collector.egg-info/
--rw-r--r--   0 kim        (501) staff       (20)      793 2024-05-23 18:35:03.000000 csle_collector-0.6.1/src/csle_collector.egg-info/PKG-INFO
--rw-r--r--   0 kim        (501) staff       (20)     6419 2024-05-23 18:35:03.000000 csle_collector-0.6.1/src/csle_collector.egg-info/SOURCES.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-23 18:35:03.000000 csle_collector-0.6.1/src/csle_collector.egg-info/dependency_links.txt
--rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:29.000000 csle_collector-0.6.1/src/csle_collector.egg-info/not-zip-safe
--rw-r--r--   0 kim        (501) staff       (20)      612 2024-05-23 18:35:03.000000 csle_collector-0.6.1/src/csle_collector.egg-info/requires.txt
--rw-r--r--   0 kim        (501) staff       (20)       15 2024-05-23 18:35:03.000000 csle_collector-0.6.1/src/csle_collector.egg-info/top_level.txt
-drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-23 18:35:03.347752 csle_collector-0.6.1/tests/
--rw-r--r--   0 kim        (501) staff       (20)    17047 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_client_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     7897 2023-10-09 07:12:58.000000 csle_collector-0.6.1/tests/test_client_manager_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     7187 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_docker_stats_manager.py
--rw-r--r--   0 kim        (501) staff       (20)      830 2023-10-09 08:04:01.000000 csle_collector-0.6.1/tests/test_docker_stats_manager_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     8856 2023-08-17 14:42:27.000000 csle_collector-0.6.1/tests/test_elk_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    34019 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_host_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     2564 2023-10-10 15:35:12.000000 csle_collector-0.6.1/tests/test_host_manager_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     5250 2023-08-17 10:51:10.000000 csle_collector-0.6.1/tests/test_kafka_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    12484 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_ossec_ids_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     1875 2023-10-10 15:35:12.000000 csle_collector-0.6.1/tests/test_ossec_ids_manager_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     9883 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_ryu_manager.py
--rw-r--r--   0 kim        (501) staff       (20)    12634 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_snort_ids_manager.py
--rw-r--r--   0 kim        (501) staff       (20)     4708 2023-10-11 07:23:20.000000 csle_collector-0.6.1/tests/test_snort_ids_manager_dao.py
--rw-r--r--   0 kim        (501) staff       (20)     5094 2023-08-17 14:04:12.000000 csle_collector-0.6.1/tests/test_traffic_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.462808 csle_collector-0.6.2/
+-rw-r--r--   0 kim        (501) staff       (20)      793 2024-05-28 16:30:10.462849 csle_collector-0.6.2/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     6209 2024-02-13 12:24:16.000000 csle_collector-0.6.2/README.md
+-rw-r--r--   0 kim        (501) staff       (20)      674 2023-08-15 10:44:03.000000 csle_collector-0.6.2/pyproject.toml
+-rw-r--r--   0 kim        (501) staff       (20)     2012 2024-05-28 16:30:10.463085 csle_collector-0.6.2/setup.cfg
+-rw-r--r--   0 kim        (501) staff       (20)       69 2023-08-15 10:44:03.000000 csle_collector-0.6.2/setup.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.436429 csle_collector-0.6.2/src/
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.438578 csle_collector-0.6.2/src/csle_collector/
+-rw-r--r--   0 kim        (501) staff       (20)       37 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)       22 2024-05-28 16:30:03.000000 csle_collector-0.6.2/src/csle_collector/__version__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.440949 csle_collector-0.6.2/src/csle_collector/client_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11529 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/client_manager/client_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     5708 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)     8592 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     2179 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     4905 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/client_manager/client_population_metrics.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.443332 csle_collector-0.6.2/src/csle_collector/client_manager/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     1538 2023-08-26 08:04:28.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)    10142 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/client.py
+-rw-r--r--   0 kim        (501) staff       (20)      340 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/client_arrival_type.py
+-rw-r--r--   0 kim        (501) staff       (20)     2646 2023-08-17 11:41:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/constant_arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3498 2023-08-17 11:41:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3333 2023-08-17 11:41:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3647 2023-08-17 11:41:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/sine_arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     3037 2023-08-17 11:41:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     5442 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py
+-rw-r--r--   0 kim        (501) staff       (20)     5167 2023-08-26 12:43:42.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflow_service.py
+-rw-r--r--   0 kim        (501) staff       (20)     5506 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflows_config.py
+-rw-r--r--   0 kim        (501) staff       (20)     4274 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/query_clients.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.444074 csle_collector-0.6.2/src/csle_collector/client_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     7493 2023-09-20 12:38:50.000000 csle_collector-0.6.2/src/csle_collector/client_manager/threads/arrival_thread.py
+-rw-r--r--   0 kim        (501) staff       (20)      972 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/threads/client_thread.py
+-rw-r--r--   0 kim        (501) staff       (20)     2375 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/client_manager/threads/producer_thread.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.444384 csle_collector-0.6.2/src/csle_collector/constants/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/constants/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    36628 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/constants/constants.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.445866 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/__init__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.446098 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 12:02:11.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    12998 2023-10-09 08:04:01.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/dao/docker_stats.py
+-rw-r--r--   0 kim        (501) staff       (20)     8158 2023-08-17 14:42:06.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2578 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)     6193 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     8932 2023-08-17 12:02:53.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     4276 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.446473 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 11:58:45.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     6475 2023-08-17 12:02:53.000000 csle_collector-0.6.2/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.447446 csle_collector-0.6.2/src/csle_collector/elk_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    10740 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2642 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)    14300 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     1540 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     6227 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/elk_manager/query_elk_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.448612 csle_collector-0.6.2/src/csle_collector/host_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/__init__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.449580 csle_collector-0.6.2/src/csle_collector/host_manager/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2152 2023-10-10 07:26:51.000000 csle_collector-0.6.2/src/csle_collector/host_manager/dao/failed_login_attempt.py
+-rw-r--r--   0 kim        (501) staff       (20)     8321 2023-10-10 15:35:12.000000 csle_collector-0.6.2/src/csle_collector/host_manager/dao/host_metrics.py
+-rw-r--r--   0 kim        (501) staff       (20)     2697 2023-10-10 15:35:12.000000 csle_collector-0.6.2/src/csle_collector/host_manager/dao/successful_login.py
+-rw-r--r--   0 kim        (501) staff       (20)    61864 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/host_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     6844 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)    28800 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)    34458 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)    17833 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/query_host_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.449850 csle_collector-0.6.2/src/csle_collector/host_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2684 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/host_manager/threads/host_monitor_thread.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.450843 csle_collector-0.6.2/src/csle_collector/kafka_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     6487 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2146 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)     8484 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     1726 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     3501 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.451646 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/__init__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.452157 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     3665 2023-10-10 15:35:12.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py
+-rw-r--r--   0 kim        (501) staff       (20)    13966 2023-10-13 14:30:45.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py
+-rw-r--r--   0 kim        (501) staff       (20)     9655 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     4448 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)    10801 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)    13730 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-r--r--   0 kim        (501) staff       (20)     5883 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.452418 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2108 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.453641 csle_collector-0.6.2/src/csle_collector/ryu_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     4241 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/query_ryu_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    15273 2023-08-17 13:01:17.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2414 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)     8367 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     2102 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.453889 csle_collector-0.6.2/src/csle_collector/ryu_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-17 12:58:31.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     3332 2023-08-17 14:41:06.000000 csle_collector-0.6.2/src/csle_collector/ryu_manager/threads/failure_detector.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.454776 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/__init__.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.456315 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)    11068 2023-10-11 07:23:20.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py
+-rw-r--r--   0 kim        (501) staff       (20)    12629 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py
+-rw-r--r--   0 kim        (501) staff       (20)     2520 2023-10-12 15:33:50.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py
+-rw-r--r--   0 kim        (501) staff       (20)     9819 2023-10-12 15:33:50.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py
+-rw-r--r--   0 kim        (501) staff       (20)     4903 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py
+-rw-r--r--   0 kim        (501) staff       (20)     6293 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    10517 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     5252 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)    10801 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)    16968 2023-10-12 15:33:50.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.456680 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/threads/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/threads/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2839 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.457426 csle_collector-0.6.2/src/csle_collector/traffic_manager/
+-rw-r--r--   0 kim        (501) staff       (20)        0 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/__init__.py
+-rw-r--r--   0 kim        (501) staff       (20)     2753 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     7861 2024-02-13 12:24:16.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     1735 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-r--r--   0 kim        (501) staff       (20)     5596 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-r--r--   0 kim        (501) staff       (20)     1526 2023-08-15 10:44:03.000000 csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.439579 csle_collector-0.6.2/src/csle_collector.egg-info/
+-rw-r--r--   0 kim        (501) staff       (20)      793 2024-05-28 16:30:10.000000 csle_collector-0.6.2/src/csle_collector.egg-info/PKG-INFO
+-rw-r--r--   0 kim        (501) staff       (20)     6419 2024-05-28 16:30:10.000000 csle_collector-0.6.2/src/csle_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2024-05-28 16:30:10.000000 csle_collector-0.6.2/src/csle_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 kim        (501) staff       (20)        1 2023-08-16 11:39:29.000000 csle_collector-0.6.2/src/csle_collector.egg-info/not-zip-safe
+-rw-r--r--   0 kim        (501) staff       (20)      612 2024-05-28 16:30:10.000000 csle_collector-0.6.2/src/csle_collector.egg-info/requires.txt
+-rw-r--r--   0 kim        (501) staff       (20)       15 2024-05-28 16:30:10.000000 csle_collector-0.6.2/src/csle_collector.egg-info/top_level.txt
+drwxr-xr-x   0 kim        (501) staff       (20)        0 2024-05-28 16:30:10.462497 csle_collector-0.6.2/tests/
+-rw-r--r--   0 kim        (501) staff       (20)    17047 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_client_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     7897 2023-10-09 07:12:58.000000 csle_collector-0.6.2/tests/test_client_manager_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     7187 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_docker_stats_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)      830 2023-10-09 08:04:01.000000 csle_collector-0.6.2/tests/test_docker_stats_manager_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     8856 2023-08-17 14:42:27.000000 csle_collector-0.6.2/tests/test_elk_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    34019 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_host_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     2564 2023-10-10 15:35:12.000000 csle_collector-0.6.2/tests/test_host_manager_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     5250 2023-08-17 10:51:10.000000 csle_collector-0.6.2/tests/test_kafka_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    12484 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_ossec_ids_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     1875 2023-10-10 15:35:12.000000 csle_collector-0.6.2/tests/test_ossec_ids_manager_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     9883 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_ryu_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)    12634 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_snort_ids_manager.py
+-rw-r--r--   0 kim        (501) staff       (20)     4708 2023-10-11 07:23:20.000000 csle_collector-0.6.2/tests/test_snort_ids_manager_dao.py
+-rw-r--r--   0 kim        (501) staff       (20)     5094 2023-08-17 14:04:12.000000 csle_collector-0.6.2/tests/test_traffic_manager.py
```

### Comparing `csle_collector-0.6.1/PKG-INFO` & `csle_collector-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.6.1/README.md` & `csle_collector-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/pyproject.toml` & `csle_collector-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/setup.cfg` & `csle_collector-0.6.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Intended Audience :: Science/Research
 
 [options]
 install_requires = 
-	csle-base>=0.6.1
+	csle-base>=0.6.2
 	grpcio>=1.57.0
 	grpcio-tools>=1.57.0
 	scipy>=1.0.0
 	confluent-kafka>=1.8.2
 	docker>=3.0.0
 	PyYaml>=5.1.1
 	requests>=2.19.0
```

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/client.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/client.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/constant_arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/eptmp_arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/eptmp_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/piece_wise_constant_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/sine_arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/sine_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/spiking_arrival_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/spiking_arrival_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflow_markov_chain.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflow_markov_chain.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflow_service.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflow_service.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/dao/workflows_config.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/dao/workflows_config.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/query_clients.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/threads/arrival_thread.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/threads/arrival_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/threads/client_thread.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/threads/client_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/client_manager/threads/producer_thread.py` & `csle_collector-0.6.2/src/csle_collector/client_manager/threads/producer_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/constants/constants.py` & `csle_collector-0.6.2/src/csle_collector/constants/constants.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/dao/docker_stats.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/dao/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py` & `csle_collector-0.6.2/src/csle_collector/docker_stats_manager/threads/docker_stats_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/elk_manager/query_elk_manager.py` & `csle_collector-0.6.2/src/csle_collector/elk_manager/query_elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/dao/failed_login_attempt.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/dao/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/dao/host_metrics.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/dao/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/dao/successful_login.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/dao/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/host_manager/threads/host_monitor_thread.py` & `csle_collector-0.6.2/src/csle_collector/host_manager/threads/host_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.6.2/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/dao/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py` & `csle_collector-0.6.2/src/csle_collector/ossec_ids_manager/threads/ossec_ids_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/query_ryu_manager.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/query_ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/ryu_manager/threads/failure_detector.py` & `csle_collector-0.6.2/src/csle_collector/ryu_manager/threads/failure_detector.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_fast_log_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_ip_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/dao/snort_ids_rule_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py` & `csle_collector-0.6.2/src/csle_collector/snort_ids_manager/threads/snort_ids_monitor_thread.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.6.2/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.6.2/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.6.2/src/csle_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.6.1
+Version: 0.6.2
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.6.1/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.6.2/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/src/csle_collector.egg-info/requires.txt` & `csle_collector-0.6.2/src/csle_collector.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-csle-base>=0.6.1
+csle-base>=0.6.2
 grpcio>=1.57.0
 grpcio-tools>=1.57.0
 scipy>=1.0.0
 confluent-kafka>=1.8.2
 docker>=3.0.0
 PyYaml>=5.1.1
 requests>=2.19.0
```

### Comparing `csle_collector-0.6.1/tests/test_client_manager.py` & `csle_collector-0.6.2/tests/test_client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_client_manager_dao.py` & `csle_collector-0.6.2/tests/test_client_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_docker_stats_manager.py` & `csle_collector-0.6.2/tests/test_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_docker_stats_manager_dao.py` & `csle_collector-0.6.2/tests/test_docker_stats_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_elk_manager.py` & `csle_collector-0.6.2/tests/test_elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_host_manager.py` & `csle_collector-0.6.2/tests/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_host_manager_dao.py` & `csle_collector-0.6.2/tests/test_host_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_kafka_manager.py` & `csle_collector-0.6.2/tests/test_kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_ossec_ids_manager.py` & `csle_collector-0.6.2/tests/test_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_ossec_ids_manager_dao.py` & `csle_collector-0.6.2/tests/test_ossec_ids_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_ryu_manager.py` & `csle_collector-0.6.2/tests/test_ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_snort_ids_manager.py` & `csle_collector-0.6.2/tests/test_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_snort_ids_manager_dao.py` & `csle_collector-0.6.2/tests/test_snort_ids_manager_dao.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.6.1/tests/test_traffic_manager.py` & `csle_collector-0.6.2/tests/test_traffic_manager.py`

 * *Files identical despite different names*

