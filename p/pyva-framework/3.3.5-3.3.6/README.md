# Comparing `tmp/pyva_framework-3.3.5.tar.gz` & `tmp/pyva_framework-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva_framework-3.3.5.tar", last modified: Wed May 29 13:27:04 2024, max compression
+gzip compressed data, was "pyva_framework-3.3.6.tar", last modified: Wed May 29 14:00:48 2024, max compression
```

## Comparing `pyva_framework-3.3.5.tar` & `pyva_framework-3.3.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.035290 pyva_framework-3.3.5/
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.5/LICENSE
--rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 13:27:04.035090 pyva_framework-3.3.5/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.5/README.md
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025237 pyva_framework-3.3.5/pyva/
--rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/Application.py
--rw-r--r--   0 szq        (501) staff       (20)      742 2024-05-29 12:48:14.000000 pyva_framework-3.3.5/pyva/Global.py
--rw-r--r--   0 szq        (501) staff       (20)     1091 2024-05-29 13:21:35.000000 pyva_framework-3.3.5/pyva/GlobalInit.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025718 pyva_framework-3.3.5/pyva/cli/
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/cli/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/cli/main.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025976 pyva_framework-3.3.5/pyva/client/
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.027169 pyva_framework-3.3.5/pyva/client/dingtalk/
--rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkContactClient.py
--rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkOauth2Client.py
--rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkRobotClient.py
--rw-r--r--   0 szq        (501) staff       (20)     6578 2024-05-29 13:05:02.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkYidaClient.py
--rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.028412 pyva_framework-3.3.5/pyva/common/
--rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/FastapiEvents.py
--rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/FastapiException.py
--rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/LoggerHandler.py
--rw-r--r--   0 szq        (501) staff       (20)     3456 2024-05-29 13:06:00.000000 pyva_framework-3.3.5/pyva/common/RequestLogRoute.py
--rw-r--r--   0 szq        (501) staff       (20)      146 2024-05-19 03:56:35.000000 pyva_framework-3.3.5/pyva/common/RequestLogStatusEnum.py
--rw-r--r--   0 szq        (501) staff       (20)      135 2024-05-19 03:56:35.000000 pyva_framework-3.3.5/pyva/common/RequestLogTypeEnum.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.029758 pyva_framework-3.3.5/pyva/config/
--rw-r--r--   0 szq        (501) staff       (20)     1129 2024-05-29 13:13:15.000000 pyva_framework-3.3.5/pyva/config/AppConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DbConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DingtalkConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DingtalkRobotConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/FastapiConfig.py
--rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/LoggingConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/MongoConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/NacosConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/RedisConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.030176 pyva_framework-3.3.5/pyva/dao/
--rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/BaseDao.py
--rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/ListDao.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.030530 pyva_framework-3.3.5/pyva/dto/
--rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/BaseDto.py
--rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/ListDto.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.031231 pyva_framework-3.3.5/pyva/entity/
--rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/BaseEntity.py
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/GeneralHumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/HumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)     2090 2024-05-23 06:15:22.000000 pyva_framework-3.3.5/pyva/entity/RequestLog.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/startupApp.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.034082 pyva_framework-3.3.5/pyva/util/
--rw-r--r--   0 szq        (501) staff       (20)     6683 2024-05-29 13:15:14.000000 pyva_framework-3.3.5/pyva/util/ConfigUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/DbUtil.py
--rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/DictUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/EntityUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/FileUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/IpUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     4024 2024-05-29 12:59:57.000000 pyva_framework-3.3.5/pyva/util/JsonUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1912 2024-05-29 12:30:08.000000 pyva_framework-3.3.5/pyva/util/LockerUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/MongoUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/NacosUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/PathUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/QrcodeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/RedisUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/TimeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.034858 pyva_framework-3.3.5/pyva_framework.egg-info/
--rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1705 2024-05-29 13:27:04.000000 pyva_framework-3.3.5/pyva_framework.egg-info/SOURCES.txt
--rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/dependency_links.txt
--rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/entry_points.txt
--rw-r--r--   0 szq        (501) staff       (20)      314 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/requires.txt
--rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/top_level.txt
--rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-29 13:27:04.035322 pyva_framework-3.3.5/setup.cfg
--rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-29 13:07:28.000000 pyva_framework-3.3.5/setup.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.760794 pyva_framework-3.3.6/
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.6/LICENSE
+-rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 14:00:48.760622 pyva_framework-3.3.6/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.6/README.md
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.750467 pyva_framework-3.3.6/pyva/
+-rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/Application.py
+-rw-r--r--   0 szq        (501) staff       (20)      742 2024-05-29 12:48:14.000000 pyva_framework-3.3.6/pyva/Global.py
+-rw-r--r--   0 szq        (501) staff       (20)     1091 2024-05-29 13:21:35.000000 pyva_framework-3.3.6/pyva/GlobalInit.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.750932 pyva_framework-3.3.6/pyva/cli/
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/cli/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/cli/main.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.751384 pyva_framework-3.3.6/pyva/client/
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/client/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.752252 pyva_framework-3.3.6/pyva/client/dingtalk/
+-rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkContactClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkOauth2Client.py
+-rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkRobotClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     6578 2024-05-29 13:05:02.000000 pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkYidaClient.py
+-rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/client/dingtalk/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.753552 pyva_framework-3.3.6/pyva/common/
+-rw-r--r--   0 szq        (501) staff       (20)     1023 2024-05-29 13:58:17.000000 pyva_framework-3.3.6/pyva/common/FastapiEvents.py
+-rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/common/FastapiException.py
+-rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/common/LoggerHandler.py
+-rw-r--r--   0 szq        (501) staff       (20)     3456 2024-05-29 13:06:00.000000 pyva_framework-3.3.6/pyva/common/RequestLogRoute.py
+-rw-r--r--   0 szq        (501) staff       (20)      146 2024-05-19 03:56:35.000000 pyva_framework-3.3.6/pyva/common/RequestLogStatusEnum.py
+-rw-r--r--   0 szq        (501) staff       (20)      135 2024-05-19 03:56:35.000000 pyva_framework-3.3.6/pyva/common/RequestLogTypeEnum.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/common/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.754819 pyva_framework-3.3.6/pyva/config/
+-rw-r--r--   0 szq        (501) staff       (20)     1129 2024-05-29 13:13:15.000000 pyva_framework-3.3.6/pyva/config/AppConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/DbConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/DingtalkConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/DingtalkRobotConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/FastapiConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/LoggingConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/MongoConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/NacosConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/RedisConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/config/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.755502 pyva_framework-3.3.6/pyva/dao/
+-rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dao/BaseDao.py
+-rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dao/ListDao.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dao/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.755883 pyva_framework-3.3.6/pyva/dto/
+-rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dto/BaseDto.py
+-rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dto/ListDto.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/dto/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.756722 pyva_framework-3.3.6/pyva/entity/
+-rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/entity/BaseEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/entity/GeneralHumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/entity/HumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     2090 2024-05-23 06:15:22.000000 pyva_framework-3.3.6/pyva/entity/RequestLog.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/entity/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/startupApp.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.759501 pyva_framework-3.3.6/pyva/util/
+-rw-r--r--   0 szq        (501) staff       (20)     6683 2024-05-29 13:15:14.000000 pyva_framework-3.3.6/pyva/util/ConfigUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/DbUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/DictUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/EntityUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/FileUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/IpUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4024 2024-05-29 12:59:57.000000 pyva_framework-3.3.6/pyva/util/JsonUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1912 2024-05-29 12:30:08.000000 pyva_framework-3.3.6/pyva/util/LockerUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/MongoUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/NacosUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/PathUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/QrcodeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/RedisUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/TimeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.6/pyva/util/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 14:00:48.760364 pyva_framework-3.3.6/pyva_framework.egg-info/
+-rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1705 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/entry_points.txt
+-rw-r--r--   0 szq        (501) staff       (20)      314 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/requires.txt
+-rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-29 14:00:48.000000 pyva_framework-3.3.6/pyva_framework.egg-info/top_level.txt
+-rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-29 14:00:48.760822 pyva_framework-3.3.6/setup.cfg
+-rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-29 13:58:44.000000 pyva_framework-3.3.6/setup.py
```

### Comparing `pyva_framework-3.3.5/LICENSE` & `pyva_framework-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/PKG-INFO` & `pyva_framework-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.5
+Version: 3.3.6
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyva_framework-3.3.5/README.md` & `pyva_framework-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/Application.py` & `pyva_framework-3.3.6/pyva/Application.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/Global.py` & `pyva_framework-3.3.6/pyva/Global.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/GlobalInit.py` & `pyva_framework-3.3.6/pyva/GlobalInit.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/cli/main.py` & `pyva_framework-3.3.6/pyva/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkContactClient.py` & `pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkContactClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkOauth2Client.py` & `pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkOauth2Client.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkRobotClient.py` & `pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkRobotClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkYidaClient.py` & `pyva_framework-3.3.6/pyva/client/dingtalk/DingtalkYidaClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/common/FastapiEvents.py` & `pyva_framework-3.3.6/pyva/common/FastapiEvents.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 
         if FastapiConfig.https:
             protocol = "https"
         else:
             protocol = "http"
 
         info = f"""启动于：{TimeUtil.getDatetimeStrNow()}
-{FastapiConfig.name} - {FastapiConfig.title}
-{FastapiConfig.description}
+{FastapiConfig.name} - {FastapiConfig.title}，{FastapiConfig.version}
 {logoText}
 Visit Root: {protocol}://localhost:{FastapiConfig.port}
 """
         if FastapiConfig.docs_url:
             info += f"Visit Docs: {protocol}://localhost:{FastapiConfig.port}{FastapiConfig.docs_url}"
 
         G.logger.warning(info)
 
     @staticmethod
     def shutdown():
         info = f"""停止于：{TimeUtil.getDatetimeStrNow()}
-{FastapiConfig.name} - {FastapiConfig.title}
+{FastapiConfig.name} - {FastapiConfig.title}，{FastapiConfig.version}
 """
         G.logger.warning(info)
