# Comparing `tmp/hume-0.5.1rc1.tar.gz` & `tmp/hume-0.6.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hume-0.5.1rc1.tar", max compression
+gzip compressed data, was "hume-0.6.0rc1.tar", max compression
```

## Comparing `hume-0.5.1rc1.tar` & `hume-0.6.0rc1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1070 2023-06-29 18:23:24.716306 hume-0.5.1rc1/LICENSE
--rw-r--r--   0        0        0     2256 2024-04-16 17:05:53.964549 hume-0.5.1rc1/README.md
--rw-r--r--   0        0        0      985 2024-04-30 12:10:05.693231 hume-0.5.1rc1/hume/__init__.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.724774 hume-0.5.1rc1/hume/_common/__init__.py
--rw-r--r--   0        0        0     4907 2024-04-30 13:04:16.986600 hume-0.5.1rc1/hume/_common/client_base.py
--rw-r--r--   0        0        0     1804 2024-04-08 23:00:47.349405 hume-0.5.1rc1/hume/_common/config_base.py
--rw-r--r--   0        0        0      121 2024-04-09 04:12:04.402577 hume-0.5.1rc1/hume/_common/protocol.py
--rw-r--r--   0        0        0       19 2024-04-08 23:37:14.346157 hume-0.5.1rc1/hume/_common/utilities/__init__.py
--rw-r--r--   0        0        0     2320 2024-04-08 23:37:14.348937 hume-0.5.1rc1/hume/_common/utilities/config_utilities.py
--rw-r--r--   0        0        0      291 2024-04-09 04:20:34.829615 hume-0.5.1rc1/hume/_common/utilities/model_utilities.py
--rw-r--r--   0        0        0      215 2024-04-09 04:20:36.584244 hume-0.5.1rc1/hume/_common/utilities/paging_utilities.py
--rw-r--r--   0        0        0     3545 2024-04-08 23:37:14.349713 hume-0.5.1rc1/hume/_common/utilities/retry_utilities.py
--rw-r--r--   0        0        0       58 2024-04-09 04:12:04.403581 hume-0.5.1rc1/hume/_common/utilities/typing_utilities.py
--rw-r--r--   0        0        0       19 2024-04-08 22:57:09.806665 hume-0.5.1rc1/hume/_measurement/__init__.py
--rw-r--r--   0        0        0      573 2024-04-08 22:57:09.806941 hume-0.5.1rc1/hume/_measurement/batch/__init__.py
--rw-r--r--   0        0        0     4387 2024-04-08 22:57:09.807530 hume-0.5.1rc1/hume/_measurement/batch/batch_job.py
--rw-r--r--   0        0        0     6046 2024-04-08 22:57:09.807740 hume-0.5.1rc1/hume/_measurement/batch/batch_job_details.py
--rw-r--r--   0        0        0      643 2024-04-08 22:57:09.807893 hume-0.5.1rc1/hume/_measurement/batch/batch_job_state.py
--rw-r--r--   0        0        0      994 2024-04-08 23:00:47.349544 hume-0.5.1rc1/hume/_measurement/batch/batch_job_status.py
--rw-r--r--   0        0        0    10353 2024-04-09 04:20:39.402038 hume-0.5.1rc1/hume/_measurement/batch/hume_batch_client.py
--rw-r--r--   0        0        0      940 2024-04-08 23:00:47.349881 hume-0.5.1rc1/hume/_measurement/batch/transcription_config.py
--rw-r--r--   0        0        0      216 2024-04-08 22:57:09.808459 hume-0.5.1rc1/hume/_measurement/stream/__init__.py
--rw-r--r--   0        0        0     3288 2024-04-09 04:12:04.404187 hume-0.5.1rc1/hume/_measurement/stream/hume_stream_client.py
--rw-r--r--   0        0        0     9411 2024-04-09 03:27:28.257593 hume-0.5.1rc1/hume/_measurement/stream/stream_socket.py
--rw-r--r--   0        0        0      602 2024-04-30 12:09:39.889889 hume-0.5.1rc1/hume/_voice/__init__.py
--rw-r--r--   0        0        0      429 2024-04-29 19:31:03.047474 hume-0.5.1rc1/hume/_voice/hume_voice_client.py
--rw-r--r--   0        0        0       19 2024-04-24 21:46:26.078781 hume-0.5.1rc1/hume/_voice/microphone/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-24 21:46:26.079063 hume-0.5.1rc1/hume/_voice/microphone/asyncio_utilities.py
--rw-r--r--   0        0        0      728 2024-04-24 21:46:26.079508 hume-0.5.1rc1/hume/_voice/microphone/audio_utilities.py
--rw-r--r--   0        0        0     3652 2024-05-02 12:12:57.948714 hume-0.5.1rc1/hume/_voice/microphone/chat_client.py
--rw-r--r--   0        0        0     3350 2024-04-24 21:46:26.080119 hume-0.5.1rc1/hume/_voice/microphone/microphone.py
--rw-r--r--   0        0        0     1667 2024-04-24 21:46:26.080399 hume-0.5.1rc1/hume/_voice/microphone/microphone_interface.py
--rw-r--r--   0        0        0     2925 2024-05-02 12:27:07.229612 hume-0.5.1rc1/hume/_voice/microphone/microphone_sender.py
--rw-r--r--   0        0        0       19 2024-04-24 21:46:26.080728 hume-0.5.1rc1/hume/_voice/mixins/__init__.py
--rw-r--r--   0        0        0     2017 2024-04-24 21:46:26.081139 hume-0.5.1rc1/hume/_voice/mixins/chat_mixin.py
--rw-r--r--   0        0        0     2841 2024-04-24 21:46:26.081459 hume-0.5.1rc1/hume/_voice/mixins/chats_mixin.py
--rw-r--r--   0        0        0     5337 2024-04-30 12:07:23.305131 hume-0.5.1rc1/hume/_voice/mixins/configs_mixin.py
--rw-r--r--   0        0        0     4289 2024-04-30 12:10:17.367400 hume-0.5.1rc1/hume/_voice/mixins/tools_mixin.py
--rw-r--r--   0        0        0       19 2024-04-24 21:46:26.082013 hume-0.5.1rc1/hume/_voice/models/__init__.py
--rw-r--r--   0        0        0     2608 2024-04-24 21:46:26.082284 hume-0.5.1rc1/hume/_voice/models/chats_models.py
--rw-r--r--   0        0        0     2425 2024-05-02 12:19:24.347700 hume-0.5.1rc1/hume/_voice/models/configs_models.py
--rw-r--r--   0        0        0     1140 2024-04-30 11:49:55.154292 hume-0.5.1rc1/hume/_voice/models/tools_models.py
--rw-r--r--   0        0        0      461 2024-04-24 21:46:26.083048 hume-0.5.1rc1/hume/_voice/session_settings.py
--rw-r--r--   0        0        0     3192 2024-05-02 12:32:05.859932 hume-0.5.1rc1/hume/_voice/voice_socket.py
--rw-r--r--   0        0        0       19 2023-06-29 18:23:24.726173 hume-0.5.1rc1/hume/error/__init__.py
--rw-r--r--   0        0        0      571 2023-11-09 21:00:40.007182 hume-0.5.1rc1/hume/error/hume_client_exception.py
--rw-r--r--   0        0        0       97 2024-04-08 23:00:47.350438 hume-0.5.1rc1/hume/models/__init__.py
--rw-r--r--   0        0        0      588 2024-04-08 23:00:47.350573 hume-0.5.1rc1/hume/models/config/__init__.py
--rw-r--r--   0        0        0      498 2024-04-08 23:00:47.350848 hume-0.5.1rc1/hume/models/config/burst_config.py
--rw-r--r--   0        0        0     2574 2024-04-08 23:00:47.351014 hume-0.5.1rc1/hume/models/config/face_config.py
--rw-r--r--   0        0        0      510 2024-04-08 23:00:47.351168 hume-0.5.1rc1/hume/models/config/facemesh_config.py
--rw-r--r--   0        0        0     2236 2024-04-08 23:00:47.351315 hume-0.5.1rc1/hume/models/config/language_config.py
--rw-r--r--   0        0        0      632 2024-04-08 23:00:47.351466 hume-0.5.1rc1/hume/models/config/model_config_base.py
--rw-r--r--   0        0        0     1001 2024-04-08 23:00:47.351600 hume-0.5.1rc1/hume/models/config/ner_config.py
--rw-r--r--   0        0        0     1786 2024-04-08 23:00:47.351778 hume-0.5.1rc1/hume/models/config/prosody_config.py
--rw-r--r--   0        0        0      805 2024-04-08 23:00:47.351947 hume-0.5.1rc1/hume/models/model_type.py
--rw-r--r--   0        0        0     2640 2024-05-02 12:34:26.254311 hume-0.5.1rc1/pyproject.toml
--rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.5.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-24 20:58:49.224091 hume-0.6.0rc1/LICENSE
+-rw-r--r--   0        0        0     2256 2024-05-24 20:58:49.224680 hume-0.6.0rc1/README.md
+-rw-r--r--   0        0        0      985 2024-05-24 20:58:49.235357 hume-0.6.0rc1/hume/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.235561 hume-0.6.0rc1/hume/_common/__init__.py
+-rw-r--r--   0        0        0     5027 2024-05-29 08:51:51.161632 hume-0.6.0rc1/hume/_common/client_base.py
+-rw-r--r--   0        0        0     1804 2024-05-24 20:58:49.236064 hume-0.6.0rc1/hume/_common/config_base.py
+-rw-r--r--   0        0        0      121 2024-05-24 20:58:49.236337 hume-0.6.0rc1/hume/_common/protocol.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.236404 hume-0.6.0rc1/hume/_common/utilities/__init__.py
+-rw-r--r--   0        0        0     2320 2024-05-24 20:58:49.236629 hume-0.6.0rc1/hume/_common/utilities/config_utilities.py
+-rw-r--r--   0        0        0      291 2024-05-24 20:58:49.236911 hume-0.6.0rc1/hume/_common/utilities/model_utilities.py
+-rw-r--r--   0        0        0      215 2024-05-24 20:58:49.237167 hume-0.6.0rc1/hume/_common/utilities/paging_utilities.py
+-rw-r--r--   0        0        0     3545 2024-05-24 20:58:49.237327 hume-0.6.0rc1/hume/_common/utilities/retry_utilities.py
+-rw-r--r--   0        0        0       58 2024-05-24 20:58:49.237899 hume-0.6.0rc1/hume/_common/utilities/typing_utilities.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.237955 hume-0.6.0rc1/hume/_measurement/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-24 20:58:49.238192 hume-0.6.0rc1/hume/_measurement/batch/__init__.py
+-rw-r--r--   0        0        0     4387 2024-05-24 20:58:49.238389 hume-0.6.0rc1/hume/_measurement/batch/batch_job.py
+-rw-r--r--   0        0        0     6046 2024-05-24 20:58:49.238555 hume-0.6.0rc1/hume/_measurement/batch/batch_job_details.py
+-rw-r--r--   0        0        0      643 2024-05-24 20:58:49.238742 hume-0.6.0rc1/hume/_measurement/batch/batch_job_state.py
+-rw-r--r--   0        0        0      994 2024-05-24 20:58:49.238927 hume-0.6.0rc1/hume/_measurement/batch/batch_job_status.py
+-rw-r--r--   0        0        0    10353 2024-05-24 20:58:49.239255 hume-0.6.0rc1/hume/_measurement/batch/hume_batch_client.py
+-rw-r--r--   0        0        0      940 2024-05-24 20:58:49.239412 hume-0.6.0rc1/hume/_measurement/batch/transcription_config.py
+-rw-r--r--   0        0        0      216 2024-05-24 20:58:49.239675 hume-0.6.0rc1/hume/_measurement/stream/__init__.py
+-rw-r--r--   0        0        0     3288 2024-05-24 20:58:49.239962 hume-0.6.0rc1/hume/_measurement/stream/hume_stream_client.py
+-rw-r--r--   0        0        0     9411 2024-05-24 20:58:49.240421 hume-0.6.0rc1/hume/_measurement/stream/stream_socket.py
+-rw-r--r--   0        0        0      602 2024-05-24 20:58:49.240584 hume-0.6.0rc1/hume/_voice/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-24 20:58:49.240941 hume-0.6.0rc1/hume/_voice/hume_voice_client.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.240993 hume-0.6.0rc1/hume/_voice/microphone/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-24 20:58:49.241753 hume-0.6.0rc1/hume/_voice/microphone/asyncio_utilities.py
+-rw-r--r--   0        0        0      728 2024-05-24 20:58:49.242003 hume-0.6.0rc1/hume/_voice/microphone/audio_utilities.py
+-rw-r--r--   0        0        0     3652 2024-05-29 15:23:35.830242 hume-0.6.0rc1/hume/_voice/microphone/chat_client.py
+-rw-r--r--   0        0        0     3350 2024-05-24 20:58:49.242598 hume-0.6.0rc1/hume/_voice/microphone/microphone.py
+-rw-r--r--   0        0        0     1667 2024-05-24 20:58:49.243439 hume-0.6.0rc1/hume/_voice/microphone/microphone_interface.py
+-rw-r--r--   0        0        0     2925 2024-05-24 20:58:49.243638 hume-0.6.0rc1/hume/_voice/microphone/microphone_sender.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.243842 hume-0.6.0rc1/hume/_voice/mixins/__init__.py
+-rw-r--r--   0        0        0     2464 2024-05-29 16:17:44.822280 hume-0.6.0rc1/hume/_voice/mixins/chat_mixin.py
+-rw-r--r--   0        0        0     5995 2024-05-29 16:12:41.956582 hume-0.6.0rc1/hume/_voice/mixins/chats_mixin.py
+-rw-r--r--   0        0        0     5337 2024-05-28 18:24:12.336999 hume-0.6.0rc1/hume/_voice/mixins/configs_mixin.py
+-rw-r--r--   0        0        0     4289 2024-05-24 20:58:49.245040 hume-0.6.0rc1/hume/_voice/mixins/tools_mixin.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.245104 hume-0.6.0rc1/hume/_voice/models/__init__.py
+-rw-r--r--   0        0        0     3669 2024-05-29 16:12:40.439856 hume-0.6.0rc1/hume/_voice/models/chats_models.py
+-rw-r--r--   0        0        0     2425 2024-05-29 15:50:48.388858 hume-0.6.0rc1/hume/_voice/models/configs_models.py
+-rw-r--r--   0        0        0     1140 2024-05-24 20:58:49.245773 hume-0.6.0rc1/hume/_voice/models/tools_models.py
+-rw-r--r--   0        0        0      461 2024-05-24 20:58:49.246706 hume-0.6.0rc1/hume/_voice/session_settings.py
+-rw-r--r--   0        0        0     3192 2024-05-24 20:58:49.246918 hume-0.6.0rc1/hume/_voice/voice_socket.py
+-rw-r--r--   0        0        0       19 2024-05-24 20:58:49.246982 hume-0.6.0rc1/hume/error/__init__.py
+-rw-r--r--   0        0        0      571 2024-05-24 20:58:49.247044 hume-0.6.0rc1/hume/error/hume_client_exception.py
+-rw-r--r--   0        0        0       97 2024-05-24 20:58:49.247234 hume-0.6.0rc1/hume/models/__init__.py
+-rw-r--r--   0        0        0      588 2024-05-24 20:58:49.247521 hume-0.6.0rc1/hume/models/config/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-24 20:58:49.247717 hume-0.6.0rc1/hume/models/config/burst_config.py
+-rw-r--r--   0        0        0     2574 2024-05-24 20:58:49.247919 hume-0.6.0rc1/hume/models/config/face_config.py
+-rw-r--r--   0        0        0      510 2024-05-24 20:58:49.248127 hume-0.6.0rc1/hume/models/config/facemesh_config.py
+-rw-r--r--   0        0        0     2236 2024-05-24 20:58:49.248317 hume-0.6.0rc1/hume/models/config/language_config.py
+-rw-r--r--   0        0        0      632 2024-05-24 20:58:49.248526 hume-0.6.0rc1/hume/models/config/model_config_base.py
+-rw-r--r--   0        0        0     1001 2024-05-24 20:58:49.248760 hume-0.6.0rc1/hume/models/config/ner_config.py
+-rw-r--r--   0        0        0     1786 2024-05-24 20:58:49.248946 hume-0.6.0rc1/hume/models/config/prosody_config.py
+-rw-r--r--   0        0        0      805 2024-05-24 20:58:49.249139 hume-0.6.0rc1/hume/models/model_type.py
+-rw-r--r--   0        0        0     2640 2024-05-29 17:04:31.768391 hume-0.6.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     3655 1970-01-01 00:00:00.000000 hume-0.6.0rc1/PKG-INFO
```

### Comparing `hume-0.5.1rc1/LICENSE` & `hume-0.6.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/README.md` & `hume-0.6.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/__init__.py` & `hume-0.6.0rc1/hume/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_common/client_base.py` & `hume-0.6.0rc1/hume/_common/client_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,16 @@
         )
 
         try:
             response = self._http_client.send(request)
             response.raise_for_status()
         except Exception as exc:  # pylint: disable=broad-exception-caught
             response_body = response.json()
