# Comparing `tmp/flexidata-0.0.6.tar.gz` & `tmp/flexidata-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexidata-0.0.6.tar", last modified: Wed May 29 17:27:40 2024, max compression
+gzip compressed data, was "flexidata-0.0.7.tar", last modified: Wed May 29 18:09:22 2024, max compression
```

## Comparing `flexidata-0.0.6.tar` & `flexidata-0.0.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0    16451 2024-05-29 17:27:40.805799 flexidata-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.661451 flexidata-0.0.6/examples/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.6/examples/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.6/examples/run.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.661451 flexidata-0.0.6/flexidata/
--rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.6/flexidata/Logger.py
--rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.6/flexidata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.692067 flexidata-0.0.6/flexidata/models/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.6/flexidata/models/__init__.py
--rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.6/flexidata/models/base.py
--rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.6/flexidata/models/detectron2.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.756844 flexidata-0.0.6/flexidata/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.6/flexidata/ocr/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.6/flexidata/ocr/agent.py
--rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.6/flexidata/ocr/google_vision.py
--rw-rw-rw-   0        0        0     6334 2024-05-25 17:08:18.000000 flexidata-0.0.6/flexidata/ocr/paddle.py
--rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.6/flexidata/ocr/tesseract.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.770368 flexidata-0.0.6/flexidata/parser/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.6/flexidata/parser/__init__.py
--rw-rw-rw-   0        0        0     2852 2024-05-29 16:41:38.000000 flexidata-0.0.6/flexidata/parser/doc.py
--rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.6/flexidata/parser/document.py
--rw-rw-rw-   0        0        0     6646 2024-05-29 17:23:54.000000 flexidata-0.0.6/flexidata/parser/docx.py
--rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/epub.py
--rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.6/flexidata/parser/html.py
--rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.6/flexidata/parser/image.py
--rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/md.py
--rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.6/flexidata/parser/odt.py
--rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.6/flexidata/parser/org.py
--rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/pdf.py
--rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.6/flexidata/parser/pptx.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/rst.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/rtf.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.770368 flexidata-0.0.6/flexidata/preprocessor/
--rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.6/flexidata/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.6/flexidata/preprocessor/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.791315 flexidata-0.0.6/flexidata/reader/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.6/flexidata/reader/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.6/flexidata/reader/factory.py
--rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.6/flexidata/reader/file_reader.py
--rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.6/flexidata/reader/google_drive.py
--rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.6/flexidata/reader/handlers.py
--rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.6/flexidata/reader/local.py
--rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.6/flexidata/reader/s3.py
--rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.6/flexidata/reader/web.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.791315 flexidata-0.0.6/flexidata/text_processing/
--rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.6/flexidata/text_processing/__init__.py
--rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.6/flexidata/text_processing/classification.py
--rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.6/flexidata/text_processing/convert_file.py
--rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.6/flexidata/text_processing/text_block.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/flexidata/utils/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.6/flexidata/utils/__init__.py
--rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.6/flexidata/utils/common.py
--rw-rw-rw-   0        0        0     5383 2024-05-29 15:30:35.000000 flexidata-0.0.6/flexidata/utils/constants.py
--rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.6/flexidata/utils/decorators.py
--rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.6/flexidata/utils/pdf.py
--rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.6/flexidata/utils/text.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/flexidata.egg-info/
--rw-rw-rw-   0        0        0    16451 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1609 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      541 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-29 17:26:56.000000 flexidata-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 17:27:40.805799 flexidata-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.6/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.6/tests/ocr/__init__.py
--rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.6/tests/ocr/test_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.6/tests/utils/__init__.py
--rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.6/tests/utils/test_common.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0    16451 2024-05-29 18:09:22.363486 flexidata-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.262069 flexidata-0.0.7/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.7/examples/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.7/examples/run.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.264713 flexidata-0.0.7/flexidata/
+-rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.7/flexidata/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.7/flexidata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.299795 flexidata-0.0.7/flexidata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.7/flexidata/models/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.7/flexidata/models/base.py
+-rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.7/flexidata/models/detectron2.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.299795 flexidata-0.0.7/flexidata/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.7/flexidata/ocr/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.7/flexidata/ocr/agent.py
+-rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.7/flexidata/ocr/google_vision.py
+-rw-rw-rw-   0        0        0     6251 2024-05-29 17:31:51.000000 flexidata-0.0.7/flexidata/ocr/paddle.py
+-rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.7/flexidata/ocr/tesseract.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.331711 flexidata-0.0.7/flexidata/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.7/flexidata/parser/__init__.py
+-rw-rw-rw-   0        0        0     2852 2024-05-29 16:41:38.000000 flexidata-0.0.7/flexidata/parser/doc.py
+-rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.7/flexidata/parser/document.py
+-rw-rw-rw-   0        0        0     7958 2024-05-29 18:07:09.000000 flexidata-0.0.7/flexidata/parser/docx.py
+-rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.7/flexidata/parser/epub.py
+-rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.7/flexidata/parser/html.py
+-rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.7/flexidata/parser/image.py
+-rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.7/flexidata/parser/md.py
+-rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.7/flexidata/parser/odt.py
+-rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.7/flexidata/parser/org.py
+-rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.7/flexidata/parser/pdf.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.7/flexidata/parser/pptx.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.7/flexidata/parser/rst.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.7/flexidata/parser/rtf.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.331711 flexidata-0.0.7/flexidata/preprocessor/
+-rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.7/flexidata/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.7/flexidata/preprocessor/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.335102 flexidata-0.0.7/flexidata/reader/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.7/flexidata/reader/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.7/flexidata/reader/factory.py
+-rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.7/flexidata/reader/file_reader.py
+-rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.7/flexidata/reader/google_drive.py
+-rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.7/flexidata/reader/handlers.py
+-rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.7/flexidata/reader/local.py
+-rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.7/flexidata/reader/s3.py
+-rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.7/flexidata/reader/web.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.347858 flexidata-0.0.7/flexidata/text_processing/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.7/flexidata/text_processing/__init__.py
+-rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.7/flexidata/text_processing/classification.py
+-rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.7/flexidata/text_processing/convert_file.py
+-rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.7/flexidata/text_processing/text_block.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/flexidata/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.7/flexidata/utils/__init__.py
+-rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.7/flexidata/utils/common.py
+-rw-rw-rw-   0        0        0     5383 2024-05-29 15:30:35.000000 flexidata-0.0.7/flexidata/utils/constants.py
+-rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.7/flexidata/utils/decorators.py
+-rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.7/flexidata/utils/pdf.py
+-rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.7/flexidata/utils/text.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/flexidata.egg-info/
+-rw-rw-rw-   0        0        0    16451 2024-05-29 18:09:22.000000 flexidata-0.0.7/flexidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1609 2024-05-29 18:09:22.000000 flexidata-0.0.7/flexidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:09:22.000000 flexidata-0.0.7/flexidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      541 2024-05-29 18:09:22.000000 flexidata-0.0.7/flexidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-29 18:09:22.000000 flexidata-0.0.7/flexidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-29 18:08:22.000000 flexidata-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:09:22.363486 flexidata-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/tests/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.7/tests/ocr/__init__.py
+-rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.7/tests/ocr/test_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:22.363486 flexidata-0.0.7/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.7/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.7/tests/utils/test_common.py
```

### Comparing `flexidata-0.0.6/LICENSE` & `flexidata-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/PKG-INFO` & `flexidata-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.6
+Version: 0.0.7
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.6/README.md` & `flexidata-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/Logger.py` & `flexidata-0.0.7/flexidata/Logger.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/models/base.py` & `flexidata-0.0.7/flexidata/models/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/models/detectron2.py` & `flexidata-0.0.7/flexidata/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/ocr/agent.py` & `flexidata-0.0.7/flexidata/ocr/agent.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/ocr/google_vision.py` & `flexidata-0.0.7/flexidata/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/ocr/paddle.py` & `flexidata-0.0.7/flexidata/ocr/paddle.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,14 @@
 from flexidata.utils.common import check_package_installed
 from flexidata.utils.constants import OCREngine
 from flexidata.text_processing.text_block import TextBlock, TextBlockMetadata
 
 config = Config()
 
 try:
-    @check_package_installed("paddleocr")
-    @check_package_installed("paddle")
     from paddleocr import PaddleOCR as PaddleOCRClient, draw_ocr
     import paddle
 except ImportError as e:
     raise ImportError(f"Failed to import PaddleOCR or Paddle: {str(e)}") from e
 
 
 class CustomPaddleOCR:
```

### Comparing `flexidata-0.0.6/flexidata/ocr/tesseract.py` & `flexidata-0.0.7/flexidata/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/doc.py` & `flexidata-0.0.7/flexidata/parser/doc.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/document.py` & `flexidata-0.0.7/flexidata/parser/document.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/docx.py` & `flexidata-0.0.7/flexidata/parser/docx.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import BinaryIO, cast, Optional, List
+from typing import BinaryIO, cast, Optional, List, Any
 from flexidata.utils.constants import FileReaderSource, FileType
 from flexidata.reader.handlers import FileHandler
 import docx
 from flexidata.text_processing.text_block import TextBlockMetadata, TextBlock
 from flexidata.text_processing.classification import TextType
 from docx import table
 from tabulate import tabulate
 from flexidata.utils.constants import FileType
 from flexidata.utils.decorators import validate_file_type_method
 
+
 class DocxParser(FileHandler):
     """Initialize the DocxParser with file handling and parsing options.
 
-        Args:
-            file_path (Optional[str]): Local path to the file, if the source is local.
-            file_url (Optional[str]): URL of the file, if the source is a web URL.
-            source (FileReaderSource): Type of file source.
-            extract_table (bool): Flag to determine if tables should be extracted.
-            extract_image (bool): Flag to determine if images should be extracted.
-            output_folder (Optional[str]): Directory path where output files are saved.
-            bucket_name (Optional[str]): S3 bucket name if source is S3.
-            file_key (Optional[str]): S3 file key if source is S3.
+    Args:
+        file_path (Optional[str]): Local path to the file, if the source is local.
+        file_url (Optional[str]): URL of the file, if the source is a web URL.
+        source (FileReaderSource): Type of file source.
+        extract_table (bool): Flag to determine if tables should be extracted.
+        extract_image (bool): Flag to determine if images should be extracted.
+        output_folder (Optional[str]): Directory path where output files are saved.
+        bucket_name (Optional[str]): S3 bucket name if source is S3.
+        file_key (Optional[str]): S3 file key if source is S3.
     """
