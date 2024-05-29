# Comparing `tmp/logistic_regression_module_universal_bank-0.0.2.tar.gz` & `tmp/logistic_regression_module_universal_bank-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logistic_regression_module_universal_bank-0.0.2.tar", last modified: Wed May 29 02:37:15 2024, max compression
+gzip compressed data, was "logistic_regression_module_universal_bank-0.0.3.tar", last modified: Wed May 29 02:41:26 2024, max compression
```

## Comparing `logistic_regression_module_universal_bank-0.0.2.tar` & `logistic_regression_module_universal_bank-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:37:15.152592 logistic_regression_module_universal_bank-0.0.2/
--rw-r--r--   0 taemin     (501) staff       (20)       23 2024-05-29 02:33:32.000000 logistic_regression_module_universal_bank-0.0.2/MANIFEST.in
--rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:37:15.152331 logistic_regression_module_universal_bank-0.0.2/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)        0 2024-05-29 01:57:52.000000 logistic_regression_module_universal_bank-0.0.2/README.md
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:37:15.150329 logistic_regression_module_universal_bank-0.0.2/lib/
--rw-r--r--   0 taemin     (501) staff       (20)       22 2024-05-29 02:37:06.000000 logistic_regression_module_universal_bank-0.0.2/lib/__init__.py
--rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module.py
-drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:37:15.151931 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/
--rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:37:15.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/PKG-INFO
--rw-r--r--   0 taemin     (501) staff       (20)      424 2024-05-29 02:37:15.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/SOURCES.txt
--rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 02:37:15.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/dependency_links.txt
--rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 02:37:15.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/requires.txt
--rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 02:37:15.000000 logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module_universal_bank.egg-info/top_level.txt
--rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 02:37:15.152708 logistic_regression_module_universal_bank-0.0.2/setup.cfg
--rw-r--r--   0 taemin     (501) staff       (20)     1235 2024-05-29 02:37:03.000000 logistic_regression_module_universal_bank-0.0.2/setup.py
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.266750 logistic_regression_module_universal_bank-0.0.3/
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.263882 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/
+-rw-r--r--   0 taemin     (501) staff       (20)       65 2024-05-29 02:40:41.000000 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/__init__.py
+-rw-r--r--   0 taemin     (501) staff       (20)     3115 2024-05-29 02:09:28.000000 logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/logistic_regression_module.py
+-rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:41:26.266488 logistic_regression_module_universal_bank-0.0.3/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)        0 2024-05-29 01:57:52.000000 logistic_regression_module_universal_bank-0.0.3/README.md
+drwxr-xr-x   0 taemin     (501) staff       (20)        0 2024-05-29 02:41:26.266056 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/
+-rw-r--r--   0 taemin     (501) staff       (20)      301 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/PKG-INFO
+-rw-r--r--   0 taemin     (501) staff       (20)      470 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/SOURCES.txt
+-rw-r--r--   0 taemin     (501) staff       (20)        1 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/dependency_links.txt
+-rw-r--r--   0 taemin     (501) staff       (20)      124 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/requires.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       43 2024-05-29 02:41:26.000000 logistic_regression_module_universal_bank-0.0.3/logistic_regression_module_universal_bank.egg-info/top_level.txt
+-rw-r--r--   0 taemin     (501) staff       (20)       38 2024-05-29 02:41:26.266864 logistic_regression_module_universal_bank-0.0.3/setup.cfg
+-rw-r--r--   0 taemin     (501) staff       (20)     1162 2024-05-29 02:41:02.000000 logistic_regression_module_universal_bank-0.0.3/setup.py
```

### Comparing `logistic_regression_module_universal_bank-0.0.2/lib/logistic_regression_module.py` & `logistic_regression_module_universal_bank-0.0.3/ logistic-regression-module-universal-bank/logistic_regression_module.py`

 * *Files identical despite different names*

### Comparing `logistic_regression_module_universal_bank-0.0.2/setup.py` & `logistic_regression_module_universal_bank-0.0.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logistic_regression_module_universal_bank", # 모듈 이름
-    version="0.0.2", # 버전
+    version="0.0.3", # 버전
     author="TaeMin", # 제작자
     author_email="taeminida@gmail.com", # contact
     description="로지스틱회귀 예제 1", # 모듈 설명
     long_description=open('README.md').read(), # README.md에 보통 모듈 설명을 해놓는다.
     long_description_content_type="text/markdown",
     install_requires=[ # 필수 라이브러리들을 포함하는 부분인 것 같음, 다른 방식으로 넣어줄 수 있는지는 알 수 없음
     "matplotlib==3.9.0", 
@@ -19,11 +19,10 @@
     "statsmodels==0.14.2", 
     "mord==0.7", 
     "seaborn==0.13.2", 
     "dmba==0.2.4", 
     ],
     package_data={'': ['LICENSE.txt', 'requirements.txt']}, # 원하는 파일 포함, 제대로 작동되지 않았음
     include_package_data=True,
+    packages = setuptools.find_packages(), # 모듈을 자동으로 찾아줌
     python_requires=">=3.9.13", # 파이썬 최소 요구 버전
-    packages=setuptools.find_packages(where="lib"),  # lib 디렉토리에서 패키지 찾기
-    package_dir={"": "lib"},  # lib 디렉토리 설정
 )
```