```

### Comparing `pyva_framework-3.3.5/pyva/common/FastapiException.py` & `pyva_framework-3.3.6/pyva/common/FastapiException.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/common/LoggerHandler.py` & `pyva_framework-3.3.6/pyva/common/LoggerHandler.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/common/RequestLogRoute.py` & `pyva_framework-3.3.6/pyva/common/RequestLogRoute.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/AppConfig.py` & `pyva_framework-3.3.6/pyva/config/AppConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/DbConfig.py` & `pyva_framework-3.3.6/pyva/config/DbConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/DingtalkConfig.py` & `pyva_framework-3.3.6/pyva/config/DingtalkConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/FastapiConfig.py` & `pyva_framework-3.3.6/pyva/config/FastapiConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/LoggingConfig.py` & `pyva_framework-3.3.6/pyva/config/LoggingConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/config/NacosConfig.py` & `pyva_framework-3.3.6/pyva/config/NacosConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/dao/BaseDao.py` & `pyva_framework-3.3.6/pyva/dao/BaseDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/dao/ListDao.py` & `pyva_framework-3.3.6/pyva/dao/ListDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/dto/BaseDto.py` & `pyva_framework-3.3.6/pyva/dto/BaseDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/dto/ListDto.py` & `pyva_framework-3.3.6/pyva/dto/ListDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/entity/BaseEntity.py` & `pyva_framework-3.3.6/pyva/entity/BaseEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/entity/GeneralHumpEntity.py` & `pyva_framework-3.3.6/pyva/entity/GeneralHumpEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/entity/RequestLog.py` & `pyva_framework-3.3.6/pyva/entity/RequestLog.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/startupApp.py` & `pyva_framework-3.3.6/pyva/startupApp.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/ConfigUtil.py` & `pyva_framework-3.3.6/pyva/util/ConfigUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/DbUtil.py` & `pyva_framework-3.3.6/pyva/util/DbUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/DictUtil.py` & `pyva_framework-3.3.6/pyva/util/DictUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/EntityUtil.py` & `pyva_framework-3.3.6/pyva/util/EntityUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/FileUtil.py` & `pyva_framework-3.3.6/pyva/util/FileUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/IpUtil.py` & `pyva_framework-3.3.6/pyva/util/IpUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/JsonUtil.py` & `pyva_framework-3.3.6/pyva/util/JsonUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/LockerUtil.py` & `pyva_framework-3.3.6/pyva/util/LockerUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/MongoUtil.py` & `pyva_framework-3.3.6/pyva/util/MongoUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/NacosUtil.py` & `pyva_framework-3.3.6/pyva/util/NacosUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/PathUtil.py` & `pyva_framework-3.3.6/pyva/util/PathUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/QrcodeUtil.py` & `pyva_framework-3.3.6/pyva/util/QrcodeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/RedisUtil.py` & `pyva_framework-3.3.6/pyva/util/RedisUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva/util/TimeUtil.py` & `pyva_framework-3.3.6/pyva/util/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/pyva_framework.egg-info/PKG-INFO` & `pyva_framework-3.3.6/pyva_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.5
+Version: 3.3.6
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyva_framework-3.3.5/pyva_framework.egg-info/SOURCES.txt` & `pyva_framework-3.3.6/pyva_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.5/setup.py` & `pyva_framework-3.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     requirements = re.sub(r'(?m)#.*$', '', requirements)
 
 setuptools.setup(
     name="pyva-framework",
-    version="3.3.5",
+    version="3.3.6",
     author="Zhenqiang Sun",
     author_email="zhenqiang.sun@gmail.com",
     description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhenqiang-sun/pyva",
     packages=setuptools.find_packages(),
```