+
     def __init__(
         self,
         file_path: Optional[str] = None,
         file_url: Optional[str] = None,
         source: FileReaderSource = FileReaderSource.LOCAL,
         extract_table: bool = False,
         extract_image: bool = False,
@@ -48,57 +50,41 @@
         document = docx.Document(cast(BinaryIO, self.get_file_content()))
         page_number = 1
         text_blocks = []
         table_index = 0
         for element in document.element.body:
             if element.tag.endswith("tbl") and self.extract_table:
                 table = document.tables[table_index]
-                for row in table.rows:
-                    for cell in row.cells:
-                        for item in cell.iter_inner_content():
-                            if type(item).__name__ == "Table":
-                                inner_table = item
-                                html_inner_table = self.convert_table_to_text(table, as_html=True)
-                                text_inner_table = self.convert_table_to_text(inner_table, as_html=False)
-                                metadata = TextBlockMetadata(
-                                    is_inner_table = True,
-                                    text_as_html = html_inner_table,
-                                    file_path=self.get_file_path_by_source(),
-                                    languages=["eng"],
-                                    filetype=FileType.DOCX,
-                                    page_number=page_number,
-                                    extraction_source="docx",
-                                )
-                                text_block = TextBlock(text_inner_table, metadata, TextType.TABLES)
-                                text_blocks.append(text_block)
-                                
                 html_table = self.convert_table_to_text(table, as_html=True)
                 text_table = self.convert_table_to_text(table, as_html=False)
                 table_index = table_index + 1
                 metadata = TextBlockMetadata(
-                        text_as_html = html_table,
-                        file_path=self.get_file_path_by_source(),
-                        languages=["eng"],
-                        filetype=FileType.DOCX,
-                        page_number=page_number,
-                        extraction_source="docx",
-                    )
+                    text_as_html=html_table,
+                    file_path=self.get_file_path_by_source(),
+                    languages=["eng"],
+                    filetype=FileType.DOCX,
+                    page_number=page_number,
+                    extraction_source="docx",
+                )
                 text_block = TextBlock(text_table, metadata, TextType.TABLES)
                 text_blocks.append(text_block)
