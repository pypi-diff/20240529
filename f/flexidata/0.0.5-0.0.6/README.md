# Comparing `tmp/flexidata-0.0.5.tar.gz` & `tmp/flexidata-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexidata-0.0.5.tar", last modified: Wed May 29 16:44:12 2024, max compression
+gzip compressed data, was "flexidata-0.0.6.tar", last modified: Wed May 29 17:27:40 2024, max compression
```

## Comparing `flexidata-0.0.5.tar` & `flexidata-0.0.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.573273 flexidata-0.0.5/
--rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    16451 2024-05-29 16:44:12.573273 flexidata-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.469292 flexidata-0.0.5/examples/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.5/examples/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.5/examples/run.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.469292 flexidata-0.0.5/flexidata/
--rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.5/flexidata/Logger.py
--rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.5/flexidata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.501252 flexidata-0.0.5/flexidata/models/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.5/flexidata/models/__init__.py
--rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.5/flexidata/models/base.py
--rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.5/flexidata/models/detectron2.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.515759 flexidata-0.0.5/flexidata/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.5/flexidata/ocr/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.5/flexidata/ocr/agent.py
--rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.5/flexidata/ocr/google_vision.py
--rw-rw-rw-   0        0        0     6334 2024-05-25 17:08:18.000000 flexidata-0.0.5/flexidata/ocr/paddle.py
--rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.5/flexidata/ocr/tesseract.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.531392 flexidata-0.0.5/flexidata/parser/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.5/flexidata/parser/__init__.py
--rw-rw-rw-   0        0        0     2852 2024-05-29 16:41:38.000000 flexidata-0.0.5/flexidata/parser/doc.py
--rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.5/flexidata/parser/document.py
--rw-rw-rw-   0        0        0     5375 2024-05-29 16:33:35.000000 flexidata-0.0.5/flexidata/parser/docx.py
--rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.5/flexidata/parser/epub.py
--rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.5/flexidata/parser/html.py
--rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.5/flexidata/parser/image.py
--rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.5/flexidata/parser/md.py
--rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.5/flexidata/parser/odt.py
--rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.5/flexidata/parser/org.py
--rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.5/flexidata/parser/pdf.py
--rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.5/flexidata/parser/pptx.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.5/flexidata/parser/rst.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.5/flexidata/parser/rtf.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.531392 flexidata-0.0.5/flexidata/preprocessor/
--rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.5/flexidata/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.5/flexidata/preprocessor/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.547598 flexidata-0.0.5/flexidata/reader/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.5/flexidata/reader/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.5/flexidata/reader/factory.py
--rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.5/flexidata/reader/file_reader.py
--rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.5/flexidata/reader/google_drive.py
--rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.5/flexidata/reader/handlers.py
--rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.5/flexidata/reader/local.py
--rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.5/flexidata/reader/s3.py
--rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.5/flexidata/reader/web.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.552509 flexidata-0.0.5/flexidata/text_processing/
--rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.5/flexidata/text_processing/__init__.py
--rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.5/flexidata/text_processing/classification.py
--rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.5/flexidata/text_processing/convert_file.py
--rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.5/flexidata/text_processing/text_block.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.557125 flexidata-0.0.5/flexidata/utils/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.5/flexidata/utils/__init__.py
--rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.5/flexidata/utils/common.py
--rw-rw-rw-   0        0        0     5383 2024-05-29 15:30:35.000000 flexidata-0.0.5/flexidata/utils/constants.py
--rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.5/flexidata/utils/decorators.py
--rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.5/flexidata/utils/pdf.py
--rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.5/flexidata/utils/text.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.568789 flexidata-0.0.5/flexidata.egg-info/
--rw-rw-rw-   0        0        0    16451 2024-05-29 16:44:12.000000 flexidata-0.0.5/flexidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1609 2024-05-29 16:44:12.000000 flexidata-0.0.5/flexidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 16:44:12.000000 flexidata-0.0.5/flexidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      541 2024-05-29 16:44:12.000000 flexidata-0.0.5/flexidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-29 16:44:12.000000 flexidata-0.0.5/flexidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-29 16:43:50.000000 flexidata-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 16:44:12.573273 flexidata-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.563209 flexidata-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.5/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.563209 flexidata-0.0.5/tests/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.5/tests/ocr/__init__.py
--rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.5/tests/ocr/test_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-29 16:44:12.563209 flexidata-0.0.5/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.5/tests/utils/__init__.py
--rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.5/tests/utils/test_common.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    16451 2024-05-29 17:27:40.805799 flexidata-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.661451 flexidata-0.0.6/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.6/examples/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.6/examples/run.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.661451 flexidata-0.0.6/flexidata/
+-rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.6/flexidata/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.6/flexidata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.692067 flexidata-0.0.6/flexidata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.6/flexidata/models/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.6/flexidata/models/base.py
+-rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.6/flexidata/models/detectron2.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.756844 flexidata-0.0.6/flexidata/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.6/flexidata/ocr/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.6/flexidata/ocr/agent.py
+-rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.6/flexidata/ocr/google_vision.py
+-rw-rw-rw-   0        0        0     6334 2024-05-25 17:08:18.000000 flexidata-0.0.6/flexidata/ocr/paddle.py
+-rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.6/flexidata/ocr/tesseract.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.770368 flexidata-0.0.6/flexidata/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.6/flexidata/parser/__init__.py
+-rw-rw-rw-   0        0        0     2852 2024-05-29 16:41:38.000000 flexidata-0.0.6/flexidata/parser/doc.py
+-rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.6/flexidata/parser/document.py
+-rw-rw-rw-   0        0        0     6646 2024-05-29 17:23:54.000000 flexidata-0.0.6/flexidata/parser/docx.py
+-rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/epub.py
+-rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.6/flexidata/parser/html.py
+-rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.6/flexidata/parser/image.py
+-rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/md.py
+-rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.6/flexidata/parser/odt.py
+-rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.6/flexidata/parser/org.py
+-rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/pdf.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.6/flexidata/parser/pptx.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/rst.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.6/flexidata/parser/rtf.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.770368 flexidata-0.0.6/flexidata/preprocessor/
+-rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.6/flexidata/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.6/flexidata/preprocessor/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.791315 flexidata-0.0.6/flexidata/reader/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.6/flexidata/reader/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.6/flexidata/reader/factory.py
+-rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.6/flexidata/reader/file_reader.py
+-rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.6/flexidata/reader/google_drive.py
+-rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.6/flexidata/reader/handlers.py
+-rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.6/flexidata/reader/local.py
+-rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.6/flexidata/reader/s3.py
+-rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.6/flexidata/reader/web.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.791315 flexidata-0.0.6/flexidata/text_processing/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.6/flexidata/text_processing/__init__.py
+-rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.6/flexidata/text_processing/classification.py
+-rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.6/flexidata/text_processing/convert_file.py
+-rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.6/flexidata/text_processing/text_block.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/flexidata/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.6/flexidata/utils/__init__.py
+-rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.6/flexidata/utils/common.py
+-rw-rw-rw-   0        0        0     5383 2024-05-29 15:30:35.000000 flexidata-0.0.6/flexidata/utils/constants.py
+-rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.6/flexidata/utils/decorators.py
+-rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.6/flexidata/utils/pdf.py
+-rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.6/flexidata/utils/text.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/flexidata.egg-info/
+-rw-rw-rw-   0        0        0    16451 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1609 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      541 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-29 17:27:40.000000 flexidata-0.0.6/flexidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-29 17:26:56.000000 flexidata-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 17:27:40.805799 flexidata-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.6/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.6/tests/ocr/__init__.py
+-rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.6/tests/ocr/test_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-29 17:27:40.805799 flexidata-0.0.6/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.6/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.6/tests/utils/test_common.py
```

### Comparing `flexidata-0.0.5/LICENSE` & `flexidata-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/PKG-INFO` & `flexidata-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.5
+Version: 0.0.6
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.5/README.md` & `flexidata-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/Logger.py` & `flexidata-0.0.6/flexidata/Logger.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/models/base.py` & `flexidata-0.0.6/flexidata/models/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/models/detectron2.py` & `flexidata-0.0.6/flexidata/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/ocr/agent.py` & `flexidata-0.0.6/flexidata/ocr/agent.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/ocr/google_vision.py` & `flexidata-0.0.6/flexidata/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/ocr/paddle.py` & `flexidata-0.0.6/flexidata/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/ocr/tesseract.py` & `flexidata-0.0.6/flexidata/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/doc.py` & `flexidata-0.0.6/flexidata/parser/doc.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/document.py` & `flexidata-0.0.6/flexidata/parser/document.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/docx.py` & `flexidata-0.0.6/flexidata/parser/docx.py`

 * *Files 25% similar despite different names*

```diff
@@ -48,18 +48,38 @@
         document = docx.Document(cast(BinaryIO, self.get_file_content()))
         page_number = 1
         text_blocks = []
         table_index = 0
         for element in document.element.body:
             if element.tag.endswith("tbl") and self.extract_table:
                 table = document.tables[table_index]
