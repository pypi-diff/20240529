# Comparing `tmp/flexidata-0.0.2.tar.gz` & `tmp/flexidata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexidata-0.0.2.tar", last modified: Sat May 18 19:51:11 2024, max compression
+gzip compressed data, was "flexidata-0.0.3.tar", last modified: Wed May 29 14:02:11 2024, max compression
```

## Comparing `flexidata-0.0.2.tar` & `flexidata-0.0.3.tar`

### file list

```diff
@@ -1,47 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.895890 flexidata-0.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    15381 2024-05-18 19:51:11.894770 flexidata-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      766 2024-05-17 13:37:32.000000 flexidata-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.820452 flexidata-0.0.2/flexidata/
--rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.2/flexidata/Logger.py
--rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.2/flexidata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.863612 flexidata-0.0.2/flexidata/models/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.2/flexidata/models/__init__.py
--rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.2/flexidata/models/base.py
--rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.2/flexidata/models/detectron2.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.867213 flexidata-0.0.2/flexidata/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.2/flexidata/ocr/__init__.py
--rw-rw-rw-   0        0        0     1804 2024-05-11 18:01:28.000000 flexidata-0.0.2/flexidata/ocr/agent.py
--rw-rw-rw-   0        0        0     1354 2024-05-13 16:13:08.000000 flexidata-0.0.2/flexidata/ocr/google_vision.py
--rw-rw-rw-   0        0        0     5193 2024-05-12 07:05:47.000000 flexidata-0.0.2/flexidata/ocr/paddle.py
--rw-rw-rw-   0        0        0     1739 2024-05-11 16:52:17.000000 flexidata-0.0.2/flexidata/ocr/tesseract.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.867213 flexidata-0.0.2/flexidata/parser/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.2/flexidata/parser/__init__.py
--rw-rw-rw-   0        0        0    21772 2024-05-17 12:54:03.000000 flexidata-0.0.2/flexidata/parser/pdf.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.883998 flexidata-0.0.2/flexidata/reader/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.2/flexidata/reader/__init__.py
--rw-rw-rw-   0        0        0      749 2024-05-10 16:16:39.000000 flexidata-0.0.2/flexidata/reader/factory.py
--rw-rw-rw-   0        0        0      311 2024-05-10 16:10:37.000000 flexidata-0.0.2/flexidata/reader/file_reader.py
--rw-rw-rw-   0        0        0      965 2024-05-10 16:16:34.000000 flexidata-0.0.2/flexidata/reader/google_drive.py
--rw-rw-rw-   0        0        0      804 2024-05-10 16:16:29.000000 flexidata-0.0.2/flexidata/reader/local.py
--rw-rw-rw-   0        0        0     1112 2024-05-10 16:16:24.000000 flexidata-0.0.2/flexidata/reader/s3.py
--rw-rw-rw-   0        0        0      930 2024-05-10 16:16:14.000000 flexidata-0.0.2/flexidata/reader/web.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.891548 flexidata-0.0.2/flexidata/utils/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.2/flexidata/utils/__init__.py
--rw-rw-rw-   0        0        0      266 2024-05-11 09:04:55.000000 flexidata-0.0.2/flexidata/utils/common.py
--rw-rw-rw-   0        0        0     2001 2024-05-11 14:11:32.000000 flexidata-0.0.2/flexidata/utils/constants.py
--rw-rw-rw-   0        0        0     4740 2024-05-05 14:05:40.000000 flexidata-0.0.2/flexidata/utils/pdf.py
--rw-rw-rw-   0        0        0    10010 2024-05-08 18:00:49.000000 flexidata-0.0.2/flexidata/utils/text.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.893641 flexidata-0.0.2/flexidata.egg-info/
--rw-rw-rw-   0        0        0    15381 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      888 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      424 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-18 19:51:11.000000 flexidata-0.0.2/flexidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      800 2024-05-18 19:50:21.000000 flexidata-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      467 2024-05-13 16:14:08.000000 flexidata-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 19:51:11.896424 flexidata-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 19:51:11.892071 flexidata-0.0.2/tests/
--rw-rw-rw-   0        0        0     2724 2024-05-13 09:24:41.000000 flexidata-0.0.2/tests/test_pdf.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.357823 flexidata-0.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    16452 2024-05-29 14:02:11.350462 flexidata-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.268321 flexidata-0.0.3/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.3/examples/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.3/examples/run.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.268321 flexidata-0.0.3/flexidata/
+-rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.3/flexidata/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.3/flexidata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.300502 flexidata-0.0.3/flexidata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.3/flexidata/models/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.3/flexidata/models/base.py
+-rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.3/flexidata/models/detectron2.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.300502 flexidata-0.0.3/flexidata/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.3/flexidata/ocr/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.3/flexidata/ocr/agent.py
+-rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.3/flexidata/ocr/google_vision.py
+-rw-rw-rw-   0        0        0     6334 2024-05-25 17:08:18.000000 flexidata-0.0.3/flexidata/ocr/paddle.py
+-rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.3/flexidata/ocr/tesseract.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.316479 flexidata-0.0.3/flexidata/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.3/flexidata/parser/__init__.py
+-rw-rw-rw-   0        0        0     6191 2024-05-25 16:16:20.000000 flexidata-0.0.3/flexidata/parser/document.py
+-rw-rw-rw-   0        0        0     5407 2024-05-23 17:57:02.000000 flexidata-0.0.3/flexidata/parser/docx.py
+-rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.3/flexidata/parser/epub.py
+-rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.3/flexidata/parser/html.py
+-rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.3/flexidata/parser/image.py
+-rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.3/flexidata/parser/md.py
+-rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.3/flexidata/parser/odt.py
+-rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.3/flexidata/parser/org.py
+-rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.3/flexidata/parser/pdf.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.3/flexidata/parser/pptx.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.3/flexidata/parser/rst.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.3/flexidata/parser/rtf.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.316479 flexidata-0.0.3/flexidata/preprocessor/
+-rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.3/flexidata/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.3/flexidata/preprocessor/base.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.332392 flexidata-0.0.3/flexidata/reader/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.3/flexidata/reader/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.3/flexidata/reader/factory.py
+-rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.3/flexidata/reader/file_reader.py
+-rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.3/flexidata/reader/google_drive.py
+-rw-rw-rw-   0        0        0    11845 2024-05-25 16:40:52.000000 flexidata-0.0.3/flexidata/reader/handlers.py
+-rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.3/flexidata/reader/local.py
+-rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.3/flexidata/reader/s3.py
+-rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.3/flexidata/reader/web.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.337626 flexidata-0.0.3/flexidata/text_processing/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.3/flexidata/text_processing/__init__.py
+-rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.3/flexidata/text_processing/classification.py
+-rw-rw-rw-   0        0        0     3747 2024-05-23 16:47:33.000000 flexidata-0.0.3/flexidata/text_processing/convert_file.py
+-rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.3/flexidata/text_processing/text_block.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.343421 flexidata-0.0.3/flexidata/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.3/flexidata/utils/__init__.py
+-rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.3/flexidata/utils/common.py
+-rw-rw-rw-   0        0        0     5318 2024-05-25 16:13:12.000000 flexidata-0.0.3/flexidata/utils/constants.py
+-rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.3/flexidata/utils/decorators.py
+-rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.3/flexidata/utils/pdf.py
+-rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.3/flexidata/utils/text.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.350462 flexidata-0.0.3/flexidata.egg-info/
+-rw-rw-rw-   0        0        0    16452 2024-05-29 14:02:11.000000 flexidata-0.0.3/flexidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1585 2024-05-29 14:02:11.000000 flexidata-0.0.3/flexidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:02:11.000000 flexidata-0.0.3/flexidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      541 2024-05-29 14:02:11.000000 flexidata-0.0.3/flexidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-29 14:02:11.000000 flexidata-0.0.3/flexidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      800 2024-05-29 14:01:45.000000 flexidata-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:02:11.357823 flexidata-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.343421 flexidata-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.348430 flexidata-0.0.3/tests/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.3/tests/ocr/__init__.py
+-rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.3/tests/ocr/test_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:02:11.350462 flexidata-0.0.3/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.3/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.3/tests/utils/test_common.py
```

### Comparing `flexidata-0.0.2/LICENSE` & `flexidata-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.2/PKG-INFO` & `flexidata-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.2
+Version: 0.0.3
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,14 +210,15 @@
 Keywords: PDF,DOCX document parsing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pdfplumber==0.11.0
 Requires-Dist: pdf2image==1.17.0
 Requires-Dist: poppler-utils==0.1.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.13.0
 Requires-Dist: layoutparser==0.3.4