+                self._process_inner_table(table, page_number, text_blocks)
             if element.tag.endswith("p"):
                 paragraph = docx.text.paragraph.Paragraph(element, document)
                 if len(paragraph.text.strip()):
                     metadata = TextBlockMetadata(
                         file_path=self.get_file_path_by_source(),
                         languages=["eng"],
                         filetype=FileType.DOCX,
                         page_number=page_number,
                         extraction_source="docx",
                     )
-                    text_type = TextType.get_text_type_by_docx_style(paragraph.style.name if paragraph.style else None)
+                    text_type = TextType.get_text_type_by_docx_style(
+                        paragraph.style.name if paragraph.style else None
+                    )
                     text_block = TextBlock(paragraph.text, metadata, text_type)
                     text_blocks.append(text_block)
 
             if page_number is not None and self._check_page_break(element):
                 page_number += 1
 
         return text_blocks
@@ -114,15 +100,15 @@
         """
         page_break_indicators = [["w:br", 'type="page"'], ["lastRenderedPageBreak"]]
         if hasattr(element, "xml"):
             for indicators in page_break_indicators:
                 if all(indicator in element.xml for indicator in indicators):
                     return True
         return False
-    
+
     def convert_table_to_text(self, table: table.Table, as_html: bool = True) -> str:
         """Converts a DOCX table to a formatted string, either as HTML or plain text.
 
         Args:
             table (table.Table): The DOCX table to convert.
             as_html (bool): Flag to determine if the output should be in HTML format.
 
