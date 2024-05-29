# Comparing `tmp/gmalglib-0.5.8.tar.gz` & `tmp/gmalglib-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.8.tar", last modified: Wed May 29 10:04:05 2024, max compression
+gzip compressed data, was "gmalglib-0.5.9.tar", last modified: Wed May 29 15:39:37 2024, max compression
```

## Comparing `gmalglib-0.5.8.tar` & `gmalglib-0.5.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.947129 gmalglib-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 10:04:01.000000 gmalglib-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 10:04:05.947129 gmalglib-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-29 10:04:01.000000 gmalglib-0.5.8/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-29 10:04:01.000000 gmalglib-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.935129 gmalglib-0.5.8/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.939128 gmalglib-0.5.8/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/sm2table.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 10:04:01.000000 gmalglib-0.5.8/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 10:04:01.000000 gmalglib-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:04:05.947129 gmalglib-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 10:04:01.000000 gmalglib-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.935129 gmalglib-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.939128 gmalglib-0.5.8/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.947129 gmalglib-0.5.8/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)  2810569 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/sm2table.c
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 10:04:01.000000 gmalglib-0.5.8/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:04:05.947129 gmalglib-0.5.8/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 10:04:05.000000 gmalglib-0.5.8/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 10:04:05.000000 gmalglib-0.5.8/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:04:05.000000 gmalglib-0.5.8/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 10:04:05.000000 gmalglib-0.5.8/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.197567 gmalglib-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 15:39:29.000000 gmalglib-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-29 15:39:37.197567 gmalglib-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-29 15:39:29.000000 gmalglib-0.5.9/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-05-29 15:39:29.000000 gmalglib-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.189567 gmalglib-0.5.9/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.189567 gmalglib-0.5.9/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/sm2table.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 15:39:29.000000 gmalglib-0.5.9/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 15:39:29.000000 gmalglib-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:39:37.197567 gmalglib-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 15:39:29.000000 gmalglib-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.189567 gmalglib-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.193567 gmalglib-0.5.9/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.197567 gmalglib-0.5.9/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21838 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)  2810569 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/sm2table.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 15:39:29.000000 gmalglib-0.5.9/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:39:37.197567 gmalglib-0.5.9/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-29 15:39:37.000000 gmalglib-0.5.9/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 15:39:37.000000 gmalglib-0.5.9/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:39:37.000000 gmalglib-0.5.9/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 15:39:37.000000 gmalglib-0.5.9/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.8/LICENSE` & `gmalglib-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/PKG-INFO` & `gmalglib-0.5.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -76,23 +76,23 @@
 
 ## Benchmark Test
 
 The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 2.391558s
-SM2.decrypt             : 1.092445s
-SM2.sign_digest         : 1.062552s
-SM2.verify_digest       : 2.096187s
-SM2.sign                : 1.067850s
-SM2.verify              : 2.055190s
-SM2.begin_key_exchange  : 1.159822s
-SM2.end_key_exchange    : 1.633471s
+SM2.encrypt             : 0.454363s (2200.88 times/s)
+SM2.decrypt             : 0.356014s (2808.88 times/s)
+SM2.sign_digest         : 0.088565s (11291.12 times/s)
+SM2.verify_digest       : 0.409243s (2443.54 times/s)
+SM2.sign                : 0.087475s (11431.80 times/s)
+SM2.verify              : 0.404026s (2475.09 times/s)
+SM2.begin_key_exchange  : 0.086665s (11538.62 times/s)
+SM2.end_key_exchange    : 0.536552s (1863.75 times/s)
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 5.118763s
+SM3.update & SM3.digest : 3.083487s (324,308,109 B/s)
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.369991s
-SM4.decrypt             : 0.297077s
+SM4.encrypt             : 0.197393s (5066040.91 times/s)
+SM4.decrypt             : 0.185619s (5387391.13 times/s)
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.050301s
+zuc.generate            : 0.028821s (34696561.22 times/s)
 ```
```

### Comparing `gmalglib-0.5.8/README.en.md` & `gmalglib-0.5.9/README.en.md`

 * *Files 21% similar despite different names*