@@ -233,33 +234,43 @@
 Requires-Dist: boto3==1.34.102
 Requires-Dist: requests==2.31.0
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: paddlepaddle==2.6.1
 Requires-Dist: paddlepaddle-gpu==2.6.1
 Requires-Dist: paddleocr==2.7.3
 Requires-Dist: google-cloud-vision==3.7.2
+Requires-Dist: python-docx==1.1.2
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: lxml==5.2.2
+Requires-Dist: python-pptx==0.6.23
+Requires-Dist: Markdown==3.6
+Requires-Dist: pypandoc==1.13
 
 # flexidata
 
 FlexiData is an open-source Python package designed for processing unstructured data. Currently, it supports PDF extraction with plans to expand to other file types in the future.
 
 ## Features
 
-- **PDF Extraction**: Efficiently extract text and metadata from PDF files.
+- **Document  Parser**: The tool is designed to parse various file types, efficiently extracting text blocks and their metadata. This enables streamlined data extraction and content manipulation across multiple document formats.
 
-## Contributing
+  ### Supported File Formats:
+    - **PDF**: For detailed extraction of text and metadata.
+    - **Images** (JPEG, PNG, BMP): Enables image data and metadata processing.
+    - **EPUB**: Converts and extracts content from EPUB files.
+    - **HTML**: Parses HTML content for data extraction.
+    - **reStructuredText (RST)**: Handles conversion and parsing of RST files.
+    - **Rich Text Format (RTF)**: Facilitates conversion and content extraction from RTF documents.
+    - **DOCX**: Allows extraction from DOCX documents, providing access to structured content and metadata.
+
+## Upcoming Features:
+- **Content Chunking**: This will enable dividing text into meaningful and manageable pieces for better processing and analysis.
+- **Data Embedding**: Planned to support embedding textual data into vector spaces for advanced data analysis and machine learning applications.
 
-Contributions to FlexiData are welcome! If you're interested in contributing, please read our contributing guidelines.
 
-## Roadmap
+## Contributing
 
-- [x] PDF extraction support
-- [ ] Support for other file formats (e.g., Word, Excel, text files)
-- [ ] Advanced text processing features (e.g., natural language processing)
+Contributions to FlexiData are welcome! If you're interested in contributing, please read our contributing guidelines.
 
 ## Development Status
 
 FlexiData is currently in active development and we are working towards releasing our first version soon.
-
-
-
-
```

### Comparing `flexidata-0.0.2/flexidata/Logger.py` & `flexidata-0.0.3/flexidata/Logger.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.2/flexidata/models/base.py` & `flexidata-0.0.3/flexidata/models/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.2/flexidata/models/detectron2.py` & `flexidata-0.0.3/flexidata/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.2/flexidata/ocr/agent.py` & `flexidata-0.0.3/flexidata/ocr/agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 from typing import Type
 from flexidata.utils.constants import OCREngine
+from flexidata.config.config import Config
 
-# Define a map from OCR engine enum values to their corresponding class paths.
-engine_map = {
-    OCREngine.TESSERACT: "flexidata.ocr.tesseract.TesseractOCR",
-    OCREngine.PADDLE: "flexidata.ocr.paddle.CustomPaddleOCR",
-    OCREngine.GOOGLE_VISION: "flexidata.ocr.google_vision.GoogleVisionOCR",
-}
-
-def get_ocr_agent(engine: OCREngine = OCREngine.TESSERACT) -> Type:
-    """
-    Dynamically imports and returns an OCR agent class based on the specified engine.
-
-    The function looks up the class path from the `engine_map` dictionary using the provided
-    `engine` parameter. It then dynamically imports the module and retrieves the class
-    by name to instantiate and return an instance of the class.
-
-    Args:
-        engine (OCREngine): The OCR engine type from the OCREngine enumeration.
-
-    Returns:
-        An instance of the OCR agent class corresponding to the specified engine.
-
-    Raises:
-        ValueError: If the specified engine is not supported.
-        ImportError: If there's an issue importing the required OCR module.
-    """
-    try:
-        # Split the fully qualified class name to module and class name
-        module_path, class_name = engine_map[engine].rsplit('.', 1)
-        print(f"module_path={module_path} class_name={class_name}")
-        # Dynamically import the module containing the OCR class
-        module = __import__(module_path, fromlist=[class_name])
-        # Create and return an instance of the OCR class
-        return getattr(module, class_name)()
-    except KeyError:
-        raise ValueError(f"Unsupported OCR engine: {engine}")
-    except ImportError as e:
-        raise ImportError(f"Could not import the required OCR module: {e}")
+config = Config()
+class OCRAgentFactory:
+    def __init__(self):
+        self.engine_map = {
+            OCREngine.TESSERACT: "flexidata.ocr.tesseract.TesseractOCR",
+            OCREngine.PADDLE: "flexidata.ocr.paddle.CustomPaddleOCR",
+            OCREngine.GOOGLE_VISION: "flexidata.ocr.google_vision.GoogleVisionOCR",
+        }
+
+    def get_ocr_agent(self, engine: OCREngine = None) -> Type:
+        """
+        Dynamically imports and returns an OCR agent class based on the specified engine.
+
+        Args:
+            engine (OCREngine): The OCR engine type from the OCREngine enumeration, defaults to configuration if None.
+
+        Returns:
+            An instance of the OCR agent class corresponding to the specified engine.
+
+        Raises:
+            ValueError: If the specified engine is not supported.
+            ImportError: If there's an issue importing the required OCR module.
+        """
+        if engine is None:
+            engine = config.get("OCR_ENGINE", OCREngine.PADDLE)
+        
+        try:
+            # Split the fully qualified class name to module and class name
+            module_path, class_name = self.engine_map[engine].rsplit('.', 1)
+            print(f"module_path={module_path} class_name={class_name}")
+            # Dynamically import the module containing the OCR class
+            module = __import__(module_path, fromlist=[class_name])
+            # Create and return an instance of the OCR class
+            return getattr(module, class_name)()
+        except KeyError:
+            raise ValueError(f"Unsupported OCR engine: {engine}")
+        except ImportError as e:
+            raise ImportError(f"Could not import the required OCR module: {e}")
+        
+    def get_current_engine(self) -> OCREngine:
+        """
+        Returns the current OCR engine set in the configuration.
+
+        Returns:
+            OCREngine: The currently set OCR engine.
+        """
+        return config.get("OCR_ENGINE", OCREngine.PADDLE)
```

### Comparing `flexidata-0.0.2/flexidata/ocr/paddle.py` & `flexidata-0.0.3/flexidata/ocr/paddle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-from typing import List, Tuple, Any
+from typing import List, Dict, Any
 import numpy as np
 from PIL import Image
 import uuid
 from flexidata.config.config import Config
+
 # Ensure necessary packages are installed
 from flexidata.utils.common import check_package_installed
+from flexidata.utils.constants import OCREngine
+from flexidata.text_processing.text_block import TextBlock, TextBlockMetadata
+
 config = Config()
 
 try:
-    check_package_installed("paddleocr")
-    check_package_installed("paddle")
+    @check_package_installed("paddleocr")
+    @check_package_installed("paddle")
     from paddleocr import PaddleOCR as PaddleOCRClient, draw_ocr
     import paddle
 except ImportError as e:
     raise ImportError(f"Failed to import PaddleOCR or Paddle: {str(e)}") from e
 
+
 class CustomPaddleOCR:
     """
     A wrapper class for PaddleOCR to simplify its usage in text extraction from images,
     automatically handling GPU availability.
 
     Attributes:
         paddle_ocr (PaddleOCRClient): The PaddleOCR client configured for use.
@@ -33,101 +38,137 @@
             lang (str): Default language for OCR operations. Defaults to 'en' (English).
         """
         gpu_available = paddle.device.cuda.device_count() > 0
         self.paddle_ocr = PaddleOCRClient(
             use_angle_cls=True,  # Whether to use angle classifier
             use_gpu=gpu_available,  # Enable GPU if available
             lang=lang,
-            show_log=False  # Disable PaddleOCR logging
+            show_log=False,  # Disable PaddleOCR logging
         )
 
-    def image_to_text(self, image: Image.Image, lang: str = "en") -> List[Tuple]:
+    def image_to_text(
+        self,
+        image: Image.Image,
+        lang: str = "en",
+        page_number=None,
+        file_path=None,
+        filetype=None,
+    ) -> List[Dict[str, Any]]:
         """
         Extracts text from an image using the configured PaddleOCR client.
 
         Args:
             image (Image.Image): The image from which to extract text.
             lang (str): The language to use for OCR. Overrides the default if specified.
 
         Returns:
             List[Tuple]: A list of tuples containing OCR results, including bounding boxes and text.
         """
-        #Ensure image is in the correct format for PaddleOCR
+        # Ensure image is in the correct format for PaddleOCR
         if not isinstance(image, np.ndarray):
             image = np.array(image)
 
         ocr_data = self.paddle_ocr.ocr(image, cls=True)
-        texts = self.group_text_to_paragraphs(ocr_data)
-        return texts
-    
+        elements = self.get_text_with_metadata(
+            ocr_data, lang, page_number, file_path, filetype
+        )
+        return elements
+
+    def get_text_with_metadata(
+        self,
+        ocr_data,
+        lang: str = "en",
+        page_number=None,
+        file_path=None,
+        filetype=None,
+    ):
+        elements = []
+        ocr_data = ocr_data[0]
+        for index in range(len(ocr_data)):
+            text = ocr_data[index][1][0]
+            metadata = TextBlockMetadata(
+                file_path=file_path,
+                languages=lang,
+                filetype=filetype,
+                page_number=page_number,
+                bbox=ocr_data[index][0],
+                extraction_source=OCREngine.PADDLE,
+            )
+            element = TextBlock(text=text, metadata=metadata)
+            elements.append(element)
+        return elements
+
     def debug_layout(self, image, ocr_data):
-        image = Image.fromarray(image).convert('RGB')
+        image = Image.fromarray(image).convert("RGB")
         result = ocr_data[0]
         boxes = [line[0] for line in result]
         txts = [line[1][0] for line in result]
         scores = [line[1][1] for line in result]
-        im_show = draw_ocr(image, boxes, txts, scores, font_path='/app/flexi-data/fonts/simfang.ttf')
+        im_show = draw_ocr(
+            image, boxes, txts, scores, font_path="/app/flexi-data/fonts/simfang.ttf"
+        )
         im_show = Image.fromarray(im_show)
         image_name = str(uuid.uuid4())
         print(f"image_name={image_name}")
-        im_show.save(f'debug/paddleocr/{image_name}.jpg')
-
+        im_show.save(f"debug/paddleocr/{image_name}.jpg")
 
     def get_text_from_ocr_data(self, ocr_data):
         texts = []
         for index in range(len(ocr_data)):
             res = ocr_data[index]
             for line in res:
                 text = line[1][0]
                 if not text:
                     continue
                 texts.append(text.strip())
         return texts
-    
+
     def group_text_to_paragraphs(self, ocr_results):
         """
         Groups OCR results into paragraphs based on vertical proximity and alignment.
 
         Args:
             ocr_results (list): List of OCR results where each element is a tuple containing
                                 the bounding box and the recognized text.
 
         Returns:
             list: A list of paragraphs, each paragraph is a string.
         """
         # Define a threshold for vertical distance and horizontal misalignment
-        vertical_threshold = config.get("PADDLE_OCR_PARAGRAPH_VERTICAL_THRESHOLD",50)  # pixels
-        horizontal_threshold = config.get("PADDLE_OCR_PARAGRAPH_HORIZONTAL_THRESHOLD",10)  # pixels
+        vertical_threshold = config.get(
+            "PADDLE_OCR_PARAGRAPH_VERTICAL_THRESHOLD", 50
+        )  # pixels
+        horizontal_threshold = config.get(
+            "PADDLE_OCR_PARAGRAPH_HORIZONTAL_THRESHOLD", 10
+        )  # pixels
 
         paragraphs = []
         current_paragraph = []
         ocr_results = ocr_results[0]
         # Sort results by the top Y coordinate of the bounding box
         ocr_results.sort(key=lambda x: x[0][0][1])
-        
+
         for index in range(len(ocr_results)):
-            bbox  = ocr_results[index][0]
+            bbox = ocr_results[index][0]
             text = ocr_results[index][1][0]
             if index == 0:
                 current_paragraph.append(text)
             else:
                 previous_bbox = ocr_results[index - 1][0]
                 # Check vertical distance and horizontal alignment
                 vertical_distance = bbox[0][1] - previous_bbox[0][1]
                 horizontal_misalignment = abs(bbox[0][0] - previous_bbox[0][0])
-                if (vertical_distance < vertical_threshold and
-                        horizontal_misalignment < horizontal_threshold):
+                if (
+                    vertical_distance < vertical_threshold
+                    and horizontal_misalignment < horizontal_threshold
+                ):
                     current_paragraph.append(text)
                 else:
                     # Combine current paragraph and start a new one
-                    paragraphs.append(' '.join(current_paragraph))
+                    paragraphs.append(" ".join(current_paragraph))
                     current_paragraph = [text]
 
         # Add the last paragraph if any
         if current_paragraph:
-            paragraphs.append(' '.join(current_paragraph))
+            paragraphs.append(" ".join(current_paragraph))
 
         return paragraphs
-                
-
-
-
```

### Comparing `flexidata-0.0.2/flexidata/parser/pdf.py` & `flexidata-0.0.3/flexidata/parser/pdf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 from pdfminer.converter import PDFPageAggregator
 from pdfminer.layout import LAParams, LTContainer, LTImage
 from pdfminer.pdfinterp import PDFPageInterpreter, PDFResourceManager
 from pdfminer.pdfpage import PDFPage
 import re
-from typing import BinaryIO, cast, Optional
-import logging
+from typing import BinaryIO, cast, Optional, List, Dict, Any, Tuple
 from pdf2image import convert_from_path, pdfinfo_from_path
+import tempfile
 from flexidata.models.base import get_model
 from PIL import Image
 import layoutparser as lp
 from flexidata.utils.constants import (
     ParserMethod,
     FileType,
     Patterns,
     FileReaderSource,
     EXTRACTIONSOURCE,
-    OCREngine,
 )
 from flexidata.utils.pdf import rect_to_bbox, normalize_whitespace
-from flexidata.utils.text import TextType
 from pdfminer.pdftypes import PDFObjRef
 from flexidata.Logger import Logger
 from flexidata.reader.factory import get_file_reader
-from flexidata.ocr.agent import get_ocr_agent
+from flexidata.ocr.agent import OCRAgentFactory
 from pdfminer.layout import LTContainer
-from rapidocr_onnxruntime import RapidOCR
 import numpy as np
 from PIL import Image
