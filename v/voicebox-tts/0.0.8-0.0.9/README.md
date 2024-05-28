# Comparing `tmp/voicebox_tts-0.0.8.tar.gz` & `tmp/voicebox_tts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox_tts-0.0.8.tar", last modified: Mon May 27 08:12:19 2024, max compression
+gzip compressed data, was "voicebox_tts-0.0.9.tar", last modified: Tue May 28 07:02:33 2024, max compression
```

## Comparing `voicebox_tts-0.0.8.tar` & `voicebox_tts-0.0.9.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.233105 voicebox_tts-0.0.8/
--rw-rw-r--   0 austin    (1000) austin    (1000)     1069 2023-10-09 03:54:09.000000 voicebox_tts-0.0.8/LICENSE
--rw-r--r--   0 austin    (1000) austin    (1000)    10058 2024-05-27 08:12:19.233105 voicebox_tts-0.0.8/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)     6443 2024-05-27 08:02:39.000000 voicebox_tts-0.0.8/README.md
--rw-rw-r--   0 austin    (1000) austin    (1000)     2112 2023-12-28 18:57:19.000000 voicebox_tts-0.0.8/pyproject.toml
--rw-rw-r--   0 austin    (1000) austin    (1000)       38 2024-05-27 08:12:19.234105 voicebox_tts-0.0.8/setup.cfg
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.226105 voicebox_tts-0.0.8/src/
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.227105 voicebox_tts-0.0.8/src/voicebox/
--rw-rw-r--   0 austin    (1000) austin    (1000)      132 2023-12-28 18:53:19.000000 voicebox_tts-0.0.8/src/voicebox/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4485 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/__main__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2198 2023-12-22 05:30:01.000000 voicebox_tts-0.0.8/src/voicebox/audio.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.228105 voicebox_tts-0.0.8/src/voicebox/effects/
--rw-rw-r--   0 austin    (1000) austin    (1000)      608 2023-12-19 03:44:53.000000 voicebox_tts-0.0.8/src/voicebox/effects/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2299 2023-12-19 04:54:52.000000 voicebox_tts-0.0.8/src/voicebox/effects/chain.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      278 2023-12-19 04:21:09.000000 voicebox_tts-0.0.8/src/voicebox/effects/dc_offset.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1141 2023-12-19 05:32:27.000000 voicebox_tts-0.0.8/src/voicebox/effects/delay.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      519 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/effects/effect.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     4185 2023-12-19 04:34:14.000000 voicebox_tts-0.0.8/src/voicebox/effects/eq.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2685 2023-12-22 05:27:07.000000 voicebox_tts-0.0.8/src/voicebox/effects/flanger.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1388 2023-12-19 04:45:50.000000 voicebox_tts-0.0.8/src/voicebox/effects/glitch.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1256 2023-12-19 04:51:38.000000 voicebox_tts-0.0.8/src/voicebox/effects/modulation.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      765 2023-12-19 04:53:06.000000 voicebox_tts-0.0.8/src/voicebox/effects/normalize.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1375 2023-12-19 04:54:52.000000 voicebox_tts-0.0.8/src/voicebox/effects/pedalboard.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      694 2023-12-19 03:11:41.000000 voicebox_tts-0.0.8/src/voicebox/effects/tail.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      188 2023-12-19 04:56:09.000000 voicebox_tts-0.0.8/src/voicebox/effects/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     6717 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/effects/vocoder.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.229105 voicebox_tts-0.0.8/src/voicebox/examples/
--rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-10-17 01:14:20.000000 voicebox_tts-0.0.8/src/voicebox/examples/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1647 2023-12-28 18:47:35.000000 voicebox_tts-0.0.8/src/voicebox/examples/battle_droid.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1293 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/examples/demo.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2208 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/examples/glados.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1384 2023-12-28 18:47:35.000000 voicebox_tts-0.0.8/src/voicebox/examples/halo_spark.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.229105 voicebox_tts-0.0.8/src/voicebox/sinks/
--rw-rw-r--   0 austin    (1000) austin    (1000)      315 2023-12-22 05:11:06.000000 voicebox_tts-0.0.8/src/voicebox/sinks/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-20 01:46:44.000000 voicebox_tts-0.0.8/src/voicebox/sinks/distributor.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/sinks/sink.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1525 2023-12-20 02:01:04.000000 voicebox_tts-0.0.8/src/voicebox/sinks/sounddevice.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2614 2023-12-20 02:01:31.000000 voicebox_tts-0.0.8/src/voicebox/sinks/wavefile.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1066 2023-12-22 07:29:42.000000 voicebox_tts-0.0.8/src/voicebox/ssml.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.230105 voicebox_tts-0.0.8/src/voicebox/tts/
--rw-rw-r--   0 austin    (1000) austin    (1000)      678 2024-05-27 07:25:12.000000 voicebox_tts-0.0.8/src/voicebox/tts/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2463 2023-12-25 04:09:47.000000 voicebox_tts-0.0.8/src/voicebox/tts/amazonpolly.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     5698 2023-12-20 02:21:26.000000 voicebox_tts-0.0.8/src/voicebox/tts/cache.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2239 2024-05-27 08:07:41.000000 voicebox_tts-0.0.8/src/voicebox/tts/elevenlabs.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3024 2023-12-22 05:46:10.000000 voicebox_tts-0.0.8/src/voicebox/tts/espeakng.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1691 2023-12-22 05:48:06.000000 voicebox_tts-0.0.8/src/voicebox/tts/googlecloudtts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1183 2023-12-25 05:18:45.000000 voicebox_tts-0.0.8/src/voicebox/tts/gtts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1767 2023-12-22 05:59:17.000000 voicebox_tts-0.0.8/src/voicebox/tts/picotts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3513 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/tts/tts.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     2605 2024-05-27 08:06:38.000000 voicebox_tts-0.0.8/src/voicebox/tts/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      194 2023-11-18 03:18:52.000000 voicebox_tts-0.0.8/src/voicebox/types.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1383 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/utils.py
--rw-rw-r--   0 austin    (1000) austin    (1000)       22 2024-05-27 08:10:52.000000 voicebox_tts-0.0.8/src/voicebox/version.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.230105 voicebox_tts-0.0.8/src/voicebox/voiceboxes/
--rw-rw-r--   0 austin    (1000) austin    (1000)      123 2023-12-28 18:37:25.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/__init__.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1684 2023-12-28 18:39:11.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/base.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     8219 2024-05-27 07:17:41.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/parallel.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1587 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/queue.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     1823 2023-12-28 18:39:11.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/simple.py
--rw-rw-r--   0 austin    (1000) austin    (1000)     3673 2023-12-28 18:32:50.000000 voicebox_tts-0.0.8/src/voicebox/voiceboxes/splitter.py
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.231105 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/
--rw-r--r--   0 austin    (1000) austin    (1000)    10058 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/PKG-INFO
--rw-rw-r--   0 austin    (1000) austin    (1000)     1693 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        1 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)      466 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/requires.txt
--rw-rw-r--   0 austin    (1000) austin    (1000)        9 2024-05-27 08:12:19.000000 voicebox_tts-0.0.8/src/voicebox_tts.egg-info/top_level.txt
-drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-27 08:12:19.231105 voicebox_tts-0.0.8/tests/
--rw-rw-r--   0 austin    (1000) austin    (1000)     2931 2023-12-22 05:27:48.000000 voicebox_tts-0.0.8/tests/test_audio.py
--rw-rw-r--   0 austin    (1000) austin    (1000)      646 2023-11-12 19:59:26.000000 voicebox_tts-0.0.8/tests/test_ssml.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.628517 voicebox_tts-0.0.9/
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1069 2023-10-09 03:54:09.000000 voicebox_tts-0.0.9/LICENSE
+-rw-r--r--   0 austin    (1000) austin    (1000)    10624 2024-05-28 07:02:33.628517 voicebox_tts-0.0.9/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)     6889 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/README.md
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2170 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/pyproject.toml
+-rw-rw-r--   0 austin    (1000) austin    (1000)       38 2024-05-28 07:02:33.628517 voicebox_tts-0.0.9/setup.cfg
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.624517 voicebox_tts-0.0.9/src/
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.624517 voicebox_tts-0.0.9/src/voicebox/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      132 2023-12-28 18:53:19.000000 voicebox_tts-0.0.9/src/voicebox/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     4410 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/src/voicebox/__main__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2198 2023-12-22 05:30:01.000000 voicebox_tts-0.0.9/src/voicebox/audio.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.625517 voicebox_tts-0.0.9/src/voicebox/effects/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      608 2023-12-19 03:44:53.000000 voicebox_tts-0.0.9/src/voicebox/effects/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2299 2023-12-19 04:54:52.000000 voicebox_tts-0.0.9/src/voicebox/effects/chain.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      278 2023-12-19 04:21:09.000000 voicebox_tts-0.0.9/src/voicebox/effects/dc_offset.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1141 2023-12-19 05:32:27.000000 voicebox_tts-0.0.9/src/voicebox/effects/delay.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      519 2023-12-28 18:32:50.000000 voicebox_tts-0.0.9/src/voicebox/effects/effect.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     4185 2023-12-19 04:34:14.000000 voicebox_tts-0.0.9/src/voicebox/effects/eq.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2685 2023-12-22 05:27:07.000000 voicebox_tts-0.0.9/src/voicebox/effects/flanger.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1388 2023-12-19 04:45:50.000000 voicebox_tts-0.0.9/src/voicebox/effects/glitch.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1256 2023-12-19 04:51:38.000000 voicebox_tts-0.0.9/src/voicebox/effects/modulation.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      765 2023-12-19 04:53:06.000000 voicebox_tts-0.0.9/src/voicebox/effects/normalize.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1375 2023-12-19 04:54:52.000000 voicebox_tts-0.0.9/src/voicebox/effects/pedalboard.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      694 2023-12-19 03:11:41.000000 voicebox_tts-0.0.9/src/voicebox/effects/tail.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      188 2023-12-19 04:56:09.000000 voicebox_tts-0.0.9/src/voicebox/effects/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     6717 2024-05-27 21:22:13.000000 voicebox_tts-0.0.9/src/voicebox/effects/vocoder.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.625517 voicebox_tts-0.0.9/src/voicebox/examples/
+-rw-rw-r--   0 austin    (1000) austin    (1000)        0 2023-10-17 01:14:20.000000 voicebox_tts-0.0.9/src/voicebox/examples/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1647 2023-12-28 18:47:35.000000 voicebox_tts-0.0.9/src/voicebox/examples/battle_droid.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1293 2024-05-27 21:22:13.000000 voicebox_tts-0.0.9/src/voicebox/examples/demo.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2208 2024-05-27 21:22:13.000000 voicebox_tts-0.0.9/src/voicebox/examples/glados.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1384 2023-12-28 18:47:35.000000 voicebox_tts-0.0.9/src/voicebox/examples/halo_spark.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.625517 voicebox_tts-0.0.9/src/voicebox/sinks/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      315 2023-12-22 05:11:06.000000 voicebox_tts-0.0.9/src/voicebox/sinks/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-20 01:46:44.000000 voicebox_tts-0.0.9/src/voicebox/sinks/distributor.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      301 2023-12-28 18:32:50.000000 voicebox_tts-0.0.9/src/voicebox/sinks/sink.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1525 2023-12-20 02:01:04.000000 voicebox_tts-0.0.9/src/voicebox/sinks/sounddevice.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2614 2023-12-20 02:01:31.000000 voicebox_tts-0.0.9/src/voicebox/sinks/wavefile.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1066 2023-12-22 07:29:42.000000 voicebox_tts-0.0.9/src/voicebox/ssml.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.626516 voicebox_tts-0.0.9/src/voicebox/tts/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      761 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/src/voicebox/tts/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2463 2023-12-25 04:09:47.000000 voicebox_tts-0.0.9/src/voicebox/tts/amazonpolly.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     5698 2023-12-20 02:21:26.000000 voicebox_tts-0.0.9/src/voicebox/tts/cache.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2239 2024-05-27 08:24:37.000000 voicebox_tts-0.0.9/src/voicebox/tts/elevenlabs.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     3024 2023-12-22 05:46:10.000000 voicebox_tts-0.0.9/src/voicebox/tts/espeakng.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1691 2023-12-22 05:48:06.000000 voicebox_tts-0.0.9/src/voicebox/tts/googlecloudtts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1183 2023-12-25 05:18:45.000000 voicebox_tts-0.0.9/src/voicebox/tts/gtts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1551 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/src/voicebox/tts/picotts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1264 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/src/voicebox/tts/pyttsx3.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     5521 2024-05-28 07:01:34.000000 voicebox_tts-0.0.9/src/voicebox/tts/tts.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2605 2024-05-27 08:24:37.000000 voicebox_tts-0.0.9/src/voicebox/tts/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      194 2023-11-18 03:18:52.000000 voicebox_tts-0.0.9/src/voicebox/types.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1383 2023-12-28 18:32:50.000000 voicebox_tts-0.0.9/src/voicebox/utils.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)       22 2024-05-28 07:01:19.000000 voicebox_tts-0.0.9/src/voicebox/version.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.626516 voicebox_tts-0.0.9/src/voicebox/voiceboxes/
+-rw-rw-r--   0 austin    (1000) austin    (1000)      123 2023-12-28 18:37:25.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/__init__.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1684 2023-12-28 18:39:11.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/base.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     8219 2024-05-27 21:22:13.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/parallel.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1587 2023-12-28 18:32:50.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/queue.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1823 2023-12-28 18:39:11.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/simple.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)     3673 2023-12-28 18:32:50.000000 voicebox_tts-0.0.9/src/voicebox/voiceboxes/splitter.py
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.627517 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/
+-rw-r--r--   0 austin    (1000) austin    (1000)    10624 2024-05-28 07:02:33.000000 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 austin    (1000) austin    (1000)     1721 2024-05-28 07:02:33.000000 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        1 2024-05-28 07:02:33.000000 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)      507 2024-05-28 07:02:33.000000 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/requires.txt
+-rw-rw-r--   0 austin    (1000) austin    (1000)        9 2024-05-28 07:02:33.000000 voicebox_tts-0.0.9/src/voicebox_tts.egg-info/top_level.txt
+drwxrwxr-x   0 austin    (1000) austin    (1000)        0 2024-05-28 07:02:33.626516 voicebox_tts-0.0.9/tests/
+-rw-rw-r--   0 austin    (1000) austin    (1000)     2931 2023-12-22 05:27:48.000000 voicebox_tts-0.0.9/tests/test_audio.py
+-rw-rw-r--   0 austin    (1000) austin    (1000)      646 2023-11-12 19:59:26.000000 voicebox_tts-0.0.9/tests/test_ssml.py
```

### Comparing `voicebox_tts-0.0.8/LICENSE` & `voicebox_tts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/PKG-INFO` & `voicebox_tts-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-tts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 Author-email: Austin Bowen <austin.bowen.314@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Austin Bowen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,14 +50,15 @@
 Requires-Dist: voicebox-tts[dev]; extra == "all"
 Requires-Dist: voicebox-tts[docs]; extra == "all"
 Requires-Dist: voicebox-tts[test]; extra == "all"
 Requires-Dist: voicebox-tts[amazon-polly]; extra == "all"
 Requires-Dist: voicebox-tts[elevenlabs]; extra == "all"
 Requires-Dist: voicebox-tts[google-cloud-tts]; extra == "all"
 Requires-Dist: voicebox-tts[gtts]; extra == "all"
