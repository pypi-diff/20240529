# Comparing `tmp/voicegain-speech-1.99.0.tar.gz` & `tmp/voicegain-speech-1.99.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicegain-speech-1.99.0.tar", last modified: Wed Feb 14 06:55:55 2024, max compression
+gzip compressed data, was "voicegain-speech-1.99.1.tar", last modified: Wed Feb 21 22:21:36 2024, max compression
```

## Comparing `voicegain-speech-1.99.0.tar` & `voicegain-speech-1.99.1.tar`

### file list

```diff
@@ -1,536 +1,536 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 06:55:55.737952 voicegain-speech-1.99.0/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2936 2024-02-14 06:55:55.737952 voicegain-speech-1.99.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2504 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/README.md
--rw-r--r--   0 root         (0) root         (0)       79 2024-02-14 06:55:55.738952 voicegain-speech-1.99.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 06:55:55.619951 voicegain-speech-1.99.0/voicegain_speech/
--rw-r--r--   0 root         (0) root         (0)    68395 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 06:55:55.624951 voicegain-speech-1.99.0/voicegain_speech/api/
--rw-r--r--   0 root         (0) root         (0)      831 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33334 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/aivr_api.py
--rw-r--r--   0 root         (0) root         (0)    52269 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/aivr_callback_api.py
--rw-r--r--   0 root         (0) root         (0)    39277 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/asr_callback_api.py
--rw-r--r--   0 root         (0) root         (0)    35241 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/audiocodes_api.py
--rw-r--r--   0 root         (0) root         (0)   144142 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/data_api.py
--rw-r--r--   0 root         (0) root         (0)   143692 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/greg_api.py
--rw-r--r--   0 root         (0) root         (0)   140315 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/meeting_api.py
--rw-r--r--   0 root         (0) root         (0)    48215 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/recognize_api.py
--rw-r--r--   0 root         (0) root         (0)   119088 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/sa_api.py
--rw-r--r--   0 root         (0) root         (0)    37228 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/security_api.py
--rw-r--r--   0 root         (0) root         (0)    57407 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/training_api.py
--rw-r--r--   0 root         (0) root         (0)   103284 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/transcribe_api.py
--rw-r--r--   0 root         (0) root         (0)    55782 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api/websocket_api.py
--rw-r--r--   0 root         (0) root         (0)    51992 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/api_client.py
--rw-r--r--   0 root         (0) root         (0)    38452 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/configuration.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 06:55:55.737952 voicegain-speech-1.99.0/voicegain_speech/models/
--rw-r--r--   0 root         (0) root         (0)    67201 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40185 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_control_messages.py
--rw-r--r--   0 root         (0) root         (0)    31448 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_end.py
--rw-r--r--   0 root         (0) root         (0)    31456 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_error.py
--rw-r--r--   0 root         (0) root         (0)    31574 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_hypothesis.py
--rw-r--r--   0 root         (0) root         (0)    30303 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_hypothesis_alternatives.py
--rw-r--r--   0 root         (0) root         (0)    31544 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_recognition.py
--rw-r--r--   0 root         (0) root         (0)    31707 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_recognition_alternatives.py
--rw-r--r--   0 root         (0) root         (0)    32581 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_response_messages.py
--rw-r--r--   0 root         (0) root         (0)    39668 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_start.py
--rw-r--r--   0 root         (0) root         (0)    31720 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_start_stt_speech_contexts.py
--rw-r--r--   0 root         (0) root         (0)    30573 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_started.py
--rw-r--r--   0 root         (0) root         (0)    30642 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ac_stop.py
--rw-r--r--   0 root         (0) root         (0)    31320 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/account_and_context_id.py
--rw-r--r--   0 root         (0) root         (0)    34223 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/advanced_regex.py
--rw-r--r--   0 root         (0) root         (0)    30250 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aircall.py
--rw-r--r--   0 root         (0) root         (0)    30290 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aircall_all_of.py
--rw-r--r--   0 root         (0) root         (0)    33370 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_core_response.py
--rw-r--r--   0 root         (0) root         (0)    33490 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_core_response_all_of.py
--rw-r--r--   0 root         (0) root         (0)    36189 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response.py
--rw-r--r--   0 root         (0) root         (0)    32419 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response_all_of.py
--rw-r--r--   0 root         (0) root         (0)    31605 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response_final.py
--rw-r--r--   0 root         (0) root         (0)    30267 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_conference_transfer.py
--rw-r--r--   0 root         (0) root         (0)    30925 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_disconnect.py
--rw-r--r--   0 root         (0) root         (0)    35420 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_event.py
--rw-r--r--   0 root         (0) root         (0)    29668 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_event_type.py
--rw-r--r--   0 root         (0) root         (0)    33126 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_existing_session.py
--rw-r--r--   0 root         (0) root         (0)    32738 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic.py
--rw-r--r--   0 root         (0) root         (0)    29531 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_media.py
--rw-r--r--   0 root         (0) root         (0)    31480 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_transfer.py
--rw-r--r--   0 root         (0) root         (0)    29617 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_type.py
--rw-r--r--   0 root         (0) root         (0)    45552 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_new_session.py
--rw-r--r--   0 root         (0) root         (0)    31022 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_phone_transfer.py
--rw-r--r--   0 root         (0) root         (0)    34959 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt.py
--rw-r--r--   0 root         (0) root         (0)    30724 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_completion.py
--rw-r--r--   0 root         (0) root         (0)    36415 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_playing.py
--rw-r--r--   0 root         (0) root         (0)    30233 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_properties_audio.py
--rw-r--r--   0 root         (0) root         (0)    30243 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_properties_html.py
--rw-r--r--   0 root         (0) root         (0)    37845 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_question.py
--rw-r--r--   0 root         (0) root         (0)    29628 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_recognition_result.py
--rw-r--r--   0 root         (0) root         (0)    35695 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_recording.py
--rw-r--r--   0 root         (0) root         (0)    42807 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_response_properties_audio.py
--rw-r--r--   0 root         (0) root         (0)    31820 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_response_properties_html.py
--rw-r--r--   0 root         (0) root         (0)    34490 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user.py
--rw-r--r--   0 root         (0) root         (0)    30596 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user_base.py
--rw-r--r--   0 root         (0) root         (0)    33362 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user_fs.py
--rw-r--r--   0 root         (0) root         (0)    32062 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_transfer.py
--rw-r--r--   0 root         (0) root         (0)    30314 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivr_vars.py
--rw-r--r--   0 root         (0) root         (0)    32390 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/aivrs_question_specifics.py
--rw-r--r--   0 root         (0) root         (0)    31670 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/answer_map_entry.py
--rw-r--r--   0 root         (0) root         (0)    29622 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_event.py
--rw-r--r--   0 root         (0) root         (0)    29713 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status.py
--rw-r--r--   0 root         (0) root         (0)    29633 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_additional.py
--rw-r--r--   0 root         (0) root         (0)    29688 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_after_input_started.py
--rw-r--r--   0 root         (0) root         (0)    29715 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_for_callback.py
--rw-r--r--   0 root         (0) root         (0)    29624 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_recognition_result.py
--rw-r--r--   0 root         (0) root         (0)    45203 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_common.py
--rw-r--r--   0 root         (0) root         (0)    35724 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_meeting_transcription.py
--rw-r--r--   0 root         (0) root         (0)    59219 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition.py
--rw-r--r--   0 root         (0) root         (0)    54583 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_defaults.py
--rw-r--r--   0 root         (0) root         (0)    43620 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
--rw-r--r--   0 root         (0) root         (0)    38376 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_timeouts.py
--rw-r--r--   0 root         (0) root         (0)    54671 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription.py
--rw-r--r--   0 root         (0) root         (0)    62236 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_async.py
--rw-r--r--   0 root         (0) root         (0)    31643 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py
--rw-r--r--   0 root         (0) root         (0)    52690 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_common.py
--rw-r--r--   0 root         (0) root         (0)    36523 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_common_lm.py
--rw-r--r--   0 root         (0) root         (0)    34702 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
--rw-r--r--   0 root         (0) root         (0)    57940 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_defaults.py
--rw-r--r--   0 root         (0) root         (0)    53321 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_sa.py
--rw-r--r--   0 root         (0) root         (0)    31829 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_speakers.py
--rw-r--r--   0 root         (0) root         (0)    33246 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
--rw-r--r--   0 root         (0) root         (0)    34449 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/asr_transcribe_queue_status.py
--rw-r--r--   0 root         (0) root         (0)    34178 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_audio_input_source.py
--rw-r--r--   0 root         (0) root         (0)    29634 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_mode.py
--rw-r--r--   0 root         (0) root         (0)    29678 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_mode_recognition.py
--rw-r--r--   0 root         (0) root         (0)    29595 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_mode_speech_analytics.py
--rw-r--r--   0 root         (0) root         (0)    29641 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_mode_transcription.py
--rw-r--r--   0 root         (0) root         (0)    31815 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_post_response_base.py
--rw-r--r--   0 root         (0) root         (0)    31210 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_post_response_base_audio.py
--rw-r--r--   0 root         (0) root         (0)    32888 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_reco_post_response.py
--rw-r--r--   0 root         (0) root         (0)    30565 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_reco_post_response_sessions.py
--rw-r--r--   0 root         (0) root         (0)    30477 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_callback_response.py
--rw-r--r--   0 root         (0) root         (0)    32109 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_request.py
--rw-r--r--   0 root         (0) root         (0)    32239 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_response.py
--rw-r--r--   0 root         (0) root         (0)    34998 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_result.py
--rw-r--r--   0 root         (0) root         (0)    30264 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_result_all_of.py
--rw-r--r--   0 root         (0) root         (0)    34598 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full.py
--rw-r--r--   0 root         (0) root         (0)    32527 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of.py
--rw-r--r--   0 root         (0) root         (0)    30937 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio.py
--rw-r--r--   0 root         (0) root         (0)    37252 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_callback.py
--rw-r--r--   0 root         (0) root         (0)    30351 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_source.py
--rw-r--r--   0 root         (0) root         (0)    30363 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
--rw-r--r--   0 root         (0) root         (0)    44609 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_result.py
--rw-r--r--   0 root         (0) root         (0)    33367 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental.py
--rw-r--r--   0 root         (0) root         (0)    31184 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail.py
--rw-r--r--   0 root         (0) root         (0)    31222 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_control_status.py
--rw-r--r--   0 root         (0) root         (0)    39957 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_result.py
--rw-r--r--   0 root         (0) root         (0)    34493 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
--rw-r--r--   0 root         (0) root         (0)    33369 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_session_established.py
--rw-r--r--   0 root         (0) root         (0)    32751 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_session_short_info.py
--rw-r--r--   0 root         (0) root         (0)    30378 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_session_url.py
--rw-r--r--   0 root         (0) root         (0)    32946 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transc_post_response.py
--rw-r--r--   0 root         (0) root         (0)    30599 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transc_post_response_sessions.py
--rw-r--r--   0 root         (0) root         (0)    35444 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transc_session_established.py
--rw-r--r--   0 root         (0) root         (0)    30405 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_callback_response.py
--rw-r--r--   0 root         (0) root         (0)    32046 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_request.py
--rw-r--r--   0 root         (0) root         (0)    31419 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_response.py
--rw-r--r--   0 root         (0) root         (0)    31847 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_response_shared.py
--rw-r--r--   0 root         (0) root         (0)    29598 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_channel.py
--rw-r--r--   0 root         (0) root         (0)    29576 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_channel_selector.py
--rw-r--r--   0 root         (0) root         (0)    29669 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_channel_selector_offline_async.py
--rw-r--r--   0 root         (0) root         (0)    29530 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_channels.py
--rw-r--r--   0 root         (0) root         (0)    30225 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_for_data_object.py
--rw-r--r--   0 root         (0) root         (0)    29645 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_format.py
--rw-r--r--   0 root         (0) root         (0)    34076 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async.py
--rw-r--r--   0 root         (0) root         (0)    30291 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async_source.py
--rw-r--r--   0 root         (0) root         (0)    35198 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async_with_callback.py
--rw-r--r--   0 root         (0) root         (0)    33213 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_base.py
--rw-r--r--   0 root         (0) root         (0)    30166 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_callback.py
--rw-r--r--   0 root         (0) root         (0)    35329 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_callback_callback.py
--rw-r--r--   0 root         (0) root         (0)    29400 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data.py
--rw-r--r--   0 root         (0) root         (0)    31582 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data_all_of.py
--rw-r--r--   0 root         (0) root         (0)    31482 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data_all_of_source.py
--rw-r--r--   0 root         (0) root         (0)    35039 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_sync.py
--rw-r--r--   0 root         (0) root         (0)    31298 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_input_sync_source.py
--rw-r--r--   0 root         (0) root         (0)    35384 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_resource_uri.py
--rw-r--r--   0 root         (0) root         (0)    29630 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_zone_class.py
--rw-r--r--   0 root         (0) root         (0)    31541 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/audio_zone_item.py
--rw-r--r--   0 root         (0) root         (0)    34154 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/base_sentence_hypothesis_or_recognition.py
--rw-r--r--   0 root         (0) root         (0)    31999 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/base_sentence_hypothesis_or_recognition_alternatives.py
--rw-r--r--   0 root         (0) root         (0)    31289 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/base_stomp_word_correction.py
--rw-r--r--   0 root         (0) root         (0)    30071 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/basic_success_response.py
--rw-r--r--   0 root         (0) root         (0)    31573 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/builtin.py
--rw-r--r--   0 root         (0) root         (0)    31633 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/builtin_all_of.py
--rw-r--r--   0 root         (0) root         (0)    29912 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_attributes.py
--rw-r--r--   0 root         (0) root         (0)    36627 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_review_answer_alone.py
--rw-r--r--   0 root         (0) root         (0)    29561 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_review_answer_type.py
--rw-r--r--   0 root         (0) root         (0)    34033 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base.py
--rw-r--r--   0 root         (0) root         (0)    43494 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base_with_answer.py
--rw-r--r--   0 root         (0) root         (0)    35791 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base_with_id.py
--rw-r--r--   0 root         (0) root         (0)    35280 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/callback_req.py
--rw-r--r--   0 root         (0) root         (0)    32038 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/callback_req_reco.py
--rw-r--r--   0 root         (0) root         (0)    30199 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/callback_resp.py
--rw-r--r--   0 root         (0) root         (0)    33981 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/caption.py
--rw-r--r--   0 root         (0) root         (0)    31041 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/compliance_settings.py
--rw-r--r--   0 root         (0) root         (0)    29591 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/config_value_status.py
--rw-r--r--   0 root         (0) root         (0)    29684 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/content_type.py
--rw-r--r--   0 root         (0) root         (0)    33108 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/continuous_recognition.py
--rw-r--r--   0 root         (0) root         (0)    53311 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/core_aivr_session.py
--rw-r--r--   0 root         (0) root         (0)    39350 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/core_aivr_session_telco_data.py
--rw-r--r--   0 root         (0) root         (0)    31030 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/cr_question_id_for_cr_config.py
--rw-r--r--   0 root         (0) root         (0)    29555 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/creating_entity.py
--rw-r--r--   0 root         (0) root         (0)    31240 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/criterion_config.py
--rw-r--r--   0 root         (0) root         (0)    31141 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/criterion_satisfied.py
--rw-r--r--   0 root         (0) root         (0)    30067 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_obj_ref.py
--rw-r--r--   0 root         (0) root         (0)    44592 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object.py
--rw-r--r--   0 root         (0) root         (0)    30061 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_all_of.py
--rw-r--r--   0 root         (0) root         (0)    38589 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_base.py
--rw-r--r--   0 root         (0) root         (0)    34950 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_ids.py
--rw-r--r--   0 root         (0) root         (0)    44371 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref.py
--rw-r--r--   0 root         (0) root         (0)    46694 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref_presigned_s3.py
--rw-r--r--   0 root         (0) root         (0)    31271 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref_presigned_s3_all_of.py
--rw-r--r--   0 root         (0) root         (0)    39562 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/data_object_with_audio.py
--rw-r--r--   0 root         (0) root         (0)    30005 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/debug_info.py
--rw-r--r--   0 root         (0) root         (0)    30855 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/debug_settings.py
--rw-r--r--   0 root         (0) root         (0)    32610 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/demo.py
--rw-r--r--   0 root         (0) root         (0)    32690 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/demo_all_of.py
--rw-r--r--   0 root         (0) root         (0)    30997 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/diarization_data.py
--rw-r--r--   0 root         (0) root         (0)    30866 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/diarization_zone.py
--rw-r--r--   0 root         (0) root         (0)    36062 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/diarization_zone_item.py
--rw-r--r--   0 root         (0) root         (0)    32728 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/disconnect.py
--rw-r--r--   0 root         (0) root         (0)    32808 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/disconnect_all_of.py
--rw-r--r--   0 root         (0) root         (0)    31060 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/error.py
--rw-r--r--   0 root         (0) root         (0)    31120 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/error_all_of.py
--rw-r--r--   0 root         (0) root         (0)    31108 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/error_info.py
--rw-r--r--   0 root         (0) root         (0)    31669 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/estimated_queue_wait.py
--rw-r--r--   0 root         (0) root         (0)    29610 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/experiment_platform.py
--rw-r--r--   0 root         (0) root         (0)    31771 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/extended_summary_item.py
--rw-r--r--   0 root         (0) root         (0)    32083 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/file_location.py
--rw-r--r--   0 root         (0) root         (0)    36031 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/formatter.py
--rw-r--r--   0 root         (0) root         (0)    30985 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/grammar.py
--rw-r--r--   0 root         (0) root         (0)    30292 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg.py
--rw-r--r--   0 root         (0) root         (0)    30332 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_all_of.py
--rw-r--r--   0 root         (0) root         (0)    37443 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio.py
--rw-r--r--   0 root         (0) root         (0)    31308 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_all_of.py
--rw-r--r--   0 root         (0) root         (0)    32953 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_base.py
--rw-r--r--   0 root         (0) root         (0)    33958 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_base_with_audio.py
--rw-r--r--   0 root         (0) root         (0)    30298 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_id.py
--rw-r--r--   0 root         (0) root         (0)    30950 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input.py
--rw-r--r--   0 root         (0) root         (0)    30280 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_audio_hash.py
--rw-r--r--   0 root         (0) root         (0)    30198 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_audio_id.py
--rw-r--r--   0 root         (0) root         (0)    30225 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_data.py
--rw-r--r--   0 root         (0) root         (0)    34305 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set.py
--rw-r--r--   0 root         (0) root         (0)    31628 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_base.py
--rw-r--r--   0 root         (0) root         (0)    31701 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_base_inclusive.py
--rw-r--r--   0 root         (0) root         (0)    32541 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_core.py
--rw-r--r--   0 root         (0) root         (0)    30305 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_id.py
--rw-r--r--   0 root         (0) root         (0)    32570 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inclusive.py
--rw-r--r--   0 root         (0) root         (0)    32650 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inclusive_core.py
--rw-r--r--   0 root         (0) root         (0)    32561 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inner.py
--rw-r--r--   0 root         (0) root         (0)    31399 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_response.py
--rw-r--r--   0 root         (0) root         (0)    35767 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_thin.py
--rw-r--r--   0 root         (0) root         (0)    38911 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment.py
--rw-r--r--   0 root         (0) root         (0)    36268 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base.py
--rw-r--r--   0 root         (0) root         (0)    35004 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base_inclusive.py
--rw-r--r--   0 root         (0) root         (0)    31959 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base_platform_data.py
--rw-r--r--   0 root         (0) root         (0)    30343 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_id.py
--rw-r--r--   0 root         (0) root         (0)    37771 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_inclusive.py
--rw-r--r--   0 root         (0) root         (0)    35942 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    35566 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_external_asr.py
--rw-r--r--   0 root         (0) root         (0)    30609 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_upload.py
--rw-r--r--   0 root         (0) root         (0)    31321 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_voicegain.py
--rw-r--r--   0 root         (0) root         (0)    31427 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_response.py
--rw-r--r--   0 root         (0) root         (0)    29711 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_status.py
--rw-r--r--   0 root         (0) root         (0)    29640 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_status_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    34622 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar.py
--rw-r--r--   0 root         (0) root         (0)    31894 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_base.py
--rw-r--r--   0 root         (0) root         (0)    30898 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_base_light.py
--rw-r--r--   0 root         (0) root         (0)    30360 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_id.py
--rw-r--r--   0 root         (0) root         (0)    31826 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_inner.py
--rw-r--r--   0 root         (0) root         (0)    33702 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_light.py
--rw-r--r--   0 root         (0) root         (0)    31011 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_interpretation.py
--rw-r--r--   0 root         (0) root         (0)    35241 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_question.py
--rw-r--r--   0 root         (0) root         (0)    32494 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_question_base.py
--rw-r--r--   0 root         (0) root         (0)    30391 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_question_id.py
--rw-r--r--   0 root         (0) root         (0)    33517 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_question_inner.py
--rw-r--r--   0 root         (0) root         (0)    31237 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
--rw-r--r--   0 root         (0) root         (0)    33713 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
--rw-r--r--   0 root         (0) root         (0)    31150 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
--rw-r--r--   0 root         (0) root         (0)    31080 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
--rw-r--r--   0 root         (0) root         (0)    30354 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_with_exp.py
--rw-r--r--   0 root         (0) root         (0)    37203 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition.py
--rw-r--r--   0 root         (0) root         (0)    34495 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition_base.py
--rw-r--r--   0 root         (0) root         (0)    30372 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition_id.py
--rw-r--r--   0 root         (0) root         (0)    29659 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_review_status.py
--rw-r--r--   0 root         (0) root         (0)    32622 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_source_of_truth.py
--rw-r--r--   0 root         (0) root         (0)    33496 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_truth_update.py
--rw-r--r--   0 root         (0) root         (0)    33256 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/greg_truth_updates.py
--rw-r--r--   0 root         (0) root         (0)    32241 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/grxml.py
--rw-r--r--   0 root         (0) root         (0)    32341 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/grxml_all_of.py
--rw-r--r--   0 root         (0) root         (0)    30750 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/gui_input.py
--rw-r--r--   0 root         (0) root         (0)    29368 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/hangup.py
--rw-r--r--   0 root         (0) root         (0)    30040 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/html_checkbox.py
--rw-r--r--   0 root         (0) root         (0)    31854 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/html_choice_item.py
--rw-r--r--   0 root         (0) root         (0)    30072 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/html_radio_buttons.py
--rw-r--r--   0 root         (0) root         (0)    30135 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/html_text_entry.py
--rw-r--r--   0 root         (0) root         (0)    29528 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/if_exists.py
--rw-r--r--   0 root         (0) root         (0)    33552 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/incident.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/inline_data.py
--rw-r--r--   0 root         (0) root         (0)    31264 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/inline_object.py
--rw-r--r--   0 root         (0) root         (0)    31276 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/inline_object1.py
--rw-r--r--   0 root         (0) root         (0)    34679 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/input.py
--rw-r--r--   0 root         (0) root         (0)    34819 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/input_all_of.py
--rw-r--r--   0 root         (0) root         (0)    30979 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/integration.py
--rw-r--r--   0 root         (0) root         (0)    36155 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/jjsgf.py
--rw-r--r--   0 root         (0) root         (0)    36295 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/jjsgf_all_of.py
--rw-r--r--   0 root         (0) root         (0)    33096 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/joined_meeting_event.py
--rw-r--r--   0 root         (0) root         (0)    31446 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_example.py
--rw-r--r--   0 root         (0) root         (0)    31431 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_group.py
--rw-r--r--   0 root         (0) root         (0)    33174 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_item.py
--rw-r--r--   0 root         (0) root         (0)    31976 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/language.py
--rw-r--r--   0 root         (0) root         (0)    37812 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_add_audio_request.py
--rw-r--r--   0 root         (0) root         (0)    55084 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_data.py
--rw-r--r--   0 root         (0) root         (0)    34548 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_data_audio_channels.py
--rw-r--r--   0 root         (0) root         (0)    34029 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_data_chat.py
--rw-r--r--   0 root         (0) root         (0)    30120 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_field.py
--rw-r--r--   0 root         (0) root         (0)    44722 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_join_request.py
--rw-r--r--   0 root         (0) root         (0)    30276 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_keyword_data.py
--rw-r--r--   0 root         (0) root         (0)    32983 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_minutes.py
--rw-r--r--   0 root         (0) root         (0)    37895 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_minutes_section.py
--rw-r--r--   0 root         (0) root         (0)    30266 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_phrase_data.py
--rw-r--r--   0 root         (0) root         (0)    40441 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_search_field.py
--rw-r--r--   0 root         (0) root         (0)    42117 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_speaker_result.py
--rw-r--r--   0 root         (0) root         (0)    51286 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_poll_result.py
--rw-r--r--   0 root         (0) root         (0)    30754 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_poll_result_all_of.py
--rw-r--r--   0 root         (0) root         (0)    50424 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_result_reference.py
--rw-r--r--   0 root         (0) root         (0)    51053 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_search_result.py
--rw-r--r--   0 root         (0) root         (0)    30369 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_search_result_all_of.py
--rw-r--r--   0 root         (0) root         (0)    38226 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_word_item_timed_with_annot.py
--rw-r--r--   0 root         (0) root         (0)    33792 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_item.py
--rw-r--r--   0 root         (0) root         (0)    37261 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_section_with_annot.py
--rw-r--r--   0 root         (0) root         (0)    30413 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_section_words_with_annot.py
--rw-r--r--   0 root         (0) root         (0)    30191 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/min_max_speakers.py
--rw-r--r--   0 root         (0) root         (0)    33032 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/min_max_speakers_diarization.py
--rw-r--r--   0 root         (0) root         (0)    38338 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/modifiable_meeting_data.py
--rw-r--r--   0 root         (0) root         (0)    35000 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/modifiable_meeting_data_response.py
--rw-r--r--   0 root         (0) root         (0)    29681 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/mood_type.py
--rw-r--r--   0 root         (0) root         (0)    31524 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/mrc_pv1_asr_settings.py
--rw-r--r--   0 root         (0) root         (0)    31497 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/mrc_pv2_asr_settings.py
--rw-r--r--   0 root         (0) root         (0)    29528 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/mrcp_version.py
--rw-r--r--   0 root         (0) root         (0)    33369 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/multipart_form_data_field.py
--rw-r--r--   0 root         (0) root         (0)    32011 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/name_value_pair.py
--rw-r--r--   0 root         (0) root         (0)    31023 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/named_entity_concept.py
--rw-r--r--   0 root         (0) root         (0)    30144 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/named_entity_type.py
--rw-r--r--   0 root         (0) root         (0)    35585 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/named_speaker.py
--rw-r--r--   0 root         (0) root         (0)    49908 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session.py
--rw-r--r--   0 root         (0) root         (0)    38322 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py
--rw-r--r--   0 root         (0) root         (0)    30261 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
--rw-r--r--   0 root         (0) root         (0)    30909 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response.py
--rw-r--r--   0 root         (0) root         (0)    29448 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response400.py
--rw-r--r--   0 root         (0) root         (0)    29448 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response401.py
--rw-r--r--   0 root         (0) root         (0)    32943 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/non_speaking_participant.py
--rw-r--r--   0 root         (0) root         (0)    32178 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/offline_progress.py
--rw-r--r--   0 root         (0) root         (0)    32342 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/output.py
--rw-r--r--   0 root         (0) root         (0)    32422 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/output_all_of.py
--rw-r--r--   0 root         (0) root         (0)    34624 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/overtalk.py
--rw-r--r--   0 root         (0) root         (0)    39959 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/performed_redaction.py
--rw-r--r--   0 root         (0) root         (0)    32816 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phone_audio_input.py
--rw-r--r--   0 root         (0) root         (0)    31034 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phone_audio_input_prompt.py
--rw-r--r--   0 root         (0) root         (0)    33665 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_example.py
--rw-r--r--   0 root         (0) root         (0)    33531 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_group.py
--rw-r--r--   0 root         (0) root         (0)    41220 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item.py
--rw-r--r--   0 root         (0) root         (0)    32495 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_location.py
--rw-r--r--   0 root         (0) root         (0)    32275 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py
--rw-r--r--   0 root         (0) root         (0)    31135 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_slots.py
--rw-r--r--   0 root         (0) root         (0)    33071 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/pii_redaction_conf.py
--rw-r--r--   0 root         (0) root         (0)    33877 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/poll_req.py
--rw-r--r--   0 root         (0) root         (0)    33653 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/poll_resp.py
--rw-r--r--   0 root         (0) root         (0)    33619 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/portal_output_init.py
--rw-r--r--   0 root         (0) root         (0)    30408 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/pre_fetch.py
--rw-r--r--   0 root         (0) root         (0)    34475 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/presigned_data_file_url_response.py
--rw-r--r--   0 root         (0) root         (0)    41077 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/progress.py
--rw-r--r--   0 root         (0) root         (0)    31893 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/progress_callback.py
--rw-r--r--   0 root         (0) root         (0)    29815 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/progress_phase.py
--rw-r--r--   0 root         (0) root         (0)    32937 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/quartiles_energy.py
--rw-r--r--   0 root         (0) root         (0)    32913 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/quartiles_pitch.py
--rw-r--r--   0 root         (0) root         (0)    31562 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/query.py
--rw-r--r--   0 root         (0) root         (0)    34722 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/reco_alt.py
--rw-r--r--   0 root         (0) root         (0)    31923 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/recog_nlsml.py
--rw-r--r--   0 root         (0) root         (0)    31093 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/recog_nlsml_no_exp.py
--rw-r--r--   0 root         (0) root         (0)    34187 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/recog_obj.py
--rw-r--r--   0 root         (0) root         (0)    33425 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/recog_obj_no_exp.py
--rw-r--r--   0 root         (0) root         (0)    34086 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/recognition_result.py
--rw-r--r--   0 root         (0) root         (0)    34795 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/requested_content.py
--rw-r--r--   0 root         (0) root         (0)    34220 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/resource_uri.py
--rw-r--r--   0 root         (0) root         (0)    34702 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/resource_uri_local_auth_conf.py
--rw-r--r--   0 root         (0) root         (0)    29618 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/results_websocket_mode.py
--rw-r--r--   0 root         (0) root         (0)    35265 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/s3.py
--rw-r--r--   0 root         (0) root         (0)    35425 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/s3_all_of.py
--rw-r--r--   0 root         (0) root         (0)    35382 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/s3_audio_input.py
--rw-r--r--   0 root         (0) root         (0)    31633 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/s3_metadata_mapping.py
--rw-r--r--   0 root         (0) root         (0)    31411 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/s3_tag_mapping.py
--rw-r--r--   0 root         (0) root         (0)    29545 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sa_conf_type.py
--rw-r--r--   0 root         (0) root         (0)    29664 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sample_rate.py
--rw-r--r--   0 root         (0) root         (0)    35624 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sentence_hypothesis_or_recognition.py
--rw-r--r--   0 root         (0) root         (0)    31058 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sentence_hypothesis_or_recognition_all_of.py
--rw-r--r--   0 root         (0) root         (0)    34081 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sentence_recognition.py
--rw-r--r--   0 root         (0) root         (0)    30241 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_content.py
--rw-r--r--   0 root         (0) root         (0)    31753 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_error_response.py
--rw-r--r--   0 root         (0) root         (0)    37769 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_init_recognition.py
--rw-r--r--   0 root         (0) root         (0)    40011 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_init_transcription.py
--rw-r--r--   0 root         (0) root         (0)    33173 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_init_transcription_diarization.py
--rw-r--r--   0 root         (0) root         (0)    30975 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/session_success_response.py
--rw-r--r--   0 root         (0) root         (0)    35584 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/settings_async_transcription.py
--rw-r--r--   0 root         (0) root         (0)    32505 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/settings_recognition.py
--rw-r--r--   0 root         (0) root         (0)    32478 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/settings_sync_transcription.py
--rw-r--r--   0 root         (0) root         (0)    34490 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/silence.py
--rw-r--r--   0 root         (0) root         (0)    31136 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/slot_entity.py
--rw-r--r--   0 root         (0) root         (0)    31083 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/slot_keyword.py
--rw-r--r--   0 root         (0) root         (0)    31170 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sos_ref.py
--rw-r--r--   0 root         (0) root         (0)    32480 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speaker_activity.py
--rw-r--r--   0 root         (0) root         (0)    33829 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speaker_result.py
--rw-r--r--   0 root         (0) root         (0)    31830 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speaker_with_percent_spoken.py
--rw-r--r--   0 root         (0) root         (0)    44637 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_base_result.py
--rw-r--r--   0 root         (0) root         (0)    32312 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel.py
--rw-r--r--   0 root         (0) root         (0)    46010 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel_result.py
--rw-r--r--   0 root         (0) root         (0)    34296 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
--rw-r--r--   0 root         (0) root         (0)    71068 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config.py
--rw-r--r--   0 root         (0) root         (0)    34754 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_identifying.py
--rw-r--r--   0 root         (0) root         (0)    68343 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    67063 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py
--rw-r--r--   0 root         (0) root         (0)    31621 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
--rw-r--r--   0 root         (0) root         (0)    31164 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_name_optional.py
--rw-r--r--   0 root         (0) root         (0)    31318 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_name_required.py
--rw-r--r--   0 root         (0) root         (0)    50364 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_core_result.py
--rw-r--r--   0 root         (0) root         (0)    35291 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_core_result_all_of.py
--rw-r--r--   0 root         (0) root         (0)    31230 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_criteria_data.py
--rw-r--r--   0 root         (0) root         (0)    31695 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion.py
--rw-r--r--   0 root         (0) root         (0)    30898 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion_data.py
--rw-r--r--   0 root         (0) root         (0)    37019 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion_item.py
--rw-r--r--   0 root         (0) root         (0)    30944 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword.py
--rw-r--r--   0 root         (0) root         (0)    31234 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_data.py
--rw-r--r--   0 root         (0) root         (0)    36268 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item.py
--rw-r--r--   0 root         (0) root         (0)    36520 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
--rw-r--r--   0 root         (0) root         (0)    32782 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
--rw-r--r--   0 root         (0) root         (0)    31914 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity.py
--rw-r--r--   0 root         (0) root         (0)    37318 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item.py
--rw-r--r--   0 root         (0) root         (0)    37606 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
--rw-r--r--   0 root         (0) root         (0)    33856 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
--rw-r--r--   0 root         (0) root         (0)    33000 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase.py
--rw-r--r--   0 root         (0) root         (0)    31217 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_data.py
--rw-r--r--   0 root         (0) root         (0)    33115 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_for_ws.py
--rw-r--r--   0 root         (0) root         (0)    31204 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
--rw-r--r--   0 root         (0) root         (0)    31043 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group.py
--rw-r--r--   0 root         (0) root         (0)    31316 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_data.py
--rw-r--r--   0 root         (0) root         (0)    31076 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
--rw-r--r--   0 root         (0) root         (0)    36431 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_item.py
--rw-r--r--   0 root         (0) root         (0)    38340 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_item.py
--rw-r--r--   0 root         (0) root         (0)    39740 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
--rw-r--r--   0 root         (0) root         (0)    31114 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_slots.py
--rw-r--r--   0 root         (0) root         (0)    61344 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_result.py
--rw-r--r--   0 root         (0) root         (0)    46671 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_result_detail.py
--rw-r--r--   0 root         (0) root         (0)    31129 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_session_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    38064 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_session_poll_response.py
--rw-r--r--   0 root         (0) root         (0)    36359 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_websocket_payload.py
--rw-r--r--   0 root         (0) root         (0)    31766 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/start_end_time_for_sub_criterion.py
--rw-r--r--   0 root         (0) root         (0)    30452 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ping.py
--rw-r--r--   0 root         (0) root         (0)    33072 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_word_correction.py
--rw-r--r--   0 root         (0) root         (0)    31291 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_word_correction_all_of.py
--rw-r--r--   0 root         (0) root         (0)    37091 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word.py
--rw-r--r--   0 root         (0) root         (0)    31229 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_all_of.py
--rw-r--r--   0 root         (0) root         (0)    35386 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base.py
--rw-r--r--   0 root         (0) root         (0)    31248 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base_all_of.py
--rw-r--r--   0 root         (0) root         (0)    33782 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base_without_spk.py
--rw-r--r--   0 root         (0) root         (0)    35658 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stream_resp.py
--rw-r--r--   0 root         (0) root         (0)    35728 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/stream_setup.py
--rw-r--r--   0 root         (0) root         (0)    29711 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/streaming_protocol.py
--rw-r--r--   0 root         (0) root         (0)    38851 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sub_criterion_config.py
--rw-r--r--   0 root         (0) root         (0)    41237 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sub_criterion_satisfied.py
--rw-r--r--   0 root         (0) root         (0)    32212 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_audio_input_source.py
--rw-r--r--   0 root         (0) root         (0)    31160 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_recognition_request.py
--rw-r--r--   0 root         (0) root         (0)    32725 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_recognition_response.py
--rw-r--r--   0 root         (0) root         (0)    30328 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_session_established.py
--rw-r--r--   0 root         (0) root         (0)    31044 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_request.py
--rw-r--r--   0 root         (0) root         (0)    32783 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_response.py
--rw-r--r--   0 root         (0) root         (0)    33222 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_result.py
--rw-r--r--   0 root         (0) root         (0)    38938 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/talk_time.py
--rw-r--r--   0 root         (0) root         (0)    32688 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/timed_sentence.py
--rw-r--r--   0 root         (0) root         (0)    32843 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/timeline_speaker.py
--rw-r--r--   0 root         (0) root         (0)    31469 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/topic_score.py
--rw-r--r--   0 root         (0) root         (0)    29568 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_bucket_type.py
--rw-r--r--   0 root         (0) root         (0)    39210 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc.py
--rw-r--r--   0 root         (0) root         (0)    31128 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc_defaults.py
--rw-r--r--   0 root         (0) root         (0)    36588 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc_statistics.py
--rw-r--r--   0 root         (0) root         (0)    34662 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_key.py
--rw-r--r--   0 root         (0) root         (0)    33912 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    29660 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_status.py
--rw-r--r--   0 root         (0) root         (0)    29700 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_status_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    29588 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/training_set_store_type.py
--rw-r--r--   0 root         (0) root         (0)    31830 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_alt.py
--rw-r--r--   0 root         (0) root         (0)    49204 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request.py
--rw-r--r--   0 root         (0) root         (0)    32616 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_audio.py
--rw-r--r--   0 root         (0) root         (0)    33150 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_diarization.py
--rw-r--r--   0 root         (0) root         (0)    34110 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_settings.py
--rw-r--r--   0 root         (0) root         (0)    30705 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_source.py
--rw-r--r--   0 root         (0) root         (0)    30351 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_response.py
--rw-r--r--   0 root         (0) root         (0)    31112 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_id.py
--rw-r--r--   0 root         (0) root         (0)    34130 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request.py
--rw-r--r--   0 root         (0) root         (0)    31807 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request_mute.py
--rw-r--r--   0 root         (0) root         (0)    30635 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request_pause.py
--rw-r--r--   0 root         (0) root         (0)    34664 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range.py
--rw-r--r--   0 root         (0) root         (0)    34844 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range_for_phrase.py
--rw-r--r--   0 root         (0) root         (0)    36080 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
--rw-r--r--   0 root         (0) root         (0)    36401 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transfer.py
--rw-r--r--   0 root         (0) root         (0)    36541 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/transfer_all_of.py
--rw-r--r--   0 root         (0) root         (0)    35969 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence.py
--rw-r--r--   0 root         (0) root         (0)    33589 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_justification.py
--rw-r--r--   0 root         (0) root         (0)    37229 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection.py
--rw-r--r--   0 root         (0) root         (0)    30332 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection_all_of.py
--rw-r--r--   0 root         (0) root         (0)    33869 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection_all_of_rejection.py
--rw-r--r--   0 root         (0) root         (0)    29584 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/vad_mode.py
--rw-r--r--   0 root         (0) root         (0)    32389 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/version.py
--rw-r--r--   0 root         (0) root         (0)    38041 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket.py
--rw-r--r--   0 root         (0) root         (0)    41095 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_init.py
--rw-r--r--   0 root         (0) root         (0)    30602 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_init_reco.py
--rw-r--r--   0 root         (0) root         (0)    36197 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_modifiable.py
--rw-r--r--   0 root         (0) root         (0)    32665 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_msg.py
--rw-r--r--   0 root         (0) root         (0)    29531 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_protocol.py
--rw-r--r--   0 root         (0) root         (0)    31006 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/websocket_resp.py
--rw-r--r--   0 root         (0) root         (0)    30363 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_alternatives.py
--rw-r--r--   0 root         (0) root         (0)    31543 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_cloud_item.py
--rw-r--r--   0 root         (0) root         (0)    31384 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_correction.py
--rw-r--r--   0 root         (0) root         (0)    33618 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_item_annotation.py
--rw-r--r--   0 root         (0) root         (0)    30410 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_item_annotations.py
--rw-r--r--   0 root         (0) root         (0)    36394 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_item_timed.py
--rw-r--r--   0 root         (0) root         (0)    31469 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_item_timing.py
--rw-r--r--   0 root         (0) root         (0)    30724 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_tree_ids.py
--rw-r--r--   0 root         (0) root         (0)    36771 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/word_tree_item.py
--rw-r--r--   0 root         (0) root         (0)    33326 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_item.py
--rw-r--r--   0 root         (0) root         (0)    36629 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section.py
--rw-r--r--   0 root         (0) root         (0)    33175 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta.py
--rw-r--r--   0 root         (0) root         (0)    32177 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta_mc.py
--rw-r--r--   0 root         (0) root         (0)    33423 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta_meeting.py
--rw-r--r--   0 root         (0) root         (0)    34156 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section_single_column.py
--rw-r--r--   0 root         (0) root         (0)    30237 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_section_words.py
--rw-r--r--   0 root         (0) root         (0)    44270 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/words_websocket_item.py
--rw-r--r--   0 root         (0) root         (0)    33913 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_emotion_item.py
--rw-r--r--   0 root         (0) root         (0)    33162 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_keyword_item.py
--rw-r--r--   0 root         (0) root         (0)    34152 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_named_entity_item.py
--rw-r--r--   0 root         (0) root         (0)    32386 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_group_item.py
--rw-r--r--   0 root         (0) root         (0)    35165 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_item.py
--rw-r--r--   0 root         (0) root         (0)    35517 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
--rw-r--r--   0 root         (0) root         (0)    31738 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range.py
--rw-r--r--   0 root         (0) root         (0)    30922 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range_nested.py
--rw-r--r--   0 root         (0) root         (0)    30910 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range_no_spk.py
--rw-r--r--   0 root         (0) root         (0)    37543 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
--rw-r--r--   0 root         (0) root         (0)    31387 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
--rw-r--r--   0 root         (0) root         (0)    32720 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_speaker.py
--rw-r--r--   0 root         (0) root         (0)    34580 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_word.py
--rw-r--r--   0 root         (0) root         (0)    32146 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/models/ws_word_edit.py
--rw-r--r--   0 root         (0) root         (0)    39207 2024-02-14 06:55:54.000000 voicegain-speech-1.99.0/voicegain_speech/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-14 06:55:55.620951 voicegain-speech-1.99.0/voicegain_speech.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2936 2024-02-14 06:55:55.000000 voicegain-speech-1.99.0/voicegain_speech.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    26123 2024-02-14 06:55:55.000000 voicegain-speech-1.99.0/voicegain_speech.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-14 06:55:55.000000 voicegain-speech-1.99.0/voicegain_speech.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2024-02-14 06:55:55.000000 voicegain-speech-1.99.0/voicegain_speech.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-02-14 06:55:55.000000 voicegain-speech-1.99.0/voicegain_speech.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 22:21:36.728861 voicegain-speech-1.99.1/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-02-21 22:21:36.728861 voicegain-speech-1.99.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2504 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       79 2024-02-21 22:21:36.729861 voicegain-speech-1.99.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 22:21:36.611859 voicegain-speech-1.99.1/voicegain_speech/
+-rw-r--r--   0 root         (0) root         (0)    68395 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 22:21:36.615859 voicegain-speech-1.99.1/voicegain_speech/api/
+-rw-r--r--   0 root         (0) root         (0)      831 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33334 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/aivr_api.py
+-rw-r--r--   0 root         (0) root         (0)    52269 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/aivr_callback_api.py
+-rw-r--r--   0 root         (0) root         (0)    39277 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/asr_callback_api.py
+-rw-r--r--   0 root         (0) root         (0)    35241 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/audiocodes_api.py
+-rw-r--r--   0 root         (0) root         (0)   144142 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/data_api.py
+-rw-r--r--   0 root         (0) root         (0)   143692 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/greg_api.py
+-rw-r--r--   0 root         (0) root         (0)   140315 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/meeting_api.py
+-rw-r--r--   0 root         (0) root         (0)    48215 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/recognize_api.py
+-rw-r--r--   0 root         (0) root         (0)   119088 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/sa_api.py
+-rw-r--r--   0 root         (0) root         (0)    37228 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/security_api.py
+-rw-r--r--   0 root         (0) root         (0)    57407 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/training_api.py
+-rw-r--r--   0 root         (0) root         (0)   103284 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/transcribe_api.py
+-rw-r--r--   0 root         (0) root         (0)    55782 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api/websocket_api.py
+-rw-r--r--   0 root         (0) root         (0)    51992 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/api_client.py
+-rw-r--r--   0 root         (0) root         (0)    38452 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/configuration.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 22:21:36.728861 voicegain-speech-1.99.1/voicegain_speech/models/
+-rw-r--r--   0 root         (0) root         (0)    67201 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40185 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_control_messages.py
+-rw-r--r--   0 root         (0) root         (0)    31448 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_end.py
+-rw-r--r--   0 root         (0) root         (0)    31456 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_error.py
+-rw-r--r--   0 root         (0) root         (0)    31574 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_hypothesis.py
+-rw-r--r--   0 root         (0) root         (0)    30303 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_hypothesis_alternatives.py
+-rw-r--r--   0 root         (0) root         (0)    31544 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    31707 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_recognition_alternatives.py
+-rw-r--r--   0 root         (0) root         (0)    32581 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_response_messages.py
+-rw-r--r--   0 root         (0) root         (0)    39668 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_start.py
+-rw-r--r--   0 root         (0) root         (0)    31720 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_start_stt_speech_contexts.py
+-rw-r--r--   0 root         (0) root         (0)    30573 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_started.py
+-rw-r--r--   0 root         (0) root         (0)    30642 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ac_stop.py
+-rw-r--r--   0 root         (0) root         (0)    31320 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/account_and_context_id.py
+-rw-r--r--   0 root         (0) root         (0)    34223 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/advanced_regex.py
+-rw-r--r--   0 root         (0) root         (0)    30250 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aircall.py
+-rw-r--r--   0 root         (0) root         (0)    30290 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aircall_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    33370 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_core_response.py
+-rw-r--r--   0 root         (0) root         (0)    33490 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_core_response_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    36189 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response.py
+-rw-r--r--   0 root         (0) root         (0)    32419 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    31605 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response_final.py
+-rw-r--r--   0 root         (0) root         (0)    30267 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_conference_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    30925 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_disconnect.py
+-rw-r--r--   0 root         (0) root         (0)    35420 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_event.py
+-rw-r--r--   0 root         (0) root         (0)    29668 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_event_type.py
+-rw-r--r--   0 root         (0) root         (0)    33126 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_existing_session.py
+-rw-r--r--   0 root         (0) root         (0)    32738 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic.py
+-rw-r--r--   0 root         (0) root         (0)    29531 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_media.py
+-rw-r--r--   0 root         (0) root         (0)    31480 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    29617 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_type.py
+-rw-r--r--   0 root         (0) root         (0)    45552 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_new_session.py
+-rw-r--r--   0 root         (0) root         (0)    31022 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_phone_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    34959 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt.py
+-rw-r--r--   0 root         (0) root         (0)    30724 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_completion.py
+-rw-r--r--   0 root         (0) root         (0)    36415 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_playing.py
+-rw-r--r--   0 root         (0) root         (0)    30233 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_properties_audio.py
+-rw-r--r--   0 root         (0) root         (0)    30243 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_properties_html.py
+-rw-r--r--   0 root         (0) root         (0)    37845 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_question.py
+-rw-r--r--   0 root         (0) root         (0)    29628 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_recognition_result.py
+-rw-r--r--   0 root         (0) root         (0)    35695 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_recording.py
+-rw-r--r--   0 root         (0) root         (0)    42807 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_response_properties_audio.py
+-rw-r--r--   0 root         (0) root         (0)    31820 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_response_properties_html.py
+-rw-r--r--   0 root         (0) root         (0)    34490 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user.py
+-rw-r--r--   0 root         (0) root         (0)    30596 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user_base.py
+-rw-r--r--   0 root         (0) root         (0)    33362 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user_fs.py
+-rw-r--r--   0 root         (0) root         (0)    32062 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_transfer.py
+-rw-r--r--   0 root         (0) root         (0)    30314 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivr_vars.py
+-rw-r--r--   0 root         (0) root         (0)    32390 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/aivrs_question_specifics.py
+-rw-r--r--   0 root         (0) root         (0)    31670 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/answer_map_entry.py
+-rw-r--r--   0 root         (0) root         (0)    29622 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_event.py
+-rw-r--r--   0 root         (0) root         (0)    29713 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status.py
+-rw-r--r--   0 root         (0) root         (0)    29633 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_additional.py
+-rw-r--r--   0 root         (0) root         (0)    29688 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_after_input_started.py
+-rw-r--r--   0 root         (0) root         (0)    29715 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_for_callback.py
+-rw-r--r--   0 root         (0) root         (0)    29624 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_recognition_result.py
+-rw-r--r--   0 root         (0) root         (0)    45203 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_common.py
+-rw-r--r--   0 root         (0) root         (0)    35724 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_meeting_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    59219 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    54583 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    43620 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py
+-rw-r--r--   0 root         (0) root         (0)    38376 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_timeouts.py
+-rw-r--r--   0 root         (0) root         (0)    54671 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    62236 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_async.py
+-rw-r--r--   0 root         (0) root         (0)    31643 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    52690 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_common.py
+-rw-r--r--   0 root         (0) root         (0)    36523 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_common_lm.py
+-rw-r--r--   0 root         (0) root         (0)    34702 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py
+-rw-r--r--   0 root         (0) root         (0)    57940 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    53321 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_sa.py
+-rw-r--r--   0 root         (0) root         (0)    31829 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_speakers.py
+-rw-r--r--   0 root         (0) root         (0)    33246 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py
+-rw-r--r--   0 root         (0) root         (0)    34449 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/asr_transcribe_queue_status.py
+-rw-r--r--   0 root         (0) root         (0)    34178 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_audio_input_source.py
+-rw-r--r--   0 root         (0) root         (0)    29634 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_mode.py
+-rw-r--r--   0 root         (0) root         (0)    29678 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_mode_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    29595 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_mode_speech_analytics.py
+-rw-r--r--   0 root         (0) root         (0)    29641 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_mode_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    31815 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_post_response_base.py
+-rw-r--r--   0 root         (0) root         (0)    31210 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_post_response_base_audio.py
+-rw-r--r--   0 root         (0) root         (0)    32888 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_reco_post_response.py
+-rw-r--r--   0 root         (0) root         (0)    30565 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_reco_post_response_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    30477 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_callback_response.py
+-rw-r--r--   0 root         (0) root         (0)    32109 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_request.py
+-rw-r--r--   0 root         (0) root         (0)    32239 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_response.py
+-rw-r--r--   0 root         (0) root         (0)    34998 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_result.py
+-rw-r--r--   0 root         (0) root         (0)    30264 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_result_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    34598 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full.py
+-rw-r--r--   0 root         (0) root         (0)    32527 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    30937 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio.py
+-rw-r--r--   0 root         (0) root         (0)    37252 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py
+-rw-r--r--   0 root         (0) root         (0)    30351 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_source.py
+-rw-r--r--   0 root         (0) root         (0)    30363 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py
+-rw-r--r--   0 root         (0) root         (0)    44609 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_result.py
+-rw-r--r--   0 root         (0) root         (0)    33367 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental.py
+-rw-r--r--   0 root         (0) root         (0)    31184 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail.py
+-rw-r--r--   0 root         (0) root         (0)    31222 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_control_status.py
+-rw-r--r--   0 root         (0) root         (0)    39957 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_result.py
+-rw-r--r--   0 root         (0) root         (0)    34493 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py
+-rw-r--r--   0 root         (0) root         (0)    33369 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_session_established.py
+-rw-r--r--   0 root         (0) root         (0)    32751 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_session_short_info.py
+-rw-r--r--   0 root         (0) root         (0)    30378 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_session_url.py
+-rw-r--r--   0 root         (0) root         (0)    32946 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transc_post_response.py
+-rw-r--r--   0 root         (0) root         (0)    30599 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transc_post_response_sessions.py
+-rw-r--r--   0 root         (0) root         (0)    35444 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transc_session_established.py
+-rw-r--r--   0 root         (0) root         (0)    30405 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_callback_response.py
+-rw-r--r--   0 root         (0) root         (0)    32046 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_request.py
+-rw-r--r--   0 root         (0) root         (0)    31419 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_response.py
+-rw-r--r--   0 root         (0) root         (0)    31847 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_response_shared.py
+-rw-r--r--   0 root         (0) root         (0)    29598 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_channel.py
+-rw-r--r--   0 root         (0) root         (0)    29576 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_channel_selector.py
+-rw-r--r--   0 root         (0) root         (0)    29669 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_channel_selector_offline_async.py
+-rw-r--r--   0 root         (0) root         (0)    29530 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_channels.py
+-rw-r--r--   0 root         (0) root         (0)    30225 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_for_data_object.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_format.py
+-rw-r--r--   0 root         (0) root         (0)    34076 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async.py
+-rw-r--r--   0 root         (0) root         (0)    30291 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async_source.py
+-rw-r--r--   0 root         (0) root         (0)    35198 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async_with_callback.py
+-rw-r--r--   0 root         (0) root         (0)    33213 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_base.py
+-rw-r--r--   0 root         (0) root         (0)    30166 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_callback.py
+-rw-r--r--   0 root         (0) root         (0)    35329 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_callback_callback.py
+-rw-r--r--   0 root         (0) root         (0)    29400 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data.py
+-rw-r--r--   0 root         (0) root         (0)    31582 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    31482 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data_all_of_source.py
+-rw-r--r--   0 root         (0) root         (0)    35039 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_sync.py
+-rw-r--r--   0 root         (0) root         (0)    31298 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_input_sync_source.py
+-rw-r--r--   0 root         (0) root         (0)    35384 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_resource_uri.py
+-rw-r--r--   0 root         (0) root         (0)    29630 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_zone_class.py
+-rw-r--r--   0 root         (0) root         (0)    31541 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/audio_zone_item.py
+-rw-r--r--   0 root         (0) root         (0)    34154 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/base_sentence_hypothesis_or_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    31999 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/base_sentence_hypothesis_or_recognition_alternatives.py
+-rw-r--r--   0 root         (0) root         (0)    31289 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/base_stomp_word_correction.py
+-rw-r--r--   0 root         (0) root         (0)    30071 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/basic_success_response.py
+-rw-r--r--   0 root         (0) root         (0)    31573 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/builtin.py
+-rw-r--r--   0 root         (0) root         (0)    31633 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/builtin_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    29912 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    36627 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_review_answer_alone.py
+-rw-r--r--   0 root         (0) root         (0)    29561 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_review_answer_type.py
+-rw-r--r--   0 root         (0) root         (0)    34033 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base.py
+-rw-r--r--   0 root         (0) root         (0)    43494 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base_with_answer.py
+-rw-r--r--   0 root         (0) root         (0)    35791 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base_with_id.py
+-rw-r--r--   0 root         (0) root         (0)    35280 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/callback_req.py
+-rw-r--r--   0 root         (0) root         (0)    32038 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/callback_req_reco.py
+-rw-r--r--   0 root         (0) root         (0)    30199 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/callback_resp.py
+-rw-r--r--   0 root         (0) root         (0)    33981 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/caption.py
+-rw-r--r--   0 root         (0) root         (0)    31041 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/compliance_settings.py
+-rw-r--r--   0 root         (0) root         (0)    29591 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/config_value_status.py
+-rw-r--r--   0 root         (0) root         (0)    29684 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/content_type.py
+-rw-r--r--   0 root         (0) root         (0)    33108 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/continuous_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    53311 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/core_aivr_session.py
+-rw-r--r--   0 root         (0) root         (0)    39350 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/core_aivr_session_telco_data.py
+-rw-r--r--   0 root         (0) root         (0)    31030 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/cr_question_id_for_cr_config.py
+-rw-r--r--   0 root         (0) root         (0)    29555 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/creating_entity.py
+-rw-r--r--   0 root         (0) root         (0)    31240 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/criterion_config.py
+-rw-r--r--   0 root         (0) root         (0)    31141 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/criterion_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)    30067 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_obj_ref.py
+-rw-r--r--   0 root         (0) root         (0)    44592 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object.py
+-rw-r--r--   0 root         (0) root         (0)    30061 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    38589 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_base.py
+-rw-r--r--   0 root         (0) root         (0)    34950 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_ids.py
+-rw-r--r--   0 root         (0) root         (0)    44371 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref.py
+-rw-r--r--   0 root         (0) root         (0)    46694 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref_presigned_s3.py
+-rw-r--r--   0 root         (0) root         (0)    31271 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref_presigned_s3_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    39562 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/data_object_with_audio.py
+-rw-r--r--   0 root         (0) root         (0)    30005 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/debug_info.py
+-rw-r--r--   0 root         (0) root         (0)    30855 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/debug_settings.py
+-rw-r--r--   0 root         (0) root         (0)    32610 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/demo.py
+-rw-r--r--   0 root         (0) root         (0)    32690 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/demo_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    30997 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/diarization_data.py
+-rw-r--r--   0 root         (0) root         (0)    30866 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/diarization_zone.py
+-rw-r--r--   0 root         (0) root         (0)    36062 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/diarization_zone_item.py
+-rw-r--r--   0 root         (0) root         (0)    32728 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)    32808 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/disconnect_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    31060 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/error.py
+-rw-r--r--   0 root         (0) root         (0)    31120 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/error_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    31108 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/error_info.py
+-rw-r--r--   0 root         (0) root         (0)    31669 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/estimated_queue_wait.py
+-rw-r--r--   0 root         (0) root         (0)    29610 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/experiment_platform.py
+-rw-r--r--   0 root         (0) root         (0)    31771 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/extended_summary_item.py
+-rw-r--r--   0 root         (0) root         (0)    32083 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/file_location.py
+-rw-r--r--   0 root         (0) root         (0)    36031 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/formatter.py
+-rw-r--r--   0 root         (0) root         (0)    30985 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/grammar.py
+-rw-r--r--   0 root         (0) root         (0)    30292 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg.py
+-rw-r--r--   0 root         (0) root         (0)    30332 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    37443 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio.py
+-rw-r--r--   0 root         (0) root         (0)    31308 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    32953 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_base.py
+-rw-r--r--   0 root         (0) root         (0)    33958 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_base_with_audio.py
+-rw-r--r--   0 root         (0) root         (0)    30298 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_id.py
+-rw-r--r--   0 root         (0) root         (0)    30950 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input.py
+-rw-r--r--   0 root         (0) root         (0)    30280 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_audio_hash.py
+-rw-r--r--   0 root         (0) root         (0)    30198 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_audio_id.py
+-rw-r--r--   0 root         (0) root         (0)    30225 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_data.py
+-rw-r--r--   0 root         (0) root         (0)    34305 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set.py
+-rw-r--r--   0 root         (0) root         (0)    31628 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_base.py
+-rw-r--r--   0 root         (0) root         (0)    31701 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_base_inclusive.py
+-rw-r--r--   0 root         (0) root         (0)    32541 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_core.py
+-rw-r--r--   0 root         (0) root         (0)    30305 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_id.py
+-rw-r--r--   0 root         (0) root         (0)    32570 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inclusive.py
+-rw-r--r--   0 root         (0) root         (0)    32650 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inclusive_core.py
+-rw-r--r--   0 root         (0) root         (0)    32561 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inner.py
+-rw-r--r--   0 root         (0) root         (0)    31399 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_response.py
+-rw-r--r--   0 root         (0) root         (0)    35767 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_thin.py
+-rw-r--r--   0 root         (0) root         (0)    38911 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment.py
+-rw-r--r--   0 root         (0) root         (0)    36268 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base.py
+-rw-r--r--   0 root         (0) root         (0)    35004 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base_inclusive.py
+-rw-r--r--   0 root         (0) root         (0)    31959 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base_platform_data.py
+-rw-r--r--   0 root         (0) root         (0)    30343 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_id.py
+-rw-r--r--   0 root         (0) root         (0)    37771 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_inclusive.py
+-rw-r--r--   0 root         (0) root         (0)    35942 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    35566 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_external_asr.py
+-rw-r--r--   0 root         (0) root         (0)    30609 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_upload.py
+-rw-r--r--   0 root         (0) root         (0)    31321 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_voicegain.py
+-rw-r--r--   0 root         (0) root         (0)    31427 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_response.py
+-rw-r--r--   0 root         (0) root         (0)    29711 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_status.py
+-rw-r--r--   0 root         (0) root         (0)    29640 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_status_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    34622 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar.py
+-rw-r--r--   0 root         (0) root         (0)    31894 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_base.py
+-rw-r--r--   0 root         (0) root         (0)    30898 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_base_light.py
+-rw-r--r--   0 root         (0) root         (0)    30360 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_id.py
+-rw-r--r--   0 root         (0) root         (0)    31826 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_inner.py
+-rw-r--r--   0 root         (0) root         (0)    33702 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_light.py
+-rw-r--r--   0 root         (0) root         (0)    31011 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_interpretation.py
+-rw-r--r--   0 root         (0) root         (0)    35241 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_question.py
+-rw-r--r--   0 root         (0) root         (0)    32494 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_question_base.py
+-rw-r--r--   0 root         (0) root         (0)    30391 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_question_id.py
+-rw-r--r--   0 root         (0) root         (0)    33517 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_question_inner.py
+-rw-r--r--   0 root         (0) root         (0)    31237 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py
+-rw-r--r--   0 root         (0) root         (0)    33713 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py
+-rw-r--r--   0 root         (0) root         (0)    31150 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py
+-rw-r--r--   0 root         (0) root         (0)    31080 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py
+-rw-r--r--   0 root         (0) root         (0)    30354 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_with_exp.py
+-rw-r--r--   0 root         (0) root         (0)    37203 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    34495 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition_base.py
+-rw-r--r--   0 root         (0) root         (0)    30372 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition_id.py
+-rw-r--r--   0 root         (0) root         (0)    29659 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_review_status.py
+-rw-r--r--   0 root         (0) root         (0)    32622 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_source_of_truth.py
+-rw-r--r--   0 root         (0) root         (0)    33496 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_truth_update.py
+-rw-r--r--   0 root         (0) root         (0)    33256 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/greg_truth_updates.py
+-rw-r--r--   0 root         (0) root         (0)    32241 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/grxml.py
+-rw-r--r--   0 root         (0) root         (0)    32341 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/grxml_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    30750 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/gui_input.py
+-rw-r--r--   0 root         (0) root         (0)    29368 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/hangup.py
+-rw-r--r--   0 root         (0) root         (0)    30040 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/html_checkbox.py
+-rw-r--r--   0 root         (0) root         (0)    31854 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/html_choice_item.py
+-rw-r--r--   0 root         (0) root         (0)    30072 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/html_radio_buttons.py
+-rw-r--r--   0 root         (0) root         (0)    30135 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/html_text_entry.py
+-rw-r--r--   0 root         (0) root         (0)    29528 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/if_exists.py
+-rw-r--r--   0 root         (0) root         (0)    33552 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/incident.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/inline_data.py
+-rw-r--r--   0 root         (0) root         (0)    31264 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/inline_object.py
+-rw-r--r--   0 root         (0) root         (0)    31276 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/inline_object1.py
+-rw-r--r--   0 root         (0) root         (0)    34679 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/input.py
+-rw-r--r--   0 root         (0) root         (0)    34819 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/input_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    30979 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/integration.py
+-rw-r--r--   0 root         (0) root         (0)    36155 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/jjsgf.py
+-rw-r--r--   0 root         (0) root         (0)    36295 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/jjsgf_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    33096 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/joined_meeting_event.py
+-rw-r--r--   0 root         (0) root         (0)    31446 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_example.py
+-rw-r--r--   0 root         (0) root         (0)    31431 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_group.py
+-rw-r--r--   0 root         (0) root         (0)    33174 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_item.py
+-rw-r--r--   0 root         (0) root         (0)    31976 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/language.py
+-rw-r--r--   0 root         (0) root         (0)    37812 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_add_audio_request.py
+-rw-r--r--   0 root         (0) root         (0)    55084 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_data.py
+-rw-r--r--   0 root         (0) root         (0)    34548 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_data_audio_channels.py
+-rw-r--r--   0 root         (0) root         (0)    34029 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_data_chat.py
+-rw-r--r--   0 root         (0) root         (0)    30120 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_field.py
+-rw-r--r--   0 root         (0) root         (0)    44722 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_join_request.py
+-rw-r--r--   0 root         (0) root         (0)    30276 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_keyword_data.py
+-rw-r--r--   0 root         (0) root         (0)    32983 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_minutes.py
+-rw-r--r--   0 root         (0) root         (0)    37895 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_minutes_section.py
+-rw-r--r--   0 root         (0) root         (0)    30266 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_phrase_data.py
+-rw-r--r--   0 root         (0) root         (0)    40441 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_search_field.py
+-rw-r--r--   0 root         (0) root         (0)    42117 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_speaker_result.py
+-rw-r--r--   0 root         (0) root         (0)    51286 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_poll_result.py
+-rw-r--r--   0 root         (0) root         (0)    30754 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_poll_result_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    50424 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_result_reference.py
+-rw-r--r--   0 root         (0) root         (0)    51053 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_search_result.py
+-rw-r--r--   0 root         (0) root         (0)    30369 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_search_result_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    38226 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_word_item_timed_with_annot.py
+-rw-r--r--   0 root         (0) root         (0)    33792 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_item.py
+-rw-r--r--   0 root         (0) root         (0)    37261 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_section_with_annot.py
+-rw-r--r--   0 root         (0) root         (0)    30413 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_section_words_with_annot.py
+-rw-r--r--   0 root         (0) root         (0)    30191 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/min_max_speakers.py
+-rw-r--r--   0 root         (0) root         (0)    33032 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/min_max_speakers_diarization.py
+-rw-r--r--   0 root         (0) root         (0)    38338 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/modifiable_meeting_data.py
+-rw-r--r--   0 root         (0) root         (0)    35000 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/modifiable_meeting_data_response.py
+-rw-r--r--   0 root         (0) root         (0)    29681 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/mood_type.py
+-rw-r--r--   0 root         (0) root         (0)    31524 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/mrc_pv1_asr_settings.py
+-rw-r--r--   0 root         (0) root         (0)    31497 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/mrc_pv2_asr_settings.py
+-rw-r--r--   0 root         (0) root         (0)    29528 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/mrcp_version.py
+-rw-r--r--   0 root         (0) root         (0)    33369 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/multipart_form_data_field.py
+-rw-r--r--   0 root         (0) root         (0)    32011 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/name_value_pair.py
+-rw-r--r--   0 root         (0) root         (0)    31023 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/named_entity_concept.py
+-rw-r--r--   0 root         (0) root         (0)    30144 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/named_entity_type.py
+-rw-r--r--   0 root         (0) root         (0)    35585 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/named_speaker.py
+-rw-r--r--   0 root         (0) root         (0)    49908 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session.py
+-rw-r--r--   0 root         (0) root         (0)    38322 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py
+-rw-r--r--   0 root         (0) root         (0)    30261 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py
+-rw-r--r--   0 root         (0) root         (0)    30909 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response400.py
+-rw-r--r--   0 root         (0) root         (0)    29448 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response401.py
+-rw-r--r--   0 root         (0) root         (0)    32943 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/non_speaking_participant.py
+-rw-r--r--   0 root         (0) root         (0)    32178 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/offline_progress.py
+-rw-r--r--   0 root         (0) root         (0)    32342 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/output.py
+-rw-r--r--   0 root         (0) root         (0)    32422 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/output_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    34624 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/overtalk.py
+-rw-r--r--   0 root         (0) root         (0)    39959 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/performed_redaction.py
+-rw-r--r--   0 root         (0) root         (0)    32816 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phone_audio_input.py
+-rw-r--r--   0 root         (0) root         (0)    31034 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phone_audio_input_prompt.py
+-rw-r--r--   0 root         (0) root         (0)    33665 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_example.py
+-rw-r--r--   0 root         (0) root         (0)    33531 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_group.py
+-rw-r--r--   0 root         (0) root         (0)    41220 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item.py
+-rw-r--r--   0 root         (0) root         (0)    32495 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_location.py
+-rw-r--r--   0 root         (0) root         (0)    32275 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py
+-rw-r--r--   0 root         (0) root         (0)    31135 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_slots.py
+-rw-r--r--   0 root         (0) root         (0)    33071 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/pii_redaction_conf.py
+-rw-r--r--   0 root         (0) root         (0)    33877 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/poll_req.py
+-rw-r--r--   0 root         (0) root         (0)    33653 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/poll_resp.py
+-rw-r--r--   0 root         (0) root         (0)    33619 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/portal_output_init.py
+-rw-r--r--   0 root         (0) root         (0)    30408 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/pre_fetch.py
+-rw-r--r--   0 root         (0) root         (0)    34475 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/presigned_data_file_url_response.py
+-rw-r--r--   0 root         (0) root         (0)    41077 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/progress.py
+-rw-r--r--   0 root         (0) root         (0)    31893 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/progress_callback.py
+-rw-r--r--   0 root         (0) root         (0)    29815 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/progress_phase.py
+-rw-r--r--   0 root         (0) root         (0)    32937 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/quartiles_energy.py
+-rw-r--r--   0 root         (0) root         (0)    32913 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/quartiles_pitch.py
+-rw-r--r--   0 root         (0) root         (0)    31562 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/query.py
+-rw-r--r--   0 root         (0) root         (0)    34722 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/reco_alt.py
+-rw-r--r--   0 root         (0) root         (0)    31923 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/recog_nlsml.py
+-rw-r--r--   0 root         (0) root         (0)    31093 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/recog_nlsml_no_exp.py
+-rw-r--r--   0 root         (0) root         (0)    34187 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/recog_obj.py
+-rw-r--r--   0 root         (0) root         (0)    33425 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/recog_obj_no_exp.py
+-rw-r--r--   0 root         (0) root         (0)    34086 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/recognition_result.py
+-rw-r--r--   0 root         (0) root         (0)    34795 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/requested_content.py
+-rw-r--r--   0 root         (0) root         (0)    34220 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/resource_uri.py
+-rw-r--r--   0 root         (0) root         (0)    34702 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/resource_uri_local_auth_conf.py
+-rw-r--r--   0 root         (0) root         (0)    29618 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/results_websocket_mode.py
+-rw-r--r--   0 root         (0) root         (0)    35265 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/s3.py
+-rw-r--r--   0 root         (0) root         (0)    35425 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/s3_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    35382 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/s3_audio_input.py
+-rw-r--r--   0 root         (0) root         (0)    31633 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/s3_metadata_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    31411 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/s3_tag_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    29545 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sa_conf_type.py
+-rw-r--r--   0 root         (0) root         (0)    29664 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sample_rate.py
+-rw-r--r--   0 root         (0) root         (0)    35624 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    31058 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sentence_hypothesis_or_recognition_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    34081 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sentence_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    30241 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_content.py
+-rw-r--r--   0 root         (0) root         (0)    31753 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_error_response.py
+-rw-r--r--   0 root         (0) root         (0)    37769 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_init_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    40011 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_init_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    33173 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_init_transcription_diarization.py
+-rw-r--r--   0 root         (0) root         (0)    30975 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/session_success_response.py
+-rw-r--r--   0 root         (0) root         (0)    35584 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/settings_async_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    32505 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/settings_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    32478 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/settings_sync_transcription.py
+-rw-r--r--   0 root         (0) root         (0)    34490 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/silence.py
+-rw-r--r--   0 root         (0) root         (0)    31136 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/slot_entity.py
+-rw-r--r--   0 root         (0) root         (0)    31083 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/slot_keyword.py
+-rw-r--r--   0 root         (0) root         (0)    31170 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sos_ref.py
+-rw-r--r--   0 root         (0) root         (0)    32480 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speaker_activity.py
+-rw-r--r--   0 root         (0) root         (0)    33829 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speaker_result.py
+-rw-r--r--   0 root         (0) root         (0)    31830 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speaker_with_percent_spoken.py
+-rw-r--r--   0 root         (0) root         (0)    44637 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_base_result.py
+-rw-r--r--   0 root         (0) root         (0)    32312 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel.py
+-rw-r--r--   0 root         (0) root         (0)    46010 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel_result.py
+-rw-r--r--   0 root         (0) root         (0)    34296 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py
+-rw-r--r--   0 root         (0) root         (0)    71068 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config.py
+-rw-r--r--   0 root         (0) root         (0)    34754 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_identifying.py
+-rw-r--r--   0 root         (0) root         (0)    68343 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    67063 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py
+-rw-r--r--   0 root         (0) root         (0)    31621 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py
+-rw-r--r--   0 root         (0) root         (0)    31164 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_name_optional.py
+-rw-r--r--   0 root         (0) root         (0)    31318 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_name_required.py
+-rw-r--r--   0 root         (0) root         (0)    50364 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_core_result.py
+-rw-r--r--   0 root         (0) root         (0)    35291 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_core_result_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    31230 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_criteria_data.py
+-rw-r--r--   0 root         (0) root         (0)    31695 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion.py
+-rw-r--r--   0 root         (0) root         (0)    30898 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion_data.py
+-rw-r--r--   0 root         (0) root         (0)    37019 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion_item.py
+-rw-r--r--   0 root         (0) root         (0)    30944 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword.py
+-rw-r--r--   0 root         (0) root         (0)    31234 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_data.py
+-rw-r--r--   0 root         (0) root         (0)    36268 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item.py
+-rw-r--r--   0 root         (0) root         (0)    36520 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py
+-rw-r--r--   0 root         (0) root         (0)    32782 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py
+-rw-r--r--   0 root         (0) root         (0)    31914 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity.py
+-rw-r--r--   0 root         (0) root         (0)    37318 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item.py
+-rw-r--r--   0 root         (0) root         (0)    37606 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py
+-rw-r--r--   0 root         (0) root         (0)    33856 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py
+-rw-r--r--   0 root         (0) root         (0)    33000 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase.py
+-rw-r--r--   0 root         (0) root         (0)    31217 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_data.py
+-rw-r--r--   0 root         (0) root         (0)    33115 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py
+-rw-r--r--   0 root         (0) root         (0)    31204 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py
+-rw-r--r--   0 root         (0) root         (0)    31043 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group.py
+-rw-r--r--   0 root         (0) root         (0)    31316 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_data.py
+-rw-r--r--   0 root         (0) root         (0)    31076 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py
+-rw-r--r--   0 root         (0) root         (0)    36431 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_item.py
+-rw-r--r--   0 root         (0) root         (0)    38340 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_item.py
+-rw-r--r--   0 root         (0) root         (0)    39740 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py
+-rw-r--r--   0 root         (0) root         (0)    31114 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_slots.py
+-rw-r--r--   0 root         (0) root         (0)    61344 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_result.py
+-rw-r--r--   0 root         (0) root         (0)    46671 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_result_detail.py
+-rw-r--r--   0 root         (0) root         (0)    31129 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_session_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    38064 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_session_poll_response.py
+-rw-r--r--   0 root         (0) root         (0)    36359 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_websocket_payload.py
+-rw-r--r--   0 root         (0) root         (0)    31766 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/start_end_time_for_sub_criterion.py
+-rw-r--r--   0 root         (0) root         (0)    30452 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ping.py
+-rw-r--r--   0 root         (0) root         (0)    33072 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_word_correction.py
+-rw-r--r--   0 root         (0) root         (0)    31291 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_word_correction_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    37091 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word.py
+-rw-r--r--   0 root         (0) root         (0)    31229 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    35386 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base.py
+-rw-r--r--   0 root         (0) root         (0)    31248 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    33782 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base_without_spk.py
+-rw-r--r--   0 root         (0) root         (0)    35658 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stream_resp.py
+-rw-r--r--   0 root         (0) root         (0)    35728 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/stream_setup.py
+-rw-r--r--   0 root         (0) root         (0)    29711 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/streaming_protocol.py
+-rw-r--r--   0 root         (0) root         (0)    38851 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sub_criterion_config.py
+-rw-r--r--   0 root         (0) root         (0)    41237 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sub_criterion_satisfied.py
+-rw-r--r--   0 root         (0) root         (0)    32212 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_audio_input_source.py
+-rw-r--r--   0 root         (0) root         (0)    31160 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_recognition_request.py
+-rw-r--r--   0 root         (0) root         (0)    32725 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_recognition_response.py
+-rw-r--r--   0 root         (0) root         (0)    30328 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_session_established.py
+-rw-r--r--   0 root         (0) root         (0)    31044 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_request.py
+-rw-r--r--   0 root         (0) root         (0)    32783 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_response.py
+-rw-r--r--   0 root         (0) root         (0)    33222 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_result.py
+-rw-r--r--   0 root         (0) root         (0)    38938 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/talk_time.py
+-rw-r--r--   0 root         (0) root         (0)    32688 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/timed_sentence.py
+-rw-r--r--   0 root         (0) root         (0)    32843 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/timeline_speaker.py
+-rw-r--r--   0 root         (0) root         (0)    31469 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/topic_score.py
+-rw-r--r--   0 root         (0) root         (0)    29568 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_bucket_type.py
+-rw-r--r--   0 root         (0) root         (0)    39210 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc.py
+-rw-r--r--   0 root         (0) root         (0)    31128 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc_defaults.py
+-rw-r--r--   0 root         (0) root         (0)    36588 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc_statistics.py
+-rw-r--r--   0 root         (0) root         (0)    34662 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_key.py
+-rw-r--r--   0 root         (0) root         (0)    33912 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    29660 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_status.py
+-rw-r--r--   0 root         (0) root         (0)    29700 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_status_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    29588 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/training_set_store_type.py
+-rw-r--r--   0 root         (0) root         (0)    31830 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_alt.py
+-rw-r--r--   0 root         (0) root         (0)    49204 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request.py
+-rw-r--r--   0 root         (0) root         (0)    32616 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_audio.py
+-rw-r--r--   0 root         (0) root         (0)    33150 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_diarization.py
+-rw-r--r--   0 root         (0) root         (0)    34110 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_settings.py
+-rw-r--r--   0 root         (0) root         (0)    30705 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_source.py
+-rw-r--r--   0 root         (0) root         (0)    30351 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_response.py
+-rw-r--r--   0 root         (0) root         (0)    31112 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_id.py
+-rw-r--r--   0 root         (0) root         (0)    34130 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request.py
+-rw-r--r--   0 root         (0) root         (0)    31807 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request_mute.py
+-rw-r--r--   0 root         (0) root         (0)    30635 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request_pause.py
+-rw-r--r--   0 root         (0) root         (0)    34664 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range.py
+-rw-r--r--   0 root         (0) root         (0)    34844 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range_for_phrase.py
+-rw-r--r--   0 root         (0) root         (0)    36080 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py
+-rw-r--r--   0 root         (0) root         (0)    36401 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transfer.py
+-rw-r--r--   0 root         (0) root         (0)    36541 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/transfer_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    35969 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence.py
+-rw-r--r--   0 root         (0) root         (0)    33589 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_justification.py
+-rw-r--r--   0 root         (0) root         (0)    37229 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection.py
+-rw-r--r--   0 root         (0) root         (0)    30332 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    33869 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection_all_of_rejection.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/vad_mode.py
+-rw-r--r--   0 root         (0) root         (0)    32389 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/version.py
+-rw-r--r--   0 root         (0) root         (0)    38041 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket.py
+-rw-r--r--   0 root         (0) root         (0)    41095 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_init.py
+-rw-r--r--   0 root         (0) root         (0)    30602 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_init_reco.py
+-rw-r--r--   0 root         (0) root         (0)    36197 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_modifiable.py
+-rw-r--r--   0 root         (0) root         (0)    32665 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_msg.py
+-rw-r--r--   0 root         (0) root         (0)    29531 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_protocol.py
+-rw-r--r--   0 root         (0) root         (0)    31006 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/websocket_resp.py
+-rw-r--r--   0 root         (0) root         (0)    30363 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_alternatives.py
+-rw-r--r--   0 root         (0) root         (0)    31543 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_cloud_item.py
+-rw-r--r--   0 root         (0) root         (0)    31384 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_correction.py
+-rw-r--r--   0 root         (0) root         (0)    33618 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_item_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    30410 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_item_annotations.py
+-rw-r--r--   0 root         (0) root         (0)    36394 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_item_timed.py
+-rw-r--r--   0 root         (0) root         (0)    31469 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_item_timing.py
+-rw-r--r--   0 root         (0) root         (0)    30724 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_tree_ids.py
+-rw-r--r--   0 root         (0) root         (0)    36771 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/word_tree_item.py
+-rw-r--r--   0 root         (0) root         (0)    33326 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_item.py
+-rw-r--r--   0 root         (0) root         (0)    36629 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section.py
+-rw-r--r--   0 root         (0) root         (0)    33175 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta.py
+-rw-r--r--   0 root         (0) root         (0)    32177 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta_mc.py
+-rw-r--r--   0 root         (0) root         (0)    33423 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta_meeting.py
+-rw-r--r--   0 root         (0) root         (0)    34156 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section_single_column.py
+-rw-r--r--   0 root         (0) root         (0)    30237 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_section_words.py
+-rw-r--r--   0 root         (0) root         (0)    44270 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/words_websocket_item.py
+-rw-r--r--   0 root         (0) root         (0)    33913 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_emotion_item.py
+-rw-r--r--   0 root         (0) root         (0)    33162 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_keyword_item.py
+-rw-r--r--   0 root         (0) root         (0)    34152 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_named_entity_item.py
+-rw-r--r--   0 root         (0) root         (0)    32386 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_group_item.py
+-rw-r--r--   0 root         (0) root         (0)    35165 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_item.py
+-rw-r--r--   0 root         (0) root         (0)    35517 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py
+-rw-r--r--   0 root         (0) root         (0)    31738 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range.py
+-rw-r--r--   0 root         (0) root         (0)    30922 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range_nested.py
+-rw-r--r--   0 root         (0) root         (0)    30910 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range_no_spk.py
+-rw-r--r--   0 root         (0) root         (0)    37543 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py
+-rw-r--r--   0 root         (0) root         (0)    31387 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py
+-rw-r--r--   0 root         (0) root         (0)    32720 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_speaker.py
+-rw-r--r--   0 root         (0) root         (0)    34580 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_word.py
+-rw-r--r--   0 root         (0) root         (0)    32146 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/models/ws_word_edit.py
+-rw-r--r--   0 root         (0) root         (0)    39207 2024-02-21 22:21:35.000000 voicegain-speech-1.99.1/voicegain_speech/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-21 22:21:36.612859 voicegain-speech-1.99.1/voicegain_speech.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2936 2024-02-21 22:21:36.000000 voicegain-speech-1.99.1/voicegain_speech.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    26123 2024-02-21 22:21:36.000000 voicegain-speech-1.99.1/voicegain_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-21 22:21:36.000000 voicegain-speech-1.99.1/voicegain_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-02-21 22:21:36.000000 voicegain-speech-1.99.1/voicegain_speech.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-02-21 22:21:36.000000 voicegain-speech-1.99.1/voicegain_speech.egg-info/top_level.txt
```

### Comparing `voicegain-speech-1.99.0/LICENSE` & `voicegain-speech-1.99.1/LICENSE`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/PKG-INFO` & `voicegain-speech-1.99.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.99.0
+Version: 1.99.1
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.1.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.99.0/README.md` & `voicegain-speech-1.99.1/README.md`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/setup.py` & `voicegain-speech-1.99.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 REQUIRES = ["urllib3 >= 1.15", "six >= 1.10", "certifi", "python-dateutil"]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="voicegain-speech",
-    version="1.99.0",
+    version="1.99.1",
     author="Huishen Zhan, Kuo Zhang, Jacek Jarmulak",
     author_email="huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai",
     description="Voicegain Speech-to-Text Python SDK",
