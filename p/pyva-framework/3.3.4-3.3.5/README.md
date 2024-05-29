# Comparing `tmp/pyva_framework-3.3.4.tar.gz` & `tmp/pyva_framework-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva_framework-3.3.4.tar", last modified: Fri May 24 08:50:13 2024, max compression
+gzip compressed data, was "pyva_framework-3.3.5.tar", last modified: Wed May 29 13:27:04 2024, max compression
```

## Comparing `pyva_framework-3.3.4.tar` & `pyva_framework-3.3.5.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.714496 pyva_framework-3.3.4/
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/LICENSE
--rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-24 08:50:13.714257 pyva_framework-3.3.4/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.4/README.md
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.704948 pyva_framework-3.3.4/pyva/
--rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/Application.py
--rw-r--r--   0 szq        (501) staff       (20)      708 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/Global.py
--rw-r--r--   0 szq        (501) staff       (20)     1010 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/GlobalInit.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.705217 pyva_framework-3.3.4/pyva/cli/
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/cli/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/cli/main.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.705343 pyva_framework-3.3.4/pyva/client/
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.706842 pyva_framework-3.3.4/pyva/client/dingtalk/
--rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkContactClient.py
--rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkOauth2Client.py
--rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkRobotClient.py
--rw-r--r--   0 szq        (501) staff       (20)     5526 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkYidaClient.py
--rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/client/dingtalk/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.707349 pyva_framework-3.3.4/pyva/common/
--rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/FastapiEvents.py
--rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/FastapiException.py
--rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/LoggerHandler.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/common/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.708696 pyva_framework-3.3.4/pyva/config/
--rw-r--r--   0 szq        (501) staff       (20)     1069 2024-05-21 06:55:20.000000 pyva_framework-3.3.4/pyva/config/AppConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/DbConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/DingtalkConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/DingtalkRobotConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/FastapiConfig.py
--rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/LoggingConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/MongoConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/config/NacosConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/RedisConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/config/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.709244 pyva_framework-3.3.4/pyva/dao/
--rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dao/BaseDao.py
--rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dao/ListDao.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dao/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.709671 pyva_framework-3.3.4/pyva/dto/
--rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dto/BaseDto.py
--rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/dto/ListDto.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/dto/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.710225 pyva_framework-3.3.4/pyva/entity/
--rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/entity/BaseEntity.py
--rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/entity/GeneralHumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/entity/HumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/entity/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/startupApp.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.712984 pyva_framework-3.3.4/pyva/util/
--rw-r--r--   0 szq        (501) staff       (20)     5269 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/ConfigUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/DbUtil.py
--rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/DictUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/EntityUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/FileUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/IpUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2006 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/JsonUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2034 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/LockerUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/MongoUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/NacosUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/PathUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/QrcodeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/RedisUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-21 06:54:51.000000 pyva_framework-3.3.4/pyva/util/TimeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.4/pyva/util/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-24 08:50:13.713972 pyva_framework-3.3.4/pyva_framework.egg-info/
--rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1578 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/SOURCES.txt
--rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/dependency_links.txt
--rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/entry_points.txt
--rw-r--r--   0 szq        (501) staff       (20)      307 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/requires.txt
--rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-24 08:50:13.000000 pyva_framework-3.3.4/pyva_framework.egg-info/top_level.txt
--rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-24 08:50:13.714533 pyva_framework-3.3.4/setup.cfg
--rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-24 08:44:20.000000 pyva_framework-3.3.4/setup.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.035290 pyva_framework-3.3.5/
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.5/LICENSE
+-rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 13:27:04.035090 pyva_framework-3.3.5/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.5/README.md
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025237 pyva_framework-3.3.5/pyva/
+-rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/Application.py
+-rw-r--r--   0 szq        (501) staff       (20)      742 2024-05-29 12:48:14.000000 pyva_framework-3.3.5/pyva/Global.py
+-rw-r--r--   0 szq        (501) staff       (20)     1091 2024-05-29 13:21:35.000000 pyva_framework-3.3.5/pyva/GlobalInit.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025718 pyva_framework-3.3.5/pyva/cli/
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/cli/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/cli/main.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.025976 pyva_framework-3.3.5/pyva/client/
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.027169 pyva_framework-3.3.5/pyva/client/dingtalk/
+-rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkContactClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkOauth2Client.py
+-rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkRobotClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     6578 2024-05-29 13:05:02.000000 pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkYidaClient.py
+-rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/client/dingtalk/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.028412 pyva_framework-3.3.5/pyva/common/
+-rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/FastapiEvents.py
+-rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/FastapiException.py
+-rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/LoggerHandler.py
+-rw-r--r--   0 szq        (501) staff       (20)     3456 2024-05-29 13:06:00.000000 pyva_framework-3.3.5/pyva/common/RequestLogRoute.py
+-rw-r--r--   0 szq        (501) staff       (20)      146 2024-05-19 03:56:35.000000 pyva_framework-3.3.5/pyva/common/RequestLogStatusEnum.py
+-rw-r--r--   0 szq        (501) staff       (20)      135 2024-05-19 03:56:35.000000 pyva_framework-3.3.5/pyva/common/RequestLogTypeEnum.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/common/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.029758 pyva_framework-3.3.5/pyva/config/
+-rw-r--r--   0 szq        (501) staff       (20)     1129 2024-05-29 13:13:15.000000 pyva_framework-3.3.5/pyva/config/AppConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DbConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DingtalkConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/DingtalkRobotConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/FastapiConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/LoggingConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/MongoConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/NacosConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/RedisConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/config/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.030176 pyva_framework-3.3.5/pyva/dao/
+-rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/BaseDao.py
+-rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/ListDao.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dao/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.030530 pyva_framework-3.3.5/pyva/dto/
+-rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/BaseDto.py
+-rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/ListDto.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/dto/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.031231 pyva_framework-3.3.5/pyva/entity/
+-rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/BaseEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/GeneralHumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/HumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     2090 2024-05-23 06:15:22.000000 pyva_framework-3.3.5/pyva/entity/RequestLog.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/entity/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/startupApp.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.034082 pyva_framework-3.3.5/pyva/util/
+-rw-r--r--   0 szq        (501) staff       (20)     6683 2024-05-29 13:15:14.000000 pyva_framework-3.3.5/pyva/util/ConfigUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/DbUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/DictUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/EntityUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/FileUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/IpUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4024 2024-05-29 12:59:57.000000 pyva_framework-3.3.5/pyva/util/JsonUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1912 2024-05-29 12:30:08.000000 pyva_framework-3.3.5/pyva/util/LockerUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/MongoUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/NacosUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/PathUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/QrcodeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/RedisUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/TimeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-27 02:31:25.000000 pyva_framework-3.3.5/pyva/util/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-29 13:27:04.034858 pyva_framework-3.3.5/pyva_framework.egg-info/
+-rw-r--r--   0 szq        (501) staff       (20)     2471 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1705 2024-05-29 13:27:04.000000 pyva_framework-3.3.5/pyva_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/entry_points.txt
+-rw-r--r--   0 szq        (501) staff       (20)      314 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/requires.txt
+-rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-29 13:27:03.000000 pyva_framework-3.3.5/pyva_framework.egg-info/top_level.txt
+-rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-29 13:27:04.035322 pyva_framework-3.3.5/setup.cfg
+-rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-29 13:07:28.000000 pyva_framework-3.3.5/setup.py
```

### Comparing `pyva_framework-3.3.4/LICENSE` & `pyva_framework-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/PKG-INFO` & `pyva_framework-3.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.4
+Version: 3.3.5
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.111.0
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: uvicorn==0.30.0
 Requires-Dist: SQLAlchemy==2.0.30