+                for row in table.rows:
+                    for cell in row.cells:
+                        for item in cell.iter_inner_content():
+                            if type(item).__name__ == "Table":
+                                inner_table = item
+                                html_inner_table = self.convert_table_to_text(table, as_html=True)
+                                text_inner_table = self.convert_table_to_text(inner_table, as_html=False)
+                                metadata = TextBlockMetadata(
+                                    is_inner_table = True,
+                                    text_as_html = html_inner_table,
+                                    file_path=self.get_file_path_by_source(),
+                                    languages=["eng"],
+                                    filetype=FileType.DOCX,
+                                    page_number=page_number,
+                                    extraction_source="docx",
+                                )
+                                text_block = TextBlock(text_inner_table, metadata, TextType.TABLES)
+                                text_blocks.append(text_block)
+                                
                 html_table = self.convert_table_to_text(table, as_html=True)
                 text_table = self.convert_table_to_text(table, as_html=False)
                 table_index = table_index + 1
                 metadata = TextBlockMetadata(
+                        text_as_html = html_table,
                         file_path=self.get_file_path_by_source(),
                         languages=["eng"],
                         filetype=FileType.DOCX,
                         page_number=page_number,
                         extraction_source="docx",
                     )
                 text_block = TextBlock(text_table, metadata, TextType.TABLES)
