# Comparing `tmp/bot_station-0.5.2.tar.gz` & `tmp/bot_station-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bot_station-0.5.2.tar", last modified: Mon May 13 20:36:11 2024, max compression
+gzip compressed data, was "bot_station-0.6.0.tar", last modified: Wed May 29 19:35:30 2024, max compression
```

## Comparing `bot_station-0.5.2.tar` & `bot_station-0.6.0.tar`

### file list

```diff
@@ -1,84 +1,100 @@
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198849 bot_station-0.5.2/
--rw-r--r--   0 mmarashan (1826057312) 593637566     1070 2024-05-05 19:58:38.000000 bot_station-0.5.2/LICENSE
--rw-r--r--   0 mmarashan (1826057312) 593637566      750 2024-05-13 20:36:11.198642 bot_station-0.5.2/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566       60 2024-05-13 20:36:00.000000 bot_station-0.5.2/README.md
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.181613 bot_station-0.5.2/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.182342 bot_station-0.5.2/bot_station/api/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.182554 bot_station-0.5.2/bot_station/api/rest/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     7837 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/api/rest/api.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184364 bot_station-0.5.2/bot_station/api/rest/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      257 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_call_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      331 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      482 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_creation_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      126 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_creation_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      433 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      401 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_train_dto.py
--rw-r--r--   0 mmarashan (1826057312) 593637566       90 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/bot_train_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      204 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/api/rest/model/web_app_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184494 bot_station-0.5.2/bot_station/data/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184584 bot_station-0.5.2/bot_station/data/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.184947 bot_station-0.5.2/bot_station/data/base/database/
--rw-r--r--   0 mmarashan (1826057312) 593637566      975 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/UUID.py
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      428 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/base/database/base_db_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.185487 bot_station-0.5.2/bot_station/data/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1291 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/data/bot/bot_factory_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     8108 2024-05-13 20:34:22.000000 bot_station-0.5.2/bot_station/data/bot/bot_impl.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2169 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/chat_message_storage_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.185727 bot_station-0.5.2/bot_station/data/bot/mapper/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/mapper/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      972 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/data/bot/mapper/document_mapper.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.186381 bot_station-0.5.2/bot_station/data/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      124 2024-05-10 19:41:12.000000 bot_station-0.5.2/bot_station/data/bot/model/qdrant_config.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      128 2024-05-10 19:41:18.000000 bot_station-0.5.2/bot_station/data/bot/model/yandex_cloud_config.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.186917 bot_station-0.5.2/bot_station/data/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566      508 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     3431 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/data/bot_station/bot_registry_impl.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187266 bot_station-0.5.2/bot_station/data/bot_station/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/data/bot_station/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      853 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/data/bot_station/model/bot_info_dto.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187624 bot_station-0.5.2/bot_station/di/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/di/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1529 2024-05-10 19:53:19.000000 bot_station-0.5.2/bot_station/di/bot_station_module.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.187876 bot_station-0.5.2/bot_station/domain/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/__init__.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.193861 bot_station-0.5.2/bot_station/domain/base/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/base/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      605 2024-05-10 20:00:38.000000 bot_station-0.5.2/bot_station/domain/base/const.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      391 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/base/utils.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.194905 bot_station-0.5.2/bot_station/domain/bot/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      970 2024-05-12 11:00:18.000000 bot_station-0.5.2/bot_station/domain/bot/bot.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      260 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot/bot_factory.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      798 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/chat_message_storage.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.196815 bot_station-0.5.2/bot_station/domain/bot/model/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      348 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot/model/bot_meta_info.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      222 2024-05-08 19:40:03.000000 bot_station-0.5.2/bot_station/domain/bot/model/document.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      254 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_call_result.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      361 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_chat_message.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      379 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot/model/lm_train_data.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.197384 bot_station-0.5.2/bot_station/domain/bot_station/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/bot_station/domain/bot_station/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566      571 2024-05-10 21:06:41.000000 bot_station-0.5.2/bot_station/domain/bot_station/bot_registry.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     2981 2024-05-12 11:02:36.000000 bot_station-0.5.2/bot_station/domain/bot_station/bot_station.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198396 bot_station-0.5.2/bot_station.egg-info/
--rw-r--r--   0 mmarashan (1826057312) 593637566      750 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/PKG-INFO
--rw-r--r--   0 mmarashan (1826057312) 593637566     2295 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/SOURCES.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566        1 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/dependency_links.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566      190 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/requires.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       18 2024-05-13 20:36:11.000000 bot_station-0.5.2/bot_station.egg-info/top_level.txt
--rw-r--r--   0 mmarashan (1826057312) 593637566       38 2024-05-13 20:36:11.198894 bot_station-0.5.2/setup.cfg
--rw-r--r--   0 mmarashan (1826057312) 593637566      834 2024-05-08 19:40:03.000000 bot_station-0.5.2/setup.py
-drwxr-xr-x   0 mmarashan (1826057312) 593637566        0 2024-05-13 20:36:11.198041 bot_station-0.5.2/tests/
--rw-r--r--   0 mmarashan (1826057312) 593637566        0 2024-05-05 19:58:38.000000 bot_station-0.5.2/tests/__init__.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     5606 2024-05-12 11:21:25.000000 bot_station-0.5.2/tests/bot_station_api_test.py
--rw-r--r--   0 mmarashan (1826057312) 593637566     1426 2024-05-12 11:03:13.000000 bot_station-0.5.2/tests/test_bot_factory.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.704303 bot_station-0.6.0/
+-rw-r--r--   0 mrmx       (501) staff       (20)     1070 2024-03-22 14:52:19.000000 bot_station-0.6.0/LICENSE
+-rw-r--r--   0 mrmx       (501) staff       (20)      744 2024-05-29 19:35:30.703463 bot_station-0.6.0/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)       85 2024-05-29 19:34:47.000000 bot_station-0.6.0/README.md
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.643928 bot_station-0.6.0/bot_station/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-11 19:43:09.000000 bot_station-0.6.0/bot_station/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.647786 bot_station-0.6.0/bot_station/api/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-03 18:22:56.000000 bot_station-0.6.0/bot_station/api/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.648708 bot_station-0.6.0/bot_station/api/rest/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-10 19:25:54.000000 bot_station-0.6.0/bot_station/api/rest/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     7482 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/api/rest/api.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.656464 bot_station-0.6.0/bot_station/api/rest/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-10 19:34:11.000000 bot_station-0.6.0/bot_station/api/rest/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      257 2024-03-15 15:56:43.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_call_dto.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      332 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_call_result.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      482 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_creation_dto.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      126 2024-03-16 18:20:34.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_creation_result.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      433 2024-04-25 19:15:25.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_dto.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      351 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/api/rest/model/bot_train_dto.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      204 2024-04-19 19:29:57.000000 bot_station-0.6.0/bot_station/api/rest/model/web_app_config.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.657454 bot_station-0.6.0/bot_station/data/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-01-17 19:01:12.000000 bot_station-0.6.0/bot_station/data/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.657957 bot_station-0.6.0/bot_station/data/base/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-05 19:09:37.000000 bot_station-0.6.0/bot_station/data/base/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.660302 bot_station-0.6.0/bot_station/data/base/database/
+-rw-r--r--   0 mrmx       (501) staff       (20)      975 2024-03-07 19:18:06.000000 bot_station-0.6.0/bot_station/data/base/database/UUID.py
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-07 18:45:55.000000 bot_station-0.6.0/bot_station/data/base/database/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      428 2024-03-10 19:14:29.000000 bot_station-0.6.0/bot_station/data/base/database/base_db_dto.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.663753 bot_station-0.6.0/bot_station/data/bot/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-01-22 19:10:59.000000 bot_station-0.6.0/bot_station/data/bot/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     1904 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot/bot_factory_impl.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3412 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot/bot_impl.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     2169 2024-05-01 11:02:16.000000 bot_station-0.6.0/bot_station/data/bot/chat_message_storage_impl.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.666466 bot_station-0.6.0/bot_station/data/bot/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-01 11:20:14.000000 bot_station-0.6.0/bot_station/data/bot/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      124 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot/model/qdrant_config.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      128 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot/model/yandex_cloud_config.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.668631 bot_station-0.6.0/bot_station/data/bot_station/
+-rw-r--r--   0 mrmx       (501) staff       (20)      510 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot_station/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3432 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot_station/bot_registry_impl.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.670126 bot_station-0.6.0/bot_station/data/bot_station/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-05 19:21:19.000000 bot_station-0.6.0/bot_station/data/bot_station/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      853 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/bot_station/model/bot_info_dto.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.672806 bot_station-0.6.0/bot_station/data/docs/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/docs/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.674246 bot_station-0.6.0/bot_station/data/docs/mapper/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/docs/mapper/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      482 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/docs/mapper/document_mapper.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     2178 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/docs/qdrant_docs_iterator.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3860 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/docs/qdrant_docs_library.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.675901 bot_station-0.6.0/bot_station/data/llm/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/llm/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      853 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/data/llm/yandex_gpt_llm.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.677780 bot_station-0.6.0/bot_station/di/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-03-12 19:30:25.000000 bot_station-0.6.0/bot_station/di/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     1603 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/di/bot_station_module.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.678780 bot_station-0.6.0/bot_station/domain/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-01-17 19:01:05.000000 bot_station-0.6.0/bot_station/domain/__init__.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.681097 bot_station-0.6.0/bot_station/domain/base/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-05 19:58:44.000000 bot_station-0.6.0/bot_station/domain/base/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      544 2024-05-01 11:28:39.000000 bot_station-0.6.0/bot_station/domain/base/const.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      391 2024-05-01 11:17:18.000000 bot_station-0.6.0/bot_station/domain/base/utils.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.684584 bot_station-0.6.0/bot_station/domain/bot/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-01-22 19:10:26.000000 bot_station-0.6.0/bot_station/domain/bot/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      472 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot/bot.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      260 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot/bot_factory.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      798 2024-05-01 11:02:16.000000 bot_station-0.6.0/bot_station/domain/bot/chat_message_storage.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.688511 bot_station-0.6.0/bot_station/domain/bot/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-01-17 19:05:53.000000 bot_station-0.6.0/bot_station/domain/bot/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      348 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot/model/bot_meta_info.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      255 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot/model/lm_call_result.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      361 2024-05-01 11:02:16.000000 bot_station-0.6.0/bot_station/domain/bot/model/lm_chat_message.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.690855 bot_station-0.6.0/bot_station/domain/bot_station/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-02-05 18:50:26.000000 bot_station-0.6.0/bot_station/domain/bot_station/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      571 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot_station/bot_registry.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3067 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/bot_station/bot_station.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.694660 bot_station-0.6.0/bot_station/domain/docs/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      779 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/docs_library.py
+-rw-r--r--   0 mrmx       (501) staff       (20)       63 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/docs_library_provider.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      249 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/docs_source.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.695993 bot_station-0.6.0/bot_station/domain/docs/model/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/model/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      277 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/docs/model/document.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.697554 bot_station-0.6.0/bot_station/domain/llm/
+-rw-r--r--   0 mrmx       (501) staff       (20)        0 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/llm/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      133 2024-05-27 19:20:39.000000 bot_station-0.6.0/bot_station/domain/llm/llm.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.702479 bot_station-0.6.0/bot_station.egg-info/
+-rw-r--r--   0 mrmx       (501) staff       (20)      744 2024-05-29 19:35:30.000000 bot_station-0.6.0/bot_station.egg-info/PKG-INFO
+-rw-r--r--   0 mrmx       (501) staff       (20)     2691 2024-05-29 19:35:30.000000 bot_station-0.6.0/bot_station.egg-info/SOURCES.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)        1 2024-05-29 19:35:30.000000 bot_station-0.6.0/bot_station.egg-info/dependency_links.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)      174 2024-05-29 19:35:30.000000 bot_station-0.6.0/bot_station.egg-info/requires.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       18 2024-05-29 19:35:30.000000 bot_station-0.6.0/bot_station.egg-info/top_level.txt
+-rw-r--r--   0 mrmx       (501) staff       (20)       38 2024-05-29 19:35:30.704467 bot_station-0.6.0/setup.cfg
+-rw-r--r--   0 mrmx       (501) staff       (20)      834 2024-05-27 19:20:39.000000 bot_station-0.6.0/setup.py
+drwxr-xr-x   0 mrmx       (501) staff       (20)        0 2024-05-29 19:35:30.701425 bot_station-0.6.0/tests/
+-rw-r--r--   0 mrmx       (501) staff       (20)      189 2024-05-27 19:20:39.000000 bot_station-0.6.0/tests/__init__.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     5943 2024-05-27 19:20:39.000000 bot_station-0.6.0/tests/bot_station_api_test.py
+-rw-r--r--   0 mrmx       (501) staff       (20)     3766 2024-05-27 19:20:39.000000 bot_station-0.6.0/tests/bot_station_test.py
+-rw-r--r--   0 mrmx       (501) staff       (20)      243 2024-05-27 19:20:39.000000 bot_station-0.6.0/tests/mock_llm.py
```

### Comparing `bot_station-0.5.2/LICENSE` & `bot_station-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/PKG-INFO` & `bot_station-0.6.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.2
+Version: 0.6.0
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
-Requires-Dist: qdrant-client==1.9.0
+Requires-Dist: qdrant-client==1.9.1
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
-Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.2
-What's new: Fix empty docs in prompt
+# Bot Station SDK 0.6.0
+What's new: Availability to load all docs from knowledge base
```

### Comparing `bot_station-0.5.2/bot_station/api/rest/api.py` & `bot_station-0.6.0/bot_station/api/rest/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,24 +9,21 @@
 from bot_station.api.rest.model.bot_call_dto import BotCallDto
 from bot_station.api.rest.model.bot_call_result import (
     BotCallResult,
     BotNotFoundCallResult,
     BotAnswerCallResult,
 )
 from bot_station.api.rest.model.bot_creation_dto import BotInfoDto