+from flexidata.text_processing.text_block import TextBlock, TextBlockMetadata
+from flexidata.reader.handlers import FileHandler
+from PIL import Image as PILImage
+from flexidata.utils.constants import FileType
+from flexidata.utils.decorators import validate_file_type_method
 
 
 logger = Logger()
 
 PDF_LOSSY_COMPRESSION_FILTERS = ["DCTDecode", "DCT", "JPXDecode"]
 PDF_LOSSLESS_COMPRESSION_FILTERS = [
     "LZWDecode",
@@ -45,26 +47,25 @@
     "RL",
     "CCITTFaxDecode",
     "CCF",
     "JBIG2Decode",
 ]
 
 
-class PDFParser:
+class PDFParser(FileHandler):
     """_summary_"""
 
     def __init__(
         self,
         file_path: Optional[str] = None,
         file_url: Optional[str] = None,
         source: FileReaderSource = FileReaderSource.LOCAL,
         method: ParserMethod = ParserMethod.AUTO,
         extract_table: bool = False,
         extract_image: bool = False,
-        output_folder: Optional[str] = None,
         bucket_name: Optional[str] = None,
         file_key: Optional[str] = None,
         **kwargs,
     ) -> None:
         """Initialize the PDF parser with specified parameters.
 
         Args:
@@ -75,58 +76,31 @@
             extract_table (bool): Flag to indicate if tables should be extracted.
             extract_image (bool): Flag to indicate if images should be extracted.
             output_folder (Optional[str]): Folder path for storing output.
             bucket_name (Optional[str]): Name of the S3 bucket (for S3 sources).
             file_key (Optional[str]): File key within the S3 bucket.
             **kwargs: Additional keyword arguments for future extensibility.
         """
+        super().__init__(source, file_path, file_url, bucket_name, file_key)
         self.pdf_resource_manager = PDFResourceManager()
         self.la_params = LAParams()
         try:
             self.device = PDFPageAggregator(
                 self.pdf_resource_manager, laparams=self.la_params
             )
             self.interpreter = PDFPageInterpreter(
                 self.pdf_resource_manager, self.device
             )
         except Exception as e:
             raise RuntimeError(f"Failed to initialize PDF parsing resources: {str(e)}")
-        self.file_path = file_path
         self.method = method
-        self.output_folder = output_folder
         self.starting_page_number = 1
         self.extract_table = extract_table
         self.extract_image = extract_image
         self.text_extractable = False
-        self.source = source
-        self.file_url = file_url
-        self.bucket_name = bucket_name
-        self.file_key = file_key
-
-    def get_file_content(self) -> BinaryIO:
-        """
-        Get the content of the file based on the specified source.
-
-        Returns:
-            BinaryIO: The file content as a binary stream.
-        """
-        # No need to generate new file content if source is local or web URL
-        if self.source == FileReaderSource.LOCAL:
-            reader = get_file_reader(source_type=self.source, file_path=self.file_path)
-        elif self.source == FileReaderSource.WEB_URL:
-            reader = get_file_reader(source_type=self.source, url=self.file_url)
-        elif self.source == FileReaderSource.S3:
-            reader = get_file_reader(
-                source_type=self.source,
-                bucket_name=self.bucket_name,
-                file_key=self.file_key,
-            )
-        else:
-            raise ValueError(f"Unsupported source type: {self.source}")
-        return reader.read_file()
 
     def set_parser_auto_method(self):
         """
         Automatically sets the parsing method based on the content characteristics of the PDF.
 
         This method determines the optimal parsing method by evaluating whether the PDF contains
         images or tables that need extraction or whether text is readily extractable. It sets the
@@ -146,47 +120,114 @@
         elif self.text_extractable:
             self.method = ParserMethod.FAST
         # If no text is directly extractable, fall back to OCR
         else:
             self.method = ParserMethod.OCR
 
         return self.method  # Return the selected method
+    
+    @validate_file_type_method([FileType.PDF])
+    def parse(self, extract_image: bool = False) -> List[List[Dict[str, Any]]]:
+        """
+        Parses the document based on the specified method set in `self.method`.
 
-    def parse(self, extract_image=False):
-        """_summary_
+        Args:
+            extract_image (bool): If True, image extraction mode is enabled.
 
         Returns:
-            _type_: _description_
+           List[List[Dict[str, Any]]]: A list of elements parsed from the document according to the chosen parser method.
         """
         if extract_image:
             self.extract_image = extract_image
-        elements = []
-        self.text_extractable, elements = self.parse_by_pdfminer()
+
+        elements: List[List[Dict[str, Any]]] = []
+
         if self.method == ParserMethod.AUTO:
             self.set_parser_auto_method()
+
+        if self.source is not FileReaderSource.LOCAL:
+            self.file_path = self.create_temp_file(cast(BinaryIO, self.get_file_content()))
+
         if self.method == ParserMethod.FAST:
-            return elements
+            self.text_extractable, elements = self.parse_by_pdfminer()
         elif self.method == ParserMethod.MODEL:
-            self.parse_by_model()
+            elements = self.parse_by_model()
         elif self.method == ParserMethod.OCR:
-            self.parse_by_ocr()
+            elements = self.parse_by_ocr()
+        
+        if self.source is not FileReaderSource.LOCAL:
+            self._delete_temp_file(self.file_path)
+        return elements
 
-    def parse_by_model(self):
+    def parse_by_model(self, is_image=False):
         """_summary_"""
         pages_image = self.convert_pdf_to_image(self.file_path, self.output_folder)
         self.process_images(pages_image=pages_image)
 
-    def parse_by_ocr(self):
-        ocr_agent = get_ocr_agent(engine=OCREngine.PADDLE)
-        for page_number, image in enumerate(
-            self.convert_pdf_to_image(), start=self.starting_page_number
-        ):
-            logger.info(f"start extracting text form page:{page_number}")
-            text = ocr_agent.image_to_text(np.array(image), lang="eng")
-            logger.info(f"text extracted form page:{page_number} = {text}")
+    def parse_by_ocr(self, is_image: bool = False) -> List[List[TextBlock]]:
+        """
+        Parses the PDF by converting it to images and applying OCR to extract text elements.
+        If 'is_image' is set to True, treats the source file as an image directly instead of a PDF.
+
+        Args:
+            is_image (bool): Flag indicating whether the source file is an image.
+
+        Returns:
+            List[List[TextBlock]]: A nested list where each sublist represents OCR'd text blocks
+            from each page or image, along with their metadata.
+        """
+        ocr_factory = OCRAgentFactory()
+        ocr_agent = ocr_factory.get_ocr_agent()  # Get the OCR agent instance
+        elements: List[List[TextBlock]] = (
+            []
+        )  # Initialize the list to hold all OCR'd elements
+
+        # Handle direct image OCR if the source file is an image
+        if is_image:
+            if self.source is not FileReaderSource.LOCAL:
+                self.file_path = self.create_temp_file(cast(BinaryIO, self.get_file_content()))
+            images = []
+            image = PILImage.open(self.file_path)
+            images.append(image)
+            for page_number, image in enumerate(images, start=1):
+                page_elements = ocr_agent.image_to_text(
+                    np.array(image),
+                    lang="eng",
+                    page_number=page_number,
+                    file_path=self.get_file_path_by_source(),
+                    filetype=FileType.PDF,
+                )
+                elements.append(page_elements)
+            if self.source is not FileReaderSource.LOCAL:
+                self._delete_temp_file(self.file_path)
+        else:
+            # Process each page of the PDF converted to images
+            # Enumerate over each image page, starting from the specified page number
+            for page_number, image in enumerate(
+                self.convert_pdf_to_image(), start=self.starting_page_number
+            ):
+                # Convert image to numpy array and perform OCR
+                page_elements = ocr_agent.image_to_text(
+                    np.array(image),
+                    lang="eng",
+                    page_number=page_number,
+                    file_path=self.get_file_path_by_source(),
+                    filetype=FileType.PDF,
+                )
+                elements.append(page_elements)
+        return elements
+
+    def get_pdf_info(self):
+        """
+        Get the information about the PDF file.
+
+        Returns:
+            dict: A dictionary containing the PDF file information.
+        """
+        return pdfinfo_from_path(self.file_path)
 
     def convert_pdf_to_image(self, pages_per_chunk=10):
         """
         Convert PDF file to images in chunks, yielding images page by page.
 
         This method divides the PDF into chunks of pages and converts each chunk into images,
         which are then yielded one at a time. This is useful for processing large PDFs or
@@ -194,16 +235,15 @@
 
         Args:
             pages_per_chunk (int): Number of pages to process in each chunk.
 
         Yields:
             str: Path to the converted image if output_folder is specified, else PIL image object.
         """