-Requires-Dist: PyMySQL==1.1.0
-Requires-Dist: sqlacodegen==2.3.0
-Requires-Dist: redis==5.0.4
+Requires-Dist: PyMySQL==1.1.1
+Requires-Dist: sqlacodegen==3.0.0rc5
+Requires-Dist: redis==5.1.0b5
 Requires-Dist: requests==2.32.1
 Requires-Dist: pyhumps==3.8.0
 Requires-Dist: nacos-sdk-python==0.1.14
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: pymongo==4.7.2
 Requires-Dist: orjson==3.10.3
-Requires-Dist: openpyxl==3.1.2
+Requires-Dist: openpyxl==3.2.0b1
 Requires-Dist: deprecated==1.2.14
 Requires-Dist: jinja2==3.1.4
 Requires-Dist: typer[all]==0.12.3
 Requires-Dist: py-ulid==1.0.3
 
 # PyVa
 PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
```

### Comparing `pyva_framework-3.3.4/README.md` & `pyva_framework-3.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/Application.py` & `pyva_framework-3.3.5/pyva/Application.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/Global.py` & `pyva_framework-3.3.5/pyva/Global.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 class G:
     # 运行模式：是否Debug模式
     debug: bool = False
     # 运行环境
     env: str = None
     # 运行目录
     path: str = None