@@ -130,7 +116,54 @@
             str: The table converted to the specified format (HTML or plain text).
         """
         fmt = "html" if as_html else "plain"
         rows = list(table.rows)
         headers = [cell.text for cell in rows[0].cells]
         data = [[cell.text for cell in row.cells] for row in rows[1:]]
         return tabulate(data, headers=headers, tablefmt=fmt)
+
+    def _process_inner_table(
+        self, table: Any, page_number: int, text_blocks: List[TextBlock]
+    ) -> None:
+        """
+        Recursively processes each table found within a table cell, converting it into text and HTML,
+        and appending the resulting TextBlock to a list.
+
+        This method iterates over each cell of a given table. If a cell contains another table ('inner table'),
+        it processes both the HTML and plain text representations of the inner table. It also creates metadata
+        and a text block for the inner table, which are then appended to a list of text blocks. This method
+        is called recursively for each inner table found.
+
+        Args:
+            table (Any): The table object to be processed, which can contain nested tables.
+            page_number (int): The page number where the table is located, used in metadata.
+            text_blocks (List[TextBlock]): A list to which the new TextBlock instances are appended.
+
+        Example:
+            >>> _process_inner_table(table_instance, 5, text_blocks_list)
+            None  # The list text_blocks_list will be modified in-place.
+        """
+        for row in table.rows:
+            for cell in row.cells:
+                for item in cell.iter_inner_content():
+                    if type(item).__name__ == "Table":
+                        inner_table = item
+                        html_inner_table = self.convert_table_to_text(
+                            table, as_html=True
+                        )
+                        text_inner_table = self.convert_table_to_text(
+                            inner_table, as_html=False
+                        )
+                        metadata = TextBlockMetadata(
+                            is_inner_table=True,
+                            text_as_html=html_inner_table,
+                            file_path=self.get_file_path_by_source(),
+                            languages=["eng"],
+                            filetype=FileType.DOCX,
+                            page_number=page_number,
+                            extraction_source="docx",
+                        )
+                        text_block = TextBlock(
+                            text_inner_table, metadata, TextType.TABLES
+                        )
+                        text_blocks.append(text_block)
+                        self._process_inner_table(item, page_number, text_blocks)
```

### Comparing `flexidata-0.0.6/flexidata/parser/epub.py` & `flexidata-0.0.7/flexidata/parser/epub.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/html.py` & `flexidata-0.0.7/flexidata/parser/html.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/image.py` & `flexidata-0.0.7/flexidata/parser/image.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/md.py` & `flexidata-0.0.7/flexidata/parser/md.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/odt.py` & `flexidata-0.0.7/flexidata/parser/odt.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/org.py` & `flexidata-0.0.7/flexidata/parser/org.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/pdf.py` & `flexidata-0.0.7/flexidata/parser/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/rst.py` & `flexidata-0.0.7/flexidata/parser/rst.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/parser/rtf.py` & `flexidata-0.0.7/flexidata/parser/rtf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/preprocessor/base.py` & `flexidata-0.0.7/flexidata/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/factory.py` & `flexidata-0.0.7/flexidata/reader/factory.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/file_reader.py` & `flexidata-0.0.7/flexidata/reader/file_reader.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/google_drive.py` & `flexidata-0.0.7/flexidata/reader/google_drive.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/handlers.py` & `flexidata-0.0.7/flexidata/reader/handlers.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/local.py` & `flexidata-0.0.7/flexidata/reader/local.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/s3.py` & `flexidata-0.0.7/flexidata/reader/s3.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/reader/web.py` & `flexidata-0.0.7/flexidata/reader/web.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/text_processing/classification.py` & `flexidata-0.0.7/flexidata/text_processing/classification.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/text_processing/convert_file.py` & `flexidata-0.0.7/flexidata/text_processing/convert_file.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/text_processing/text_block.py` & `flexidata-0.0.7/flexidata/text_processing/text_block.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/utils/common.py` & `flexidata-0.0.7/flexidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/utils/constants.py` & `flexidata-0.0.7/flexidata/utils/constants.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/utils/decorators.py` & `flexidata-0.0.7/flexidata/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/utils/pdf.py` & `flexidata-0.0.7/flexidata/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata/utils/text.py` & `flexidata-0.0.7/flexidata/utils/text.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata.egg-info/PKG-INFO` & `flexidata-0.0.7/flexidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.6
+Version: 0.0.7
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.6/flexidata.egg-info/SOURCES.txt` & `flexidata-0.0.7/flexidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/flexidata.egg-info/requires.txt` & `flexidata-0.0.7/flexidata.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/pyproject.toml` & `flexidata-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flexidata"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Kalyanakannan Padivasu", email="Kalyanakannan.p@gmail.com" },
 ]
 description = "FlexiData is an open-source Python package designed for processing unstructured data."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["PDF,DOCX document parsing"]
```

### Comparing `flexidata-0.0.6/requirements.txt` & `flexidata-0.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.6/tests/ocr/test_agent.py` & `flexidata-0.0.7/tests/ocr/test_agent.py`

 * *Files identical despite different names*

