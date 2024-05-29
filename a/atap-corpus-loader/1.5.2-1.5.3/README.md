# Comparing `tmp/atap_corpus_loader-1.5.2.tar.gz` & `tmp/atap_corpus_loader-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atap_corpus_loader-1.5.2.tar", max compression
+gzip compressed data, was "atap_corpus_loader-1.5.3.tar", max compression
```

## Comparing `atap_corpus_loader-1.5.2.tar` & `atap_corpus_loader-1.5.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.5.2/LICENSE
--rw-r--r--   0        0        0     1116 2024-05-14 05:28:19.959163 atap_corpus_loader-1.5.2/README.md
--rw-r--r--   0        0        0     2893 2024-04-24 06:52:07.725642 atap_corpus_loader-1.5.2/atap_corpus_loader/CorpusLoader.py
--rw-r--r--   0        0        0       56 2024-04-10 06:28:42.036892 atap_corpus_loader-1.5.2/atap_corpus_loader/__init__.py
--rw-r--r--   0        0        0    17303 2024-05-14 01:54:30.177048 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/Controller.py
--rw-r--r--   0        0        0     3726 2024-04-04 00:22:30.044441 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/CorpusExportService.py
--rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/__init__.py
--rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/CorpusHeader.py
--rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/DataType.py
--rw-r--r--   0        0        0     9018 2024-05-14 01:54:30.177961 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/FileReference.py
--rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
--rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
--rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/__init__.py
--rw-r--r--   0        0        0       41 2024-05-14 01:54:30.178176 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/FileLoadError.py
--rw-r--r--   0        0        0     4349 2024-05-14 01:54:30.178393 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/FileLoaderService.py
--rw-r--r--   0        0        0     7116 2024-05-14 01:54:30.178630 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/LoaderService.py
--rw-r--r--   0        0        0     6926 2024-05-23 01:54:52.553786 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/OniLoaderService.py
--rw-r--r--   0        0        0       41 2024-05-14 01:54:30.179103 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/__init__.py
--rw-r--r--   0        0        0     2878 2024-05-14 01:54:30.179326 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py
--rw-r--r--   0        0        0     2333 2024-05-14 01:54:30.179627 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py
--rw-r--r--   0        0        0      100 2024-05-14 01:54:30.179808 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/__init__.py
--rw-r--r--   0        0        0     1273 2024-05-14 01:54:30.179990 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
--rw-r--r--   0        0        0     1388 2024-05-14 01:54:30.180169 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
--rw-r--r--   0        0        0     1295 2024-05-14 01:54:30.180348 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
--rw-r--r--   0        0        0     1561 2024-05-14 01:54:30.180526 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
--rw-r--r--   0        0        0     1293 2024-05-14 01:54:30.180703 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
--rw-r--r--   0        0        0     1286 2024-05-14 01:54:30.180867 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
--rw-r--r--   0        0        0     1268 2024-05-14 01:54:30.181031 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
--rw-r--r--   0        0        0     1659 2024-05-14 01:54:30.181234 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
--rw-r--r--   0        0        0      396 2024-05-14 01:54:30.181406 atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/__init__.py
--rw-r--r--   0        0        0     3032 2024-05-14 01:54:30.181897 atap_corpus_loader-1.5.2/atap_corpus_loader/view/ViewWrapperWidget.py
--rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.5.2/atap_corpus_loader/view/__init__.py
--rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/AbstractWidget.py
--rw-r--r--   0        0        0     5745 2024-04-10 06:28:42.037873 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/CorpusInfoWidget.py
--rw-r--r--   0        0        0     6626 2024-04-18 05:38:14.976878 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/FileLoaderWidget.py
--rw-r--r--   0        0        0     5410 2024-05-14 05:28:19.959710 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/FileSelectorWidget.py
--rw-r--r--   0        0        0     8527 2024-05-14 01:54:30.182393 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/MetaEditorWidget.py
--rw-r--r--   0        0        0     5651 2024-05-14 01:54:30.182949 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/OniLoaderWidget.py
--rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/__init__.py
--rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.5.2/atap_corpus_loader/view/notifications/NotifierService.py
--rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.5.2/atap_corpus_loader/view/notifications/__init__.py
--rw-r--r--   0        0        0     2182 2024-05-14 01:54:30.183614 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/TooltipManager.py
--rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/__init__.py
--rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/build_button.md
--rw-r--r--   0        0        0      972 2024-04-24 06:52:07.728330 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
--rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
--rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
--rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
--rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
--rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
--rw-r--r--   0        0        0      431 2024-05-14 01:54:30.184025 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/oni_api_key.md
--rw-r--r--   0        0        0      545 2024-05-23 00:24:18.132407 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/oni_provider.md
--rw-r--r--   0        0        0      372 2024-05-14 01:54:30.184405 atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/oni_retrieve_collection.md
--rw-r--r--   0        0        0      855 2024-05-23 01:55:31.331905 atap_corpus_loader-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 atap_corpus_loader-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.5.3/LICENSE
+-rw-r--r--   0        0        0     1116 2024-05-14 05:28:19.959163 atap_corpus_loader-1.5.3/README.md
+-rw-r--r--   0        0        0     2893 2024-04-24 06:52:07.725642 atap_corpus_loader-1.5.3/atap_corpus_loader/CorpusLoader.py
+-rw-r--r--   0        0        0       56 2024-04-10 06:28:42.036892 atap_corpus_loader-1.5.3/atap_corpus_loader/__init__.py
+-rw-r--r--   0        0        0    17303 2024-05-14 01:54:30.177048 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/Controller.py
+-rw-r--r--   0        0        0     3726 2024-04-04 00:22:30.044441 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/CorpusExportService.py
+-rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/__init__.py
+-rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/CorpusHeader.py
+-rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/DataType.py
+-rw-r--r--   0        0        0     9018 2024-05-14 01:54:30.177961 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/FileReference.py
+-rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
+-rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
+-rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-14 01:54:30.178176 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/FileLoadError.py
+-rw-r--r--   0        0        0     4349 2024-05-14 01:54:30.178393 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/FileLoaderService.py
+-rw-r--r--   0        0        0     7116 2024-05-14 01:54:30.178630 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/LoaderService.py
+-rw-r--r--   0        0        0     6926 2024-05-23 02:02:01.915465 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/OniLoaderService.py
+-rw-r--r--   0        0        0       41 2024-05-14 01:54:30.179103 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/__init__.py
+-rw-r--r--   0        0        0     2878 2024-05-14 01:54:30.179326 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py
+-rw-r--r--   0        0        0     2333 2024-05-14 01:54:30.179627 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py
+-rw-r--r--   0        0        0      100 2024-05-14 01:54:30.179808 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-29 02:23:28.723540 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1388 2024-05-14 01:54:30.180169 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
+-rw-r--r--   0        0        0     1311 2024-05-29 02:23:28.724087 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
+-rw-r--r--   0        0        0     1561 2024-05-14 01:54:30.180526 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
+-rw-r--r--   0        0        0     1307 2024-05-29 02:23:28.724483 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1286 2024-05-14 01:54:30.180867 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
+-rw-r--r--   0        0        0     1294 2024-05-29 02:23:28.724846 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
+-rw-r--r--   0        0        0     1659 2024-05-14 01:54:30.181234 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
+-rw-r--r--   0        0        0      396 2024-05-14 01:54:30.181406 atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/__init__.py
+-rw-r--r--   0        0        0     3032 2024-05-14 01:54:30.181897 atap_corpus_loader-1.5.3/atap_corpus_loader/view/ViewWrapperWidget.py
+-rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.5.3/atap_corpus_loader/view/__init__.py
+-rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/AbstractWidget.py
+-rw-r--r--   0        0        0     5745 2024-04-10 06:28:42.037873 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/CorpusInfoWidget.py
+-rw-r--r--   0        0        0     6638 2024-05-29 02:23:28.725422 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/FileLoaderWidget.py
+-rw-r--r--   0        0        0     5410 2024-05-14 05:28:19.959710 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/FileSelectorWidget.py
+-rw-r--r--   0        0        0     8527 2024-05-14 01:54:30.182393 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/MetaEditorWidget.py
+-rw-r--r--   0        0        0     5651 2024-05-14 01:54:30.182949 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/OniLoaderWidget.py
+-rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/__init__.py
+-rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.5.3/atap_corpus_loader/view/notifications/NotifierService.py
+-rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.5.3/atap_corpus_loader/view/notifications/__init__.py
+-rw-r--r--   0        0        0     2182 2024-05-14 01:54:30.183614 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/TooltipManager.py
+-rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/__init__.py
+-rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/build_button.md
+-rw-r--r--   0        0        0      972 2024-04-24 06:52:07.728330 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
+-rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
+-rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
+-rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
+-rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
+-rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
+-rw-r--r--   0        0        0      431 2024-05-14 01:54:30.184025 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/oni_api_key.md
+-rw-r--r--   0        0        0      545 2024-05-23 00:24:18.132407 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/oni_provider.md
+-rw-r--r--   0        0        0      372 2024-05-14 01:54:30.184405 atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/oni_retrieve_collection.md
+-rw-r--r--   0        0        0      860 2024-05-29 02:23:31.837049 atap_corpus_loader-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2090 1970-01-01 00:00:00.000000 atap_corpus_loader-1.5.3/PKG-INFO
```

### Comparing `atap_corpus_loader-1.5.2/LICENSE` & `atap_corpus_loader-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/README.md` & `atap_corpus_loader-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/CorpusLoader.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/CorpusLoader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/Controller.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/Controller.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/CorpusExportService.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/CorpusExportService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/CorpusHeader.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/CorpusHeader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/FileReference.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/FileReference.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/FileLoaderService.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/FileLoaderService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/LoaderService.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/LoaderService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/OniLoaderService.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/OniLoaderService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderFactory.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/FileLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,11 +20,11 @@
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_csv(file_buf, header=0, usecols=included_headers)
+        df: DataFrame = read_csv(file_buf, dtype=object, header=0, usecols=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,11 +20,11 @@
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, engine='odf', header=0, names=included_headers)
+        df: DataFrame = read_excel(file_buf, engine='odf', dtype=object, header=0, usecols=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,11 +20,11 @@
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_csv(file_buf, sep='\t', header=0, usecols=included_headers)
+        df: DataFrame = read_csv(file_buf, sep='\t', dtype=object, header=0, usecols=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from atap_corpus_loader.controller.data_objects import CorpusHeader, DataType
 from atap_corpus_loader.controller.loader_service.file_loader_strategy.FileLoaderStrategy import FileLoaderStrategy
 
 
 class XLSXLoaderStrategy(FileLoaderStrategy):
     def get_inferred_headers(self) -> list[CorpusHeader]:
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, nrows=2)
+        df: DataFrame = read_excel(file_buf, header=0, nrows=2)
         headers: list[CorpusHeader] = []
         for header_name, dtype_obj in df.dtypes.items():
             dtype: DataType
             try:
                 dtype = DataType(str(dtype_obj))
             except ValueError:
                 dtype = DataType.TEXT
             headers.append(CorpusHeader(str(header_name), dtype))
 
         return headers
 
     def get_dataframe(self, headers: list[CorpusHeader]) -> DataFrame:
         included_headers: list[str] = [header.name for header in headers if header.include]
         file_buf: BytesIO = self.file_ref.get_content_buffer()
-        df: DataFrame = read_excel(file_buf, header=0, names=included_headers)
+        df: DataFrame = read_excel(file_buf, dtype=object, header=0, usecols=included_headers)
         dtypes_applied_df: DataFrame = FileLoaderStrategy._apply_selected_dtypes(df, headers)
 
         return dtypes_applied_df
```

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/controller/loader_service/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/ViewWrapperWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/ViewWrapperWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/AbstractWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/CorpusInfoWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/CorpusInfoWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/FileLoaderWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/FileLoaderWidget.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,12 +119,12 @@
         self._set_button_status_on_operation(curr_loading=True)
         self.controller.unload_all()
         self.view_handler.update_displays()
         self._set_button_status_on_operation(curr_loading=False)
 
     def build_corpus(self, *_):
         self._set_button_status_on_operation(curr_loading=True)
-        success: bool = self.view_handler.build_corpus(self.corpus_name_input.value)
+        success: bool = self.view_handler.build_corpus(self.corpus_name_input.value_input)
         if success:
-            self.corpus_name_input.value = ""
+            self.corpus_name_input.value_input = ""
             self.unload_all()
         self._set_button_status_on_operation(curr_loading=False)
```

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/FileSelectorWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/FileSelectorWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/MetaEditorWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/MetaEditorWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/gui/OniLoaderWidget.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/gui/OniLoaderWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/notifications/NotifierService.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/notifications/NotifierService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/TooltipManager.py` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/TooltipManager.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/load_buttons.md` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/load_buttons.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/meta_editor.md` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/meta_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/atap_corpus_loader/view/tooltips/markdown/oni_provider.md` & `atap_corpus_loader-1.5.3/atap_corpus_loader/view/tooltips/markdown/oni_provider.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.5.2/pyproject.toml` & `atap_corpus_loader-1.5.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "atap-corpus-loader"
-version = "1.5.2"
+version = "1.5.3"
 description = " A GUI loader for atap_corpus using the Panel library."
 authors = ["Hamish Croser <hamish.croser@sydney.edu.au>"]
 readme = "README.md"
 documentation = "https://australian-text-analytics-platform.github.io/atap-corpus-loader/DOCS.html"
 repository = "https://github.com/Australian-Text-Analytics-Platform/atap-corpus-loader"
 license = "MIT"
 packages = [{include = "atap_corpus_loader"}]
 exclude = ["*/.ipynb_checkpoints/*", "*log.txt"]
 
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<3.12.0"
-pandas = "~=2.1.0"
+pandas = ">2.0"
 atap_corpus = "~=0.1.13"
-panel = "~=1.4.0"
+panel = "~=1.4.2,!=1.4.3"
 odfpy = "~=1.4.0"
 python-docx = "~=1.1.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `atap_corpus_loader-1.5.2/PKG-INFO` & `atap_corpus_loader-1.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: atap-corpus-loader
-Version: 1.5.2
+Version: 1.5.3
 Summary:  A GUI loader for atap_corpus using the Panel library.
 Home-page: https://github.com/Australian-Text-Analytics-Platform/atap-corpus-loader
 License: MIT
 Author: Hamish Croser
 Author-email: hamish.croser@sydney.edu.au
 Requires-Python: >=3.10.0,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: atap_corpus (>=0.1.13,<0.2.0)
 Requires-Dist: odfpy (>=1.4.0,<1.5.0)
-Requires-Dist: pandas (>=2.1.0,<2.2.0)
-Requires-Dist: panel (>=1.4.0,<1.5.0)
+Requires-Dist: pandas (>2.0)
+Requires-Dist: panel (>=1.4.2,<1.5.0,!=1.4.3)
 Requires-Dist: python-docx (>=1.1.0,<1.2.0)
 Project-URL: Documentation, https://australian-text-analytics-platform.github.io/atap-corpus-loader/DOCS.html
 Project-URL: Repository, https://github.com/Australian-Text-Analytics-Platform/atap-corpus-loader
 Description-Content-Type: text/markdown
 
 # Corpus Loader
```