+    # 运行IP
+    ip: str = None
     # 静态资源路径
     staticPath: str = None
     # 临时文件路径
     temporaryPath: str = None
     # 静态资源路径
     resPath: str = None
     # 静态资源路径
```

### Comparing `pyva_framework-3.3.4/pyva/GlobalInit.py` & `pyva_framework-3.3.5/pyva/GlobalInit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 
 from pyva.Global import G
 from pyva.common.LoggerHandler import LoggingHandler
+from pyva.util.IpUtil import IpUtil
 
 
 def GlobalInit(AppConfig):
     G.logger.info("GlobalInit")
 
     if G.isInitialized:
         G.logger.info("GlobalInit-isInitialized")
@@ -26,14 +27,16 @@
     G.staticPath = G.path + os.sep + "static"
     # 模板文件路径
     G.templatesPath = G.path + os.sep + "templates"
     # 临时文件路径
     G.temporaryPath = G.path + os.sep + "temporary"
     # 静态资源路径
     G.resPath = AppConfig.rootPath + os.sep + "res"
+    # 运行IP
+    G.ip = IpUtil.getHostIp()
 
     # 配置日志处理器
     G.logger.addHandler(LoggingHandler())
 
     # G初始化完成
     G.isInitialized = True
```

### Comparing `pyva_framework-3.3.4/pyva/cli/main.py` & `pyva_framework-3.3.5/pyva/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkContactClient.py` & `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkContactClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkOauth2Client.py` & `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkOauth2Client.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkRobotClient.py` & `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkRobotClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/client/dingtalk/DingtalkYidaClient.py` & `pyva_framework-3.3.5/pyva/client/dingtalk/DingtalkYidaClient.py`

 * *Files 13% similar despite different names*

```diff
@@ -180,7 +180,38 @@
         data = self.oauth.post(url=url, json=body)
 
         if not data:
             return True
         else:
             logger.warning(data)
             return False
