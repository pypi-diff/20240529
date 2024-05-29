# Comparing `tmp/ytdl_sub-2024.5.11.tar.gz` & `tmp/ytdl_sub-2024.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ytdl_sub-2024.5.11.tar", last modified: Sat May 11 02:58:38 2024, max compression
+gzip compressed data, was "ytdl_sub-2024.5.29.tar", last modified: Wed May 29 02:49:21 2024, max compression
```

## Comparing `ytdl_sub-2024.5.11.tar` & `ytdl_sub-2024.5.29.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.873420 ytdl_sub-2024.5.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_transaction_log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.877420 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/dl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/config_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/overrides.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/preset_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/preset_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/variable_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/source_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdl_options_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.881420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/base_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry_parent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.885420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/custom_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/function_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    42312 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.885420 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/override_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/audio_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/date_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/embed_thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/file_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_include.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/match_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/music_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/output_directory_nfo_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/split_by_chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/throttle_protection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/plugins/video_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/internal/view.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/singles.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.889420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.893420 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/boolean_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/conditional_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/date_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/json_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/numeric_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/regex_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/string_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/script_output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/array.py
--rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/resolvable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/syntax_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable_dependency.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exception_formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/name_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/type_checking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/base_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_download.py
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.897420 ytdl_sub-2024.5.11/src/ytdl_sub/thread/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/thread/log_entries_downloaded_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.901420 ytdl_sub-2024.5.11/src/ytdl_sub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/ffmpeg.py
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/scriptable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/subtitles.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/thumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.901420 ytdl_sub-2024.5.11/src/ytdl_sub/validators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/audo_codec_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/file_path_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/nfo_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/regex_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/source_variable_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/strict_dict_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_formatter_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_select_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/validators/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-05-11 02:58:27.000000 ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:58:38.905420 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    51272 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 02:58:38.000000 ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.921910 ytdl_sub-2024.5.29/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    51271 2024-05-29 02:49:21.921910 ytdl_sub-2024.5.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9325 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:49:21.921910 ytdl_sub-2024.5.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.889910 ytdl_sub-2024.5.29/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.893910 ytdl_sub-2024.5.29/src/ytdl_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.897909 ytdl_sub-2024.5.29/src/ytdl_sub/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9286 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/output_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/output_transaction_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.897909 ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/dl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6683 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.897909 ytdl_sub-2024.5.29/src/ytdl_sub/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9123 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/config_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/overrides.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.897909 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7360 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/plugin_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/plugin_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/preset_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/preset_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.897909 ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/variable_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/info_json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/info_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6619 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/info_json/info_json_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/source_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20577 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12438 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/ytdl_options_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10134 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/ytdlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/entries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/base_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9628 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/entry_parent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/custom_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/function_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42312 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/variable_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/variable_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.901910 ytdl_sub-2024.5.29/src/ytdl_sub/entries/variables/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/entries/variables/override_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.905910 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/audio_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14569 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/date_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/embed_thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8339 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/file_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/filter_exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/filter_include.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.905910 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/internal/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/match_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/music_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/output_directory_nfo_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/split_by_chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/throttle_protection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/plugins/video_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.905910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.905910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/players.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    23681 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/url.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.905910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/internal/view.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.909910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/singles.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.909910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.909910 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34839 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.909910 ytdl_sub-2024.5.29/src/ytdl_sub/script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.913910 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/boolean_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/conditional_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/date_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/json_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/numeric_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/regex_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/string_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21725 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22535 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/script_output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.913910 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11506 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/resolvable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/syntax_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/types/variable_dependency.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.913910 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/exception_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/name_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9293 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/type_checking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.913910 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/base_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16237 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_ytdl_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.913910 ytdl_sub-2024.5.29/src/ytdl_sub/thread/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/thread/log_entries_downloaded_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.917910 ytdl_sub-2024.5.29/src/ytdl_sub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/ffmpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/scriptable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.917910 ytdl_sub-2024.5.29/src/ytdl_sub/validators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/audo_codec_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/file_path_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/nfo_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/regex_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/source_variable_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/strict_dict_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9068 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_formatter_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_select_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9352 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/validators/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.921910 ytdl_sub-2024.5.29/src/ytdl_sub/ytdl_additions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/ytdl_additions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23454 2024-05-29 02:49:09.000000 ytdl_sub-2024.5.29/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:49:21.921910 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51271 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 02:49:21.000000 ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/top_level.txt
```

### Comparing `ytdl_sub-2024.5.11/LICENSE` & `ytdl_sub-2024.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/PKG-INFO` & `ytdl_sub-2024.5.29/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.5.11
+Version: 2024.5.29
 Summary: Automate downloading metadata generation with YoutubeDL
 Author: Jesse Bannon
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,27 +685,27 @@
 Classifier: License :: Public Domain
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yt-dlp==2024.04.09
+Requires-Dist: yt-dlp==2024.5.27
 Requires-Dist: colorama~=0.4
 Requires-Dist: mergedeep~=1.3
 Requires-Dist: mediafile~=0.12
 Requires-Dist: PyYAML~=6.0
 Provides-Extra: test
 Requires-Dist: coverage[toml]<8.0,>=6.3; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
 Requires-Dist: pytest-rerunfailures~=14.0; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black==24.4.2; extra == "lint"
 Requires-Dist: isort==5.13.2; extra == "lint"
