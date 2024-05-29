# Comparing `tmp/openwillis-2.1.4.tar.gz` & `tmp/openwillis-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwillis-2.1.4.tar", last modified: Mon Apr  8 16:05:28 2024, max compression
+gzip compressed data, was "openwillis-2.1.6.tar", last modified: Wed May 29 18:46:46 2024, max compression
```

## Comparing `openwillis-2.1.4.tar` & `openwillis-2.1.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.702885 openwillis-2.1.4/
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-04-08 16:04:57.000000 openwillis-2.1.4/LICENSE.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-04-08 16:04:57.000000 openwillis-2.1.4/MANIFEST.in
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 16:05:28.702974 openwillis-2.1.4/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1063 2024-04-08 16:04:57.000000 openwillis-2.1.4/README.md
--rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-04-08 16:04:57.000000 openwillis-2.1.4/RELEASE.md
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.692184 openwillis-2.1.4/openwillis/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.693730 openwillis-2.1.4/openwillis/measures/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/api.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.695758 openwillis-2.1.4/openwillis/measures/audio/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/acoustic.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.696352 openwillis-2.1.4/openwillis/measures/audio/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/config/acoustic.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/config/speech.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/speech_separation_labels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/speech_separation_nlabels.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     4055 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_cloud.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_vosk.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5004 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_whisper.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.698578 openwillis-2.1.4/openwillis/measures/audio/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/acoustic_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/disvoice_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/separation_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/transcribe_util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/util.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     5939 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/audio/util/whisperx_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.699020 openwillis-2.1.4/openwillis/measures/commons/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/commons/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/commons/common.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.699565 openwillis-2.1.4/openwillis/measures/gps/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/gps/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/gps/geolocation_processing.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.699974 openwillis-2.1.4/openwillis/measures/gps/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/gps/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/gps/util/gps_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.700605 openwillis-2.1.4/openwillis/measures/text/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/text/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.700862 openwillis-2.1.4/openwillis/measures/text/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/text/config/text.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/text/speech_attribute.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.701205 openwillis-2.1.4/openwillis/measures/text/util/
--rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/text/util/__init__.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    70872 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/text/util/characteristics_util.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.702160 openwillis-2.1.4/openwillis/measures/video/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/__init__.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.702636 openwillis-2.1.4/openwillis/measures/video/config/
--rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/config/eye.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/config/facial.json
--rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/eye_blink.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/face_landmark.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/measures/video/facial_emotion.py
--rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-04-08 16:04:57.000000 openwillis-2.1.4/openwillis/usability.py
-drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-04-08 16:05:28.693452 openwillis-2.1.4/openwillis.egg-info/
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/PKG-INFO
--rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/SOURCES.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/dependency_links.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/not-zip-safe
--rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/requires.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-04-08 16:05:28.000000 openwillis-2.1.4/openwillis.egg-info/top_level.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-04-08 16:04:57.000000 openwillis-2.1.4/requirements.txt
--rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-04-08 16:05:28.703339 openwillis-2.1.4/setup.cfg
--rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-04-08 16:04:58.000000 openwillis-2.1.4/setup.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.956688 openwillis-2.1.6/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13641 2024-05-29 18:46:28.000000 openwillis-2.1.6/LICENSE.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      305 2024-05-29 18:46:28.000000 openwillis-2.1.6/MANIFEST.in
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-05-29 18:46:46.956769 openwillis-2.1.6/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1063 2024-05-29 18:46:28.000000 openwillis-2.1.6/README.md
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      227 2024-05-29 18:46:28.000000 openwillis-2.1.6/RELEASE.md
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.946791 openwillis-2.1.6/openwillis/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      749 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.948248 openwillis-2.1.6/openwillis/measures/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      614 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/api.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.949932 openwillis-2.1.6/openwillis/measures/audio/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      740 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    11989 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/acoustic.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.950366 openwillis-2.1.6/openwillis/measures/audio/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2212 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/config/acoustic.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    27050 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/config/speech.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     3152 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/speech_separation_labels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5679 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/speech_separation_nlabels.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     4240 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_cloud.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     8333 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_vosk.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5131 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_whisper.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.952256 openwillis-2.1.6/openwillis/measures/audio/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    17921 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/acoustic_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    19402 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/disvoice_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    14319 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/separation_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    15317 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/transcribe_util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1764 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/util.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     5954 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/audio/util/whisperx_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.952830 openwillis-2.1.6/openwillis/measures/commons/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      114 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/commons/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     2794 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/commons/common.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.953206 openwillis-2.1.6/openwillis/measures/gps/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      109 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/gps/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6791 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/gps/geolocation_processing.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.953584 openwillis-2.1.6/openwillis/measures/gps/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/gps/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12880 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/gps/util/gps_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.954150 openwillis-2.1.6/openwillis/measures/text/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      124 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/text/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.954427 openwillis-2.1.6/openwillis/measures/text/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     6544 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/text/config/text.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    12198 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/text/speech_attribute.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.954730 openwillis-2.1.6/openwillis/measures/text/util/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/text/util/__init__.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    70872 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/text/util/characteristics_util.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.956118 openwillis-2.1.6/openwillis/measures/video/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      318 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/__init__.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.956516 openwillis-2.1.6/openwillis/measures/video/config/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      484 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/config/eye.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1877 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/config/facial.json
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    13215 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/eye_blink.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    22642 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/face_landmark.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)    10473 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/measures/video/facial_emotion.py
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      145 2024-05-29 18:46:28.000000 openwillis-2.1.6/openwillis/usability.py
+drwxr-xr-x   0 vijayyadav   (501) staff       (20)        0 2024-05-29 18:46:46.948020 openwillis-2.1.6/openwillis.egg-info/
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1362 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/PKG-INFO
+-rw-r--r--   0 vijayyadav   (501) staff       (20)     1868 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/SOURCES.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/dependency_links.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)        1 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/not-zip-safe
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      414 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/requires.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       11 2024-05-29 18:46:46.000000 openwillis-2.1.6/openwillis.egg-info/top_level.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      427 2024-05-29 18:46:28.000000 openwillis-2.1.6/requirements.txt
+-rw-r--r--   0 vijayyadav   (501) staff       (20)       79 2024-05-29 18:46:46.956977 openwillis-2.1.6/setup.cfg
+-rw-r--r--   0 vijayyadav   (501) staff       (20)      934 2024-05-29 18:46:28.000000 openwillis-2.1.6/setup.py
```

### Comparing `openwillis-2.1.4/LICENSE.txt` & `openwillis-2.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/PKG-INFO` & `openwillis-2.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.4
+Version: 2.1.6
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-2.1.4/README.md` & `openwillis-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/__init__.py` & `openwillis-2.1.6/openwillis/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/api.py` & `openwillis-2.1.6/openwillis/measures/api.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/__init__.py` & `openwillis-2.1.6/openwillis/measures/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/acoustic.py` & `openwillis-2.1.6/openwillis/measures/audio/acoustic.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/config/acoustic.json` & `openwillis-2.1.6/openwillis/measures/audio/config/acoustic.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/config/speech.json` & `openwillis-2.1.6/openwillis/measures/audio/config/speech.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/speech_separation_labels.py` & `openwillis-2.1.6/openwillis/measures/audio/speech_separation_labels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/speech_separation_nlabels.py` & `openwillis-2.1.6/openwillis/measures/audio/speech_separation_nlabels.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_cloud.py` & `openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_cloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -101,13 +101,17 @@
         The transcript of the recording.
 
     ------------------------------------------------------------------------------------------------------
     """
     input_param = read_kwargs(kwargs)
     measures = get_config()
     json_response, transcript = tutil.transcribe_audio(s3_uri, input_param)
-    
+
+    present_labels = [x['speaker_label'] for x in json_response['results']['items'] if 'speaker_label' in x]
+    if len(set(present_labels)) != 2:
+        return json_response, transcript
+
     if input_param['speaker_labels'] == True and input_param['context'].lower() in measures['scale'].split(','):
         content_dict = tutil.extract_content(json_response)
         
         json_response = tutil.get_clinical_labels(input_param['context'], measures, content_dict, json_response)
     return json_response, transcript
```

### Comparing `openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_vosk.py` & `openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_vosk.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/speech_transcribe_whisper.py` & `openwillis-2.1.6/openwillis/measures/audio/speech_transcribe_whisper.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,17 @@
     input_param['context'] = kwargs.get('context', '')
     input_param['max_speakers'] = kwargs.get('max_speakers', None)
     input_param['min_speakers'] = kwargs.get('min_speakers', None)
 
     input_param['hf_token'] = kwargs.get('hf_token', '')
     input_param['del_model'] = kwargs.get('del_model', False) #Temp filter
     input_param['infra_model'] = kwargs.get('infra_model', [True, None, None]) #Temp filter
-    
+    input_param['compute_type'] = kwargs.get('compute_type', 'int16')
+    input_param['batch_size'] = kwargs.get('batch_size', 16)
+
     return input_param
 
 def run_whisperx(filepath, input_param):
     """
     ------------------------------------------------------------------------------------------------------
 
     Transcribe audio data using the WhisperX model.
