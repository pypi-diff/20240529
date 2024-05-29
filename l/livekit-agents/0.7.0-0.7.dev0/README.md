# Comparing `tmp/livekit_agents-0.7.0.tar.gz` & `tmp/livekit_agents-0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_agents-0.7.0.tar", last modified: Wed May 29 21:31:45 2024, max compression
+gzip compressed data, was "livekit_agents-0.7.dev0.tar", last modified: Thu May 23 15:56:19 2024, max compression
```

## Comparing `livekit_agents-0.7.0.tar` & `livekit_agents-0.7.dev0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.030901 livekit_agents-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-29 21:31:45.030901 livekit_agents-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.014901 livekit_agents-0.7.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.018901 livekit_agents-0.7.0/livekit/agents/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.018901 livekit_agents-0.7.0/livekit/agents/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/sleep.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/aio/wait_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/apipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/cli/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/cli/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/cli/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/codecs/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/codecs/mp3.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/http_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/ipc/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc/job_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc/job_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/ipc_enc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/job_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/job_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/llm/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/llm/function_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/llm/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/stt/
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/stt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/stt/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/stt/stt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.022901 livekit_agents-0.7.0/livekit/agents/tokenize/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36820 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/_basic_hyphenator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/_basic_sent.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/_basic_word.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/token_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tokenize/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.026901 livekit_agents-0.7.0/livekit/agents/transcription/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/transcription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/transcription/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/transcription/stt_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (127)    12202 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/transcription/tts_forwarder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.026901 livekit_agents-0.7.0/livekit/agents/tts/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tts/stream_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/tts/tts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.026901 livekit_agents-0.7.0/livekit/agents/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/_noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/exp_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/http_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/utils/moving_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/vad.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.026901 livekit_agents-0.7.0/livekit/agents/voice_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/voice_assistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32898 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/voice_assistant/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/voice_assistant/plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/livekit/agents/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:31:45.026901 livekit_agents-0.7.0/livekit_agents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-29 21:31:45.000000 livekit_agents-0.7.0/livekit_agents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 21:31:45.000000 livekit_agents-0.7.0/livekit_agents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:31:45.000000 livekit_agents-0.7.0/livekit_agents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 21:31:45.000000 livekit_agents-0.7.0/livekit_agents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:31:45.000000 livekit_agents-0.7.0/livekit_agents.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:31:45.030901 livekit_agents-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 21:31:40.000000 livekit_agents-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.781198 livekit_agents-0.7.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/aio/wait_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/apipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/cli/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.785198 livekit_agents-0.7.dev0/livekit/agents/codecs/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/codecs/mp3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/http_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/ipc/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6139 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/job_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/job_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/ipc_enc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/job_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/job_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/function_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/llm/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/stt/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/stt/stt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/tokenize/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36820 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_hyphenator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_sent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_word.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/token_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tokenize/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/transcription/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/stt_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/transcription/tts_forwarder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.789198 livekit_agents-0.7.dev0/livekit/agents/tts/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/stream_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/tts/tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit/agents/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/_noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/exp_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/http_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/utils/moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/vad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32625 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/voice_assistant/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18976 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/livekit/agents/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/livekit_agents.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:56:19.000000 livekit_agents-0.7.dev0/livekit_agents.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:56:19.793198 livekit_agents-0.7.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 15:56:15.000000 livekit_agents-0.7.dev0/setup.py
```

### Comparing `livekit_agents-0.7.0/PKG-INFO` & `livekit_agents-0.7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.7.0
+Version: 0.7.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.7.0/livekit/agents/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/channel.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/channel.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/debug.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/debug.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/interval.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/interval.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/select.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/select.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/sleep.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/sleep.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/aio/wait_group.py` & `livekit_agents-0.7.dev0/livekit/agents/aio/wait_group.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/apipe.py` & `livekit_agents-0.7.dev0/livekit/agents/apipe.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/cli/cli.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -197,16 +197,16 @@
 
     setup_logging(args.log_level, args.production)
 
     loop = asyncio.get_event_loop()
     worker = Worker(args.opts, loop=loop)
 
     loop.set_debug(args.asyncio_debug)