-        logger.info("Starting conversion of PDF to images.")
-        pdf_info = pdfinfo_from_path(self.file_path)
+        pdf_info = self.get_pdf_info()
 
         # Iterate over each chunk of pages
         for start_page in range(1, pdf_info["Pages"] + 1, pages_per_chunk):
             end_page = min(start_page + pages_per_chunk - 1, pdf_info["Pages"])
 
             # Convert pages from start_page to end_page
             if self.output_folder:
@@ -381,61 +421,57 @@
                 result = [text[1] for text in result]
                 # Join all recognized text segments from this image and append to the overall text
                 text += "\n".join(result)
 
         # Return the concatenated text from all images
         return text
 
-    def parse_by_pdfminer(self):
-        """_summary_
+    def parse_by_pdfminer(self)-> Tuple[bool, List[List[TextBlock]]]:
+        """
+        Parses the PDF file using pdfminer, extracting text blocks and their metadata.
 
         Returns:
-            _type_: _description_
+            Tuple[bool, List[List[TextBlock]]]: A tuple containing a boolean indicating if text was extractable,
+            and a list of lists of TextBlock instances for each page.
         """
         text_extractable = False
         elements = []
         fp = cast(BinaryIO, self.get_file_content())
         for page_number, (page, page_layout) in enumerate(
             self.get_pdfminer_pages(fp), start=self.starting_page_number
         ):
             page_elements = []
             width, height = page_layout.width, page_layout.height
-            logger.info(
-                f"started processing page_number={page_number} width={width}, height={height}"
-            )
             # if page.annots:
             #     logger.info(f"page_number={page_number} has a annotation")
             #     urls = self.get_urls(page.annots, page_number, height)
             for element_obj in page_layout:
                 element_bbox = rect_to_bbox(element_obj.bbox, height)
                 if hasattr(element_obj, "get_text"):
                     texts = [element_obj.get_text()]
                 else:
                     text = self.extract_text(element_obj)
                     texts = re.split(Patterns.WHITESPACE_NEWLINE_PATTERN, text)
                 for text in texts:
                     text = normalize_whitespace(text)
                     if text:
+                        metadata = TextBlockMetadata(
+                            file_path=self.get_file_path_by_source(),
+                            languages=["eng"],
+                            filetype=FileType.PDF,
+                            page_number=page_number,
+                            bbox=element_bbox,
+                            layout_height=height,
+                            layout_width=width,
+                            extraction_source=EXTRACTIONSOURCE.PDF_MINER,
+                        )
+                        element = TextBlock(text=text, metadata=metadata)
                         text_extractable = True
-                        text_type = TextType.find_text_type(text)
-                        element = {"Type": text_type, "Text": text}
-                        element["metadata"] = {
-                            "file_path": self.file_path,
-                            "languages": ["eng"],
-                            "filetype": FileType.PDF,
-                            "page_numer": page_number,
-                            "bbox": element_bbox,
-                            "layout_height": height,
-                            "layout_width": width,
-                            "extraction_source": EXTRACTIONSOURCE.PDF_MINER,
-                        }
                         page_elements.append(element)
             elements.append(page_elements)
-            logger.info(f"completed for page={page_number}")
-        logger.info(f"page_elements={elements}")
         return text_extractable, elements
 
     def extract_text(self, element):
         """
         Recursively extract text from a layout element of a PDF page.
 
         This function checks the type of the element and appropriately extracts text. If the element
```

### Comparing `flexidata-0.0.2/flexidata/utils/pdf.py` & `flexidata-0.0.3/flexidata/utils/pdf.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from PIL import ImageDraw
 import fitz
 import re
+from flexidata.utils.decorators import is_debug_enabled
 
 def rect_to_bbox(rect, page_height):
     """
     Converts a rectangle's coordinates from a PDF coordinate system (origin at bottom-left)
     to a more standard bounding box format (origin at top-left).
 
     This is useful for graphic operations that expect coordinates with the origin at the top-left,
@@ -27,15 +28,15 @@
     y2 = page_height - y2
 
     # Return the converted bounding box
     return [x1, y1, x2, y2]
 
 
 
-def normalize_whitespace(text):
+def normalize_whitespace(text: str) -> str:
     """
     Normalize the whitespace in a text string.
 
     This function replaces non-breaking spaces and newlines with a single space and collapses
     multiple spaces into a single space.
 
     Args:
@@ -67,32 +68,14 @@
         Args:
             file_name (str): Path to the PDF file to be debugged.
             debug (bool): Whether to enable debugging features.
         """
         self.debug = debug  # Set the debugging flag
         self.pages = fitz.open(file_name)  # Open the PDF file with fitz
 
-    @staticmethod
-    def is_debug_enabled(method):
-        """
-        Decorator to check if debugging is enabled before executing a method.
-        This is useful for controlling the execution of debugging-specific methods.
-        
-        Args:
-            method (callable): The method to be wrapped by the decorator.
-        
-        Returns:
-            callable: A wrapper function that checks the debug state before method execution.
-        """
-        def wrapper(self, *args, **kwargs):
-            if not self.debug:
-                return False  # If debugging is not enabled, do nothing
-            return method(self, *args, **kwargs)  # Otherwise, execute the method
-        return wrapper
-
     def get_page(self, page_number):
         """
         Retrieves a specific page from the PDF document.
         
         Args:
             page_number (int): The page number to retrieve (1-indexed).
```

### Comparing `flexidata-0.0.2/flexidata/utils/text.py` & `flexidata-0.0.3/flexidata/reader/handlers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,278 +1,279 @@
-import re
-from flexidata.utils.constants import Patterns
-import nltk
-from nltk.tokenize import sent_tokenize, word_tokenize
-from functools import wraps
-from nltk import pos_tag
-from langdetect import detect
-from langdetect.lang_detect_exception import LangDetectException
-from flexidata.Logger import Logger
-
-logger = Logger()
-
-
-def ensure_nltk_package(package_category, package_name):
-    def decorator(func):
-        @wraps(func)
-        def wrapper(*args, **kwargs):
-            try:
-                # Try to find the package
-                nltk.find(f"{package_category}/{package_name}")
-            except LookupError:
-                # If not found, download the package
-                print(f"{package_name} not found, downloading now...")
-                nltk.download(package_name)
-            return func(*args, **kwargs)
-        return wrapper
-    return decorator
+from typing import BinaryIO
+from flexidata.utils.constants import FileReaderSource, ParserMethod
+from flexidata.reader.factory import get_file_reader
+import os
+from io import BytesIO
+import tempfile
+from urllib.parse import urlparse, unquote
+from flexidata.utils.constants import FileType
 
