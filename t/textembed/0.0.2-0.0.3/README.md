# Comparing `tmp/textembed-0.0.2.tar.gz` & `tmp/textembed-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textembed-0.0.2.tar", last modified: Sat May 25 20:06:32 2024, max compression
+gzip compressed data, was "textembed-0.0.3.tar", last modified: Wed May 29 17:33:39 2024, max compression
```

## Comparing `textembed-0.0.2.tar` & `textembed-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.767008 textembed-0.0.2/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)    11357 2024-05-09 02:26:44.000000 textembed-0.0.2/LICENSE
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     5088 2024-05-25 20:06:32.766696 textembed-0.0.2/PKG-INFO
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1944 2024-05-21 18:08:40.000000 textembed-0.0.2/README.md
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       38 2024-05-25 20:06:32.767074 textembed-0.0.2/setup.cfg
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2783 2024-05-21 17:33:43.000000 textembed-0.0.2/setup.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.756629 textembed-0.0.2/src/
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.758988 textembed-0.0.2/src/textembed/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      173 2024-05-25 19:30:05.000000 textembed-0.0.2/src/textembed/__init__.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.761771 textembed-0.0.2/src/textembed/api/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:03:33.000000 textembed-0.0.2/src/textembed/api/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1480 2024-05-18 06:41:14.000000 textembed-0.0.2/src/textembed/api/docs.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2660 2024-05-25 19:12:49.000000 textembed-0.0.2/src/textembed/api/embed.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1603 2024-05-19 11:18:20.000000 textembed-0.0.2/src/textembed/api/monitor.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     3406 2024-05-18 19:33:48.000000 textembed-0.0.2/src/textembed/api/schemas.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.762363 textembed-0.0.2/src/textembed/application/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-17 19:06:13.000000 textembed-0.0.2/src/textembed/application/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2056 2024-05-24 18:21:49.000000 textembed-0.0.2/src/textembed/application/application.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.763089 textembed-0.0.2/src/textembed/batch/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      107 2024-05-23 17:30:42.000000 textembed-0.0.2/src/textembed/batch/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4101 2024-05-25 19:12:58.000000 textembed-0.0.2/src/textembed/batch/batch_processor.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.763645 textembed-0.0.2/src/textembed/cache/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:12:00.000000 textembed-0.0.2/src/textembed/cache/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       28 2024-05-19 11:26:25.000000 textembed-0.0.2/src/textembed/cache/cache.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.764539 textembed-0.0.2/src/textembed/engine/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-05 17:38:30.000000 textembed-0.0.2/src/textembed/engine/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1862 2024-05-25 19:03:14.000000 textembed-0.0.2/src/textembed/engine/args.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     4210 2024-05-25 19:00:57.000000 textembed-0.0.2/src/textembed/engine/async_engine.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.765422 textembed-0.0.2/src/textembed/executor/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-18 19:35:33.000000 textembed-0.0.2/src/textembed/executor/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1731 2024-05-19 09:12:34.000000 textembed-0.0.2/src/textembed/executor/base.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.765931 textembed-0.0.2/src/textembed/executor/embedder/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-19 09:25:22.000000 textembed-0.0.2/src/textembed/executor/embedder/__init__.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2901 2024-05-25 18:40:21.000000 textembed-0.0.2/src/textembed/executor/embedder/sentence_transformer.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      494 2024-05-19 04:53:46.000000 textembed-0.0.2/src/textembed/executor/primitives.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1584 2024-05-25 19:11:54.000000 textembed-0.0.2/src/textembed/log.py
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     2491 2024-05-25 19:22:38.000000 textembed-0.0.2/src/textembed/server.py
-drwxr-xr-x   0 kevaldekivadiya   (501) staff       (20)        0 2024-05-25 20:06:32.760332 textembed-0.0.2/src/textembed.egg-info/
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     5088 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/PKG-INFO
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)      935 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/SOURCES.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)        1 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/dependency_links.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)     1062 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/requires.txt
--rw-r--r--   0 kevaldekivadiya   (501) staff       (20)       10 2024-05-25 20:06:32.000000 textembed-0.0.2/src/textembed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-29 17:33:35.000000 textembed-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 17:33:35.000000 textembed-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 17:33:39.445384 textembed-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-29 17:33:35.000000 textembed-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 17:33:35.000000 textembed-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:33:39.445384 textembed-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-29 17:33:35.000000 textembed-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.437384 textembed-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.441384 textembed-0.0.3/src/textembed/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.441384 textembed-0.0.3/src/textembed/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/application/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/batch/batch_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/cache/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/async_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/executor/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/embedder/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/top_level.txt
```

### Comparing `textembed-0.0.2/LICENSE` & `textembed-0.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2024] Keval Dekivadiya
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `textembed-0.0.2/PKG-INFO` & `textembed-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.2
+Version: 0.0.3
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
@@ -85,42 +85,30 @@
 TextEmbed is a high-throughput, low-latency REST API designed for serving vector embeddings. It supports a wide range of sentence-transformer models and frameworks, making it suitable for various applications in natural language processing.
 
 ## Features
 
 - **High Throughput & Low Latency:** Designed to handle a large number of requests efficiently.
 - **Flexible Model Support:** Works with various sentence-transformer models.
 - **Scalable:** Easily integrates into larger systems and scales with demand.
-- **REST API:** Simple and accessible API endpoints.
+- **Batch Processing:** Supports batch processing for better and faster inference.
+- **OpenAI Compatible REST API Endpoint:** Provides an OpenAI compatible REST API endpoint.
 
 ## Getting Started
 
 ### Prerequisites
 
-Ensure you have Python 3.10 or higher installed. You will also need to install the required dependencies.
+Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
-1. Clone the repository:
-    ```bash
-    git clone https://github.com/kevaldekivadiya2415/textembed.git
-    cd textembed
-    ```
-
-2. Install the dependencies:
+1. Install the required dependencies:
     ```bash
     pip install -r requirements.txt
     ```
 
-### Running the Server
-
-1. Set up the package in development mode:
-    ```bash
-    python3 setup.py develop
-    ```
-
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
 
     Replace `<Model Name>` with the name of the model you want to use.
 
@@ -128,20 +116,19 @@
     ```bash
     python3 -m textembed.server --help
     ```
 
 ### Running with Docker (Recommended)
 You can also run TextEmbed using Docker. The Docker image is available on Docker Hub.
 ```bash