-    loop.slow_callback_duration = 0.05  # 50ms
-    aio.debug.hook_slow_callbacks(2)
+    loop.slow_callback_duration = 0.03  # 30ms
+    aio.debug.hook_slow_callbacks(0.75)
 
     if args.room:
         # directly connect to a specific roomj
         @worker.once("worker_registered")
         def _connect_on_register(worker_id: str, server_info: models.ServerInfo):
             logger.info("connecting to room %s", args.room)
             loop.create_task(worker.simulate_job(args.room, args.participant_identity))
```

### Comparing `livekit_agents-0.7.0/livekit/agents/cli/log.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/log.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/cli/protocol.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/cli/watcher.py` & `livekit_agents-0.7.dev0/livekit/agents/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/codecs/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/codecs/mp3.py` & `livekit_agents-0.7.dev0/livekit/agents/codecs/mp3.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/http_server.py` & `livekit_agents-0.7.dev0/livekit/agents/http_server.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/ipc/job_main.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/job_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,16 +167,16 @@
     # current process pid
     logger.debug(
         "process started",
         extra={"url": args.url},
     )
 
     pipe = apipe.AsyncPipe(cch, loop, protocol.IPC_MESSAGES)
-    loop.slow_callback_duration = 0.05  # 50ms
-    aio.debug.hook_slow_callbacks(2)  # start warning after 2s
+    loop.slow_callback_duration = 0.03  # 30ms
+    aio.debug.hook_slow_callbacks(0.75)
     loop.set_debug(args.asyncio_debug)
 
     room = rtc.Room(loop=loop)
     main_task = loop.create_task(_start(pipe, args, room))
 
     try:
         loop.run_until_complete(main_task)
```

### Comparing `livekit_agents-0.7.0/livekit/agents/ipc/job_process.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/job_process.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/ipc/protocol.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc/protocol.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/ipc_enc.py` & `livekit_agents-0.7.dev0/livekit/agents/ipc_enc.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/job_context.py` & `livekit_agents-0.7.dev0/livekit/agents/job_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/job_request.py` & `livekit_agents-0.7.dev0/livekit/agents/job_request.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/llm/__init__.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/llm/function_context.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/function_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/llm/llm.py` & `livekit_agents-0.7.dev0/livekit/agents/llm/llm.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/plugin.py` & `livekit_agents-0.7.dev0/livekit/agents/plugin.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/stt/stream_adapter.py` & `livekit_agents-0.7.dev0/livekit/agents/stt/stream_adapter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/stt/stt.py` & `livekit_agents-0.7.dev0/livekit/agents/stt/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/_basic_hyphenator.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_hyphenator.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/_basic_sent.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_sent.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/_basic_word.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/_basic_word.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/basic.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/basic.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/token_stream.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/token_stream.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/tokenize/tokenizer.py` & `livekit_agents-0.7.dev0/livekit/agents/tokenize/tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/transcription/_utils.py` & `livekit_agents-0.7.dev0/livekit/agents/transcription/_utils.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/transcription/stt_forwarder.py` & `livekit_agents-0.7.dev0/livekit/agents/transcription/stt_forwarder.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/transcription/tts_forwarder.py` & `livekit_agents-0.7.dev0/livekit/agents/transcription/tts_forwarder.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,33 +21,30 @@
     track_id: str
     language: str
     speed: float
     auto_playout: bool
     word_tokenizer: tokenize.WordTokenizer
     sentence_tokenizer: tokenize.SentenceTokenizer
     hyphenate_word: Callable[[str], list[str]]
-    new_sentence_delay: float
-    debug: bool = False
 
 
 @define
 class _SegmentData:
     sentence_stream: tokenize.SentenceStream
     text: str
-    sentence_count: int
     audio_duration: float
     avg_speed: float | None
     processed_hyphenes: int
-    ready_future: asyncio.Future  # marked ready on the first audio frame
+    first_frame_future: asyncio.Future
 
 
 def _validate_playout(seg: _SegmentData) -> None:
     if seg.audio_duration == 0.0:
         with contextlib.suppress(asyncio.InvalidStateError):
-            seg.ready_future.set_result(None)
+            seg.first_frame_future.set_result(None)
 
 
 @define
 class _PendingSegments:
     cur_audio: _SegmentData
     cur_text: _SegmentData
     q: deque[_SegmentData]
