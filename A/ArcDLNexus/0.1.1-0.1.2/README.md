# Comparing `tmp/arcdlnexus-0.1.1.tar.gz` & `tmp/arcdlnexus-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcdlnexus-0.1.1.tar", last modified: Wed May 29 10:23:11 2024, max compression
+gzip compressed data, was "arcdlnexus-0.1.2.tar", last modified: Wed May 29 10:33:51 2024, max compression
```

## Comparing `arcdlnexus-0.1.1.tar` & `arcdlnexus-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 10:23:11.995873 arcdlnexus-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-29 10:23:11.985900 arcdlnexus-0.1.1/ArcDLNexus/
--rw-rw-rw-   0        0        0       46 2024-05-29 10:22:00.000000 arcdlnexus-0.1.1/ArcDLNexus/__init__.py
--rw-rw-rw-   0        0        0     6814 2024-05-29 10:04:20.000000 arcdlnexus-0.1.1/ArcDLNexus/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 10:23:11.993878 arcdlnexus-0.1.1/ArcDLNexus.egg-info/
--rw-rw-rw-   0        0        0     5093 2024-05-29 10:23:11.000000 arcdlnexus-0.1.1/ArcDLNexus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-29 10:23:11.000000 arcdlnexus-0.1.1/ArcDLNexus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 10:23:11.000000 arcdlnexus-0.1.1/ArcDLNexus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 10:23:11.000000 arcdlnexus-0.1.1/ArcDLNexus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 10:23:11.000000 arcdlnexus-0.1.1/ArcDLNexus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     5093 2024-05-29 10:23:11.994876 arcdlnexus-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3851 2024-05-28 13:14:10.000000 arcdlnexus-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 10:23:11.995873 arcdlnexus-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.306396 arcdlnexus-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.288444 arcdlnexus-0.1.2/ArcDLNexus/
+-rw-rw-rw-   0        0        0       46 2024-05-29 10:33:49.000000 arcdlnexus-0.1.2/ArcDLNexus/__init__.py
+-rw-rw-rw-   0        0        0     6814 2024-05-29 10:04:20.000000 arcdlnexus-0.1.2/ArcDLNexus/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:33:51.304402 arcdlnexus-0.1.2/ArcDLNexus.egg-info/
+-rw-rw-rw-   0        0        0     6134 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 10:33:51.000000 arcdlnexus-0.1.2/ArcDLNexus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6134 2024-05-29 10:33:51.305399 arcdlnexus-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4892 2024-05-29 10:33:49.000000 arcdlnexus-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:33:51.306396 arcdlnexus-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.2/setup.py
```

### Comparing `arcdlnexus-0.1.1/ArcDLNexus/main.py` & `arcdlnexus-0.1.2/ArcDLNexus/main.py`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.1/ArcDLNexus.egg-info/PKG-INFO` & `arcdlnexus-0.1.2/ArcDLNexus.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.1
+Version: 0.1.2
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
@@ -62,21 +62,23 @@
 >モジュール（パッケージ）のバージョンは requirements.txt を参照してください
 
 # モジュールについて
 ## タスク
  - [x] モジュールを公開する
 <!--- 必須マーク : <span style="color:red">＊</span> -->
 ## ドキュメント
-| 関数       | パラメータ                                                                                                                  | 説明                                                                                                                         |
-|----------|------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
-| download | **phone** -- str: 電話番号<span style="color:red">＊</span>                                                                 | これは例外で関数ではなく、`Class`です。また、PayNexusを利用するために必要（Discord.pyでいう```discord.Client()```のようなものです）                                  |
-|          | **password** -- str: パスワード<span style="color:red">＊</span>                                                             |                                                                                                                            |
-|          | **client_uuid** -- str: ログイン済み`client_uuid `                                                                           | login関数を使用してログインすると既存のログイン時のjsonに加え、`client_uuid`が追加されて返ってくるのでそちらをここで指定します                                                 |
-|          | **session_save** -- str: ファイルパス                                                                                        | ログイン情報を保存するためのファイルパスを指定、拡張子はお任せ                                                                                            | | 支払いのワンタイムコードを作成する(ホーム画面にあるあのバーコードとおなじ)                                                                                     |
-
+| 関数       | パラメータ                                                     | 説明                                                                                                                                                                              |
+|----------|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| download | **url** -- str: アーカイブのURL<span style="color:red">＊</span> | アーカイブは次のような形式で、日付が指定されている必要があります。https://web.archive.org/web/{アーカイブの日付}/{サイトのURL}                                                                                               |
+|          | **path** -- str: ファイルを保存するフォルダパス                          | c:\のような絶対パスではなく、OSに縛られない./などの相対パスのみサポートしています。デフォルトは「./archive_download」です。                                                                                                      |
+|          | **mode** -- str: モード（0～2）                                 | モードは3種類に分けられています。                                                                                                                                                               |
+|          |                                                           | モード0 - アーカイブをダウンロードして復元のみ: ウェブページをアーカイブからダウンロードして元の状態に復元し、関連ファイルはダウンロードされず、ページの表示に必要なファイルやリソースはすべてアーカイブ前のURLから取得します。                                                            |
+|          |                                                           | モード1 - 関連ファイルを可能な限りダウンロード + モード0の機能: ウェブページのアーカイブをダウンロードし、そのページに関連するファイル（画像、スクリプト、スタイルシートなど）も可能な限りダウンロードし、ページを完全に表示するために必要なすべてのリソースが揃います（手動処理必要）。                               |
+|          |                                                           | モード2 - ダウンロードしたファイルで既存の関連ファイルURLを上書き + モード0と1の機能: ウェブページのアーカイブをダウンロードし、関連するすべてのファイルをダウンロードし、必要なファイルやリソースのURLをダウンロードしたファイルのパスに上書きし（ダウンロードできなかった場合はスルー）、ページを完全にオフラインで閲覧できるようにします。 |
+    
 ## 使用例
 ```python
 import ArcDLNexus
 
 ArcDLNexus.download(url="https://web.archive.org/web/20240204090521/https://home.disnana.com/",
                          path="./recovery_archive/",
                          mode=2)