-docker run keval2415/textembed:0.0.1 --help
+docker run kevaldekivadiya/textembed:latest --help
 ```
 This command will show the help message for the TextEmbed server, detailing the available options and usage.
 
 For Example:
 ```bash
-docker run -p 8000:8000 keval2415/textembed:0.0.1 --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
+docker run -p 8000:8000 kevaldekivadiya/textembed:latest --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
 ```
 
 ### Accessing the API
 
 Once the server is running, you can access the API documentation via Swagger UI.
-
```

### Comparing `textembed-0.0.2/README.md` & `textembed-0.0.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,42 +3,30 @@
 TextEmbed is a high-throughput, low-latency REST API designed for serving vector embeddings. It supports a wide range of sentence-transformer models and frameworks, making it suitable for various applications in natural language processing.
 
 ## Features
 
 - **High Throughput & Low Latency:** Designed to handle a large number of requests efficiently.
 - **Flexible Model Support:** Works with various sentence-transformer models.
 - **Scalable:** Easily integrates into larger systems and scales with demand.
-- **REST API:** Simple and accessible API endpoints.
+- **Batch Processing:** Supports batch processing for better and faster inference.
+- **OpenAI Compatible REST API Endpoint:** Provides an OpenAI compatible REST API endpoint.
 
 ## Getting Started
 
 ### Prerequisites
 
-Ensure you have Python 3.10 or higher installed. You will also need to install the required dependencies.
+Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
-1. Clone the repository:
-    ```bash
-    git clone https://github.com/kevaldekivadiya2415/textembed.git
-    cd textembed
-    ```
-
-2. Install the dependencies:
+1. Install the required dependencies:
     ```bash
     pip install -r requirements.txt
     ```
 
-### Running the Server
-
-1. Set up the package in development mode:
-    ```bash
-    python3 setup.py develop
-    ```
-
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
 
     Replace `<Model Name>` with the name of the model you want to use.
 