-@ensure_nltk_package('tokenizers', 'punkt')
-def tokenize_sentences(text):
+class FileHandler:
     """
-    Tokenizes the given text into sentences.
-    
-    Parameters:
-    text (str): The text to tokenize into sentences.
-    
-    Returns:
-    list: A list of sentences extracted from the text.
-    
-    Example:
-    >>> sample_text = "Hello world. This is an example sentence. Short here."
-    >>> tokenize_sentences(sample_text)
-    ['Hello world. ', 'This is an example sentence.', 'Short here.']
-    """
-    return sent_tokenize(text)
+    Initializes a FileHandler object with details about the file source.
 
-@ensure_nltk_package('tokenizers','punkt')
-def tokenize_words(text):
-    """
-    Tokenizes the input text into words using NLTK's word_tokenize.
-    
-    Parameters:
-    text (str): The text to be tokenized into words.
-    
-    Returns:
-    list: A list of words and punctuation from the text.
-    
-    Example:
-    >>> sample_text = "Hello, world! This is an example."
-    >>> tokenize_words(sample_text)
-    ['Hello', ',', 'world', '!', 'This', 'is', 'an', 'example', '.']
+    Args:
+        source (str): The source type of the file, e.g., 'local', 'web_url', or 's3'.
+        file_path (str, optional): The file path if the source is local. Defaults to None.
+        file_url (str, optional): The URL of the file if the source is a web URL. Defaults to None.
+        bucket_name (str, optional): The name of the S3 bucket if the source is S3. Defaults to None.
+        file_key (str, optional): The key of the file within the S3 bucket if the source is S3. Defaults to None.
     """
-    return word_tokenize(text)
 
-def no_of_sentence(text, min_word_length):
-    count = 0
-    sentences = tokenize_sentences(text)
-    for sentence in sentences:
-        words = [word for word in tokenize_words(sentence) if word != "."]
-        if len(words) < min_word_length:
-            continue
-        count = count + 1
-    return count
+    def __init__(self, source, file_path=None, file_url=None, bucket_name=None, file_key=None, file_type=None):
+        self.source = source
+        self.file_path = file_path
+        self.file_url = file_url
+        self.bucket_name = bucket_name
+        self.file_key = file_key
+        if source not in [FileReaderSource.LOCAL, FileReaderSource.WEB_URL, FileReaderSource.S3]:
+            raise ValueError(f"Unsupported source type: {source}")
+
+        if source == FileReaderSource.LOCAL and not file_path:
+            raise ValueError("File path must be provided for local files.")
+        if source == FileReaderSource.WEB_URL and not file_url:
+            raise ValueError("File URL must be provided for web URL sources.")
+        if source == FileReaderSource.S3 and not (bucket_name and file_key):
+            raise ValueError("Bucket name and file key must be provided for S3 sources.")
+        if file_type is None:
+            self.file_type = self._get_file_extension()
+        else:
+            self.file_type = file_type
 
+    def get_file_content(self) -> BinaryIO:
+        """
+        Get the content of the file based on the specified source.
 
-def is_title(text, title_max_word_length=12, sentence_min_word_length=5):
-    """
-    Determines whether the provided text can be classified as a title based on several criteria.
-    
-    This function assesses the given text to decide if it fits the characteristics commonly
-    associated with titles. It evaluates conditions such as text length, numeric content,
-    punctuation, and word count to make this determination.
-
-    Parameters:
-    - text (str): The text to evaluate.
-    - title_max_word_length (int): Optional. The maximum number of words a title can
-      have to still be considered a title. Defaults to 12.
+        Returns:
+            BinaryIO: The file content as a binary stream.
+        """
+        # No need to generate new file content if source is local or web URL
+        if self.source == FileReaderSource.LOCAL:
+            reader = get_file_reader(source_type=self.source, file_path=self.file_path)
+        elif self.source == FileReaderSource.WEB_URL:
+            reader = get_file_reader(source_type=self.source, url=self.file_url)
+        elif self.source == FileReaderSource.S3:
+            reader = get_file_reader(
+                source_type=self.source,
+                bucket_name=self.bucket_name,
+                file_key=self.file_key,
+            )
+        else:
+            raise ValueError(f"Unsupported source type: {self.source}")
+        return reader.read_file()
     
-    Returns:
-    - bool: True if the text is likely a title, otherwise False.
+    def get_file_path_by_source(self):
+        """
+        Get the file path based on the specified source type.
 
-    Examples:
-    >>> is_title("Chapter 1: An Introduction")
-    False
-    >>> is_title("Introduction to Programming")
-    True
-    >>> is_title("12345")
-    False
-    >>> is_title("This is an excessively long sentence that should not be considered a title")
-    False
-
-    Logic:
-    - Returns False if the text is empty.
-    - Returns False if the text is numeric.
-    - Returns False if the text is determined to be numeric using the TextType.numeric_text.
-    - Returns False if the text ends with a punctuation mark, which is checked using
-      TextType.ends_with_punctuation.
-    - Returns False if the text ends with a comma.
-    - Returns False if the text contains more words than `title_max_word_length`.
-    
-    If none of the above conditions are met, the text is likely a title, and True is returned.
-    """
-    if len(text) == 0:
-        return False
-    if text.isnumeric() or TextType.numeric_text(text):
-        return False
-    if TextType.ends_with_punctuation(text):
-        return False
-    
-    try:
-        if detect(text) != 'en':
-            return False
-    except LangDetectException as e:
-        logger.info(f"LangDetectException: {e}")
-        return False
-    
-    if text.endswith(","):
-        return False
-    if len(text.split(" ")) > title_max_word_length:
-        return False
-    if no_of_sentence(text, sentence_min_word_length) > 1:
-        return False
+        Returns:
+            str: The file path based on the source type.
+        """
+        if self.source == FileReaderSource.LOCAL:
+            return self.file_path
+        elif self.source == FileReaderSource.WEB_URL:
+            return self.file_url
+        elif self.source == FileReaderSource.S3:
+            return self.file_key
+        else:
+            raise ValueError(f"Unsupported source type: {self.source}")
+        
+    def create_temp_file(self, file_content: BinaryIO) -> str:
+        """
+        Creates a temporary file from a BinaryIO stream.
+
+        Args:
+            file_content (BinaryIO): The BinaryIO stream containing the file data.
+
+        Returns:
+            str: The file path to the temporary file.
+        """
+        with tempfile.NamedTemporaryFile(delete=False) as tmp:
+            tmp.write(file_content.read())  # Write the BinaryIO content to a temp file
+            return tmp.name
     
-    return True
 
+    def _delete_temp_file(self, temp_file_path: str):
+        """
+        Deletes a temporary file specified by the file path.
 
-def is_list_item(text):
-    return bool(Patterns.LIST_ITEM_REGEX.match(text))
+        Args:
+            temp_file_path (str): The file path of the temporary file to be deleted.
+        """
+        try:
+            os.remove(temp_file_path)  # Attempt to remove the temporary file
+            print(f"Temporary file {temp_file_path} has been deleted successfully.")
+        except OSError as e:
+            print(f"Error: {temp_file_path} : {e.strerror}")  # Handle errors encountered during file deletion
 
