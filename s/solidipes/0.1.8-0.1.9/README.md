# Comparing `tmp/solidipes-0.1.8.tar.gz` & `tmp/solidipes-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipes-0.1.8.tar", max compression
+gzip compressed data, was "solidipes-0.1.9.tar", max compression
```

## Comparing `solidipes-0.1.8.tar` & `solidipes-0.1.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0      774 2023-11-16 16:27:01.101462 solidipes-0.1.8/AUTHORS
--rw-r--r--   0        0        0    35129 2023-11-16 16:27:01.105461 solidipes-0.1.8/LICENSE
--rw-r--r--   0        0        0     1272 2023-08-31 08:57:41.644682 solidipes-0.1.8/README.md
--rw-r--r--   0        0        0     2605 2024-05-16 10:52:39.708777 solidipes-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      379 2024-05-16 10:52:39.712777 solidipes-0.1.8/solidipes/__init__.py
--rw-r--r--   0        0        0      895 2024-04-26 09:02:52.939581 solidipes-0.1.8/solidipes/loaders/__init__.py
--rw-r--r--   0        0        0     5707 2024-04-15 07:08:11.288179 solidipes-0.1.8/solidipes/loaders/abaqus.py
--rw-r--r--   0        0        0      532 2024-05-15 12:13:53.770557 solidipes-0.1.8/solidipes/loaders/binary.py
--rw-r--r--   0        0        0     9147 2024-05-02 15:05:35.925093 solidipes-0.1.8/solidipes/loaders/cached_metadata.py
--rw-r--r--   0        0        0     1975 2024-05-02 15:47:42.837257 solidipes-0.1.8/solidipes/loaders/code_snippet.py
--rw-r--r--   0        0        0     6049 2024-04-19 17:51:44.056123 solidipes-0.1.8/solidipes/loaders/data_container.py
--rw-r--r--   0        0        0     6131 2024-05-02 15:05:35.925093 solidipes-0.1.8/solidipes/loaders/file.py
--rw-r--r--   0        0        0     2320 2024-04-26 09:02:52.939581 solidipes-0.1.8/solidipes/loaders/file_sequence.py
--rw-r--r--   0        0        0      335 2024-04-15 11:23:15.272215 solidipes-0.1.8/solidipes/loaders/geof_mesh.py
--rw-r--r--   0        0        0     1657 2024-04-26 09:36:07.215633 solidipes-0.1.8/solidipes/loaders/group.py
--rw-r--r--   0        0        0      355 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/hdf5.py
--rw-r--r--   0        0        0     1589 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/image.py
--rw-r--r--   0        0        0     1386 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/image_sequence.py
--rw-r--r--   0        0        0      449 2024-04-15 07:08:11.292179 solidipes-0.1.8/solidipes/loaders/matlab.py
--rw-r--r--   0        0        0      336 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/loaders/meshio.py
--rw-r--r--   0        0        0    75469 2024-04-15 11:23:15.276215 solidipes-0.1.8/solidipes/loaders/mime_types.py
--rw-r--r--   0        0        0      392 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/notebook.py
--rw-r--r--   0        0        0     6704 2023-11-10 06:38:59.297788 solidipes-0.1.8/solidipes/loaders/parse_inp.py
--rw-r--r--   0        0        0      598 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/pdf.py
--rw-r--r--   0        0        0     4970 2024-04-15 11:23:15.276215 solidipes-0.1.8/solidipes/loaders/pyvista_mesh.py
--rw-r--r--   0        0        0     1471 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/sequence.py
--rw-r--r--   0        0        0      596 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/loaders/symlink.py
--rw-r--r--   0        0        0     1702 2024-04-15 07:08:11.296179 solidipes-0.1.8/solidipes/loaders/table.py
--rw-r--r--   0        0        0      721 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/text.py
--rw-r--r--   0        0        0      329 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/video.py
--rw-r--r--   0        0        0     5001 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/xdmf.py
--rw-r--r--   0        0        0      452 2024-04-15 07:08:11.300179 solidipes-0.1.8/solidipes/loaders/xml.py
--rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/reports/__init__.py
--rw-r--r--   0        0        0     3537 2024-04-26 17:57:48.050239 solidipes-0.1.8/solidipes/reports/curation.py
--rw-r--r--   0        0        0     6480 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/jtcam.py
--rw-r--r--   0        0        0     8405 2023-04-26 08:20:35.886224 solidipes-0.1.8/solidipes/reports/jtcam_small_logo.png
--rw-r--r--   0        0        0    28449 2023-04-26 08:20:35.890224 solidipes-0.1.8/solidipes/reports/jupyter_logo.png
--rw-r--r--   0        0        0      310 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/report.py
--rw-r--r--   0        0        0    28738 2024-05-16 10:52:17.832288 solidipes-0.1.8/solidipes/reports/web_report.py
--rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/reports/widgets/__init__.py
--rw-r--r--   0        0        0     7827 2023-12-19 14:01:29.288781 solidipes-0.1.8/solidipes/reports/widgets/custom_widgets.py
--rw-r--r--   0        0        0     2530 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/reports/widgets/gitlab_issues.py
--rw-r--r--   0        0        0      631 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.css
--rw-r--r--   0        0        0      109 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.html
--rw-r--r--   0        0        0    18299 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/reports/widgets/zenodo.py
--rw-r--r--   0        0        0      132 2024-04-22 10:44:07.489071 solidipes-0.1.8/solidipes/scanners/__init__.py
--rw-r--r--   0        0        0    13080 2024-05-02 14:10:42.580154 solidipes-0.1.8/solidipes/scanners/scanner.py
--rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/scripts/__init__.py
--rw-r--r--   0        0        0     3276 2023-09-29 11:08:26.065427 solidipes-0.1.8/solidipes/scripts/download.py
--rw-r--r--   0        0        0     1255 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/generate_report.py
--rw-r--r--   0        0        0     4213 2023-10-13 10:23:46.696651 solidipes-0.1.8/solidipes/scripts/init.py
--rw-r--r--   0        0        0     1022 2023-09-14 07:54:57.371005 solidipes-0.1.8/solidipes/scripts/main.py
--rw-r--r--   0        0        0    10148 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/mount.py
--rw-r--r--   0        0        0     1133 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/quick_view.py
--rw-r--r--   0        0        0     2570 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/unmount.py
--rw-r--r--   0        0        0     1189 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/scripts/upload.py
--rw-r--r--   0        0        0        0 2024-05-16 10:52:32.348613 solidipes-0.1.8/solidipes/uploaders/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-15 07:08:11.312179 solidipes-0.1.8/solidipes/uploaders/renku.py
--rw-r--r--   0        0        0      314 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/uploaders/uploader.py
--rw-r--r--   0        0        0    10769 2024-04-26 17:57:48.050239 solidipes-0.1.8/solidipes/uploaders/zenodo.py
--rw-r--r--   0        0        0     1457 2024-04-22 10:44:07.493071 solidipes-0.1.8/solidipes/utils/__init__.py
--rw-r--r--   0        0        0    18232 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/utils/cloud.py
--rw-r--r--   0        0        0     1863 2024-04-26 08:08:46.255817 solidipes-0.1.8/solidipes/utils/config.py
--rw-r--r--   0        0        0     1151 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/git_infos.py
--rw-r--r--   0        0        0    24251 2023-09-29 11:08:26.069427 solidipes-0.1.8/solidipes/utils/languages-iso-639-2.csv
--rw-r--r--   0        0        0    16110 2023-09-29 11:08:26.073427 solidipes-0.1.8/solidipes/utils/licenses.csv
--rw-r--r--   0        0        0     1177 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/list_subclasses.py
--rw-r--r--   0        0        0     1133 2023-09-29 11:08:26.073427 solidipes-0.1.8/solidipes/utils/metadata.py
--rw-r--r--   0        0        0     2500 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/utils/solidipes_logging.py
--rw-r--r--   0        0        0    12754 2024-05-01 15:10:16.133710 solidipes-0.1.8/solidipes/utils/utils.py
--rw-r--r--   0        0        0     1535 2024-04-19 17:51:44.064123 solidipes-0.1.8/solidipes/utils/viewer_backends.py
--rw-r--r--   0        0        0     8610 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/utils/zenodo_utils.py
--rw-r--r--   0        0        0      584 2024-04-22 10:44:07.497071 solidipes-0.1.8/solidipes/viewers/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/binary.py
--rw-r--r--   0        0        0     1857 2024-04-24 16:29:05.346347 solidipes-0.1.8/solidipes/viewers/code_snippet.py
--rw-r--r--   0        0        0     2963 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/hdf5.py
--rw-r--r--   0        0        0     1588 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/image.py
--rw-r--r--   0        0        0     1197 2023-11-13 10:56:42.404659 solidipes-0.1.8/solidipes/viewers/matlab.py
--rw-r--r--   0        0        0     1765 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/notebook.py
--rw-r--r--   0        0        0     1553 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/pdf.py
--rw-r--r--   0        0        0     5256 2024-04-19 17:51:44.068123 solidipes-0.1.8/solidipes/viewers/pyvista_plotter.py
--rw-r--r--   0        0        0      853 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/symlink.py
--rw-r--r--   0        0        0     3806 2024-04-15 11:23:15.280216 solidipes-0.1.8/solidipes/viewers/table.py
--rw-r--r--   0        0        0     2031 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/text.py
--rw-r--r--   0        0        0      849 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/video.py
--rw-r--r--   0        0        0     2228 2023-09-29 11:08:26.077427 solidipes-0.1.8/solidipes/viewers/viewer.py
--rw-r--r--   0        0        0      799 2024-04-15 11:23:15.284216 solidipes-0.1.8/solidipes/viewers/xdmf.py
--rw-r--r--   0        0        0     1024 2024-04-15 11:23:15.284216 solidipes-0.1.8/solidipes/viewers/xml.py
--rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 solidipes-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      774 2023-12-19 09:01:53.478020 solidipes-0.1.9/AUTHORS
+-rw-r--r--   0        0        0    35129 2023-12-19 09:01:53.482020 solidipes-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1272 2023-08-31 08:58:31.249455 solidipes-0.1.9/README.md
+-rw-r--r--   0        0        0     2605 2024-05-29 07:31:42.980748 solidipes-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      379 2024-05-29 07:31:42.980748 solidipes-0.1.9/solidipes/__init__.py
+-rw-r--r--   0        0        0      895 2024-04-29 07:25:59.199919 solidipes-0.1.9/solidipes/loaders/__init__.py
+-rw-r--r--   0        0        0     5707 2024-04-15 08:16:52.251380 solidipes-0.1.9/solidipes/loaders/abaqus.py
+-rw-r--r--   0        0        0      532 2024-05-15 14:04:36.879505 solidipes-0.1.9/solidipes/loaders/binary.py
+-rw-r--r--   0        0        0    10085 2024-05-28 09:41:41.316708 solidipes-0.1.9/solidipes/loaders/cached_metadata.py
+-rw-r--r--   0        0        0     2139 2024-05-27 19:37:09.827712 solidipes-0.1.9/solidipes/loaders/code_snippet.py
+-rw-r--r--   0        0        0     6185 2024-05-28 09:41:41.316708 solidipes-0.1.9/solidipes/loaders/data_container.py
+-rw-r--r--   0        0        0     6443 2024-05-28 09:41:41.316708 solidipes-0.1.9/solidipes/loaders/file.py
+-rw-r--r--   0        0        0     2320 2024-04-29 07:25:59.199919 solidipes-0.1.9/solidipes/loaders/file_sequence.py
+-rw-r--r--   0        0        0      335 2024-04-15 11:23:18.360284 solidipes-0.1.9/solidipes/loaders/geof_mesh.py
+-rw-r--r--   0        0        0     1657 2024-04-29 07:25:59.199919 solidipes-0.1.9/solidipes/loaders/group.py
+-rw-r--r--   0        0        0      355 2024-04-15 08:16:52.251380 solidipes-0.1.9/solidipes/loaders/hdf5.py
+-rw-r--r--   0        0        0     1589 2024-04-15 08:16:52.255380 solidipes-0.1.9/solidipes/loaders/image.py
+-rw-r--r--   0        0        0     1386 2024-04-15 08:16:52.255380 solidipes-0.1.9/solidipes/loaders/image_sequence.py
+-rw-r--r--   0        0        0      449 2024-04-15 08:16:52.255380 solidipes-0.1.9/solidipes/loaders/matlab.py
+-rw-r--r--   0        0        0      336 2024-04-29 07:25:59.199919 solidipes-0.1.9/solidipes/loaders/meshio.py
+-rw-r--r--   0        0        0    75802 2024-05-27 19:37:09.827712 solidipes-0.1.9/solidipes/loaders/mime_types.py
+-rw-r--r--   0        0        0      392 2024-04-15 08:16:52.259380 solidipes-0.1.9/solidipes/loaders/notebook.py
+-rw-r--r--   0        0        0     6704 2023-12-19 09:01:53.490020 solidipes-0.1.9/solidipes/loaders/parse_inp.py
+-rw-r--r--   0        0        0      598 2024-04-15 08:16:52.259380 solidipes-0.1.9/solidipes/loaders/pdf.py
+-rw-r--r--   0        0        0     4970 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/loaders/pyvista_mesh.py
+-rw-r--r--   0        0        0     1471 2024-04-15 08:16:52.259380 solidipes-0.1.9/solidipes/loaders/sequence.py
+-rw-r--r--   0        0        0      596 2024-04-15 08:16:52.259380 solidipes-0.1.9/solidipes/loaders/symlink.py
+-rw-r--r--   0        0        0     1992 2024-05-27 19:37:09.827712 solidipes-0.1.9/solidipes/loaders/table.py
+-rw-r--r--   0        0        0      757 2024-05-27 19:37:09.831712 solidipes-0.1.9/solidipes/loaders/text.py
+-rw-r--r--   0        0        0      329 2024-04-15 08:16:52.259380 solidipes-0.1.9/solidipes/loaders/video.py
+-rw-r--r--   0        0        0     5001 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/loaders/xdmf.py
+-rw-r--r--   0        0        0      482 2024-05-29 07:31:16.900162 solidipes-0.1.9/solidipes/loaders/xml.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:35.728585 solidipes-0.1.9/solidipes/reports/__init__.py
+-rw-r--r--   0        0        0     3537 2024-04-29 07:25:59.199919 solidipes-0.1.9/solidipes/reports/curation.py
+-rw-r--r--   0        0        0     6480 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/reports/jtcam.py
+-rw-r--r--   0        0        0     8405 2023-04-26 08:21:26.047444 solidipes-0.1.9/solidipes/reports/jtcam_small_logo.png
+-rw-r--r--   0        0        0    28449 2023-04-26 08:21:26.047444 solidipes-0.1.9/solidipes/reports/jupyter_logo.png
+-rw-r--r--   0        0        0      310 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/reports/report.py
+-rw-r--r--   0        0        0    29393 2024-05-28 09:41:41.316708 solidipes-0.1.9/solidipes/reports/web_report.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:35.728585 solidipes-0.1.9/solidipes/reports/widgets/__init__.py
+-rw-r--r--   0        0        0     7827 2023-12-20 09:04:57.349569 solidipes-0.1.9/solidipes/reports/widgets/custom_widgets.py
+-rw-r--r--   0        0        0     2530 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/reports/widgets/gitlab_issues.py
+-rw-r--r--   0        0        0      631 2023-09-14 07:55:02.903092 solidipes-0.1.9/solidipes/reports/widgets/speech_bubble.css
+-rw-r--r--   0        0        0      109 2023-09-14 07:55:02.903092 solidipes-0.1.9/solidipes/reports/widgets/speech_bubble.html
+-rw-r--r--   0        0        0    18299 2024-04-29 07:25:59.203919 solidipes-0.1.9/solidipes/reports/widgets/zenodo.py
+-rw-r--r--   0        0        0      132 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/scanners/__init__.py
+-rw-r--r--   0        0        0    13080 2024-05-02 14:10:48.268280 solidipes-0.1.9/solidipes/scanners/scanner.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:35.728585 solidipes-0.1.9/solidipes/scripts/__init__.py
+-rw-r--r--   0        0        0     3276 2023-09-29 07:09:15.608597 solidipes-0.1.9/solidipes/scripts/download.py
+-rw-r--r--   0        0        0     1255 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/scripts/generate_report.py
+-rw-r--r--   0        0        0     4213 2023-09-29 07:09:15.608597 solidipes-0.1.9/solidipes/scripts/init.py
+-rw-r--r--   0        0        0     1022 2023-09-14 07:55:02.907093 solidipes-0.1.9/solidipes/scripts/main.py
+-rw-r--r--   0        0        0    10148 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/scripts/mount.py
+-rw-r--r--   0        0        0     1133 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/scripts/quick_view.py
+-rw-r--r--   0        0        0     2570 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/scripts/unmount.py
+-rw-r--r--   0        0        0     1189 2024-04-15 08:16:52.263380 solidipes-0.1.9/solidipes/scripts/upload.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:31:35.728585 solidipes-0.1.9/solidipes/uploaders/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/uploaders/renku.py
+-rw-r--r--   0        0        0      314 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/uploaders/uploader.py
+-rw-r--r--   0        0        0    10769 2024-04-29 07:25:59.203919 solidipes-0.1.9/solidipes/uploaders/zenodo.py
+-rw-r--r--   0        0        0     1457 2024-04-17 07:36:21.734014 solidipes-0.1.9/solidipes/utils/__init__.py
+-rw-r--r--   0        0        0    18232 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/utils/cloud.py
+-rw-r--r--   0        0        0     1863 2024-04-29 07:25:59.207919 solidipes-0.1.9/solidipes/utils/config.py
+-rw-r--r--   0        0        0     1151 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/utils/git_infos.py
+-rw-r--r--   0        0        0    24251 2023-09-29 07:09:15.612597 solidipes-0.1.9/solidipes/utils/languages-iso-639-2.csv
+-rw-r--r--   0        0        0    16110 2023-09-29 07:09:15.612597 solidipes-0.1.9/solidipes/utils/licenses.csv
+-rw-r--r--   0        0        0     1177 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/utils/list_subclasses.py
+-rw-r--r--   0        0        0     1133 2023-09-29 07:09:15.616597 solidipes-0.1.9/solidipes/utils/metadata.py
+-rw-r--r--   0        0        0     2500 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/utils/solidipes_logging.py
+-rw-r--r--   0        0        0    12754 2024-05-01 15:10:19.417783 solidipes-0.1.9/solidipes/utils/utils.py
+-rw-r--r--   0        0        0     1535 2024-04-17 07:36:21.734014 solidipes-0.1.9/solidipes/utils/viewer_backends.py
+-rw-r--r--   0        0        0     8610 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/utils/zenodo_utils.py
+-rw-r--r--   0        0        0      584 2024-04-15 08:16:52.267380 solidipes-0.1.9/solidipes/viewers/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-15 11:23:18.364284 solidipes-0.1.9/solidipes/viewers/binary.py
+-rw-r--r--   0        0        0     1981 2024-05-27 09:30:49.566608 solidipes-0.1.9/solidipes/viewers/code_snippet.py
+-rw-r--r--   0        0        0     2963 2024-04-15 11:23:18.368284 solidipes-0.1.9/solidipes/viewers/hdf5.py
+-rw-r--r--   0        0        0     1588 2024-04-15 11:23:18.368284 solidipes-0.1.9/solidipes/viewers/image.py
+-rw-r--r--   0        0        0     1197 2023-12-19 09:01:53.494020 solidipes-0.1.9/solidipes/viewers/matlab.py
+-rw-r--r--   0        0        0     1765 2024-04-15 11:23:18.368284 solidipes-0.1.9/solidipes/viewers/notebook.py
+-rw-r--r--   0        0        0     1553 2023-09-29 07:09:15.616597 solidipes-0.1.9/solidipes/viewers/pdf.py
+-rw-r--r--   0        0        0     5256 2024-04-17 07:36:21.734014 solidipes-0.1.9/solidipes/viewers/pyvista_plotter.py
+-rw-r--r--   0        0        0      853 2023-09-29 07:09:15.616597 solidipes-0.1.9/solidipes/viewers/symlink.py
+-rw-r--r--   0        0        0     4400 2024-05-27 19:37:09.831712 solidipes-0.1.9/solidipes/viewers/table.py
+-rw-r--r--   0        0        0     2031 2023-10-13 15:08:39.249827 solidipes-0.1.9/solidipes/viewers/text.py
+-rw-r--r--   0        0        0      849 2023-09-29 07:09:15.620597 solidipes-0.1.9/solidipes/viewers/video.py
+-rw-r--r--   0        0        0     2228 2023-09-29 07:09:15.620597 solidipes-0.1.9/solidipes/viewers/viewer.py
+-rw-r--r--   0        0        0      799 2024-04-15 11:23:18.368284 solidipes-0.1.9/solidipes/viewers/xdmf.py
+-rw-r--r--   0        0        0     1024 2024-04-15 11:23:18.368284 solidipes-0.1.9/solidipes/viewers/xml.py
+-rw-r--r--   0        0        0     3518 1970-01-01 00:00:00.000000 solidipes-0.1.9/PKG-INFO
```

### Comparing `solidipes-0.1.8/AUTHORS` & `solidipes-0.1.9/AUTHORS`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/LICENSE` & `solidipes-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/README.md` & `solidipes-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/pyproject.toml` & `solidipes-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "solidipes"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python package for the DCSM project"
 authors = [
 	"Guillaume Anciaux <guillaume.anciaux@epfl.ch>",
 	"Son Pham-Ba <son.phamba@epfl.ch>"
 ]
 license = "GPL-3.0-or-later"
 readme = "README.md"
```