@@ -46,20 +34,19 @@
     ```bash
     python3 -m textembed.server --help
     ```
 
 ### Running with Docker (Recommended)
 You can also run TextEmbed using Docker. The Docker image is available on Docker Hub.
 ```bash
-docker run keval2415/textembed:0.0.1 --help
+docker run kevaldekivadiya/textembed:latest --help
 ```
 This command will show the help message for the TextEmbed server, detailing the available options and usage.
 
 For Example:
 ```bash
-docker run -p 8000:8000 keval2415/textembed:0.0.1 --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
+docker run -p 8000:8000 kevaldekivadiya/textembed:latest --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
 ```
 
 ### Accessing the API
 
-Once the server is running, you can access the API documentation via Swagger UI.
-
+Once the server is running, you can access the API documentation via Swagger UI.
```

### Comparing `textembed-0.0.2/setup.py` & `textembed-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,16 +73,16 @@
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
-            "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
+            "Programming Language :: Python :: 3.12",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
         ],
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `textembed-0.0.2/src/textembed/api/docs.py` & `textembed-0.0.3/src/textembed/api/docs.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.2/src/textembed/api/embed.py` & `textembed-0.0.3/src/textembed/api/embed.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 from textembed.api.schemas import (
     EmbeddingData,
     EmbeddingRequest,
     EmbeddingResponse,
     ModelDetails,
     ModelList,
+    Usage,
 )
 from textembed.engine.args import AsyncEngineArgs
 from textembed.engine.async_engine import AsyncEngine
 from textembed.log import logger
 
 embed_router = APIRouter(prefix="/v1", tags=["Embedding"])
 
@@ -66,28 +67,34 @@
         embed_request.input = [embed_request.input]
 
     start_time = time.perf_counter()
 
     # Generate embeddings
     loop = asyncio.get_running_loop()
     future = loop.create_future()
-    await async_engine.aembed(sentences=embed_request.input, future=future)
-    embeddings = await future
+    await async_engine.aembed(sentences=embed_request.input, future=future)  # type: ignore
+    results = await future
 
     logger.info(
         "Received request with %d inputs. Processed in %.4f ms",
         len(embed_request.input),
         (time.perf_counter() - start_time) * 1000,
     )
 
+    embeddings = results[0]
+    usage = results[1]
     embedding_data = [
         EmbeddingData(
             object="embedding",
             embedding=emb,
             index=count,
+            usage=Usage(
+                prompt_tokens=usage[count],
+                total_tokens=usage[count],
+            ),
         )
         for count, emb in enumerate(embeddings)
     ]
 
     response = EmbeddingResponse(
         object="embedding",
         data=embedding_data,
```

### Comparing `textembed-0.0.2/src/textembed/api/monitor.py` & `textembed-0.0.3/src/textembed/api/monitor.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.2/src/textembed/api/schemas.py` & `textembed-0.0.3/src/textembed/api/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,25 +73,38 @@
     """
 
     input: List[str]
     model: Optional[str] = None
     user: Optional[str] = None
 
 
+class Usage(BaseModel):
+    """Sentence prompt and total tokens
+
+    Attributes:
+        prompt_tokens (str): Count of prompt tokens.
+        total_tokens (str): Count of total tokens.
+    """
+
+    prompt_tokens: int
+    total_tokens: int
+
+
 class EmbeddingData(BaseModel):
     """Embedding data containing the embedding vector and index.
 
     Attributes:
         object (Literal["embedding"]): Type of the object, default is "embedding".
         embedding (List[Union[float, int]]): Embedding vector.
         index (int): Index of the embedding in the input list.
     """
 
     object: Literal["embedding"] = "embedding"
     embedding: List[Union[float, int]]
+    usage: Usage
     index: int
 
 
 class EmbeddingResponse(BaseModel):
     """Response containing embedding data in OpenAI format.
 
     Attributes:
```

### Comparing `textembed-0.0.2/src/textembed/application/application.py` & `textembed-0.0.3/src/textembed/application/application.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.2/src/textembed/batch/batch_processor.py` & `textembed-0.0.3/src/textembed/batch/batch_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,20 +68,25 @@
             if requests:
                 all_texts = [
                     text for req in requests for text in req[0]
                 ]  # Flatten list of lists
                 futures = [req[1] for req in requests]
 
                 try:
-                    embeddings = await self.model.generate_embeddings(all_texts)
+                    embeddings, usage = await self.model.process_batch(all_texts)
                     # Split embeddings back to individual futures
                     idx = 0
                     for future, req in zip(futures, requests):
                         num_texts = len(req[0])