+
+    def searchInstances(self, formUuid: str, searchFieldJson: str = None, currentPage: int = None, pageSize: int = None):
+        """
+        查询表单实例数据新版S
+
+        :doc https://open-dev.dingtalk.com/apiExplorer#/?devType=org&api=yida_1.0%23SearchFormDatas
+        :param formUuid 表单UUID
+        :param searchFieldJson 根据表单内组件值查询
+        :param currentPage 分页参数，当前页。
+        :param pageSize 分页参数，每页显示条数。
+        """
+
+        url = self.apiUrlRoot + "/v1.0/yida/forms/instances/search"
+
+        body = {
+            "appType": self.appType,
+            "systemToken": self.systemToken,
+            "userId": self.userId,
+            "formUuid": formUuid,
+            "searchFieldJson": searchFieldJson,
+            "currentPage": currentPage,
+            "pageSize": pageSize,
+        }
+
+        data = self.oauth.post(url=url, json=body)
+
+        if "totalCount" in data:
+            return data
+        else:
+            logger.warning(data)
+            return None
```

### Comparing `pyva_framework-3.3.4/pyva/common/FastapiEvents.py` & `pyva_framework-3.3.5/pyva/common/FastapiEvents.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/common/FastapiException.py` & `pyva_framework-3.3.5/pyva/common/FastapiException.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/common/LoggerHandler.py` & `pyva_framework-3.3.5/pyva/common/LoggerHandler.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/config/AppConfig.py` & `pyva_framework-3.3.5/pyva/config/AppConfig.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,10 +33,12 @@
     # 运行进程数：debug模式则默认为1，非debug模式按照配置进行启动
     workers: int = 2
     # token有效秒数
     tokenExpire: int = 86400
     # log输出至钉钉
     log2dingtalk: bool = False
     # 安全模式：是否启用HTTPS
-    https = False
+    https: bool = False
     # 访问限制Token
     accessToken: str = ""
+    # 配置文件缓存
+    configCache: bool = True
```

### Comparing `pyva_framework-3.3.4/pyva/config/DbConfig.py` & `pyva_framework-3.3.5/pyva/config/DbConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/config/DingtalkConfig.py` & `pyva_framework-3.3.5/pyva/config/DingtalkConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/config/FastapiConfig.py` & `pyva_framework-3.3.5/pyva/config/FastapiConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/config/LoggingConfig.py` & `pyva_framework-3.3.5/pyva/config/LoggingConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/config/NacosConfig.py` & `pyva_framework-3.3.5/pyva/config/NacosConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/dao/BaseDao.py` & `pyva_framework-3.3.5/pyva/dao/BaseDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/dao/ListDao.py` & `pyva_framework-3.3.5/pyva/dao/ListDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/dto/BaseDto.py` & `pyva_framework-3.3.5/pyva/dto/BaseDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/dto/ListDto.py` & `pyva_framework-3.3.5/pyva/dto/ListDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/entity/BaseEntity.py` & `pyva_framework-3.3.5/pyva/entity/BaseEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/entity/GeneralHumpEntity.py` & `pyva_framework-3.3.5/pyva/entity/GeneralHumpEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/startupApp.py` & `pyva_framework-3.3.5/pyva/startupApp.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/ConfigUtil.py` & `pyva_framework-3.3.5/pyva/util/ConfigUtil.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 
 import yaml
 from humps.main import pascalize
 
 from pyva.Global import G
 from pyva.util.DictUtil import DictUtil
+from pyva.util.JsonUtil import JsonUtil
 from pyva.util.NacosUtil import NacosUtil
 
 
 class ConfigUtil:
     """
     配置工具类，读取配置、合并配置等
 
@@ -126,15 +127,15 @@
 
         Args:
             srcPath (str): 源路径
             applicationConfig (object): 应用配置对象
             serviceEnabled (bool, optional): Nacos服务是否启用，默认为True
         """
 
-        if not hasattr(applicationConfig, "nacos"):
+        if not applicationConfig.get("nacos"):
             return
 
         NacosConfig = ConfigUtil.importConfig(srcPath, "nacos")
 
         if NacosConfig:
             ConfigUtil.updateConfig(NacosConfig, applicationConfig.get("nacos"))
 
