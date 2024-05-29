# Comparing `tmp/gpt_computer_assistant-0.5.5.tar.gz` & `tmp/gpt_computer_assistant-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_computer_assistant-0.5.5.tar", last modified: Wed May 29 10:38:10 2024, max compression
+gzip compressed data, was "gpt_computer_assistant-0.5.6.tar", last modified: Wed May 29 10:41:39 2024, max compression
```

## Comparing `gpt_computer_assistant-0.5.5.tar` & `gpt_computer_assistant-0.5.6.tar`

### file list

```diff
@@ -1,124 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.999216 gpt_computer_assistant-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.987216 gpt_computer_assistant-0.5.5/.git/
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/FETCH_HEAD
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/HEAD
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/config
--rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/description
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.987216 gpt_computer_assistant-0.5.5/.git/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/fsmonitor-watchman.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/post-update.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1649 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-merge-commit.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-push.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/pre-receive.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     2783 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/push-to-checkout.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     2308 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/sendemail-validate.sample
--rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/hooks/update.sample
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/index
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.987216 gpt_computer_assistant-0.5.5/.git/info/
--rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/info/exclude
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.987216 gpt_computer_assistant-0.5.5/.git/logs/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/HEAD
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.git/logs/refs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.987216 gpt_computer_assistant-0.5.5/.git/logs/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.991216 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-different-profiles-mode
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-icon
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-input-box-and-button
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-just-text-mode
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-reset-system
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Added-splitting-long-audios
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/Fixed-high-delay-problem
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/logs/refs/remotes/origin/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.git/objects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.991216 gpt_computer_assistant-0.5.5/.git/objects/pack/
--r--r--r--   0 runner    (1001) docker     (127)     8716 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.idx
--r--r--r--   0 runner    (1001) docker     (127)    60543 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.pack
--r--r--r--   0 runner    (1001) docker     (127)     1144 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.rev
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.git/refs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.991216 gpt_computer_assistant-0.5.5/.git/refs/heads/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/heads/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.git/refs/remotes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.991216 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-different-profiles-mode
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-icon
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-input-box-and-button
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-just-text-mode
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-reset-system
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Added-splitting-long-audios
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/Fixed-high-delay-problem
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/remotes/origin/master
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/.git/refs/tags/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.1.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.1.1
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.1.2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.2.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.3.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.4.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.0
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.1
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.2
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.3
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.4
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.git/refs/tags/v0.5.5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.983216 gpt_computer_assistant-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.github/workflows/deploys.yml
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.github/workflows/release_generation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 10:38:09.999216 gpt_computer_assistant-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/bump.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/background.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/chat_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/proccess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/gpt_computer_assistant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/gui/button.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/gui/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/llm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/screen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/screen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/screen/shot.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.999216 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_16.png
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_24.png
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_256.png
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_32.png
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_48.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:38:09.995216 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4681 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 10:38:09.000000 gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:38:09.999216 gpt_computer_assistant-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 10:38:01.000000 gpt_computer_assistant-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.010893 gpt_computer_assistant-0.5.6/.git/
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/config
+-rwxr-xr-x   0 runner    (1001) docker     (127)       73 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/description
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      478 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      896 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4726 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/fsmonitor-watchman.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      189 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      424 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1649 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      416 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-merge-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1374 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4898 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/pre-receive.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1492 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2783 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/push-to-checkout.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2308 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/sendemail-validate.sample
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3650 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/index
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/info/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      240 2024-05-29 10:41:29.000000 gpt_computer_assistant-0.5.6/.git/info/exclude
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.006893 gpt_computer_assistant-0.5.6/.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.006893 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-different-profiles-mode
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-just-text-mode
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/Fixed-high-delay-problem
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/logs/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.006893 gpt_computer_assistant-0.5.6/.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/objects/pack/
+-r--r--r--   0 runner    (1001) docker     (127)     8996 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.idx
+-r--r--r--   0 runner    (1001) docker     (127)    61456 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.pack
+-r--r--r--   0 runner    (1001) docker     (127)     1184 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.rev
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.010893 gpt_computer_assistant-0.5.6/.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.014893 gpt_computer_assistant-0.5.6/.git/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.006893 gpt_computer_assistant-0.5.6/.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.018894 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-different-profiles-mode
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-icon
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-input-box-and-button
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-just-text-mode
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-reset-system
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Added-splitting-long-audios
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/Fixed-high-delay-problem
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/remotes/origin/master
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.018894 gpt_computer_assistant-0.5.6/.git/refs/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.1.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.1.1
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.1.2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.2.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.3.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.4.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.0
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.1
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.2
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.3
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.4
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.5
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.git/refs/tags/v0.5.6
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.010893 gpt_computer_assistant-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.018894 gpt_computer_assistant-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.github/workflows/deploys.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.github/workflows/release_generation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/bump.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.018894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/chat_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5459 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/proccess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10689 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/gpt_computer_assistant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/gui/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/gui/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/llm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/screen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/screen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/screen/shot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_16.png
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_256.png
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_48.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:41:39.018894 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 10:41:38.000000 gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:41:39.022894 gpt_computer_assistant-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 10:41:30.000000 gpt_computer_assistant-0.5.6/setup.py
```

### Comparing `gpt_computer_assistant-0.5.5/.git/FETCH_HEAD` & `gpt_computer_assistant-0.5.6/.git/FETCH_HEAD`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 c5b97d087ae232f4124b062d8d25f6a699db7adc		branch 'Added-different-profiles-mode' of https://github.com/onuratakan/gpt-computer-assistant
 022602896b15b5f11ad0dae0eaf31ca8b831b4eb		branch 'Added-icon' of https://github.com/onuratakan/gpt-computer-assistant
 f95a6816826e3b6cc5a2909ef8aef549d07a84b0		branch 'Added-input-box-and-button' of https://github.com/onuratakan/gpt-computer-assistant
 6a17387dda1243d1f09a807d5a2050d671e75c67		branch 'Added-just-text-mode' of https://github.com/onuratakan/gpt-computer-assistant
 f78094740a29a0b2e1eca2342d212905402a677e		branch 'Added-reset-system' of https://github.com/onuratakan/gpt-computer-assistant
 ea9dc1adcbee374bf5b901a5f11a3c9737b0518e		branch 'Added-splitting-long-audios' of https://github.com/onuratakan/gpt-computer-assistant
 aa3faf3045dcf6d80fd424b210d02aee0b2476d4		branch 'Fixed-high-delay-problem' of https://github.com/onuratakan/gpt-computer-assistant
-c7f5d1052f93504bff5527db3bb2f4a8619cd566		branch 'master' of https://github.com/onuratakan/gpt-computer-assistant
+06a8461621130428f5d4be2642a37bcb62d7e1c4		branch 'master' of https://github.com/onuratakan/gpt-computer-assistant
 920866c012c25fbbe11d9f162ad26b386402190f		tag 'v0.1.0' of https://github.com/onuratakan/gpt-computer-assistant
 cb203784ebebd5e6885ae69822caa8d8cfaf4ed4		tag 'v0.1.1' of https://github.com/onuratakan/gpt-computer-assistant
 d77bb1033a9d51fb08619c8b63860e57e10a11b1		tag 'v0.1.2' of https://github.com/onuratakan/gpt-computer-assistant
 365d62393dc41c08e483d3c917da0ff85fcaae0f		tag 'v0.2.0' of https://github.com/onuratakan/gpt-computer-assistant
 d967f0e3518a5b57926ed042290d1032c14e2e5a		tag 'v0.3.0' of https://github.com/onuratakan/gpt-computer-assistant
 c7926ae60405f5b243d9b4efee3b601cd7f2626d		tag 'v0.4.0' of https://github.com/onuratakan/gpt-computer-assistant
 c4ceb708ba860a5d0efec7661978e1f48881da70		tag 'v0.5.0' of https://github.com/onuratakan/gpt-computer-assistant
 227564663235da9afcbce78c10bfbcca1f5698ed		tag 'v0.5.1' of https://github.com/onuratakan/gpt-computer-assistant
 a93ff7af535e15fb644a3da6ca21d496bc980e87		tag 'v0.5.2' of https://github.com/onuratakan/gpt-computer-assistant
 aae17c3207063f00265522ea7fcd1ef971cccc85		tag 'v0.5.3' of https://github.com/onuratakan/gpt-computer-assistant
 1723625f6ac0e9fb4a39f5b90d1cef73ac7d53bb		tag 'v0.5.4' of https://github.com/onuratakan/gpt-computer-assistant
 c7f5d1052f93504bff5527db3bb2f4a8619cd566		tag 'v0.5.5' of https://github.com/onuratakan/gpt-computer-assistant
+06a8461621130428f5d4be2642a37bcb62d7e1c4		tag 'v0.5.6' of https://github.com/onuratakan/gpt-computer-assistant
```

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/commit-msg.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/fsmonitor-watchman.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/fsmonitor-watchman.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/pre-commit.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/pre-push.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/pre-rebase.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/pre-receive.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/pre-receive.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/prepare-commit-msg.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/push-to-checkout.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/push-to-checkout.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/sendemail-validate.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/sendemail-validate.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/hooks/update.sample` & `gpt_computer_assistant-0.5.6/.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.idx` & `gpt_computer_assistant-0.5.6/.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.idx`

 * *Files 13% similar despite different names*

```diff
@@ -1,545 +1,563 @@
 00000000: ff74 4f63 0000 0002 0000 0001 0000 0004  .tOc............
 00000010: 0000 0006 0000 0006 0000 0008 0000 0008  ................