@@ -64,39 +61,20 @@
     def __init__(
         self,
         *,
         room: rtc.Room,
         participant: rtc.Participant | str,
         track: rtc.Track | rtc.TrackPublication | str | None = None,
         language: str = "",
-        speed: float = 3.83,
-        new_sentence_delay: float = 0.7,
+        speed: float = 4,
         auto_playout: bool = True,
         word_tokenizer: tokenize.WordTokenizer = tokenize.basic.WordTokenizer(),
         sentence_tokenizer: tokenize.SentenceTokenizer = tokenize.basic.SentenceTokenizer(),
         hyphenate_word: Callable[[str], list[str]] = tokenize.basic.hyphenate_word,
-        debug: bool = False,
     ):
-        """
-        Args:
-            room: room where the transcription will be sent
-            participant: participant or identity that is pushing the TTS
-            track: track where the TTS audio is being sent
-            language: language of the text
-            speed: average speech speed in characters per second (used by default if the full audio is not received yet)
-            new_sentence_delay: delay in seconds between sentences
-            auto_playout: if True, the forwarder will automatically start the transcription once the
-                first audio frame is received. If False, you need to call segment_playout_started
-                to start the transcription.
-            word_tokenizer: word tokenizer used to split the text into words
-            sentence_tokenizer: sentence tokenizer used to split the text into sentences
-            hyphenate_word: function that returns a list of hyphenes for a given word
-            debug: if True, debug messages will be printed
-
-        """
         identity = participant if isinstance(participant, str) else participant.identity
 
         if track is None:
             track = _utils.find_micro_track_id(room, identity)
         elif isinstance(track, (rtc.TrackPublication, rtc.Track)):
             track = track.sid
 
@@ -106,15 +84,14 @@
             track_id=track,
             language=language,
             speed=speed,
             auto_playout=auto_playout,
             word_tokenizer=word_tokenizer,
             sentence_tokenizer=sentence_tokenizer,
             hyphenate_word=hyphenate_word,
-            new_sentence_delay=new_sentence_delay,
         )
 
         self._main_task = asyncio.create_task(self._run())
 
         # current segment where the user may still be pushing text & audio
         first_segment = self._create_segment()
         segments_q = deque()
@@ -124,88 +101,68 @@
             cur_audio=first_segment,
             cur_text=first_segment,
             q=segments_q,
         )
 
         self._seg_queue = asyncio.Queue[Optional[_SegmentData]]()
         self._seg_queue.put_nowait(first_segment)
-        self._validated_playout_q = asyncio.Queue[None]()
 
-        self._closed = False
+        self._validated_playout_q = asyncio.Queue[None]()
 
     def segment_playout_started(self) -> None:
         """Call this function when the playout of the audio segment starts,
         this will start forwarding the transcription for the current segment.
 
         This is only needed if auto_playout is set to False.
 
         Note that you don't need to wait for the first synthesized audio frame to call this function.
         The forwarder will wait for the first audio frame before starting the transcription.
         """
         self._validated_playout_q.put_nowait(None)
 
     def push_audio(self, frame: rtc.AudioFrame | None, **kwargs) -> None:
-        if self._closed:
-            raise RuntimeError("push_audio called after close")
-
         if frame is not None:
             frame_duration = frame.samples_per_channel / frame.sample_rate
             cur_seg = self._pending_segment.cur_audio
             _validate_playout(cur_seg)
             cur_seg.audio_duration += frame_duration
         else:
             self.mark_audio_segment_end()
 
     def mark_audio_segment_end(self) -> None:
-        if self._closed:
-            raise RuntimeError("mark_audio_segment_end called after close")
-
         try:
             # get last ended segment (text always end before audio)
             seg = self._pending_segment.q.popleft()
         except IndexError:
             raise IndexError(
                 "mark_audio_segment_end called before any mark_text_segment_end"
             )
 
         seg.avg_speed = len(self._calc_hyphenes(seg.text)) / seg.audio_duration
         self._pending_segment.cur_audio = self._pending_segment.q[0]
-        self._log_debug(
-            f"mark_audio_segment_end: calculated avg speed: {seg.avg_speed}"
-        )
 
     def push_text(self, text: str | None) -> None:
-        if self._closed:
-            raise RuntimeError("push_text called after close")
-
         if text is not None:
             cur_seg = self._pending_segment.cur_text
             cur_seg.text += text
             cur_seg.sentence_stream.push_text(text)
         else:
             self.mark_text_segment_end()
 
     def mark_text_segment_end(self) -> None:
-        if self._closed:
-            raise RuntimeError("mark_text_segment_end called after close")
-
         # create new segment on "mark_text_segment_end"
         self._pending_segment.cur_text.sentence_stream.mark_segment_end()
         new_seg = self._create_segment()
         self._pending_segment.cur_text = new_seg
         self._pending_segment.q.append(new_seg)
         self._seg_queue.put_nowait(new_seg)
 
     async def aclose(self, *, wait: bool = True) -> None:
-        self._closed = True
         self._seg_queue.put_nowait(None)
 
-        for seg in self._pending_segment.q:
-            seg.ready_future.cancel()
-
         if not wait:
             self._main_task.cancel()
 
         with contextlib.suppress(asyncio.CancelledError):
             await self._main_task
 
     async def _run(self) -> None:
@@ -218,19 +175,18 @@
         except Exception:
             logger.exception("error in tts transcription")
 
     def _create_segment(self) -> _SegmentData:
         return _SegmentData(
             sentence_stream=self._opts.sentence_tokenizer.stream(),
             text="",
-            sentence_count=0,
             audio_duration=0.0,
             avg_speed=None,
             processed_hyphenes=0,
-            ready_future=asyncio.Future(),
+            first_frame_future=asyncio.Future(),
         )
 
     async def _forward(self, q: asyncio.Queue[rtc.TranscriptionSegment | None]):
         while True:
             seg = await q.get()
             if seg is None:
                 break
@@ -250,73 +206,61 @@
             # sentence data
             seg_id = (
                 _utils.segment_uuid()
             )  # put each sentence in a different transcription segment
             words = self._opts.word_tokenizer.tokenize(text=tokenized_sentence)
             processed_words = []
 
-            text = ""
             for word in words:
                 word_hyphenes = len(self._opts.hyphenate_word(word))
                 processed_words.append(word)
 
-                # elapsed time since the start of the seg
-                elapsed_time = time.time() - start_time
+                elapsed_time = (
+                    time.time() - start_time
+                )  # elapsed time since the start of the seg
                 text = self._opts.word_tokenizer.format_words(processed_words)
 
                 delay = 0
                 if seg.avg_speed is not None:
-                    estimated_pauses_s = (
-                        seg.sentence_count * self._opts.new_sentence_delay
-                    )
-                    hyph_pauses = estimated_pauses_s * seg.avg_speed
-
                     target_hyphenes = round(seg.avg_speed * elapsed_time)
-                    dt = target_hyphenes - seg.processed_hyphenes - hyph_pauses
+                    dt = target_hyphenes - seg.processed_hyphenes
                     to_wait_hyphenes = max(0, word_hyphenes - dt)
                     delay = to_wait_hyphenes / seg.avg_speed
                 else:
                     delay = word_hyphenes / self._opts.speed
 
-                halfdelay = delay / 2
-                await asyncio.sleep(halfdelay)
+                await asyncio.sleep(delay)
+
+                seg.processed_hyphenes += word_hyphenes
                 q.put_nowait(
                     rtc.TranscriptionSegment(
                         id=seg_id,
                         text=text,
                         start_time=0,
                         end_time=0,
                         final=False,
                     )
                 )
-                await asyncio.sleep(halfdelay)
-                seg.processed_hyphenes += word_hyphenes
 
             q.put_nowait(
                 rtc.TranscriptionSegment(
                     id=seg_id,
                     text=tokenized_sentence,
                     start_time=0,
                     end_time=0,
                     final=True,
                 )
             )
 
-            await asyncio.sleep(self._opts.new_sentence_delay)
-            seg.sentence_count += 1
-
         while True:
             audio_seg = await self._seg_queue.get()
             if audio_seg is None:
                 break
 
-            try:
-                await audio_seg.ready_future
-            except asyncio.CancelledError:
-                continue
+            await audio_seg.first_frame_future
 
             if not self._opts.auto_playout:
                 _ = await self._validated_playout_q.get()
 
             start_time = time.time()
             sentence_stream = audio_seg.sentence_stream
 
@@ -328,15 +272,10 @@
 
         q.put_nowait(None)
 
     def _calc_hyphenes(self, text: str) -> list[str]:
         hyphenes = []
         words = self._opts.word_tokenizer.tokenize(text=text)
         for word in words:
-            new = self._opts.hyphenate_word(word)
-            hyphenes.extend(new)
+            hyphenes.extend(self._opts.hyphenate_word(word))
 
         return hyphenes
