# Comparing `tmp/logisticbank-0.0.1.tar.gz` & `tmp/logisticbank-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logisticbank-0.0.1.tar", last modified: Wed May 29 08:03:16 2024, max compression
+gzip compressed data, was "logisticbank-0.0.2.tar", last modified: Wed May 29 08:25:31 2024, max compression
```

## Comparing `logisticbank-0.0.1.tar` & `logisticbank-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:03:16.029395 logisticbank-0.0.1/
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:03:16.026392 logisticbank-0.0.1/ logisticbank/
--rw-r--r--   0 taemin     (501) staff       (20)      385 2024-05-29 08:01:54.000000 logisticbank-0.0.1/ logisticbank/__init__.py
--rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logisticbank-0.0.1/ logisticbank/logistic_regression_module.py
--rw-r--r--   0 taemin     (501) staff       (20)      284 2024-05-29 08:03:16.029121 logisticbank-0.0.1/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)       19 2024-05-29 07:20:15.000000 logisticbank-0.0.1/README.md
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:03:16.028679 logisticbank-0.0.1/logisticbank.egg-info/
--rw-r--r--   0 taemin     (501) staff       (20)      284 2024-05-29 08:03:15.000000 logisticbank-0.0.1/logisticbank.egg-info/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)      267 2024-05-29 08:03:15.000000 logisticbank-0.0.1/logisticbank.egg-info/SOURCES.txt
--rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 08:03:15.000000 logisticbank-0.0.1/logisticbank.egg-info/dependency_links.txt
--rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 08:03:15.000000 logisticbank-0.0.1/logisticbank.egg-info/requires.txt
--rw-r--r--   0 taemin     (501) staff       (20)       14 2024-05-29 08:03:15.000000 logisticbank-0.0.1/logisticbank.egg-info/top_level.txt
--rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 08:03:16.029513 logisticbank-0.0.1/setup.cfg
--rw-r--r--   0 taemin     (501) staff       (20)     1096 2024-05-29 08:02:55.000000 logisticbank-0.0.1/setup.py
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:25:31.712302 logisticbank-0.0.2/
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:25:31.709157 logisticbank-0.0.2/ logisticbank/
+-rw-r--r--   0 taemin     (501) staff       (20)     3278 2024-05-29 08:25:28.000000 logisticbank-0.0.2/ logisticbank/__init__.py
+-rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logisticbank-0.0.2/ logisticbank/logistic_regression_module.py
+-rw-r--r--   0 taemin     (501) staff       (20)      284 2024-05-29 08:25:31.711918 logisticbank-0.0.2/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)       19 2024-05-29 07:20:15.000000 logisticbank-0.0.2/README.md
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 08:25:31.711429 logisticbank-0.0.2/logisticbank.egg-info/
+-rw-r--r--   0 taemin     (501) staff       (20)      284 2024-05-29 08:25:31.000000 logisticbank-0.0.2/logisticbank.egg-info/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)      267 2024-05-29 08:25:31.000000 logisticbank-0.0.2/logisticbank.egg-info/SOURCES.txt
+-rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 08:25:31.000000 logisticbank-0.0.2/logisticbank.egg-info/dependency_links.txt
+-rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 08:25:31.000000 logisticbank-0.0.2/logisticbank.egg-info/requires.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       14 2024-05-29 08:25:31.000000 logisticbank-0.0.2/logisticbank.egg-info/top_level.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 08:25:31.712452 logisticbank-0.0.2/setup.cfg
+-rw-r--r--   0 taemin     (501) staff       (20)     1096 2024-05-29 08:25:26.000000 logisticbank-0.0.2/setup.py
```

### Comparing `logisticbank-0.0.1/ logisticbank/logistic_regression_module.py` & `logisticbank-0.0.2/ logisticbank/logistic_regression_module.py`

 * *Files identical despite different names*

### Comparing `logisticbank-0.0.1/setup.py` & `logisticbank-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logisticbank", # 모듈 이름
-    version="0.0.1", # 버전
+    version="0.0.2", # 버전
     author="TaeMin", # 제작자
     author_email="taeminida@gmail.com", # contact
     description="로지스틱회귀 예제 1", # 모듈 설명
     long_description=open('README.md').read(), # README.md에 보통 모듈 설명을 해놓는다.
     long_description_content_type="text/markdown",
     install_requires=[ # 필수 라이브러리들을 포함하는 부분인 것 같음, 다른 방식으로 넣어줄 수 있는지는 알 수 없음
     "matplotlib==3.9.0",
```