-from bot_station.api.rest.model.bot_creation_result import BotCreationResult
 from bot_station.api.rest.model.bot_dto import BotDto
 from bot_station.api.rest.model.bot_train_dto import BotTrainDto
-from bot_station.api.rest.model.bot_train_result import BotTrainResult
 from bot_station.api.rest.model.web_app_config import WebAppConfig
 from bot_station.domain.bot.bot import Bot
-from bot_station.domain.bot.model.document import Document
+from bot_station.domain.docs.model.document import Document
 from bot_station.domain.bot.model.bot_meta_info import BotMetaInfo
 from bot_station.domain.bot.model.lm_chat_message import LMUserMessage
-from bot_station.domain.bot.model.lm_train_data import DocumentsTrainData
 from bot_station.domain.bot_station.bot_station import BotStation
 
 
 class LoggingRoute(APIRoute):
     def get_route_handler(self) -> Callable:
         original_route_handler = super().get_route_handler()
 
@@ -60,21 +57,22 @@
     bot_id: str | None = await BotStationWebApp.update(dto)
     if bot_id is not None:
         return Response(status_code=status.HTTP_200_OK)
     else:
         return Response(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR)
 
 
-@router.post("/train", status_code=200)
+@router.post("/train", status_code=200, description="Returns ID of new document")
 async def train(*, dto: BotTrainDto) -> Any:
     logging.debug(f"/train dto : {dto}")