-
-    def _log_debug(self, msg: str, **kwargs) -> None:
-        if self._opts.debug:
-            logger.debug(msg, **kwargs)
```

### Comparing `livekit_agents-0.7.0/livekit/agents/tts/tts.py` & `livekit_agents-0.7.dev0/livekit/agents/tts/tts.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/utils/event_emitter.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/event_emitter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/utils/exp_filter.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/exp_filter.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/utils/http_context.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/http_context.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/utils/misc.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/misc.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/utils/moving_average.py` & `livekit_agents-0.7.dev0/livekit/agents/utils/moving_average.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/vad.py` & `livekit_agents-0.7.dev0/livekit/agents/vad.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit/agents/version.py` & `livekit_agents-0.7.dev0/livekit/agents/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.7.0"
+__version__ = "0.7.dev0"
```

### Comparing `livekit_agents-0.7.0/livekit/agents/voice_assistant/assistant.py` & `livekit_agents-0.7.dev0/livekit/agents/voice_assistant/assistant.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,14 @@
 
 @define(kw_only=True, frozen=True)
 class _AssistantOptions:
     plotting: bool
     debug: bool
     allow_interruptions: bool
     int_speech_duration: float
-    # some STT doesn't support streaming (e.g Whisper)
-    # so it doesn't make sense to wait for a certain amount of words
-    # before interrupting the speech. we should set this to 0 in that case
     int_min_words: int
     base_volume: float
     transcription: bool
     word_tokenizer: tokenize.WordTokenizer
     sentence_tokenizer: tokenize.SentenceTokenizer
     hyphenate_word: Callable[[str], list[str]]
     transcription_speed: float
@@ -99,36 +96,40 @@
     "agent_speech_interrupted",
     "function_calls_collected",
     "function_calls_finished",
 ]
 
 
 class VoiceAssistant(utils.EventEmitter[EventTypes]):