-@ensure_nltk_package("taggers", "averaged_perceptron_tagger")
-def narrative_features(text, check_pronouns=False, check_temporal=False):
-    sentences = tokenize_sentences(text.lower())
-    verb_count = 0
-    first_person_pronouns_count = 0
-    temporal_words_count = 0
-    first_person_pronouns = {'i', 'we', 'us', 'our', 'ours', 'myself', 'ourselves'}
-    temporal_words = {'then', 'after', 'before', 'finally', 'previously', 'formerly'}
-
-    for sentence in sentences:
-        tokens = tokenize_words(sentence)
-        tagged_tokens = pos_tag(tokens)
-
-        for word, tag in tagged_tokens:
-            if tag.startswith('VB'):  # Any form of verb
-                verb_count += 1
-            if check_pronouns:
-                first_person_pronouns_count += sum(1 for word, _ in tagged_tokens if word.lower() in first_person_pronouns)
-
-            if check_temporal:
-                temporal_words_count += sum(1 for word, _ in tagged_tokens if word.lower() in temporal_words)
-
-    is_narrative = verb_count > 0
-    if check_pronouns:
-        is_narrative = is_narrative and first_person_pronouns_count > 0
-    if check_temporal:
-        is_narrative = is_narrative and temporal_words_count > 0
+    def _create_temp_file_with_content(self, content: str, file_type: str) -> str:
+        """
+        Creates a temporary file with the given content and file type.
 
-    return is_narrative
+        Args:
+            content (str): The content to write to the temporary file.
+            file_type (str): The file type/extension of the file (e.g., 'html', 'txt', 'json').
 
-def is_narrative_text(text):
+        Returns:
+            str: The path to the temporary file.
 
-    if len(text) == 0:
-        return False
-    
-    if text.isnumeric() or TextType.numeric_text(text):
-        return False
-    try:
-        if detect(text) != 'en':
-            return False
-    except LangDetectException as e:
-        logger.info(f"LangDetectException: {e}")
-        return False
+        Raises:
+            ValueError: If the file type is not supported.
+        """
+        # Define a mapping of file types to file extensions
+        file_extensions = {
+            'html': '.html',
+            'txt': '.txt',
+            'json': '.json',
+            'xml': '.xml',
+            'odt': '.odt',
+        }
+
+        # Check if the file type is supported
+        if file_type not in file_extensions:
+            raise ValueError(f"Unsupported file type: {file_type}")
+
+        # Get the file extension
+        extension = file_extensions[file_type]
+
+        # Create a temporary file with the appropriate extension
+        temp_file = tempfile.NamedTemporaryFile(delete=False, suffix=extension, mode='w', encoding='utf-8')
+
+        try:
+            # Write the content to the temporary file
+            temp_file.write(content)
+            temp_file.close()  # Ensure all data is written and file is closed
+            return temp_file
+        except Exception as e:
+            # If an error occurs, ensure the file is removed
+            os.unlink(temp_file.name)
+            raise RuntimeError(f"Failed to create temporary file: {e}") from e
+        
+    def byte_io_to_String(self, file_content: BytesIO) -> str:
+        """
+        Converts the contents of a BytesIO object into a string.
+
+        This method resets the read position of the BytesIO object to the beginning,
+        reads the bytes, and decodes them into a string using UTF-8 encoding. This is 
+        commonly used to convert binary data from files into a readable and processable 
+        string format.
 
-    if no_of_sentence(text, 3) < 2 and (not narrative_features(text)):
-        return False
+        Args:
+            file_content (BytesIO): The BytesIO object containing the file's binary content.
 
-    return True
+        Returns:
+            str: The decoded string content of the binary data.
+        """
+        file_content.seek(0)  # Reset the read position of the BytesIO object to the start
+        string_content = file_content.read().decode('utf-8')  # Decode the byte content to a string
+        return string_content
 
+    
+    def _get_extension_from_local_path(self, local_path: str) -> str:
+        """
+        Extracts the file extension from a local file path and retrieves its MIME type.
 
+        This method splits the file path to extract the extension, removes any leading periods,
+        converts the extension to lowercase, and then uses this extension to look up the
+        corresponding MIME type from a predefined list or dictionary of file types.
 
-class TextType:
-    """
-    Provides classification of text into predefined categories based on specific characteristics.
+        Args:
+            local_path (str): The path of the file on the local file system from which to extract the extension.
 
-    This class is designed to classify texts as titles, list items, or other types based on
-    patterns and functions that check for specific attributes in the text. It utilizes regular
-    expressions to determine if text ends with punctuation or is numeric, supporting text
-    analysis and processing tasks.
-
-    Attributes:
-        TITLE_TYPE (str): Represents a text identified as a title.
-        LIST_ITEM (str): Represents a text identified as a list item.
-        UNKNOWN (str): Default type when text does not match any specific category.
-
-    Methods:
-        find_text_type(text): Determines the type of the given text by checking against
-                              predefined criteria for list items and titles. Returns 'Unknown'
-                              if the text does not meet any specific criteria.
-        ends_with_punctuation(text): Checks if the text ends with a punctuation mark.
-                                     Returns True if it does, False otherwise.
-        numeric_text(text): Determines if the text is numeric. Returns True if it is,
-                            False otherwise.
-
-    Example usage:
-        >>> TextType.find_text_type("Chapter 1: Introduction")
-        'Title'
-        >>> TextType.ends_with_punctuation("Hello, world!")
-        True
-        >>> TextType.numeric_text("1234")
-        True
-    """
+        Returns:
+            str: The MIME type corresponding to the extracted file extension.
+        """
+        extension = (os.path.splitext(local_path)[1].lstrip('.')).lower()  # Extract and process the file extension
+        return FileType.get_mime_type(extension)  # Retrieve the MIME type based on the file extension
+    
+    def _get_extension_from_s3_key(self, s3_key: str) -> str:
+        """
+        Extracts the file extension from an S3 object key and retrieves its MIME type.
 
-    EMAILL_TYPE = "Email"
-    TITLE_TYPE = "Title"
-    LIST_ITEM = "ListItem"
-    NERATIVE_TEXT = "NerativeText"
-    UNKNOWN = "Unknown"
-
-    @staticmethod
-    def find_text_type(text):
-        """
-        Determines the type of the given text by evaluating it against predefined criteria for list items and titles.
-
-        This method classifies text as a list item, title, or unknown based on specific checks performed by
-        helper functions (`is_list_item` and `is_title`). It sequentially tests each condition and returns
-        the corresponding text type upon the first match.
+        This method takes the S3 object key, which often represents the file name and path
+        in the S3 bucket, splits it to extract the extension part, cleans it by removing any leading periods,
+        converts it to lowercase, and then uses this extension to look up the corresponding MIME type
+        from a predefined list or dictionary of file types.
 
-        Parameters:
-        - text (str): The text whose type is to be determined.
+        Args:
+            s3_key (str): The S3 object key from which to extract the file extension.
 
         Returns:
-        - str: The determined type of the text. It can be 'ListItem' if the text qualifies as a list item,
-            'Title' if it qualifies as a title, or 'Unknown' if it does not meet any specific criteria.
+            str: The MIME type corresponding to the extracted file extension.
+        """
+        extension = (os.path.splitext(s3_key)[1].lstrip('.')).lower()  # Extract and process the file extension
+        return FileType.get_mime_type(extension)  # Retrieve the MIME type based on the file extension
+    
 
-        Examples:
-        >>> TextType.find_text_type("1. Introduction")
-        'ListItem'
-        >>> TextType.find_text_type("Introduction to Python")
-        'Title'
-        >>> TextType.find_text_type("This text does not fit any known category.")
-        'Unknown'
-
-        The method uses the following logic:
-        - First, it checks if the text is a list item using `is_list_item`. If true, it returns 'ListItem'.
-        - If the first check fails, it checks if the text is a title using `is_title`. If true, it returns 'Title'.
-        - If all checks fail, it returns 'Unknown'.
-        """
-        if is_list_item(text):
-            return TextType.LIST_ITEM
-        elif is_narrative_text(text):
-            return TextType.NERATIVE_TEXT
-        elif is_title(text):
-            return TextType.TITLE_TYPE
-        else:
-            return TextType.UNKNOWN
+    def _get_extension_from_google_drive(file_id: str) -> str:
+        pass
 