-    result: BotTrainResult = await BotStationWebApp.train(dto)
-    if result is BotTrainResult.SUCCESS:
-        return Response(status_code=status.HTTP_200_OK)
-    if result is BotTrainResult.BOT_NOT_FOUND:
+    try:
+        doc: Document = await BotStationWebApp.train(dto)
+        return doc.id
+    except ValueError:
+        logging.debug(f"incorrect dto : {dto}")
         return Response(status_code=status.HTTP_404_NOT_FOUND)
 
 
 @router.post("/call", status_code=200, response_model=BotAnswerCallResult)
 async def call(*, dto: BotCallDto) -> Any:
     logging.debug(f"/call dto : {dto}")
     result: BotCallResult = await BotStationWebApp.call(dto)
@@ -157,32 +155,27 @@
             await BotStationWebApp.bot_station.update(meta_info)
             return meta_info.id
         except Exception as e:
             logging.warning(e)
             return None
 
     @staticmethod
-    async def train(dto: BotTrainDto) -> BotTrainResult:
+    async def train(dto: BotTrainDto) -> Document:
         bot: Bot | None = await BotStationWebApp.bot_station.get_bot(bot_id=dto.bot_id)
         if bot is None:
-            return BotTrainResult.BOT_NOT_FOUND
+            raise ValueError(f"Bot with id {dto.bot_id} not exist")
         else:
-            await bot.train(
-                DocumentsTrainData(
-                    docs=[
-                        Document(
-                            data=dto.data,
-                            id=dto.id,
-                            source_link=dto.source_link,
-                            metadata=dto.metadata,
-                        )
-                    ]
-                )
+            await bot.docs_library.load()
+            doc = await bot.docs_library.create_document(
+                data=dto.data,
+                source_link=dto.source_link,
+                metadata=dto.metadata,
             )
-            return BotTrainResult.SUCCESS
+            await bot.docs_library.close()
+            return doc
 
     @staticmethod
     async def call(dto: BotCallDto) -> BotCallResult:
         bot: Bot | None = await BotStationWebApp.bot_station.get_bot(bot_id=dto.bot_id)
         if bot is None:
             return BotNotFoundCallResult()
         else:
```

### Comparing `bot_station-0.5.2/bot_station/data/base/database/UUID.py` & `bot_station-0.6.0/bot_station/data/base/database/UUID.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/bot_station/data/bot/chat_message_storage_impl.py` & `bot_station-0.6.0/bot_station/data/bot/chat_message_storage_impl.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/bot_station/data/bot_station/bot_registry_impl.py` & `bot_station-0.6.0/bot_station/data/bot_station/bot_registry_impl.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bot_station.data.bot_station import db_path
 from bot_station.data.bot_station.model.bot_info_dto import BotInfoDto
 from bot_station.domain.bot_station.bot_registry import BotRegistry
 from bot_station.domain.bot.model.bot_meta_info import BotMetaInfo
 
 
 class BotRegistryImpl(BotRegistry):
-    __engine = create_engine(db_path, echo=True)
+    __engine = create_engine(db_path, echo=False)
     __storage = {}
 
     async def create(self, config: BotMetaInfo) -> BotMetaInfo:
         session = Session(self.__engine)
         dto = BotInfoDto(
             id=config.id,
             name=config.name,
```

### Comparing `bot_station-0.5.2/bot_station/data/bot_station/model/bot_info_dto.py` & `bot_station-0.6.0/bot_station/data/bot_station/model/bot_info_dto.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/bot_station/di/bot_station_module.py` & `bot_station-0.6.0/bot_station/di/bot_station_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,8 +30,11 @@
     def __get_bot_factory(
             env_config: YandexCloudConfig,
             qdrant_config: QdrantConfig,
     ) -> BotFactory:
         if BotStationModule.overrides_bot_factory is not None:
             return BotStationModule.overrides_bot_factory
         else:
-            return BotFactoryImpl(yandex_cloud_config=env_config, qdrant_config=qdrant_config)
+            factory = BotFactoryImpl()
+            factory.yandex_cloud_config = env_config
+            factory.qdrant_config = qdrant_config
+            return factory
```

### Comparing `bot_station-0.5.2/bot_station/domain/base/const.py` & `bot_station-0.6.0/bot_station/domain/base/const.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,8 +3,7 @@
             """
 
 # TODO: обернуть это и пути в ConfigProvider и передавать через конструктор
 data_folder_path = "./.data"
 databases_path = data_folder_path + "/database"
 message_history_path = data_folder_path + "/message_history"
 chat_files_path = data_folder_path + "/chat_files"
-embeddings_cache_dir = data_folder_path + "/embedings_cache"
```

### Comparing `bot_station-0.5.2/bot_station/domain/bot/chat_message_storage.py` & `bot_station-0.6.0/bot_station/domain/bot/chat_message_storage.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/bot_station/domain/bot_station/bot_registry.py` & `bot_station-0.6.0/bot_station/domain/bot_station/bot_registry.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/bot_station/domain/bot_station/bot_station.py` & `bot_station-0.6.0/bot_station/domain/bot_station/bot_station.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,38 +60,40 @@
             raise Exception("Bot id is None!")
         bot = self.__in_memory_bots.get(bot_id, None)
         if bot is not None:
             return bot
 
         meta = await self.bot_registry.get(bot_id)
         if meta is None:
-            logging.warning(f"No bot_station in registry {bot_id}")
+            logging.warning(f"No {bot_id} in registry!")
             return None
         else:
             bot = await self.bot_factory.create(meta=meta)
+            await bot.docs_library.load()
             self.__in_memory_bots[bot_id] = bot
             return bot
 
     async def get_bots_list(self) -> List[BotMetaInfo]:
         logging.debug("get_bots_list")
         return await self.bot_registry.get_all()
 
     async def delete(self, bot_id: str) -> bool:
         logging.debug(f"delete {bot_id}")
         bot = await self.get_bot(bot_id=bot_id)
         if bot is not None:
-            await bot.delete()
+            await bot.docs_library.load()
+            await bot.docs_library.clear()
             await self.bot_registry.delete(bot_id=bot_id)
             self.__in_memory_bots.pop(bot_id, None)
             return True
         else:
-            logging.warning(f"No bot_station in registry {bot_id}")
+            logging.warning(f"No {bot_id} in registry")
             return False
 
     async def update(self, info: BotMetaInfo):
         logging.debug(f"Update {info}")
         await self.bot_registry.update(info)
         # reload bot
         bot = self.__in_memory_bots.pop(info.id, None)
         if bot is not None:
             logging.debug(f"Close {bot.meta}")
-            await bot.close()
+            await bot.docs_library.close()
```

### Comparing `bot_station-0.5.2/bot_station.egg-info/PKG-INFO` & `bot_station-0.6.0/bot_station.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: bot_station
-Version: 0.5.2
+Version: 0.6.0
 Summary: Bot Station SDK + Web App
 Author: Maxim Marashan
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
 Requires-Dist: langchain==0.1.17
 Requires-Dist: langchain-community==0.0.36
-Requires-Dist: qdrant-client==1.9.0
+Requires-Dist: qdrant-client==1.9.1
 Requires-Dist: fastembed==0.2.7
 Requires-Dist: yandexcloud==0.271.0
-Requires-Dist: tiktoken==0.6.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: fastapi==0.110.3
 Requires-Dist: uvicorn==0.29.0
 
-# Bot Station SDK 0.5.2
-What's new: Fix empty docs in prompt
+# Bot Station SDK 0.6.0
+What's new: Availability to load all docs from knowledge base
```

### Comparing `bot_station-0.5.2/bot_station.egg-info/SOURCES.txt` & `bot_station-0.6.0/bot_station.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,49 +13,60 @@
 bot_station/api/rest/model/__init__.py
 bot_station/api/rest/model/bot_call_dto.py
 bot_station/api/rest/model/bot_call_result.py
 bot_station/api/rest/model/bot_creation_dto.py
 bot_station/api/rest/model/bot_creation_result.py
 bot_station/api/rest/model/bot_dto.py
 bot_station/api/rest/model/bot_train_dto.py
-bot_station/api/rest/model/bot_train_result.py
 bot_station/api/rest/model/web_app_config.py
 bot_station/data/__init__.py
 bot_station/data/base/__init__.py
 bot_station/data/base/database/UUID.py
 bot_station/data/base/database/__init__.py
 bot_station/data/base/database/base_db_dto.py
 bot_station/data/bot/__init__.py
 bot_station/data/bot/bot_factory_impl.py
 bot_station/data/bot/bot_impl.py
 bot_station/data/bot/chat_message_storage_impl.py
-bot_station/data/bot/mapper/__init__.py
-bot_station/data/bot/mapper/document_mapper.py
 bot_station/data/bot/model/__init__.py
 bot_station/data/bot/model/qdrant_config.py
 bot_station/data/bot/model/yandex_cloud_config.py
 bot_station/data/bot_station/__init__.py
 bot_station/data/bot_station/bot_registry_impl.py
 bot_station/data/bot_station/model/__init__.py
 bot_station/data/bot_station/model/bot_info_dto.py
+bot_station/data/docs/__init__.py
+bot_station/data/docs/qdrant_docs_iterator.py
+bot_station/data/docs/qdrant_docs_library.py
+bot_station/data/docs/mapper/__init__.py
+bot_station/data/docs/mapper/document_mapper.py
+bot_station/data/llm/__init__.py
+bot_station/data/llm/yandex_gpt_llm.py
 bot_station/di/__init__.py
 bot_station/di/bot_station_module.py
 bot_station/domain/__init__.py
 bot_station/domain/base/__init__.py
 bot_station/domain/base/const.py
 bot_station/domain/base/utils.py
 bot_station/domain/bot/__init__.py
 bot_station/domain/bot/bot.py
 bot_station/domain/bot/bot_factory.py
 bot_station/domain/bot/chat_message_storage.py
 bot_station/domain/bot/model/__init__.py
 bot_station/domain/bot/model/bot_meta_info.py
-bot_station/domain/bot/model/document.py
 bot_station/domain/bot/model/lm_call_result.py
 bot_station/domain/bot/model/lm_chat_message.py
-bot_station/domain/bot/model/lm_train_data.py
 bot_station/domain/bot_station/__init__.py
 bot_station/domain/bot_station/bot_registry.py
 bot_station/domain/bot_station/bot_station.py
+bot_station/domain/docs/__init__.py
+bot_station/domain/docs/docs_library.py
+bot_station/domain/docs/docs_library_provider.py
+bot_station/domain/docs/docs_source.py
+bot_station/domain/docs/model/__init__.py
+bot_station/domain/docs/model/document.py
+bot_station/domain/llm/__init__.py
+bot_station/domain/llm/llm.py
 tests/__init__.py
 tests/bot_station_api_test.py
-tests/test_bot_factory.py
+tests/bot_station_test.py
+tests/mock_llm.py
```

### Comparing `bot_station-0.5.2/setup.py` & `bot_station-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `bot_station-0.5.2/tests/bot_station_api_test.py` & `bot_station-0.6.0/tests/bot_station_api_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,62 @@
 import logging
 import unittest
 
 from fastapi.testclient import TestClient
 
 from bot_station.api.rest.api import BotStationWebApp
 from bot_station.api.rest.model.web_app_config import WebAppConfig
+from bot_station.data.bot.bot_factory_impl import BotFactoryImpl
 from bot_station.data.bot.model.qdrant_config import QdrantConfig
 from bot_station.data.bot.model.yandex_cloud_config import YandexCloudConfig
+from bot_station.data.docs.qdrant_docs_library import QdrantDocsLibrary
 from bot_station.di.bot_station_module import BotStationModule
-from bot_station.domain.bot.bot import Bot
+from bot_station.domain.bot.bot_factory import BotFactory
 from bot_station.domain.bot_station.bot_station import BotStation
-from test_bot_factory import TestBotFactory, TestBot
+from mock_llm import MockLLM
 
 logging.basicConfig(
     format="%(asctime)s.%(msecs)06f %(levelname)-8s [%(filename)s:%(lineno)d] %(message)s",
     datefmt="%d-%m-%Y:%H:%M:%S",
     level=logging.DEBUG,
 )
 
 
-def launch_test_web_app(bot: Bot):
+def launch_test_web_app(bot_factory: BotFactory):
     yandex_cloud_config = YandexCloudConfig(
         api_key="",
         folder_id="",
         model_name="",
     )
     qdrant_config = QdrantConfig(
         qdrant_url=None,
         qdrant_db_path=".data/qdrant",
     )
-    bot_factory = TestBotFactory()
-    bot_factory.set_bot(bot)
     BotStationModule.provide_bot_factory(bot_factory)
     test_bot_station: BotStation = BotStationModule.create_bot_station(yandex_cloud_config=yandex_cloud_config,
                                                                        qdrant_config=qdrant_config)
 
     BotStationWebApp.prepare(bot_station=test_bot_station, config=WebAppConfig())
 
 
 class BotStationApiTest(unittest.TestCase):
     bot_station_test_client: TestClient
-    mock_bot: TestBot
+    docs_library = QdrantDocsLibrary(
+        collection_name="",
+        qdrant_config=QdrantConfig(
+            qdrant_url=None,
+            qdrant_db_path="./.data/qdrant")
+    )
+    llm = MockLLM()
+    bot_factory = BotFactoryImpl()
+    bot_factory.docs_library = docs_library
+    bot_factory.llm = llm
 
     def setUp(self):
-        self.mock_bot = TestBot()
-        launch_test_web_app(self.mock_bot)
+        launch_test_web_app(self.bot_factory)
         self.bot_station_test_client = TestClient(BotStationWebApp.api)
 
     def create(self, bot_id: str, check_response: bool = False):
         response = self.bot_station_test_client.post(
             url="/create",
             json={
                 "id": bot_id,
@@ -73,30 +81,29 @@
     def test_train(self):
         bot_id = "test_train"
         self.create(bot_id=bot_id, check_response=False)
         response = self.bot_station_test_client.post(
             url="/train",
             json={
                 "bot_id": bot_id,
-                "id": "1",
                 "data": "FastAPI is a modern, fast, web framework for building APIs with Python.",
                 "source_link": "https://aaa.ru"
             }
         )
         self.assertEqual(200, response.status_code)
+        self.assertTrue(len(response.content) > 0)
         self.delete(bot_id=bot_id, check_response=True)
 
     def test_train_with_metadata(self):
         bot_id = "test_train_with_metadata"
         self.create(bot_id=bot_id, check_response=False)
         response = self.bot_station_test_client.post(
             url="/train",
             json={
                 "bot_id": bot_id,
-                "id": "1",
                 "data": "FastAPI is a modern, fast, web framework for building APIs with Python.",
                 "source_link": "https://aaa.ru",
                 "metadata": {"a": "b"}
             }
         )
         self.assertEqual(200, response.status_code)
         self.delete(bot_id=bot_id, check_response=True)
@@ -114,15 +121,15 @@
         self.assertEqual(404, response.status_code)
 
     def test_call(self):
         answer = "FastAPI is a modern, web framework"
 
         bot_id = "test_call"
         self.create(bot_id=bot_id, check_response=False)
-        self.mock_bot.set_next_answer(answer)
+        self.bot_factory.llm.set_next_answer(answer)
         response = self.bot_station_test_client.post(
             url="/call",
             json={
                 "bot_id": bot_id,
                 "chat_id": 1,
                 "data": "What is FastAPI?"
             }
```