@@ -152,24 +153,71 @@
         初始化启动配置
 
         Args:
             AppConfig (object): 应用配置对象
         """
         applicationConfig = ConfigUtil.readApplicationConfigByYaml(AppConfig)
         ConfigUtil.readApplicationConfigByNacos(AppConfig.srcPath, applicationConfig, False)
+
+        if AppConfig.configCache:
+            ConfigUtil.saveTemporary(AppConfig, applicationConfig)
+
         ConfigUtil.updateConfig(AppConfig, applicationConfig.get("app"))
 
     @staticmethod
     def initConfigForGlobal(AppConfig):
         """
         初始化全局配置
 
         Args:
             AppConfig (object): 应用配置对象
         """
-        applicationConfig = ConfigUtil.readApplicationConfigByYaml(AppConfig)
-        ConfigUtil.readApplicationConfigByNacos(AppConfig.srcPath, applicationConfig)
+
+        if AppConfig.configCache:
+            applicationConfig = ConfigUtil.readTemporary(AppConfig)
+        else:
+            applicationConfig = None
+
+        if not applicationConfig:
+            applicationConfig = ConfigUtil.readApplicationConfigByYaml(AppConfig)
+            ConfigUtil.readApplicationConfigByNacos(AppConfig.srcPath, applicationConfig)
 
         for key, value in applicationConfig.items():
             configClass = ConfigUtil.importConfig(AppConfig.srcPath, key)
             if configClass:
                 ConfigUtil.updateConfig(configClass, value)
+
+    @staticmethod
+    def getTemporaryFilePath(AppConfig):
+        filePath = f"{AppConfig.srcPath}{os.sep}temporary{os.sep}application-tmp.json"
+        return filePath
+
+    @staticmethod
+    def saveTemporary(AppConfig, applicationConfig):
+        filePath = ConfigUtil.getTemporaryFilePath(AppConfig)
+
+        # 打开一个文件以追加内容，如果文件不存在则创建它
+        with open(filePath, 'w') as file:
+            # 向文件中追加内容
+            file.write(JsonUtil.encode(applicationConfig))
+
+    @staticmethod
+    def readTemporary(AppConfig):
+        filePath = ConfigUtil.getTemporaryFilePath(AppConfig)
+
+        if not os.path.exists(filePath):
+            return None
+
+        with open(filePath, 'r') as file:
+            # 读取文件的全部内容
+            content = file.read()
+
+        return JsonUtil.decode(content)
+
+    @staticmethod
+    def deleteTemporary(AppConfig):
+        filePath = ConfigUtil.getTemporaryFilePath(AppConfig)
+
+        if not os.path.exists(filePath):
+            return None
+
+        os.remove(filePath)
```

### Comparing `pyva_framework-3.3.4/pyva/util/DbUtil.py` & `pyva_framework-3.3.5/pyva/util/DbUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/DictUtil.py` & `pyva_framework-3.3.5/pyva/util/DictUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/EntityUtil.py` & `pyva_framework-3.3.5/pyva/util/EntityUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/FileUtil.py` & `pyva_framework-3.3.5/pyva/util/FileUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/IpUtil.py` & `pyva_framework-3.3.5/pyva/util/IpUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/LockerUtil.py` & `pyva_framework-3.3.5/pyva/util/LockerUtil.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,27 +42,21 @@
 
         返回值：
         - 如果存在锁，返回锁的值；否则返回None
         """
         return self.redis.getString(self.getFullKey(key))
 
     def hasLocked(self, key: str):
-        warn("请使用新方法：isLocked", DeprecationWarning)
         """
         判断是否存在锁（已废弃，请使用isLocked方法）
-
-        参数：
-        - key: 锁键名
-
-        返回值：
-        - 如果存在锁，返回锁的值；否则返回None
         """
+        warn("请使用新方法：isLocked", DeprecationWarning)
         return self.isLocked(key)
 