-00000020: 0000 0008 0000 000a 0000 000a 0000 000c  ................
-00000030: 0000 000d 0000 000e 0000 0010 0000 0011  ................
-00000040: 0000 0012 0000 0013 0000 0014 0000 0015  ................
-00000050: 0000 0015 0000 0015 0000 0019 0000 0019  ................
-00000060: 0000 001c 0000 001d 0000 001e 0000 001e  ................
-00000070: 0000 001e 0000 001e 0000 0020 0000 0020  ........... ... 
-00000080: 0000 0020 0000 0020 0000 0021 0000 0022  ... ... ...!..."
-00000090: 0000 0023 0000 0024 0000 0024 0000 0026  ...#...$...$...&
-000000a0: 0000 0026 0000 0027 0000 0028 0000 0029  ...&...'...(...)
-000000b0: 0000 002a 0000 002a 0000 002a 0000 002b  ...*...*...*...+
-000000c0: 0000 002b 0000 002b 0000 002b 0000 002d  ...+...+...+...-
-000000d0: 0000 002f 0000 0030 0000 0032 0000 0034  .../...0...2...4
-000000e0: 0000 0036 0000 0036 0000 0038 0000 0039  ...6...6...8...9
-000000f0: 0000 003a 0000 003b 0000 003c 0000 003e  ...:...;...<...>
-00000100: 0000 0042 0000 0045 0000 0046 0000 0046  ...B...E...F...F
-00000110: 0000 0046 0000 0046 0000 0048 0000 004b  ...F...F...H...K
-00000120: 0000 004b 0000 004b 0000 004b 0000 004c  ...K...K...K...L
-00000130: 0000 004c 0000 004c 0000 004f 0000 0052  ...L...L...O...R
-00000140: 0000 0052 0000 0053 0000 0054 0000 0054  ...R...S...T...T
-00000150: 0000 0055 0000 0055 0000 0055 0000 0057  ...U...U...U...W
-00000160: 0000 0057 0000 0057 0000 0058 0000 0058  ...W...W...X...X
-00000170: 0000 0058 0000 005a 0000 005a 0000 005b  ...X...Z...Z...[
-00000180: 0000 005d 0000 0060 0000 0062 0000 0063  ...]...`...b...c
-00000190: 0000 0064 0000 0064 0000 0064 0000 0064  ...d...d...d...d
-000001a0: 0000 0065 0000 0066 0000 0069 0000 0069  ...e...f...i...i
-000001b0: 0000 006a 0000 006a 0000 006b 0000 006e  ...j...j...k...n
-000001c0: 0000 006f 0000 0072 0000 0073 0000 0074  ...o...r...s...t
-000001d0: 0000 0074 0000 0074 0000 0075 0000 0077  ...t...t...u...w
-000001e0: 0000 0078 0000 007a 0000 007b 0000 007c  ...x...z...{...|
-000001f0: 0000 007d 0000 007d 0000 007f 0000 0081  ...}...}........
-00000200: 0000 0083 0000 0083 0000 0085 0000 0087  ................
-00000210: 0000 0088 0000 0088 0000 0089 0000 008a  ................
-00000220: 0000 008d 0000 008d 0000 0090 0000 0091  ................
-00000230: 0000 0091 0000 0091 0000 0091 0000 0092  ................
-00000240: 0000 0092 0000 0094 0000 0094 0000 0095  ................
-00000250: 0000 0097 0000 0097 0000 0097 0000 0098  ................
-00000260: 0000 0099 0000 0099 0000 0099 0000 0099  ................
-00000270: 0000 0099 0000 009b 0000 009c 0000 009d  ................
-00000280: 0000 009e 0000 009e 0000 009f 0000 00a0  ................
-00000290: 0000 00a2 0000 00a3 0000 00a4 0000 00a6  ................
-000002a0: 0000 00a7 0000 00a8 0000 00ab 0000 00ae  ................
-000002b0: 0000 00b2 0000 00b3 0000 00b3 0000 00b4  ................
-000002c0: 0000 00b4 0000 00b5 0000 00b7 0000 00b8  ................
-000002d0: 0000 00b9 0000 00b9 0000 00b9 0000 00ba  ................
-000002e0: 0000 00bc 0000 00be 0000 00c0 0000 00c1  ................
-000002f0: 0000 00c1 0000 00c2 0000 00c4 0000 00c4  ................
-00000300: 0000 00c6 0000 00c7 0000 00c7 0000 00c8  ................
-00000310: 0000 00ca 0000 00ca 0000 00cc 0000 00cd  ................
-00000320: 0000 00ce 0000 00d1 0000 00d3 0000 00d4  ................
-00000330: 0000 00d5 0000 00d6 0000 00d7 0000 00d8  ................
-00000340: 0000 00d8 0000 00da 0000 00da 0000 00da  ................
-00000350: 0000 00dd 0000 00de 0000 00de 0000 00df  ................
-00000360: 0000 00df 0000 00e0 0000 00e0 0000 00e1  ................
-00000370: 0000 00e2 0000 00e4 0000 00e4 0000 00e6  ................
-00000380: 0000 00eb 0000 00eb 0000 00ef 0000 00f1  ................
-00000390: 0000 00f3 0000 00f3 0000 00f5 0000 00f6  ................
-000003a0: 0000 00f9 0000 00fb 0000 00fc 0000 00fe  ................
-000003b0: 0000 00ff 0000 0100 0000 0100 0000 0101  ................
-000003c0: 0000 0101 0000 0102 0000 0102 0000 0103  ................
-000003d0: 0000 0104 0000 0105 0000 0106 0000 0106  ................
-000003e0: 0000 0108 0000 0109 0000 010a 0000 010c  ................
-000003f0: 0000 010c 0000 010e 0000 0110 0000 0110  ................
-00000400: 0000 0111 0000 0111 00dd d47f dfd7 1a8b  ................
+00000020: 0000 0009 0000 000b 0000 000b 0000 000d  ................
+00000030: 0000 000e 0000 000f 0000 0011 0000 0012  ................
+00000040: 0000 0013 0000 0014 0000 0015 0000 0016  ................
+00000050: 0000 0016 0000 0016 0000 001a 0000 001a  ................
+00000060: 0000 001d 0000 001e 0000 0020 0000 0020  ........... ... 
+00000070: 0000 0021 0000 0021 0000 0023 0000 0024  ...!...!...#...$
+00000080: 0000 0024 0000 0024 0000 0025 0000 0026  ...$...$...%...&
+00000090: 0000 0027 0000 0028 0000 0028 0000 002a  ...'...(...(...*
+000000a0: 0000 002a 0000 002b 0000 002c 0000 002e  ...*...+...,....
+000000b0: 0000 002f 0000 002f 0000 002f 0000 0030  .../.../.../...0
+000000c0: 0000 0030 0000 0030 0000 0030 0000 0032  ...0...0...0...2
+000000d0: 0000 0034 0000 0035 0000 0037 0000 0039  ...4...5...7...9
+000000e0: 0000 003b 0000 003b 0000 003d 0000 003e  ...;...;...=...>
+000000f0: 0000 003f 0000 0040 0000 0041 0000 0043  ...?...@...A...C
+00000100: 0000 0047 0000 004a 0000 004b 0000 004b  ...G...J...K...K
+00000110: 0000 004c 0000 004c 0000 004e 0000 0051  ...L...L...N...Q
+00000120: 0000 0051 0000 0051 0000 0051 0000 0052  ...Q...Q...Q...R
+00000130: 0000 0052 0000 0052 0000 0055 0000 0058  ...R...R...U...X
+00000140: 0000 0058 0000 0059 0000 005a 0000 005a  ...X...Y...Z...Z
+00000150: 0000 005b 0000 005b 0000 005b 0000 005d  ...[...[...[...]
+00000160: 0000 005d 0000 005d 0000 005e 0000 005e  ...]...]...^...^
+00000170: 0000 005e 0000 0060 0000 0060 0000 0061  ...^...`...`...a
+00000180: 0000 0063 0000 0066 0000 0068 0000 0069  ...c...f...h...i
+00000190: 0000 006a 0000 006a 0000 006a 0000 006a  ...j...j...j...j
+000001a0: 0000 006b 0000 006c 0000 006f 0000 006f  ...k...l...o...o
+000001b0: 0000 0070 0000 0070 0000 0071 0000 0074  ...p...p...q...t
+000001c0: 0000 0075 0000 0078 0000 0079 0000 007a  ...u...x...y...z
+000001d0: 0000 007a 0000 007a 0000 007b 0000 007d  ...z...z...{...}
+000001e0: 0000 007e 0000 0080 0000 0081 0000 0082  ...~............
+000001f0: 0000 0083 0000 0083 0000 0085 0000 0087  ................
+00000200: 0000 0089 0000 0089 0000 008b 0000 008d  ................
+00000210: 0000 008e 0000 008e 0000 008f 0000 0090  ................
+00000220: 0000 0093 0000 0093 0000 0096 0000 0097  ................
+00000230: 0000 0097 0000 0097 0000 0097 0000 0098  ................
+00000240: 0000 0098 0000 009a 0000 009a 0000 009b  ................
+00000250: 0000 009d 0000 009d 0000 009d 0000 009e  ................
+00000260: 0000 009f 0000 009f 0000 009f 0000 009f  ................
+00000270: 0000 009f 0000 00a1 0000 00a2 0000 00a3  ................
+00000280: 0000 00a4 0000 00a4 0000 00a5 0000 00a6  ................
+00000290: 0000 00a8 0000 00a9 0000 00aa 0000 00ac  ................
+000002a0: 0000 00ad 0000 00ae 0000 00b1 0000 00b4  ................
+000002b0: 0000 00b8 0000 00b9 0000 00b9 0000 00ba  ................
+000002c0: 0000 00ba 0000 00bb 0000 00bd 0000 00be  ................
+000002d0: 0000 00bf 0000 00bf 0000 00bf 0000 00c0  ................
+000002e0: 0000 00c2 0000 00c4 0000 00c6 0000 00c7  ................
+000002f0: 0000 00c7 0000 00c8 0000 00ca 0000 00ca  ................
+00000300: 0000 00cc 0000 00cd 0000 00cd 0000 00ce  ................
+00000310: 0000 00d0 0000 00d0 0000 00d2 0000 00d3  ................
+00000320: 0000 00d4 0000 00d7 0000 00d9 0000 00da  ................
+00000330: 0000 00db 0000 00dc 0000 00dd 0000 00de  ................
+00000340: 0000 00de 0000 00e0 0000 00e0 0000 00e0  ................
+00000350: 0000 00e3 0000 00e4 0000 00e4 0000 00e5  ................
+00000360: 0000 00e6 0000 00e7 0000 00e7 0000 00e8  ................
+00000370: 0000 00e9 0000 00eb 0000 00eb 0000 00ed  ................
+00000380: 0000 00f2 0000 00f2 0000 00f6 0000 00f8  ................
+00000390: 0000 00fa 0000 00fa 0000 00fc 0000 00fd  ................
+000003a0: 0000 0100 0000 0102 0000 0104 0000 0106  ................
+000003b0: 0000 0107 0000 0108 0000 0108 0000 010a  ................
+000003c0: 0000 010a 0000 010b 0000 010b 0000 010c  ................
+000003d0: 0000 010d 0000 010e 0000 010f 0000 010f  ................
+000003e0: 0000 0111 0000 0112 0000 0113 0000 0116  ................
+000003f0: 0000 0116 0000 0118 0000 011a 0000 011a  ................
+00000400: 0000 011b 0000 011b 00dd d47f dfd7 1a8b  ................
 00000410: b29c 7c1e ba49 3daf 4967 93c2 0180 f89b  ..|..I=.Ig......
 00000420: e496 a0ae 013b ee5a d694 b83e 83ae fde6  .....;.Z...>....
 00000430: 01cb 31ed 14ca 49cd a7c6 7b2d dc79 6a89  ..1...I...{-.yj.
 00000440: 8f88 45d4 01f5 0b52 87ff b115 4de5 4f1d  ..E....R....M.O.
 00000450: ba3f 07ae 6cbd 1e89 0226 0289 6b15 b5f1  .?..l....&..k...
 00000460: 1ad0 dae0 eaf3 1ca8 b831 b4eb 02e2 e3ff  .........1......
 00000470: 9b9a b5a5 646b 8d52 d2fc c1c5 ab6c cffa  ....dk.R.....l..
 00000480: 0488 e2c8 7683 914c 32de aaa8 667e 7497  ....v..L2...f~t.
 00000490: f76a 04d8 04c7 bfac c732 846e 5d1e 459d  .j.......2.n].E.
-000004a0: 18b3 1b08 07e3 db6e 0725 883b 4fee 1fed  .......n.%.;O...
-000004b0: 28e6 bc64 a993 11c9 4684 0053 076b 11c0  (..d....F..S.k..
-000004c0: 012f 9e04 a9d5 4016 1c16 ecb5 0bce f460  ./....@........`
-000004d0: 09a6 8b4b bcdd f77d 7431 7fd9 e224 50d8  ...K...}t1...$P.
-000004e0: c445 607e 09f4 9f7d 68f4 2b0f 750e 2aba  .E`~...}h.+.u.*.
-000004f0: 9acb 1daa c79d 50c9 0aac 1694 4d6b 28c7  ......P.....Mk(.
-00000500: fc05 9944 50df 60a7 6888 f41f 0b34 c374  ...DP.`.h....4.t
-00000510: 78ab 675c 6ad3 9730 ccf9 8af1 88e7 0ff9  x.g\j..0........
-00000520: 0c2e 2a86 e7d7 efbf 512b cf6b 85cf 6a38  ..*.....Q+.k..j8
-00000530: a898 0019 0c91 98ac ccb3 d1ad d56b 4496  .............kD.
-00000540: e591 fa18 cbaf 64fc 0d82 432f c2d9 3143  ......d...C/..1C
-00000550: d515 42d0 f4ed 03b6 3bff 69a2 0ea0 e38a  ..B.....;.i.....
-00000560: 01b8 958f fbcf 297a a773 effe 3623 34d0  ......)z.s..6#4.
-00000570: 0fee 61e9 f377 8410 9916 ff54 035f 13f5  ..a..w.....T._..
-00000580: 14df 8360 1025 1521 c1c9 9f77 238b 4860  ...`.%.!...w#.H`
-00000590: 3be0 42ba 5823 a198 1129 d93b 10cf ecb6  ;.B.X#...).;....
-000005a0: 235a 9e7f 4ab5 3cc7 24ed 056c 1427 6e10  #Z..J.<.$..l.'n.
-000005b0: d8a0 d752 dc35 3a7c d10a 253b c579 379a  ...R.5:|..%;.y7.
-000005c0: 1433 ce41 50bb b18b f7b3 c2d6 c4b8 9b32  .3.AP..........2
-000005d0: 084c 1e7d 146c addd 63f0 e9df a465 4491  .L.}.l..c....eD.
-000005e0: 1313 6c6e 330e 20cd 149b 0c8c 5257 8dc6  ..ln3. .....RW..
-000005f0: 3594 ea2a 36cb 3cfd 7feb 0b17 165c 1d7d  5..*6.<......\.}
-00000600: e49a 08aa f59e d43a c2a9 ba68 b811 30e8  .......:...h..0.
-00000610: 1666 45c6 e558 e949 854d 6828 6bf7 a958  .fE..X.I.Mh(k..X
-00000620: 2a47 a2a0 16f3 c37c 7b5d 4e84 c784 5968  *G.....|{]N...Yh
-00000630: 05df 80c6 acbf 1568 1723 625f 6ac0 e9fb  .......h.#b_j...
-00000640: 4a39 f5b9 0d1c ef73 ac7d 53bb 18b4 e9fc  J9.....s.}S.....
-00000650: ef00 0284 d53a 8288 d7e2 7c5e 3564 58cc  .....:....|^5dX.
-00000660: 1cf3 c9c3 075c 1fab a1eb d396 5764 e2ec  .....\......Wd..
-00000670: af17 751b 1cf4 502a 6173 de16 a0db 5cd2  ..u...P*as....\.
-00000680: e32b 2cd8 0f07 83d0 2044 d5a0 9f55 22b9  .+,..... D...U".
-00000690: 616b 252c 0891 a6e8 aa7b ca64 2175 1d36  ak%,.....{.d!u.6
-000006a0: f8f1 7ce9 6aaf c278 22e2 0b6f c35e 999d  ..|.j..x"..o.^..
-000006b0: 2275 6466 3235 da9a fcbc e78c 10bf bcca  "udf25..........
-000006c0: 1f56 98ed 2302 d30b 1108 da08 5d35 9b7b  .V..#.......]5.{
-000006d0: 0054 2e6d 1846 0766 2559 1dca 5a32 c357  .T.m.F.f%Y..Z2.W
-000006e0: c6e7 d67c 9d88 fdf9 9e57 2191 25f2 e150  ...|.....W!.%..P
-000006f0: 2c69 b4cf 1669 971b 9616 8399 2ca6 6ba4  ,i...i......,.k.
-00000700: 27d5 b1bf 06a5 daa9 29cb 20bf d4a1 6010  '.......). ...`.
-00000710: 7e6c 8063 284d 716a b3c7 2c7c 1ec5 1fa5  ~l.c(Mqj..,|....
-00000720: 23db e011 09f2 320a 29d2 daac 5904 9917  #.....2.)...Y...
-00000730: 2e55 4126 d72d 43d3 0ed5 a046 2a42 2fef  .UA&.-C....F*B/.
-00000740: b908 c755 9dd2 f716 8efc 378b 8785 ba62  ...U......7....b
-00000750: 2df2 9c70 5bc4 7bc7 c268 e8c4 92b6 458e  -..p[.{..h....E.
-00000760: 3b67 b03b 31ce d298 ccae 493b e277 6bdb  ;g.;1.....I;.wk.
-00000770: 7184 b4e3 6003 36da 31d7 7150 caee 8e4d  q...`.6.1.qP...M
-00000780: ec78 f304 09f4 fe0d eab6 11c1 32d8 331c  .x..........2.3.
-00000790: 3e6f 336e df84 ee6e 954e 0e72 1de3 a1a4  >o3n...n.N.r....
-000007a0: 32e8 3d4f cefa 3337 032a 8247 709f 7b53  2.=O..37.*.Gp.{S
-000007b0: 03b1 32e9 3370 fbd1 c498 f950 017e df7e  ..2.3p.....P.~.~
-000007c0: 2c97 7834 a9df 0ff3 34c0 bb3d 74e1 47d3  ,.x4....4..=t.G.
-000007d0: c9f2 0418 c0f5 1abb 06a4 6efd 34fc f02c  ..........n.4..,
-000007e0: f342 4990 f69a a8e4 f751 2b31 0cb5 15aa  .BI......Q+1....
-000007f0: 355a e6e3 9381 137f 02e6 af0d a71f d969  5Z.............i
-00000800: 2974 9429 35a8 559d 8e8f 8390 86cb bd78  )t.)5.U........x
-00000810: 32a5 9c0d df0e 5bf6 360c ff80 3fc6 5590  2.....[.6...?.U.
-00000820: e0d0 27f9 a255 de67 569f 098d 365d 6239  ..'..U.gV...6]b9
-00000830: 3dc4 1c08 e483 d3c9 17da 0ff8 5fca ae0f  =..........._...
-00000840: 3850 1419 135d df9b 36fa d8bd 2e4f 612b  8P...]..6....Oa+
-00000850: 5be2 e775 3894 9563 e601 a524 7c22 e6bd  [..u8..c...$|"..
-00000860: 1f6e ad7d f98e 0a8d 3911 2369 cdb9 958c  .n.}....9.#i....
-00000870: 956f e5bc a73f 34f7 4d75 2891 3a7c 49fa  .o...?4.Mu(.:|I.
-00000880: 26f4 32f2 91f4 f49b 21b4 804c 0f5b 1178  &.2.....!..L.[.x
-00000890: 3baf b2ce f39b 0d2d 3b2d ff8a 301d 54b1  ;......-;-..0.T.
-000008a0: c839 2969 3c0a b25e 76cc 5ed1 1c73 b8fe  .9)i<..^v.^..s..
-000008b0: a7aa 5496 ebad a7ce 3de3 3dde ee30 fce9  ..T.....=.=..0..
-000008c0: 17ab 3a10 b9cb 365b 625b 9fea 3def 1c80  ..:...6[b[..=...
-000008d0: d6b0 cdbc 7ded 1060 4a95 aad6 62ce bb4c  ....}..`J...b..L
-000008e0: 3e52 8de3 bf3e 0e9d eed6 d86d 0033 89b7  >R...>.....m.3..
-000008f0: cb85 84a3 3e5f 999b 65e4 d565 2911 1ad1  ....>_..e..e)...
-00000900: 92bf c6de 425c af47 3e69 9a2f a996 ddb0  ....B\.G>i./....
-00000910: f8b3 f6e1 4432 2091 56f0 2438 3eb7 bc56  ....D2 .V.$8>..V
-00000920: e4df 97de 4168 f673 d2ad 0c87 934a 3c44  ....Ah.s.....J<D
-00000930: 3f05 0000 f2c4 5598 557b 2475 49b2 73d1  ?.....U.U{$uI.s.
-00000940: 1881 f3df 3f0c 6fb8 2eb9 cfd9 0542 a8dc  ....?.o......B..
-00000950: 2572 f632 97e5 f65d 3ff6 be70 55a7 961c  %r.2...]?..pU...
-00000960: d77e 3ebf c323 2730 223b 51c3 40e6 0d18  .~>..#'0";Q.@...
-00000970: 6d78 d3e8 53df cf06 77ac 1884 8e9f 8e58  mx..S...w......X
-00000980: 4471 35ed 9af9 bf37 13da 009f 3875 d0bb  Dq5....7....8u..
-00000990: 3a2a 9b74 4477 b3e9 5a6c 3a22 d991 37b0  :*.tDw..Zl:"..7.
-000009a0: 0859 53a8 7d7f fe9a 4508 ca52 16d7 d238  .YS.}...E..R...8
-000009b0: 30a7 d1ec 0df7 8aa2 6e33 cb40 456b 4288  0.......n3.@EkB.
-000009c0: e355 ea73 6090 7fee 092b b823 35e8 8f80  .U.s`....+.#5...
-000009d0: 4580 739d a623 49c6 a495 ff9f c82f 8c61  E.s..#I....../.a
-000009e0: 61d3 7161 49cd 9536 f437 89ff c916 0caa  a.qaI..6.7......
-000009f0: df9a 10e4 3dee 51f4 4c06 bf6b 863b e410  ....=.Q.L..k.;..
-00000a00: bac2 8981 a2a3 8726 fc6c 0f08 4c76 5c8e  .......&.l..Lv\.
-00000a10: 185b a58b 2940 0aa0 4159 3efb b06c b0f5  .[..)@..AY>..l..
-00000a20: 4cf1 a726 2bc2 065d 939f d8ae 1261 957e  L..&+..].....a.~
-00000a30: 48fb ea8b 4d72 18da aa31 ae06 9d5d 620a  H...Mr...1...]b.
-00000a40: 13c0 bbac 435b 4cbb 4da8 26bd a9a8 9d63  ....C[L.M.&....c
-00000a50: e26d 45d1 a21c 3f63 7b19 a972 4dd6 6e60  .mE...?c{..rM.n`
-00000a60: 7078 e4a1 3333 8a1c 03a6 d316 083d b588  px..33.......=..
-00000a70: 4fad 480f 0c74 0a54 d524 976a cde9 3369  O.H..t.T.$.j..3i
-00000a80: 3350 4ff7 50aa 047f d1f7 7bac ba02 28d0  3PO.P.....{...(.
-00000a90: d3e7 a8b3 42cb 24ec 5217 9473 2a87 4182  ....B.$.R..s*.A.
-00000aa0: d35a d847 eca2 dd45 d091 d351 5550 24f2  .Z.G...E...QUP$.
-00000ab0: 3d09 12c9 af2c 1ea3 8653 3abb 2609 efb9  =....,...S:.&...
-00000ac0: 5569 91ac f0e9 2153 612e 4b34 ac5f 4290  Ui....!Sa.K4._B.
-00000ad0: 43e1 1c53 58ff 10c2 6e80 dcd2 39c1 c1ef  C..SX...n...9...
-00000ae0: 2758 9904 8e15 56d7 5b11 9f7b bc8c 6940  'X....V.[..{..i@
-00000af0: 091b 70d3 0c1e a19c 3ae4 e1dc 5b8b 005f  ..p.....:...[.._
-00000b00: aff9 ea30 8819 4373 0a5f 392f 20d5 bcca  ...0..Cs._9/ ...
-00000b10: 5dd1 ad3c aa9a 991f e496 20a4 421e 7c98  ]..<...... .B.|.
-00000b20: a062 9eb7 5e88 5b0b d90d a8c0 3367 3c2d  .b..^.[.....3g<-
-00000b30: fce1 34ed 7504 b2c9 5e97 43b2 7f36 b434  ..4.u...^.C..6.4
-00000b40: 170f ddb6 de8b f4ad c7c3 dcb8 5f9c 46f3  ............_.F.
-00000b50: cf03 ba61 f4ca be43 19f1 a8fa 32f7 6548  ...a...C....2.eH
-00000b60: 5fd2 113a 71bb 4036 3ad5 4eec 3a29 cf70  _..:q.@6:.N.:).p
-00000b70: a372 6fa9 5fd2 88d5 2a65 2516 ddd6 fb0e  .ro._...*e%.....
-00000b80: 6952 f3b1 25ef 882c 6085 3683 f131 2404  iR..%..,`.6..1$.
-00000b90: c291 6881 ae68 3836 18ff 2547 60d5 5ede  ..h..h86..%G`.^.
-00000ba0: f5c8 f65d a462 0621 9f91 e867 6226 693d  ...].b.!...gb&i=
-00000bb0: 61a9 6482 6631 eb4d cc3b 1384 57f6 8c8a  a.d.f1.M.;..W...
-00000bc0: 8b4e b688 62bb e9e0 94c7 f3fd 4f91 6168  .N..b.......O.ah
-00000bd0: 8ea0 2dd5 af44 bbab 6662 1dd8 b841 7b21  ..-..D..fb...A{!
-00000be0: b241 ea72 9afe c054 7b58 7c4d 671f 9a4b  .A.r...T{X|Mg..K
-00000bf0: 5dc7 3eda f677 a721 be3f 6fea 219e b94a  ].>..w.!.?o.!..J
-00000c00: 6858 aa9c 032c a838 5ef6 b6ed d9e2 3227  hX...,.8^.....2'
-00000c10: 12a5 03f8 688d 76ad 3267 9e92 fe3b d2d3  ....h.v.2g...;..
-00000c20: d14d 43a5 bd26 e0d8 68bc 17f9 ff21 04a9  .MC..&..h....!..
-00000c30: d7b6 7770 58bb 4c34 3ca7 2609 6a17 387d  ..wpX.L4<.&.j.8}
-00000c40: da12 43d1 f09a 807d 5a20 50d6 71e7 5c67  ..C....}Z P.q.\g
-00000c50: 6cf9 c5d5 cec9 654c 1ba3 d197 a132 fe20  l.....eL.....2. 
-00000c60: dda9 a243 6d30 3c33 e6a8 ea6d 6c16 85fe  ...Cm0<3...ml...
-00000c70: 429f 2adc 1f64 7a5d 6ddb 754a 665f fafe  B.*..dz]m.uJf_..
-00000c80: da03 4d0c 5d84 580d 643f ec79 6df8 84a4  ..M.].X.d?.ym...
-00000c90: 8c4f 636a 7703 38fb d37a d665 9159 b384  .Ocjw.8..z.e.Y..
-00000ca0: 6ea9 cb6d 897d 54f8 fa4d 3d05 bc22 4648  n..m.}T..M=.."FH
-00000cb0: 99af 89ee 6f54 adf8 ddd1 87dc 2a54 da6a  ....oT......*T.j
-00000cc0: 9450 03ee f73d 45eb 6fa4 a259 671a bd66  .P...=E.o..Yg..f
-00000cd0: bb93 8108 0171 0f4d 3226 266e 6ff2 3dcf  .....q.M2&&no.=.
-00000ce0: 38eb 6f5f 6869 0c8a 7da1 ac79 dc64 cc71  8.o_hi..}..y.d.q
-00000cf0: 7042 a650 7bbb cd65 bc85 fb9b 8626 dd68  pB.P{..e.....&.h
-00000d00: ea23 f250 71e3 b40d cca6 a041 4014 fd87  .#.Pq......A@...
-00000d10: 843a 2a1f e4ef be80 7429 0546 dae1 1066  .:*.....t).F...f
-00000d20: 6c3e 88fe 2a30 1a93 55b9 05c1 7596 fa84  l>..*0..U...u...
-00000d30: bbf1 9980 7aa8 b538 db31 6853 8fbd 118a  ....z..8.1hS....
-00000d40: 75df 5b97 7829 e935 4376 b55b f0cc 34a3  u.[.x).5Cv.[..4.
-00000d50: 63fd 5b23 7687 73ef 949d 6014 816b fb1a  c.[#v.s...`..k..
-00000d60: 88fd e9d0 77f3 5fb6 7778 0c7a a96e 36d7  ....w._.wx.z.n6.
-00000d70: 4ecd 984a 4d75 4aaa c916 efd9 77e2 9b0c  N..JMuJ.....w...
-00000d80: f476 f1a5 0f47 6d89 819a 9312 d0c7 f5fc  .v...Gm.........
-00000d90: 784c 476d c42c 4136 8b6d 1ba1 b910 466e  xLGm.,A6.m....Fn
-00000da0: 4926 291a 7903 41eb 4499 0c1a af03 1f2f  I&).y.A.D....../
-00000db0: db19 87c4 bf6e 3f6a 7a87 06d0 7a14 6ddd  .....n?jz...z.m.
-00000dc0: 6b94 f121 619d 12b0 4aa3 18dc 7c3f 8495  k..!a...J...|?..
-00000dd0: d70c 3139 0533 997a 83ce 63bd c0fd 4b52  ..19.3.z..c...KR
-00000de0: 7c6e 75ab 8a2c 040b 00d5 9bd2 24d7 2674  |nu..,......$.&t
-00000df0: 59f1 007b 7d9b 1542 cfe9 4310 f40d b66a  Y..{}..B..C....j
-00000e00: f976 51a2 9cdf 2a78 7dda 0565 2d3e 0933  .vQ...*x}..e->.3
-00000e10: f9a2 86c1 c875 d077 1369 ef76 7e7b 95e1  .....u.w.i.v~{..
-00000e20: 9c5a 8c33 3e77 1f41 f2ae 7ec6 1376 60e3  .Z.3>w.A..~..v`.
-00000e30: 7edf 096b ac95 8071 a9da 9f28 8262 1127  ~..k...q...(.b.'
-00000e40: 9fd6 cb9d 8028 600f 1523 6a79 58bc 0c6e  .....(`..#jyX..n
-00000e50: 4dec cc20 91e9 8a84 802c 28e7 e9d9 119c  M.. .....,(.....
-00000e60: 315c a80d f1ee cfd1 670e a3ef 816a a231  1\......g....j.1
-00000e70: 16ce 8311 e612 6cd1 5a69 8544 95ca b4dc  ......l.Zi.D....
-00000e80: 8194 4274 f6bf c49e 0e0b b67a 9c81 695c  ..Bt.......z..i\
-00000e90: bf90 e0e7 8226 9d5b 29a5 7cd3 fda0 07c6  .....&.[).|.....
-00000ea0: c786 d211 19a1 ed23 84e8 7ef0 838e 2648  .......#..~...&H
-00000eb0: a797 c794 924b a192 234d 3f2d 85c0 14e1  .....K..#M?-....
-00000ec0: 400b 943a 1497 8dca 028a f980 e93b c00e  @..:.........;..
-00000ed0: 862a cd05 bfd2 822b 4f12 681d 9efb a224  .*.....+O.h....$
-00000ee0: 7bbb 1807 8699 1ad6 2983 9978 a859 bca1  {.......)..x.Y..
-00000ef0: d18f 1efc 31e8 57b7 86f0 2915 7af2 7140  ....1.W...).z.q@
-00000f00: 8ecd ef17 7a79 63e9 8346 8af9 8817 8c36  ....zyc..F.....6
-00000f10: ea5d a1f9 15e1 6821 9957 6606 5f5b 6d73  .]....h!.Wf._[ms
-00000f20: 88dd c31d 05ad 8f61 3568 8f09 938d bc6c  .......a5h.....l
-00000f30: 8737 d3fa 88e6 6128 8ad6 c373 9f2e 7ff5  .7....a(...s....
-00000f40: 914e f372 27e2 a68e 8951 b1b0 f703 7a49  .N.r'....Q....zI
-00000f50: 3d27 5ab0 fec5 9f7d 7ebb 0954 8dfd 3318  ='Z....}~..T..3.
-00000f60: 74ae 3d3c cb5b f773 0862 39d0 e9ee 07b7  t.=<.[.s.b9.....
-00000f70: 8f8a ab00 7ddc 625f 1d2c 8c53 b11c 596c  ....}.b_.,.S..Yl
-00000f80: b9e7 bfbe 8fbc 1f9d ec85 d119 83cd bda2  ................
-00000f90: cca0 194f 49cb bd9d 9165 546b ddee 6246  ...OI....eTk..bF
-00000fa0: bd4e 8ab0 fc32 cf36 2bca cb8f 9208 66c0  .N...2.6+.....f.
-00000fb0: 12c2 5fbb e11d 9f16 2ad2 6b38 6402 190f  .._.....*.k8d...
-00000fc0: 920d e909 d079 46eb 3c8d 8564 b8d8 1b0b  .....yF.<..d....
-00000fd0: 9f79 f6d9 95af 810d a5f3 c8a0 0053 7e76  .y...........S~v
-00000fe0: ac19 d601 3180 a30e 966d 853d dfd4 03ca  ....1....m.=....
-00000ff0: 6d2f c1b0 2ced a83c cf9e 34be 9b32 0284  m/..,..<..4..2..
-00001000: 16f4 ad2c e050 e2bc a50b 3643 bf53 d939  ...,.P....6C.S.9
-00001010: 9bd4 414f 9100 287c c7cc b134 a801 69fe  ..AO..(|...4..i.
-00001020: 6be6 f013 9c37 669c fc00 9427 5882 a966  k....7f....'X..f
-00001030: bc95 f449 ddb1 90aa 9d47 933c 7bda c7e1  ...I.....G.<{...
-00001040: 44c7 9988 b39f cc09 0afd 02ca 9e9b 32e6  D.............2.
-00001050: 1733 4a73 337a ba1a 8aef ff4f d4ba 38a6  .3Js3z.....O..8.
-00001060: a0b7 1932 6868 e0e7 1536 4ced e59f 4db3  ...2hh...6L...M.
-00001070: 0591 d846 a1ac 4ed2 cfed 865b c368 7980  ...F..N....[.hy.
-00001080: 3a3b a1ba 531c c53d a285 ae6d 645e f9a5  :;..S..=...md^..
-00001090: b7e0 055c 3d58 8af7 85e2 9dda a2bb 54fe  ...\=X........T.
-000010a0: 8acf 2a8c 6d15 0c5c 0e89 b983 f721 ee0e  ..*.m..\.....!..
-000010b0: a3ec 8691 03d2 e3dc 18fb 5930 3123 9f5c  ..........Y01#.\
-000010c0: abf3 be1e a42a 39aa 0aae 12ca 3dfb fa82  .....*9.....=...
-000010d0: ad50 7cce 0a2c 2df1 a591 f756 00d9 ff2a  .P|..,-....V...*
-000010e0: bb7a d6ec 6aa8 2b9e 3c11 26d0 a5a5 1843  .z..j.+.<.&....C
-000010f0: 0b76 0fc3 ce3e 0834 cf90 79db cfb6 da1f  .v...>.4..y.....
-00001100: a6ba a636 d0f5 3143 269b 968c 58c3 6819  ...6..1C&...X.h.
-00001110: 8b91 0bf5 a7f3 a641 d9ea 72f5 1911 b41c  .......A..r.....
-00001120: 4f99 6ad4 7230 00a2 a841 8e57 a4e8 a6f2  O.j.r0...A.W....
-00001130: 8cec 8a95 04e5 f9e7 b4a3 1bba a852 e343  .............R.C
-00001140: 4638 f815 4709 3243 23dc d6ef e909 0a67  F8..G.2C#......g
-00001150: a86e 13e3 567f d165 1199 e0be 5716 6bb8  .n..V..e....W.k.
-00001160: a88c a5cf a93f f7af 535e 15fb 644a 3da6  .....?..S^..dJ=.
-00001170: ca21 d496 bc98 0e87 a94c e1a1 b2d8 d1db  .!.......L......
-00001180: da64 dce5 6418 8f74 480f 2f03 a94e d9b1  .d..d..tH./..N..
-00001190: 8b51 adb0 4a3e 0250 d016 41f8 03b1 6b4a  .Q..J>.P..A...kJ
-000011a0: aa3f af30 45dc f6d8 0fd4 24b2 10d0 2aee  .?.0E.....$...*.
-000011b0: 0b24 76d4 aa6c aa64 5ee6 6d82 20e4 8946  .$v..l.d^.m. ..F
-000011c0: 6e95 585c b428 ace8 aa96 92c2 4e2c d742  n.X\.(......N,.B
-000011d0: be01 6017 53e0 64b3 589c 4285 aae1 7c32  ..`.S.d.X.B...|2
-000011e0: 0706 3f00 2655 22ea 7fcd 1ef9 71cc cc85  ..?.&U".....q...
-000011f0: ab44 4fae c380 805a f86f 23bb 673c 8094  .DO....Z.o#.g<..
-00001200: 1d07 b847 ad00 c606 d0e3 aa41 0ff0 dd50  ...G.......A...P
-00001210: 9938 282b 21c0 2d45 afb8 bfa3 153b c2d7  .8(+!.-E.....;..
-00001220: 9b4c ca8b 8c7d ec66 d816 979f b0e6 a5a3  .L...}.f........
-00001230: 137b 7fe6 8f10 77fc a0f7 95f1 d89d d24e  .{....w........N
-00001240: b0ef 7617 668e 1a3d bf36 4ce6 4b25 214b  ..v.f..=.6L.K%!K
-00001250: 96b1 8b22 b14e 1c10 9ef6 582a 30f9 1b6f  ...".N....X*0..o
-00001260: fc27 2af2 5418 7b7e b2cb 8072 2c6d 0e61  .'*.T.{~...r,m.a
-00001270: 4ca6 4214 6f34 86a1 cb84 55c6 b525 32ad  L.B.o4....U..%2.
-00001280: cf7e 7245 a9d3 0908 0a1c 8d5f 8269 1be1  .~rE......._.i..
-00001290: b69f 2b64 4291 26cb db65 bdfc f8fb 74d2  ..+dB.&..e....t.
-000012a0: 563a 78b4 b6d2 6cfe 0653 baba 78b0 8eef  V:x...l..S..x...
-000012b0: b82e be57 069f 3e84 b774 aec3 980b 1fea  ...W..>..t......
-000012c0: f8ad bdec 34b8 b5e7 49d9 f489 b79a 7def  ....4...I.....}.
-000012d0: 50be eb46 660f d51f 8165 7f26 02a4 d2a1  P..Ff....e.&....
-000012e0: b812 2b62 0dc6 fd61 6c4a 7c45 3259 9ffb  ..+b...alJ|E2Y..
-000012f0: ce82 a4ff b8ec 5c4a 53ed 4d65 40aa 9b08  ......\JS.Me@...
-00001300: ad82 2e7f 1ae3 4c03 b96d 623a 82de 0268  ......L..mb:...h
-00001310: 3fc6 762b 21a9 7d57 b65f eb5d bbf3 07ff  ?.v+!.}W._.]....
-00001320: 3ce7 2e6c f8df 49bc 07ab 19ea c8f0 bf6b  <..l..I........k
-00001330: bce0 4f51 51ef c1d9 5de9 5f9a 82e8 e8e5  ..OQQ...]._.....
-00001340: 5308 eb62 bcfb 8940 46e6 e2bb 40c0 2520  S..b...@F...@.% 
-00001350: 721d ec5b a4ed 4f94 be9d c361 7df9 314c  r..[..O....a}.1L
-00001360: d5e8 cc20 d6fb 7d71 5b86 c3a9 bebc 19a2  ... ..}q[.......
-00001370: 8531 46d8 6974 fc1a 5496 a8ec afc0 7001  .1F.it..T.....p.
-00001380: bff7 7398 1b53 4d2d 283a eeaf 4f13 5954  ..s..SM-(:..O.YT
-00001390: 5412 8151 c1a3 cd27 5bed 2f28 b18d a9c9  T..Q...'[./(....
-000013a0: d954 6783 4f19 51a3 c2b5 d1ac f4af 894f  .Tg.O.Q........O
-000013b0: 5fa8 9064 c006 b13f 1c5c d512 c2c3 39d9  _..d...?.\....9.
-000013c0: 8466 e36a 3512 afe2 7281 c649 72bc 5c43  .f.j5...r..Ir.\C
-000013d0: c497 2490 7117 db59 238d 10d2 8d6d 1139  ..$.q..Y#....m.9
-000013e0: 0b77 a68d c4ce b708 ba86 0a5d 0efe c766  .w.........]...f
-000013f0: 1978 e1f4 8881 da70 c5b9 7d08 7ae2 32f4  .x.....p..}.z.2.
-00001400: 124b 062d 8d25 f6a6 99db 7adc c63a 6859  .K.-.%....z..:hY
-00001410: 9674 c77f c43f ba7a c193 52d0 a6c0 c961  .t...?.z..R....a
-00001420: c723 b47d 51d7 5a6a d656 299e ba5e 6a86  .#.}Q.Zj.V)..^j.
-00001430: 482a 3ba6 c792 6ae6 0405 f5b2 43d9 b4ef  H*;...j.....C...
-00001440: ee3b 601c d7f2 626d c7f5 d105 2f93 504b  .;`...bm..../.PK
-00001450: ff55 27db 3bb2 f4a8 619c d566 c8b0 cac0  .U'.;...a..f....
-00001460: 8185 4d01 38b4 9d3f 0e56 3aef ea99 2dd1  ..M.8..?.V:...-.
-00001470: c8f0 0699 181e 53ff 0551 2a20 58d0 9910  ......S..Q* X...
-00001480: 00ff 2e75 c93f 88bc db0e 6cd8 f7dd 75d1  ...u.?....l...u.
-00001490: 869f e4ca 33c2 b743 cafc ce98 5b49 bb24  ....3..C....[I.$
-000014a0: 1488 dee9 f590 0a56 2524 4985 cb20 3784  .......V%$I.. 7.
-000014b0: ebeb d5e6 885a e698 22ca a8d8 cfaf 4ed4  .....Z..".....N.
-000014c0: cc32 fb60 a921 776f 4ffe 97f1 a718 dbbf  .2.`.!woO.......
-000014d0: 8951 20b0 cd94 0740 6aab 7801 64e2 cfdb  .Q ....@j.x.d...
-000014e0: 10cb 6082 e92f 4ab2 cf74 1b81 bc74 61bc  ..`../J..t...ta.
-000014f0: b592 c215 2ee6 27b3 1b80 2157 cfca 8f83  ......'...!W....
-00001500: da3c f40a c8ca 0813 f8e9 1aa6 1918 155d  .<.............]
-00001510: d235 4ba5 ef0d 2041 7c4b d318 5238 9ddb  .5K... A|K..R8..
-00001520: cf11 f5bf d240 4d7c 2381 a079 3332 8add  .....@M|#..y32..
-00001530: 2a3f 55c0 5757 a598 d2b1 291e 883c 3f9d  *?U.WW....)..<?.
-00001540: 5692 733d 17ec ce23 70c4 0e78 d3e9 c40d  V.s=...#p..x....
-00001550: c20d b746 44a1 10c2 65ba cac2 c832 9d36  ...FD...e....2.6
-00001560: d564 cd08 2d74 81d5 a8b0 406a 7431 78ee  .d..-t....@jt1x.
-00001570: 1be1 7406 d77b b103 3a9d 51fb 0861 9c8b  ..t..{..:.Q..a..
-00001580: 6386 0e57 e10a 11b1 d967 f0e3 518a 5b57  c..W.....g..Q.[W
-00001590: 926e d042 290d 1032 c14e 2e5a daff 91bd  .n.B)..2.N.Z....
-000015a0: a246 920d dfef c4d4 f2f2 2860 2525 d26a  .F........(`%%.j
-000015b0: db80 a150 3755 7412 42c1 8617 a5e0 6dc5  ...P7Ut.B.....m.
-000015c0: b9a9 cee5 db9b 66f1 c32b 9c01 349e c0e7  ......f..+..4...
-000015d0: 11a0 cb71 b487 cee9 dd4f 663d 5c7c b396  ...q.....Of=\|..
-000015e0: 1e68 d656 ea13 8f83 1b20 2429 dd75 b6da  .h.V..... $).u..
-000015f0: edbd 78f3 5e08 3b4d e818 3fb2 c722 bf13  ..x.^.;M..?.."..
-00001600: de30 f0b3 c514 2b03 458b ae01 58bb 69a0  .0....+.E...X.i.
-00001610: 0bb2 d57b de41 62dd 1943 3851 ae15 c7f9  ...{.Ab..C8Q....
-00001620: 1a9d 74b8 9566 4057 de4a ac57 d4b7 7be4  ..t..f@W.J.W..{.
-00001630: 2a82 adf9 755d 4eb7 11ca f8c0 de91 dcae  *...u]N.........
-00001640: 25aa c7d3 0294 3c70 45f9 80ab 35dd cb48  %.....<pE...5..H
-00001650: dee3 c25b e088 ed87 1b0b bcd8 be9f 490c  ...[..........I.
-00001660: 5c81 0ac2 e04d 74a1 48a5 3b66 0bed e3bb  \....Mt.H.;f....
-00001670: 1d3d 2649 a5b9 0334 e04f 9606 19cc 7622  .=&I...4.O....v"
-00001680: 3f68 7115 d0c1 9232 42a3 6898 e09e 50a6  ?hq....2B.h...P.
-00001690: b199 3437 a769 501c b4e2 695a 56e2 5fed  ..47.iP...iZV._.
-000016a0: e0a4 09e6 9964 0445 6c4e 2da8 c700 492d  .....d.ElN-...I-
-000016b0: 811d 1f9d e189 ae1a 43a9 9f66 2334 f82b  ........C..f#4.+
-000016c0: d815 068c d496 7b38 e1d6 8ffc 007d e403  ......{8.....}..
-000016d0: 4742 712a f72a 0352 3ef3 70fe e247 eeb0  GBq*.*.R>.p..G..
-000016e0: 629d c5d9 881e fe68 441c 79ff ea8f 885f  b......hD.y...._
-000016f0: e285 6269 9fe1 a2ee 1c4f 5d4b 3232 95c2  ..bi.....O]K22..
-00001700: 3ae2 697b e4c1 4033 551e 6292 dbbc 2a4b  :.i{..@3U.b...*K
-00001710: e443 c33a 3b04 f9ae e4e2 d206 a214 b26d  .C.:;..........m
-00001720: 103d 53e1 be4f fcf9 57e4 27db e53e f57d  .=S..O..W.'..>.}
-00001730: a109 9e80 4f70 08f7 cd4e 8879 817d 364e  ....Op...N.y.}6N
-00001740: e610 b3d7 a44e b79c be09 9d27 f245 448c  .....N.....'.ED.
-00001750: 5ecd bf09 e69d e29b b2d1 d643 4b8b 29ae  ^..........CK.).
-00001760: 775a d8c2 e48c 5391 e6fc 34af 4a8f 603b  wZ....S...4.J.`;
-00001770: 4cf8 40ea 342d de03 c0a8 5d82 e794 4e14  L.@.4-....]...N.
-00001780: a44e 60c6 a68b 29fc 4b31 50b7 680a aeb4  .N`...).K1P.h...
-00001790: e7dc 7a7b d3ae 99e9 e704 fd03 1de9 1dcb  ..z{............
-000017a0: c5cd 116f e898 8aec 01e6 5c99 9109 5098  ...o......\...P.
-000017b0: 0230 9bc2 a781 5db8 e940 4fa4 7750 2176  .0....]..@O.wP!v
-000017c0: ac80 b88b e458 3a1e a305 a5bf e968 e86b  .....X:......h.k
-000017d0: f3d2 83f4 8e4c b483 cb8a e9a7 5178 9486  .....L......Qx..
-000017e0: ea9d c1ad cbee 374b f5b9 01a5 f11a 3c97  ......7K......<.
-000017f0: 37b0 518e eb87 9404 f6d7 d489 daae 129f  7.Q.............
-00001800: dba9 26f6 7f8c 7708 ed08 b5df b70e 776c  ..&...w.......wl
-00001810: 72b4 3c7e 5e90 509f 9566 a32e efc3 ac6e  r.<~^.P..f.....n
-00001820: 98c7 b60a c84a 08a2 aaa2 4a74 6617 8746  .....J....Jtf..F
-00001830: f14f 5656 1893 a634 b60e 0239 9b6f 0e02  .OVV...4...9.o..
-00001840: d871 d7e3 f24f 57b3 eb80 39e1 c8d3 e423  .q...OW...9....#
-00001850: 0a6a 0697 92ea b5f3 f390 ef81 b1a8 96ac  .j..............
-00001860: 8b8e c388 e189 7125 a537 24be f413 32fd  ......q%.7$...2.
-00001870: c472 1eea cbd7 ccd6 e5ac c6c9 90dd 2d7f  .r............-.
-00001880: f633 edd3 c761 2dcc 4ede 3aff 172a e7a0  .3...a-.N.:..*..
-00001890: fb6a 1705 f69a 178a fddf a735 0b5c 5778  .j.........5.\Wx
-000018a0: 0399 cccc ff00 650f f780 9474 0a29 a0b2  ......e....t.)..
-000018b0: e1ec a234 2d21 2905 402a 677e f876 9eb1  ...4-!).@*g~.v..
-000018c0: 087c 7f09 03c4 2e41 52d7 637a 79b6 d343  .|.....AR.czy..C
-000018d0: f95a 6816 826e 3b6c c5a2 909e f8ae f549  .Zh..n;l.......I
-000018e0: d07a 84b0 f98a 9ff7 dbca 4e98 b5ba 343a  .z........N...4:
-000018f0: 83cd 588a 0d29 54a5 fb33 3acb 04fc 9d25  ..X..)T..3:....%
-00001900: 7ad4 3dcf f4e3 b1c2 e1ce 95df fb90 5390  z.=...........S.
-00001910: dc36 462c fb3a f0a3 035b c1a0 923d 02ba  .6F,.:...[...=..
-00001920: fc56 84df f4f8 5978 212a dbca 6f0e f241  .V....Yx!*..o..A
-00001930: f92c 2cf0 fcfc 9c8a 4db8 095a 6332 0df9  .,,.....M..Zc2..
-00001940: cee4 7eb8 282c c2e9 fe68 d259 df55 0d5a  ..~.(,...h.Y.U.Z
-00001950: 694b 5594 fbc4 7017 98b0 ba57 3c0e 5daa  iKU...p....W<.].
-00001960: 9426 b1d2 3df4 1a63 c4bb 041f cfba 267d  .&..=..c......&}
-00001970: 90d7 fc69 b25a 2cdf 3f67 91b8 5530 8271  ...i.Z,.?g..U0.q
-00001980: 1336 5390 b768 d554 4a23 b09c 22b0 5574  .6S..h.TJ#..".Ut
-00001990: d6e2 99c5 04db b713 cf23 151c 737c 9258  .........#..s|.X
-000019a0: 3ceb d074 0a28 ab1a c0ee 48ae fd47 cc89  <..t.(....H..G..
-000019b0: ec27 31e1 0f47 3bf3 23aa 9ebb 83f8 c87d  .'1..G;.#......}
-000019c0: 5312 ffa3 eb9a c438 402c f3ac 6756 8645  S......8@,..gV.E
-000019d0: 5246 fcc0 7b52 f34d 3461 2371 e34d 9b21  RF..{R.M4a#q.M.!
-000019e0: b5c8 f238 569c efaf 112e eaef c9b8 27fd  ...8V.........'.
-000019f0: c2cd ecd0 956b 1e14 d8a0 76c5 b007 7768  .....k....v...wh
-00001a00: 98d4 947d f2be e2ff 7070 5294 5aa6 36f8  ...}....ppR.Z.6.
-00001a10: 613a 8038 fa3b fca6 0315 132f a30b 9315  a:.8.;...../....
-00001a20: 3cfa 101d f60a 0874 49f3 a895 29f1 e562  <......tI...)..b
-00001a30: fc75 b350 bb13 fbb9 ca09 5e5a 2c8c 2670  .u.P......^Z,.&p
-00001a40: 609d 373d 3f98 3a9a 84ec fd1d d38c a8d1  `.7=?.:.........
-00001a50: 04f7 4eef e97d 11ea 94e4 d657 cbc6 8a7e  ..N..}.....W...~
-00001a60: 697d 4f1d 5529 0a01 732b 49a2 01ba 81fc  i}O.U)..s+I.....
-00001a70: a651 efa8 ec0d d7af 8a97 a427 38d1 2009  .Q.........'8. .
-00001a80: 6695 2349 efb1 5d0e 4fc9 7768 66bd 11c6  f.#I..].O.whf...
-00001a90: b565 6cca ed05 99c8 f3ca 5737 5bc7 6aca  .el.......W7[.j.
-00001aa0: c5fe e67b d1d8 d598 d0c2 2407 63e9 0052  ...{......$.c..R
-00001ab0: 4ea7 6d6b 273f 0ea9 6209 bda7 8ee6 37fb  N.mk'?..b.....7.
-00001ac0: 507e 3d8e 593a 8740 08dd 9b59 14ca 5bc0  P~=.Y:.@...Y..[.
-00001ad0: 730d 45cb 1c68 c80e 42aa 568c 4259 a81f  s.E..h..B.V.BY..
-00001ae0: 9e19 6fe7 148c 94f0 2f48 fc5f 93de cdd4  ..o...../H._....
-00001af0: 0b3f 7b6c bb2d f6ca df49 556b cf2f 05a4  .?{l.-...IUk./..
-00001b00: 908e c271 08bf ee29 951f 36f3 7047 ee9b  ...q...)..6.pG..
-00001b10: d5e4 ece0 feae f4cf fbdd ccf5 cc05 6a9e  ..............j.
-00001b20: 2f8b 42f2 1f5f ca18 d3dc a083 5ee5 3f04  /.B.._......^.?.
-00001b30: c485 dbfc 1e63 d883 be19 3a75 b619 668d  .....c....:u..f.
-00001b40: 24bd 1f12 d6d4 a821 4f2d 4775 838b 6d35  $......!O-Gu..m5
-00001b50: cf74 ee9a 8214 25f2 1bde f2cd 99b2 a41f  .t....%.........
-00001b60: 1f8d 96d8 af5c 4816 fc27 d410 f8af df30  .....\H..'.....0
-00001b70: 3b33 fa1b 2e6e 00ce 9568 b83c 6b88 504a  ;3...n...h.<k.PJ
-00001b80: b020 229e 2997 8e76 231b db3d 97f5 f4be  . ".)..v#..=....
-00001b90: 9e8d e866 2822 80ac 7f6d f04b 48b6 bdfe  ...f("...m.KH...
-00001ba0: 7315 c5ee 5dfa cd90 0e9b d730 b196 7ee7  s...]......0..~.
-00001bb0: 67a0 1e7e bd39 7464 2da8 393e f245 3e14  g..~.9td-.9>.E>.
-00001bc0: a975 ef48 35cd f071 c7fb d20f fe73 124a  .u.H5..q.....s.J
-00001bd0: 25a0 317c 63e9 ba03 3741 c5e7 f4f7 eec9  %.1|c...7A......
-00001be0: 449c 8ab6 007f f2f4 f28d 8428 14a1 c3b5  D..........(....
-00001bf0: 2d5c 0128 9d75 8d06 f55c a45f 626c e406  -\.(.u...\._bl..
-00001c00: 330b c910 a597 dff1 6ab1 1a13 20c3 be01  3.......j... ...
-00001c10: b363 46e9 ab9c 6877 5def 3901 fef3 efff  .cF...hw].9.....
-00001c20: a9e9 c093 e086 e9d9 0071 c4f6 3fad 593f  .........q..?.Y?
-00001c30: a411 a5fb ee7f 350f 978d 830b bd5e 6b33  ......5......^k3
-00001c40: 8dbd b39c 5d6a 6b8e 2442 6a12 aa89 132b  ....]jk.$Bj....+
-00001c50: b403 1cdc 1338 e146 bb90 c89b 0dc5 c21d  .....8.F........
-00001c60: d7a3 352b f703 72f8 0de2 b65f b211 a7fc  ..5+..r...._....
-00001c70: f03a a9d8 16ed 4d3b 9034 3a6e eb26 8c09  .:....M;.4:n.&..
-00001c80: 6d69 11a9 0dbd 538e 1d3b a937 b88d e288  mi....S..;.7....
-00001c90: d453 98ec d465 f2e0 f1e0 3760 76a6 b227  .S...e....7`v..'
-00001ca0: e793 ef4e 9b97 9a79 494e d527 43b2 eb5b  ...N...yIN.'C..[
-00001cb0: f5ee 0530 6596 e541 c783 2f05 d025 6a19  ...0e..A../..%j.
-00001cc0: 677b 2478 c00c 3b06 6f70 ddeb 58aa 76c5  g{$x..;.op..X.v.
-00001cd0: f04d 19c8 ed5d 801d 3c4f 72c5 6a1a 79dc  .M...]..<Or.j.y.
-00001ce0: 7ec5 6e92 4763 101c 0de2 586d 99d2 c97f  ~.n.Gc....Xm....
-00001cf0: 63ab 660f 2d38 25d1 4bab 64f6 01de f13e  c.f.-8%.K.d....>
-00001d00: 5f41 c86d 2b26 ff96 f929 573f cd5b 07fd  _A.m+&...)W?.[..
-00001d10: dd22 b101 cbe0 beca cb26 c754 e831 85ec  .".......&.T.1..
-00001d20: e57c 2e66 7fee 2ec4 ca6d 7a25 70d0 897b  .|.f.....mz%p..{
-00001d30: 23fc dffd 6db7 d623 6e76 0029 e139 aaf6  #...m..#nv.).9..
-00001d40: df9e 26be b988 54aa cb2c 19bc 9bbc f8e7  ..&...T..,......
-00001d50: ff76 0474 1983 93cf a0a5 4164 96c8 2e24  .v.t......Ad...$
-00001d60: 55cc 7aec f2bf 1da9 e4c5 e7ca f192 48e6  U.z...........H.
-00001d70: 8a50 bd94 51c3 f578 d27a bb29 ca2b 00a7  .P..Q..x.z.).+..
-00001d80: c218 0cee 038a 9293 58c4 29ac 2efd 63a0  ........X.)...c.
-00001d90: 0e77 75b2 44c0 d7e1 c994 c26c 1a45 e0a4  .wu.D......l.E..
-00001da0: 0000 b4c8 0000 3d92 0000 3609 0000 3cf8  ......=...6...<.
-00001db0: 0000 46d4 0000 e266 0000 ebe8 0000 b37f  ..F....f........
-00001dc0: 0000 7932 0000 97f7 0000 9989 0000 73da  ..y2..........s.
-00001dd0: 0000 ea04 0000 27c8 0000 affb 0000 875b  ......'........[
-00001de0: 0000 36fd 0000 e1b8 0000 43a0 0000 d89d  ..6.......C.....
-00001df0: 0000 9c8d 0000 9558 0000 790a 0000 ac3e  .......X..y....>
-00001e00: 0000 0904 0000 1e3f 0000 af3e 0000 93d1  .......?...>....
-00001e10: 0000 d757 0000 b341 0000 3a7c 0000 4774  ...W...A..:|..Gt
-00001e20: 0000 2ea3 0000 8b39 0000 095d 0000 8464  .......9...]...d
-00001e30: 0000 068c 0000 2631 0000 3645 0000 0e58  ......&1..6E...X
-00001e40: 0000 df8e 0000 e175 0000 893a 0000 2c26  .......u...:..,&
-00001e50: 0000 b818 0000 9334 0000 3fdc 0000 8911  .......4..?.....
-00001e60: 0000 b058 0000 8be9 0000 47d8 0000 0a01  ...X......G.....
-00001e70: 0000 8a45 0000 8a97 0000 7944 0000 6e9a  ...E......yD..n.
-00001e80: 0000 2bf0 0000 b24e 0000 b487 0000 ba95  ..+....N........
-00001e90: 0000 3fb9 0000 9970 0000 078f 0000 ebd0  ..?....p........
-00001ea0: 0000 bac6 0000 e64a 0000 9a51 0000 01f8  .......J...Q....
-00001eb0: 0000 3387 0000 bb38 0000 4220 0000 be66  ..3....8..B ...f
-00001ec0: 0000 05b7 0000 7484 0000 ae30 0000 3c3e  ......t....0..<>
-00001ed0: 0000 4017 0000 33fb 0000 93b1 0000 91ce  ..@...3.........
-00001ee0: 0000 a5d5 0000 0930 0000 ec35 0000 32d8  .......0...5..2.
-00001ef0: 0000 e353 0000 3d0d 0000 9b50 0000 3dc7  ...S..=....P..=.
-00001f00: 0000 3b82 0000 b026 0000 9a23 0000 d93e  ..;....&...#...>
-00001f10: 0000 91a2 0000 be7c 0000 a489 0000 3bf3  .......|......;.
-00001f20: 0000 a561 0000 98d9 0000 ad8f 0000 995d  ...a...........]
-00001f30: 0000 b1af 0000 877c 0000 368e 0000 b0cc  .......|..6.....
-00001f40: 0000 b4b5 0000 3a3c 0000 dc40 0000 00af  ......:<...@....
-00001f50: 0000 36e5 0000 aa35 0000 aaaf 0000 48c3  ..6....5......H.
-00001f60: 0000 c1aa 0000 a167 0000 ebff 0000 dfd1  .......g........
-00001f70: 0000 ab53 0000 3ac2 0000 b171 0000 e31d  ...S..:....q....
-00001f80: 0000 4360 0000 4aaf 0000 b199 0000 e132  ..C`..J........2
-00001f90: 0000 03dc 0000 08b3 0000 86b1 0000 0369  ...............i
-00001fa0: 0000 4333 0000 dd89 0000 dabe 0000 3b07  ..C3..........;.
-00001fb0: 0000 9742 0000 c4da 0000 77f4 0000 2bbb  ...B......w...+.
-00001fc0: 0000 9d04 0000 2503 0000 4d35 0000 afd3  ......%...M5....
-00001fd0: 0000 1ee2 0000 3439 0000 e1fb 0000 34f9  ......49......4.
-00001fe0: 0000 79a9 0000 937e 0000 940a 0000 0ad9  ..y....~........
-00001ff0: 0000 4824 0000 9a65 0000 af11 0000 24d7  ..H$...e......$.
-00002000: 0000 425e 0000 c808 0000 e37b 0000 1e2d  ..B^.......{...-
-00002010: 0000 8340 0000 4273 0000 1e71 0000 2fb4  ...@..Bs...q../.
-00002020: 0000 e05a 0000 d5a6 0000 d688 0000 96e5  ...Z............
-00002030: 0000 9505 0000 12c1 0000 e52a 0000 9130  ...........*...0
-00002040: 0000 e087 0000 7866 0000 2491 0000 000c  ......xf..$.....
-00002050: 0000 47b9 0000 a5b6 0000 0e14 0000 03a6  ..G.............
-00002060: 0000 94ae 0000 d7fa 0000 deb6 0000 11c2  ................
-00002070: 0000 331e 0000 0764 0000 05f2 0000 2e00  ..3....d........
-00002080: 0000 0ab7 0000 dba5 0000 0a7a 0000 83ad  ...........z....
-00002090: 0000 cb33 0000 b298 0000 26aa 0000 ce62  ...3......&....b
-000020a0: 0000 94db 0000 e229 0000 e0b2 0000 d18f  .......)........
-000020b0: 0000 af69 0000 e2e0 0000 41dd 0000 2667  ...i......A...&g
-000020c0: 0000 972f 0000 ad48 0000 9ba7 0000 258e  .../...H......%.
-000020d0: 0000 2703 0000 ad1c 0000 36a2 0000 3457  ..'.......6...4W
-000020e0: 0000 d6b5 0000 428b 0000 26e7 0000 7997  ......B...&...y.
-000020f0: 0000 d497 0000 9837 0000 8bce 0000 7892  .......7......x.
-00002100: 0000 0a37 0000 abee 0000 7d1e 0000 470a  ...7......}...G.
-00002110: 0000 83da 0000 a5a3 0000 2566 0000 95ff  ..........%f....
-00002120: 0000 413a 0000 9b0a 0000 8bb8 0000 9b91  ..A:............
-00002130: 0000 96a2 0000 3d75 0000 e02c 0000 d4cb  ......=u...,....
-00002140: 0000 3db0 0000 a242 0000 9c60 0000 3cb6  ..=....B...`..<.
-00002150: 0000 40ea 0000 b09d 0000 9bc0 0000 7466  ..@...........tf
-00002160: 0000 9214 0000 05db 0000 4115 0000 9823  ..........A....#
-00002170: 0000 8f61 0000 2e32 0000 a8f7 0000 aaa6  ...a...2........
-00002180: 0000 279f 0000 90ee 0000 d4f9 0000 975d  ..'............]
-00002190: 0000 023b 0000 991c 0000 7cee 0000 3b47  ...;......|...;G
-000021a0: 0000 88c4 0000 b276 0000 3000 0000 8b7c  .......v..0....|
-000021b0: 0000 741c 0000 922d 0000 e0f5 0000 9fc3  ..t....-........
-000021c0: 0000 8f23 0000 b07e 0000 77c4 0000 e2a3  ...#...~..w.....
-000021d0: 0000 3237 0000 8363 0000 40be 0000 da23  ..27...c..@....#
-000021e0: 0000 6b03 7f7d 2c81 2fc9 c652 e037 7f6b  ..k..},./..R.7.k
-000021f0: 4148 f381 51d8 a136 faf9 1c4d 0cb9 167c  AH..Q..6...M...|
-00002200: 1c7d 3720 abd1 7aa9 01af e60d            .}7 ..z.....
+000004a0: 18b3 1b08 07e3 db6e 06a8 4616 2113 0428  .......n..F.!..(
+000004b0: f5d4 be26 42a3 7bcb 62d7 e1c4 0725 883b  ...&B.{.b....%.;
+000004c0: 4fee 1fed 28e6 bc64 a993 11c9 4684 0053  O...(..d....F..S
+000004d0: 076b 11c0 012f 9e04 a9d5 4016 1c16 ecb5  .k.../....@.....
+000004e0: 0bce f460 09a6 8b4b bcdd f77d 7431 7fd9  ...`...K...}t1..
+000004f0: e224 50d8 c445 607e 09f4 9f7d 68f4 2b0f  .$P..E`~...}h.+.
+00000500: 750e 2aba 9acb 1daa c79d 50c9 0aac 1694  u.*.......P.....
+00000510: 4d6b 28c7 fc05 9944 50df 60a7 6888 f41f  Mk(....DP.`.h...
+00000520: 0b34 c374 78ab 675c 6ad3 9730 ccf9 8af1  .4.tx.g\j..0....
+00000530: 88e7 0ff9 0c2e 2a86 e7d7 efbf 512b cf6b  ......*.....Q+.k
+00000540: 85cf 6a38 a898 0019 0c91 98ac ccb3 d1ad  ..j8............
+00000550: d56b 4496 e591 fa18 cbaf 64fc 0d82 432f  .kD.......d...C/
+00000560: c2d9 3143 d515 42d0 f4ed 03b6 3bff 69a2  ..1C..B.....;.i.
+00000570: 0ea0 e38a 01b8 958f fbcf 297a a773 effe  ..........)z.s..
+00000580: 3623 34d0 0fee 61e9 f377 8410 9916 ff54  6#4...a..w.....T
+00000590: 035f 13f5 14df 8360 1025 1521 c1c9 9f77  ._.....`.%.!...w
+000005a0: 238b 4860 3be0 42ba 5823 a198 1129 d93b  #.H`;.B.X#...).;
+000005b0: 10cf ecb6 235a 9e7f 4ab5 3cc7 24ed 056c  ....#Z..J.<.$..l
+000005c0: 1427 6e10 d8a0 d752 dc35 3a7c d10a 253b  .'n....R.5:|..%;
+000005d0: c579 379a 1433 ce41 50bb b18b f7b3 c2d6  .y7..3.AP.......
+000005e0: c4b8 9b32 084c 1e7d 146c addd 63f0 e9df  ...2.L.}.l..c...
+000005f0: a465 4491 1313 6c6e 330e 20cd 149b 0c8c  .eD...ln3. .....
+00000600: 5257 8dc6 3594 ea2a 36cb 3cfd 7feb 0b17  RW..5..*6.<.....
+00000610: 165c 1d7d e49a 08aa f59e d43a c2a9 ba68  .\.}.......:...h
+00000620: b811 30e8 1666 45c6 e558 e949 854d 6828  ..0..fE..X.I.Mh(
+00000630: 6bf7 a958 2a47 a2a0 16f3 c37c 7b5d 4e84  k..X*G.....|{]N.
+00000640: c784 5968 05df 80c6 acbf 1568 1723 625f  ..Yh.......h.#b_
+00000650: 6ac0 e9fb 4a39 f5b9 0d1c ef73 ac7d 53bb  j...J9.....s.}S.
+00000660: 1853 d346 d7ad 03dd b20b 6093 e2c7 a1ed  .S.F......`.....
+00000670: 8a3a 72b2 18b4 e9fc ef00 0284 d53a 8288  .:r..........:..
+00000680: d7e2 7c5e 3564 58cc 1a03 eb1a b938 e53b  ..|^5dX......8.;
+00000690: cd11 68ce cc2b f86e 20aa 761b 1cf3 c9c3  ..h..+.n .v.....
+000006a0: 075c 1fab a1eb d396 5764 e2ec af17 751b  .\......Wd....u.
+000006b0: 1cf4 502a 6173 de16 a0db 5cd2 e32b 2cd8  ..P*as....\..+,.
+000006c0: 0f07 83d0 1d2b bf74 d823 f98f c203 f082  .....+.t.#......
+000006d0: b56e 911f fa50 492e 2044 d5a0 9f55 22b9  .n...PI. D...U".
+000006e0: 616b 252c 0891 a6e8 aa7b ca64 2175 1d36  ak%,.....{.d!u.6
+000006f0: f8f1 7ce9 6aaf c278 22e2 0b6f c35e 999d  ..|.j..x"..o.^..
+00000700: 2275 6466 3235 da9a fcbc e78c 10bf bcca  "udf25..........
+00000710: 1f56 98ed 2302 d30b 1108 da08 5d35 9b7b  .V..#.......]5.{
+00000720: 0054 2e6d 1846 0766 2559 1dca 5a32 c357  .T.m.F.f%Y..Z2.W
+00000730: c6e7 d67c 9d88 fdf9 9e57 2191 25f2 e150  ...|.....W!.%..P
+00000740: 2c69 b4cf 1669 971b 9616 8399 2ca6 6ba4  ,i...i......,.k.
+00000750: 27d5 b1bf 06a5 daa9 29cb 20bf d4a1 6010  '.......). ...`.
+00000760: 7e6c 8063 284d 716a b3c7 2c7c 1ec5 1fa5  ~l.c(Mqj..,|....
+00000770: 23db e011 09f2 320a 297d ac16 0961 f0ae  #.....2.)}...a..
+00000780: ea73 2374 aae4 2697 5013 3328 29d2 daac  .s#t..&.P.3()...
+00000790: 5904 9917 2e55 4126 d72d 43d3 0ed5 a046  Y....UA&.-C....F
+000007a0: 2a42 2fef b908 c755 9dd2 f716 8efc 378b  *B/....U......7.
+000007b0: 8785 ba62 2df2 9c70 5bc4 7bc7 c268 e8c4  ...b-..p[.{..h..
+000007c0: 92b6 458e 3b67 b03b 31ce d298 ccae 493b  ..E.;g.;1.....I;
+000007d0: e277 6bdb 7184 b4e3 6003 36da 31d7 7150  .wk.q...`.6.1.qP
+000007e0: caee 8e4d ec78 f304 09f4 fe0d eab6 11c1  ...M.x..........
+000007f0: 32d8 331c 3e6f 336e df84 ee6e 954e 0e72  2.3.>o3n...n.N.r
+00000800: 1de3 a1a4 32e8 3d4f cefa 3337 032a 8247  ....2.=O..37.*.G
+00000810: 709f 7b53 03b1 32e9 3370 fbd1 c498 f950  p.{S..2.3p.....P
+00000820: 017e df7e 2c97 7834 a9df 0ff3 34c0 bb3d  .~.~,.x4....4..=
+00000830: 74e1 47d3 c9f2 0418 c0f5 1abb 06a4 6efd  t.G...........n.
+00000840: 34fc f02c f342 4990 f69a a8e4 f751 2b31  4..,.BI......Q+1
+00000850: 0cb5 15aa 355a e6e3 9381 137f 02e6 af0d  ....5Z..........
+00000860: a71f d969 2974 9429 35a8 559d 8e8f 8390  ...i)t.)5.U.....
+00000870: 86cb bd78 32a5 9c0d df0e 5bf6 360c ff80  ...x2.....[.6...
+00000880: 3fc6 5590 e0d0 27f9 a255 de67 569f 098d  ?.U...'..U.gV...
+00000890: 365d 6239 3dc4 1c08 e483 d3c9 17da 0ff8  6]b9=...........
+000008a0: 5fca ae0f 3850 1419 135d df9b 36fa d8bd  _...8P...]..6...
+000008b0: 2e4f 612b 5be2 e775 3894 9563 e601 a524  .Oa+[..u8..c...$
+000008c0: 7c22 e6bd 1f6e ad7d f98e 0a8d 3911 2369  |"...n.}....9.#i
+000008d0: cdb9 958c 956f e5bc a73f 34f7 4d75 2891  .....o...?4.Mu(.
+000008e0: 3a7c 49fa 26f4 32f2 91f4 f49b 21b4 804c  :|I.&.2.....!..L
+000008f0: 0f5b 1178 3baf b2ce f39b 0d2d 3b2d ff8a  .[.x;......-;-..
+00000900: 301d 54b1 c839 2969 3c0a b25e 76cc 5ed1  0.T..9)i<..^v.^.
+00000910: 1c73 b8fe a7aa 5496 ebad a7ce 3de3 3dde  .s....T.....=.=.
+00000920: ee30 fce9 17ab 3a10 b9cb 365b 625b 9fea  .0....:...6[b[..
+00000930: 3def 1c80 d6b0 cdbc 7ded 1060 4a95 aad6  =.......}..`J...
+00000940: 62ce bb4c 3e52 8de3 bf3e 0e9d eed6 d86d  b..L>R...>.....m
+00000950: 0033 89b7 cb85 84a3 3e5f 999b 65e4 d565  .3......>_..e..e
+00000960: 2911 1ad1 92bf c6de 425c af47 3e69 9a2f  ).......B\.G>i./
+00000970: a996 ddb0 f8b3 f6e1 4432 2091 56f0 2438  ........D2 .V.$8
+00000980: 3eb7 bc56 e4df 97de 4168 f673 d2ad 0c87  >..V....Ah.s....
+00000990: 934a 3c44 3f05 0000 f2c4 5598 557b 2475  .J<D?.....U.U{$u
+000009a0: 49b2 73d1 1881 f3df 3f0c 6fb8 2eb9 cfd9  I.s.....?.o.....
+000009b0: 0542 a8dc 2572 f632 97e5 f65d 3ff6 be70  .B..%r.2...]?..p
+000009c0: 55a7 961c d77e 3ebf c323 2730 223b 51c3  U....~>..#'0";Q.
+000009d0: 40e6 0d18 6d78 d3e8 53df cf06 77ac 1884  @...mx..S...w...
+000009e0: 8e9f 8e58 424a b1c4 93de ac0b 8f36 5f23  ...XBJ.......6_#
+000009f0: f732 fd74 e86a bcad 4471 35ed 9af9 bf37  .2.t.j..Dq5....7
+00000a00: 13da 009f 3875 d0bb 3a2a 9b74 4477 b3e9  ....8u..:*.tDw..
+00000a10: 5a6c 3a22 d991 37b0 0859 53a8 7d7f fe9a  Zl:"..7..YS.}...
+00000a20: 4508 ca52 16d7 d238 30a7 d1ec 0df7 8aa2  E..R...80.......
+00000a30: 6e33 cb40 456b 4288 e355 ea73 6090 7fee  n3.@EkB..U.s`...
+00000a40: 092b b823 35e8 8f80 4580 739d a623 49c6  .+.#5...E.s..#I.
+00000a50: a495 ff9f c82f 8c61 61d3 7161 49cd 9536  ...../.aa.qaI..6
+00000a60: f437 89ff c916 0caa df9a 10e4 3dee 51f4  .7..........=.Q.
+00000a70: 4c06 bf6b 863b e410 bac2 8981 a2a3 8726  L..k.;.........&
+00000a80: fc6c 0f08 4c76 5c8e 185b a58b 2940 0aa0  .l..Lv\..[..)@..
+00000a90: 4159 3efb b06c b0f5 4cf1 a726 2bc2 065d  AY>..l..L..&+..]
+00000aa0: 939f d8ae 1261 957e 48fb ea8b 4d72 18da  .....a.~H...Mr..
+00000ab0: aa31 ae06 9d5d 620a 13c0 bbac 435b 4cbb  .1...]b.....C[L.
+00000ac0: 4da8 26bd a9a8 9d63 e26d 45d1 a21c 3f63  M.&....c.mE...?c
+00000ad0: 7b19 a972 4dd6 6e60 7078 e4a1 3333 8a1c  {..rM.n`px..33..
+00000ae0: 03a6 d316 083d b588 4fad 480f 0c74 0a54  .....=..O.H..t.T
+00000af0: d524 976a cde9 3369 3350 4ff7 50aa 047f  .$.j..3i3PO.P...
+00000b00: d1f7 7bac ba02 28d0 d3e7 a8b3 42cb 24ec  ..{...(.....B.$.
+00000b10: 5217 9473 2a87 4182 d35a d847 eca2 dd45  R..s*.A..Z.G...E
+00000b20: d091 d351 5550 24f2 3d09 12c9 af2c 1ea3  ...QUP$.=....,..
+00000b30: 8653 3abb 2609 efb9 5569 91ac f0e9 2153  .S:.&...Ui....!S
+00000b40: 612e 4b34 ac5f 4290 43e1 1c53 58ff 10c2  a.K4._B.C..SX...
+00000b50: 6e80 dcd2 39c1 c1ef 2758 9904 8e15 56d7  n...9...'X....V.
+00000b60: 5b11 9f7b bc8c 6940 091b 70d3 0c1e a19c  [..{..i@..p.....
+00000b70: 3ae4 e1dc 5b8b 005f aff9 ea30 8819 4373  :...[.._...0..Cs
+00000b80: 0a5f 392f 20d5 bcca 5dd1 ad3c aa9a 991f  ._9/ ...]..<....
+00000b90: e496 20a4 421e 7c98 a062 9eb7 5e88 5b0b  .. .B.|..b..^.[.
+00000ba0: d90d a8c0 3367 3c2d fce1 34ed 7504 b2c9  ....3g<-..4.u...
+00000bb0: 5e97 43b2 7f36 b434 170f ddb6 de8b f4ad  ^.C..6.4........
+00000bc0: c7c3 dcb8 5f9c 46f3 cf03 ba61 f4ca be43  ...._.F....a...C
+00000bd0: 19f1 a8fa 32f7 6548 5fd2 113a 71bb 4036  ....2.eH_..:q.@6
+00000be0: 3ad5 4eec 3a29 cf70 a372 6fa9 5fd2 88d5  :.N.:).p.ro._...
+00000bf0: 2a65 2516 ddd6 fb0e 6952 f3b1 25ef 882c  *e%.....iR..%..,
+00000c00: 6085 3683 f131 2404 c291 6881 ae68 3836  `.6..1$...h..h86
+00000c10: 18ff 2547 60d5 5ede f5c8 f65d a462 0621  ..%G`.^....].b.!
+00000c20: 9f91 e867 6226 693d 61a9 6482 6631 eb4d  ...gb&i=a.d.f1.M
+00000c30: cc3b 1384 57f6 8c8a 8b4e b688 62bb e9e0  .;..W....N..b...
+00000c40: 94c7 f3fd 4f91 6168 8ea0 2dd5 af44 bbab  ....O.ah..-..D..
+00000c50: 6662 1dd8 b841 7b21 b241 ea72 9afe c054  fb...A{!.A.r...T
+00000c60: 7b58 7c4d 671f 9a4b 5dc7 3eda f677 a721  {X|Mg..K].>..w.!
+00000c70: be3f 6fea 219e b94a 6858 aa9c 032c a838  .?o.!..JhX...,.8
+00000c80: 5ef6 b6ed d9e2 3227 12a5 03f8 688d 76ad  ^.....2'....h.v.
+00000c90: 3267 9e92 fe3b d2d3 d14d 43a5 bd26 e0d8  2g...;...MC..&..
+00000ca0: 68bc 17f9 ff21 04a9 d7b6 7770 58bb 4c34  h....!....wpX.L4
+00000cb0: 3ca7 2609 6a17 387d da12 43d1 f09a 807d  <.&.j.8}..C....}
+00000cc0: 5a20 50d6 71e7 5c67 6cf9 c5d5 cec9 654c  Z P.q.\gl.....eL
+00000cd0: 1ba3 d197 a132 fe20 dda9 a243 6d30 3c33  .....2. ...Cm0<3
+00000ce0: e6a8 ea6d 6c16 85fe 429f 2adc 1f64 7a5d  ...ml...B.*..dz]
+00000cf0: 6ddb 754a 665f fafe da03 4d0c 5d84 580d  m.uJf_....M.].X.
+00000d00: 643f ec79 6df8 84a4 8c4f 636a 7703 38fb  d?.ym....Ocjw.8.
+00000d10: d37a d665 9159 b384 6ea9 cb6d 897d 54f8  .z.e.Y..n..m.}T.
+00000d20: fa4d 3d05 bc22 4648 99af 89ee 6f54 adf8  .M=.."FH....oT..
+00000d30: ddd1 87dc 2a54 da6a 9450 03ee f73d 45eb  ....*T.j.P...=E.
+00000d40: 6fa4 a259 671a bd66 bb93 8108 0171 0f4d  o..Yg..f.....q.M
+00000d50: 3226 266e 6ff2 3dcf 38eb 6f5f 6869 0c8a  2&&no.=.8.o_hi..
+00000d60: 7da1 ac79 dc64 cc71 7042 a650 7bbb cd65  }..y.d.qpB.P{..e
+00000d70: bc85 fb9b 8626 dd68 ea23 f250 71e3 b40d  .....&.h.#.Pq...
+00000d80: cca6 a041 4014 fd87 843a 2a1f e4ef be80  ...A@....:*.....
+00000d90: 7429 0546 dae1 1066 6c3e 88fe 2a30 1a93  t).F...fl>..*0..
+00000da0: 55b9 05c1 7596 fa84 bbf1 9980 7aa8 b538  U...u.......z..8
+00000db0: db31 6853 8fbd 118a 75df 5b97 7829 e935  .1hS....u.[.x).5
+00000dc0: 4376 b55b f0cc 34a3 63fd 5b23 7687 73ef  Cv.[..4.c.[#v.s.
+00000dd0: 949d 6014 816b fb1a 88fd e9d0 77f3 5fb6  ..`..k......w._.
+00000de0: 7778 0c7a a96e 36d7 4ecd 984a 4d75 4aaa  wx.z.n6.N..JMuJ.
+00000df0: c916 efd9 77e2 9b0c f476 f1a5 0f47 6d89  ....w....v...Gm.
+00000e00: 819a 9312 d0c7 f5fc 784c 476d c42c 4136  ........xLGm.,A6
+00000e10: 8b6d 1ba1 b910 466e 4926 291a 7903 41eb  .m....FnI&).y.A.
+00000e20: 4499 0c1a af03 1f2f db19 87c4 bf6e 3f6a  D....../.....n?j
+00000e30: 7a87 06d0 7a14 6ddd 6b94 f121 619d 12b0  z...z.m.k..!a...
+00000e40: 4aa3 18dc 7c3f 8495 d70c 3139 0533 997a  J...|?....19.3.z
+00000e50: 83ce 63bd c0fd 4b52 7c6e 75ab 8a2c 040b  ..c...KR|nu..,..
+00000e60: 00d5 9bd2 24d7 2674 59f1 007b 7d9b 1542  ....$.&tY..{}..B
+00000e70: cfe9 4310 f40d b66a f976 51a2 9cdf 2a78  ..C....j.vQ...*x
+00000e80: 7dda 0565 2d3e 0933 f9a2 86c1 c875 d077  }..e->.3.....u.w
+00000e90: 1369 ef76 7e7b 95e1 9c5a 8c33 3e77 1f41  .i.v~{...Z.3>w.A
+00000ea0: f2ae 7ec6 1376 60e3 7edf 096b ac95 8071  ..~..v`.~..k...q
+00000eb0: a9da 9f28 8262 1127 9fd6 cb9d 8028 600f  ...(.b.'.....(`.
+00000ec0: 1523 6a79 58bc 0c6e 4dec cc20 91e9 8a84  .#jyX..nM.. ....
+00000ed0: 802c 28e7 e9d9 119c 315c a80d f1ee cfd1  .,(.....1\......
+00000ee0: 670e a3ef 816a a231 16ce 8311 e612 6cd1  g....j.1......l.
+00000ef0: 5a69 8544 95ca b4dc 8194 4274 f6bf c49e  Zi.D......Bt....
+00000f00: 0e0b b67a 9c81 695c bf90 e0e7 8226 9d5b  ...z..i\.....&.[
+00000f10: 29a5 7cd3 fda0 07c6 c786 d211 19a1 ed23  ).|............#
+00000f20: 84e8 7ef0 838e 2648 a797 c794 924b a192  ..~...&H.....K..
+00000f30: 234d 3f2d 85c0 14e1 400b 943a 1497 8dca  #M?-....@..:....
+00000f40: 028a f980 e93b c00e 862a cd05 bfd2 822b  .....;...*.....+
+00000f50: 4f12 681d 9efb a224 7bbb 1807 8699 1ad6  O.h....${.......
+00000f60: 2983 9978 a859 bca1 d18f 1efc 31e8 57b7  )..x.Y......1.W.
+00000f70: 86f0 2915 7af2 7140 8ecd ef17 7a79 63e9  ..).z.q@....zyc.
+00000f80: 8346 8af9 8817 8c36 ea5d a1f9 15e1 6821  .F.....6.]....h!
+00000f90: 9957 6606 5f5b 6d73 88dd c31d 05ad 8f61  .Wf._[ms.......a
+00000fa0: 3568 8f09 938d bc6c 8737 d3fa 88e6 6128  5h.....l.7....a(
+00000fb0: 8ad6 c373 9f2e 7ff5 914e f372 27e2 a68e  ...s.....N.r'...
+00000fc0: 8951 b1b0 f703 7a49 3d27 5ab0 fec5 9f7d  .Q....zI='Z....}
+00000fd0: 7ebb 0954 8dfd 3318 74ae 3d3c cb5b f773  ~..T..3.t.=<.[.s
+00000fe0: 0862 39d0 e9ee 07b7 8f8a ab00 7ddc 625f  .b9.........}.b_
+00000ff0: 1d2c 8c53 b11c 596c b9e7 bfbe 8fbc 1f9d  .,.S..Yl........
+00001000: ec85 d119 83cd bda2 cca0 194f 49cb bd9d  ...........OI...
+00001010: 9165 546b ddee 6246 bd4e 8ab0 fc32 cf36  .eTk..bF.N...2.6
+00001020: 2bca cb8f 9208 66c0 12c2 5fbb e11d 9f16  +.....f..._.....
+00001030: 2ad2 6b38 6402 190f 920d e909 d079 46eb  *.k8d........yF.
+00001040: 3c8d 8564 b8d8 1b0b 9f79 f6d9 95af 810d  <..d.....y......
+00001050: a5f3 c8a0 0053 7e76 ac19 d601 3180 a30e  .....S~v....1...
+00001060: 966d 853d dfd4 03ca 6d2f c1b0 2ced a83c  .m.=....m/..,..<
+00001070: cf9e 34be 9b32 0284 16f4 ad2c e050 e2bc  ..4..2.....,.P..
+00001080: a50b 3643 bf53 d939 9bd4 414f 9100 287c  ..6C.S.9..AO..(|
+00001090: c7cc b134 a801 69fe 6be6 f013 9c37 669c  ...4..i.k....7f.
+000010a0: fc00 9427 5882 a966 bc95 f449 ddb1 90aa  ...'X..f...I....
+000010b0: 9d47 933c 7bda c7e1 44c7 9988 b39f cc09  .G.<{...D.......
+000010c0: 0afd 02ca 9e9b 32e6 1733 4a73 337a ba1a  ......2..3Js3z..
+000010d0: 8aef ff4f d4ba 38a6 a0b7 1932 6868 e0e7  ...O..8....2hh..
+000010e0: 1536 4ced e59f 4db3 0591 d846 a1ac 4ed2  .6L...M....F..N.
+000010f0: cfed 865b c368 7980 3a3b a1ba 531c c53d  ...[.hy.:;..S..=
+00001100: a285 ae6d 645e f9a5 b7e0 055c 3d58 8af7  ...md^.....\=X..
+00001110: 85e2 9dda a2bb 54fe 8acf 2a8c 6d15 0c5c  ......T...*.m..\
+00001120: 0e89 b983 f721 ee0e a3ec 8691 03d2 e3dc  .....!..........
+00001130: 18fb 5930 3123 9f5c abf3 be1e a42a 39aa  ..Y01#.\.....*9.
+00001140: 0aae 12ca 3dfb fa82 ad50 7cce 0a2c 2df1  ....=....P|..,-.
+00001150: a591 f756 00d9 ff2a bb7a d6ec 6aa8 2b9e  ...V...*.z..j.+.
+00001160: 3c11 26d0 a5a5 1843 0b76 0fc3 ce3e 0834  <.&....C.v...>.4
+00001170: cf90 79db cfb6 da1f a6ba a636 d0f5 3143  ..y........6..1C
+00001180: 269b 968c 58c3 6819 8b91 0bf5 a7f3 a641  &...X.h........A
+00001190: d9ea 72f5 1911 b41c 4f99 6ad4 7230 00a2  ..r.....O.j.r0..
+000011a0: a841 8e57 a4e8 a6f2 8cec 8a95 04e5 f9e7  .A.W............
+000011b0: b4a3 1bba a852 e343 4638 f815 4709 3243  .....R.CF8..G.2C
+000011c0: 23dc d6ef e909 0a67 a86e 13e3 567f d165  #......g.n..V..e
+000011d0: 1199 e0be 5716 6bb8 a88c a5cf a93f f7af  ....W.k......?..
+000011e0: 535e 15fb 644a 3da6 ca21 d496 bc98 0e87  S^..dJ=..!......
+000011f0: a94c e1a1 b2d8 d1db da64 dce5 6418 8f74  .L.......d..d..t
+00001200: 480f 2f03 a94e d9b1 8b51 adb0 4a3e 0250  H./..N...Q..J>.P
+00001210: d016 41f8 03b1 6b4a aa3f af30 45dc f6d8  ..A...kJ.?.0E...
+00001220: 0fd4 24b2 10d0 2aee 0b24 76d4 aa6c aa64  ..$...*..$v..l.d
+00001230: 5ee6 6d82 20e4 8946 6e95 585c b428 ace8  ^.m. ..Fn.X\.(..
+00001240: aa96 92c2 4e2c d742 be01 6017 53e0 64b3  ....N,.B..`.S.d.
+00001250: 589c 4285 aae1 7c32 0706 3f00 2655 22ea  X.B...|2..?.&U".
+00001260: 7fcd 1ef9 71cc cc85 ab44 4fae c380 805a  ....q....DO....Z
+00001270: f86f 23bb 673c 8094 1d07 b847 ad00 c606  .o#.g<.....G....
+00001280: d0e3 aa41 0ff0 dd50 9938 282b 21c0 2d45  ...A...P.8(+!.-E
+00001290: afb8 bfa3 153b c2d7 9b4c ca8b 8c7d ec66  .....;...L...}.f
+000012a0: d816 979f b0e6 a5a3 137b 7fe6 8f10 77fc  .........{....w.
+000012b0: a0f7 95f1 d89d d24e b0ef 7617 668e 1a3d  .......N..v.f..=
+000012c0: bf36 4ce6 4b25 214b 96b1 8b22 b14e 1c10  .6L.K%!K...".N..
+000012d0: 9ef6 582a 30f9 1b6f fc27 2af2 5418 7b7e  ..X*0..o.'*.T.{~
+000012e0: b2cb 8072 2c6d 0e61 4ca6 4214 6f34 86a1  ...r,m.aL.B.o4..
+000012f0: cb84 55c6 b525 32ad cf7e 7245 a9d3 0908  ..U..%2..~rE....
+00001300: 0a1c 8d5f 8269 1be1 b69f 2b64 4291 26cb  ..._.i....+dB.&.
+00001310: db65 bdfc f8fb 74d2 563a 78b4 b6d2 6cfe  .e....t.V:x...l.
+00001320: 0653 baba 78b0 8eef b82e be57 069f 3e84  .S..x......W..>.
+00001330: b774 aec3 980b 1fea f8ad bdec 34b8 b5e7  .t..........4...
+00001340: 49d9 f489 b79a 7def 50be eb46 660f d51f  I.....}.P..Ff...
+00001350: 8165 7f26 02a4 d2a1 b812 2b62 0dc6 fd61  .e.&......+b...a
+00001360: 6c4a 7c45 3259 9ffb ce82 a4ff b8ec 5c4a  lJ|E2Y........\J
+00001370: 53ed 4d65 40aa 9b08 ad82 2e7f 1ae3 4c03  S.Me@.........L.
+00001380: b96d 623a 82de 0268 3fc6 762b 21a9 7d57  .mb:...h?.v+!.}W
+00001390: b65f eb5d bbf3 07ff 3ce7 2e6c f8df 49bc  ._.]....<..l..I.
+000013a0: 07ab 19ea c8f0 bf6b bce0 4f51 51ef c1d9  .......k..OQQ...
+000013b0: 5de9 5f9a 82e8 e8e5 5308 eb62 bcfb 8940  ]._.....S..b...@
+000013c0: 46e6 e2bb 40c0 2520 721d ec5b a4ed 4f94  F...@.% r..[..O.
+000013d0: be9d c361 7df9 314c d5e8 cc20 d6fb 7d71  ...a}.1L... ..}q
+000013e0: 5b86 c3a9 bebc 19a2 8531 46d8 6974 fc1a  [........1F.it..
+000013f0: 5496 a8ec afc0 7001 bff7 7398 1b53 4d2d  T.....p...s..SM-
+00001400: 283a eeaf 4f13 5954 5412 8151 c1a3 cd27  (:..O.YTT..Q...'
+00001410: 5bed 2f28 b18d a9c9 d954 6783 4f19 51a3  [./(.....Tg.O.Q.
+00001420: c2b5 d1ac f4af 894f 5fa8 9064 c006 b13f  .......O_..d...?
+00001430: 1c5c d512 c2c3 39d9 8466 e36a 3512 afe2  .\....9..f.j5...
+00001440: 7281 c649 72bc 5c43 c497 2490 7117 db59  r..Ir.\C..$.q..Y
+00001450: 238d 10d2 8d6d 1139 0b77 a68d c4ce b708  #....m.9.w......
+00001460: ba86 0a5d 0efe c766 1978 e1f4 8881 da70  ...]...f.x.....p
+00001470: c5b9 7d08 7ae2 32f4 124b 062d 8d25 f6a6  ..}.z.2..K.-.%..
+00001480: 99db 7adc c63a 6859 9674 c77f c43f ba7a  ..z..:hY.t...?.z
+00001490: c193 52d0 a6c0 c961 c723 b47d 51d7 5a6a  ..R....a.#.}Q.Zj
+000014a0: d656 299e ba5e 6a86 482a 3ba6 c792 6ae6  .V)..^j.H*;...j.
+000014b0: 0405 f5b2 43d9 b4ef ee3b 601c d7f2 626d  ....C....;`...bm
+000014c0: c7f5 d105 2f93 504b ff55 27db 3bb2 f4a8  ..../.PK.U'.;...
+000014d0: 619c d566 c8b0 cac0 8185 4d01 38b4 9d3f  a..f......M.8..?
+000014e0: 0e56 3aef ea99 2dd1 c8f0 0699 181e 53ff  .V:...-.......S.
+000014f0: 0551 2a20 58d0 9910 00ff 2e75 c93f 88bc  .Q* X......u.?..
+00001500: db0e 6cd8 f7dd 75d1 869f e4ca 33c2 b743  ..l...u.....3..C
+00001510: cafc ce98 5b49 bb24 1488 dee9 f590 0a56  ....[I.$.......V
+00001520: 2524 4985 cb20 3784 ebeb d5e6 885a e698  %$I.. 7......Z..
+00001530: 22ca a8d8 cfaf 4ed4 cc32 fb60 a921 776f  ".....N..2.`.!wo
+00001540: 4ffe 97f1 a718 dbbf 8951 20b0 cd94 0740  O........Q ....@
+00001550: 6aab 7801 64e2 cfdb 10cb 6082 e92f 4ab2  j.x.d.....`../J.
+00001560: cf74 1b81 bc74 61bc b592 c215 2ee6 27b3  .t...ta.......'.
+00001570: 1b80 2157 cfca 8f83 da3c f40a c8ca 0813  ..!W.....<......
+00001580: f8e9 1aa6 1918 155d d235 4ba5 ef0d 2041  .......].5K... A
+00001590: 7c4b d318 5238 9ddb cf11 f5bf d240 4d7c  |K..R8.......@M|
+000015a0: 2381 a079 3332 8add 2a3f 55c0 5757 a598  #..y32..*?U.WW..
+000015b0: d2b1 291e 883c 3f9d 5692 733d 17ec ce23  ..)..<?.V.s=...#
+000015c0: 70c4 0e78 d3e9 c40d c20d b746 44a1 10c2  p..x.......FD...
+000015d0: 65ba cac2 c832 9d36 d564 cd08 2d74 81d5  e....2.6.d..-t..
+000015e0: a8b0 406a 7431 78ee 1be1 7406 d6ed da2a  ..@jt1x...t....*
+000015f0: 8d75 6ab3 1c9e bf94 4cb0 3990 4542 2a7b  .uj.....L.9.EB*{
+00001600: d77b b103 3a9d 51fb 0861 9c8b 6386 0e57  .{..:.Q..a..c..W
+00001610: e10a 11b1 d967 f0e3 518a 5b57 926e d042  .....g..Q.[W.n.B
+00001620: 290d 1032 c14e 2e5a daff 91bd a246 920d  )..2.N.Z.....F..
+00001630: dfef c4d4 f2f2 2860 2525 d26a db80 a150  ......(`%%.j...P
+00001640: 3755 7412 42c1 8617 a5e0 6dc5 b9a9 cee5  7Ut.B.....m.....
+00001650: db9b 66f1 c32b 9c01 349e c0e7 11a0 cb71  ..f..+..4......q
+00001660: b487 cee9 dd4f 663d 5c7c b396 1e68 d656  .....Of=\|...h.V
+00001670: ea13 8f83 1b20 2429 dd75 b6da edbd 78f3  ..... $).u....x.
+00001680: 5e08 3b4d e818 3fb2 c722 bf13 de30 f0b3  ^.;M..?.."...0..
+00001690: c514 2b03 458b ae01 58bb 69a0 0bb2 d57b  ..+.E...X.i....{
+000016a0: de41 62dd 1943 3851 ae15 c7f9 1a9d 74b8  .Ab..C8Q......t.
+000016b0: 9566 4057 de4a ac57 d4b7 7be4 2a82 adf9  .f@W.J.W..{.*...
+000016c0: 755d 4eb7 11ca f8c0 de91 dcae 25aa c7d3  u]N.........%...
+000016d0: 0294 3c70 45f9 80ab 35dd cb48 dee3 c25b  ..<pE...5..H...[
+000016e0: e088 ed87 1b0b bcd8 be9f 490c 5c81 0ac2  ..........I.\...
+000016f0: e04d 74a1 48a5 3b66 0bed e3bb 1d3d 2649  .Mt.H.;f.....=&I
+00001700: a5b9 0334 e04f 9606 19cc 7622 3f68 7115  ...4.O....v"?hq.
+00001710: d0c1 9232 42a3 6898 e09e 50a6 b199 3437  ...2B.h...P...47
+00001720: a769 501c b4e2 695a 56e2 5fed e0a4 09e6  .iP...iZV._.....
+00001730: 9964 0445 6c4e 2da8 c700 492d 811d 1f9d  .d.ElN-...I-....
+00001740: e189 ae1a 43a9 9f66 2334 f82b d815 068c  ....C..f#4.+....
+00001750: d496 7b38 e1d6 8ffc 007d e403 4742 712a  ..{8.....}..GBq*
+00001760: f72a 0352 3ef3 70fe e247 eeb0 629d c5d9  .*.R>.p..G..b...
+00001770: 881e fe68 441c 79ff ea8f 885f e285 6269  ...hD.y...._..bi
+00001780: 9fe1 a2ee 1c4f 5d4b 3232 95c2 3ae2 697b  .....O]K22..:.i{
+00001790: e4c1 4033 551e 6292 dbbc 2a4b e443 c33a  ..@3U.b...*K.C.:
+000017a0: 3b04 f9ae e4e2 d206 a214 b26d 103d 53e1  ;..........m.=S.
+000017b0: be4f fcf9 57e4 27db e53e f57d a109 9e80  .O..W.'..>.}....
+000017c0: 4f70 08f7 cd4e 8879 817d 364e e610 b3d7  Op...N.y.}6N....
+000017d0: a44e b79c be09 9d27 f245 448c 5ecd bf09  .N.....'.ED.^...
+000017e0: e69d e29b b2d1 d643 4b8b 29ae 775a d8c2  .......CK.).wZ..
+000017f0: e48c 5391 e6fc 34af 4a8f 603b 4cf8 40ea  ..S...4.J.`;L.@.
+00001800: 342d de03 c0a8 5d82 e794 4e14 a44e 60c6  4-....]...N..N`.
+00001810: a68b 29fc 4b31 50b7 680a aeb4 e7dc 7a7b  ..).K1P.h.....z{
+00001820: d3ae 99e9 e704 fd03 1de9 1dcb c5cd 116f  ...............o
+00001830: e878 21b4 2c4c b6ca 6081 e64d b74a 7786  .x!.,L..`..M.Jw.
+00001840: cf68 1fee e898 8aec 01e6 5c99 9109 5098  .h........\...P.
+00001850: 0230 9bc2 a781 5db8 e940 4fa4 7750 2176  .0....]..@O.wP!v
+00001860: ac80 b88b e458 3a1e a305 a5bf e968 e86b  .....X:......h.k
+00001870: f3d2 83f4 8e4c b483 cb8a e9a7 5178 9486  .....L......Qx..
+00001880: ea9d c1ad cbee 374b f5b9 01a5 f11a 3c97  ......7K......<.
+00001890: 37b0 518e eb87 9404 f6d7 d489 daae 129f  7.Q.............
+000018a0: dba9 26f6 7f8c 7708 ed08 b5df b70e 776c  ..&...w.......wl
+000018b0: 72b4 3c7e 5e90 509f 9566 a32e ed4f a920  r.<~^.P..f...O. 
+000018c0: f22b 6acc 55c9 6d41 94d1 078b ee9b 70a5  .+j.U.mA......p.
+000018d0: efc3 ac6e 98c7 b60a c84a 08a2 aaa2 4a74  ...n.....J....Jt
+000018e0: 6617 8746 f14f 5656 1893 a634 b60e 0239  f..F.OVV...4...9
+000018f0: 9b6f 0e02 d871 d7e3 f24f 57b3 eb80 39e1  .o...q...OW...9.
+00001900: c8d3 e423 0a6a 0697 92ea b5f3 f390 ef81  ...#.j..........
+00001910: b1a8 96ac 8b8e c388 e189 7125 a537 24be  ..........q%.7$.
+00001920: f413 32fd c472 1eea cbd7 ccd6 e5ac c6c9  ..2..r..........
+00001930: 90dd 2d7f f633 edd3 c761 2dcc 4ede 3aff  ..-..3...a-.N.:.
+00001940: 172a e7a0 fb6a 1705 f69a 178a fddf a735  .*...j.........5
+00001950: 0b5c 5778 0399 cccc ff00 650f f780 9474  .\Wx......e....t
+00001960: 0a29 a0b2 e1ec a234 2d21 2905 402a 677e  .).....4-!).@*g~
+00001970: f876 9eb1 087c 7f09 03c4 2e41 52d7 637a  .v...|.....AR.cz
+00001980: 79b6 d343 f919 8185 c34c 1115 7c41 1ac3  y..C.....L..|A..
+00001990: a3d1 e9a4 4454 67d1 f95a 6816 826e 3b6c  ....DTg..Zh..n;l
+000019a0: c5a2 909e f8ae f549 d07a 84b0 f98a 9ff7  .......I.z......
+000019b0: dbca 4e98 b5ba 343a 83cd 588a 0d29 54a5  ..N...4:..X..)T.
+000019c0: fb33 3acb 04fc 9d25 7ad4 3dcf f4e3 b1c2  .3:....%z.=.....
+000019d0: e1ce 95df fb90 5390 dc36 462c fb3a f0a3  ......S..6F,.:..
+000019e0: 035b c1a0 923d 02ba fc56 84df f4f8 5978  .[...=...V....Yx
+000019f0: 212a dbca 6f0e f241 f92c 2cf0 fcfc 9c8a  !*..o..A.,,.....
+00001a00: 4db8 095a 6332 0df9 cee4 7eb8 282c c2e9  M..Zc2....~.(,..
+00001a10: fe68 d259 df55 0d5a 694b 5594 fbc4 7017  .h.Y.U.ZiKU...p.
+00001a20: 98b0 ba57 3c0e 5daa 9426 b1d2 3df4 1a63  ...W<.]..&..=..c
+00001a30: c4bb 041f cfba 267d 1d67 7dcd b25a 2cdf  ......&}.g}..Z,.
+00001a40: 3f67 91b8 d6d7 7a9d 5530 8271 1336 5390  ?g....z.U0.q.6S.
+00001a50: b768 d554 4a23 b09c 22b0 5574 d6e2 99c5  .h.TJ#..".Ut....
+00001a60: 04db b713 cf23 151c 737c 9258 8d07 2601  .....#..s|.X..&.
+00001a70: 0a28 ab1a c0ee 48ae fd47 cc89 ec27 31e1  .(....H..G...'1.
+00001a80: 0f47 3bf3 23aa 9ebb 83f8 c87d 5312 ffa3  .G;.#......}S...
+00001a90: eb9a c438 402c f3ac 6756 8645 f024 d6c8  ...8@,..gV.E.$..
+00001aa0: 5246 fcc0 0645 6b74 7b52 f34d 3461 2371  RF...Ekt{R.M4a#q
+00001ab0: 65a0 e4f2 e34d 9b21 b5c8 f238 569c efaf  e....M.!...8V...
+00001ac0: 112e eaef c9b8 27fd c2cd ecd0 956b 1e14  ......'......k..
+00001ad0: d8a0 76c5 492d 8bf7 4ccc b391 999f 6fee  ..v.I-..L.....o.
+00001ae0: f2be e2ff 7070 5294 5aa6 36f8 613a 8038  ....ppR.Z.6.a:.8
+00001af0: fa3b fca6 0315 132f a30b 9315 3cfa 101d  .;...../....<...
+00001b00: f60a 0874 49f3 a895 29f1 e562 fc75 b350  ...tI...)..b.u.P
+00001b10: bb13 fbb9 ca09 5e5a 2c8c 2670 609d 373d  ......^Z,.&p`.7=
+00001b20: 3f98 3a9a 84ec fd1d d38c a8d1 04f7 4eef  ?.:...........N.
+00001b30: e97d 11ea 94e4 d657 cbc6 8a7e ddd3 deaf  .}.....W...~....
+00001b40: 5529 0a01 732b 49a2 01ba 81fc a651 efa8  U)..s+I......Q..
+00001b50: 9a6f ad68 ec0d d7af 8a97 a427 38d1 2009  .o.h.......'8. .
+00001b60: 6695 2349 efb1 5d0e 4fc9 7768 66bd 11c6  f.#I..].O.whf...
+00001b70: b565 6cca ed05 99c8 f3ca 5737 5bc7 6aca  .el.......W7[.j.
+00001b80: c5fe e67b d1d8 d598 d0c2 2407 0196 52de  ...{......$...R.
+00001b90: 4ea7 6d6b 273f 0ea9 6209 bda7 8ee6 37fb  N.mk'?..b.....7.
+00001ba0: 507e 3d8e 593a 8740 08dd 9b59 14ca 5bc0  P~=.Y:.@...Y..[.
+00001bb0: 730d 45cb 1c68 c80e 42aa 568c 4259 a81f  s.E..h..B.V.BY..
+00001bc0: 9e19 6fe7 148c 94f0 2f48 fc5f 93de cdd4  ..o...../H._....
+00001bd0: 0b3f 7b6c bb2d f6ca df49 556b cf2f 05a4  .?{l.-...IUk./..
+00001be0: 908e c271 ed26 1fff 951f 36f3 7047 ee9b  ...q.&....6.pG..
+00001bf0: d5e4 ece0 feae f4cf fbdd ccf5 cc05 6a9e  ..............j.
+00001c00: 2f8b 42f2 1f5f ca18 d2ba a998 5ee5 3f04  /.B.._......^.?.
+00001c10: c485 dbfc 1e63 d883 be19 3a75 b619 668d  .....c....:u..f.
+00001c20: 24bd 1f12 d6d4 a821 45ce ca4c 838b 6d35  $......!E..L..m5
+00001c30: cf74 ee9a 8214 25f2 1bde f2cd 99b2 a41f  .t....%.........
+00001c40: a3e9 41a5 af5c 4816 fc27 d410 f8af df30  ..A..\H..'.....0
+00001c50: 3b33 fa1b 2e6e 00ce 9568 b83c 6b88 504a  ;3...n...h.<k.PJ
+00001c60: b020 229e 2997 8e76 231b db3d 97f5 f4be  . ".)..v#..=....
+00001c70: 9e8d e866 aae3 2f4a 7f6d f04b 48b6 bdfe  ...f../J.m.KH...
+00001c80: 7315 c5ee 5dfa cd90 0e9b d730 b196 7ee7  s...]......0..~.
+00001c90: 67a0 1e7e bd39 7464 2da8 393e f245 3e14  g..~.9td-.9>.E>.
+00001ca0: a975 ef48 35cd f071 c7fb d20f fe73 124a  .u.H5..q.....s.J
+00001cb0: 25a0 317c 63e9 ba03 3741 c5e7 6a57 0f44  %.1|c...7A..jW.D
+00001cc0: 449c 8ab6 007f f2f4 f28d 8428 14a1 c3b5  D..........(....
+00001cd0: 2d5c 0128 9d75 8d06 f55c a45f 9665 d5bf  -\.(.u...\._.e..
+00001ce0: 330b c910 a597 dff1 6ab1 1a13 20c3 be01  3.......j... ...
+00001cf0: b363 46e9 ab9c 6877 5def 3901 fef3 efff  .cF...hw].9.....
+00001d00: a9e9 c093 45a9 96d7 0071 c4f6 3fad 593f  ....E....q..?.Y?
+00001d10: a411 a5fb ee7f 350f 978d 830b bd5e 6b33  ......5......^k3
+00001d20: 8dbd b39c 5d6a 6b8e 2442 6a12 aa89 132b  ....]jk.$Bj....+
+00001d30: b403 1cdc 1338 e146 bb90 c89b 0dc5 c21d  .....8.F........
+00001d40: b772 ddf5 950b 9fa1 0de2 b65f b211 a7fc  .r........._....
+00001d50: ddf2 d39d 16ed 4d3b 9034 3a6e eb26 8c09  ......M;.4:n.&..
+00001d60: 6d69 11a9 0dbd 538e 1d3b a937 b88d e288  mi....S..;.7....
+00001d70: d453 98ec d465 f2e0 f1e0 3760 76a6 b227  .S...e....7`v..'
+00001d80: e793 ef4e 9b97 9a79 494e d527 43b2 eb5b  ...N...yIN.'C..[
+00001d90: f5ee 0530 6596 e541 c783 2f05 d025 6a19  ...0e..A../..%j.
+00001da0: 677b 2478 c00c 3b06 6f70 ddeb 58aa 76c5  g{$x..;.op..X.v.
+00001db0: f04d 19c8 ed5d 801d 4760 ff5c 3c4f 72c5  .M...]..G`.\<Or.
+00001dc0: 6a1a 79dc 7ec5 6e92 4763 101c 0de2 586d  j.y.~.n.Gc....Xm
+00001dd0: 99d2 c97f 63ab 660f d876 5cfe 4bab 64f6  ....c.f..v\.K.d.
+00001de0: 01de f13e 5f41 c86d 2b26 ff96 f929 573f  ...>_A.m+&...)W?
+00001df0: cd5b 07fd dd22 b101 cbe0 beca cb26 c754  .[...".......&.T
+00001e00: e831 85ec e57c 2e66 7fee 2ec4 ca6d 7a25  .1...|.f.....mz%
+00001e10: 70d0 897b 23fc dffd 6db7 d623 6e76 0029  p..{#...m..#nv.)
+00001e20: e139 aaf6 df9e 26be b988 54aa 9fb3 a55e  .9....&...T....^
+00001e30: cb2c 19bc 9bbc f8e7 ff76 0474 1983 93cf  .,.......v.t....
+00001e40: a0a5 4164 96c8 2e24 1e63 c464 55cc 7aec  ..Ad...$.c.dU.z.
+00001e50: f2bf 1da9 e4c5 e7ca f192 48e6 8a50 bd94  ..........H..P..
+00001e60: 6037 1d46 d27a bb29 ca2b 00a7 c218 0cee  `7.F.z.).+......
+00001e70: a416 fa59 038a 9293 3196 cee6 2efd 63a0  ...Y....1.....c.
+00001e80: 0e77 75b2 44c0 d7e1 c994 c26c 1a45 e0a4  .wu.D......l.E..
+00001e90: 0000 b4c8 0000 3d92 0000 3609 0000 3cf8  ......=...6...<.
+00001ea0: 0000 46d4 0000 e4d5 0000 ef2c 0000 b37f  ..F........,....
+00001eb0: 0000 d6b5 0000 7932 0000 97f7 0000 9989  ......y2........
+00001ec0: 0000 73da 0000 ed48 0000 27c8 0000 affb  ..s....H..'.....
+00001ed0: 0000 875b 0000 36fd 0000 e3c0 0000 43a0  ...[..6.......C.
+00001ee0: 0000 d9da 0000 9c8d 0000 9558 0000 790a  ...........X..y.
+00001ef0: 0000 ac3e 0000 0904 0000 1e3f 0000 af3e  ...>.......?...>
+00001f00: 0000 93d1 0000 d7f9 0000 d93f 0000 b341  ...........?...A
+00001f10: 0000 e430 0000 3a7c 0000 4774 0000 ef43  ...0..:|..Gt...C
+00001f20: 0000 2ea3 0000 8b39 0000 095d 0000 8464  .......9...]...d
+00001f30: 0000 068c 0000 2631 0000 3645 0000 0e58  ......&1..6E...X
+00001f40: 0000 dec6 0000 e394 0000 e351 0000 893a  ...........Q...:
+00001f50: 0000 2c26 0000 b818 0000 9334 0000 3fdc  ..,&.......4..?.
+00001f60: 0000 8911 0000 b058 0000 8be9 0000 47d8  .......X......G.
+00001f70: 0000 0a01 0000 8a45 0000 8a97 0000 7944  .......E......yD
+00001f80: 0000 6e9a 0000 2bf0 0000 b24e 0000 b487  ..n...+....N....
+00001f90: 0000 ba95 0000 3fb9 0000 9970 0000 078f  ......?....p....
+00001fa0: 0000 ef14 0000 bac6 0000 e8e4 0000 9a51  ...............Q
+00001fb0: 0000 01f8 0000 3387 0000 bb38 0000 e5c0  ......3....8....
+00001fc0: 0000 4220 0000 be66 0000 05b7 0000 7484  ..B ...f......t.
+00001fd0: 0000 ae30 0000 3c3e 0000 4017 0000 33fb  ...0..<>..@...3.
+00001fe0: 0000 93b1 0000 91ce 0000 a5d5 0000 0930  ...............0
+00001ff0: 0000 efc6 0000 32d8 0000 dff3 0000 3d0d  ......2.......=.
+00002000: 0000 9b50 0000 3dc7 0000 3b82 0000 b026  ...P..=...;....&
+00002010: 0000 9a23 0000 da7b 0000 91a2 0000 be7c  ...#...{.......|
+00002020: 0000 a489 0000 3bf3 0000 a561 0000 98d9  ......;....a....
+00002030: 0000 ad8f 0000 995d 0000 b1af 0000 877c  .......].......|
+00002040: 0000 368e 0000 b0cc 0000 b4b5 0000 3a3c  ..6...........:<
+00002050: 0000 e0cb 0000 00af 0000 36e5 0000 aa35  ..........6....5
+00002060: 0000 aaaf 0000 48c3 0000 c1aa 0000 a167  ......H........g
+00002070: 0000 ef90 0000 e4aa 0000 ab53 0000 3ac2  ...........S..:.
+00002080: 0000 b171 0000 ef5a 0000 4360 0000 4aaf  ...q...Z..C`..J.
+00002090: 0000 b199 0000 e2cb 0000 03dc 0000 08b3  ................
+000020a0: 0000 86b1 0000 0369 0000 4333 0000 e10e  .......i..C3....
+000020b0: 0000 dbfb 0000 3b07 0000 9742 0000 c4da  ......;....B....
+000020c0: 0000 77f4 0000 2bbb 0000 9d04 0000 2503  ..w...+.......%.
+000020d0: 0000 4d35 0000 afd3 0000 1ee2 0000 3439  ..M5..........49
+000020e0: 0000 e402 0000 34f9 0000 79a9 0000 937e  ......4...y....~
+000020f0: 0000 940a 0000 0ad9 0000 4824 0000 9a65  ..........H$...e
+00002100: 0000 af11 0000 24d7 0000 425e 0000 c808  ......$...B^....
+00002110: 0000 e615 0000 1e2d 0000 8340 0000 4273  .......-...@..Bs
+00002120: 0000 1e71 0000 2fb4 0000 e1ad 0000 d5a6  ...q../.........
+00002130: 0000 d688 0000 96e5 0000 9505 0000 12c1  ................
+00002140: 0000 e7c4 0000 9130 0000 e209 0000 7866  .......0......xf
+00002150: 0000 2491 0000 000c 0000 47b9 0000 a5b6  ..$.......G.....
+00002160: 0000 0e14 0000 03a6 0000 94ae 0000 d89c  ................
+00002170: 0000 e5e8 0000 11c2 0000 331e 0000 0764  ..........3....d
+00002180: 0000 05f2 0000 2e00 0000 0ab7 0000 dce2  ................
+00002190: 0000 0a7a 0000 83ad 0000 cb33 0000 b298  ...z.......3....
+000021a0: 0000 26aa 0000 ce62 0000 94db 0000 e46d  ..&....b.......m
+000021b0: 0000 e24b 0000 d18f 0000 af69 0000 e54d  ...K.......i...M
+000021c0: 0000 41dd 0000 2667 0000 972f 0000 ad48  ..A...&g.../...H
+000021d0: 0000 9ba7 0000 258e 0000 2703 0000 ad1c  ......%...'.....
+000021e0: 0000 36a2 0000 3457 0000 d757 0000 428b  ..6...4W...W..B.
+000021f0: 0000 26e7 0000 7997 0000 d497 0000 9837  ..&...y........7
+00002200: 0000 8bce 0000 7892 0000 0a37 0000 abee  ......x....7....
+00002210: 0000 7d1e 0000 470a 0000 83da 0000 a5a3  ..}...G.........
+00002220: 0000 2566 0000 ed20 0000 95ff 0000 413a  ..%f... ......A:
+00002230: 0000 9b0a 0000 8bb8 0000 9b91 0000 96a2  ................
+00002240: 0000 3d75 0000 e16a 0000 d4cb 0000 3db0  ..=u...j......=.
+00002250: 0000 a242 0000 9c60 0000 3cb6 0000 40ea  ...B...`..<...@.
+00002260: 0000 b09d 0000 9bc0 0000 7466 0000 9214  ..........tf....
+00002270: 0000 05db 0000 4115 0000 9823 0000 8f61  ......A....#...a
+00002280: 0000 2e32 0000 a8f7 0000 aaa6 0000 279f  ...2..........'.
+00002290: 0000 90ee 0000 d4f9 0000 dd7d 0000 975d  ...........}...]
+000022a0: 0000 023b 0000 991c 0000 7cee 0000 3b47  ...;......|...;G
+000022b0: 0000 88c4 0000 e30e 0000 b276 0000 3000  ...........v..0.
+000022c0: 0000 8b7c 0000 741c 0000 922d 0000 e28e  ...|..t....-....
+000022d0: 0000 9fc3 0000 8f23 0000 b07e 0000 e58a  .......#...~....
+000022e0: 0000 77c4 0000 e511 0000 3237 0000 8363  ..w.......27...c
+000022f0: 0000 40be 0000 db60 0000 6b03 0694 3882  ..@....`..k...8.
+00002300: 1218 a77c 1378 81c8 0226 39fb 9c2f 8ee4  ...|.x...&9../..
+00002310: 9d65 df89 e0fc c608 f525 5226 d379 8f46  .e.......%R&.y.F
+00002320: 1edb 0a44                                ...D
```

### Comparing `gpt_computer_assistant-0.5.5/.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.pack` & `gpt_computer_assistant-0.5.6/.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.pack`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 5041 434b 0000 0002 0000 0111 910e 789c  PACK..........x.
+00000000: 5041 434b 0000 0002 0000 011b 910e 789c  PACK..........x.
 00000010: 8dcb 310e c230 0c40 d13d a7f0 8e84 1237  ..1..0.@.=.....7
 00000020: 711a 0921 0103 5c23 4e1c daa1 2d2a 2e5c  q..!..\#N...-*.\
 00000030: 9f1e 813f ffa7 ab08 74cd 166a dca3 702a  ...?....t..j..p*
 00000040: ad26 1b3c e6be 160c 111b 7598 a284 46a1  .&.<......u...F.
 00000050: 9a57 5e65 5660 2b2d 928b 44bd b8dc 556e  .W^eV`+-..D...Un
 00000060: 1df9 22e4 1903 3acf 89d8 f58c 68f2 a6c3  .."...:.....h...
 00000070: b2c2 7dd4 c7c6 7029 3a2e f31b ae8b c2e9  ..}...p):.......
@@ -3429,356 +3429,413 @@
 0000d640: 4b33 8b52 7353 f34a 8af5 4a2a 4a18 6af2  K3.RsS.J..J*J.j.
 0000d650: 4a57 77e9 b070 335c 9d7d 49e5 ba5a 49e4  JWw..p3\.}I..ZI.
 0000d660: 4786 6aa8 dae2 d492 d202 bd82 4a86 4387  G.j.........J.C.
 0000d670: 2d6f b6a4 3dce 3215 5aff a8a8 f198 67d1  -o..=.2.Z.....g.
 0000d680: 9e18 6700 101c 5e1c ee01 8062 789c 011e  ..g...^....bx...
 0000d690: 00e1 ffe6 01e6 0190 5a14 a591 f756 00d9  ........Z....V..
 0000d6a0: ff2a bb7a d6ec 6aa8 2b9e 3c11 26d0 916e  .*.z..j.+.<.&..n
-0000d6b0: 78e9 000e de91 0e78 9c8d 8d41 0ec2 2010  x......x...A.. .
-0000d6c0: 00ef bc62 ef26 0d2c a52c 8931 510f fa0d  ...b.&.,.,.1Q...
-0000d6d0: a08b eda1 ada1 5bfd be3c c139 cf64 a432  ......[..<.9.d.2
-0000d6e0: 03c6 1eb1 7049 4153 f6ce 8571 c4e2 cd40  ....pIAS...q...@
-0000d6f0: 5cb2 f594 c893 4b71 40f5 8e95 5701 a3d1  \.....Kq@...W...
-0000d700: 1987 269b 1c42 f11e 2da5 9e06 6d13 eb1e  ..&..B..-...m...
-0000d710: 5374 8436 9a40 2a1e 326d 151e b33c 8f04  St.6.@*.2m...<..
-0000d720: d72c f3b6 ee70 db04 ce17 30ed 107c d096  .,...p....0..|..
-0000d730: e0a4 1b2a 6fcb 328b f0df 81ba 4f71 7df1  ...*o.2.....Oq}.
-0000d740: 081f ae7b 3361 3d96 d4f2 ef2c 137c 74e7  ...{3a=....,.|t.
-0000d750: 3aa7 7e3c 0640 b391 0e78 9c8d cb4d 0e82  :.~<.@...x...M..
-0000d760: 3010 40e1 7d4f 317b 1332 ed50 da26 c644  0.@.}O1{.2.P.&.D
-0000d770: 5de8 35fa 3315 1614 0383 5e5f 8ee0 5bbf  ].5.3.....^_..[.
-0000d780: 4f56 6640 8ec8 e423 eae4 83f5 b5a6 5c4d  OVf@...#......\M
-0000d790: 7031 3a47 5c2b d360 88fa 82ea 1d57 6e02  p1:G\+.`.....Wn.
-0000d7a0: 96bd b709 5309 58a2 cf48 3438 caa6 d4cc  ....S.X..H48....
-0000d7b0: 9a7a 2ece 629f 4c0e 2aee 322e 2b3c 2679  .z..b.L.*.2.+<&y
-0000d7c0: ee09 ae59 a6a5 6d70 5b04 ce17 d04e 0fc1  ...Y..mp[....N..
-0000d7d0: 79ab 039c f048 e565 9e27 11fe 1ba8 fb18  y....H.e.'......
-0000d7e0: db8b 0b7c 78dd 8e13 da3e a783 7f27 19e1  ...|x....>...'..
-0000d7f0: 839d ed7a f503 4877 4257 910e 789c 8d8b  ...z..HwBW..x...
-0000d800: 390e c230 1000 7bbf 627b a468 6de3 4b42  9..0..{.b{.hm.KB
-0000d810: 4840 01df f0da 1b92 220e 4a36 e1fb e409  H@......".J6....
-0000d820: 4c33 cd8c 2ccc 50d9 628f 648b d367 4368  L3..,.P.b.d..gCh
-0000d830: cf2e 5266 d487 c8a7 8c48 64aa 0ba4 3e79  ..Rf.....Hd...>y
-0000d840: e126 10b8 f698 3ce5 925c c4a0 73aa 39f5  .&....<..\..s.9.
-0000d850: 2646 e38d d626 a4be fa42 a9aa bcc9 302f  &F...&...B....0/
-0000d860: f01c e5b5 11dc 8a8c 735b e13e 0b5c aea0  ........s[.>.\..
-0000d870: 83f6 2944 eb1d 9cf0 4095 799a 4611 fe7b  ..)D....@.y.F..{
-0000d880: 508f 21b7 3757 d879 598f 12da 36d1 b17f  P.!.7W.yY...6...
-0000d890: 4719 60c7 ce75 56fd 00f5 c141 ea98 0e78  G.`..uV....A...x
-0000d8a0: 9c9d cc41 0ac2 3010 40d1 7d4e 91bd 2049  ...A..0.@.}N.. I
-0000d8b0: a649 1810 f100 4a17 d285 cbc9 6452 0b4d  .I....J.....dR.M
-0000d8c0: 2b21 bdbf 9ec1 ed87 f77b 13d1 810b b2cf  +!.......{......
-0000d8d0: 9e85 31f8 816d 22c8 1623 5970 459c c999  ..1..m"..#YpE...
-0000d8e0: 90dc 00ea 434d b6ae 6d74 109c 2f81 d808  ....CM..mt../...
-0000d8f0: 9634 1060 f109 4db6 2c25 0271 cc1e 5252  .4.`..M.,%.q..RR
-0000d900: 74f4 f7de f4b8 1d4d 4ff7 e939 bef4 853a  t......MO..9...:
-0000d910: e57d a6cd 84db 5c69 59cf bcd7 eb6f 6903  .}....\iY....oi.
-0000d920: 4634 16f4 c980 31ea 57eb d2bb fca7 d563  F4....1.W......c
-0000d930: d996 4aab 2e42 fd68 a2be e729 45f5 9d14  ..J..B.h...)E...
-0000d940: 789c 9d8d 3d4e c430 1085 fb9c c2dd 1608  x...=N.0........
-0000d950: 3276 fc8b 10e2 00a0 2dd0 1694 93f1 3889  2v......-.....8.
-0000d960: 9638 91e3 dc1f 5370 015e f9f4 beef d5c2  .8....Sp.^......
-0000d970: 2c54 882a 2292 09a0 4390 4eb1 315a 2a1b  ,T.*"...C.N.1Z*.
-0000d980: 9d8a 7a88 0370 3408 da76 3b16 ce55 244a  ..z..p4..v;..U$J
-0000d990: 14c8 a38e a387 60d0 0e83 8298 0231 6bc7  ......`......1k.
-0000d9a0: a357 5e11 290e 7f7b 4496 8eda c681 1d12  .W^.)..{D.......
-0000d9b0: 80b2 c628 c5e8 1245 c929 3849 2dde 7478  ...(...E.)8I-.tx
-0000d9c0: d679 2be2 9acf 226e efb7 cfeb 9778 c18a  .y+..."n.....x..
-0000d9d0: 719b 3083 7d9b 565c be9f 685b 5f85 74d2  q.0.}.V\..h[_.t.
-0000d9e0: 06e7 0d68 f100 0340 d7da 75a9 95ff 4777  ...h...@..u...Gw
-0000d9f0: 1f5c 2616 63c1 4cb3 b8ac 7834 d345 6c49  .\&.c.L...x4.ElI
-0000da00: ccb5 eec7 73df 4f4b 9dcf f117 efb7 76d0  ....s.OK......v.
-0000da10: bc77 ccfd b4d7 473c 8ee5 a898 6bf7 0329  .w....G<....k..)
-0000da20: 5b66 419c 0d78 9c9d cbb1 0ac2 3010 80e1  [fA..x......0...
-0000da30: 3d4f 915d 904b 422f 7720 e2e4 2474 900e  =O.].KB/w ..$t..
-0000da40: 8ed7 5c52 0bb6 9590 828f afcf e0fa 7ffc  ..\R............
-0000da50: ade6 6c89 5453 700a 9d28 1574 a143 a202  ..l.TSp..(.t.C..
-0000da60: cc81 744c 9828 86a8 a188 794b cd6b b331  ..tL.(....yK.k.1
-0000da70: eb4f 7194 c41d 4174 c22a 5c3c 9147 ef9c  .Oq...At.*\<.G..
-0000da80: 8f5c 14d3 c86a 646f cfad da7e ddab 1d6e  .\...jdo...~...n
-0000da90: c3bd 7fd8 9334 d16d 9215 f032 2d32 bf8e  .....4.m...2-2..
-0000daa0: 695b ced6 4587 1ca9 036f 0f10 00cc af2e  i[..E....o......
-0000dab0: 736b f9bf db5c e78f f902 2368 4068 9d14  sk...\....#h@h..
-0000dac0: 789c 9d90 3d4e c430 1484 fb9c c2dd 1608  x...=N.0........
-0000dad0: e2bf e71f 8410 0700 6d81 b6a0 7cb6 9f93  ........m...|...
-0000dae0: 6889 1339 cefd 3105 1740 d38d e69b 91a6  h..9..1..@......
-0000daf0: 5522 1622 719d 4180 a01c 45f2 90c8 43f6  U"."q.A...E...C.
-0000db00: e824 b92e 00c5 1d05 2387 1d2b 95c6 0248  .$......#..+...H
-0000db10: 5012 53cc 96ac d480 3e29 eeb9 e328 a24b  P.S.....>)...(.K
-0000db20: 909d 345e 0412 7f79 f42a 678b 1914 9080  ..4^...y.*g.....
-0000db30: 1c8c d6a8 129a 8852 24ed 4d88 de71 7276  .......R$.M..qrv
-0000db40: c0b3 cd5b 65d7 7256 767b bf7d 5ebf d80b  ...[e.rVv{.}^...
-0000db50: 364c db84 859b b769 c5e5 fb29 6eeb 2b13  6L.....i...)n.+.
-0000db60: 5618 6f9d d292 3d70 c5f9 d0dd 7569 8dfe  V.o...=p....ui..
-0000db70: 470f 1f54 a77e 44c5 1267 7659 f1e8 4d17  G..T.~D..gvY..M.
-0000db80: b665 36b7 b61f cfe3 382d 6d3e c32f 3e6e  .e6.....8-m>./>n
-0000db90: 7da0 f7de b18c d3de 1ef1 3896 a361 69c3  }.........8..ai.
-0000dba0: 0faa e266 909c 0d78 9c9d cbb1 0ac2 3010  ...f...x......0.
-0000dbb0: 00d0 3d5f 915d 90bb 245e 1a10 7172 123a  ..=_.]..$^..qr.:
-0000dbc0: 4807 c7bb f4a2 05db 4a48 c1cf d76f 707d  H.......JH...op}
-0000dbd0: f05a 55b5 3181 0fa8 1242 4a90 91b9 80c7  .ZU.1....BJ.....
-0000dbe0: e2ca 2898 ba98 8314 525f 88cd 9bab 2ecd  ..(.....R_......
-0000dbf0: 0a68 8984 91a8 5364 3f4a f114 b252 1077  .h....Sd?J...R.w
-0000dc00: 7018 2491 6027 ce19 deda 73ad b65f b66a  p.$.`'....s.._.j
-0000dc10: 87eb 70eb eff6 c88d c7f5 c10b d0f9 31f3  ..p...........1.
-0000dc20: f4da e775 3e59 8c48 2976 3e80 dd81 0730  ...u>Y.H)v>....0
-0000dc30: 3f9d a7d6 f4bf 6d2e d3c7 7c01 0049 4030  ?.....m...|..I@0
-0000dc40: ab15 7801 3331 0002 05bd f4cc 928c d224  ..x.31.........$
-0000dc50: 867b 8f0f 453f e878 db2e cdbd e7c6 bef9  .{..E?.x........
-0000dc60: 9e3c 318d 5c87 0c0d 0ccc 4c4c c04a 32d3  .<1.\.....LL.J2.
-0000dc70: f3f2 8b52 19e6 ba4f b6a9 be75 fca1 cbf1  ...R...O...u....
-0000dc80: 991d 9be7 9fe1 e4fa cb74 0aaa cac7 d3d9  .........t......
-0000dc90: d52f d895 c1f0 7a61 c0a9 777d be6f 2a3e  ./....za..w}.o*>
-0000dca0: b370 7ef9 c7fb 6a9b e041 a812 5f47 3f4f  .p~...j..A.._G?O
-0000dcb0: 37d7 e010 bdcc 3c86 953e 0f17 6eba 71f1  7.....<..>..n.q.
-0000dcc0: f6ad 943b 4f53 24fa 4b3c f8f5 99a1 ca82  ...;OS$.K<......
-0000dcd0: 5c1d 5d7c 5df5 7253 189a d4e6 466b 2ead  \.]|].rS....Fk..
-0000dce0: b9fc 7701 fbb1 e36d 9704 2517 be55 862a  ..w....m..%..U.*
-0000dcf0: 4a2a cd2d d02b a864 b837 f1ce 3ad5 55c7  J*.-.+.d.7..:.U.
-0000dd00: 2f33 4db1 2970 fdd9 b0da f4ee 690f 13b0  /3M.)p......i...
-0000dd10: cfd2 0b4a e293 f373 0b4a 4b52 8be2 138b  ...J...s.JKR....
-0000dd20: 8b33 8b4b 12f3 4a18 eaaa a73e 9c13 d563  .3.K..J....>...c
-0000dd30: 6c57 2eef f869 5ddd 31e1 b284 c750 338b  lW...i].1....P3.
-0000dd40: 520b 4b33 8b52 7353 f34a 8af5 4a2a 4a18  R.K3.RsS.J..J*J.
-0000dd50: 7826 ce58 7366 f3c5 b557 b35d a63d 9df8  x&.Xsf...W.].=..
-0000dd60: 4be2 f4fa 943f 50b5 c5a9 25a5 6007 d8c5  K....?P...%.`...
-0000dd70: cf9c 9dfa e46a aaa6 a0d4 c549 fb8f dd73  .....j.....I...s
-0000dd80: 8a59 ef0e 0083 0491 3ea1 1478 0133 3430  .Y......>..x.340
-0000dd90: 3033 3151 888f cfcc cb2c 898f d72b a864  031Q.....,...+.d
-0000dda0: 2870 5a16 50bd fb6c ea9e d6df b3db d4ee  (pZ.P..l........
-0000ddb0: 66bc 52fe 1460 6200 040a 89e9 a979 250c  f.R..`b......y%.
-0000ddc0: 41e2 538a b5da 1d9b 2e47 dd70 7fb3 e8ae  A.S......G.p....
-0000ddd0: eb85 8997 03a1 f2a5 2999 f90c 9736 6aca  ........)....6j.
-0000dde0: 75d8 d8cf 0d9b 546c 2bfe e69c 72c1 11be  u.....Tl+...r...
-0000ddf0: 0a43 8835 e905 25f1 c9f9 b905 a525 a945  .C.5..%......%.E
-0000de00: f189 c5c5 99c5 2589 7925 204b c562 646b  ......%.y% K.bdk
-0000de10: 9fcc e258 f575 de15 ab43 2b77 65ec 1034  ...X.u...C+we..4
-0000de20: 7801 3134 bd34 9361 c176 49a3 8c8c 07cf  x.14.4.a.vI.....
-0000de30: 45cd 7cde 3e9d efbb 9975 e20d 37a8 9139  E.|.>....u..7..9
-0000de40: 39b9 20fd 259a ac6e b71e 0aa4 e5d8 75fc  9. .%..n......u.
-0000de50: d332 909a 1cba 93f5 2044 7f71 7251 6a6a  .2...... D.qrQjj
-0000de60: 1ec3 f953 fdcd b76c be70 9d38 c521 fce3  ...S...l.p.8.!..
-0000de70: a5d4 3249 09d1 58a8 1140 4714 811d a1e0  ..2I..X..@G.....
-0000de80: 7275 c1fc 50a5 9d89 d9aa 3a1c 1397 bd58  ru..P.....:....X
-0000de90: 557d 2a05 6248 6949 664e 31c3 c235 7e97  U}*.bHiIfN1..5~.
-0000dea0: cebf 6d8b 3e9c 51d9 6065 bd70 57b0 cc51  ..m.>.Q.`e.pW..Q
-0000deb0: 5b00 a891 8107 ae0e 7801 3334 3030 3331  [.......x.340031
-0000dec0: 5188 8fcf cccb 2c89 8fd7 2ba8 6448 6835  Q.....,...+.dHh5
-0000ded0: 6bfe 68a8 c272 6862 46e3 ba0c 0b33 89ff  k.h..rhbF....3..
-0000dee0: aaee 8610 6589 e9a9 7925 2035 b3af 38fa  ....e...y% 5..8.
-0000def0: 4f64 d0a8 397e 66a3 c90a c6cc 7fd9 cf3e  Od..9~f........>
-0000df00: 08c3 d414 1767 1697 2442 d46d f493 1198  .....g..$B.m....
-0000df10: f72d 42cb e0a7 74fe 1f75 ad4f 2112 d575  .-B...t..u.O!..u
-0000df20: 5075 4989 c9d9 e945 f9a5 7929 2003 9f4f  PuI....E..y) ..O
-0000df30: f113 59e2 9770 6c59 b7e6 1f6f c380 ed19  ..Y..plY...o....
-0000df40: 5ceb b640 1526 6724 96c4 6700 cdcc 2faa  \..@.&g$..g.../.
-0000df50: 0429 5db6 6b99 d985 af86 ce6a b3a7 f544  .)].k......j...D
-0000df60: 1cce 90ec 9ec8 fd15 aab4 a028 3f39 39b5  ...........(?99.
-0000df70: b818 a46c 2dc3 31b6 0b8f 5739 f27f b81b  ...l-.1...W9....
-0000df80: 30d3 4243 5bf1 80ae 2b00 6910 5b50 e403  0.BC[...+.i.[P..
-0000df90: 854e 789c 0134 00cb ffdb 02db 0290 f714  .Nx..4..........
-0000dfa0: 71e3 b40d cca6 a041 4014 fd87 843a 2a1f  q......A@....:*.
-0000dfb0: e4ef be80 930b 013c 140a ac16 944d 6b28  .......<.....Mk(
-0000dfc0: c7fc 0599 4450 df60 a768 88f4 1f81 1317  ....DP.`.h......
-0000dfd0: bbef 0483 4878 9c3b c874 90c9 ddd0 c0c0  ....Hx.;.t......
-0000dfe0: ccc4 4421 3e3e 332f b324 3e5e afa0 92c1  ..D!>>3/.$>^....
-0000dff0: 7fad 073f 4f09 57c8 5595 e959 675f 1a67  ...?O.W.U..Yg_.g
-0000e000: 1a07 f87f 3731 0002 85c4 f4d4 bc12 86d5  ....71..........
-0000e010: 2efe eb0e 3734 44fd c857 de9d 6ed3 3045  ....74D..W..n.0E
-0000e020: 967d 87fb 44f7 5f00 436f 1dc7 ef01 801e  .}..D._.Co......
-0000e030: 789c 011f 00e0 ffdb 02db 0290 f714 a285  x...............
-0000e040: ae6d 645e f9a5 b7e0 055c 3d58 8af7 85e2  .md^.....\=X....
-0000e050: 9dda 930b 0150 03b7 0fd3 ee01 8009 789c  .....P........x.
-0000e060: 011e 00e1 ffc1 02c1 0290 3314 a841 8e57  ..........3..A.W
-0000e070: a4e8 a6f2 8cec 8a95 04e5 f9e7 b4a3 1bba  ................
-0000e080: 9147 faeb 1e10 aeee 0182 5178 9c7b c7f8  .G........Qx.{..
-0000e090: 8e71 82b9 88d1 0b5b ff73 bf8c cd99 b59a  .q.....[.s......
-0000e0a0: dc0b e657 0733 6f34 7a39 d17b 3100 c18a  ...W.3o4z9.{1...
-0000e0b0: 0cb3 e403 8772 789c 0134 00cb ffdb 02db  .....rx..4......
-0000e0c0: 0290 f714 f633 edd3 c761 2dcc 4ede 3aff  .....3...a-.N.:.
-0000e0d0: 172a e7a0 fb6a 1705 930b 013c 14e2 47ee  .*...j.....<..G.
-0000e0e0: b062 9dc5 d988 1efe 6844 1c79 ffea 8f88  .b......hD.y....
-0000e0f0: 5fc2 8a1a a5e0 0380 1b78 9c3b c874 9049  _........x.;.t.I
-0000e100: ddd0 c0c0 ccc4 4421 3e3e 332f b324 3e5e  ......D!>>3/.$>^
-0000e110: afa0 9261 55ce aa94 b867 b94d 0a4f 3add  ...aU....g.M.O:.
-0000e120: f2a6 46c4 6cd1 58f3 62a3 ba14 2300 a037  ..F.l.X.b...#..7
-0000e130: 1288 e403 8872 789c 0134 00cb ffdb 02db  .....rx..4......
-0000e140: 0290 f714 bebc 19a2 8531 46d8 6974 fc1a  .........1F.it..
-0000e150: 5496 a8ec afc0 7001 930b 013c 1445 08ca  T.....p....<.E..
-0000e160: 5216 d7d2 3830 a7d1 ec0d f78a a26e 33cb  R...80.......n3.
-0000e170: 408b fd18 6fe4 0389 3578 9c01 3400 cbff  @...o...5x..4...
-0000e180: db02 db02 90f7 14bb f307 ff3c e72e 6cf8  ...........<..l.
-0000e190: df49 bc07 ab19 eac8 f0bf 6b93 0b01 3c14  .I........k...<.
-0000e1a0: 0488 e2c8 7683 914c 32de aaa8 667e 7497  ....v..L2...f~t.
-0000e1b0: f76a 04d8 cce3 1ac3 e403 832a 789c 0134  .j.........*x..4
-0000e1c0: 00cb ffdb 02db 0290 f714 02e2 e3ff 9b9a  ................
-0000e1d0: b5a5 646b 8d52 d2fc c1c5 ab6c cffa 930b  ..dk.R.....l....
-0000e1e0: 013c 143e 5f99 9b65 e4d5 6529 111a d192  .<.>_..e..e)....
-0000e1f0: bfc6 de42 5caf 47f0 b71b 7eef 0181 4978  ...B\.G...~...Ix
-0000e200: 9c01 1f00 e0ff db02 db02 90f7 14f9 8a9f  ................
-0000e210: f7db ca4e 98b5 ba34 3a83 cd58 8a0d 2954  ...N...4:..X..)T
-0000e220: a593 0b01 5010 3d0f 27e0 0388 2078 9c3b  ....P.=.'... x.;
-0000e230: c874 9049 ddd0 c0c0 ccc4 4421 3e3e 332f  .t.I......D!>>3/
-0000e240: b324 3e5e afa0 92a1 acbd f8fd 94b9 0922  .$>^..........."
-0000e250: 8dd9 bfa5 3afe bebc 50fe 397e db46 7529  ....:...P.9~.Fu)
-0000e260: 4600 ae4a 13f9 e003 8415 789c 3bc8 7490  F..J......x.;.t.
-0000e270: 49dd d0c0 c0cc c444 213e 3e33 2fb3 243e  I......D!>>3/.$>
-0000e280: 5eaf a092 a1c0 6959 40f5 eeb3 a97b 5a7f  ^.....iY@....{Z.
-0000e290: cf6e 53bb 9bf1 4af9 53c0 4675 2946 00a9  .nS...J.S.Fu)F..
-0000e2a0: d913 5ee0 0384 5278 9c3b c874 9049 ddd0  ..^...Rx.;.t.I..
-0000e2b0: c0c0 ccc4 4421 3e3e 332f b324 3e5e afa0  ....D!>>3/.$>^..
-0000e2c0: 9261 55ce aa94 b867 b94d 0a4f 3add f2a6  .aU....g.M.O:...
-0000e2d0: 46c4 6cd1 58f3 62a3 ba14 2300 a037 1288  F.l.X.b...#..7..
-0000e2e0: e003 826b 789c 3bc8 7490 49dd d0c0 c0cc  ...kx.;.t.I.....
-0000e2f0: c444 213e 3e33 2fb3 243e 5eaf a092 c174  .D!>>3/.$>^....t
-0000e300: 45e8 dcbe fee6 096d a7f7 5618 2d9d c37b  E......m..V.-..{
-0000e310: 9f2f fadb 4675 2946 009e d512 7ab1 0378  ./..Fu)F....z..x
-0000e320: 9c4b 2bca cf55 d02b 2e49 2c2a 51c8 cc2d  .K+..U.+.I,*Q..-
-0000e330: c807 5260 0e17 1757 7c7c 596a 5171 667e  ..R`...W||YjQqf~
-0000e340: 5e7c bc82 ad82 ba81 9ea9 9ea9 3a17 00b2  ^|..........:...
-0000e350: 210f a5eb 0188 1d78 9c7b c7f8 8e71 c22d  !......x.{...q.-
-0000e360: 11bb ed7b c29e dc9f 7ecf 31e3 5bf1 a5b5  ...{....~.1.[...
-0000e370: 3ced 93bd 6c5c 00cd 700e 1dba 3b78 9cbd  <...l\..p...;x..
-0000e380: 52bb 6edc 3010 ecf5 150b b991 8203 3f20  R.n.0.........? 
-0000e390: c015 2912 2040 0ac3 4e8a 2008 e43d 6a25  ..). @..N. ..=j%
-0000e3a0: 11a1 489a 5cda f1df 6749 ddc3 38b8 4a61  ..H.\...gI..8.Ja
-0000e3b0: 16a2 48cd ccee 8c76 8a7e 05a5 ac5d c1ac  ..H....v.~...]..
-0000e3c0: c147 860f 4d59 53b9 b7e8 e639 6258 945e  .G..MYS....9bX.^
-0000e3d0: 48ff 09de 3856 e9d1 1aa6 13fa be9e eef1  H...8V..........
-0000e3e0: 8962 f316 3144 3a64 63f9 84d7 0bf2 8033  .b..1D:dc......3
-0000e3f0: 391e e82f e9cc 3e9e 4839 24ef 8c3e 21bf  9../..>.H9$..>!.
-0000e400: 9b59 34d9 7b9b 60bf 9dba 7e3b 2b72 78b0  .Y4.{.`...~;+rx.
-0000e410: 34a0 d087 488f d944 5a45 b200 bfa0 4d74  4...H..DZE....Mt
-0000e420: a66d f0d2 8e14 364e 0446 9a60 a6eb 1eba  .m....6N.F.`....
-0000e430: fe63 03b2 2271 8eee ad2e 958e 844c 4351  .c.."q.......LCQ
-0000e440: 1c34 5a6b dc7c a117 c5d5 8f64 bb7e b715  .4Zk.|.....d.~..
-0000e450: ed4b 186d db5e 02a9 1da8 aa9a ce26 057a  .K.m.^.......&.z
-0000e460: 8510 d140 d114 3f68 5566 2301 1b3a 336e  ...@..?hUf#..:3n
-0000e470: 5f78 f1ee eef3 edb7 26d4 5709 2058 b17a  _x......&.W. X.z
-0000e480: f920 2e6f e0a7 cfa0 51ac d4b6 8117 aa7d  . .o....Q......}
-0000e490: c903 02a6 5476 f95a bb69 8a42 3556 8296  ....Tv.Z.i.B5V..
-0000e4a0: adab 5938 5c69 dfbe 2ad2 eeea fd48 4947  ..Y8\i..*....HIG
-0000e4b0: 13d8 78b7 6f3f 1deb 425a c85a 053f 52a9  ..x.o?..BZ.Z.?R.
-0000e4c0: 65aa fe96 0ec1 2601 daaf 2bba 3129 f8ea  e.....&...+.1)..
-0000e4d0: 4266 61f8 6c47 3810 203c a135 e315 5070  Bfa.lG8. <.5..Pp
-0000e4e0: 13bc 888d 6774 5cf4 126d 3e7c e6c2 f7d3  ....gt\..m>|....
-0000e4f0: 46cc b4ab b0a3 5e88 32a5 60b8 c0e0 d9f0  F.....^.2.`.....
-0000e500: 020f f5aa 534a f50f ea68 62ca 4eef 5f79  ....SJ...hb.N._y
-0000e510: 5331 bb5d d3ff d7fc bec3 48fd 3aff a2df  S1.]......H.:...
-0000e520: 7d9d aaa6 f907 8fbe 5167 ba26 789c 8d90  }.......Qg.&x...
-0000e530: 4f4b c430 10c5 effd 14a1 a714 245d f5b6  OK.0........$]..
-0000e540: d08b 7a58 4111 5d2f 2212 d224 ed0e e6cf  ..zXA.]/"..$....
-0000e550: 9aa4 8722 7e77 63da ba6e a968 6e99 79bf  ..."~wc..n.hn.y.
-0000e560: 9979 af71 5623 c54c cb77 0c0c e556 ebce  .y.qV#.L.w...V..
-0000e570: 40e8 49fc 07aa a5f7 ac95 7407 3e58 07d2  @.I.......t.>X..
-0000e580: 23d0 7beb 02da dedf 5c46 c1ed d0df a476  #.{.....\F.....v
-0000e590: 9f35 5fc3 48cd f86b eb6c 67c4 a456 4a8f  .5_.H..k.lg..VJ.
-0000e5a0: 237a 6aa1 05c3 5496 8d3d eb47 8c74 0194  #zj...T..=.G.t..
-0000e5b0: 27a2 9ea8 5686 6f4a d459 7c42 36a9 ba70  '...V.oJ.Y|B6..p
-0000e5c0: 5b8f 8b75 86e2 db3b 3001 e79b ebed e3dd  [..u...;0.......
-0000e5d0: c313 baba c84f 6693 7051 2425 b7c6 481e  .....Of.pQ$%..H.
-0000e5e0: c01a 542d 1bc2 49e7 632d 8a28 882a 6735  ..T-..I.c-.(.*g5
-0000e5f0: 3f3d 3b8f 230f 30f5 21ae 6cab 26f7 6f0a  ?=;.#.0.!.l.&.o.
-0000e600: 825c 9765 f93e dff8 910f 3ba1 414a 1a7c  .\.e.>....;.AJ.|
-0000e610: a0c9 68c3 17a8 aad0 6af0 707c 1d61 424c  ..h.....j.p|.aBL
-0000e620: 6ef1 4294 cfab 9722 4b9c 93a1 73e6 073a  n.B...."K...s..:
-0000e630: 9487 e0b8 92cc 0dd1 cd22 fb3d 5292 205c  .........".=R. \
-0000e640: fc25 fbcf 859f f97d d72f b8d6 0278 9ced  .%.....}./...x..
-0000e650: 574b 8fdb 3610 befb 5710 3e49 cd46 4872  WK..6...W.>I.FHr
-0000e660: 5cc0 c716 4d90 1712 2f7a d82e 085a a22d  \...M.../z...Z.-
-0000e670: 66f9 1048 2a5d fdfb 0e49 917a 39b1 9383  f..H*]...I.z9...
-0000e680: 1ba0 f6c1 9686 33df 3c38 fc86 de6b 2550  ......3.<8...k%P
-0000e690: 5170 2e10 138d d216 fdb6 da7b 1931 8619  Qp.........{.1..
-0000e6a0: 4ba4 1d16 fa95 b226 16d7 b0a8 74b7 582c  K......&....t.X,
-0000e6b0: 485b 3155 586b e292 a54f 165b 854d 4369  H[1UXk...O.[.MCi
-0000e6c0: 594f d58c 4df0 61d9 293a 8319 9ca6 a5d2  YO..M.a.):......
-0000e6d0: 5554 f532 5c11 4b56 49ef d0b2 c2b0 8324  UT.2\.KVI......$
-0000e6e0: 3c01 fa37 5c13 5971 aa57 ab18 4ead 29a9  <..7\.Yq.W..N.).
-0000e6f0: 983c 44db a63b 1041 a395 604f 4e39 6933  .<D..;.A..`ON9i3
-0000e700: 41e3 b306 2425 a2c3 d632 6e8a 6a37 aac0  A...$%...2n.j7..
-0000e710: 6a08 67be 6a3a 63a9 c046 b5b2 c25c 95c4  j.g.j:c..F...\..
-0000e720: 3225 6fc0 5b89 436e 23e1 97d6 586c 4a4d  2%o.[.Cn#...XlJM
-0000e730: a934 b5b2 b821 b6be 4133 01b8 aae8 1e35  .4...!..A3.....5
-0000e740: 5a95 d418 ec4b 9259 f248 4796 9bad 6ee9  Z....K.Y.HG...n.
-0000e750: 0d0a d210 80d7 dbfc 41b8 8185 4a49 7044  ........A...JIpD
-0000e760: be52 cc04 39d0 20ce 6f57 083e 07ae 7650  .R..9. .oW.>..vP
-0000e770: cb71 a99d 387c 5b28 05b8 618d 0b18 6d66  .q..8|[(..a...mf
-0000e780: 7b97 1dc9 2a0f 866c bf8c e636 2c2d 705f  {...*..l...6,-p_
-0000e790: 2d81 8f56 b187 f65f d0c7 98c9 a6b5 60bb  -..V..._......`.
-0000e7a0: befb fcfb a75b b47e 3641 fd5e 1c31 8c01  .....[.~6A.^.1..
-0000e7b0: e519 c0a0 bf25 fa60 6baa 91da a3a3 98af  .....%.`k.......
-0000e7c0: 56c9 b96a 6df0 9e8e 4f96 d06e d081 5aec  V..jm...O..n..Z.
-0000e7d0: 4f8f 803d 838a c753 94e5 452f 31bd 1267  O..=...S..E/1..g
-0000e7e0: 144c f3c5 b66f 66ef 4326 498e 28ec 227a  .L...of.C&I.(."z
-0000e7f0: af24 cd5d 43f6 e9ce f67a 48b6 6cb5 065f  .$.]C....zH.l.._
-0000e800: bc8b 4119 88fe 8c40 13c0 3282 01dc 9785  ..A....@..2.....
-0000e810: 9884 03d0 4b7f f7cf 5f3e 1425 c407 e2fb  ....K..._>.%....
-0000e820: 170f 13e3 a536 7081 505f 6976 1c27 5f4d  .....6p.P_iv.'_M
-0000e830: ccbf 9347 c929 d159 3e51 df2b 8d62 a44c  ...G.).Y>Q.+.b.L
-0000e840: 1e71 3ecd ec84 0752 5551 9af5 bff9 b9d1  .q>....RUQ......
-0000e850: 8d6d ff6c 0591 effa 97be 4e9b fb71 591f  .m.l......N..qY.
-0000e860: f23e ef33 1187 4e0d 355b 74ef 5421 6e4e  .>.3..N.5[t.T!nN
-0000e870: f0d1 6806 adb9 feab 569c a2b7 6fdf a10f  ..h.....V...o...
-0000e880: 77db 8f77 dbf5 59ed 9d0f 6775 cacf c3bc  w..w..Y...gu....
-0000e890: 01ea 308d 9286 6247 d45d 4105 8393 901a  ..0...bG.]A.....
-0000e8a0: 5942 8733 833d 49fa d122 5445 3926 a565  YB.3.=I.."TE9&.e
-0000e8b0: d015 f9b0 4309 c69f 93cd 6c0e 8d6a 30ea  ....C.....l..j0.
-0000e8c0: 194f a99c 7481 6ef2 e976 c749 d340 964a  .O..t.n..v.I.@.J
-0000e8d0: 8021 d578 3125 8128 c269 c73b f534 3177  .!.x1%.(.i.;.41w
-0000e8e0: e764 bc58 58f5 9113 26b7 de15 da00 d5ac  .d.XX...&.......
-0000e8f0: 97fd 3535 31d4 7af5 71f0 49f5 481a 612c  ..551.z.q.I.H.a,
-0000e900: ccf2 1825 3891 fbd1 5730 c98e 2f88 d6b0  ...%8...W0../...
-0000e910: b2e0 8a54 d9a4 b4df d675 8e66 50ff d40c  ...T.....u.fP...
-0000e920: ba66 ace4 9a66 d79a 6e1e a54f 1ea6 6f61  .f...f..n..O..oa
-0000e930: 38a5 4df6 a278 3945 3add 3ed0 7b4d 43ab  8.M..x9E:.>.{MC.
-0000e940: d840 4399 d2a3 0b70 47ca 471c 2e05 ae49  .@C....pG.G....I
-0000e950: e2ed a0d8 fa27 18a9 1a22 dc0c d5cc bf65  .....'...".....e
-0000e960: 0d97 19a2 a323 c7c1 b717 69ab 1f68 909f  .....#....i..h..
-0000e970: a9da cfd6 ca65 7aba 54b3 5bcc 3042 5c91  .....ez.T.[.0B\.
-0000e980: 4ecd f5f5 6b7f 55f2 d307 91d1 a42c 3c91  N...k.U......,<.
-0000e990: 77aa 4556 010d 082a 7690 2b7a e394 0de9  w.EV...*v.+z....
-0000e9a0: 907a 2cd6 632a 7324 f6fa 3d70 18ca 3ce0  .z,.c*s$..=p..<.
-0000e9b0: 8094 03ab 25df f905 c7fc b13b 601e 6e98  ....%......;`.n.
-0000e9c0: 1721 fae8 e717 22e9 4b1c a62b 47a3 5f84  .!....".K..+G._.
-0000e9d0: a3d3 d3b8 2257 aefe 0fb9 7ad8 9b29 69fb  ...."W....z..)i.
-0000e9e0: 3a79 88d3 941d feda 5f90 47d3 dfa0 0bd1  :y......_.G.....
-0000e9f0: e679 fb76 e5cc 2b67 5e39 f3ff c499 ff02  .y.v..+g^9......
-0000ea00: 5136 db93 b13a 789c 7d53 5d6f d430 107c  Q6...:x.}S]o.0.|
-0000ea10: f7af 30ee 432f 281f 952a 108a 6444 250a  ..0.C/(..*..dD%.
-0000ea20: 42a2 2a82 f601 5528 7293 bd9c b9c4 36de  B.*...U(r.....6.
-0000ea30: 35ed 81f8 eff8 9c0b a855 eff2 e087 99f1  5........U......
-0000ea40: eeec ac73 f4ac 0ae8 ab5b 6d2a b7a1 9535  ...s.....[m*...5
-0000ea50: a7ec 8817 cf0b deda 4e9b bee6 8196 c5ab  ........N.......
-0000ea60: 2dc2 d8d2 db91 2350 7064 ed80 5c8f ce7a  -.....#Ppd..\..z
-0000ea70: 9a10 c6ee 34ad b875 6016 c71e 7e04 ed61  ....4..u`...~..a
-0000ea80: 0443 58d2 3d1d 675c 215f ba9a f1f8 6983  .CX.=.g\!_....i.
-0000ea90: a486 a1d9 a990 cb48 951e 54b7 c858 2ab6  .......H..T..X*.
-0000eaa0: 483a a346 90a2 77d4 b476 7481 c037 0a51  H:.F..w..vt..7.Q
-0000eab0: c7cb 8644 9e24 3fc1 a3b6 468a 93f2 4579  ...D.$?...F...Ey
-0000eac0: ba03 3bc0 d66b 4789 10e2 fda7 ab78 4ed4  ..;..kG......xN.
-0000ead0: 604d df3c e4cb ef56 9b45 f22d 3e9f 9fbd  `M.<...V.E.->...
-0000eae0: bd38 2fc7 4ee4 1ccc 9480 1429 0191 2587  .8/.N......)..%.
-0000eaf0: 8336 808b 2c7b ba5c 346a 280e ddd0 c645  .6..,{.\4j(....E
-0000eb00: eb04 f754 8dca af3b 7b67 760e 821f a458  ...T...;{gv....X
-0000eb10: 1139 acab aa8f 9185 db32 8e57 5913 bc22  .9.......2.WY.."
-0000eb20: b556 a68a 1317 f3c4 c5e3 8955 884b f252  .V.........U.K.R
-0000eb30: 5c46 3d3f 4b17 f8f5 c7eb 2f97 5f1f 081a  \F=?K...../._...
-0000eb40: 1895 8e9d 62c9 cef6 ca9c bc7c d36f 916d  ....b......|.o.m
-0000eb50: af39 0bdd 82c1 68f3 e2c3 d50e 72aa 5dab  .9....h.....r.].
-0000eb60: 1e50 deec 8d9d ef61 ca78 ef20 df07 7d80  .P.....a.x. ..}.
-0000eb70: 8d11 0298 0382 407a c043 ed43 a7ad f896  ......@z.C.C....
-0000eb80: 3ff9 c2e4 6360 9245 c37e d3b8 b87f 42f9  ?...c`.E.~....B.
-0000eb90: 3b41 db4f c42d a21d a099 f68a a2e6 3762  ;A.O.-........7b
-0000eba0: 6ef9 afa3 dc37 0929 4f75 3a67 3b7f f2a9  n....7.)Ou:g;...
-0000ebb0: f094 71fa cbfe 5b13 af25 9f5f ee2f ed1a  ..q...[..%._./..
-0000ebc0: 544b 90ef d480 90b3 8c31 f617 ed83 3928  TK.......1....9(
-0000ebd0: 6c82 4c78 9c5b c8be 907d c269 4693 8d67  l.Lx.[...}.iF..g
-0000ebe0: ae32 0100 2059 0535 6c18 789c 5bc8 be90  .2.. Y.5l.x.[...
-0000ebf0: 7dc2 6946 d38d 67ae 3201 0020 5e05 36b1  }.iF..g.2.. ^.6.
-0000ec00: 0378 9c4b 2bca cf55 d02b 2e49 2c2a 51c8  .x.K+..U.+.I,*Q.
-0000ec10: cc2d c807 5260 0e17 1757 7c7c 596a 5171  .-..R`...W||YjQq
-0000ec20: 667e 5e7c bc82 ad82 ba81 9ea9 9e89 3a17  f~^|..........:.
-0000ec30: 00b2 1e0f a4b1 0378 9c4b 2bca cf55 d02b  .......x.K+..U.+
-0000ec40: 2e49 2c2a 51c8 cc2d c807 5260 0e17 1757  .I,*Q..-..R`...W
-0000ec50: 7c7c 596a 5171 667e 5e7c bc82 ad82 ba81  ||YjQqf~^|......
-0000ec60: 9ea9 9eb1 3a17 00b2 1b0f a37f 7d2c 812f  ....:.......},./
-0000ec70: c9c6 52e0 377f 6b41 48f3 8151 d8a1 36    ..R.7.kAH..Q..6
+0000d6b0: 78e9 000e de91 0e78 9c8d cb4d 0e82 3010  x......x...M..0.
+0000d6c0: 40e1 7d4f 317b 13d2 ffd2 c498 a80b bdc6  @.}O1{..........
+0000d6d0: b433 0a0b 8a81 01af 2f47 f0ad df27 0b33  .3....../G...'.3
+0000d6e0: 30f9 1766 ab5f d696 88b5 8650 7324 6fb2  0..f._.....Ps$o.
+0000d6f0: 27a3 535f 9873 491a 83fa e0c2 4dc0 f4c1  '.S_.sI.....M...
+0000d700: 91f3 9112 9276 44c5 ea12 7576 6c6b 42c3  .....vD...uvlkB.
+0000d710: d4a3 c364 8b55 b8c9 302f f018 e5b9 15b8  ...d.U..0/......
+0000d720: 5619 e7b6 c26d 1638 5fc0 2413 73ca d61b  V....m.8_.$.s...
+0000d730: 38e9 2355 e769 1a45 f86f a0ee 03b6 3713  8.#U.i.E.o....7.
+0000d740: ecbc acc7 096d 9bca c1bf a30c b0eb 2e74  .....m.........t
+0000d750: 51fd 0034 fd42 3791 0e78 9c8d 8d41 0ec2  Q..4.B7..x...A..
+0000d760: 2010 00ef bc62 ef26 0d2c a52c 8931 510f   ....b.&.,.,.1Q.
+0000d770: fa0d a08b eda1 ada1 5bfd be3c c139 cf64  ........[..<.9.d
+0000d780: a432 03c6 1eb1 7049 4153 f6ce 8571 c4e2  .2....pIAS...q..
+0000d790: cd40 5cb2 f594 c893 4b71 40f5 8e95 5701  .@\.....Kq@...W.
+0000d7a0: a3d1 1987 269b 1c42 f11e 2da5 9e06 6d13  ....&..B..-...m.
+0000d7b0: eb1e 5374 8436 9a40 2a1e 326d 151e b33c  ..St.6.@*.2m...<
+0000d7c0: 8f04 d72c f3b6 ee70 db04 ce17 30ed 107c  ...,...p....0..|
+0000d7d0: d096 e0a4 1b2a 6fcb 328b f0df 81ba 4f71  .....*o.2.....Oq
+0000d7e0: 7df1 081f ae7b 3361 3d96 d4f2 ef2c 137c  }....{3a=....,.|
+0000d7f0: 74e7 3aa7 7e3c 0640 b391 0e78 9c8d cb4d  t.:.~<.@...x...M
+0000d800: 0e82 3010 40e1 7d4f 317b 1332 ed50 da26  ..0.@.}O1{.2.P.&
+0000d810: c644 5de8 35fa 3315 1614 0383 5e5f 8ee0  .D].5.3.....^_..
+0000d820: 5bbf 4f56 6640 8ec8 e423 eae4 83f5 b5a6  [.OVf@...#......
+0000d830: 5c4d 7031 3a47 5c2b d360 88fa 82ea 1d57  \Mp1:G\+.`.....W
+0000d840: 6e02 96bd b709 5309 58a2 cf48 3438 caa6  n.....S.X..H48..
+0000d850: d4cc 9a7a 2ece 629f 4c0e 2aee 322e 2b3c  ...z..b.L.*.2.+<
+0000d860: 2679 ee09 ae59 a6a5 6d70 5b04 ce17 d04e  &y...Y..mp[....N
+0000d870: 0fc1 79ab 039c f048 e565 9e27 11fe 1ba8  ..y....H.e.'....
+0000d880: fb18 db8b 0b7c 78dd 8e13 da3e a783 7f27  .....|x....>...'
+0000d890: 19e1 839d ed7a f503 4877 4257 910e 789c  .....z..HwBW..x.
+0000d8a0: 8d8b 390e c230 1000 7bbf 627b a468 6de3  ..9..0..{.b{.hm.
+0000d8b0: 4b42 4840 01df f0da 1b92 220e 4a36 e1fb  KBH@......".J6..
+0000d8c0: e409 4c33 cd8c 2ccc 50d9 628f 648b d367  ..L3..,.P.b.d..g
+0000d8d0: 4368 cf2e 5266 d487 c8a7 8c48 64aa 0ba4  Ch..Rf.....Hd...
+0000d8e0: 3e79 e126 10b8 f698 3ce5 925c c4a0 73aa  >y.&....<..\..s.
+0000d8f0: 39f5 2646 e38d d626 a4be fa42 a9aa bcc9  9.&F...&...B....
+0000d900: 302f f01c e5b5 11dc 8a8c 735b e13e 0b5c  0/........s[.>.\
+0000d910: aea0 83f6 2944 eb1d 9cf0 4095 799a 4611  ....)D....@.y.F.
+0000d920: fe7b 508f 21b7 3757 d879 598f 12da 36d1  .{P.!.7W.yY...6.
+0000d930: b17f 4719 60c7 ce75 56fd 00f5 c141 ea9c  ..G.`..uV....A..
+0000d940: 0d78 9c9d cbbd 0ac2 3010 00e0 3d4f 915d  .x......0...=O.]
+0000d950: 90fc de25 20e2 e424 7490 0e8e 97e4 520b  ...% ..$t.....R.
+0000d960: b695 9082 8faf cfe0 fac1 d71b b3e4 80c1  ................
+0000d970: e8e4 4c76 3941 2650 4133 b892 d011 6280  ..Lv9A&PA3....b.
+0000d980: 5c21 e8ca 2cde d478 ed32 63f5 452b 6f6a  \!..,..x.2c.E+oj
+0000d990: b45e b954 abf7 064b b229 99ea 2880 8eb9  .^.T...K.)..(...
+0000d9a0: 7800 417b 7f6e 4d0e ebde e478 1bef c343  x.A{.nM....x...C
+0000d9b0: 9ea8 53d9 265a 155c a685 e6d7 316f cb59  ..S.&Z.\....1o.Y
+0000d9c0: 6ad4 1031 1a63 e541 59a5 c44f 97b9 77fe  j..1.c.AY..O..w.
+0000d9d0: 6f8b ebfc 115f 2fcb 407d 980e 789c 9dcc  o...._/.@}..x...
+0000d9e0: 410a c230 1040 d17d 4e91 bd20 49a6 4918  A..0.@.}N.. I.I.
+0000d9f0: 10f1 004a 17d2 85cb c964 520b 4d2b 21bd  ...J.....dR.M+!.
+0000da00: bf9e c1ed 87f7 7b13 d181 0bb2 cf9e 8531  ......{........1
+0000da10: f881 6d22 c816 2359 7045 9cc9 9990 dc00  ..m"..#YpE......
+0000da20: ea43 4db6 ae6d 7410 9c2f 81d8 0896 3410  .CM..mt../....4.
+0000da30: 60f1 094d b62c 2502 71cc 1e52 5274 f4f7  `..M.,%.q..RRt..
+0000da40: def4 b81d 4d4f f7e9 39be f485 3ae5 7da6  ....MO..9...:.}.
+0000da50: cd84 db5c 6959 cfbc d7eb 6f69 0346 3416  ...\iY....oi.F4.
+0000da60: f4c9 8031 ea57 ebd2 bbfc a7d5 63d9 964a  ...1.W......c..J
+0000da70: ab2e 42fd 68a2 bee7 2945 f59d 1478 9c9d  ..B.h...)E...x..
+0000da80: 8d3d 4ec4 3010 85fb 9cc2 dd16 0832 76fc  .=N.0........2v.
+0000da90: 8b10 e200 a02d d016 9493 f138 8996 3891  .....-.....8..8.
+0000daa0: e3dc 1f53 7001 5ef9 f4be efd5 c22c 5488  ...Sp.^......,T.
+0000dab0: 2a22 9209 a043 904e b131 5a2a 1b9d 8a7a  *"...C.N.1Z*...z
+0000dac0: 8803 7034 08da 763b 16ce 5524 4a14 c8a3  ..p4..v;..U$J...
+0000dad0: 8ea3 8760 d00e 8382 9802 316b c7a3 575e  ...`......1k..W^
+0000dae0: 1129 0e7f 7b44 968e dac6 811d 1280 b2c6  .)..{D..........
+0000daf0: 28c5 e812 45c9 2938 492d de74 78d6 792b  (...E.)8I-.tx.y+
+0000db00: e29a cf22 6eef b7cf eb97 78c1 8a71 9b30  ..."n.....x..q.0
+0000db10: 837d 9b56 5cbe 9f68 5b5f 8574 d206 e70d  .}.V\..h[_.t....
+0000db20: 68f1 0003 40d7 da75 a995 ff47 771f 5c26  h...@..u...Gw.\&
+0000db30: 1663 c14c b3b8 ac78 34d3 456c 49cc b5ee  .c.L...x4.ElI...
+0000db40: c773 df4f 4b9d cff1 17ef b776 d0bc 77cc  .s.OK......v..w.
+0000db50: fdb4 d747 3c8e e5a8 986b f703 295b 6641  ...G<....k..)[fA
+0000db60: 9c0d 789c 9dcb b10a c230 1080 e13d 4f91  ..x......0...=O.
+0000db70: 5d90 4b42 2f77 20e2 e424 7490 0e8e d75c  ].KB/w ..$t....\
+0000db80: 520b b695 9082 8faf cfe0 fa7f fcad e66c  R..............l
+0000db90: 8954 5370 0a9d 2815 74a1 43a2 02cc 8174  .TSp..(.t.C....t
+0000dba0: 4c98 2886 a8a1 8879 4bcd 6bb3 31eb 4f71  L.(....yK.k.1.Oq
+0000dbb0: 94c4 1d41 74c2 2a5c 3c91 47ef 9c8f 5c14  ...At.*\<.G...\.
+0000dbc0: d3c8 6a64 6fcf adda 7edd ab1d 6ec3 bd7f  ..jdo...~...n...
+0000dbd0: d893 34d1 6d92 15f0 322d 32bf 8e69 5bce  ..4.m...2-2..i[.
+0000dbe0: d645 871c a903 6f0f 1000 ccaf 2e73 6bf9  .E....o......sk.
+0000dbf0: bfdb 5ce7 8ff9 0223 6840 689d 1478 9c9d  ..\....#h@h..x..
+0000dc00: 903d 4ec4 3014 84fb 9cc2 dd16 08e2 bfe7  .=N.0...........
+0000dc10: 1f84 1007 006d 81b6 a07c b69f 9368 8913  .....m...|...h..
+0000dc20: 39ce fd31 0517 40d3 8de6 9b91 a655 2216  9..1..@......U".
+0000dc30: 2271 9d41 80a0 1c45 f290 c843 f6e8 24b9  "q.A...E...C..$.
+0000dc40: 2e00 c51d 0523 871d 2b95 c602 4850 1253  .....#..+...HP.S
+0000dc50: cc96 acd4 803e 29ee b9e3 28a2 4b90 9d34  .....>)...(.K..4
+0000dc60: 5e04 127f 79f4 2a67 8b19 1490 801c 8cd6  ^...y.*g........
+0000dc70: a812 9a88 5224 ed4d 88de 7172 76c0 b3cd  ....R$.M..qrv...
+0000dc80: 5b65 d772 5676 7bbf 7d5e bfd8 0b36 4cdb  [e.rVv{.}^...6L.
+0000dc90: 8485 9bb7 69c5 e5fb 296e eb2b 1356 186f  ....i...)n.+.V.o
+0000dca0: 9dd2 923d 70c5 f9d0 dd75 698d fe47 0f1f  ...=p....ui..G..
+0000dcb0: 54a7 7e44 c512 6776 59f1 e84d 17b6 6536  T.~D..gvY..M..e6
+0000dcc0: b7b6 1fcf e338 2d6d 3ec3 2f3e 6e7d a0f7  .....8-m>./>n}..
+0000dcd0: deb1 8cd3 de1e f138 96a3 6169 c30f aae2  .......8..ai....
+0000dce0: 6690 9c0d 789c 9dcb b10a c230 1000 d03d  f...x......0...=
+0000dcf0: 5f91 5d90 bb24 5e1a 1071 7212 3a48 07c7  _.]..$^..qr.:H..
+0000dd00: bbf4 a205 db4a 48c1 cfd7 6f70 7df0 5a55  .....JH...op}.ZU
+0000dd10: b531 810f a812 424a 9091 b980 c7e2 ca28  .1....BJ.......(
+0000dd20: 98ba 9883 1452 5f88 cd9b ab2e cd0a 6889  .....R_.......h.
+0000dd30: 8491 a853 643f 4af1 14b2 5210 7770 1824  ...Sd?J...R.wp.$
+0000dd40: 9160 27ce 19de da73 adb6 5fb6 6a87 eb70  .`'....s.._.j..p
+0000dd50: ebef f6c8 8dc7 f5c1 0bd0 f931 f3f4 dae7  ...........1....
+0000dd60: 753e 598c 4829 763e 80dd 8107 303f 9da7  u>Y.H)v>....0?..
+0000dd70: d6f4 bf6d 2ed3 c77c 0100 4940 30ab 1578  ...m...|..I@0..x
+0000dd80: 0133 3100 0205 bdf4 cc92 8cd2 2486 7b8f  .31.........$.{.
+0000dd90: 0f45 3fe8 78db 2ecd bde7 c6be f99e 3c31  .E?.x.........<1
+0000dda0: 8d5c 870c 0d0c cc4c 4cc0 4a32 d3f3 f28b  .\.....LL.J2....
+0000ddb0: 5219 e6ba 4fb6 a9be 75fc a1cb f199 1d9b  R...O...u.......
+0000ddc0: e79f e1e4 facb 740a aaca c7d3 d9d5 2fd8  ......t......./.
+0000ddd0: 95c1 f07a 61c0 a977 7dbe 6f2a 3eb3 707e  ...za..w}.o*>.p~
+0000dde0: f9c7 fb6a 9be0 41a8 125f 473f 4f37 d7e0  ...j..A.._G?O7..
+0000ddf0: 10bd cc3c 8695 3e0f 176e ba71 f1f6 ad94  ...<..>..n.q....
+0000de00: 3b4f 5324 fa4b 3cf8 f599 a1ca 825c 1d5d  ;OS$.K<......\.]
+0000de10: 7c5d f572 5318 9ad4 e646 6b2e adb9 fc77  |].rS....Fk....w
+0000de20: 01fb b1e3 6d97 0425 17be 5586 2a4a 2acd  ....m..%..U.*J*.
+0000de30: 2dd0 2ba8 64b8 37f1 ce3a d555 c72f 334d  -.+.d.7..:.U./3M
+0000de40: b129 70fd d9b0 daf4 ee69 0f13 b0cf d20b  .)p......i......
+0000de50: 4ae2 93f3 730b 4a4b 528b e213 8b8b 338b  J...s.JKR.....3.
+0000de60: 4b12 f34a 1834 6bd7 8871 267e 58f7 aa58  K..J.4k..q&~X..X
+0000de70: b964 d513 b5e9 01c2 c61a 5033 8b52 0b4b  .d........P3.R.K
+0000de80: 338b 5273 53f3 4a8a f54a 2a4a 1878 26ce  3.RsS.J..J*J.x&.
+0000de90: 5873 66f3 c5b5 57b3 5da6 3d9d f84b e2f4  Xsf...W.].=..K..
+0000dea0: fa94 3f50 b5c5 a925 a560 07b0 743c 3a51  ..?P...%.`..t<:Q
+0000deb0: d63c d1c7 e8de aa15 6975 25d3 bf67 b1dc  .<......iu%..g..
+0000dec0: 0000 07d8 905a a114 7801 3334 3030 3331  .....Z..x.340031
+0000ded0: 5188 8fcf cccb 2c89 8fd7 2ba8 6428 6b2f  Q.....,...+.d(k/
+0000dee0: 7e3f 656e 8248 63f6 6fa9 8ebf 2f2f 947f  ~?en.Hc.o...//..
+0000def0: 8edf 6662 0004 0a89 e9a9 7925 0c4e 5e1b  ..fb......y%.N^.
+0000df00: 8f4c beb7 86bb df2c 5ef9 bbd1 df92 1759  .L.....,^......Y
+0000df10: 7bd6 42e5 4b53 32f3 192e 6dd4 94eb b0b1  {.B.KS2...m.....
+0000df20: 9f1b 36a9 d856 fccd 39e5 8223 7c15 8610  ..6..V..9..#|...
+0000df30: 6bd2 0b4a e293 f373 0b4a 4b52 8be2 138b  k..J...s.JKR....
+0000df40: 8b33 8b4b 12f3 4a40 968a c5c8 d63e 99c5  .3.K..J@.....>..
+0000df50: b1ea ebbc 2b56 8756 eeca d821 68f0 0262  ....+V.V...!h..b
+0000df60: 687a 6926 c382 ed92 4619 190f 9e8b 9af9  hzi&....F.......
+0000df70: bc7d 3adf 7733 ebc4 1b6e 5023 7372 7241  .}:.w3...nP#srrA
+0000df80: fa4b 3459 dd6e 3d14 48cb b1eb f8a7 6520  .K4Y.n=.H.....e 
+0000df90: 3539 7427 eb41 88fe e2e4 a2d4 d43c 86f3  59t'.A.......<..
+0000dfa0: a7fa 9b6f d97c e13a 718a 43f8 c74b a965  ...o.|.:q.C..K.e
+0000dfb0: 9212 a2b1 5023 808e 2802 3b42 c1e5 ea82  ....P#..(.;B....
+0000dfc0: f9a1 4a3b 13b3 5575 3826 2e7b b1aa fa54  ..J;..Uu8&.{...T
+0000dfd0: 0ac4 90d2 92cc 9c62 8685 6bfc 2e9d 7fdb  .......b..k.....
+0000dfe0: 167d 38a3 b2c1 ca7a e1ae 6099 a3b6 00bc  .}8....z..`.....
+0000dff0: e182 02ae 0e78 0133 3430 3033 3151 888f  .....x.340031Q..
+0000e000: cfcc cb2c 898f d72b a864 4868 356b fe68  ...,...+.dHh5k.h
+0000e010: a8c2 7268 6246 e3ba 0c0b 3389 ffaa ee86  ..rhbF....3.....
+0000e020: 1065 89e9 a979 2520 35b3 af38 fa4f 64d0  .e...y% 5..8.Od.
+0000e030: a839 7e66 a3c9 0ac6 cc7f d9cf 3e08 c3d4  .9~f........>...
+0000e040: 1417 6716 9724 42d4 6df4 9311 98f7 2d42  ..g..$B.m.....-B
+0000e050: cbe0 a774 fe1f 75ad 4f21 12d5 7550 7549  ...t..u.O!..uPuI
+0000e060: 89c9 d9e9 45f9 a579 2920 039f 4ff1 1359  ....E..y) ..O..Y
+0000e070: e297 706c 59b7 e61f 6fc3 80ed 195c ebb6  ..plY...o....\..
+0000e080: 4015 2667 2496 c467 00cd cc2f aa04 295d  @.&g$..g.../..)]
+0000e090: b66b 99d9 85af 86ce 6ab3 a7f5 441c ce90  .k......j...D...
+0000e0a0: ec9e c8fd 15aa b4a0 283f 3939 b5b8 18a4  ........(?99....
+0000e0b0: cc6e fb9e b027 f7a7 df73 ccf8 567c 692d  .n...'...s..V|i-
+0000e0c0: 4ffb 642f 1b17 007f df5d 56e4 0385 4e78  O.d/.....]V...Nx
+0000e0d0: 9c01 3400 cbff db02 db02 90f7 147e 7b95  ..4..........~{.
+0000e0e0: e19c 5a8c 333e 771f 41f2 ae7e c613 7660  ..Z.3>w.A..~..v`
+0000e0f0: e393 0b01 3c14 3e5f 999b 65e4 d565 2911  ....<.>_..e..e).
+0000e100: 1ad1 92bf c6de 425c af47 80e3 1830 ef04  ......B\.G...0..
+0000e110: 8348 789c 3bc8 7490 c9dd d0c0 c0cc c444  .Hx.;.t........D
+0000e120: 213e 3e33 2fb3 243e 5eaf a092 a1c0 6959  !>>3/.$>^.....iY
+0000e130: 40f5 eeb3 a97b 5a7f cf6e 53bb 9bf1 4af9  @....{Z..nS...J.
+0000e140: 5380 8901 1028 24a6 a7e6 9530 0489 4f29  S....($....0..O)
+0000e150: d66a 776c ba1c 75c3 fdcd a2bb ae17 265e  .jwl..u.......&^
+0000e160: 0e9c e8fe 0b00 c8c4 21e5 e403 866d 789c  ........!....mx.
+0000e170: 0134 00cb ffdb 02db 0290 f714 a285 ae6d  .4.............m
+0000e180: 645e f9a5 b7e0 055c 3d58 8af7 85e2 9dda  d^.....\=X......
+0000e190: 930b 013c 140a ac16 944d 6b28 c7fc 0599  ...<.....Mk(....
+0000e1a0: 4450 df60 a768 88f4 1fa8 0d18 f1ef 0484  DP.`.h..........
+0000e1b0: 6778 9c3b c874 90c9 ddd0 c0c0 ccc4 4421  gx.;.t........D!
+0000e1c0: 3e3e 332f b324 3e5e afa0 92c1 7fad 073f  >>3/.$>^.......?
+0000e1d0: 4f09 57c8 5595 e959 675f 1a67 1a07 f87f  O.W.U..Yg_.g....
+0000e1e0: 3731 0002 85c4 f4d4 bc12 8615 8e7d e14b  71...........}.K
+0000e1f0: 5e2c fbd4 f3a6 6b2a cbd3 9fcf b72c 96de  ^,....k*.....,..
+0000e200: 35d1 fd17 0065 fb21 1de3 0383 1678 9c01  5....e.!.....x..
+0000e210: 3300 ccff ee01 ee01 9037 1432 e83d 4fce  3........7.2.=O.
+0000e220: fa33 3703 2a82 4770 9f7b 5303 b132 e991  .37.*.Gp.{S..2..
+0000e230: 4b8f 14ad 00c6 06d0 e3aa 410f f0dd 5099  K.........A...P.
+0000e240: 3828 2b21 c02d 4530 ef15 6de4 0388 4e78  8(+!.-E0..m...Nx
+0000e250: 9c01 3400 cbff db02 db02 90f7 14f6 33ed  ..4...........3.
+0000e260: d3c7 612d cc4e de3a ff17 2ae7 a0fb 6a17  ..a-.N.:..*...j.
+0000e270: 0593 0b01 3c14 e247 eeb0 629d c5d9 881e  ....<..G..b.....
+0000e280: fe68 441c 79ff ea8f 885f c28a 1aa5 e003  .hD.y...._......
+0000e290: 8061 789c 3bc8 7490 49dd d0c0 c0cc c444  .ax.;.t.I......D
+0000e2a0: 213e 3e33 2fb3 243e 5eaf a092 6155 ceaa  !>>3/.$>^...aU..
+0000e2b0: 94b8 67b9 4d0a 4f3a ddf2 a646 c46c d158  ..g.M.O:...F.l.X
+0000e2c0: f362 a3ba 1423 00a0 3712 88e4 0389 4e78  .b...#..7.....Nx
+0000e2d0: 9c01 3400 cbff db02 db02 90f7 14be bc19  ..4.............
+0000e2e0: a285 3146 d869 74fc 1a54 96a8 ecaf c070  ..1F.it..T.....p
+0000e2f0: 0193 0b01 3c14 4508 ca52 16d7 d238 30a7  ....<.E..R...80.
+0000e300: d1ec 0df7 8aa2 6e33 cb40 8bfd 186f e403  ......n3.@...o..
+0000e310: 8a11 789c 0134 00cb ffdb 02db 0290 f714  ..x..4..........
+0000e320: 1a03 eb1a b938 e53b cd11 68ce cc2b f86e  .....8.;..h..+.n
+0000e330: 20aa 761b 930b 013c 141d 2bbf 74d8 23f9   .v....<..+.t.#.
+0000e340: 8fc2 03f0 82b5 6e91 1ffa 5049 2e5f 7817  ......n...PI._x.
+0000e350: 0de4 0384 0678 9c01 3400 cbff db02 db02  .....x..4.......
+0000e360: 90f7 14bb f307 ff3c e72e 6cf8 df49 bc07  .......<..l..I..
+0000e370: ab19 eac8 f0bf 6b93 0b01 3c14 0488 e2c8  ......k...<.....
+0000e380: 7683 914c 32de aaa8 667e 7497 f76a 04d8  v..L2...f~t..j..
+0000e390: cce3 1ac3 ef01 832a 789c bbcd 749b 69c2  .......*x...t.i.
+0000e3a0: 7791 c2c7 5b78 cf2c 5be0 e820 f2b7 bdc5  w...[x.,[.. ....
+0000e3b0: 4a4b fec9 fb7d 0d93 b919 0300 f61c 0e9d  JK...}..........
+0000e3c0: e403 2c78 9c01 3400 cbff db02 db02 90f7  ..,x..4.........
+0000e3d0: 1402 e2e3 ff9b 9ab5 a564 6b8d 52d2 fcc1  .........dk.R...
+0000e3e0: c5ab 6ccf fa93 0b01 3c14 3e5f 999b 65e4  ..l.....<.>_..e.
+0000e3f0: d565 2911 1ad1 92bf c6de 425c af47 f0b7  .e).......B\.G..
+0000e400: 1b7e ef01 8237 789c 011f 00e0 ffdb 02db  .~...7x.........
+0000e410: 0290 f714 f98a 9ff7 dbca 4e98 b5ba 343a  ..........N...4:
+0000e420: 83cd 588a 0d29 54a5 930b 0150 103d 0f27  ..X..)T....P.=.'
+0000e430: e003 896a 789c 3bc8 7490 49dd d0c0 c0cc  ...jx.;.t.I.....
+0000e440: c444 213e 3e33 2fb3 243e 5eaf a092 e1a7  .D!>>3/.$>^.....
+0000e450: 6463 eb61 1f41 d11a 47a9 c38b 2fbe 5ce2  dc.a.A..G.../.\.
+0000e460: 1292 7e71 a3ba 1423 0093 7911 efe0 0385  ..~q...#..y.....
+0000e470: 5f78 9c3b c874 9049 ddd0 c0c0 ccc4 4421  _x.;.t.I......D!
+0000e480: 3e3e 332f b324 3e5e afa0 92a1 acbd f8fd  >>3/.$>^........
+0000e490: 94b9 0922 8dd9 bfa5 3afe bebc 50fe 397e  ..."....:...P.9~
+0000e4a0: db46 7529 4600 ae4a 13f9 ee01 847d 789c  .Fu)F..J.....}x.
+0000e4b0: 3bc8 7490 6982 b1c8 6a17 ff75 871b 1aa2  ;.t.i...j..u....
+0000e4c0: 7ee4 2bef 4eb7 6998 22cb bec3 7da2 fb2f  ~.+.N.i."...}../
+0000e4d0: 00c8 920d 58e0 032b 789c 3bc8 7490 49dd  ....X..+x.;.t.I.
+0000e4e0: d0c0 c0cc c444 213e 3e33 2fb3 243e 5eaf  .....D!>>3/.$>^.
+0000e4f0: a092 a1c0 6959 40f5 eeb3 a97b 5a7f cf6e  ....iY@....{Z..n
+0000e500: 53bb 9bf1 4af9 53c0 4675 2946 00a9 d913  S...J.S.Fu)F....
+0000e510: 5ee0 0367 789c 3bc8 7490 49dd d0c0 c0cc  ^..gx.;.t.I.....
+0000e520: c444 213e 3e33 2fb3 243e 5eaf a092 6155  .D!>>3/.$>^...aU
+0000e530: ceaa 94b8 67b9 4d0a 4f3a ddf2 a646 c46c  ....g.M.O:...F.l
+0000e540: d158 f362 a3ba 1423 00a0 3712 88e0 0384  .X.b...#..7.....
+0000e550: 3f78 9c3b c874 9049 ddd0 c0c0 ccc4 4421  ?x.;.t.I......D!
+0000e560: 3e3e 332f b324 3e5e afa0 92c1 7445 e8dc  >>3/.$>^....tE..
+0000e570: befe e609 6da7 f756 182d 9dc3 7b9f 2ffa  ....m..V.-..{./.
+0000e580: db46 7529 4600 9ed5 127a b103 789c 4b2b  .Fu)F....z..x.K+
+0000e590: cacf 55d0 2b2e 492c 2a51 c8cc 2dc8 0752  ..U.+.I,*Q..-..R
+0000e5a0: 600e 1717 577c 7c59 6a51 7166 7e5e 7cbc  `...W||YjQqf~^|.
+0000e5b0: 82ad 82ba 819e a99e 993a 1700 b224 0fa6  .........:...$..
+0000e5c0: eb01 8a4d 789c 7bc7 f88e 71c2 2d91 6b6f  ...Mx.{...q.-.ko
+0000e5d0: 6f69 f596 666d 9699 b77f 8acf 06cb 09ae  oi..fm..........
+0000e5e0: 4e5a d500 c7b3 0d41 ee01 865f 789c 011e  NZ.....A..._x...
+0000e5f0: 00e1 ffee 01ee 0190 3714 9bd4 414f 9100  ........7...AO..
+0000e600: 287c c7cc b134 a801 69fe 6be6 f013 914b  (|...4..i.k....K
+0000e610: a3d2 4c0e 49ba 3b78 9cbd 52bb 6edc 3010  ..L.I.;x..R.n.0.
+0000e620: ecf5 150b b991 8203 3f20 c015 2912 2040  ........? ..). @
+0000e630: 0ac3 4e8a 2008 e43d 6a25 11a1 489a 5cda  ..N. ..=j%..H.\.
+0000e640: f1df 6749 ddc3 38b8 4a61 16a2 48cd ccee  ..gI..8.Ja..H...
+0000e650: 8c76 8a7e 05a5 ac5d c1ac c147 860f 4d59  .v.~...]...G..MY
+0000e660: 53b9 b7e8 e639 6258 945e 48ff 09de 3856  S....9bX.^H...8V
+0000e670: e9d1 1aa6 13fa be9e eef1 8962 f316 3144  ...........b..1D
+0000e680: 3a64 63f9 84d7 0bf2 8033 391e e82f e9cc  :dc......39../..
+0000e690: 3e9e 4839 24ef 8c3e 21bf 9b59 34d9 7b9b  >.H9$..>!..Y4.{.
+0000e6a0: 60bf 9dba 7e3b 2b72 78b0 34a0 d087 488f  `...~;+rx.4...H.
+0000e6b0: d944 5a45 b200 bfa0 4d74 a66d f0d2 8e14  .DZE....Mt.m....
+0000e6c0: 364e 0446 9a60 a6eb 1eba fe63 03b2 2271  6N.F.`.....c.."q
+0000e6d0: 8eee ad2e 958e 844c 4351 1c34 5a6b dc7c  .......LCQ.4Zk.|
+0000e6e0: a117 c5d5 8f64 bb7e b715 ed4b 186d db5e  .....d.~...K.m.^
+0000e6f0: 02a9 1da8 aa9a ce26 057a 8510 d140 d114  .......&.z...@..
+0000e700: 3f68 5566 2301 1b3a 336e 5f78 f1ee eef3  ?hUf#..:3n_x....
+0000e710: edb7 26d4 5709 2058 b17a f920 2e6f e0a7  ..&.W. X.z. .o..
+0000e720: cfa0 51ac d4b6 8117 aa7d c903 02a6 5476  ..Q......}....Tv
+0000e730: f95a bb69 8a42 3556 8296 adab 5938 5c69  .Z.i.B5V....Y8\i
+0000e740: dfbe 2ad2 eeea fd48 4947 13d8 78b7 6f3f  ..*....HIG..x.o?
+0000e750: 1deb 425a c85a 053f 52a9 65aa fe96 0ec1  ..BZ.Z.?R.e.....
+0000e760: 2601 daaf 2bba 3129 f8ea 4266 61f8 6c47  &...+.1)..Bfa.lG
+0000e770: 3810 203c a135 e315 5070 13bc 888d 6774  8. <.5..Pp....gt
+0000e780: 5cf4 126d 3e7c e6c2 f7d3 46cc b4ab b0a3  \..m>|....F.....
+0000e790: 5e88 32a5 60b8 c0e0 d9f0 020f f5aa 534a  ^.2.`.........SJ
+0000e7a0: f50f ea68 62ca 4eef 5f79 5331 bb5d d3ff  ...hb.N._yS1.]..
+0000e7b0: d7fc bec3 48fd 3aff a2df 7d9d aaa6 f907  ....H.:...}.....
+0000e7c0: 8fbe 5167 ba26 789c 8d90 4f4b c430 10c5  ..Qg.&x...OK.0..
+0000e7d0: effd 14a1 a714 245d f5b6 d08b 7a58 4111  ......$]....zXA.
+0000e7e0: 5d2f 2212 d224 ed0e e6cf 9aa4 8722 7e77  ]/"..$......."~w
+0000e7f0: 63da ba6e a968 6e99 79bf 9979 af71 5623  c..n.hn.y..y.qV#
+0000e800: c54c cb77 0c0c e556 ebce 40e8 49fc 07aa  .L.w...V..@.I...
+0000e810: a5f7 ac95 7407 3e58 07d2 23d0 7beb 02da  ....t.>X..#.{...
+0000e820: dedf 5c46 c1ed d0df a476 9f35 5fc3 48cd  ..\F.....v.5_.H.
+0000e830: f86b eb6c 67c4 a456 4a8f 237a 6aa1 05c3  .k.lg..VJ.#zj...
+0000e840: 5496 8d3d eb47 8c74 0194 27a2 9ea8 5686  T..=.G.t..'...V.
+0000e850: 6f4a d459 7c42 36a9 ba70 5b8f 8b75 86e2  oJ.Y|B6..p[..u..
+0000e860: db3b 3001 e79b ebed e3dd c313 baba c84f  .;0............O
+0000e870: 6693 7051 2425 b7c6 481e c01a 542d 1bc2  f.pQ$%..H...T-..
+0000e880: 49e7 632d 8a28 882a 6735 3f3d 3b8f 230f  I.c-.(.*g5?=;.#.
+0000e890: 30f5 21ae 6cab 26f7 6f0a 825c 9765 f93e  0.!.l.&.o..\.e.>
+0000e8a0: dff8 910f 3ba1 414a 1a7c a0c9 68c3 17a8  ....;.AJ.|..h...
+0000e8b0: aad0 6af0 707c 1d61 424c 6ef1 4294 cfab  ..j.p|.aBLn.B...
+0000e8c0: 9722 4b9c 93a1 73e6 073a 9487 e0b8 92cc  ."K...s..:......
+0000e8d0: 0dd1 cd22 fb3d 5292 205c fc25 fbcf 859f  ...".=R. \.%....
+0000e8e0: f97d d72f b8d6 0278 01ed 574b 6f1b 3710  .}./...x..WKo.7.
+0000e8f0: beeb 5710 3aad 1297 4872 34a0 638b a6c8  ..W.:...Hr4.c...
+0000e900: c368 65f4 e018 04b5 4b69 592f 970b 929b  .he.....KiY/....
+0000e910: 5aff be33 e492 fb12 2cb9 89d3 1ec4 83b1  Z..3....,.......
+0000e920: 22e7 cd6f bea1 7746 2b42 6955 2922 55a3  "..o..wF+BiU)"U.
+0000e930: 8d23 af16 3bbf c7ad 95d6 f1da f507 dd49  .#..;..........I
+0000e940: 5e72 c74a 38d4 e630 3ba4 bc2d a4a6 ced9  ^r.J8..0;..-....
+0000e950: 78e4 c4a3 634e 33db 0891 979d 8d4e ccba  x...cN3......N..
+0000e960: 643e 1ca3 202a 2cc6 7246 e4da 14d1 a277  d>.. *,.rF.....w
+0000e970: c10a eef8 22c9 ed5b 49ad dcd7 bc8a 52e1  ...."..[I.....R.
+0000e980: 172b 795d 54c2 2c16 5d7e ae34 8217 b2de  .+y]T.,.]~.4....
+0000e990: 47dd e6b0 e74a 442d 251f 5138 494b 25e2  G....JD-%.Q8IK%.
+0000e9a0: b701 4b5a c5c0 5a27 2b4b 8b6d 547c 054a  ..KZ..Z'+K.mT|.J
+0000e9b0: b042 f1e8 f4d4 1eac 138a 59dd d605 ab74  .B........Y....t
+0000e9c0: ce9d d4f5 1551 3267 21b7 c1e6 5fad 75cc  .....Q2g!..._.u.
+0000e9d0: e646 88da 96da b186 bbf2 8a4c 36c0 5521  .F.........L6.U!
+0000e9e0: 76a4 313a 17d6 325f 92cc f107 31d0 5c6f  v.1:..2_....1.\o
+0000e9f0: 4c2b ae48 d80d 0178 b9f5 2fbc b270 50e8  L+.H...x../..pP.
+0000ea00: 1a1c f1af 8249 c5f7 226c afae 1704 d6be  .....I.."l......
+0000ea10: d25b a8e5 b0d4 b8bd f087 0e4a 01f1 c806  .[.........J....
+0000ea20: b320 6b32 bebb ec48 56ab a028 77f3 68ae  . k2...HV..(w.h.
+0000ea30: c311 5a1f d97d 3737 7cb4 8a9d 691f 18e0  ..Z..}77|...i...
+0000ea40: 98c9 ba69 1de8 2e6f fff8 f9f7 6bb2 7c3d  ...i...o....k.|=
+0000ea50: b2fa 541c 1802 aede ca6b 3043 bed4 e4b3  ..T......k0C....
+0000ea60: 2b85 217a 478e da7c 178c a29a 6e5d f09e  +.!zG..|....n]..
+0000ea70: da27 4bd6 aec8 5e38 e6bb 47c1 9d41 c563  .'K...^8..G..A.c
+0000ea80: 1765 2bda edd8 4ea8 92a2 76d9 6a76 edeb  .e+...N...v.jv..
+0000ea90: 090c 48aa 68c2 0b11 70b9 e493 ae05 5426  ..H.h...p.....T&
+0000eaa0: a53b b9eb 70c9 986c de1a 03be aa03 8b21  .;..p..l.......!
+0000eab0: 40ed ce08 d4d7 1b0d cc23 e88d e379 c501  @........#...y..
+0000eac0: ce9d 6d30 3df7 77f7 d3db 7b9a 0316 218c  ..m0=.w...{...!.
+0000ead0: bb37 f7c9 302a cfa5 a911 4a7f 15d9 fc04  .7..0*....J.....
+0000eae0: ed74 6040 555c 4fe4 9157 829b 6c35 f2b6  .t`@U\O..W..l5..
+0000eaf0: d386 c448 657d c4f9 38b3 131e 7851 c4bc  ...He}..8...xQ..
+0000eb00: b3ce ead8 dd13 d10d 757f 6d15 af3f 06c4  ........u.m..?..
+0000eb10: 645d 9dd6 77c3 b2de afba bccf b4d8 2335  d]..w.........#5
+0000eb20: d40c 13e9 f7e0 92fa 1fc3 cb09 606a 8c04  ............`j..
+0000eb30: 682e ff2c 7525 c887 0f1f c9e7 dbcd cded  h..,u%..........
+0000eb40: 6679 16bc 4301 7cd1 c7fc 4c53 c300 21da  fy..C.|...LS..!.
+0000eb50: 46d7 56c0 072f 0e54 2809 9d90 805c 6b18  F.V../.T(....\k.
+0000eb60: 1996 7992 f4a3 45e9 4254 8ce7 4e02 2a3a  ..y...E.BT..N.*:
+0000eb70: f6c2 8492 19e4 4fc8 693c 877c 5b86 6e1d  ......O.i<.|[.n.
+0000eb80: 60c6 536a c50f 7e06 0d8d a1c1 8eda f70d  `.Sj..~.........
+0000eb90: 34b1 56d0 e6c2 b014 751c 0340 1481 81d8  4.V.....u..@....
+0000eba0: 563f 8ec0 857d 323c a44e df54 5cd6 1b18  V?...}2<.N.T\...
+0000ebb0: 77d9 8aac 816a 9673 7c8d 55ac 705e bcbf  w....j.s|.U.p^..
+0000ebc0: 9f01 a242 8930 d294 4618 0b83 a2e0 69d3  ...B.0..F.....i.
+0000ebd0: 2738 0ad0 8f3e 2a6b 5f6e 148c 2b1c a8d6  '8...>*k_n..+...
+0000ebe0: ca9c 569a 17d9 a8b4 8308 4061 288b 8e26  ..V.......@a(..&
+0000ebf0: 1df6 7729 0135 4321 84ec b6b5 2078 2479  ..w).5C!.... x$y
+0000ec00: 98be d456 4234 d91b fa76 ece8 347c e081  ...VB4...v..4|..
+0000ec10: d234 a288 008a d974 9c88 3f31 c02d cf1f  .4.....t..?1.-..
+0000ec20: 5878 1420 48e2 eb80 6efc 178c 5403 11ae  Xx. H...n...T...
+0000ec30: 7dcd 7c35 fb28 26da 145e 4b06 918a 9691  }.|5.(&..^K.....
+0000ec40: 83fb 7cd2 7d20 06a7 897e 23ac 9e01 1088  ..|.} ...~#.....
+0000ec50: ebd9 554b 0899 647b aa56 98e9 e952 4d5e  ..UK..d{.V...RM^
+0000ec60: 31fd 70c3 2205 3cfb 0010 efb3 b9be 7c4f  1.p.".<.......|O
+0000ec70: 9005 fc8b 82f0 c103 8912 24f2 836e 89d3  ..........$..n..
+0000ec80: 4003 4aa8 ad30 94fc 86c2 961f 887e a04b  @.J..0.......~.K
+0000ec90: 6fb6 a332 24b1 f79f 80c3 48e6 0df6 61ac  o..2$.....H...a.
+0000eca0: 80d5 92ef 8e27 fade 831a a4fe ffce 63de  .....'........c.
+0000ecb0: d35b 1f87 7f03 827f bf10 5f2f 4df4 e808  .[........_/M...
+0000ecc0: fd9c c6cb 0f23 690c 07d7 4b36 d385 a3a1  .....#i...K6....
+0000ecd0: c0ff 0b8e f657 0d7f fe2d ff5c b8fa fcb9  .....W...-.\....
+0000ece0: 761e 57a7 1b01 6af0 3dd8 fdeb e967 9a37  v.W...j.=....g.7
+0000ecf0: 719a b251 2c52 cb0f e1d1 f46f 50a0 b317  q..Q,R.....oP...
+0000ed00: a74d 2cd2 8533 6f2e ef5a fa1f bc6b 5387  .M,..3o..Z...kS.
+0000ed10: c68f 67be d92e 9cf9 629c f90f 5136 db93  ..g.....b...Q6..
+0000ed20: e002 873c 789c 7ba1 7559 6b43 2dfb e618  ...<x.{.uYkC-...
+0000ed30: a142 c6cd 5f39 7458 802c 1ee6 cd26 028a  .B.._9tX.,...&..
+0000ed40: 4c60 1600 cae7 0a31 b13a 789c 7d53 5d6f  L`.....1.:x.}S]o
+0000ed50: d430 107c f7af 30ee 432f 281f 952a 108a  .0.|..0.C/(..*..
+0000ed60: 6444 250a 42a2 2a82 f601 5528 7293 bd9c  dD%.B.*...U(r...
+0000ed70: b9c4 36de 35ed 81f8 eff8 9c0b a855 eff2  ..6.5........U..
+0000ed80: e087 99f1 eeec ac73 f4ac 0ae8 ab5b 6d2a  .......s.....[m*
+0000ed90: b7a1 9535 a7ec 8817 cf0b deda 4e9b bee6  ...5........N...
+0000eda0: 8196 c5ab 2dc2 d8d2 db91 2350 7064 ed80  ....-.....#Ppd..
+0000edb0: 5c8f ce7a 9a10 c6ee 34ad b875 6016 c71e  \..z....4..u`...
+0000edc0: 7e04 ed61 0443 58d2 3d1d 675c 215f ba9a  ~..a.CX.=.g\!_..
+0000edd0: f1f8 6983 a486 a1d9 a990 cb48 951e 54b7  ..i........H..T.
+0000ede0: c858 2ab6 483a a346 90a2 77d4 b476 7481  .X*.H:.F..w..vt.
+0000edf0: c037 0a51 c7cb 8644 9e24 3fc1 a3b6 468a  .7.Q...D.$?...F.
+0000ee00: 93f2 4579 ba03 3bc0 d66b 4789 10e2 fda7  ..Ey..;..kG.....
+0000ee10: ab78 4ed4 604d df3c e4cb ef56 9b45 f22d  .xN.`M.<...V.E.-
+0000ee20: 3e9f 9fbd bd38 2fc7 4ee4 1ccc 9480 1429  >....8/.N......)
+0000ee30: 0191 2587 8336 808b 2c7b ba5c 346a 280e  ..%..6..,{.\4j(.
+0000ee40: ddd0 c645 eb04 f754 8dca af3b 7b67 760e  ...E...T...;{gv.
+0000ee50: 821f a458 1139 acab aa8f 9185 db32 8e57  ...X.9.......2.W
+0000ee60: 5913 bc22 b556 a68a 1317 f3c4 c5e3 8955  Y..".V.........U
+0000ee70: 884b f252 5c46 3d3f 4b17 f8f5 c7eb 2f97  .K.R\F=?K...../.
+0000ee80: 5f1f 081a 1895 8e9d 62c9 cef6 ca9c bc7c  _.......b......|
+0000ee90: d36f 916d af39 0bdd 82c1 68f3 e2c3 d50e  .o.m.9....h.....
+0000eea0: 72aa 5dab 1e50 deec 8d9d ef61 ca78 ef20  r.]..P.....a.x. 
+0000eeb0: df07 7d80 8d11 0298 0382 407a c043 ed43  ..}.......@z.C.C
+0000eec0: a7ad f896 3ff9 c2e4 6360 9245 c37e d3b8  ....?...c`.E.~..
+0000eed0: b87f 42f9 3b41 db4f c42d a21d a099 f68a  ..B.;A.O.-......
+0000eee0: a2e6 3762 6ef9 afa3 dc37 0929 4f75 3a67  ..7bn....7.)Ou:g
+0000eef0: 3b7f f2a9 f094 71fa cbfe 5b13 af25 9f5f  ;.....q...[..%._
+0000ef00: ee2f ed1a 544b 90ef d480 90b3 8c31 f617  ./..TK.......1..
+0000ef10: ed83 3928 6c82 4c78 9c5b c8be 907d c269  ..9(l.Lx.[...}.i
+0000ef20: 4693 8d67 ae32 0100 2059 0535 6c18 789c  F..g.2.. Y.5l.x.
+0000ef30: 5bc8 be90 7dc2 6946 d38d 67ae 3201 0020  [...}.iF..g.2.. 
+0000ef40: 5e05 366c 1778 9c5b c8be 907d c269 46b3  ^.6l.x.[...}.iF.
+0000ef50: 8d67 ae32 0100 2063 0537 b103 789c 4b2b  .g.2.. c.7..x.K+
+0000ef60: cacf 55d0 2b2e 492c 2a51 c8cc 2dc8 0752  ..U.+.I,*Q..-..R
+0000ef70: 600e 1717 577c 7c59 6a51 7166 7e5e 7cbc  `...W||YjQqf~^|.
+0000ef80: 82ad 82ba 819e a99e a93a 1700 b221 0fa5  .........:...!..
+0000ef90: b103 789c 4b2b cacf 55d0 2b2e 492c 2a51  ..x.K+..U.+.I,*Q
+0000efa0: c8cc 2dc8 0752 600e 1717 577c 7c59 6a51  ..-..R`...W||YjQ
+0000efb0: 7166 7e5e 7cbc 82ad 82ba 819e a99e 893a  qf~^|..........:
+0000efc0: 1700 b21e 0fa4 b103 789c 4b2b cacf 55d0  ........x.K+..U.
+0000efd0: 2b2e 492c 2a51 c8cc 2dc8 0752 600e 1717  +.I,*Q..-..R`...
+0000efe0: 577c 7c59 6a51 7166 7e5e 7cbc 82ad 82ba  W||YjQqf~^|.....
+0000eff0: 819e a99e b13a 1700 b21b 0fa3 0694 3882  .....:........8.
+0000f000: 1218 a77c 1378 81c8 0226 39fb 9c2f 8ee4  ...|.x...&9../..
```

### Comparing `gpt_computer_assistant-0.5.5/.github/workflows/deploys.yml` & `gpt_computer_assistant-0.5.6/.github/workflows/deploys.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.github/workflows/release.yml` & `gpt_computer_assistant-0.5.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.github/workflows/release_generation.yml` & `gpt_computer_assistant-0.5.6/.github/workflows/release_generation.yml`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/.gitignore` & `gpt_computer_assistant-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/LICENSE` & `gpt_computer_assistant-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/PKG-INFO` & `gpt_computer_assistant-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt_computer_assistant
-Version: 0.5.5
+Version: 0.5.6
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.5.5 Summary: GPT
+Metadata-Version: 2.1 Name: gpt_computer_assistant Version: 0.5.6 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
 pipeline to providing native install scripts (.exe). ![intro](https://
 github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
```

### Comparing `gpt_computer_assistant-0.5.5/README.md` & `gpt_computer_assistant-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/bump.py` & `gpt_computer_assistant-0.5.6/bump.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/agent.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/agent.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/assistant.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/background.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/background.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/chat_history.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/chat_history.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/agent/proccess.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/agent/proccess.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     signal_handler.assistant_response_ready.emit()
 
     if not is_just_text_model_active():
         response_path = text_to_speech(llm_output)
 
         def play_text():
             from ..gpt_computer_assistant import the_input_box
-            if the_input_box.toPlainText() == "":
+            if the_input_box.text() == "":
                 the_input_box.setText(llm_output)
          
 
         def play_audio():
             play_text()
             mixer.init()
             mixer.music.load(response_path)
@@ -123,15 +123,15 @@
 
     signal_handler.assistant_response_ready.emit()
 
     if not is_just_text_model_active():
         response_path = text_to_speech(llm_output)
         def play_text():
             from ..gpt_computer_assistant import the_input_box
-            if the_input_box.toPlainText() == "":
+            if the_input_box.text() == "":
                 the_input_box.setText(llm_output)
          
 
         def play_audio():
             play_text()
             mixer.init()
             mixer.music.load(response_path)
@@ -176,15 +176,15 @@
 
     signal_handler.assistant_response_ready.emit()
 
     if not is_just_text_model_active():
         response_path = text_to_speech(llm_output)
         def play_text():
             from ..gpt_computer_assistant import the_input_box
-            if the_input_box.toPlainText() == "":
+            if the_input_box.text() == "":
                 the_input_box.setText(llm_output)
          
 
         def play_audio():
             play_text()
             mixer.init()
             mixer.music.load(response_path)
```

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/record.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/record.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/stt.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/stt.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/audio/tts.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/audio/tts.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/gpt_computer_assistant.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/gpt_computer_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/gui/button.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/gui/button.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/start.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/start.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/db.py` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/db.py`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_24.png` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_24.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_256.png` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_256.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_32.png` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_32.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant/utils/media/icon_48.png` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant/utils/media/icon_48.png`

 * *Files identical despite different names*

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/PKG-INFO` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-computer-assistant
-Version: 0.5.5
+Version: 0.5.6
 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant
 Author: Onur Atakan ULUSOY
 Author-email: atadogan06@gmail.com
 License: MIT
 Description: # GPT Computer Assistant
         Hi, this is an unofficial work for providing ChatGPT MacOS app to Windows and Linux. In this way this is a fresh and stable work. You can easily install as Python library for this time but we will prepare a pipeline to providing native install scripts (.exe).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.5.5 Summary: GPT
+Metadata-Version: 2.1 Name: gpt-computer-assistant Version: 0.5.6 Summary: GPT
 Home-page: https://github.com/onuratakan/gpt-computer-assistant Author: Onur
 Atakan ULUSOY Author-email: atadogan06@gmail.com License: MIT Description: #
 GPT Computer Assistant Hi, this is an unofficial work for providing ChatGPT
 MacOS app to Windows and Linux. In this way this is a fresh and stable work.
 You can easily install as Python library for this time but we will prepare a
 pipeline to providing native install scripts (.exe). ![intro](https://
 github.com/onuratakan/gpt-computer-assistant/assets/41792982/d44d0efd-7354-
```

### Comparing `gpt_computer_assistant-0.5.5/gpt_computer_assistant.egg-info/SOURCES.txt` & `gpt_computer_assistant-0.5.6/gpt_computer_assistant.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 ./.git/logs/refs/remotes/origin/Added-icon
 ./.git/logs/refs/remotes/origin/Added-input-box-and-button
 ./.git/logs/refs/remotes/origin/Added-just-text-mode
 ./.git/logs/refs/remotes/origin/Added-reset-system
 ./.git/logs/refs/remotes/origin/Added-splitting-long-audios
 ./.git/logs/refs/remotes/origin/Fixed-high-delay-problem
 ./.git/logs/refs/remotes/origin/master
-./.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.idx
-./.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.pack
-./.git/objects/pack/pack-7f7d2c812fc9c652e0377f6b4148f38151d8a136.rev
+./.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.idx
+./.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.pack
+./.git/objects/pack/pack-069438821218a77c137881c8022639fb9c2f8ee4.rev
 ./.git/refs/heads/master
 ./.git/refs/remotes/origin/Added-different-profiles-mode
 ./.git/refs/remotes/origin/Added-icon
 ./.git/refs/remotes/origin/Added-input-box-and-button
 ./.git/refs/remotes/origin/Added-just-text-mode
 ./.git/refs/remotes/origin/Added-reset-system
 ./.git/refs/remotes/origin/Added-splitting-long-audios
@@ -59,14 +59,15 @@
 ./.git/refs/tags/v0.4.0
 ./.git/refs/tags/v0.5.0
 ./.git/refs/tags/v0.5.1
 ./.git/refs/tags/v0.5.2
 ./.git/refs/tags/v0.5.3
 ./.git/refs/tags/v0.5.4
 ./.git/refs/tags/v0.5.5
+./.git/refs/tags/v0.5.6
 ./.github/workflows/deploys.yml
 ./.github/workflows/release.yml
 ./.github/workflows/release_generation.yml
 ./gpt_computer_assistant/__init__.py
 ./gpt_computer_assistant/gpt_computer_assistant.py
 ./gpt_computer_assistant/llm.py
 ./gpt_computer_assistant/start.py
```

### Comparing `gpt_computer_assistant-0.5.5/setup.py` & `gpt_computer_assistant-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import setup
 
 with open('requirements.txt') as fp:
     install_requires = fp.read()
 setup(
     name="gpt_computer_assistant",
-    version="0.5.5",
+    version="0.5.6",
     description="""GPT""",
     long_description="".join(open("README.md", encoding="utf-8").readlines()),
     long_description_content_type="text/markdown",
     url="https://github.com/onuratakan/gpt-computer-assistant",
     author="Onur Atakan ULUSOY",
     author_email="atadogan06@gmail.com",
     license="MIT",
```