-                        future.set_result(embeddings[idx : idx + num_texts])
+                        future.set_result(
+                            (
+                                embeddings[idx : idx + num_texts],
+                                usage[idx : idx + num_texts],
+                            )
+                        )
                         idx += num_texts
                 except Exception as e:
                     for future in futures:
                         future.set_exception(e)
 
                 logger.debug(
                     "Worker %d processed batch in %.4f ms",
```

### Comparing `textembed-0.0.2/src/textembed/engine/args.py` & `textembed-0.0.3/src/textembed/engine/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,21 +13,23 @@
         model (str): The path or identifier of the model to be used by the engine.
         served_model_name (Optional[str]): An optional name to be used for serving the model.
                                            If not provided, it is derived from the last two segments of the model path.
         trust_remote_code (bool): Whether to trust remote code.
         workers (int): The number of worker tasks to process requests. Defaults to the number of CPU cores.
         batch_size (int): The maximum number of requests to process in a single batch.
                           Must be greater than or equal to 1.
+        embedding_dtype(str): Embedding data type for final generate embedding.
     """
 
     model: str
     served_model_name: Optional[str] = None
     trust_remote_code: bool = True
     workers: int = multiprocessing.cpu_count()
     batch_size: int = 32
+    embedding_dtype: str = "float32"
 
     def __post_init__(self):
         # If served_model_name is not provided, derive it from the model path
         if self.served_model_name is None:
             # Split the model path and take the last two segments to form the served_model_name
             segments = self.model.split("/")
             if len(segments) >= 2:
```

### Comparing `textembed-0.0.2/src/textembed/engine/async_engine.py` & `textembed-0.0.3/src/textembed/engine/async_engine.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.2/src/textembed/executor/embedder/sentence_transformer.py` & `textembed-0.0.3/src/textembed/executor/embedder/sentence_transformer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Sentence Transformers"""
 
-from typing import Any, Dict, List
+from typing import Dict, List, Tuple
 
 import numpy as np
 import torch
 from sentence_transformers import SentenceTransformer, util
 from torch import Tensor
 
 from textembed.engine.args import AsyncEngineArgs
 from textembed.executor.base import BaseEmbedder
+from textembed.executor.primitives import EmbeddingDtype
 
 
 class SentenceTransformerEmbedder(SentenceTransformer, BaseEmbedder):
     """Sentence Transformer Embedder for embedding creation.
 
     This class extends SentenceTransformer and implements the BaseEmbedder interface
     to provide a complete embedding creation workflow including preprocessing,
@@ -26,62 +27,85 @@
             engine_args (AsyncEngineArgs): The arguments required to configure the engine.
         """
         super().__init__(
             model_name_or_path=engine_args.model,
             device="cpu",
             trust_remote_code=engine_args.trust_remote_code,
         )
+        self.embedding_dtype = engine_args.embedding_dtype
         self.eval()
 
-    async def preprocess(self, sentences: List[str]) -> Any:
-        """Preprocesses input sentences for embedding.
+    async def preprocess(
+        self, sentences: List[str]
+    ) -> Tuple[Dict[str, Tensor], List[int]]:
+        """Tokenizes the input sentences.
 
         Args:
-            sentences (List[str]): List of sentences to be embedded.
+            sentences (List[str]): List of sentences to be tokenized.
 
         Returns:
-            Any: Tokenized features ready for core processing.
+            Tuple[Dict[str, Tensor], List[int]]: Tokenized features and lengths of sentences
         """
-        features = self.tokenize(sentences)
-        return features
-
-    async def core_process(self, features: Dict[str, Tensor]) -> Tensor:
-        """Runs the core embedding process on the input features.
+        tokenized = self.tokenize(sentences)
+        usage = [len(sentence) for sentence in sentences]
+        return tokenized, usage
+
+    async def transfer_to_device(
+        self, features: Dict[str, Tensor]
+    ) -> Dict[str, Tensor]:
+        """Moves the tokenized features to the appropriate device.
 
         Args:
             features (Dict[str, Tensor]): Tokenized features.
 
         Returns:
+            Dict[str, Tensor]: Features moved to the specified device.
+        """
+        return util.batch_to_device(features, self.device)
+
+    async def generate_embeddings(self, features: Dict[str, Tensor]) -> Tensor:
+        """Performs the forward pass to generate sentence embeddings.
+
+        Args:
+            features (Dict[str, Tensor]): Tokenized features moved to the device.
+
+        Returns:
             Tensor: Raw embeddings from the model.
         """
         with torch.inference_mode():
-            features = util.batch_to_device(features, self.device)
-            out_features = self.forward(features)["sentence_embedding"]
-        return out_features
+            return self.forward(features)["sentence_embedding"]
 
-    async def postprocess(self, out_features: Tensor) -> List[np.ndarray]:
-        """Postprocesses the raw embeddings to the final format.
+    async def postprocess(self, out_features: Tensor) -> np.ndarray:
+        """Converts the output tensors to numpy arrays of the specified data type.
 
         Args:
             out_features (Tensor): Raw embeddings from the model.
 
         Returns:
-            np.ndarray: Postprocessed embeddings in numpy array format.
+            np.ndarray: Postprocessed embeddings in the specified numpy array format.
         """
-        with torch.inference_mode():
-            embeddings = out_features.detach().cpu().numpy()
-        return embeddings
+        embeddings = out_features.detach().cpu().numpy()
+        if self.embedding_dtype == EmbeddingDtype.BINARY.value:
+            return (embeddings > 0).astype(np.uint8)
+        elif self.embedding_dtype == EmbeddingDtype.INT8.value:
+            return embeddings.astype(np.int8)
+        elif self.embedding_dtype == EmbeddingDtype.FLOAT16.value:
+            return embeddings.astype(np.float16)
+        elif self.embedding_dtype == EmbeddingDtype.FLOAT32.value:
+            return embeddings.astype(np.float32)
+        else:
+            raise ValueError(f"Unsupported dtype: {self.embedding_dtype}")
 
-    async def generate_embeddings(self, sentences: List[str]) -> List[np.ndarray]:
-        """Generates embeddings for the input sentences.
+    async def process_batch(self, sentences: List[str]) -> Tuple[np.ndarray, List[int]]:
+        """Processes a batch of sentences to generate embeddings.
 
         Args:
-            sentences (List[str]): Input sentences to generate embeddings for.
+            sentences (List[str]): List of sentences to be embedded.
 
         Returns:
-            List[np.ndarray]: Generated embeddings.
+            Tuple[np.ndarray, List[int]]: Generated embeddings and lengths of sentences.
         """
-        features = await self.preprocess(sentences)
-        out_features = await self.core_process(features)
+        features, lengths = await self.preprocess(sentences)
+        features = await self.transfer_to_device(features)
+        out_features = await self.generate_embeddings(features)
         embeddings = await self.postprocess(out_features)
-
-        return embeddings
+        return embeddings, lengths  # type: ignore
```

### Comparing `textembed-0.0.2/src/textembed/log.py` & `textembed-0.0.3/src/textembed/log.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.2/src/textembed/server.py` & `textembed-0.0.3/src/textembed/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import multiprocessing
 import warnings
 
 import typer
 import uvicorn
 from typing_extensions import Annotated
 
+from textembed.api.errors import EmbeddingException, embedding_exception_handler
 from textembed.application.application import create_application
 from textembed.engine.args import AsyncEngineArgs
 
 # Filter out all warnings
 warnings.filterwarnings("ignore")
 
 app_typer = typer.Typer()
@@ -42,37 +43,49 @@
         int,
         typer.Option(help="The number of worker processes."),
     ] = None,  # type: ignore
     batch_size: Annotated[
         int,
         typer.Option(help="The batch size for processing requests."),
     ] = 32,