### Comparing `solidipes-0.1.8/solidipes/loaders/__init__.py` & `solidipes-0.1.9/solidipes/loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/abaqus.py` & `solidipes-0.1.9/solidipes/loaders/abaqus.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/binary.py` & `solidipes-0.1.9/solidipes/loaders/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/cached_metadata.py` & `solidipes-0.1.9/solidipes/loaders/cached_metadata.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import atexit
 import os
 import sched
 import time
-from typing import Optional
 
 import transaction
 import ZODB
 import ZODB.FileStorage
 from BTrees.OOBTree import BTree
 from zc.lockfile import LockError
 
@@ -27,20 +26,32 @@
 
 class cached_property(property):
     """Decorator class to indicate that a property must be cached"""
 
 
 class cached_loadable(DataContainer.loadable):
     """Decorator class to indicate that a loadable must be cached"""
+    def __init__(self, func):
+        super().__init__(func)
 
+    def foo(self, obj, *args, **kwargs):
+        data = DataContainer.loadable.foo(self, obj, *args, **kwargs)
+        obj.set_cached_metadata_entry(self.key, data)
+        return data
+
+    def foo_setter(self, obj, value, *args, **kwargs):
+        DataContainer.loadable.foo_setter(self, obj, value, *args, **kwargs)
+        obj.save_field_to_cache(self.key)
+
+
+_default_cached_attributes = {}
+"List of @cached_property and @cached_loadable in the class"
 