```

### Comparing `arcdlnexus-0.1.1/LICENSE` & `arcdlnexus-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.1/PKG-INFO` & `arcdlnexus-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.1
+Version: 0.1.2
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
@@ -62,21 +62,23 @@
 >モジュール（パッケージ）のバージョンは requirements.txt を参照してください
 
 # モジュールについて
 ## タスク
  - [x] モジュールを公開する
 <!--- 必須マーク : <span style="color:red">＊</span> -->
 ## ドキュメント
-| 関数       | パラメータ                                                                                                                  | 説明                                                                                                                         |
-|----------|------------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
-| download | **phone** -- str: 電話番号<span style="color:red">＊</span>                                                                 | これは例外で関数ではなく、`Class`です。また、PayNexusを利用するために必要（Discord.pyでいう```discord.Client()```のようなものです）                                  |
-|          | **password** -- str: パスワード<span style="color:red">＊</span>                                                             |                                                                                                                            |
-|          | **client_uuid** -- str: ログイン済み`client_uuid `                                                                           | login関数を使用してログインすると既存のログイン時のjsonに加え、`client_uuid`が追加されて返ってくるのでそちらをここで指定します                                                 |
-|          | **session_save** -- str: ファイルパス                                                                                        | ログイン情報を保存するためのファイルパスを指定、拡張子はお任せ                                                                                            | | 支払いのワンタイムコードを作成する(ホーム画面にあるあのバーコードとおなじ)                                                                                     |
-
+| 関数       | パラメータ                                                     | 説明                                                                                                                                                                              |
+|----------|-----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| download | **url** -- str: アーカイブのURL<span style="color:red">＊</span> | アーカイブは次のような形式で、日付が指定されている必要があります。https://web.archive.org/web/{アーカイブの日付}/{サイトのURL}                                                                                               |
+|          | **path** -- str: ファイルを保存するフォルダパス                          | c:\のような絶対パスではなく、OSに縛られない./などの相対パスのみサポートしています。デフォルトは「./archive_download」です。                                                                                                      |
+|          | **mode** -- str: モード（0～2）                                 | モードは3種類に分けられています。                                                                                                                                                               |
+|          |                                                           | モード0 - アーカイブをダウンロードして復元のみ: ウェブページをアーカイブからダウンロードして元の状態に復元し、関連ファイルはダウンロードされず、ページの表示に必要なファイルやリソースはすべてアーカイブ前のURLから取得します。                                                            |
+|          |                                                           | モード1 - 関連ファイルを可能な限りダウンロード + モード0の機能: ウェブページのアーカイブをダウンロードし、そのページに関連するファイル（画像、スクリプト、スタイルシートなど）も可能な限りダウンロードし、ページを完全に表示するために必要なすべてのリソースが揃います（手動処理必要）。                               |
+|          |                                                           | モード2 - ダウンロードしたファイルで既存の関連ファイルURLを上書き + モード0と1の機能: ウェブページのアーカイブをダウンロードし、関連するすべてのファイルをダウンロードし、必要なファイルやリソースのURLをダウンロードしたファイルのパスに上書きし（ダウンロードできなかった場合はスルー）、ページを完全にオフラインで閲覧できるようにします。 |
+    
 ## 使用例
 ```python
 import ArcDLNexus
 
 ArcDLNexus.download(url="https://web.archive.org/web/20240204090521/https://home.disnana.com/",
                          path="./recovery_archive/",
                          mode=2)
```

### Comparing `arcdlnexus-0.1.1/setup.py` & `arcdlnexus-0.1.2/setup.py`

 * *Files identical despite different names*