-    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.0.tar.gz',
+    download_url='https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.1.tar.gz',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=REQUIRES,
     packages=setuptools.find_packages(),
     include_package_data=True,
 )
```

### Comparing `voicegain-speech-1.99.0/voicegain_speech/__init__.py` & `voicegain-speech-1.99.1/voicegain_speech/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/__init__.py` & `voicegain-speech-1.99.1/voicegain_speech/api/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/aivr_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/aivr_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/aivr_callback_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/aivr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/asr_callback_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/asr_callback_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/audiocodes_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/audiocodes_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/data_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/data_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/greg_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/greg_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/meeting_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/meeting_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/recognize_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/recognize_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/sa_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/sa_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/security_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/security_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/training_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/training_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/transcribe_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/transcribe_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api/websocket_api.py` & `voicegain-speech-1.99.1/voicegain_speech/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/api_client.py` & `voicegain-speech-1.99.1/voicegain_speech/api_client.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/configuration.py` & `voicegain-speech-1.99.1/voicegain_speech/configuration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/exceptions.py` & `voicegain-speech-1.99.1/voicegain_speech/exceptions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/__init__.py` & `voicegain-speech-1.99.1/voicegain_speech/models/__init__.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_control_messages.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_control_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_end.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_end.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_error.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_hypothesis.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_hypothesis.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_hypothesis_alternatives.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_hypothesis_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_recognition_alternatives.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_response_messages.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_response_messages.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_start.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_start.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_start_stt_speech_contexts.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_start_stt_speech_contexts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_started.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ac_stop.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ac_stop.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/account_and_context_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/account_and_context_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/advanced_regex.py` & `voicegain-speech-1.99.1/voicegain_speech/models/advanced_regex.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aircall.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aircall.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aircall_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aircall_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_core_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_core_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_core_response_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_core_response_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_callback_response_final.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_callback_response_final.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_conference_transfer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_conference_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_disconnect.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_event.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_event_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_event_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_existing_session.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_existing_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_media.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_media.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_transfer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_logic_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_logic_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_new_session.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_new_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_phone_transfer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_phone_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_completion.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_completion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_playing.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_playing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_properties_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_prompt_properties_html.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_prompt_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_question.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_recognition_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_recording.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_recording.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_response_properties_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_response_properties_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_response_properties_html.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_response_properties_html.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_session_user_fs.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_session_user_fs.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_transfer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivr_vars.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivr_vars.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/aivrs_question_specifics.py` & `voicegain-speech-1.99.1/voicegain_speech/models/aivrs_question_specifics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/answer_map_entry.py` & `voicegain-speech-1.99.1/voicegain_speech/models/answer_map_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_event.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_additional.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_additional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_after_input_started.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_after_input_started.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_processing_status_for_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_processing_status_for_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_recognition_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_common.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_meeting_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_meeting_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_defaults.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_grammars_etc.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_grammars_etc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_recognition_timeouts.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_recognition_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_async.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_async_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_async_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_common.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_common.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_common_lm.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_common_lm.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_default_timeouts.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_default_timeouts.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_defaults.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_sa.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_sa.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_speakers.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_settings_transcription_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/asr_transcribe_queue_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/asr_transcribe_queue_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_audio_input_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_mode.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_mode_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_mode_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_mode_speech_analytics.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_mode_speech_analytics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_mode_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_mode_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_post_response_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_post_response_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_post_response_base_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_post_response_base_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_reco_post_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_reco_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_reco_post_response_sessions.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_reco_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_callback_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_recognition_result_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_recognition_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_audio_source_data_store.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_full_all_of_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_full_all_of_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_control_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_control_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_result_incremental_detail_result_incremental_transcript.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_session_established.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_session_short_info.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_session_short_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_session_url.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_session_url.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transc_post_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transc_post_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transc_post_response_sessions.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transc_post_response_sessions.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transc_session_established.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transc_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_callback_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_callback_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/async_transcription_response_shared.py` & `voicegain-speech-1.99.1/voicegain_speech/models/async_transcription_response_shared.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_channel.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_channel_selector.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_channel_selector.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_channel_selector_offline_async.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_channel_selector_offline_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_channels.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_channels.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_for_data_object.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_for_data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_format.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_format.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_async_with_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_async_with_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_callback_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_callback_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_data_all_of_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_data_all_of_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_sync.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_sync.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_input_sync_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_input_sync_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_resource_uri.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_zone_class.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_zone_class.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/audio_zone_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/audio_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/base_sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/base_sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/base_sentence_hypothesis_or_recognition_alternatives.py` & `voicegain-speech-1.99.1/voicegain_speech/models/base_sentence_hypothesis_or_recognition_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/base_stomp_word_correction.py` & `voicegain-speech-1.99.1/voicegain_speech/models/base_stomp_word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/basic_success_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/basic_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/builtin.py` & `voicegain-speech-1.99.1/voicegain_speech/models/builtin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/builtin_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/builtin_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_attributes.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_attributes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_review_answer_alone.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_review_answer_alone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_review_answer_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_review_answer_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base_with_answer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base_with_answer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/call_review_config_question_base_with_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/call_review_config_question_base_with_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/callback_req.py` & `voicegain-speech-1.99.1/voicegain_speech/models/callback_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/callback_req_reco.py` & `voicegain-speech-1.99.1/voicegain_speech/models/callback_req_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/callback_resp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/callback_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/caption.py` & `voicegain-speech-1.99.1/voicegain_speech/models/caption.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/compliance_settings.py` & `voicegain-speech-1.99.1/voicegain_speech/models/compliance_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/config_value_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/config_value_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/content_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/content_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/continuous_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/continuous_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/core_aivr_session.py` & `voicegain-speech-1.99.1/voicegain_speech/models/core_aivr_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/core_aivr_session_telco_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/core_aivr_session_telco_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/cr_question_id_for_cr_config.py` & `voicegain-speech-1.99.1/voicegain_speech/models/cr_question_id_for_cr_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/creating_entity.py` & `voicegain-speech-1.99.1/voicegain_speech/models/creating_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/criterion_config.py` & `voicegain-speech-1.99.1/voicegain_speech/models/criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/criterion_satisfied.py` & `voicegain-speech-1.99.1/voicegain_speech/models/criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_obj_ref.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_obj_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_ids.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref_presigned_s3.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref_presigned_s3.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_no_sos_ref_presigned_s3_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_no_sos_ref_presigned_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/data_object_with_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/data_object_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/debug_info.py` & `voicegain-speech-1.99.1/voicegain_speech/models/debug_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/debug_settings.py` & `voicegain-speech-1.99.1/voicegain_speech/models/debug_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/demo.py` & `voicegain-speech-1.99.1/voicegain_speech/models/demo.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/demo_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/demo_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/diarization_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/diarization_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/diarization_zone.py` & `voicegain-speech-1.99.1/voicegain_speech/models/diarization_zone.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/diarization_zone_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/diarization_zone_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/disconnect.py` & `voicegain-speech-1.99.1/voicegain_speech/models/disconnect.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/disconnect_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/disconnect_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/error.py` & `voicegain-speech-1.99.1/voicegain_speech/models/error.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/error_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/error_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/error_info.py` & `voicegain-speech-1.99.1/voicegain_speech/models/error_info.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/estimated_queue_wait.py` & `voicegain-speech-1.99.1/voicegain_speech/models/estimated_queue_wait.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/experiment_platform.py` & `voicegain-speech-1.99.1/voicegain_speech/models/experiment_platform.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/extended_summary_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/extended_summary_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/file_location.py` & `voicegain-speech-1.99.1/voicegain_speech/models/file_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/formatter.py` & `voicegain-speech-1.99.1/voicegain_speech/models/formatter.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/grammar.py` & `voicegain-speech-1.99.1/voicegain_speech/models/grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_base_with_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_base_with_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_audio_hash.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_audio_hash.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_audio_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_audio_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_input_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_input_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_base_inclusive.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_core.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inclusive.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inclusive_core.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inclusive_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_inner.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_set_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_set_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_audio_thin.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_audio_thin.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base_inclusive.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_base_platform_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_base_platform_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_inclusive.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_inclusive.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_external_asr.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_external_asr.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_upload.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_upload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_platform_voicegain.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_platform_voicegain.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_experiment_status_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_experiment_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_base_light.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_base_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_inner.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_grammar_light.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_grammar_light.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_interpretation.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_interpretation.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_question.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_question.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_question_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_question_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_question_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_question_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_question_inner.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_question_inner.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_nlsml_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_obj_core.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_no_exp_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_obj_or_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recog_base_with_exp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recog_base_with_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_recognition_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_recognition_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_review_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_review_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_source_of_truth.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_source_of_truth.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_truth_update.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_truth_update.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/greg_truth_updates.py` & `voicegain-speech-1.99.1/voicegain_speech/models/greg_truth_updates.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/grxml.py` & `voicegain-speech-1.99.1/voicegain_speech/models/grxml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/grxml_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/grxml_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/gui_input.py` & `voicegain-speech-1.99.1/voicegain_speech/models/gui_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/hangup.py` & `voicegain-speech-1.99.1/voicegain_speech/models/hangup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/html_checkbox.py` & `voicegain-speech-1.99.1/voicegain_speech/models/html_checkbox.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/html_choice_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/html_choice_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/html_radio_buttons.py` & `voicegain-speech-1.99.1/voicegain_speech/models/html_radio_buttons.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/html_text_entry.py` & `voicegain-speech-1.99.1/voicegain_speech/models/html_text_entry.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/if_exists.py` & `voicegain-speech-1.99.1/voicegain_speech/models/if_exists.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/incident.py` & `voicegain-speech-1.99.1/voicegain_speech/models/incident.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/inline_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/inline_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/inline_object.py` & `voicegain-speech-1.99.1/voicegain_speech/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/inline_object1.py` & `voicegain-speech-1.99.1/voicegain_speech/models/inline_object1.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/input.py` & `voicegain-speech-1.99.1/voicegain_speech/models/input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/input_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/input_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/integration.py` & `voicegain-speech-1.99.1/voicegain_speech/models/integration.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/jjsgf.py` & `voicegain-speech-1.99.1/voicegain_speech/models/jjsgf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/jjsgf_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/jjsgf_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/joined_meeting_event.py` & `voicegain-speech-1.99.1/voicegain_speech/models/joined_meeting_event.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_example.py` & `voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_group.py` & `voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/keyword_spot_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/keyword_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/language.py` & `voicegain-speech-1.99.1/voicegain_speech/models/language.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_add_audio_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_add_audio_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_data_audio_channels.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_data_audio_channels.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_data_chat.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_data_chat.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_field.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_field.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_join_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_join_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_keyword_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_keyword_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_minutes.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_minutes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_minutes_section.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_minutes_section.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_phrase_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_phrase_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_search_field.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_search_field.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_speaker_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_speaker_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_poll_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_poll_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_poll_result_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_poll_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_result_reference.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_result_reference.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_search_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_search_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_transcribe_search_result_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_transcribe_search_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_word_item_timed_with_annot.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_word_item_timed_with_annot.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_section_with_annot.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_section_with_annot.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/meeting_words_section_words_with_annot.py` & `voicegain-speech-1.99.1/voicegain_speech/models/meeting_words_section_words_with_annot.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/min_max_speakers.py` & `voicegain-speech-1.99.1/voicegain_speech/models/min_max_speakers.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/min_max_speakers_diarization.py` & `voicegain-speech-1.99.1/voicegain_speech/models/min_max_speakers_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/modifiable_meeting_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/modifiable_meeting_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/modifiable_meeting_data_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/modifiable_meeting_data_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/mood_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/mood_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/mrc_pv1_asr_settings.py` & `voicegain-speech-1.99.1/voicegain_speech/models/mrc_pv1_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/mrc_pv2_asr_settings.py` & `voicegain-speech-1.99.1/voicegain_speech/models/mrc_pv2_asr_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/mrcp_version.py` & `voicegain-speech-1.99.1/voicegain_speech/models/mrcp_version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/multipart_form_data_field.py` & `voicegain-speech-1.99.1/voicegain_speech/models/multipart_form_data_field.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/name_value_pair.py` & `voicegain-speech-1.99.1/voicegain_speech/models/name_value_pair.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/named_entity_concept.py` & `voicegain-speech-1.99.1/voicegain_speech/models/named_entity_concept.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/named_entity_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/named_entity_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/named_speaker.py` & `voicegain-speech-1.99.1/voicegain_speech/models/named_speaker.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session.py` & `voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response_poll.py` & `voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response_poll.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/new_speech_analytics_session_response_websocket.py` & `voicegain-speech-1.99.1/voicegain_speech/models/new_speech_analytics_session_response_websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response400.py` & `voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response400.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/non_session_error_response401.py` & `voicegain-speech-1.99.1/voicegain_speech/models/non_session_error_response401.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/non_speaking_participant.py` & `voicegain-speech-1.99.1/voicegain_speech/models/non_speaking_participant.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/offline_progress.py` & `voicegain-speech-1.99.1/voicegain_speech/models/offline_progress.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/output.py` & `voicegain-speech-1.99.1/voicegain_speech/models/output.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/output_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/output_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/overtalk.py` & `voicegain-speech-1.99.1/voicegain_speech/models/overtalk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/performed_redaction.py` & `voicegain-speech-1.99.1/voicegain_speech/models/performed_redaction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phone_audio_input.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phone_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phone_audio_input_prompt.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phone_audio_input_prompt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_example.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_example.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_group.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_location.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_location.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_location_dialogue.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_location_dialogue.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/phrase_spot_item_slots.py` & `voicegain-speech-1.99.1/voicegain_speech/models/phrase_spot_item_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/pii_redaction_conf.py` & `voicegain-speech-1.99.1/voicegain_speech/models/pii_redaction_conf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/poll_req.py` & `voicegain-speech-1.99.1/voicegain_speech/models/poll_req.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/poll_resp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/poll_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/portal_output_init.py` & `voicegain-speech-1.99.1/voicegain_speech/models/portal_output_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/pre_fetch.py` & `voicegain-speech-1.99.1/voicegain_speech/models/pre_fetch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/presigned_data_file_url_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/presigned_data_file_url_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/progress.py` & `voicegain-speech-1.99.1/voicegain_speech/models/progress.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/progress_callback.py` & `voicegain-speech-1.99.1/voicegain_speech/models/progress_callback.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/progress_phase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/progress_phase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/quartiles_energy.py` & `voicegain-speech-1.99.1/voicegain_speech/models/quartiles_energy.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/quartiles_pitch.py` & `voicegain-speech-1.99.1/voicegain_speech/models/quartiles_pitch.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/query.py` & `voicegain-speech-1.99.1/voicegain_speech/models/query.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/reco_alt.py` & `voicegain-speech-1.99.1/voicegain_speech/models/reco_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/recog_nlsml.py` & `voicegain-speech-1.99.1/voicegain_speech/models/recog_nlsml.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/recog_nlsml_no_exp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/recog_nlsml_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/recog_obj.py` & `voicegain-speech-1.99.1/voicegain_speech/models/recog_obj.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/recog_obj_no_exp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/recog_obj_no_exp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/recognition_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/recognition_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/requested_content.py` & `voicegain-speech-1.99.1/voicegain_speech/models/requested_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/resource_uri.py` & `voicegain-speech-1.99.1/voicegain_speech/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/resource_uri_local_auth_conf.py` & `voicegain-speech-1.99.1/voicegain_speech/models/resource_uri_local_auth_conf.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/results_websocket_mode.py` & `voicegain-speech-1.99.1/voicegain_speech/models/results_websocket_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/s3.py` & `voicegain-speech-1.99.1/voicegain_speech/models/s3.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/s3_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/s3_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/s3_audio_input.py` & `voicegain-speech-1.99.1/voicegain_speech/models/s3_audio_input.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/s3_metadata_mapping.py` & `voicegain-speech-1.99.1/voicegain_speech/models/s3_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/s3_tag_mapping.py` & `voicegain-speech-1.99.1/voicegain_speech/models/s3_tag_mapping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sa_conf_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sa_conf_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sample_rate.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sample_rate.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sentence_hypothesis_or_recognition_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sentence_hypothesis_or_recognition_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sentence_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sentence_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_content.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_content.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_error_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_error_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_init_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_init_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_init_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_init_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_init_transcription_diarization.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_init_transcription_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/session_success_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/session_success_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/settings_async_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/settings_async_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/settings_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/settings_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/settings_sync_transcription.py` & `voicegain-speech-1.99.1/voicegain_speech/models/settings_sync_transcription.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/silence.py` & `voicegain-speech-1.99.1/voicegain_speech/models/silence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/slot_entity.py` & `voicegain-speech-1.99.1/voicegain_speech/models/slot_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/slot_keyword.py` & `voicegain-speech-1.99.1/voicegain_speech/models/slot_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sos_ref.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sos_ref.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speaker_activity.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speaker_activity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speaker_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speaker_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speaker_with_percent_spoken.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speaker_with_percent_spoken.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_base_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_base_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_channel_with_transcribe.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_channel_with_transcribe.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_identifying.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_identifying.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_modifiable_base_meeting_minutes.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_name_optional.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_name_optional.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_config_name_required.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_config_name_required.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_core_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_core_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_core_result_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_core_result_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_criteria_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_criteria_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_emotion_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_keyword_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_named_entity_item_for_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_for_ws.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_for_ws_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_data.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_data.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_for_ws.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_group_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_itemfor_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_phrase_slots.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_phrase_slots.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_result_detail.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_result_detail.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_session_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_session_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_session_poll_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_session_poll_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/speech_analytics_websocket_payload.py` & `voicegain-speech-1.99.1/voicegain_speech/models/speech_analytics_websocket_payload.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/start_end_time_for_sub_criterion.py` & `voicegain-speech-1.99.1/voicegain_speech/models/start_end_time_for_sub_criterion.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ping.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ping.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_word_correction.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_word_correction_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_word_correction_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stomp_ws_word_base_without_spk.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stomp_ws_word_base_without_spk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stream_resp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stream_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/stream_setup.py` & `voicegain-speech-1.99.1/voicegain_speech/models/stream_setup.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/streaming_protocol.py` & `voicegain-speech-1.99.1/voicegain_speech/models/streaming_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sub_criterion_config.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sub_criterion_config.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sub_criterion_satisfied.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sub_criterion_satisfied.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_audio_input_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_audio_input_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_recognition_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_recognition_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_recognition_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_recognition_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_session_established.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_session_established.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/sync_transcription_result.py` & `voicegain-speech-1.99.1/voicegain_speech/models/sync_transcription_result.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/talk_time.py` & `voicegain-speech-1.99.1/voicegain_speech/models/talk_time.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/timed_sentence.py` & `voicegain-speech-1.99.1/voicegain_speech/models/timed_sentence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/timeline_speaker.py` & `voicegain-speech-1.99.1/voicegain_speech/models/timeline_speaker.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/topic_score.py` & `voicegain-speech-1.99.1/voicegain_speech/models/topic_score.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_bucket_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_bucket_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc_defaults.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc_defaults.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_doc_statistics.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_doc_statistics.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_key.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_key.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_status.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_status.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_status_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_status_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/training_set_store_type.py` & `voicegain-speech-1.99.1/voicegain_speech/models/training_set_store_type.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_alt.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_alt.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_audio.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_audio.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_diarization.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_diarization.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_settings.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_settings.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_request_source.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_request_source.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_meeting_response.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_meeting_response.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_id.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_id.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request_mute.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request_mute.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcribe_session_modify_request_pause.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcribe_session_modify_request_pause.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range_for_phrase.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range_for_phrase.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transcript_position_range_for_phrase_with_chn.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transfer.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transfer.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/transfer_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/transfer_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence.py` & `voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_justification.py` & `voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_justification.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection.py` & `voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/typed_sentence_with_rejection_all_of_rejection.py` & `voicegain-speech-1.99.1/voicegain_speech/models/typed_sentence_with_rejection_all_of_rejection.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/vad_mode.py` & `voicegain-speech-1.99.1/voicegain_speech/models/vad_mode.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/version.py` & `voicegain-speech-1.99.1/voicegain_speech/models/version.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_init.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_init.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_init_reco.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_init_reco.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_modifiable.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_modifiable.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_msg.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_msg.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_protocol.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_protocol.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/websocket_resp.py` & `voicegain-speech-1.99.1/voicegain_speech/models/websocket_resp.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_alternatives.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_alternatives.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_cloud_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_cloud_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_correction.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_correction.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_item_annotation.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_item_annotation.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_item_annotations.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_item_annotations.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_item_timed.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_item_timed.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_item_timing.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_item_timing.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_tree_ids.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_tree_ids.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/word_tree_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/word_tree_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta_mc.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta_mc.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section_meta_meeting.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section_meta_meeting.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section_single_column.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section_single_column.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_section_words.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_section_words.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/words_websocket_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/words_websocket_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_emotion_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_emotion_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_keyword_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_keyword_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_named_entity_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_named_entity_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_group_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_group_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_item.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_item.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_phrase_item_inside_group.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_phrase_item_inside_group.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range_nested.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range_nested.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sa_position_range_no_spk.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sa_position_range_no_spk.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_sentence_hypothesis_or_recognition_all_of.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_speaker.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_speaker.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_word.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_word.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/models/ws_word_edit.py` & `voicegain-speech-1.99.1/voicegain_speech/models/ws_word_edit.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech/rest.py` & `voicegain-speech-1.99.1/voicegain_speech/rest.py`

 * *Files identical despite different names*

### Comparing `voicegain-speech-1.99.0/voicegain_speech.egg-info/PKG-INFO` & `voicegain-speech-1.99.1/voicegain_speech.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: voicegain-speech
-Version: 1.99.0
+Version: 1.99.1
 Summary: Voicegain Speech-to-Text Python SDK
 Home-page: UNKNOWN
 Author: Huishen Zhan, Kuo Zhang, Jacek Jarmulak
 Author-email: huishen@voicegain.ai, kuo@voicegain.ai, jacek@voicegain.ai
 License: UNKNOWN
-Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.0.tar.gz
+Download-URL: https://github.com/voicegain/python-sdk/archive/refs/tags/1.99.1.tar.gz
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Voicegain Speech-to-Text Python SDK
 
 Python SDK for the [Voicegain](https://www.voicegain.ai) [Speech-to-Text API](https://portal.voicegain.ai/api/v1/index.html).
```

### Comparing `voicegain-speech-1.99.0/voicegain_speech.egg-info/SOURCES.txt` & `voicegain-speech-1.99.1/voicegain_speech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

