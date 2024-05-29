# Comparing `tmp/scoda-2.1b6.tar.gz` & `tmp/scoda-2.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scoda-2.1b6.tar", last modified: Mon May 27 14:59:19 2024, max compression
+gzip compressed data, was "scoda-2.1b7.tar", last modified: Wed May 29 13:55:38 2024, max compression
```

## Comparing `scoda-2.1b6.tar` & `scoda-2.1b7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-27 14:59:09.000000 scoda-2.1b6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-27 14:59:19.139394 scoda-2.1b6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-27 14:59:09.000000 scoda-2.1b6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-27 14:59:09.000000 scoda-2.1b6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/config/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/elements/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/enumerations/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/tokenisation_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/enumerations/tokeniser_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.135394 scoda-2.1b6/scoda/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/bar_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/sequence_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/tokenisation_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/exceptions/track_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/midi/
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/midi/midi_track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/misc/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/music_theory.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/scoda_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/misc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/sequences/
--rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/absolute_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/abstract_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    31799 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/relative_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/sequences/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda/tokenisation/
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/base_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/gridlike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/midilike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/notelike_tokenisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9199 2024-05-27 14:59:09.000000 scoda-2.1b6/scoda/tokenisation/transposed_notelike_tokenisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 14:59:19.139394 scoda-2.1b6/scoda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 14:59:19.000000 scoda-2.1b6/scoda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 14:59:19.139394 scoda-2.1b6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 13:55:33.000000 scoda-2.1b7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 13:55:38.214386 scoda-2.1b7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-29 13:55:33.000000 scoda-2.1b7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-29 13:55:33.000000 scoda-2.1b7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.206386 scoda-2.1b7/scoda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.210386 scoda-2.1b7/scoda/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/config/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.210386 scoda-2.1b7/scoda/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/elements/bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/elements/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/elements/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/elements/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.210386 scoda-2.1b7/scoda/enumerations/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/enumerations/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/enumerations/tokenisation_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/enumerations/tokeniser_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.210386 scoda-2.1b7/scoda/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/exceptions/bar_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/exceptions/sequence_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/exceptions/tokenisation_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/exceptions/track_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.210386 scoda-2.1b7/scoda/midi/
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/midi/midi_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/midi/midi_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/midi/midi_track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/scoda/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/misc/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/misc/music_theory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/misc/scoda_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6517 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/misc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/scoda/sequences/
+-rw-r--r--   0 runner    (1001) docker     (127)    21887 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/sequences/absolute_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/sequences/abstract_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31799 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/sequences/relative_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23992 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/sequences/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/scoda/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     6850 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/scoda/tokenisation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/tokenisation/base_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/tokenisation/gridlike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/tokenisation/midilike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/tokenisation/notelike_tokenisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-29 13:55:33.000000 scoda-2.1b7/scoda/tokenisation/transposed_notelike_tokenisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:55:38.214386 scoda-2.1b7/scoda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-29 13:55:38.000000 scoda-2.1b7/scoda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-29 13:55:38.000000 scoda-2.1b7/scoda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:55:38.000000 scoda-2.1b7/scoda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-29 13:55:38.000000 scoda-2.1b7/scoda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 13:55:38.000000 scoda-2.1b7/scoda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:55:38.214386 scoda-2.1b7/setup.cfg
```

### Comparing `scoda-2.1b6/LICENSE.md` & `scoda-2.1b7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/PKG-INFO` & `scoda-2.1b7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b6
+Version: 2.1b7
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b6/README.md` & `scoda-2.1b7/README.md`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/pyproject.toml` & `scoda-2.1b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "scoda"
-version = "2.1-beta.6"
+version = "2.1-beta.7"
 authors = [{ name = "Felix Schön", email = "schoen@kr.tuwien.ac.at" }]
 description = "A MIDI and music data manipulation library"
 readme = "README.md"
 requires-python = ">= 3.11"
 keywords = ["midi", "music"]
 license = { file = "LICENSE.md" }
 dependencies = [
```