```

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/acoustic_util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/acoustic_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/disvoice_util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/disvoice_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/separation_util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/separation_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/transcribe_util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/transcribe_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/audio/util/whisperx_util.py` & `openwillis-2.1.6/openwillis/measures/audio/util/whisperx_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         The path to the audio file to be transcribed.
     model: str
         name of the pretrained model
     device: str
         cpu vs gpu
     compute_type: str
         computation format
-    batch_size: str
+    batch_size: int
         batch size
     infra_model:list
         whisper model artifacts (this is optional param: to optimize willisInfra) 
     language: str
         language code
 
         
@@ -149,26 +149,25 @@
         A transcription response object in JSON format
     transcript : str
         The transcript of the recording.
 
     ------------------------------------------------------------------------------------------------------
     """
     device = 'cpu'
-    compute_type = "int16"
-    batch_size = 16
+    compute_type = input_param['compute_type']
     
     json_response = json.dumps({})
     transcript = ''
     
     try:
         if torch.cuda.is_available():
             device = 'cuda'
             compute_type = "float16"
     
-        transcribe_json, audio = transcribe_whisper(filepath, input_param['model'], device, compute_type, batch_size, input_param['infra_model'], input_param['language'])
+        transcribe_json, audio = transcribe_whisper(filepath, input_param['model'], device, compute_type, input_param['batch_size'], input_param['infra_model'], input_param['language'])
     
         # Align whisper output
         model_a, metadata = whisperx.load_align_model(language_code=input_param['language'], device=device)
         align_json = whisperx.align(transcribe_json["segments"], model_a, metadata, audio, device, return_char_alignments=False)
     
         if input_param['del_model']:
             delete_model(model_a)
```