+    _SAY_CUSTOM_PRIORITY = 3
+    _SAY_AGENT_ANSWER_PRIORITY = 2
+    _SAY_CALL_CONTEXT_PRIORITY = 1
+
     def __init__(
         self,
         *,
         vad: avad.VAD,
         stt: astt.STT,
         llm: allm.LLM,
         tts: atts.TTS,
         chat_ctx: allm.ChatContext | None = None,
         fnc_ctx: allm.FunctionContext | None = None,
         allow_interruptions: bool = True,
         interrupt_volume: float = 0.05,
-        interrupt_speech_duration: float = 0.65,
+        interrupt_speech_duration: float = 0.7,
         interrupt_min_words: int = 3,
         base_volume: float = 1.0,
         debug: bool = False,
         plotting: bool = False,
         loop: asyncio.AbstractEventLoop | None = None,
         transcription: bool = True,
         sentence_tokenizer: tokenize.SentenceTokenizer = tokenize.basic.SentenceTokenizer(),
         word_tokenizer: tokenize.WordTokenizer = tokenize.basic.WordTokenizer(),
         hyphenate_word: Callable[[str], list[str]] = tokenize.basic.hyphenate_word,
-        transcription_speed: float = 3.83,
+        transcription_speed: float = 4,
     ) -> None:
         super().__init__()
         self._loop = loop or asyncio.get_event_loop()
         self._opts = _AssistantOptions(
             plotting=plotting,
             debug=debug,
             allow_interruptions=allow_interruptions,
@@ -147,16 +148,14 @@
         self._speaking, self._user_speaking = False, False
         self._plotter = plotter.AssistantPlotter(self._loop)
 
         self._audio_source, self._audio_stream = None, None
         self._closed, self._started, self._ready = False, False, False
         self._linked_participant = ""
 
-        self._pending_validation = False
-
         # tasks
         self._launch_task: asyncio.Task | None = None
         self._recognize_task: asyncio.Task | None = None
         self._update_task: asyncio.Task | None = None
         self._play_task: asyncio.Task | None = None
         self._tasks = set[asyncio.Task]()
 
@@ -164,21 +163,24 @@
         self._maybe_answer_task: asyncio.Task | None = None
         self._playing_speech: _SpeechData | None = None
         self._answer_speech: _SpeechData | None = None
         self._playout_start_time: float | None = None
 
         # synthesis state
         self._speech_playing: _SpeechData | None = None  # validated and playing speech
+        self._speech_queue = asyncio.PriorityQueue[_SpeechData]()
         self._user_speaking, self._agent_speaking = False, False
 
         self._target_volume = self._opts.base_volume
         self._vol_filter = utils.ExpFilter(0.9, max_val=self._opts.base_volume)
         self._vol_filter.apply(1.0, self._opts.base_volume)
         self._speech_prob = 0.0
-        self._last_speech_prob = 0.0
+        self._speaking_avg = utils.MovingAverage(
+            int(self._opts.int_speech_duration * 100)
+        )
         self._transcripted_text, self._interim_text = "", ""
         self._start_future = asyncio.Future()
 
     def on(self, event: EventTypes, callback: Callable | None = None) -> Callable:
         """Register a callback for an event
 
         Args:
@@ -203,20 +205,30 @@
     @property
     def started(self) -> bool:
         return self._started
 
     async def say(
         self,
         source: str | allm.LLMStream | AsyncIterable[str],
-        *,
         allow_interruptions: bool = True,
         add_to_ctx: bool = True,
+        force_stream: bool = False,  # force the usage of TTS stream
+        enqueue: bool = True,
     ) -> None:
         with contextlib.suppress(asyncio.CancelledError):
-            await self._start_future
+            if not self._started:
+                await self._start_future
+
+        if isinstance(source, str) and force_stream:
+            text = source
+
+            async def _gen():
+                yield text
+
+            source = _gen()
 
         data = _SpeechData(
             source=source,
             allow_interruptions=allow_interruptions,
             add_to_ctx=add_to_ctx,
             val_ch=aio.Chan[None](),
         )
@@ -396,22 +408,26 @@
         self._audio_stream = audio_stream
         self._ready = True
         self._recognize_task = asyncio.create_task(self._recognize_loop())
 
     def _recv_final_transcript(self, ev: astt.SpeechEvent):
         self._log_debug(f"assistant - received transcript {ev.alternatives[0].text}")
         self._transcripted_text += ev.alternatives[0].text
+        self._interrupt_if_needed()
         self._maybe_answer(self._transcripted_text)
 
     def _recv_interim_transcript(self, ev: astt.SpeechEvent):
         self._interim_text = ev.alternatives[0].text
+        self._interrupt_if_needed()
 
     def _transcript_finished(self, ev: astt.SpeechEvent):
         self._log_debug("assistant - transcript finished")
-        self._pending_validation = True
+        self._transcripted_text = self._interim_text = ""
+        self._interrupt_if_needed()
+        self._validate_answer_if_needed()
 
     def _did_vad_inference(self, ev: avad.VADEvent):
         self._plotter.plot_value("vad_raw", ev.raw_inference_prob)
         self._plotter.plot_value("vad_smoothed", ev.probability)
         self._plotter.plot_value("vad_dur", ev.inference_duration * 1000)
         self._speech_prob = ev.raw_inference_prob
 
@@ -420,15 +436,16 @@
         self._plotter.plot_event("user_started_speaking")
         self._user_speaking = True
         self.emit("user_started_speaking")
 
     def _user_stopped_speaking(self, speech_duration: float):
         self._log_debug(f"assistant - user stopped speaking {speech_duration:.2f}s")
         self._plotter.plot_event("user_started_speaking")
-        self._pending_validation = True
+        self._interrupt_if_needed()
+        self._validate_answer_if_needed()
         self._user_speaking = False
         self.emit("user_stopped_speaking")
 
     def _agent_started_speaking(self):
         self._log_debug("assistant - agent started speaking")
         self._plotter.plot_event("agent_started_speaking")
         self._agent_speaking = True
@@ -481,103 +498,94 @@
                     elif stt_event.type == astt.SpeechEventType.INTERIM_TRANSCRIPT:
                         self._recv_interim_transcript(stt_event)
                     elif stt_event.type == astt.SpeechEventType.END_OF_SPEECH:
                         self._transcript_finished(stt_event)
         except Exception:
             logger.exception("error in recognize loop")
         finally:
-            await asyncio.gather(
-                stt_forwarder.aclose(wait=False),
-                stt_stream.aclose(wait=False),
-                vad_stream.aclose(wait=False),
-                select.aclose(),
-            )
+            await stt_forwarder.aclose(wait=False)
+            await stt_stream.aclose(wait=False)
+            await vad_stream.aclose(wait=False)
+            await select.aclose()
 
     async def _update_loop(self):
-        """Update the volume every 10ms based on the speech probability, decide whether to interrupt
-        and when to validate an answer"""
-        speech_prob_avg = utils.MovingAverage(100)
-        speaking_avg_validation = utils.MovingAverage(210)
-        interruption_speaking_avg = utils.MovingAverage(
-            int(self._opts.int_speech_duration * 100)
-        )
+        """Update the volume every 10ms based on the speech probability"""
+        speech_prob_avg = utils.MovingAverage(100)  # avg over 1s
 
-        interval_10ms = aio.interval(0.01)
-
-        vad_pw = 2.4  # TODO(theomonnom): should this be exposed?
+        vad_pw = 2.4  # should this be exposed
         while not self._closed:
-            await interval_10ms.tick()
-
-            speech_prob_avg.add_sample(self._speech_prob)
-            speaking_avg_validation.add_sample(int(self._user_speaking))
-            interruption_speaking_avg.add_sample(int(self._user_speaking))
-
             bvol = self._opts.base_volume
+
+            self._speaking_avg.add_sample(int(self._user_speaking))
+            speech_prob_avg.add_sample(
+                self._speech_prob
+            )  # not totally accurate due to timing between vad inference and this task
             self._target_volume = max(0, 1 - speech_prob_avg.get_avg() * vad_pw) * bvol
 
             if self._playing_speech:
                 if not self._playing_speech.allow_interruptions:
                     # avoid volume to go to 0 even if speech probability is high
                     self._target_volume = max(self._target_volume, bvol * 0.5)
 
                 if self._playing_speech.interrupted:
                     # the current speech is interrupted, target volume should be 0
                     self._target_volume = 0
 
             if self._user_speaking:
-                if (
-                    interruption_speaking_avg.get_avg() >= 0.1
-                ):  # allow 10% of "noise"/false positives in the VAD?
-                    self._interrupt_if_needed()
-            elif self._pending_validation:
-                if speaking_avg_validation.get_avg() <= 0.05:
-                    self._pending_validation = False
-                    self._validate_answer_if_needed()
+                self._interrupt_if_needed()
 
             if self._opts.plotting:
                 self._plotter.plot_value("raw_t_vol", self._target_volume)
                 self._plotter.plot_value("vol", self._vol_filter.filtered())
 
+            await asyncio.sleep(0.01)
+
     def _interrupt_if_needed(self):
         """Check whether the current speech should be interrupted"""
         if (
             not self._playing_speech
             or not self._opts.allow_interruptions
             or self._playing_speech.interrupted
         ):
             return
 
+        if (
+            self._speaking_avg.get_avg() < 0.9
+        ):  # allow 10% of "noise"/false positives in the VAD?
+            return
+
         if self._opts.int_min_words != 0:
+            # some STT doesn't support streaming (e.g Whisper)
+            # so it doesn't make sense to wait for a certain amount of words
+            # before interrupting the speech
             txt = self._transcripted_text.strip().split()
             if len(txt) <= self._opts.int_min_words:
                 txt = self._interim_text.strip().split()
                 if len(txt) <= self._opts.int_min_words:
                     return
 
         if (
             self._playout_start_time is not None
-            and (time.time() - self._playout_start_time) < 1
-        ):  # don't interrupt new speech (if they're not older than 1s)
+            and (time.time() - self._playout_start_time) < 0.5
+        ):  # don't interrupt new speech (if they're not older than 0.5s)
             return
 
         self._log_debug("assistant - interrupting speech")
         self._playing_speech.interrupted = True
-        self._validate_answer_if_needed()
 
     def _validate_answer_if_needed(self):
         if self._answer_speech is None:
             return
 
         if self._agent_speaking and (
             self._playing_speech and not self._playing_speech.interrupted
         ):
             return
 
         self._log_debug("assistant - validating answer")
-        self._transcripted_text = self._interim_text = ""
         _validate_speech(self._answer_speech)
 
     def _maybe_answer(self, text: str) -> None:
         async def _answer_if_validated(
             ctx: allm.ChatContext, data: _SpeechData
         ) -> None:
             try:
@@ -608,17 +616,14 @@
         self._maybe_answer_task = t
         self._tasks.add(t)
         t.add_done_callback(self._tasks.discard)
 
     async def _start_speech(
         self, data: _SpeechData, *, interrupt_current_if_possible: bool
     ) -> None:
-        with contextlib.suppress(asyncio.CancelledError):
-            await self._start_future
-
         if data.source is None:
             raise ValueError("source must be provided")
 
         # interrupt the current speech if possible, otherwise wait before playing the new speech
         if self._playing_speech is not None:
             assert self._play_task is not None
 
@@ -631,16 +636,14 @@
                 self._playing_speech.interrupted = True
 
             logger.debug("assistant - waiting for current speech to finish")
             await self._play_task
             logger.debug("assistant - current speech finished")
         elif self._play_task is not None:
             self._play_task.cancel()
-            with contextlib.suppress(asyncio.CancelledError):
-                await self._play_task
 
         self._play_task = asyncio.create_task(self._play_speech_if_validated(data))
 
     async def _play_speech_if_validated(self, data: _SpeechData) -> None:
         """
         Start synthesis and playout the speech only if validated
         """
@@ -690,32 +693,30 @@
                 role=allm.ChatRole.ASSISTANT,
             )
 
             if data.add_to_ctx:
                 self._chat_ctx.messages.append(msg)
                 if data.interrupted:
                     self.emit("agent_speech_interrupted", self._chat_ctx, msg)
-                    await tts_forwarder.aclose(wait=False)
                 else:
                     self.emit("agent_speech_committed", self._chat_ctx, msg)
-                    await tts_forwarder.aclose()
 
             self._log_debug(
                 "assistant - playout finished", extra={"interrupted": data.interrupted}
             )
 
         except Exception:
             logger.exception("error while playing speech")
         finally:
             self._playing_speech = None
             with contextlib.suppress(asyncio.CancelledError):
                 _synthesize_task.cancel()
                 await _synthesize_task
 
-            await tts_forwarder.aclose(wait=False)
+            await tts_forwarder.aclose()
             self._log_debug("assistant - play_speech_if_validated finished")
 
     async def _synthesize_task(
         self,
         data: _SpeechData,
         po_tx: aio.ChanSender[rtc.AudioFrame],
         tts_forwarder: transcription.TTSSegmentsForwarder | utils._noop.Nop,
```

### Comparing `livekit_agents-0.7.0/livekit/agents/voice_assistant/plotter.py` & `livekit_agents-0.7.dev0/livekit/agents/voice_assistant/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,40 +23,40 @@
     MSG_ID: ClassVar[int] = 1
 
     which: PlotType = "vad_raw"
     x: float = 0.0
     y: float = 0.0
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.which).to_bytes(4, byteorder="big"))
+        b.write(len(self.which).to_bytes(4))
         b.write(self.which.encode())
         b.write(struct.pack("d", self.x))
         b.write(struct.pack("d", self.y))
 
     def read(self, b: io.BytesIO) -> None:
-        which_len = int.from_bytes(b.read(4), byteorder="big")
+        which_len = int.from_bytes(b.read(4))
         self.which = b.read(which_len).decode()  # type: ignore
         self.x = struct.unpack("d", b.read(8))[0]
         self.y = struct.unpack("d", b.read(8))[0]
 
 
 @define(kw_only=True)
 class PlotEventMessage:
     MSG_ID: ClassVar[int] = 2
 
     which: EventType = "user_started_speaking"
     x: float = 0.0
 
     def write(self, b: io.BytesIO) -> None:
-        b.write(len(self.which).to_bytes(4, byteorder="big"))
+        b.write(len(self.which).to_bytes(4))
         b.write(self.which.encode())
         b.write(struct.pack("d", self.x))
 
     def read(self, b: io.BytesIO) -> None:
-        which_len = int.from_bytes(b.read(4), byteorder="big")
+        which_len = int.from_bytes(b.read(4))
         self.which = b.read(which_len).decode()  # type: ignore
         self.x = struct.unpack("d", b.read(8))[0]
 
 
 PLT_MESSAGES: dict = {
     PlotMessage.MSG_ID: PlotMessage,
     PlotEventMessage.MSG_ID: PlotEventMessage,
```

### Comparing `livekit_agents-0.7.0/livekit/agents/worker.py` & `livekit_agents-0.7.dev0/livekit/agents/worker.py`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/livekit_agents.egg-info/PKG-INFO` & `livekit_agents-0.7.dev0/livekit_agents.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-agents
-Version: 0.7.0
+Version: 0.7.dev0
 Summary: LiveKit Python Agents
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,agents,AI
```

### Comparing `livekit_agents-0.7.0/livekit_agents.egg-info/SOURCES.txt` & `livekit_agents-0.7.dev0/livekit_agents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `livekit_agents-0.7.0/setup.py` & `livekit_agents-0.7.dev0/setup.py`

 * *Files identical despite different names*

