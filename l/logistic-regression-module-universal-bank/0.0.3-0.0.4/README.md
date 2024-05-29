# Comparing `tmp/logistic_regression_module_universal_bank-0.0.3.tar.gz` & `tmp/logistic_regression_module_universal_bank-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logistic_regression_module_universal_bank-0.0.3.tar", last modified: Wed May 29 02:41:26 2024, max compression
+gzip compressed data, was "logistic_regression_module_universal_bank-0.0.4.tar", last modified: Wed May 29 06:46:49 2024, max compression
```

## Comparing `logistic_regression_module_universal_bank-0.0.3.tar` & `logistic_regression_module_universal_bank-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.266750 logistic_regression_module_universal_bank-0.0.3/
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.263882 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/
--rw-r--r--   0 taemin     (501) staff       (20)       65 2024-05-29 02:40:41.000000 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/__init__.py
--rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/logistic_regression_module.py
--rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:41:26.266488 logistic_regression_module_universal_bank-0.0.3/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)        0 2024-05-29 01:57:52.000000 logistic_regression_module_universal_bank-0.0.3/README.md
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.266056 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/
--rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)      470 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/SOURCES.txt
--rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/dependency_links.txt
--rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/requires.txt
--rw-r--r--   0 taemin     (501) staff       (20)       43 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/top_level.txt
--rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 02:41:26.266864 logistic_regression_module_universal_bank-0.0.3/setup.cfg
--rw-r--r--   0 taemin     (501) staff       (20)     1162 2024-05-29 02:41:02.000000 logistic_regression_module_universal_bank-0.0.3/setup.py
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 06:46:49.202466 logistic_regression_module_universal_bank-0.0.4/
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 06:46:49.199563 logistic_regression_module_universal_bank-0.0.4/ logistic-regression-module-universal-bank/
+-rw-r--r--   0 taemin     (501) staff       (20)      186 2024-05-29 06:46:31.000000 logistic_regression_module_universal_bank-0.0.4/ logistic-regression-module-universal-bank/__init__.py
+-rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logistic_regression_module_universal_bank-0.0.4/ logistic-regression-module-universal-bank/logistic_regression_module.py
+-rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 06:46:49.202162 logistic_regression_module_universal_bank-0.0.4/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)        0 2024-05-29 01:57:52.000000 logistic_regression_module_universal_bank-0.0.4/README.md
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 06:46:49.201661 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/
+-rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 06:46:49.000000 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)      470 2024-05-29 06:46:49.000000 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/SOURCES.txt
+-rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 06:46:49.000000 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/dependency_links.txt
+-rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 06:46:49.000000 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/requires.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       43 2024-05-29 06:46:49.000000 logistic_regression_module_universal_bank-0.0.4/logistic_regression_module_universal_bank.egg-info/top_level.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 06:46:49.202605 logistic_regression_module_universal_bank-0.0.4/setup.cfg
+-rw-r--r--   0 taemin     (501) staff       (20)     1162 2024-05-29 06:46:47.000000 logistic_regression_module_universal_bank-0.0.4/setup.py
```

### Comparing `logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/logistic_regression_module.py` & `logistic_regression_module_universal_bank-0.0.4/ logistic-regression-module-universal-bank/logistic_regression_module.py`

 * *Files identical despite different names*

### Comparing `logistic_regression_module_universal_bank-0.0.3/setup.py` & `logistic_regression_module_universal_bank-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logistic_regression_module_universal_bank", # 모듈 이름
-    version="0.0.3", # 버전
+    version="0.0.4", # 버전
     author="TaeMin", # 제작자
     author_email="taeminida@gmail.com", # contact
     description="로지스틱회귀 예제 1", # 모듈 설명
     long_description=open('README.md').read(), # README.md에 보통 모듈 설명을 해놓는다.
     long_description_content_type="text/markdown",
     install_requires=[ # 필수 라이브러리들을 포함하는 부분인 것 같음, 다른 방식으로 넣어줄 수 있는지는 알 수 없음
     "matplotlib==3.9.0",
```