-class CachedMetadata(DataContainer):
-    _default_cached_attributes: Optional[set] = None
-    "List of @cached_property and @cached_loadable in the class"
 
+class CachedMetadata(DataContainer):
     _storage = None
     _transaction_manager = transaction.TransactionManager()
     _global_cached_metadata = None
     _scheduler = sched.scheduler()
     _scheduled_commit = None
 
     def __init__(self, **kwargs):
@@ -49,35 +60,37 @@
         self.load_cached_metadata()
 
     def _get_default_cached_attributes(self) -> set:
         """Build the list of cached fields from the class description"""
 
         # Cannot be done on the instance because checking the loadable fields would trigger loading
         cls = self.__class__
+        cls_name = cls.__name__
 
-        if cls._default_cached_attributes is not None:
-            return cls._default_cached_attributes
+        if cls_name in _default_cached_attributes:
+            return _default_cached_attributes[cls_name]
 
-        cls._default_cached_attributes = set()
+        _default_cached_attributes[cls_name] = set()
 
         for attribute_name in dir(cls):
             attribute = getattr(cls, attribute_name)
 
             if isinstance(attribute, cached_property) or isinstance(attribute, cached_loadable):
-                cls._default_cached_attributes.add(attribute_name)
+                _default_cached_attributes[cls_name].add(attribute_name)
 