```diff
@@ -59,23 +59,23 @@
 
 ## Benchmark Test
 
 The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 2.391558s
-SM2.decrypt             : 1.092445s
-SM2.sign_digest         : 1.062552s
-SM2.verify_digest       : 2.096187s
-SM2.sign                : 1.067850s
-SM2.verify              : 2.055190s
-SM2.begin_key_exchange  : 1.159822s
-SM2.end_key_exchange    : 1.633471s
+SM2.encrypt             : 0.454363s (2200.88 times/s)
+SM2.decrypt             : 0.356014s (2808.88 times/s)
+SM2.sign_digest         : 0.088565s (11291.12 times/s)
+SM2.verify_digest       : 0.409243s (2443.54 times/s)
+SM2.sign                : 0.087475s (11431.80 times/s)
+SM2.verify              : 0.404026s (2475.09 times/s)
+SM2.begin_key_exchange  : 0.086665s (11538.62 times/s)
+SM2.end_key_exchange    : 0.536552s (1863.75 times/s)
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 5.118763s
+SM3.update & SM3.digest : 3.083487s (324,308,109 B/s)
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.369991s
-SM4.decrypt             : 0.297077s
+SM4.encrypt             : 0.197393s (5066040.91 times/s)
+SM4.decrypt             : 0.185619s (5387391.13 times/s)
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.050301s
+zuc.generate            : 0.028821s (34696561.22 times/s)
 ```
```

### Comparing `gmalglib-0.5.8/README.md` & `gmalglib-0.5.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -62,23 +62,23 @@
 
 ## 性能测试
 
 性能测试代码见 [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py), `13th Gen Intel(R) Core(TM) i7-13700H` 上测试结果如下:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 0.453286s (2206.12 times/s)
-SM2.decrypt             : 0.353108s (2831.99 times/s)
-SM2.sign_digest         : 0.086778s (11523.62 times/s)
-SM2.verify_digest       : 0.407510s (2453.92 times/s)
-SM2.sign                : 0.088102s (11350.42 times/s)
-SM2.verify              : 0.415350s (2407.61 times/s)
-SM2.begin_key_exchange  : 0.119090s (8396.99 times/s)
-SM2.end_key_exchange    : 0.535585s (1867.12 times/s)
+SM2.encrypt             : 0.454363s (2200.88 times/s)
+SM2.decrypt             : 0.356014s (2808.88 times/s)
+SM2.sign_digest         : 0.088565s (11291.12 times/s)
+SM2.verify_digest       : 0.409243s (2443.54 times/s)
+SM2.sign                : 0.087475s (11431.80 times/s)
+SM2.verify              : 0.404026s (2475.09 times/s)
+SM2.begin_key_exchange  : 0.086665s (11538.62 times/s)
+SM2.end_key_exchange    : 0.536552s (1863.75 times/s)
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 3.061764s (326,609,116 B/s)
+SM3.update & SM3.digest : 3.083487s (324,308,109 B/s)
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.188778s (5297230.24 times/s)
-SM4.decrypt             : 0.186436s (5363756.56 times/s)
+SM4.encrypt             : 0.197393s (5066040.91 times/s)
+SM4.decrypt             : 0.185619s (5387391.13 times/s)
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.037984s (26326735.85 times/s)
+zuc.generate            : 0.028821s (34696561.22 times/s)
 ```
```

### Comparing `gmalglib-0.5.8/include/gmalglib/bignum.h` & `gmalglib-0.5.9/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/include/gmalglib/random.h` & `gmalglib-0.5.9/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/include/gmalglib/sm2.h` & `gmalglib-0.5.9/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/include/gmalglib/sm2curve.h` & `gmalglib-0.5.9/include/gmalglib/sm2curve.h`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 extern const UInt256* const SM2_PARAMS_B;
 extern const SM2Point* const SM2_PARAMS_G;
 extern const UInt256* const SM2_PARAMS_N;
 
 void SM2JacobPointMont_ToPoint(const SM2JacobPointMont* X, SM2Point* Y);
 void SM2JacobPointMont_FromPoint(const SM2Point* X, SM2JacobPointMont* Y);
 
+int SM2Point_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2Point* X);
+uint64_t SM2Point_ToBytes(const SM2Point* X, int pc_mode, uint8_t* bytes);
 uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes);
 int SM2JacobPointMont_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2JacobPointMont* X);
 
 int SM2JacobPointMont_IsInf(const SM2JacobPointMont* X);
 void SM2JacobPointMont_SetInf(SM2JacobPointMont* X);
 int SM2JacobPointMont_IsOnCurve(const SM2JacobPointMont* X);
 int SM2JacobPointMont_IsEqual(const SM2JacobPointMont* X, const SM2JacobPointMont* Y);