+    embedding_dtype: Annotated[
+        str,
+        typer.Option(
+            help="The data type for the embeddings. Choose from 'binary', 'int8', 'float16', or 'float32'. Default is 'float32'."
+        ),
+    ] = "float32",
 ):
     """
     Starts the application with the specified configuration.
 
     Args:
         model (str): The name or path of the Huggingface model to be used.
         served_model_name (str): The name under which the model will be served.
         trust_remote_code (bool): Whether to trust remote code when loading the model.
         host (str): The host address on which the application will run.
         port (int): The port number on which the application will run.
         workers (int): The number of worker processes.
         batch_size (int): The batch size for processing requests.
+        embedding_dtype (str): The data type for the embeddings. Choose from 'binary', 'int8', 'float16', or 'float32
     """
     engine_args = AsyncEngineArgs(
         model=model,
         served_model_name=served_model_name or None,  # Set to None if empty string
         trust_remote_code=trust_remote_code,
         workers=workers if workers is not None else multiprocessing.cpu_count(),
         batch_size=batch_size,
+        embedding_dtype=embedding_dtype,
     )
 
     app = create_application(
         engine_args=engine_args,
         doc_extra={"host": host, "port": port},
     )
+
+    # Handle Errors
+    app.add_exception_handler(EmbeddingException, embedding_exception_handler)  # type: ignore
+
     uvicorn.run(app, host=host, port=port, log_level="error")
 
 
 if __name__ == "__main__":
     app_typer()