### Comparing `scoda-2.1b6/scoda/config/settings.json` & `scoda-2.1b7/scoda/config/settings.json`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/elements/bar.py` & `scoda-2.1b7/scoda/elements/bar.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/elements/composition.py` & `scoda-2.1b7/scoda/elements/composition.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/elements/message.py` & `scoda-2.1b7/scoda/elements/message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/elements/track.py` & `scoda-2.1b7/scoda/elements/track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/enumerations/tokeniser_type.py` & `scoda-2.1b7/scoda/enumerations/tokeniser_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import enum
 
 
 class TokeniserType(enum.Enum):
     STANDARD_MIDILIKE_TOKENISER = "standard_midilike_tokeniser"
+    COF_MIDILIKE_TOKENISER = "cof_midilike_tokeniser"
     STANDARD_NOTELIKE_TOKENISER = "standard_notelike_tokeniser"
     LARGE_DICTIONARY_NOTELIKE_TOKENISER = "large_dictionary_notelike_tokeniser"
     COF_NOTELIKE_TOKENISER = "cof_notelike_tokeniser"
     LARGE_DICTIONARY_COF_NOTELIKE_TOKENISER = "large_dictionary_cof_notelike_tokeniser"
     GRIDLIKE_TOKENISER = "gridlike_tokeniser"
     TRANSPOSED_NOTELIKE_TOKENISER = "transposed_notelike_tokeniser"
```

### Comparing `scoda-2.1b6/scoda/midi/midi_file.py` & `scoda-2.1b7/scoda/midi/midi_file.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/midi/midi_message.py` & `scoda-2.1b7/scoda/midi/midi_message.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/midi/midi_track.py` & `scoda-2.1b7/scoda/midi/midi_track.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/misc/music_theory.py` & `scoda-2.1b7/scoda/misc/music_theory.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/misc/scoda_logging.py` & `scoda-2.1b7/scoda/misc/scoda_logging.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/misc/util.py` & `scoda-2.1b7/scoda/misc/util.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/sequences/absolute_sequence.py` & `scoda-2.1b7/scoda/sequences/absolute_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/sequences/abstract_sequence.py` & `scoda-2.1b7/scoda/sequences/abstract_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/sequences/relative_sequence.py` & `scoda-2.1b7/scoda/sequences/relative_sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/sequences/sequence.py` & `scoda-2.1b7/scoda/sequences/sequence.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/settings/settings.py` & `scoda-2.1b7/scoda/settings/settings.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/tokenisation/base_tokenisation.py` & `scoda-2.1b7/scoda/tokenisation/base_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/tokenisation/gridlike_tokenisation.py` & `scoda-2.1b7/scoda/tokenisation/gridlike_tokenisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,30 +6,28 @@
 from scoda.enumerations.tokenisation_flags import TokenisationFlags
 from scoda.exceptions.tokenisation_exception import TokenisationException
 from scoda.sequences.sequence import Sequence
 from scoda.tokenisation.base_tokenisation import BaseTokeniser
 
 
 class BaseGridlikeTokeniser(BaseTokeniser, ABC):
-    TOKEN_SEPARATOR = None
-
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__()
 
         self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
 
 class GridlikeTokeniser(BaseGridlikeTokeniser):
     """Tokeniser that uses grid-like temporal representation. Note that input sequences are expected to represent bars,
     as the grid size definition is redone for each input sequence.
 
     [        0] ... pad
     [        1] ... start
     [        2] ... stop
-    [        3] ... grid
+    [        3] ... bar separator
     [  4 -  27] ... grid time definition
     [ 28 - 115] ... note on
     [116 - 203] ... note off
     [204 - 218] ... time signature numerator in eights from 2/8 to 16/8
     """
 
     def __init__(self, running_time_sig: bool) -> None:
```

### Comparing `scoda-2.1b6/scoda/tokenisation/midilike_tokenisation.py` & `scoda-2.1b7/scoda/tokenisation/midilike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/tokenisation/notelike_tokenisation.py` & `scoda-2.1b7/scoda/tokenisation/notelike_tokenisation.py`

 * *Files identical despite different names*

### Comparing `scoda-2.1b6/scoda/tokenisation/transposed_notelike_tokenisation.py` & `scoda-2.1b7/scoda/tokenisation/transposed_notelike_tokenisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,26 +14,25 @@
 
     def __init__(self, running_time_sig: bool) -> None:
         super().__init__()
 
         self.flags[TokenisationFlags.RUNNING_TIME_SIG] = running_time_sig
 
 