```

### Comparing `gmalglib-0.5.8/include/gmalglib/sm3.h` & `gmalglib-0.5.9/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/pyproject.toml` & `gmalglib-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/setup.py` & `gmalglib-0.5.9/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/bignum.c` & `gmalglib-0.5.9/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/random.c` & `gmalglib-0.5.9/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/sm2.c` & `gmalglib-0.5.9/src/gmalglib/core/sm2.c`

 * *Files 1% similar despite different names*

```diff
@@ -700,87 +700,90 @@
 
 cleanup:
     free(plain_buffer);
     return err;
 }
 
 static
-int _SM2_BeginKeyExchange(SM2* self, SM2JacobPointMont* random_pt, SM2ModN* t)
+int _SM2_BeginKeyExchange(SM2* self, SM2Point* random_pt, SM2ModN* t)
 {
     SM2ModNMont r = { 0 };
-    SM2Point R = { 0 };
+    SM2JacobPointMont R = { 0 };
+    SM2ModN x_bar = { 0 };
 
     if (!RandomUInt256(&self->rand_alg, CONSTS_N_MINUS_ONE, &r))
         return SM2_ERR_RANDOM_FAILED;
 
-    SM2JacobPointMont_MulG(&r, random_pt);
+    SM2JacobPointMont_MulG(&r, &R);
+    SM2JacobPointMont_ToPoint(&R, random_pt);
 
     // w        =   ceil(ceil(log2(N)) / 2) - 1         = 127
     // 2^w      =   0x80000000000000000000000000000000
     // 2^w - 1  =   0x7fffffffffffffffffffffffffffffff
     // x_bar    =   2^w + (x & (2^w - 1))
-    SM2JacobPointMont_ToPoint(random_pt, &R);
-    R.x.u64[3] = 0;
-    R.x.u64[2] = 0;
-    R.x.u64[1] |= 0x8000000000000000;
+    x_bar = random_pt->x;
+    x_bar.u64[3] = 0;
+    x_bar.u64[2] = 0;
+    x_bar.u64[1] |= 0x8000000000000000;
 
-    SM2ModN_ToMont(&R.x, &R.x);
+    SM2ModN_ToMont(&x_bar, &x_bar);
     SM2ModN_ToMont(&r, &r);
 
-    SM2ModN_MontMul(&R.x, &r, t);
+    SM2ModN_MontMul(&x_bar, &r, t);
     SM2ModN_FromMont(t, t);
     SM2ModN_Add(&self->sk, t, t);
 
     return 0;
 }
 
 int SM2_BeginKeyExchange(SM2* self, SM2ModN* t, uint8_t* random_pt)
 {
     int ret = 0;
-    SM2JacobPointMont R = { 0 };
+    SM2Point R = { 0 };
 
     if (!self->has_sk)
         return SM2_ERR_NEED_SK;
 
     ret = _SM2_BeginKeyExchange(self, &R, t);
     if (ret != 0)
         return ret;
 
-    SM2JacobPointMont_ToBytes(&R, self->pc_mode, random_pt);
+    SM2Point_ToBytes(&R, self->pc_mode, random_pt);
     return 0;
 }
 
 static