-Requires-Dist: pylint==3.1.0; extra == "lint"
+Requires-Dist: pylint==3.2.0; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0; extra == "docs"
 Requires-Dist: sphinx-book-theme~=1.0; extra == "docs"
 Provides-Extra: build
 Requires-Dist: build~=1.2; extra == "build"
 Requires-Dist: twine~=5.0; extra == "build"
```

### Comparing `ytdl_sub-2024.5.11/README.md` & `ytdl_sub-2024.5.29/README.md`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/pyproject.toml` & `ytdl_sub-2024.5.29/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Topic :: Multimedia :: Video",
     "License :: Public Domain",
     "Environment :: Console",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "yt-dlp==2024.04.09",
+    "yt-dlp==2024.5.27",
     "colorama~=0.4",
     "mergedeep~=1.3",
     "mediafile~=0.12",
     "PyYAML~=6.0",
 ]
 urls = { Homepage = "https://github.com/jmbannon/ytdl-sub" }
 
@@ -45,15 +45,15 @@
     "coverage[toml]>=6.3,<8.0",
     "pytest>=7.2,<9.0",
     "pytest-rerunfailures~=14.0",
 ]
 lint = [
     "black==24.4.2",
     "isort==5.13.2",
-    "pylint==3.1.0",
+    "pylint==3.2.0",
 ]
 docs = [
     "sphinx~=7.0",
     "sphinx-rtd-theme~=2.0",
     "sphinx-book-theme~=1.0",
 ]
 build = [
```

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/cli/entrypoint.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_summary.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/cli/output_summary.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/cli/output_transaction_log.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/cli/output_transaction_log.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/dl.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/dl.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/cli/parsers/main.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/cli/parsers/main.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/config_file.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/config_file.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/config_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/config_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/defaults.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/defaults.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/overrides.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/overrides.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/plugin_mapping.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/plugin_mapping.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/plugin/preset_plugins.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/plugin/preset_plugins.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/preset.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/preset.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/preset_options.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/preset_options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/options.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/config/validators/variable_validation.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/config/validators/variable_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/info_json/info_json_downloader.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/info_json/info_json_downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/source_plugin.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/source_plugin.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/downloader.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/downloader.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/url/validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/url/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdl_options_builder.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/ytdl_options_builder.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/downloaders/ytdlp.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/downloaders/ytdlp.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/base_entry.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/base_entry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/entry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/entry_parent.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/entry_parent.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/custom_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/custom_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/function_scripts.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/function_scripts.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_definitions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/variable_definitions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/script/variable_types.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/script/variable_types.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/entries/variables/override_variables.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/entries/variables/override_variables.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/main.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/main.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/audio_extract.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/audio_extract.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/chapters.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/date_range.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/date_range.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/embed_thumbnail.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/embed_thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/file_convert.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/file_convert.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_exclude.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/filter_exclude.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/filter_include.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/filter_include.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/format.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/format.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/internal/view.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/internal/view.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/match_filters.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/match_filters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/music_tags.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/music_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/nfo_tags.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/output_directory_nfo_tags.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/output_directory_nfo_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/regex.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/regex.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/split_by_chapters.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/split_by_chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/subtitles.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/subtitles.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/throttle_protection.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/throttle_protection.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/plugins/video_tags.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/plugins/video_tags.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/__init__.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/download_deletion_options.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/media_quality.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/players.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/players.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/url.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/helpers/url_bilateral.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/albums_from_chapters.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/albums_from_playlists.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/other_websites.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music/singles.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music/singles.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/music_video_base.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/music_videos/music_videos.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/episode.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_by_date.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml` & `ytdl_sub-2024.5.29/src/ytdl_sub/prebuilt_presets/tv_show/tv_show_collection.yaml`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/__init__.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/array_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/array_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/boolean_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/boolean_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/conditional_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/conditional_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/error_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/error_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/json_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/json_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/map_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/map_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/numeric_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/numeric_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/regex_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/regex_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/functions/string_functions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/functions/string_functions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/parser.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/parser.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/script.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/script.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/script_output.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/script_output.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/array.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/array.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/function.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/function.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/map.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/map.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/resolvable.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/resolvable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/syntax_tree.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/syntax_tree.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/variable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/types/variable_dependency.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/types/variable_dependency.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exception_formatters.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/exception_formatters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/exceptions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/name_validation.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/name_validation.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/script/utils/type_checking.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/script/utils/type_checking.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/base_subscription.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/base_subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_download.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_download.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/subscriptions/subscription_ytdl_options.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/subscriptions/subscription_ytdl_options.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/thread/log_entries_downloaded_listener.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/thread/log_entries_downloaded_listener.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/chapters.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/chapters.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/datetime.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/exceptions.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/ffmpeg.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_handler.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_lock.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_lock.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/file_path.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/file_path.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/logger.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/retry.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/retry.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/script.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/script.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/scriptable.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/scriptable.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/thumbnail.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/thumbnail.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/xml.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/xml.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/utils/yaml.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/audo_codec_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/audo_codec_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/file_path_validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/file_path_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/nfo_validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/nfo_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/regex_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/regex_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/source_variable_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/source_variable_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/strict_dict_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/strict_dict_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_datetime.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_datetime.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_formatter_validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_formatter_validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/string_select_validator.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/string_select_validator.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/validators/validators.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/validators/validators.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py` & `ytdl_sub-2024.5.29/src/ytdl_sub/ytdl_additions/enhanced_download_archive.py`

 * *Files identical despite different names*

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/PKG-INFO` & `ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ytdl-sub
-Version: 2024.5.11
+Version: 2024.5.29
 Summary: Automate downloading metadata generation with YoutubeDL
 Author: Jesse Bannon
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,27 +685,27 @@
 Classifier: License :: Public Domain
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: yt-dlp==2024.04.09
+Requires-Dist: yt-dlp==2024.5.27
 Requires-Dist: colorama~=0.4
 Requires-Dist: mergedeep~=1.3
 Requires-Dist: mediafile~=0.12
 Requires-Dist: PyYAML~=6.0
 Provides-Extra: test
 Requires-Dist: coverage[toml]<8.0,>=6.3; extra == "test"
 Requires-Dist: pytest<9.0,>=7.2; extra == "test"
 Requires-Dist: pytest-rerunfailures~=14.0; extra == "test"
 Provides-Extra: lint
 Requires-Dist: black==24.4.2; extra == "lint"
 Requires-Dist: isort==5.13.2; extra == "lint"
-Requires-Dist: pylint==3.1.0; extra == "lint"
+Requires-Dist: pylint==3.2.0; extra == "lint"
 Provides-Extra: docs
 Requires-Dist: sphinx~=7.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme~=2.0; extra == "docs"
 Requires-Dist: sphinx-book-theme~=1.0; extra == "docs"
 Provides-Extra: build
 Requires-Dist: build~=1.2; extra == "build"
 Requires-Dist: twine~=5.0; extra == "build"
```

### Comparing `ytdl_sub-2024.5.11/src/ytdl_sub.egg-info/SOURCES.txt` & `ytdl_sub-2024.5.29/src/ytdl_sub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