+
+    
+    def _get_file_extension(self) -> str:
+        """
+        Determines the file extension based on the source of the file.
+
+        Depending on the file source specified (e.g., web URL, local storage, S3, or Google Drive),
+        this method delegates to the appropriate helper function to extract the file extension.
         
+        Returns:
+            str: The file extension of the specified file.
         
-    @staticmethod
-    def ends_with_punctuation(text):
-        ends_in_punct_pattern = re.compile(Patterns.END_WITH_PUNCTUATION)
-        return bool(ends_in_punct_pattern.search(text))
-
-    @staticmethod
-    def numeric_text(text):
-        numeric_text_pattern = re.compile(Patterns.NUMERIC_REGEX)
-        return bool(numeric_text_pattern.search(text))
-    
+        Raises:
+            ValueError: If the file source is not supported, indicating the need for a valid source specification.
+        """
+        if self.source == "web_url":
+            return self._get_file_extension_from_url(self.file_url)
+        elif self.source == "local":
+            return self._get_extension_from_local_path(self.file_path)
+        elif self.source == "s3":
+            return self._get_extension_from_s3_key(self.file_key)
+        elif self.source == "google_drive":
+            return self._get_extension_from_google_drive(self.file_key)
+        else:
+            raise ValueError(f"Unsupported source type: {self.source}")
+
+
+    
+    def _get_file_extension_from_url(url: str) -> str:
+        """
+        Extracts the file extension from a URL, handling URLs that may include query parameters or fragments.
+
+        Args:
+            url (str): The URL from which to extract the file extension.
+
+        Returns:
+            str: The file extension extracted from the URL, or an empty string if no extension could be identified.
+        """
+        # Parse the URL to remove any query parameters or fragments
+        parsed_url = urlparse(url)
+        # Unquote to decode any URL-encoded parts of the path (e.g., %20 for space)
+        path = unquote(parsed_url.path)
+        extension = os.path.splitext(path)[1][1:]  # Remove the dot and extract the extension
+        if extension:
+            return FileType.get_mime_type(extension)
+        else:
+            return FileType.HTML  # Default to HTML if no extension is present
+    
+    def _create_temp_directory(self) -> str:
+        """
+        Creates a temporary directory and returns the path to the directory.
+
+        Returns:
+            str: The path to the temporary directory.
+        """
+        return tempfile.TemporaryDirectory()
+    
+    def _delete_temp_directory(self, temp_dir: str):
+        """
+        Deletes a temporary directory and its contents.
+
+        Args:
+            temp_dir (str): The path to the temporary directory to delete.
+        """
+        try:
+            temp_dir.cleanup()  # Cleanup the temporary directory
+            print(f"Temporary directory {temp_dir} has been deleted successfully.")
+        except OSError as e:
+            print(f"Error: {temp_dir} : {e.strerror}")
+
```

### Comparing `flexidata-0.0.2/flexidata.egg-info/PKG-INFO` & `flexidata-0.0.3/flexidata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.2
+Version: 0.0.3
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -210,14 +210,15 @@
 Keywords: PDF,DOCX document parsing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: pdfplumber==0.11.0
 Requires-Dist: pdf2image==1.17.0
 Requires-Dist: poppler-utils==0.1.0
 Requires-Dist: pillow==10.3.0
 Requires-Dist: numpy==1.26.4
 Requires-Dist: scipy==1.13.0
 Requires-Dist: layoutparser==0.3.4
@@ -233,33 +234,43 @@
 Requires-Dist: boto3==1.34.102
 Requires-Dist: requests==2.31.0
 Requires-Dist: pytesseract==0.3.10
 Requires-Dist: paddlepaddle==2.6.1
 Requires-Dist: paddlepaddle-gpu==2.6.1
 Requires-Dist: paddleocr==2.7.3
 Requires-Dist: google-cloud-vision==3.7.2
+Requires-Dist: python-docx==1.1.2
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: lxml==5.2.2
+Requires-Dist: python-pptx==0.6.23
+Requires-Dist: Markdown==3.6
+Requires-Dist: pypandoc==1.13
 
 # flexidata
 
 FlexiData is an open-source Python package designed for processing unstructured data. Currently, it supports PDF extraction with plans to expand to other file types in the future.
 
 ## Features
 
-- **PDF Extraction**: Efficiently extract text and metadata from PDF files.
+- **Document  Parser**: The tool is designed to parse various file types, efficiently extracting text blocks and their metadata. This enables streamlined data extraction and content manipulation across multiple document formats.
 
-## Contributing
+  ### Supported File Formats:
+    - **PDF**: For detailed extraction of text and metadata.
+    - **Images** (JPEG, PNG, BMP): Enables image data and metadata processing.
+    - **EPUB**: Converts and extracts content from EPUB files.
+    - **HTML**: Parses HTML content for data extraction.
+    - **reStructuredText (RST)**: Handles conversion and parsing of RST files.
+    - **Rich Text Format (RTF)**: Facilitates conversion and content extraction from RTF documents.
+    - **DOCX**: Allows extraction from DOCX documents, providing access to structured content and metadata.
+
+## Upcoming Features:
+- **Content Chunking**: This will enable dividing text into meaningful and manageable pieces for better processing and analysis.
+- **Data Embedding**: Planned to support embedding textual data into vector spaces for advanced data analysis and machine learning applications.
 
-Contributions to FlexiData are welcome! If you're interested in contributing, please read our contributing guidelines.
 
-## Roadmap
+## Contributing
 
-- [x] PDF extraction support
-- [ ] Support for other file formats (e.g., Word, Excel, text files)
-- [ ] Advanced text processing features (e.g., natural language processing)
+Contributions to FlexiData are welcome! If you're interested in contributing, please read our contributing guidelines.
 
 ## Development Status
 
 FlexiData is currently in active development and we are working towards releasing our first version soon.
-
-
-
-
```

### Comparing `flexidata-0.0.2/flexidata.egg-info/SOURCES.txt` & `flexidata-0.0.3/flexidata.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.py
+examples/__init__.py
+examples/run.py
 flexidata/Logger.py
 flexidata/__init__.py
 flexidata.egg-info/PKG-INFO
 flexidata.egg-info/SOURCES.txt
 flexidata.egg-info/dependency_links.txt
 flexidata.egg-info/requires.txt
 flexidata.egg-info/top_level.txt
@@ -16,21 +18,44 @@
 flexidata/models/detectron2.py
 flexidata/ocr/__init__.py
 flexidata/ocr/agent.py
 flexidata/ocr/google_vision.py
 flexidata/ocr/paddle.py
 flexidata/ocr/tesseract.py
 flexidata/parser/__init__.py
+flexidata/parser/document.py
+flexidata/parser/docx.py
+flexidata/parser/epub.py
+flexidata/parser/html.py
+flexidata/parser/image.py
+flexidata/parser/md.py
+flexidata/parser/odt.py
+flexidata/parser/org.py
 flexidata/parser/pdf.py
+flexidata/parser/pptx.py
+flexidata/parser/rst.py
+flexidata/parser/rtf.py
+flexidata/preprocessor/__init__.py
+flexidata/preprocessor/base.py
 flexidata/reader/__init__.py
 flexidata/reader/factory.py
 flexidata/reader/file_reader.py
 flexidata/reader/google_drive.py
+flexidata/reader/handlers.py
 flexidata/reader/local.py
 flexidata/reader/s3.py
 flexidata/reader/web.py
+flexidata/text_processing/__init__.py
+flexidata/text_processing/classification.py
+flexidata/text_processing/convert_file.py
+flexidata/text_processing/text_block.py
 flexidata/utils/__init__.py
 flexidata/utils/common.py
 flexidata/utils/constants.py
+flexidata/utils/decorators.py
 flexidata/utils/pdf.py
 flexidata/utils/text.py
-tests/test_pdf.py
+tests/__init__.py
+tests/ocr/__init__.py
+tests/ocr/test_agent.py
+tests/utils/__init__.py
+tests/utils/test_common.py
```

### Comparing `flexidata-0.0.2/pyproject.toml` & `flexidata-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flexidata"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Kalyanakannan Padivasu", email="Kalyanakannan.p@gmail.com" },
 ]
 description = "FlexiData is an open-source Python package designed for processing unstructured data."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["PDF,DOCX document parsing"]
```