-int _SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const SM2JacobPointMont* random_pt, const SM2JacobPointMont* pk, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key)
+int _SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const SM2Point* random_pt, const SM2JacobPointMont* pk, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key)
 {
     SM2JacobPointMont S = { 0 };
-    SM2Point R = { 0 };
+    SM2Point tmp = { 0 };
     SM3 sm3 = { 0 };
     uint8_t buffer[32] = { 0 };
+    SM2ModN x_bar = random_pt->x;
 
     // x_bar
-    SM2JacobPointMont_ToPoint(random_pt, &R);
-    R.x.u64[3] = 0;
-    R.x.u64[2] = 0;
-    R.x.u64[1] |= 0x8000000000000000;
+    x_bar.u64[3] = 0;
+    x_bar.u64[2] = 0;
+    x_bar.u64[1] |= 0x8000000000000000;
 
-    SM2JacobPointMont_Mul(&R.x, random_pt, &S);
+    SM2JacobPointMont_FromPoint(random_pt, &S);
+    SM2JacobPointMont_Mul(&x_bar, &S, &S);
     SM2JacobPointMont_Add(pk, &S, &S);
     SM2JacobPointMont_Mul(t, &S, &S);
 
     if (SM2JacobPointMont_IsInf(&S))
         return SM2_ERR_INVALID_SPOINT;
 
-    SM2JacobPointMont_ToPoint(&S, &R);
+    SM2JacobPointMont_ToPoint(&S, &tmp);
 
     SM3_Init(&sm3);
 
-    UInt256_ToBytes(&R.x, buffer);
+    UInt256_ToBytes(&tmp.x, buffer);
     SM3_Update(&sm3, buffer, 32);
-    UInt256_ToBytes(&R.y, buffer);
+    UInt256_ToBytes(&tmp.y, buffer);
     SM3_Update(&sm3, buffer, 32);
 
     _SM2_GetEntityInfo(pk, uid, uid_len, buffer);
 
     if (is_responder)
     {
         SM3_Update(&sm3, buffer, 32);
@@ -796,25 +799,25 @@
         return SM2_ERR_KEY_OVERFLOW;
 
     return 0;
 }
 
 int SM2_EndKeyExchange(SM2* self, const SM2ModN* t, const uint8_t* random_pt, uint64_t random_pt_len, const uint8_t* pk, uint64_t pk_len, const uint8_t* uid, uint64_t uid_len, int is_responder, uint64_t klen, uint8_t* key)
 {
-    SM2JacobPointMont R = { 0 };
+    SM2Point R = { 0 };
     SM2JacobPointMont P = { 0 };
     int ret = 0;
 
     if (!self->has_pk)
         return SM2_ERR_NEED_PK;
 
     if (UInt256_IsZero(t) || UInt256_Cmp(t, CONSTS_N_MINUS_ONE) > 0)
         return SM2_ERR_INVALID_T;
 
-    if (SM2JacobPointMont_FromBytes(random_pt, random_pt_len, &R) != 0)
+    if (SM2Point_FromBytes(random_pt, random_pt_len, &R) != 0)
         return SM2_ERR_INVALID_R;
 
     if (SM2JacobPointMont_FromBytes(pk, pk_len, &P) != 0)
         return SM2_ERR_INVALID_PK;
 
     if (uid == NULL)
     {
```

### Comparing `gmalglib-0.5.8/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.9/src/gmalglib/core/sm2curve.c`

 * *Files 2% similar despite different names*

```diff
@@ -133,14 +133,23 @@
 {
     if (UInt256_Sub(x, y, z))
     {
         UInt256_Sub(z, CONSTS_NEG_P, z);
     }
 }
 
+static
+void SM2ModP_Neg(const SM2ModP* x, SM2ModP* y)
+{
+    if (UInt256_Sub(CONSTS_P, x, y))
+    {
+        UInt256_Sub(y, CONSTS_NEG_P, y);
+    }
+}
+
 static 
 void SM2ModP_MontMul(const SM2ModPMont* x, const SM2ModPMont* y, SM2ModPMont* z)
 {
     UInt512 _xy = { 0 };
     UInt512* xy = &_xy;
     UInt512 _z_tmp = { 0 };
     UInt512* z_tmp = &_z_tmp;
@@ -255,18 +264,15 @@
     *y = y_tmp;
     return ret;
 }
 
 static 
 void SM2ModP_MontNeg(const SM2ModPMont* x, SM2ModPMont* y)
 {
-    if (UInt256_Sub(CONSTS_P, x, y))
-    {
-        UInt256_Sub(y, CONSTS_NEG_P, y);
-    }
+    SM2ModP_Neg(x, y);
 }
 
 static 
 void SM2ModP_MontInv(const SM2ModPMont* x, SM2ModPMont* y)
 {
     SM2ModP_MontPow(x, CONSTS_P_MINUS_TWO, y);
 }
@@ -399,115 +405,156 @@
     {
         SM2ModP_ToMont(&X->x, &Y->x);
         SM2ModP_ToMont(&X->y, &Y->y);
         Y->z = *CONSTS_MODP_MONT_ONE;
     }
 }
 
-uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes)
+static
+int SM2Point_IsOnCurve(const SM2Point* X)
 {
-    SM2Point pt = { 0 };
-    SM2JacobPointMont_ToPoint(X, &pt);
+    SM2ModPMont left = { 0 };
+    SM2ModPMont right = { 0 };
+    SM2ModPMont x = { 0 };
+    SM2ModPMont y = { 0 };
+
+    if (X->is_inf)
+        return 1;
+
+    SM2ModP_ToMont(&X->x, &x);
+    SM2ModP_ToMont(&X->y, &y);
+
+    // left = y^2 + 3x
+    SM2ModP_MontMul(&y, &y, &left);
+    SM2ModP_MontAdd(&left, &x, &left);
+    SM2ModP_MontAdd(&left, &x, &left);
+    SM2ModP_MontAdd(&left, &x, &left);
+
+    // right = x^3 + b
+    SM2ModP_MontMul(&x, &x, &right);
+    SM2ModP_MontMul(&right, &x, &right);
+    SM2ModP_MontAdd(&right, CONSTS_MODP_MONT_B, &right);
 
-    if (pt.is_inf)
+    return UInt256_Cmp(&left, &right) == 0;
+}
+
+uint64_t SM2Point_ToBytes(const SM2Point* X, int pc_mode, uint8_t* bytes)
+{
+    if (X->is_inf)
     {
         bytes[0] = 0x00;
         return 1;
     }
 
     if (pc_mode == SM2_PCMODE_COMPRESS)
     {
-        if (pt.y.u8[0] & 0x1)
+        if (X->y.u8[0] & 0x1)
             bytes[0] = 0x03;
         else
             bytes[0] = 0x02;
-        UInt256_ToBytes(&pt.x, bytes + 1);
+        UInt256_ToBytes(&X->x, bytes + 1);
         return 33;
     }
     else if (pc_mode == SM2_PCMODE_MIX)
     {
-        if (pt.y.u8[0] & 0x1)
+        if (X->y.u8[0] & 0x1)
             bytes[0] = 0x07;
         else
             bytes[0] = 0x06;
-        UInt256_ToBytes(&pt.x, bytes + 1);
-        UInt256_ToBytes(&pt.y, bytes + 33);
+        UInt256_ToBytes(&X->x, bytes + 1);
+        UInt256_ToBytes(&X->y, bytes + 33);
         return 65;
     }
     else
     {
         bytes[0] = 0x04;
-        UInt256_ToBytes(&pt.x, bytes + 1);
-        UInt256_ToBytes(&pt.y, bytes + 33);
+        UInt256_ToBytes(&X->x, bytes + 1);
+        UInt256_ToBytes(&X->y, bytes + 33);
         return 65;
     }
 
     return 0;
 }
 
-int SM2JacobPointMont_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2JacobPointMont* X)
+int SM2Point_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2Point* X)
 {
-    SM2Point pt = { 0 };
     uint8_t pc = bytes[0];
     int ylsb = 0;
 
     if (pc == 0x00)
     {
         if (bytes_len != 1)
             return SM2CURVE_ERR_INVALIDPC;
 
-        SM2JacobPointMont_SetInf(X);
+        X->is_inf = 1;
     }
     else if (pc == 0x04 || pc == 0x06 || pc == 0x07)
     {
         if (bytes_len != SM2_POINTBYTES_FULL_LENGTH)
             return SM2CURVE_ERR_INVALIDPC;
 
-        UInt256_FromBytes(bytes + 1, &pt.x);
-        UInt256_FromBytes(bytes + 33, &pt.y);
-        pt.is_inf = 0;
-        SM2JacobPointMont_FromPoint(&pt, X);
-        if (!SM2JacobPointMont_IsOnCurve(X))
+        UInt256_FromBytes(bytes + 1, &X->x);
+        UInt256_FromBytes(bytes + 33, &X->y);
+        X->is_inf = 0;
+        if (!SM2Point_IsOnCurve(X))
             return SM2CURVE_ERR_NOTONCURVE;
     }
     else if (pc == 0x02 || pc == 0x03)
     {
         if (bytes_len != SM2_POINTBYTES_HALF_LENGTH)
             return SM2CURVE_ERR_INVALIDPC;
 
-        UInt256_FromBytes(bytes + 1, &pt.x);
-        if (UInt256_Cmp(&pt.x, CONSTS_P) >= 0)
+        UInt256_FromBytes(bytes + 1, &X->x);
+        if (UInt256_Cmp(&X->x, CONSTS_P) >= 0)
             return SM2CURVE_ERR_NOTONCURVE;
 
-        SM2ModP_ToMont(&pt.x, &X->x);
-        X->z = *CONSTS_MODP_MONT_ONE;
+        SM2ModP_ToMont(&X->x, &X->x);
 
         // compute y
         SM2ModP_MontMul(&X->x, &X->x, &X->y);
         SM2ModP_MontAdd(&X->y, CONSTS_MODP_MONT_A, &X->y);
         SM2ModP_MontMul(&X->x, &X->y, &X->y);
         SM2ModP_MontAdd(&X->y, CONSTS_MODP_MONT_B, &X->y);
         if (!SM2ModP_MontHasSqrt(&X->y, &X->y))
             return SM2CURVE_ERR_NOTONCURVE;
 
-        SM2ModP_FromMont(&X->y, &pt.y);
-        ylsb = pt.y.u8[0] & 0x1;
+        SM2ModP_FromMont(&X->x, &X->x);
+        SM2ModP_FromMont(&X->y, &X->y);
+        ylsb = X->y.u8[0] & 0x1;
         if ((pc == 0x02 && ylsb) || (pc == 0x03 && !ylsb))
         {
-            SM2ModP_MontNeg(&X->y, &X->y);
+            SM2ModP_Neg(&X->y, &X->y);
         }
     }
     else
     {
         return SM2CURVE_ERR_INVALIDPC;
     }
 
     return 0;
 }
 
+uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes)
+{
+    SM2Point pt = { 0 };
+    SM2JacobPointMont_ToPoint(X, &pt);
+    return SM2Point_ToBytes(&pt, pc_mode, bytes);
+}
+
+int SM2JacobPointMont_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2JacobPointMont* X)
+{
+    SM2Point pt = { 0 };
+    int ret = SM2Point_FromBytes(bytes, bytes_len, &pt);
+    if (ret != 0)
+        return ret;
+
+    SM2JacobPointMont_FromPoint(&pt, X);
+    return 0;
+}
+
 static 
 void _SM2JacobPointMont_Dbl(const SM2JacobPointMont* X, SM2JacobPointMont* Y)
 {
     // order is IMPORTANT to avoid data overwrite
 
     SM2ModPMont t1 = { 0 };
     SM2ModPMont t2 = { 0 };
```

### Comparing `gmalglib-0.5.8/src/gmalglib/core/sm2table.c` & `gmalglib-0.5.9/src/gmalglib/core/sm2table.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/sm3.c` & `gmalglib-0.5.9/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/sm4.c` & `gmalglib-0.5.9/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/core/zuc.c` & `gmalglib-0.5.9/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/coremodule.c` & `gmalglib-0.5.9/src/gmalglib/coremodule.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/sm2.pyi` & `gmalglib-0.5.9/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/sm3.pyi` & `gmalglib-0.5.9/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/wrapped.py` & `gmalglib-0.5.9/src/gmalglib/wrapped.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib/zuc.pyi` & `gmalglib-0.5.9/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.8/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.9/src/gmalglib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.8
+Version: 0.5.9
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
@@ -76,23 +76,23 @@
 
 ## Benchmark Test
 
 The benchmark test code can be found in [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py). The test results on the `13th Gen Intel(R) Core(TM) i7-13700H` are as follows:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 2.391558s
-SM2.decrypt             : 1.092445s
-SM2.sign_digest         : 1.062552s
-SM2.verify_digest       : 2.096187s
-SM2.sign                : 1.067850s
-SM2.verify              : 2.055190s
-SM2.begin_key_exchange  : 1.159822s
-SM2.end_key_exchange    : 1.633471s
+SM2.encrypt             : 0.454363s (2200.88 times/s)
+SM2.decrypt             : 0.356014s (2808.88 times/s)
+SM2.sign_digest         : 0.088565s (11291.12 times/s)
+SM2.verify_digest       : 0.409243s (2443.54 times/s)
+SM2.sign                : 0.087475s (11431.80 times/s)
+SM2.verify              : 0.404026s (2475.09 times/s)
+SM2.begin_key_exchange  : 0.086665s (11538.62 times/s)
+SM2.end_key_exchange    : 0.536552s (1863.75 times/s)
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 5.118763s
+SM3.update & SM3.digest : 3.083487s (324,308,109 B/s)
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.369991s
-SM4.decrypt             : 0.297077s
+SM4.encrypt             : 0.197393s (5066040.91 times/s)
+SM4.decrypt             : 0.185619s (5387391.13 times/s)
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.050301s
+zuc.generate            : 0.028821s (34696561.22 times/s)
 ```
```

### Comparing `gmalglib-0.5.8/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.9/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