+            if "message" in response_body:
+                raise HumeClientException(response_body["message"]) from exc
             raise HumeClientException(str(response_body)) from exc
 
         return response
 
     def _get_client_headers(self) -> Dict[str, str]:
         return {
             "X-Hume-Api-Key": self._api_key,
```

### Comparing `hume-0.5.1rc1/hume/_common/config_base.py` & `hume-0.6.0rc1/hume/_common/config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_common/utilities/config_utilities.py` & `hume-0.6.0rc1/hume/_common/utilities/config_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_common/utilities/retry_utilities.py` & `hume-0.6.0rc1/hume/_common/utilities/retry_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/__init__.py` & `hume-0.6.0rc1/hume/_measurement/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/batch_job.py` & `hume-0.6.0rc1/hume/_measurement/batch/batch_job.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/batch_job_details.py` & `hume-0.6.0rc1/hume/_measurement/batch/batch_job_details.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/batch_job_state.py` & `hume-0.6.0rc1/hume/_measurement/batch/batch_job_state.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/batch_job_status.py` & `hume-0.6.0rc1/hume/_measurement/batch/batch_job_status.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/hume_batch_client.py` & `hume-0.6.0rc1/hume/_measurement/batch/hume_batch_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/batch/transcription_config.py` & `hume-0.6.0rc1/hume/_measurement/batch/transcription_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/stream/hume_stream_client.py` & `hume-0.6.0rc1/hume/_measurement/stream/hume_stream_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_measurement/stream/stream_socket.py` & `hume-0.6.0rc1/hume/_measurement/stream/stream_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/__init__.py` & `hume-0.6.0rc1/hume/_voice/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/asyncio_utilities.py` & `hume-0.6.0rc1/hume/_voice/microphone/asyncio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/audio_utilities.py` & `hume-0.6.0rc1/hume/_voice/microphone/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/chat_client.py` & `hume-0.6.0rc1/hume/_voice/microphone/chat_client.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/microphone.py` & `hume-0.6.0rc1/hume/_voice/microphone/microphone.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/microphone_interface.py` & `hume-0.6.0rc1/hume/_voice/microphone/microphone_interface.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/microphone/microphone_sender.py` & `hume-0.6.0rc1/hume/_voice/microphone/microphone_sender.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/mixins/chat_mixin.py` & `hume-0.6.0rc1/hume/_voice/mixins/chat_mixin.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,25 +16,37 @@
 
 class ChatMixin(ClientBase):
     """Client operations for EVI WebSocket connections."""
 
     DEFAULT_MAX_PAYLOAD_SIZE_BYTES: ClassVar[int] = 2**24
 
     @asynccontextmanager
-    async def connect(self, config_id: Optional[str] = None) -> AsyncIterator[VoiceSocket]:
+    async def connect(
+        self,
+        config_id: Optional[str] = None,
+        chat_group_id: Optional[str] = None,
+    ) -> AsyncIterator[VoiceSocket]:
         """Connect to the EVI API.
 
         Args:
             config_id (Optional[str]): Config ID.
         """
         uri_base = self._build_endpoint("evi", "chat", Protocol.WS)
 
+        if config_id is not None and chat_group_id is not None:
+            raise HumeClientException(
+                "If resuming from a chat_group_id you must not provide a config_id. "
+                "The original config for the chat group will be used automatically."
+            )
+
         params: Dict[str, Any] = {}
         if config_id is not None:
             params["config_id"] = config_id
+        if chat_group_id is not None:
+            params["chat_group_id"] = chat_group_id
 
         encoded_params = urllib.parse.urlencode(params)
         uri = f"{uri_base}?{encoded_params}"
 
         logger.info("Connecting to EVI API at %s", uri)
 
         max_size = self.DEFAULT_MAX_PAYLOAD_SIZE_BYTES
```

### Comparing `hume-0.5.1rc1/hume/_voice/mixins/configs_mixin.py` & `hume-0.6.0rc1/hume/_voice/mixins/configs_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/mixins/tools_mixin.py` & `hume-0.6.0rc1/hume/_voice/mixins/tools_mixin.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/models/chats_models.py` & `hume-0.6.0rc1/hume/_voice/models/configs_models.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,112 +1,114 @@
-"""API request and response models for EVI chats."""
+"""API request and response models for EVI configurations."""
 
-from enum import Enum
 from typing import List, Optional
 
-from pydantic import UUID4, BaseModel
+from hume._common.utilities.model_utilities import BaseModel
+from hume._voice.models.tools_models import ToolMeta
 
-from hume._common.utilities.typing_utilities import JsonObject
-from hume._voice.models.configs_models import ConfigMeta
 
+class PromptResponse(BaseModel):
+    """Response model for an EVI prompt."""
 
-class ChatStatus(str, Enum):
-    """Status codes for EVI chats."""
+    id: str
+    version: int
+    version_description: Optional[str]
+    name: str
+    created_on: int
+    modified_on: int
+    text: Optional[str]
 
-    ACTIVE = "ACTIVE"
-    USER_ENDED = "USER_ENDED"
-    USER_TIMEOUT = "USER_TIMEOUT"
-    ERROR = "ERROR"
 
+class PromptsResponse(BaseModel):
+    """Response model for a page of EVI prompts."""
 
-class EventType(str, Enum):
-    """Identifier for the type of event in an EVI session."""
+    page_number: int
+    page_size: int
+    prompts: List[PromptResponse]
 
-    SYSTEM_PROMPT = "SYSTEM_PROMPT"
-    USER_MESSAGE = "USER_MESSAGE"
-    USER_INTERRUPTION = "USER_INTERRUPTION"
-    AGENT_MESSAGE = "AGENT_MESSAGE"
-    FUNCTION_CALL = "FUNCTION_CALL"
 
+class PromptMeta(BaseModel):
+    """Prompt metadata."""
 
-class Role(str, Enum):
-    """Identifier for the speaker of a turn in an EVI session."""
+    id: str
+    version: int
 
-    USER = "USER"
-    AGENT = "AGENT"
-    SYSTEM = "SYSTEM"
 
+class LanguageModelConfig(BaseModel):
+    """Language model configuration for EVI."""
 
-class FunctionCall(BaseModel):
-    """Function call model."""
+    model_provider: str
+    model_resource: str
+    temperature: Optional[float] = None
 
-    target: Optional[str] = None
-    params: Optional[JsonObject] = None
-    result: Optional[JsonObject] = None
 
+class PostPromptRequest(BaseModel):
+    """Post request model for creating a new EVI prompt."""
 
-class ChatEvent(BaseModel):
-    """Chat event model."""
+    name: str
+    version_description: Optional[str]
+    text: Optional[str]
 
-    id: UUID4
-    timestamp: int
-    role: Role
-    type: EventType
-    message_text: Optional[str] = None
-    function_call: Optional[FunctionCall] = None
-    emotion_features: Optional[JsonObject] = None
-    metadata: Optional[JsonObject] = None
+
+class ConfigResponse(BaseModel):
+    """Response model for an EVI configurations."""
+
+    id: str
+    version: int
+    version_description: Optional[str]
+    name: str
+    created_on: int
+    modified_on: int
+    prompt: Optional[PromptResponse]
 
 
-class ChatEventsResponse(BaseModel):
-    """Response model for a page of EVI chat events."""
+class ConfigsResponse(BaseModel):
+    """Response model for a page of EVI configurations."""
 
-    id: UUID4
-    resumed_from_id: Optional[UUID4] = None
-    tag: Optional[str] = None
-    status: ChatStatus
-    start_timestamp: int
-    end_timestamp: Optional[int] = None
-    events_page: List[ChatEvent]
-    metadata: Optional[JsonObject] = None
     page_number: int
     page_size: int
-    config: ConfigMeta
+    configs_page: List[ConfigResponse]
 
 
-class ChatMessage(BaseModel):
-    """Chat message model."""
+class VoiceIdentityConfig(BaseModel):
+    """Configuration for changing the voice of EVI."""
 
-    timestamp: int
-    role: Role
-    type: EventType
-    message_text: Optional[str] = None
-    function_call: Optional[FunctionCall] = None
-    emotion_features: Optional[JsonObject] = None
-    metadata: Optional[JsonObject] = None
+    provider: Optional[str] = None
+    name: Optional[str] = None
 
 
-class ChatResponse(BaseModel):
-    """Response model for an EVI chat."""
+class BuiltinToolConfig(BaseModel):
+    """Configuration for a built-in EVI tool."""
 
-    id: str
-    resumed_from_id: Optional[UUID4] = None
-    tag: Optional[str] = None
-    status: Optional[ChatStatus]
-    start_timestamp: int
-    end_timestamp: int
-    metadata: Optional[JsonObject] = None
-    config: ConfigMeta
+    name: str
+    tool_type: str
+    fallback_content: Optional[str]
 
 
-class ChatsResponse(BaseModel):
-    """Response model for a page of EVI chats."""
+class PostConfigRequest(BaseModel):
+    """Post request model for creating a new EVI configuration."""
 
-    chats_page: List[ChatResponse]
-    page_number: int
-    page_size: int
+    name: str
+    version_description: Optional[str]
+    prompt: PromptMeta
+    voice: Optional[VoiceIdentityConfig]
+    language_model: Optional[LanguageModelConfig]
+    tools: Optional[List[ToolMeta]]
+
+
+class ConfigMeta(BaseModel):
+    """EVI configuration metadata."""
+
+    id: Optional[str]
+    version: Optional[int]
 
 
-class VoiceChat(BaseModel):
-    """Voice chat model."""
+class VoiceConfig(BaseModel):
+    """EVI configuration."""
 
     id: str
+    name: str
+    description: Optional[str]
+    created_on: int
+    modified_on: int
+    # TODO: Add tool info
+    prompt: Optional[str]
```

### Comparing `hume-0.5.1rc1/hume/_voice/models/tools_models.py` & `hume-0.6.0rc1/hume/_voice/models/tools_models.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/_voice/voice_socket.py` & `hume-0.6.0rc1/hume/_voice/voice_socket.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/error/hume_client_exception.py` & `hume-0.6.0rc1/hume/error/hume_client_exception.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/__init__.py` & `hume-0.6.0rc1/hume/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/face_config.py` & `hume-0.6.0rc1/hume/models/config/face_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/language_config.py` & `hume-0.6.0rc1/hume/models/config/language_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/model_config_base.py` & `hume-0.6.0rc1/hume/models/config/model_config_base.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/ner_config.py` & `hume-0.6.0rc1/hume/models/config/ner_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/config/prosody_config.py` & `hume-0.6.0rc1/hume/models/config/prosody_config.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/hume/models/model_type.py` & `hume-0.6.0rc1/hume/models/model_type.py`

 * *Files identical despite different names*

### Comparing `hume-0.5.1rc1/pyproject.toml` & `hume-0.6.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
   "communication",
   "learning",
 ]
 license = "Proprietary"
 name = "hume"
 readme = "README.md"
 repository = "https://github.com/HumeAI/hume-python-sdk"
