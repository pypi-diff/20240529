# Comparing `tmp/aligo-6.2.2.tar.gz` & `tmp/aligo-6.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aligo-6.2.2.tar", last modified: Fri Apr  5 08:19:16 2024, max compression
+gzip compressed data, was "aligo-6.2.3.tar", last modified: Wed May 29 07:58:47 2024, max compression
```

## Comparing `aligo-6.2.2.tar` & `aligo-6.2.3.tar`

### file list

```diff
@@ -1,219 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-05 08:19:11.000000 aligo-6.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-05 08:19:16.947844 aligo-6.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-04-05 08:19:11.000000 aligo-6.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 08:19:11.000000 aligo-6.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-05 08:19:11.000000 aligo-6.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:19:16.947844 aligo-6.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.911844 aligo-6.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.915844 aligo-6.2.2/src/aligo/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.919844 aligo-6.2.2/src/aligo/apis/
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Aligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/CustomShare.py
--rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/SyncFolder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.923844 aligo-6.2.2/src/aligo/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Album.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Audio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20148 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/BaseAligo.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Compress.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Copy.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Drive.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/EMail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/File.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/LoginServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Move.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Other.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Recyclebin.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/SBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Share.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Star.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Template.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/User.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/Video.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.923844 aligo-6.2.2/src/aligo/error/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.931844 aligo-6.2.2/src/aligo/request/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AimSearchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AlbumListFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/AlbumListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ArchiveStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ArchiveUncompressRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchCancelShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchCopyFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchGetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchMoveFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchMoveToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchRestoreRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchStarFilesRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/BatchSubRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CancelShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CompleteFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CopyFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateFolderRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/CreateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetAudioPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDefaultDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFilePathRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetRecycleBinListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareFileListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkDownloadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetShareTokenRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetStarredListRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetUploadUrlRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetVideoPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ListToCleanRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/MoveFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/MoveFileToTrashRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/PrivateShareRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/RenameFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/RestoreFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/SearchFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/SearchShareFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/ShareFileSaveToDriveRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/StarredFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/TemplateRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/UpdateFileRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/UpdateShareLinkRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/request/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.939844 aligo-6.2.2/src/aligo/response/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AimSearchResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AlbumInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/AlbumListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ArchiveStatusResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ArchiveUncompressResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/BatchSubResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CancelShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CopyFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CreateFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/CreateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/DuplicateListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetAudioPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetFilePathResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetOfficePreviewUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetPersonalInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetRecycleBinListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareFileListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkDownloadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetShareTokenResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetStarredListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetUploadUrlResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetVideoPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListMyDrivesResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ListToCleanResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/MoveFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/MoveFileToTrashResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/PrivateShareResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/RestoreFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/RewardSpaceResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/SearchFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/SearchShareFileResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareFileSaveToDriveResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareItemInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/ShareLinkExtractCodeResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/TemplateResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/UpdateShareLinkResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/UsersVipInfoResponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/response/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioMusicMeta.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/AudioTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseAlbum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseDrive.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseShareFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/BaseUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/CroppingBoundary.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/CroppingSuggestionItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/DriveCapacityDetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/DriveFile.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/EMailConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FaceThumbnail.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FieldsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/FolderSizeInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageQuality.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ImageTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ListAlbumItem.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/LoginDevice.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/MediaTransCodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Null.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/PersonalRightsInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/PersonalSpaceInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Privilege.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/RateLimit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ShareLinkBaseFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/ShareLinkSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/SystemTag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/Type.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/UploadPartInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMediaAudioStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoMediaVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreview.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreviewPlayInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoPreviewSprite.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/VideoTranscodeTemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/utils/LoginTimout.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:11.000000 aligo-6.2.2/src/aligo/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:19:16.947844 aligo-6.2.2/src/aligo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7222 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-05 08:19:16.000000 aligo-6.2.2/src/aligo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.400884 aligo-6.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 07:58:42.000000 aligo-6.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-29 07:58:47.400884 aligo-6.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-05-29 07:58:42.000000 aligo-6.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 07:58:42.000000 aligo-6.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-29 07:58:42.000000 aligo-6.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:58:47.400884 aligo-6.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.360883 aligo-6.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.364883 aligo-6.2.3/src/aligo/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 07:58:46.000000 aligo-6.2.3/src/aligo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.368883 aligo-6.2.3/src/aligo/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Aligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5094 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/CustomShare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23848 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17900 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/SyncFolder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.372883 aligo-6.2.3/src/aligo/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Album.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20148 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/BaseAligo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Compress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Drive.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/EMail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/File.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/LoginServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Recyclebin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/SBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9768 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Share.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Star.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/User.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/Video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.372883 aligo-6.2.3/src/aligo/error/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.384883 aligo-6.2.3/src/aligo/request/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AimSearchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AlbumListFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/AlbumListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ArchiveStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ArchiveUncompressRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchCancelShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchCopyFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchGetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchMoveFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchMoveToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchRestoreRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchStarFilesRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/BatchSubRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CancelShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CompleteFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CopyFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateFolderRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/CreateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetAudioPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDefaultDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFilePathRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetRecycleBinListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareFileListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareLinkVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetShareTokenRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetStarredListRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetUploadUrlRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetVideoPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/GetVideoPreviewPlayInfoRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ListToCleanRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/MoveFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/MoveFileToTrashRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/PrivateShareRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/RenameFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/RestoreFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/SearchFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/SearchShareFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/ShareFileSaveToDriveRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/StarredFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/TemplateRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/UpdateFileRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/UpdateShareLinkRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/request/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.392884 aligo-6.2.3/src/aligo/response/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AimSearchResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AlbumInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/AlbumListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ArchiveStatusResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ArchiveUncompressResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/BatchSubResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CancelShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CopyFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CreateFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/CreateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/DuplicateListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetAudioPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetFilePathResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetOfficePreviewUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetPersonalInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetRecycleBinListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareFileListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkDownloadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetShareTokenResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetStarredListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetUploadUrlResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetVideoPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/GetVideoPreviewPlayInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListMyDrivesResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ListToCleanResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/MoveFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/MoveFileToTrashResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/PrivateShareResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/RestoreFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/RewardSpaceResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/SearchFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/SearchShareFileResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareFileSaveToDriveResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareItemInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/ShareLinkExtractCodeResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/TemplateResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/UpdateShareLinkResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/UsersVipInfoResponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/response/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioMusicMeta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/AudioTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseAlbum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseDrive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseShareFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/BaseUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/CroppingBoundary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/CroppingSuggestionItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/DriveCapacityDetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/DriveFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/EMailConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FaceThumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FieldsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/FolderSizeInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageQuality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ImageTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ListAlbumItem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/LoginDevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/MediaTransCodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Null.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/PersonalRightsInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/PersonalSpaceInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Privilege.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/RateLimit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ShareLinkBaseFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/ShareLinkSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/SystemTag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/UploadPartInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMediaAudioStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoMediaVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreviewPlayInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoPreviewSprite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/VideoTranscodeTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/utils/LoginTimout.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:42.000000 aligo-6.2.3/src/aligo/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:58:47.396884 aligo-6.2.3/src/aligo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 07:58:47.000000 aligo-6.2.3/src/aligo.egg-info/top_level.txt
```

### Comparing `aligo-6.2.2/LICENSE` & `aligo-6.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/PKG-INFO` & `aligo-6.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.2
+Version: 6.2.3
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
@@ -42,14 +42,20 @@
 [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
 
 ```sh
 pip install -U aligo
 pip install git+https://github.com/foyoux/aligo.git
 ```
 
+> **Notes：** 最近官方更新了接口，导致 `get_file_list` 无法直接获取下载链接，现在需要单独使用 `get_download_url` 接口获取下载链接。
+> 
+> 对于不常用（没有封装）的接口，可以直接通过 `self.post` 方法直接发送请求。
+>
+> 接口变动较多，有问题请反馈，我会尽快修复。
+
 ## 快速入门
 
 ```python
 """快速入门"""
 from aligo import Aligo
 
 if __name__ == '__main__':
```

### Comparing `aligo-6.2.2/README.md` & `aligo-6.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
 
 ```sh
 pip install -U aligo
 pip install git+https://github.com/foyoux/aligo.git
 ```
 
+> **Notes：** 最近官方更新了接口，导致 `get_file_list` 无法直接获取下载链接，现在需要单独使用 `get_download_url` 接口获取下载链接。
+> 
+> 对于不常用（没有封装）的接口，可以直接通过 `self.post` 方法直接发送请求。
+>
+> 接口变动较多，有问题请反馈，我会尽快修复。
+
 ## 快速入门
 
 ```python
 """快速入门"""
 from aligo import Aligo
 
 if __name__ == '__main__':
```

### Comparing `aligo-6.2.2/pyproject.toml` & `aligo-6.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Album.py` & `aligo-6.2.3/src/aligo/apis/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Aligo.py` & `aligo-6.2.3/src/aligo/apis/Aligo.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 ):
     """阿里云盘"""
 
     def __init__(
             self,
             name: str = 'aligo', *,
             refresh_token: str = None,
-            show: Callable[[str], None] = None,
+            show: Callable[[str], str] = None,
             level: int = logging.DEBUG,
             use_aria2: bool = False,
             proxies: Dict = None,
             port: int = None,
             email: EMailConfig = None,
             request_failed_delay: float = 3,
             requests_timeout: float = None,
```

### Comparing `aligo-6.2.2/src/aligo/apis/Audio.py` & `aligo-6.2.3/src/aligo/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Compress.py` & `aligo-6.2.3/src/aligo/apis/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Copy.py` & `aligo-6.2.3/src/aligo/apis/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Create.py` & `aligo-6.2.3/src/aligo/apis/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/CustomShare.py` & `aligo-6.2.3/src/aligo/apis/CustomShare.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Download.py` & `aligo-6.2.3/src/aligo/apis/Download.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,10 +161,14 @@
         if file_id:
             file = self._core_get_file(GetFileRequest(file_id=file_id, drive_id=drive_id))
 
         if file:
             if file.type == 'folder':
                 raise AligoException('文件类型不对：期待文件，得到的是文件夹')
             file_path = os.path.join(local_folder, file.name)
-            url = file.download_url or file.url
+            url = file.download_url or file.url or self._core_get_download_url(GetDownloadUrlRequest(
+                file_id=file.file_id,
+                drive_id=file.drive_id,
+                file_name=file.name,
+            )).url
 
         return self._core_download_file(file_path, url)
```

### Comparing `aligo-6.2.2/src/aligo/apis/Drive.py` & `aligo-6.2.3/src/aligo/apis/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Duplicate.py` & `aligo-6.2.3/src/aligo/apis/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/File.py` & `aligo-6.2.3/src/aligo/apis/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Move.py` & `aligo-6.2.3/src/aligo/apis/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Other.py` & `aligo-6.2.3/src/aligo/apis/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Recyclebin.py` & `aligo-6.2.3/src/aligo/apis/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Search.py` & `aligo-6.2.3/src/aligo/apis/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Share.py` & `aligo-6.2.3/src/aligo/apis/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Star.py` & `aligo-6.2.3/src/aligo/apis/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/SyncFolder.py` & `aligo-6.2.3/src/aligo/apis/SyncFolder.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Update.py` & `aligo-6.2.3/src/aligo/apis/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/apis/Video.py` & `aligo-6.2.3/src/aligo/apis/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Album.py` & `aligo-6.2.3/src/aligo/core/Album.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Audio.py` & `aligo-6.2.3/src/aligo/core/Audio.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Auth.py` & `aligo-6.2.3/src/aligo/core/Auth.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/BaseAligo.py` & `aligo-6.2.3/src/aligo/core/BaseAligo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Compress.py` & `aligo-6.2.3/src/aligo/core/Compress.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Config.py` & `aligo-6.2.3/src/aligo/core/Config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """..."""
 # 主机
 API_HOST = 'https://api.aliyundrive.com'
+# API_HOST = 'https://api.alipan.com'
 AUTH_HOST = 'https://auth.aliyundrive.com'
 WEBSV_HOST = 'https://websv.aliyundrive.com'
 PASSPORT_HOST = 'https://passport.aliyundrive.com'
 MEMBER_HOST = 'https://member.aliyundrive.com'
 USER_HOST = 'https://user.aliyundrive.com'
 
 # 登录相关
@@ -116,12 +117,13 @@
 V2_TEMPLATE_TEST = '/v2/template/test'
 
 # 参数
 CLIENT_ID = '25dzX3vbYqktVxyX'
 UNI_PARAMS = {'appName': 'aliyun_drive'}
 UNI_HEADERS = {
     'Referer': 'https://aliyundrive.com',
-    'User-Agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) '
-                   'Chrome/91.0.4472.114 Safari/537.36'),
+    # 'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36',
+    'User-Agent': 'AliApp(AYSD/5.8.0) com.alicloud.databox/37029260 Channel/36176927979800@rimet_android_5.8.0 language/zh-CN /Android Mobile/Xiaomi Redmi',
     # 没有此请求头，list file 获取不到 download_url 字段，url 不支持断点续传
-    'x-canary': 'client=web,app=adrive,version=v4.1.0',
+    # 'x-canary': 'client=web,app=adrive,version=v4.1.0',
+    'x-canary': 'client=Android,app=adrive,version=v5.8.0',
 }
```

### Comparing `aligo-6.2.2/src/aligo/core/Copy.py` & `aligo-6.2.3/src/aligo/core/Copy.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Core.py` & `aligo-6.2.3/src/aligo/core/Core.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Create.py` & `aligo-6.2.3/src/aligo/core/Create.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Download.py` & `aligo-6.2.3/src/aligo/core/Download.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from aligo.request import BatchDownloadUrlRequest, GetDownloadUrlRequest, BatchRequest, BatchSubRequest
 from aligo.response import BatchDownloadUrlResponse, GetDownloadUrlResponse
 from aligo.types import BaseFile
 
 
 class Download(BaseAligo):
     """..."""
-    _DOWNLOAD_CHUNK_SIZE = 8388608  # 8 MB
+    _DOWNLOAD_CHUNK_SIZE = 1024 * 1024  # 1 MB
 
     def _core_get_download_url(self, body: GetDownloadUrlRequest) -> GetDownloadUrlResponse:
         """..."""
         response = self.post(V2_FILE_GET_DOWNLOAD_URL, body=body)
         return self._result(response, GetDownloadUrlResponse)
 
     def _core_batch_download_url(self, body: BatchDownloadUrlRequest) -> Iterator[BatchDownloadUrlResponse]:
@@ -128,10 +128,17 @@
         >>> # noinspection PyShadowingNames
         >>> file_path = ali.download_files([ali.get_file_by_path('xxx.mp3')])
         >>> print(file_path)
         """
         rt = []
         for file in files:
             file_path = os.path.join(local_folder, file.name)
-            file_path = self._core_download_file(file_path, file.download_url or file.url)
+            file_path = self._core_download_file(
+                file_path,
+                file.download_url or file.url or self._core_get_download_url(GetDownloadUrlRequest(
+                    file_id=file.file_id,
+                    drive_id=file.drive_id,
+                    file_name=file.name,
+                )).url
+            )
             rt.append(file_path)
         return rt
```

### Comparing `aligo-6.2.2/src/aligo/core/Drive.py` & `aligo-6.2.3/src/aligo/core/Drive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Duplicate.py` & `aligo-6.2.3/src/aligo/core/Duplicate.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/EMail.py` & `aligo-6.2.3/src/aligo/core/EMail.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/File.py` & `aligo-6.2.3/src/aligo/core/File.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/LoginServer.py` & `aligo-6.2.3/src/aligo/core/LoginServer.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Move.py` & `aligo-6.2.3/src/aligo/core/Move.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Other.py` & `aligo-6.2.3/src/aligo/core/Other.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Recyclebin.py` & `aligo-6.2.3/src/aligo/core/Recyclebin.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/SBox.py` & `aligo-6.2.3/src/aligo/core/SBox.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Search.py` & `aligo-6.2.3/src/aligo/core/Search.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Share.py` & `aligo-6.2.3/src/aligo/core/Share.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Star.py` & `aligo-6.2.3/src/aligo/core/Star.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/Update.py` & `aligo-6.2.3/src/aligo/core/Update.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/core/User.py` & `aligo-6.2.3/src/aligo/core/User.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     sbox_drive_id: str = field(default=None, repr=False)
     status: str = field(default=None, repr=False)
     updated_at: int = field(default=None, repr=False)
     user_data: UserData = field(default=None, repr=False)
     user_id: str = None
     user_name: str = None
     vip_identity: str = field(default=None, repr=False)
+    display_name: str = None
 
 
 class User(BaseAligo):
     """..."""
 
     def get_user(self, f5: bool = False) -> BaseUser:
         """
```

### Comparing `aligo-6.2.2/src/aligo/core/Video.py` & `aligo-6.2.3/src/aligo/core/Video.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/AlbumListFilesRequest.py` & `aligo-6.2.3/src/aligo/request/AlbumListFilesRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/CreateFileRequest.py` & `aligo-6.2.3/src/aligo/request/CreateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/CreateShareLinkRequest.py` & `aligo-6.2.3/src/aligo/request/CreateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetFileListRequest.py` & `aligo-6.2.3/src/aligo/request/GetFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetFileRequest.py` & `aligo-6.2.3/src/aligo/request/GetFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetRecycleBinListRequest.py` & `aligo-6.2.3/src/aligo/request/GetRecycleBinListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetShareFileListRequest.py` & `aligo-6.2.3/src/aligo/request/GetShareFileListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetShareLinkDownloadUrlRequest.py` & `aligo-6.2.3/src/aligo/request/GetShareLinkDownloadUrlRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetShareLinkListRequest.py` & `aligo-6.2.3/src/aligo/request/GetShareLinkListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/GetStarredListRequest.py` & `aligo-6.2.3/src/aligo/request/GetStarredListRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/SearchFileRequest.py` & `aligo-6.2.3/src/aligo/request/SearchFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/UpdateFileRequest.py` & `aligo-6.2.3/src/aligo/request/UpdateFileRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/UpdateShareLinkRequest.py` & `aligo-6.2.3/src/aligo/request/UpdateShareLinkRequest.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/request/__init__.py` & `aligo-6.2.3/src/aligo/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/CreateFileResponse.py` & `aligo-6.2.3/src/aligo/response/CreateFileResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/CreateShareLinkResponse.py` & `aligo-6.2.3/src/aligo/response/CreateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/DuplicateListResponse.py` & `aligo-6.2.3/src/aligo/response/DuplicateListResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/GetShareInfoResponse.py` & `aligo-6.2.3/src/aligo/response/GetShareInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py` & `aligo-6.2.3/src/aligo/response/GetShareLinkVideoPreviewPlayInfoResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/GetShareTokenResponse.py` & `aligo-6.2.3/src/aligo/response/GetShareTokenResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/UpdateShareLinkResponse.py` & `aligo-6.2.3/src/aligo/response/UpdateShareLinkResponse.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/response/__init__.py` & `aligo-6.2.3/src/aligo/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/BaseAlbum.py` & `aligo-6.2.3/src/aligo/types/BaseAlbum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/BaseDrive.py` & `aligo-6.2.3/src/aligo/types/BaseDrive.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/BaseFile.py` & `aligo-6.2.3/src/aligo/types/BaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/BaseShareFile.py` & `aligo-6.2.3/src/aligo/types/BaseShareFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/BaseUser.py` & `aligo-6.2.3/src/aligo/types/BaseUser.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,7 +30,8 @@
     need_change_password_next_login: bool = field(default=False, repr=False)
     permission: str = field(default=None, repr=False)
     creator: str = field(default=None, repr=False)
     expired_at: int = field(default=None, repr=False)
     default_location: str = field(default=None, repr=False)
     phone_region: str = field(default=None, repr=False)
     last_login_time: int = field(default=None, repr=False)
+    path_status: str = None
```

### Comparing `aligo-6.2.2/src/aligo/types/Enum.py` & `aligo-6.2.3/src/aligo/types/Enum.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/ImageMedia.py` & `aligo-6.2.3/src/aligo/types/ImageMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/ListAlbumItem.py` & `aligo-6.2.3/src/aligo/types/ListAlbumItem.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/Null.py` & `aligo-6.2.3/src/aligo/types/Null.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/ShareLinkBaseFile.py` & `aligo-6.2.3/src/aligo/types/ShareLinkBaseFile.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/ShareLinkSchema.py` & `aligo-6.2.3/src/aligo/types/ShareLinkSchema.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/Token.py` & `aligo-6.2.3/src/aligo/types/Token.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,7 +30,8 @@
     need_rp_verify: bool = field(default=None, repr=False)
     device_id: str = field(default=None, repr=False)
     domain_id: str = field(default=None, repr=False)
     # noinspection SpellCheckingInspection
     hlogin_url: str = field(default=None, repr=False)
     # x-signature x-device-id x-nonce
     x_device_id: str = field(default=None, repr=False)
+    path_status: str = None
```

### Comparing `aligo-6.2.2/src/aligo/types/UserConfig.py` & `aligo-6.2.3/src/aligo/types/UserConfig.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/VideoMedia.py` & `aligo-6.2.3/src/aligo/types/VideoMedia.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/VideoPreview.py` & `aligo-6.2.3/src/aligo/types/VideoPreview.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/VideoPreviewPlayInfo.py` & `aligo-6.2.3/src/aligo/types/VideoPreviewPlayInfo.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo/types/__init__.py` & `aligo-6.2.3/src/aligo/types/__init__.py`

 * *Files identical despite different names*

### Comparing `aligo-6.2.2/src/aligo.egg-info/PKG-INFO` & `aligo-6.2.3/src/aligo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aligo
-Version: 6.2.2
+Version: 6.2.3
 Summary: aliyun drive sdk
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/aligo
 Project-URL: Homepage, https://github.com/foyoux/aligo
 Project-URL: Bug Tracker, https://github.com/foyoux/aligo/issues
 Keywords: aligo
 Classifier: Programming Language :: Python
@@ -42,14 +42,20 @@
 [![python version](https://img.shields.io/pypi/pyversions/aligo)](https://pypi.org/project/aligo/)  [![Downloads](https://static.pepy.tech/personalized-badge/aligo?period=total&units=international_system&left_color=black&right_color=orange&left_text=Downloads)](https://pepy.tech/project/aligo)
 
 ```sh
 pip install -U aligo
 pip install git+https://github.com/foyoux/aligo.git
 ```
 
+> **Notes：** 最近官方更新了接口，导致 `get_file_list` 无法直接获取下载链接，现在需要单独使用 `get_download_url` 接口获取下载链接。
+> 
+> 对于不常用（没有封装）的接口，可以直接通过 `self.post` 方法直接发送请求。
+>
+> 接口变动较多，有问题请反馈，我会尽快修复。
+
 ## 快速入门
 
 ```python
 """快速入门"""
 from aligo import Aligo
 
 if __name__ == '__main__':
```

### Comparing `aligo-6.2.2/src/aligo.egg-info/SOURCES.txt` & `aligo-6.2.3/src/aligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