-        return cls._default_cached_attributes
+        return _default_cached_attributes[cls_name]
 
     def clear_cached_metadata(self, fields=[]):
         if self.unique_identifier not in self.global_cached_metadata:
             return
 
         if fields:
             for field in fields:
-                del self.global_cached_metadata[self.unique_identifier][field]
+                if field in self.global_cached_metadata[self.unique_identifier]:
+                    del self.global_cached_metadata[self.unique_identifier][field]
             self.update_global_cached_metadata(self.unique_identifier)
 
         else:
             del self.global_cached_metadata[self.unique_identifier]
 
     def get_cached_metadata(self):
         if self.unique_identifier not in self.global_cached_metadata:
@@ -85,24 +98,35 @@
 
         return self.global_cached_metadata[self.unique_identifier]
 
     @cached_property
     def modified_time(self):
         raise NotImplementedError
 
-    def load_cached_metadata(self):
-        """Load cached metadata and put in _data_collection (as attributes)"""
-
+    def is_cache_invalid(self):
         cached_metadata = self.get_cached_metadata()
 
         # Check if update is necessary
         cache_modified_time = cached_metadata.get("modified_time", 0)
-        if cache_modified_time < self.modified_time:
+        from .file_sequence import FileSequence
+
+        if isinstance(self, FileSequence):
+            modified_time = self.file_info.modified_time
+        else:
+            modified_time = os.path.getmtime(self.path)
+        logger.info(f"{self.path} , cached_time {cache_modified_time}, time {modified_time}")
+        return cache_modified_time < modified_time
+
+    def load_cached_metadata(self):
+        """Load cached metadata and put in _data_collection (as attributes)"""
+
+        if self.is_cache_invalid():
             self.update_cached_metadata()
 