-# TODO
 class TransposedNotelikeTokeniser(BaseTransposedNotelikeTokeniser):
     """Tokeniser that uses transposed temporal representation with a note-like approach, i.e., all occurrences of a note
     are shown first before any other note is handled. Note that input sequences are expected to represent bars,
     as the transposed representation is done on a per-bar basis.
 
     [        0] ... pad
     [        1] ... start
     [        2] ... stop
-    [        3] ... play
+    [        3] ... bar separator
     [        4] ... wait
-    [        5] ... bar border
+    [        5] ... play
     [  6 -  29] ... value definition
     [ 30 - 117] ... note
     [118 - 132] ... time signature numerator in eights from 2/8 to 16/8
     """
 
     def __init__(self, running_value: bool, running_time_sig: bool) -> None:
         super().__init__(running_time_sig)
@@ -107,15 +106,15 @@
                                                                       index_time_def=6))
 
                     # Check if value of note has to be defined
                     if not (self.prv_value == msg_value and self.flags.get(TokenisationFlags.RUNNING_VALUE, False)):
                         tokens.extend(self._general_tokenise_flush_time_buffer(msg_value, index_time_def=6))
 
                     # Play note
-                    tokens.append(3)
+                    tokens.append(5)
 
                     self.cur_time_target = max(self.cur_time_target, self.cur_time + msg_value)
                     self.prv_type = MessageType.NOTE_ON
                     self.prv_value = msg_value
                 elif msg_type == MessageType.TIME_SIGNATURE:
                     msg_numerator = event_pairing[0].numerator
                     msg_denominator = event_pairing[0].denominator
@@ -144,15 +143,15 @@
             tokens.extend(
                 self._notelike_tokenise_flush_rest_buffer(apply_target=True, wait_token=4, index_time_def=6))
 
         if reset_time:
             self.reset_time()
 
         # Insert bar border mark
-        tokens.append(5)
+        tokens.append(3)
 
         if insert_border_tokens:
             tokens.insert(0, 1)
             tokens.append(2)
 
         return tokens
 
@@ -168,31 +167,31 @@
         prv_value = math.nan
         prv_numerator = math.nan
 
         for token in tokens:
             if token <= 2:
                 prv_type = "sequence_control"
             elif token == 3:
+                time_bar_start += prv_numerator * PPQN / 2
+                cur_time_bar = 0
+
+                prv_type = "bar_border"
+            elif token == 4:
+                cur_time_bar += prv_value
+
+                prv_type = MessageType.WAIT
+            elif token == 5:
                 seq.add_absolute_message(
                     Message(message_type=MessageType.NOTE_ON, note=prv_note,
                             time=time_bar_start + cur_time_bar))
                 seq.add_absolute_message(
                     Message(message_type=MessageType.NOTE_OFF, note=prv_note,
                             time=time_bar_start + cur_time_bar + prv_value))
 
                 prv_type = MessageType.NOTE_ON
-            elif token == 4:
-                cur_time_bar += prv_value
-
-                prv_type = MessageType.WAIT
-            elif token == 5:
-                time_bar_start += prv_numerator * PPQN / 2
-                cur_time_bar = 0
-
-                prv_type = "bar_border"
             elif 6 <= token <= 29:
                 if prv_type == "value_definition":
                     prv_value += token - 5
                 else:
                     prv_value = token - 5
 
                 prv_type = "value_definition"
```

### Comparing `scoda-2.1b6/scoda.egg-info/PKG-INFO` & `scoda-2.1b7/scoda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scoda
-Version: 2.1b6
+Version: 2.1b7
 Summary: A MIDI and music data manipulation library
 Author-email: Felix Schön <schoen@kr.tuwien.ac.at>
 License: MIT License
         
         Copyright (c) 2023 Felix Schön
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `scoda-2.1b6/scoda.egg-info/SOURCES.txt` & `scoda-2.1b7/scoda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