-version = "0.5.1rc1"
+version = "0.6.0rc1"
 
 [tool.poetry.dependencies]
 httpx = { extras = ["http2"], version = "^0.27.0" }
 jupyter = { version = "^1.0.0", optional = true }
 pydantic = "^2.6.4"
 pydub = "^0.25.1"
 python = ">=3.9,<4"
@@ -82,19 +82,19 @@
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.black]
 line-length = 120
 
 [tool.covcheck.group.unit.coverage]
-branch = 45.0
+branch = 42.0
 line = 71.0
 
 [tool.covcheck.group.service.coverage]
-branch = 57.0
+branch = 56.0
 line = 80.0
 
 [tool.isort]
 line_length = 120
 profile = "black"
 src_paths = "*"
```

### Comparing `hume-0.5.1rc1/PKG-INFO` & `hume-0.6.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hume
-Version: 0.5.1rc1
+Version: 0.6.0rc1
 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk
 License: Proprietary
 Keywords: hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev
 Author-email: dev@hume.ai
 Requires-Python: >=3.9,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hume Version: 0.5.1rc1 Summary: Hume AI Python SDK
+Metadata-Version: 2.1 Name: hume Version: 0.6.0rc1 Summary: Hume AI Python SDK
 Home-page: https://github.com/HumeAI/hume-python-sdk License: Proprietary
 Keywords:
 hume,ai,evi,empathic,multimodal,expression,analysis,sentiment,voice,recognition,detection,emotion,interface,speech,audio,vision,expressive,embeddings,communication,learning
 Author: Hume AI Dev Author-email: dev@hume.ai Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