+        cached_metadata = self.get_cached_metadata()
         # Update _data_collection
         for key, value in cached_metadata.items():
             self.add(key, transform_dict_to_data_containers(value))
             self.cached_attributes.add(key)
 
         if "valid_loading" in self._data_collection:
             if self.valid_loading is False:
@@ -110,15 +134,14 @@
 
         return cached_metadata
 
     def update_cached_metadata(self):
         """Update cached metadata with instance's fields listed in cached_attributes"""
 
         cached_metadata = self.get_cached_metadata()
-
         for key in self.cached_attributes:
             try:
                 cached_metadata[key] = transform_data_containers_to_dict(getattr(self, key))
             except AttributeError:
                 pass
 
         self.update_global_cached_metadata(self.unique_identifier)
@@ -209,15 +232,15 @@
     @classmethod
     def _commit(cls):
         """Update cached metadata database"""
 
         if cls._global_cached_metadata is None:
             return
 
-        logger.debug("Committing cached metadata")
+        logger.info("Committing cached metadata")
         cls._transaction_manager.commit()
         cls._scheduled_commit = None
 
     @classmethod
     def _schedule_commit(cls):
         """Schedule later update of metadata database"""
```

### Comparing `solidipes-0.1.8/solidipes/loaders/code_snippet.py` & `solidipes-0.1.9/solidipes/loaders/code_snippet.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import os
 
 import pylint.lint
 from pylint.reporters.collecting_reporter import CollectingReporter as Reporter
 
 from .. import viewers
+from ..utils import solidipes_logging as logging
 from .text import Text
 
+logger = logging.getLogger()
+
 
 class CodeSnippet(Text):
     supported_extensions = ["py", "cc", "hh", "m", "sh"]
     supported_mime_types = ["text/x-shellscript/"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -41,19 +44,20 @@
             formatted_msg = f"{fname}:{msg['line']}:{msg['column']}:{msg['msg_id']}:{msg['symbol']}: {msg['msg']}"
             if msg["msg_id"][0] in ["E", "F"]:
                 lint_messages.append((msg["msg_id"], formatted_msg))
         return lint_messages
 
     @Text.cached_loadable
     def lint_raw(self):
+        logger.info(f"re-lint {self.file_info.path}")
         fname = self.file_info.path
 
         if os.path.splitext(fname)[1] == ".py":
             rep = Reporter()
-            pylint.lint.Run([fname], reporter=rep, exit=False)
+            pylint.lint.Run([fname, "--clear-cache-post-run", "y"], reporter=rep, exit=False)
             dict_messages = []
 
             for message in rep.messages:
                 dict_message = message.__dict__
 
                 if "confidence" in dict_message:
                     dict_message["confidence"] = dict_message["confidence"]._asdict()
```

### Comparing `solidipes-0.1.8/solidipes/loaders/data_container.py` & `solidipes-0.1.9/solidipes/loaders/data_container.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,35 @@
         except Exception as e:
             self.errors.append(str(e))
 
     return foo
 
 
 ################################################################
+class loadable(property):
+    def __init__(self, func):
+        self.key = func.__name__
+        self.func = func
+        super().__init__(self.foo, self.foo_setter)
+
+    def foo(self, obj, *args, **kwargs):
+        logger.debug(obj)
+        if self.key in obj._data_collection and obj._data_collection[self.key] is not None:
+            return obj._data_collection[self.key]
+        data = self.func(obj, *args, **kwargs)
+        if data is None:
+            raise Exception(f'Data "{self.key}" could not be loaded')
+        obj._data_collection[self.key] = data
+        return data
+
+    def foo_setter(self, obj, value, *args, **kwargs):
+        obj._data_collection[self.key] = value
+
+
+################################################################
 
 
 class DataContainer:
     """Container class for other structured data containers"""
 
     def __init__(self, initial_data={}, name=None, unique_identifier=None, **kwargs):
         logger.debug(f"Creating data container {type(self)}")
@@ -30,15 +51,15 @@
         #: Set entry to "None" to mark as loadable.
         self._data_collection = initial_data.copy()
         clss = set([self.__class__])
         while clss:
             new_clss = set()
             for cls in clss:
                 for key, v in cls.__dict__.items():
-                    if isinstance(v, DataContainer.loadable):
+                    if isinstance(v, loadable):
                         if key not in self._data_collection:
                             self.add(key)
                 for c in cls.__bases__:
                     new_clss.add(c)
             clss = new_clss
 
         #: Default viewer for this file. Optionally override this in
@@ -163,28 +184,14 @@
 
     def __str__(self):
         return self.__class__.__name__
 
     def __repr__(self):
         return self._data_collection.__repr__()
 
-    class loadable(property):
-        def __init__(self, func):
-            key = func.__name__
-
-            def foo(obj, *args, **kwargs):
-                logger.debug(obj)
-                if key in obj._data_collection and obj._data_collection[key] is not None:
-                    return obj._data_collection[key]
-                data = func(obj, *args, **kwargs)
-                if data is None:
-                    raise Exception(f'Data "{key}" could not be loaded')
-                obj._data_collection[key] = data
-                return data
 
-            def foo_setter(obj, value, *args, **kwargs):
-                obj._data_collection[key] = value
+################################################################
 
-            super().__init__(foo, foo_setter)
 
+DataContainer.loadable = loadable
 
 ################################################################
```

### Comparing `solidipes-0.1.8/solidipes/loaders/file.py` & `solidipes-0.1.9/solidipes/loaders/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,18 +92,18 @@
             "size": stats.st_size,
             "changed_time": stats.st_ctime,
             "created_time": stats.st_ctime,
             "modified_time": stats.st_mtime,
             "permissions": stats.st_mode,
             "owner": stats.st_uid,
             "group": stats.st_gid,
-            "path": self.path,
+            "path": self.path.strip(),
             "type": mime_type,
-            "charset": charset,
-            "extension": get_extension(self.path),
+            "charset": charset.strip(),
+            "extension": get_extension(self.path).strip(),
         })
 
     @classmethod
     def check_file_support(cls, path):
         """Check mime type, then extension of file"""
 
         mime_type, _ = get_mime_type(path)