### Comparing `openwillis-2.1.4/openwillis/measures/commons/common.py` & `openwillis-2.1.6/openwillis/measures/commons/common.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/gps/geolocation_processing.py` & `openwillis-2.1.6/openwillis/measures/gps/geolocation_processing.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/gps/util/gps_util.py` & `openwillis-2.1.6/openwillis/measures/gps/util/gps_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/text/config/text.json` & `openwillis-2.1.6/openwillis/measures/text/config/text.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/text/speech_attribute.py` & `openwillis-2.1.6/openwillis/measures/text/speech_attribute.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/text/util/characteristics_util.py` & `openwillis-2.1.6/openwillis/measures/text/util/characteristics_util.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/video/config/facial.json` & `openwillis-2.1.6/openwillis/measures/video/config/facial.json`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/video/eye_blink.py` & `openwillis-2.1.6/openwillis/measures/video/eye_blink.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/video/face_landmark.py` & `openwillis-2.1.6/openwillis/measures/video/face_landmark.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis/measures/video/facial_emotion.py` & `openwillis-2.1.6/openwillis/measures/video/facial_emotion.py`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/openwillis.egg-info/PKG-INFO` & `openwillis-2.1.6/openwillis.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwillis
-Version: 2.1.4
+Version: 2.1.6
 Summary: digital health measurement
 Home-page: https://github.com/bklynhlth/openwillis
 Author: bklynhlth
 Author-email: admin@bklynhlth.com
 License: Apache
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `openwillis-2.1.4/openwillis.egg-info/SOURCES.txt` & `openwillis-2.1.6/openwillis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwillis-2.1.4/setup.py` & `openwillis-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = fp.read()
 
 setuptools.setup(name='openwillis',
-                 version='2.1.4',
+                 version='2.1.6',
                  description='digital health measurement',
                  long_description=long_description,
                  long_description_content_type="text/markdown",
                  url='https://github.com/bklynhlth/openwillis',
                  author='bklynhlth',
                  python_requires='>=3.6',
                  install_requires=install_requires,
```