```

### Comparing `textembed-0.0.2/src/textembed.egg-info/PKG-INFO` & `textembed-0.0.3/src/textembed.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.2
+Version: 0.0.3
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.11.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
@@ -85,42 +85,30 @@
 TextEmbed is a high-throughput, low-latency REST API designed for serving vector embeddings. It supports a wide range of sentence-transformer models and frameworks, making it suitable for various applications in natural language processing.
 
 ## Features
 
 - **High Throughput & Low Latency:** Designed to handle a large number of requests efficiently.
 - **Flexible Model Support:** Works with various sentence-transformer models.
 - **Scalable:** Easily integrates into larger systems and scales with demand.
-- **REST API:** Simple and accessible API endpoints.
+- **Batch Processing:** Supports batch processing for better and faster inference.
+- **OpenAI Compatible REST API Endpoint:** Provides an OpenAI compatible REST API endpoint.
 
 ## Getting Started
 
 ### Prerequisites
 
-Ensure you have Python 3.10 or higher installed. You will also need to install the required dependencies.
+Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
-1. Clone the repository:
-    ```bash
-    git clone https://github.com/kevaldekivadiya2415/textembed.git
-    cd textembed
-    ```
-
-2. Install the dependencies:
+1. Install the required dependencies:
     ```bash
     pip install -r requirements.txt
     ```
 
-### Running the Server
-
-1. Set up the package in development mode:
-    ```bash
-    python3 setup.py develop
-    ```
-
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
 
     Replace `<Model Name>` with the name of the model you want to use.
 
@@ -128,20 +116,19 @@
     ```bash
     python3 -m textembed.server --help
     ```
 
 ### Running with Docker (Recommended)
 You can also run TextEmbed using Docker. The Docker image is available on Docker Hub.
 ```bash
-docker run keval2415/textembed:0.0.1 --help
+docker run kevaldekivadiya/textembed:latest --help
 ```
 This command will show the help message for the TextEmbed server, detailing the available options and usage.
 
 For Example:
 ```bash
-docker run -p 8000:8000 keval2415/textembed:0.0.1 --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
+docker run -p 8000:8000 kevaldekivadiya/textembed:latest --model sentence-transformers/all-MiniLM-L6-v2 --port 8000
 ```
 
 ### Accessing the API
 
 Once the server is running, you can access the API documentation via Swagger UI.
-
```

### Comparing `textembed-0.0.2/src/textembed.egg-info/SOURCES.txt` & `textembed-0.0.3/src/textembed.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 src/textembed/__init__.py
 src/textembed/log.py
 src/textembed/server.py
 src/textembed.egg-info/PKG-INFO
 src/textembed.egg-info/SOURCES.txt
 src/textembed.egg-info/dependency_links.txt
 src/textembed.egg-info/requires.txt
 src/textembed.egg-info/top_level.txt
 src/textembed/api/__init__.py
 src/textembed/api/docs.py
 src/textembed/api/embed.py
+src/textembed/api/errors.py
 src/textembed/api/monitor.py
 src/textembed/api/schemas.py
 src/textembed/application/__init__.py
 src/textembed/application/application.py
 src/textembed/batch/__init__.py
 src/textembed/batch/batch_processor.py
 src/textembed/cache/__init__.py
```

### Comparing `textembed-0.0.2/src/textembed.egg-info/requires.txt` & `textembed-0.0.3/requirements.txt`

 * *Files identical despite different names*