@@ -176,20 +176,30 @@
         raise FileNotFoundError(f'File "{path}" does not exist')
 
     # Get cached preferred loader
     loader_dict = {loader.__name__: loader for loader in loader_list}
     preferred_loader = get_cached_preferred_loader(path, loader_dict)
 
     if preferred_loader:
-        return preferred_loader(path=path)
+        try:
+            return preferred_loader(path=path)
+        except RuntimeError as e:
+            import streamlit as st
+
+            st.error(f"Cannot load {path}: {e}")
 
     # If no cached preferred loader, try to find a loader
     for loader in loader_list:
         if loader.check_file_support(path):
-            return loader(path=path)
+            try:
+                return loader(path=path)
+            except RuntimeError as e:
+                import streamlit as st
+
+                st.error(f"Cannot load {path}: {e}")
 
     # If no extension or unknown extension, assume binary
     return Binary(path=path)
 
 
 def get_cached_preferred_loader(path: str, loader_dict: dict[str, Type[File]]) -> Optional[Type[File]]:
     """Get the preferred loader for a file from global cache"""
```

### Comparing `solidipes-0.1.8/solidipes/loaders/file_sequence.py` & `solidipes-0.1.9/solidipes/loaders/file_sequence.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/group.py` & `solidipes-0.1.9/solidipes/loaders/group.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/image.py` & `solidipes-0.1.9/solidipes/loaders/image.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/image_sequence.py` & `solidipes-0.1.9/solidipes/loaders/image_sequence.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/mime_types.py` & `solidipes-0.1.9/solidipes/loaders/mime_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,24 @@
 
 from ..utils import get_mimes
 from ..utils import solidipes_logging as logging
 
 logger = logging.getLogger()
 
 _mime_types = """
+application/libmultiscale/config                config
+application/lammps/input                        in
+application/lammps/data                         data
+application/lammps/restart                      restart
+application/numpy/array                         npy npz
 application/notebook                            ipynb
 application/x-matlab-data                       mat
 application/paraview                                pvd
-application/vtk                                     vtk vtp vts vtu
+application/paraview/state                          pvsm
+application/vtk                                     vtk vtp vts vtu pvtu
 application/1d-interleaved-parityfec
 application/3gpdash-qoe-report+xml
 application/3gpp-ims+xml
 application/3gppHal+json
 application/3gppHalForms+json
 application/A2L					a2l
 application/ace+cbor
```

### Comparing `solidipes-0.1.8/solidipes/loaders/parse_inp.py` & `solidipes-0.1.9/solidipes/loaders/parse_inp.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/pdf.py` & `solidipes-0.1.9/solidipes/loaders/pdf.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/pyvista_mesh.py` & `solidipes-0.1.9/solidipes/loaders/pyvista_mesh.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/sequence.py` & `solidipes-0.1.9/solidipes/loaders/sequence.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/symlink.py` & `solidipes-0.1.9/solidipes/loaders/symlink.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/loaders/table.py` & `solidipes-0.1.9/solidipes/loaders/table.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,49 @@
 from .. import viewers
 from .file import File
 
 
 class Table(File):
     """Table file loaded with Pandas"""
 
-    supported_mime_types = ["text/csv", "application/vnd.ms-excel"]
-    supported_extensions = ["csv", "xlsx"]
+    supported_mime_types = ["text/csv", "application/vnd.ms-excel", "application/numpy/array"]
+    supported_extensions = ["csv", "xlsx", "npy"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
         path = kwargs["path"]
 
         # find loader matching file extension
         if self.file_info.type == "text/csv":
             self.pandas_loader = self.read_csv
         elif self.file_info.type == "application/vnd.ms-excel" or self.file_info.extension in ["xlsx"]:
             self.pandas_loader = pd.read_excel
+        elif self.file_info.type.startswith("application/numpy"):
+            self.pandas_loader = self.read_numpy
         else:
             raise RuntimeError(f"File type not supported: {path} {self.file_info.type}")
 
         self.default_viewer = viewers.Table
 
     def read_csv(self, fname, **kwargs):
         import csv
 
         with open(fname) as fp:
             sep = csv.Sniffer().sniff(fp.readline()).delimiter
             ret = pd.read_csv(fname, sep=sep, **kwargs)
             return ret
 
+    def read_numpy(self, fname, **kwargs):
+        import numpy
+
+        f = numpy.load(fname)
+        f = pd.DataFrame(f)
+        return f
+
     def validate_header(self, header):
         for h in header:
             try:
                 h = float(h)
                 self.errors.append(f"Incorrect header: {header}")
                 break
             except Exception:
```

### Comparing `solidipes-0.1.8/solidipes/loaders/text.py` & `solidipes-0.1.9/solidipes/loaders/text.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .. import viewers
 from .file import File
 
 
 class Text(File):
     """Text file, potentially formatted with markdown"""
 
-    supported_mime_types = ["text/plain"]
-    supported_extensions = ["txt"]
+    supported_mime_types = ["text/plain", "application/lammps"]
+    supported_extensions = ["txt", "in", "data"]
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.default_viewer = viewers.Text
 
     @File.loadable
     def text(self):
```

### Comparing `solidipes-0.1.8/solidipes/loaders/xdmf.py` & `solidipes-0.1.9/solidipes/loaders/xdmf.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/curation.py` & `solidipes-0.1.9/solidipes/reports/curation.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/jtcam.py` & `solidipes-0.1.9/solidipes/reports/jtcam.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/jtcam_small_logo.png` & `solidipes-0.1.9/solidipes/reports/jtcam_small_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/jupyter_logo.png` & `solidipes-0.1.9/solidipes/reports/jupyter_logo.png`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/web_report.py` & `solidipes-0.1.9/solidipes/reports/web_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,15 +310,19 @@
             f"Download {os.path.basename(e.file_info.path)} ({DataSize(file_size):.2a})",
             data=open(e.file_info.path, "rb"),
             file_name=os.path.basename(e.file_info.path),
             key="download_" + e.unique_identifier,
         )
         try:
             _link = self._get_jupyter_link()
-            _link += "/" + os.path.dirname(e.file_info.path)
+            if _link.strip()[-1] != "/":
+                _link += "/"
+            if "tree" not in _link:
+                _link += "tree/"
+            _link += os.path.dirname(e.file_info.path).replace("./", "")
             col2.markdown(
                 f"[Edit in Jupyterlab]({_link}/)",
                 unsafe_allow_html=True,
             )
             _link = self._get_filebrowser_link()
             _link += "/" + os.path.dirname(e.file_info.path)
             col2.markdown(
@@ -517,14 +521,20 @@
         if not all_found_files:
             st.markdown(f"#### Nothing in the paths: {selected_paths}")
             return
 
         with self.tab_files:
             self.display_files(all_found_files, selected_paths)
 
+        with self.progress_layout:
+            with st.spinner("Saving cache to YAML format"):
+                from solidipes.loaders.cached_metadata import CachedMetadata
+
+                CachedMetadata._write_cached_metadata_to_yaml()
+
         if self.show_advanced:
             self.logs.markdown("---")
 
             with self.logs.expander("Logs"):
                 from solidipes.utils import get_study_log_path
 
                 col1, col2 = st.columns(2)
@@ -640,16 +650,22 @@
 
     def _open_in_filebrowser_button(self):
         with self.filebrowser_control:
             self._write_filebrowser_link()
 
     def _environment_info(self):
         with self.env_layout.expander("Environment"):
+            st.write("sh env")
             table_env = [k for k in os.environ.items()]
-            st.dataframe(table_env)
+            st.dataframe(table_env, use_container_width=True)
+            import pkg_resources
+
+            st.write("pip packages")
+            table_env = [p.project_name for p in pkg_resources.working_set]
+            st.dataframe(table_env, use_container_width=True)
 
     def _git_info(self):
         with self.git_control.container():
             changed_files = self.git_get_changed_files()
             changed_files = [e for e in changed_files if not e.startswith(".solidipes/cloud/")]
             if changed_files:
                 with st.expander("Modified Files", expanded=False):
```

### Comparing `solidipes-0.1.8/solidipes/reports/widgets/custom_widgets.py` & `solidipes-0.1.9/solidipes/reports/widgets/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/widgets/gitlab_issues.py` & `solidipes-0.1.9/solidipes/reports/widgets/gitlab_issues.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/widgets/speech_bubble.css` & `solidipes-0.1.9/solidipes/reports/widgets/speech_bubble.css`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/reports/widgets/zenodo.py` & `solidipes-0.1.9/solidipes/reports/widgets/zenodo.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scanners/scanner.py` & `solidipes-0.1.9/solidipes/scanners/scanner.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/download.py` & `solidipes-0.1.9/solidipes/scripts/download.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/generate_report.py` & `solidipes-0.1.9/solidipes/scripts/generate_report.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/init.py` & `solidipes-0.1.9/solidipes/scripts/init.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/main.py` & `solidipes-0.1.9/solidipes/scripts/main.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/mount.py` & `solidipes-0.1.9/solidipes/scripts/mount.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/quick_view.py` & `solidipes-0.1.9/solidipes/scripts/quick_view.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/unmount.py` & `solidipes-0.1.9/solidipes/scripts/unmount.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/scripts/upload.py` & `solidipes-0.1.9/solidipes/scripts/upload.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/uploaders/renku.py` & `solidipes-0.1.9/solidipes/uploaders/renku.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/uploaders/zenodo.py` & `solidipes-0.1.9/solidipes/uploaders/zenodo.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/__init__.py` & `solidipes-0.1.9/solidipes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/cloud.py` & `solidipes-0.1.9/solidipes/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/config.py` & `solidipes-0.1.9/solidipes/utils/config.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/git_infos.py` & `solidipes-0.1.9/solidipes/utils/git_infos.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/languages-iso-639-2.csv` & `solidipes-0.1.9/solidipes/utils/languages-iso-639-2.csv`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/licenses.csv` & `solidipes-0.1.9/solidipes/utils/licenses.csv`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/list_subclasses.py` & `solidipes-0.1.9/solidipes/utils/list_subclasses.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/metadata.py` & `solidipes-0.1.9/solidipes/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/solidipes_logging.py` & `solidipes-0.1.9/solidipes/utils/solidipes_logging.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/utils.py` & `solidipes-0.1.9/solidipes/utils/utils.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/viewer_backends.py` & `solidipes-0.1.9/solidipes/utils/viewer_backends.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/utils/zenodo_utils.py` & `solidipes-0.1.9/solidipes/utils/zenodo_utils.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/__init__.py` & `solidipes-0.1.9/solidipes/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/binary.py` & `solidipes-0.1.9/solidipes/viewers/binary.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/code_snippet.py` & `solidipes-0.1.9/solidipes/viewers/code_snippet.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,21 +43,23 @@
                 print(m)
 
         elif viewer_backends.current_backend == "streamlit":
             if len(self.text) > 2000:
                 self.text = self.text[:50000] + "\n... more truncated content ..."
             st.code(self.text, language=guess_language(self.path), line_numbers=True)
             with st.expander("Linting feedback"):
-                st.markdown("### Errors")
-                for m in self.lint:
-                    if m[0][0] in ["E", "F"]:
-                        st.text(m[1])
-                st.markdown("### Warnings")
-                for m in self.lint:
-                    if m[0][0] not in ["E", "F"]:
-                        st.text(m[1])
+                errors = [m[1] for m in self.lint if m[0][0] in ["E", "F"]]
+                warnings = [m[1] for m in self.lint if m[0][0] not in ["E", "F"]]
+                if errors:
+                    st.markdown("### Errors")
+                    for m in errors:
+                        st.text(m)
+                if warnings:
+                    st.markdown("### Warnings")
+                    for m in warnings:
+                        st.text(m)
 
         else:  # pure python
             print(self.text)
             print("pylint")
             for m in self.lint:
                 print(m)
```

### Comparing `solidipes-0.1.8/solidipes/viewers/hdf5.py` & `solidipes-0.1.9/solidipes/viewers/hdf5.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/image.py` & `solidipes-0.1.9/solidipes/viewers/image.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/matlab.py` & `solidipes-0.1.9/solidipes/viewers/matlab.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/notebook.py` & `solidipes-0.1.9/solidipes/viewers/notebook.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/pdf.py` & `solidipes-0.1.9/solidipes/viewers/pdf.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/pyvista_plotter.py` & `solidipes-0.1.9/solidipes/viewers/pyvista_plotter.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/symlink.py` & `solidipes-0.1.9/solidipes/viewers/symlink.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/table.py` & `solidipes-0.1.9/solidipes/viewers/table.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,25 +29,30 @@
 
     def show_plot(self):
         if self.data_container is None:
             raise Exception("No data to show")
 
         table = self.data_container.table
         cols = table.columns
+        colsX = [c for c in cols] + ["Row"]
+        defaultX = 0
+        if len(cols) == 1:
+            defaultX = 1
 
         c1, c2 = st.columns(2)
         marker = None
         line = "-"
 
         with c1:
             tab_col_select, tab_advanced = st.tabs(["Column selection", "Advanced"])
             with tab_col_select:
                 xaxis = st.radio(
                     "X-axis",
-                    options=cols,
+                    options=colsX,
+                    index=defaultX,
                     horizontal=True,
                     key="xaxis_" + self.data_container.file_info.path,
                 )
                 yaxis = st.multiselect(
                     "Y-axis",
                     options=cols,
                     default=[c for c in cols if c != xaxis],
@@ -69,29 +74,38 @@
         if marker == "":
             marker = None
         if line == "":
             line = "None"
 
         fig = plt.figure(figsize=(7, 5))
         axe = fig.add_subplot(111)
-        if not np.issubdtype(table[xaxis].dtype, np.number):
+        if xaxis != "Row" and not np.issubdtype(table[xaxis].dtype, np.number):
             st.warning(f"Cannot plot '{xaxis}' as it is of type {table[xaxis].dtype} which is not a number")
             return
 
         for y in yaxis:
             if not np.issubdtype(table[y].dtype, np.number):
                 st.warning(f"Cannot plot '{y}' as it is of type {table[y].dtype} which is not a number")
                 continue
-            axe.plot(
-                table[xaxis],
-                table[y],
-                label=y,
-                marker=marker,
-                linestyle=line,
-            )
+
+            if xaxis == "Row":
+                axe.plot(
+                    table[y],
+                    label=y,
+                    marker=marker,
+                    linestyle=line,
+                )
+            else:
+                axe.plot(
+                    table[xaxis],
+                    table[y],
+                    label=y,
+                    marker=marker,
+                    linestyle=line,
+                )
         axe.set_xlabel(xaxis)
         axe.legend(loc="best")
         with c2:
             st.pyplot(fig)
 
     @wrap_errors
     def show(self):
@@ -101,17 +115,21 @@
         if viewer_backends.current_backend == "jupyter notebook":
             display(self.data_container.table)
 
         elif viewer_backends.current_backend == "streamlit":
             if self.data_container.table.shape[1] < 20:
                 tab_figure, tab_raw = st.tabs(["Figure", "Raw Data"])
                 with tab_figure:
-                    self.show_plot()
+                    try:
+                        self.show_plot()
+                    except Exception as e:
+                        st.error(e)
+                        st.exception(e)
                 with tab_raw:
-                    st.dataframe(self.data_container.table)
+                    st.dataframe(self.data_container.table.style.format("{:e}"))
             else:
                 st.dataframe(self.data_container.table.iloc[:20])
                 if self.data_container.table.shape[0] > 20:
                     st.write("Truncated the long file...")
 
         else:  # python
             print(self.data_container.table)
```

### Comparing `solidipes-0.1.8/solidipes/viewers/text.py` & `solidipes-0.1.9/solidipes/viewers/text.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/video.py` & `solidipes-0.1.9/solidipes/viewers/video.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/viewer.py` & `solidipes-0.1.9/solidipes/viewers/viewer.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/xdmf.py` & `solidipes-0.1.9/solidipes/viewers/xdmf.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/solidipes/viewers/xml.py` & `solidipes-0.1.9/solidipes/viewers/xml.py`

 * *Files identical despite different names*

### Comparing `solidipes-0.1.8/PKG-INFO` & `solidipes-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipes
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for the DCSM project
 Home-page: https://gitlab.com/groups/dcsm
 License: GPL-3.0-or-later
 Author: Guillaume Anciaux
 Author-email: guillaume.anciaux@epfl.ch
 Requires-Python: >=3.9.12,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