```

### Comparing `flexidata-0.0.5/flexidata/parser/epub.py` & `flexidata-0.0.6/flexidata/parser/epub.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/html.py` & `flexidata-0.0.6/flexidata/parser/html.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/image.py` & `flexidata-0.0.6/flexidata/parser/image.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/md.py` & `flexidata-0.0.6/flexidata/parser/md.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/odt.py` & `flexidata-0.0.6/flexidata/parser/odt.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/org.py` & `flexidata-0.0.6/flexidata/parser/org.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/pdf.py` & `flexidata-0.0.6/flexidata/parser/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/rst.py` & `flexidata-0.0.6/flexidata/parser/rst.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/parser/rtf.py` & `flexidata-0.0.6/flexidata/parser/rtf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/preprocessor/base.py` & `flexidata-0.0.6/flexidata/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/factory.py` & `flexidata-0.0.6/flexidata/reader/factory.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/file_reader.py` & `flexidata-0.0.6/flexidata/reader/file_reader.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/google_drive.py` & `flexidata-0.0.6/flexidata/reader/google_drive.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/handlers.py` & `flexidata-0.0.6/flexidata/reader/handlers.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/local.py` & `flexidata-0.0.6/flexidata/reader/local.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/s3.py` & `flexidata-0.0.6/flexidata/reader/s3.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/reader/web.py` & `flexidata-0.0.6/flexidata/reader/web.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/text_processing/classification.py` & `flexidata-0.0.6/flexidata/text_processing/classification.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/text_processing/convert_file.py` & `flexidata-0.0.6/flexidata/text_processing/convert_file.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/text_processing/text_block.py` & `flexidata-0.0.6/flexidata/text_processing/text_block.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/utils/common.py` & `flexidata-0.0.6/flexidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/utils/constants.py` & `flexidata-0.0.6/flexidata/utils/constants.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/utils/decorators.py` & `flexidata-0.0.6/flexidata/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/utils/pdf.py` & `flexidata-0.0.6/flexidata/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata/utils/text.py` & `flexidata-0.0.6/flexidata/utils/text.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata.egg-info/PKG-INFO` & `flexidata-0.0.6/flexidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.5
+Version: 0.0.6
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.5/flexidata.egg-info/SOURCES.txt` & `flexidata-0.0.6/flexidata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/flexidata.egg-info/requires.txt` & `flexidata-0.0.6/flexidata.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/pyproject.toml` & `flexidata-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flexidata"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Kalyanakannan Padivasu", email="Kalyanakannan.p@gmail.com" },
 ]
 description = "FlexiData is an open-source Python package designed for processing unstructured data."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["PDF,DOCX document parsing"]
```

### Comparing `flexidata-0.0.5/requirements.txt` & `flexidata-0.0.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.5/tests/ocr/test_agent.py` & `flexidata-0.0.6/tests/ocr/test_agent.py`

 * *Files identical despite different names*