+Requires-Dist: voicebox-tts[pyttsx3]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
@@ -73,14 +74,16 @@
 Requires-Dist: elevenlabs; extra == "elevenlabs"
 Requires-Dist: pydub; extra == "elevenlabs"
 Provides-Extra: google-cloud-tts
 Requires-Dist: google-cloud-texttospeech; extra == "google-cloud-tts"
 Provides-Extra: gtts
 Requires-Dist: gTTS; extra == "gtts"
 Requires-Dist: pydub; extra == "gtts"
+Provides-Extra: pyttsx3
+Requires-Dist: pyttsx3; extra == "pyttsx3"
 
 # voicebox
 
 ![python-package](https://github.com/austin-bowen/voicebox/actions/workflows/python-package.yml/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/voicebox-tts)
 [![PyPI - Version](https://img.shields.io/pypi/v/voicebox-tts)](https://pypi.org/project/voicebox-tts/)
 [![Documentation Status](https://readthedocs.org/projects/voicebox/badge/?version=latest)](https://voicebox.readthedocs.io/en/latest/?badge=latest)
@@ -170,14 +173,25 @@
 
 Very basic offline TTS engine.
 
 - Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
+### pyttsx3 [🌐](https://pyttsx3.readthedocs.io/)
+
+Offline TTS engine wrapper with support for the built-in TTS engines on Windows
+(SAPI5) and macOS (NSSpeechSynthesizer), as well as espeak on Linux.
+By default, it will use the most appropriate engine for your platform.
+
+- Class: [`voicebox.tts.Pyttsx3TTS`](voicebox.tts.pyttsx3.Pyttsx3TTS)
+- Setup:
+  1. `pip install "voicebox-tts[pyttsx3]"`
+  2. On Debian/Ubuntu: `sudo apt install espeak`
+
 ## Effects
 
 Built-in effect classes are located in the
 [`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
```

### Comparing `voicebox_tts-0.0.8/README.md` & `voicebox_tts-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,25 @@
 
 Very basic offline TTS engine.
 
 - Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
+### pyttsx3 [🌐](https://pyttsx3.readthedocs.io/)
+
+Offline TTS engine wrapper with support for the built-in TTS engines on Windows
+(SAPI5) and macOS (NSSpeechSynthesizer), as well as espeak on Linux.
+By default, it will use the most appropriate engine for your platform.
+
+- Class: [`voicebox.tts.Pyttsx3TTS`](voicebox.tts.pyttsx3.Pyttsx3TTS)
+- Setup:
+  1. `pip install "voicebox-tts[pyttsx3]"`
+  2. On Debian/Ubuntu: `sudo apt install espeak`
+
 ## Effects
 
 Built-in effect classes are located in the
 [`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
```

### Comparing `voicebox_tts-0.0.8/pyproject.toml` & `voicebox_tts-0.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     "voicebox-tts[dev]",
     "voicebox-tts[docs]",
     "voicebox-tts[test]",
     "voicebox-tts[amazon-polly]",
     "voicebox-tts[elevenlabs]",
     "voicebox-tts[google-cloud-tts]",
     "voicebox-tts[gtts]",
+    "voicebox-tts[pyttsx3]",
 ]
 dev = [
     "build",
     "invoke",
     "twine",
 ]
 docs = [
@@ -75,14 +76,17 @@
 google-cloud-tts = [
     "google-cloud-texttospeech",
 ]
 gtts = [
     "gTTS",
     "pydub",
 ]
+pyttsx3 = [
+    "pyttsx3",
+]
 
 [project.urls]
 Homepage = "https://github.com/austin-bowen/voicebox"
 Issues = "https://github.com/austin-bowen/voicebox/issues"
 
 [tool.setuptools.dynamic]
 version = { attr = "voicebox.version.__version__" }
```

### Comparing `voicebox_tts-0.0.8/src/voicebox/__main__.py` & `voicebox_tts-0.0.9/src/voicebox/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 import argparse
 import sys
 
-from voicebox import ParallelVoicebox
+from voicebox import SimpleVoicebox
 from voicebox.effects.normalize import Normalize
 from voicebox.sinks import WaveFile, SoundDevice
 from voicebox.ssml import SSML
 from voicebox.tts.tts import TTS
-from voicebox.voiceboxes.splitter import SimpleSentenceSplitter
 
 
 def main():
     args = _parse_args()
 
     text = _get_text(args)
 
     tts = _get_tts(args)
     effects = _get_effects(args)
     sink = _get_sink(args)
 
-    voicebox = ParallelVoicebox(
+    voicebox = SimpleVoicebox(
         tts=tts,
         effects=effects,
         sink=sink,
-        text_splitter=SimpleSentenceSplitter(),
     )
 
-    try:
-        voicebox.say(text)
-        voicebox.wait_until_done()
-    except KeyboardInterrupt:
-        pass
+    voicebox.say(text)
 
 
 def _parse_args():
     parser = argparse.ArgumentParser()
 
     parser.add_argument('text', nargs='?', help='Text to speak. If not given, text is read from stdin.')
 
     # TTS args
-    parser.add_argument('--tts', choices=('espeak-ng', 'googlecloudtts', 'gtts', 'picotts'), default='picotts',
-                        help='Which TTS engine to use. Default: picotts')
+    parser.add_argument(
+        '--tts',
+        choices=('espeak-ng', 'googlecloudtts', 'gtts', 'picotts', 'pyttsx3'),
+        default='picotts',
+        help='Which TTS engine to use. Default: picotts',
+    )
     parser.add_argument('--lang', help='Language code')
     parser.add_argument('--voice', help='Voice name')
     parser.add_argument('--ssml', action='store_true', help='Treat text as SSML')
     parser.add_argument('--pitch', help='Voice pitch')
     parser.add_argument('--speed', help='Voice speed')
 
     # Effect args
@@ -67,15 +65,15 @@
 
     text = text.strip()
 
     return SSML(text) if args.ssml else text
 
 
 def _get_tts(args) -> TTS:
-    if args.tts == 'espeakng':
+    if args.tts == 'espeak-ng':
         from voicebox.tts import ESpeakConfig, ESpeakNG
 
         return ESpeakNG(ESpeakConfig(
             voice=args.voice,
             word_gap_seconds=0.0,
             pitch=int(args.pitch) if args.pitch is not None else None,
             speed=int(args.speed) if args.speed is not None else None,
@@ -105,14 +103,18 @@
         from voicebox.tts import gTTS
         return gTTS(lang=args.lang) if args.lang is not None else gTTS()
 
     elif args.tts == 'picotts':
         from voicebox.tts import PicoTTS
         return PicoTTS(language=args.lang)
 
+    elif args.tts == 'pyttsx3':
+        from voicebox.tts import Pyttsx3TTS
+        return Pyttsx3TTS()
+
     else:
         raise ValueError(f'Unrecognized tts: {args.tts}')
 
 
 def _get_effects(args):
     effects = []
```

### Comparing `voicebox_tts-0.0.8/src/voicebox/audio.py` & `voicebox_tts-0.0.9/src/voicebox/audio.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/__init__.py` & `voicebox_tts-0.0.9/src/voicebox/effects/__init__.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/chain.py` & `voicebox_tts-0.0.9/src/voicebox/effects/chain.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/delay.py` & `voicebox_tts-0.0.9/src/voicebox/effects/delay.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/effect.py` & `voicebox_tts-0.0.9/src/voicebox/effects/effect.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/eq.py` & `voicebox_tts-0.0.9/src/voicebox/effects/eq.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/flanger.py` & `voicebox_tts-0.0.9/src/voicebox/effects/flanger.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/glitch.py` & `voicebox_tts-0.0.9/src/voicebox/effects/glitch.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/modulation.py` & `voicebox_tts-0.0.9/src/voicebox/effects/modulation.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/normalize.py` & `voicebox_tts-0.0.9/src/voicebox/effects/normalize.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/pedalboard.py` & `voicebox_tts-0.0.9/src/voicebox/effects/pedalboard.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/tail.py` & `voicebox_tts-0.0.9/src/voicebox/effects/tail.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/effects/vocoder.py` & `voicebox_tts-0.0.9/src/voicebox/effects/vocoder.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/examples/battle_droid.py` & `voicebox_tts-0.0.9/src/voicebox/examples/battle_droid.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/examples/demo.py` & `voicebox_tts-0.0.9/src/voicebox/examples/demo.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/examples/glados.py` & `voicebox_tts-0.0.9/src/voicebox/examples/glados.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/examples/halo_spark.py` & `voicebox_tts-0.0.9/src/voicebox/examples/halo_spark.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/sinks/sounddevice.py` & `voicebox_tts-0.0.9/src/voicebox/sinks/sounddevice.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/sinks/wavefile.py` & `voicebox_tts-0.0.9/src/voicebox/sinks/wavefile.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/ssml.py` & `voicebox_tts-0.0.9/src/voicebox/ssml.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/__init__.py` & `voicebox_tts-0.0.9/src/voicebox/tts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,11 +21,16 @@
 try:
     from voicebox.tts.gtts import gTTS
 except ImportError:
     pass
 
 from voicebox.tts.picotts import PicoTTS
 
+try:
+    from voicebox.tts.pyttsx3 import Pyttsx3TTS
+except ImportError:
+    pass
+
 
 def default_tts() -> TTS:
     """Returns a new instance of the default TTS, :class:`PicoTTS`."""
     return PicoTTS()
```

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/amazonpolly.py` & `voicebox_tts-0.0.9/src/voicebox/tts/amazonpolly.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/cache.py` & `voicebox_tts-0.0.9/src/voicebox/tts/cache.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/elevenlabs.py` & `voicebox_tts-0.0.9/src/voicebox/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/espeakng.py` & `voicebox_tts-0.0.9/src/voicebox/tts/espeakng.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/googlecloudtts.py` & `voicebox_tts-0.0.9/src/voicebox/tts/googlecloudtts.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/gtts.py` & `voicebox_tts-0.0.9/src/voicebox/tts/gtts.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/tts/utils.py` & `voicebox_tts-0.0.9/src/voicebox/tts/utils.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/utils.py` & `voicebox_tts-0.0.9/src/voicebox/utils.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/voiceboxes/base.py` & `voicebox_tts-0.0.9/src/voicebox/voiceboxes/base.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/voiceboxes/parallel.py` & `voicebox_tts-0.0.9/src/voicebox/voiceboxes/parallel.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/voiceboxes/queue.py` & `voicebox_tts-0.0.9/src/voicebox/voiceboxes/queue.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/voiceboxes/simple.py` & `voicebox_tts-0.0.9/src/voicebox/voiceboxes/simple.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox/voiceboxes/splitter.py` & `voicebox_tts-0.0.9/src/voicebox/voiceboxes/splitter.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/src/voicebox_tts.egg-info/PKG-INFO` & `voicebox_tts-0.0.9/src/voicebox_tts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-tts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python text-to-speech library with built-in voice effects and support for multiple TTS engines.
 Author-email: Austin Bowen <austin.bowen.314@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Austin Bowen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -50,14 +50,15 @@
 Requires-Dist: voicebox-tts[dev]; extra == "all"
 Requires-Dist: voicebox-tts[docs]; extra == "all"
 Requires-Dist: voicebox-tts[test]; extra == "all"
 Requires-Dist: voicebox-tts[amazon-polly]; extra == "all"
 Requires-Dist: voicebox-tts[elevenlabs]; extra == "all"
 Requires-Dist: voicebox-tts[google-cloud-tts]; extra == "all"
 Requires-Dist: voicebox-tts[gtts]; extra == "all"
+Requires-Dist: voicebox-tts[pyttsx3]; extra == "all"
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: invoke; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == "docs"
 Requires-Dist: sphinx; extra == "docs"
@@ -73,14 +74,16 @@
 Requires-Dist: elevenlabs; extra == "elevenlabs"
 Requires-Dist: pydub; extra == "elevenlabs"
 Provides-Extra: google-cloud-tts
 Requires-Dist: google-cloud-texttospeech; extra == "google-cloud-tts"
 Provides-Extra: gtts
 Requires-Dist: gTTS; extra == "gtts"
 Requires-Dist: pydub; extra == "gtts"
+Provides-Extra: pyttsx3
+Requires-Dist: pyttsx3; extra == "pyttsx3"
 
 # voicebox
 
 ![python-package](https://github.com/austin-bowen/voicebox/actions/workflows/python-package.yml/badge.svg)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/voicebox-tts)
 [![PyPI - Version](https://img.shields.io/pypi/v/voicebox-tts)](https://pypi.org/project/voicebox-tts/)
 [![Documentation Status](https://readthedocs.org/projects/voicebox/badge/?version=latest)](https://voicebox.readthedocs.io/en/latest/?badge=latest)
@@ -170,14 +173,25 @@
 
 Very basic offline TTS engine.
 
 - Class: [`voicebox.tts.PicoTTS`](voicebox.tts.picotts.PicoTTS)
 - Setup:
   - On Debian/Ubuntu: `sudo apt install libttspico-utils`
 
+### pyttsx3 [🌐](https://pyttsx3.readthedocs.io/)
+
+Offline TTS engine wrapper with support for the built-in TTS engines on Windows
+(SAPI5) and macOS (NSSpeechSynthesizer), as well as espeak on Linux.
+By default, it will use the most appropriate engine for your platform.
+
+- Class: [`voicebox.tts.Pyttsx3TTS`](voicebox.tts.pyttsx3.Pyttsx3TTS)
+- Setup:
+  1. `pip install "voicebox-tts[pyttsx3]"`
+  2. On Debian/Ubuntu: `sudo apt install espeak`
+
 ## Effects
 
 Built-in effect classes are located in the
 [`voicebox.effects`](voicebox.effects) package,
 and can be imported like:
 
 ```python
```

### Comparing `voicebox_tts-0.0.8/src/voicebox_tts.egg-info/SOURCES.txt` & `voicebox_tts-0.0.9/src/voicebox_tts.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/voicebox/tts/amazonpolly.py
 src/voicebox/tts/cache.py
 src/voicebox/tts/elevenlabs.py
 src/voicebox/tts/espeakng.py
 src/voicebox/tts/googlecloudtts.py
 src/voicebox/tts/gtts.py
 src/voicebox/tts/picotts.py
+src/voicebox/tts/pyttsx3.py
 src/voicebox/tts/tts.py
 src/voicebox/tts/utils.py
 src/voicebox/voiceboxes/__init__.py
 src/voicebox/voiceboxes/base.py
 src/voicebox/voiceboxes/parallel.py
 src/voicebox/voiceboxes/queue.py
 src/voicebox/voiceboxes/simple.py
```

### Comparing `voicebox_tts-0.0.8/tests/test_audio.py` & `voicebox_tts-0.0.9/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `voicebox_tts-0.0.8/tests/test_ssml.py` & `voicebox_tts-0.0.9/tests/test_ssml.py`

 * *Files identical despite different names*