-    def lock(self, key: str, expiration=None):
+    def lock(self, key: str, expiration: int = 3600):
         """
         加锁
 
         参数：
         - key: 锁键名
         - expiration: 锁的过期时间（可选）
```

### Comparing `pyva_framework-3.3.4/pyva/util/MongoUtil.py` & `pyva_framework-3.3.5/pyva/util/MongoUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/NacosUtil.py` & `pyva_framework-3.3.5/pyva/util/NacosUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/PathUtil.py` & `pyva_framework-3.3.5/pyva/util/PathUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/QrcodeUtil.py` & `pyva_framework-3.3.5/pyva/util/QrcodeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/RedisUtil.py` & `pyva_framework-3.3.5/pyva/util/RedisUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva/util/TimeUtil.py` & `pyva_framework-3.3.5/pyva/util/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.4/pyva_framework.egg-info/PKG-INFO` & `pyva_framework-3.3.5/pyva_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.4
+Version: 3.3.5
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: fastapi==0.111.0
-Requires-Dist: uvicorn==0.29.0
+Requires-Dist: uvicorn==0.30.0
 Requires-Dist: SQLAlchemy==2.0.30
-Requires-Dist: PyMySQL==1.1.0
-Requires-Dist: sqlacodegen==2.3.0
-Requires-Dist: redis==5.0.4
+Requires-Dist: PyMySQL==1.1.1
+Requires-Dist: sqlacodegen==3.0.0rc5
+Requires-Dist: redis==5.1.0b5
 Requires-Dist: requests==2.32.1
 Requires-Dist: pyhumps==3.8.0
 Requires-Dist: nacos-sdk-python==0.1.14
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: pymongo==4.7.2
 Requires-Dist: orjson==3.10.3
-Requires-Dist: openpyxl==3.1.2
+Requires-Dist: openpyxl==3.2.0b1
 Requires-Dist: deprecated==1.2.14
 Requires-Dist: jinja2==3.1.4
 Requires-Dist: typer[all]==0.12.3
 Requires-Dist: py-ulid==1.0.3
 
 # PyVa
 PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
```

### Comparing `pyva_framework-3.3.4/pyva_framework.egg-info/SOURCES.txt` & `pyva_framework-3.3.5/pyva_framework.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 pyva/client/dingtalk/DingtalkOauth2Client.py
 pyva/client/dingtalk/DingtalkRobotClient.py
 pyva/client/dingtalk/DingtalkYidaClient.py
 pyva/client/dingtalk/__init__.py
 pyva/common/FastapiEvents.py
 pyva/common/FastapiException.py
 pyva/common/LoggerHandler.py
+pyva/common/RequestLogRoute.py
+pyva/common/RequestLogStatusEnum.py
+pyva/common/RequestLogTypeEnum.py
 pyva/common/__init__.py
 pyva/config/AppConfig.py
 pyva/config/DbConfig.py
 pyva/config/DingtalkConfig.py
 pyva/config/DingtalkRobotConfig.py
 pyva/config/FastapiConfig.py
 pyva/config/LoggingConfig.py
@@ -33,14 +36,15 @@
 pyva/dao/__init__.py
 pyva/dto/BaseDto.py
 pyva/dto/ListDto.py
 pyva/dto/__init__.py
 pyva/entity/BaseEntity.py
 pyva/entity/GeneralHumpEntity.py
 pyva/entity/HumpEntity.py
+pyva/entity/RequestLog.py
 pyva/entity/__init__.py
 pyva/util/ConfigUtil.py
 pyva/util/DbUtil.py
 pyva/util/DictUtil.py
 pyva/util/EntityUtil.py
 pyva/util/FileUtil.py
 pyva/util/IpUtil.py
```

### Comparing `pyva_framework-3.3.4/setup.py` & `pyva_framework-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     requirements = re.sub(r'(?m)#.*$', '', requirements)
 
 setuptools.setup(
     name="pyva-framework",
-    version="3.3.4",
+    version="3.3.5",
     author="Zhenqiang Sun",
     author_email="zhenqiang.sun@gmail.com",
     description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhenqiang-sun/pyva",
     packages=setuptools.find_packages(),
```

