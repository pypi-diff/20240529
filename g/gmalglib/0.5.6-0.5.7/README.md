# Comparing `tmp/gmalglib-0.5.6.tar.gz` & `tmp/gmalglib-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.5.6.tar", last modified: Tue May 28 00:55:53 2024, max compression
+gzip compressed data, was "gmalglib-0.5.7.tar", last modified: Wed May 29 08:58:46 2024, max compression
```

## Comparing `gmalglib-0.5.6.tar` & `gmalglib-0.5.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-28 00:55:37.000000 gmalglib-0.5.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-28 00:55:53.186000 gmalglib-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-28 00:55:37.000000 gmalglib-0.5.6/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-28 00:55:37.000000 gmalglib-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.174000 gmalglib-0.5.6/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.178001 gmalglib-0.5.6/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/bignum.h
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/random.h
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2.h
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2curve.h
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm2table.h
--rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-28 00:55:37.000000 gmalglib-0.5.6/include/gmalglib/zuc.h
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-28 00:55:37.000000 gmalglib-0.5.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:55:53.186000 gmalglib-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-28 00:55:37.000000 gmalglib-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.174000 gmalglib-0.5.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.178001 gmalglib-0.5.6/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/src/gmalglib/core/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/bignum.c
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/random.c
--rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2.c
--rw-r--r--   0 runner    (1001) docker     (127)    19181 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2curve.c
--rw-r--r--   0 runner    (1001) docker     (127)  2810569 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm2table.c
--rw-r--r--   0 runner    (1001) docker     (127)     6957 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/core/zuc.c
--rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/coremodule.c
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm4.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/wrapped.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/zuc.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 00:55:37.000000 gmalglib-0.5.6/src/gmalglib/zuc.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:55:53.186000 gmalglib-0.5.6/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 00:55:53.000000 gmalglib-0.5.6/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.241544 gmalglib-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 08:58:40.000000 gmalglib-0.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 08:58:46.241544 gmalglib-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-29 08:58:40.000000 gmalglib-0.5.7/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-29 08:58:40.000000 gmalglib-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.233544 gmalglib-0.5.7/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.233544 gmalglib-0.5.7/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/bignum.h
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/random.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/sm2.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/sm2curve.h
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/sm2table.h
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-29 08:58:40.000000 gmalglib-0.5.7/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-29 08:58:40.000000 gmalglib-0.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:58:46.241544 gmalglib-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 08:58:40.000000 gmalglib-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.233544 gmalglib-0.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.237544 gmalglib-0.5.7/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-29 08:58:40.000000 gmalglib-0.5.7/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.241544 gmalglib-0.5.7/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-05-29 08:58:40.000000 gmalglib-0.5.7/src/gmalglib/core/bignum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-29 08:58:40.000000 gmalglib-0.5.7/src/gmalglib/core/random.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21780 2024-05-29 08:58:40.000000 gmalglib-0.5.7/src/gmalglib/core/sm2.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21060 2024-05-29 08:58:40.000000 gmalglib-0.5.7/src/gmalglib/core/sm2curve.c
+-rw-r--r--   0 runner    (1001) docker     (127)  2810569 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/core/sm2table.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    39972 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4195 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/wrapped.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 08:58:41.000000 gmalglib-0.5.7/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:58:46.241544 gmalglib-0.5.7/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-29 08:58:46.000000 gmalglib-0.5.7/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 08:58:46.000000 gmalglib-0.5.7/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:58:46.000000 gmalglib-0.5.7/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 08:58:46.000000 gmalglib-0.5.7/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.5.6/LICENSE` & `gmalglib-0.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/PKG-INFO` & `gmalglib-0.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.5.6/README.en.md` & `gmalglib-0.5.7/README.en.md`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/README.md` & `gmalglib-0.5.7/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -62,23 +62,23 @@
 
 ## 性能测试
 
 性能测试代码见 [benchmark.py](https://github.com/ww-rm/gmalglib/blob/main/benchmark.py), `13th Gen Intel(R) Core(TM) i7-13700H` 上测试结果如下:
 
 ```plain
 ==================== SM2 Benchmark Test (1000 times, 32 bytes data) ====================
-SM2.encrypt             : 0.766956s
-SM2.decrypt             : 0.678737s
-SM2.sign_digest         : 0.100963s
-SM2.verify_digest       : 0.707086s
-SM2.sign                : 0.100675s
-SM2.verify              : 0.729823s
-SM2.begin_key_exchange  : 0.153279s
-SM2.end_key_exchange    : 0.988622s
+SM2.encrypt             : 0.482069s (2074.39 times/s)
+SM2.decrypt             : 0.380268s (2629.72 times/s)
+SM2.sign_digest         : 0.100307s (9969.43 times/s)
+SM2.verify_digest       : 0.419963s (2381.16 times/s)
+SM2.sign                : 0.103122s (9697.30 times/s)
+SM2.verify              : 0.411118s (2432.39 times/s)
+SM2.begin_key_exchange  : 0.150200s (6657.79 times/s)
+SM2.end_key_exchange    : 0.536930s (1862.44 times/s)
 ==================== SM3 Benchmark Test (1,000,000,000 bytes data) ====================
-SM3.update & SM3.digest : 3.014004s
+SM3.update & SM3.digest : 3.082285s (324,434,643 B/s)
 ==================== SM4 Benchmark Test (1000000 times) ====================
-SM4.encrypt             : 0.185529s
-SM4.decrypt             : 0.184629s
+SM4.encrypt             : 0.199543s (5011458.70 times/s)
+SM4.decrypt             : 0.186599s (5359085.53 times/s)
 ==================== ZUC Benchmark Test (1000000 times) ====================
-zuc.generate            : 0.029673s
+zuc.generate            : 0.030584s (32697048.76 times/s)
 ```
```

### Comparing `gmalglib-0.5.6/include/gmalglib/bignum.h` & `gmalglib-0.5.7/include/gmalglib/bignum.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/include/gmalglib/random.h` & `gmalglib-0.5.7/include/gmalglib/random.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/include/gmalglib/sm2.h` & `gmalglib-0.5.7/include/gmalglib/sm2.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/include/gmalglib/sm2curve.h` & `gmalglib-0.5.7/include/gmalglib/sm2curve.h`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 uint64_t SM2JacobPointMont_ToBytes(const SM2JacobPointMont* X, int pc_mode, uint8_t* bytes);
 int SM2JacobPointMont_FromBytes(const uint8_t* bytes, uint64_t bytes_len, SM2JacobPointMont* X);
 
 int SM2JacobPointMont_IsInf(const SM2JacobPointMont* X);
 void SM2JacobPointMont_SetInf(SM2JacobPointMont* X);
 int SM2JacobPointMont_IsOnCurve(const SM2JacobPointMont* X);
 int SM2JacobPointMont_IsEqual(const SM2JacobPointMont* X, const SM2JacobPointMont* Y);
+void SM2JacobPointMont_Dbl(const SM2JacobPointMont* X, SM2JacobPointMont* Y);
 void SM2JacobPointMont_Add(const SM2JacobPointMont* X, const SM2JacobPointMont* Y, SM2JacobPointMont* Z);
 void SM2JacobPointMont_Mul(const UInt256* k, const SM2JacobPointMont* X, SM2JacobPointMont* Y);
 void SM2JacobPointMont_Neg(const SM2JacobPointMont* X, SM2JacobPointMont* Y);
 void SM2JacobPointMont_Sub(const SM2JacobPointMont* X, const SM2JacobPointMont* Y, SM2JacobPointMont* Z);
 void SM2JacobPointMont_MulG(const UInt256* k, SM2JacobPointMont* X);
 
 #ifdef _DEBUG
```

### Comparing `gmalglib-0.5.6/include/gmalglib/sm3.h` & `gmalglib-0.5.7/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/pyproject.toml` & `gmalglib-0.5.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/setup.py` & `gmalglib-0.5.7/setup.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/bignum.c` & `gmalglib-0.5.7/src/gmalglib/core/bignum.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/random.c` & `gmalglib-0.5.7/src/gmalglib/core/random.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/sm2.c` & `gmalglib-0.5.7/src/gmalglib/core/sm2.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/sm2curve.c` & `gmalglib-0.5.7/src/gmalglib/core/sm2curve.c`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 
 #ifdef _DEBUG
 
 #include <stdio.h>
 
 #endif // _DEBUG
 
+#define POINTMUL_WSIZE          4
+#define POINTMUL_TSIZE          (1 << (POINTMUL_WSIZE - 1))
+
 
 // 0xFFFFFFFE_FFFFFFFF_FFFFFFFF_FFFFFFFF_FFFFFFFF_00000000_FFFFFFFF_FFFFFFFF
 static const UInt256 _CONSTS_P = { .u32 = {
     0xFFFFFFFF, 0xFFFFFFFF, 0x00000000, 0xFFFFFFFF,
     0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFF, 0xFFFFFFFE
 } };
 static const UInt256* const CONSTS_P = &_CONSTS_P;
@@ -512,14 +515,26 @@
 
     // y' = t1(t2 - x') - t3
     SM2ModP_MontSub(&t2, &Y->x, &Y->y);
     SM2ModP_MontMul(&t1, &Y->y, &Y->y);
     SM2ModP_MontSub(&Y->y, &t3, &Y->y);
 }
 
+void SM2JacobPointMont_Dbl(const SM2JacobPointMont* X, SM2JacobPointMont* Y)
+{
+    if (SM2JacobPointMont_IsInf(X))
+    {
+        *Y = *X;
+    }
+    else
+    {
+        _SM2JacobPointMont_Dbl(X, Y);
+    }
+}
+
 static 
 void _SM2JacobPointMont_Add(const SM2JacobPointMont* X, const SM2JacobPointMont* Y, SM2JacobPointMont* Z)
 {
     SM2ModPMont t1 = { 0 };
     SM2ModPMont t2 = { 0 };
     SM2ModPMont t3 = { 0 };
     SM2ModPMont t4 = { 0 };
@@ -588,39 +603,99 @@
     }
     else
     {
         _SM2JacobPointMont_Add(X, Y, Z);
     }
 }
 
-void SM2JacobPointMont_Mul(const UInt256* k, const SM2JacobPointMont* X, SM2JacobPointMont* Y)
-{
-    int32_t i;
-    uint32_t j;
-    uint64_t tmp = 0;
+//static
+//void _SM2JacobPointMont_Mul_DblAndAdd(const UInt256* k, const SM2JacobPointMont* X, SM2JacobPointMont* Y)
+//{
+//    int32_t i;
+//    uint32_t j;
+//    uint64_t tmp = 0;
+//    SM2JacobPointMont Y_tmp = { 0 };
+//    SM2JacobPointMont_SetInf(&Y_tmp);
+//
+//    for (i = 3; i >= 0; i--)
+//    {
+//        tmp = k->u64[i];
+//        for (j = 0; j < 64; j++)
+//        {
+//            SM2JacobPointMont_Dbl(&Y_tmp, &Y_tmp);
+//            if (tmp & 0x8000000000000000)
+//            {
+//                SM2JacobPointMont_Add(&Y_tmp, X, &Y_tmp);
+//            }
+//            tmp <<= 1;
+//        }
+//    }
+//
+//    *Y = Y_tmp;
+//}
+
+static
+void _SM2JacobPointMont_Mul_SlidingWindow(const UInt256* k, const SM2JacobPointMont* X, SM2JacobPointMont* Y)
+{
+    int32_t i = 0;
+    int32_t j = 0;
+    int32_t w = 0;
+    uint32_t wvalue = 0;
     SM2JacobPointMont Y_tmp = { 0 };
-    SM2JacobPointMont_SetInf(&Y_tmp);
 
-    for (i = 3; i >= 0; i--)
+    // pre-compute, save odd points, 1, 3, 5, ..., 2^w - 1
+    SM2JacobPointMont table[POINTMUL_TSIZE] = { *X };
+    SM2JacobPointMont_Dbl(X, &Y_tmp);
+    for (i = 0; i < POINTMUL_TSIZE - 1; i++)
     {
-        tmp = k->u64[i];
-        for (j = 0; j < 64; j++)
+        SM2JacobPointMont_Add(table + i, &Y_tmp, table + i + 1);
+    }
+
+    SM2JacobPointMont_SetInf(&Y_tmp);
+    i = 255;
+    while (i >= 0)
+    {
+        wvalue = (k->u64[i / 64] >> (i % 64)) & 0x1;
+
+        if (wvalue == 0)
         {
-            SM2JacobPointMont_Add(&Y_tmp, &Y_tmp, &Y_tmp);
-            if (tmp & 0x8000000000000000)
+            SM2JacobPointMont_Dbl(&Y_tmp, &Y_tmp);
+            i--;
+        }
+        else
+        {
+            // find a longest 1...1 bits in window size
+            j = i;
+            for (w = i - 1; w >= 0 && w > i - POINTMUL_WSIZE; w--)
             {
-                SM2JacobPointMont_Add(&Y_tmp, X, &Y_tmp);
+                if ((k->u64[w / 64] >> (w % 64)) & 0x1)
+                {
+                    wvalue = (wvalue << (j - w)) | 0x1;
+                    j = w;
+                }
             }
-            tmp <<= 1;
+
+            while (i >= j)
+            {
+                SM2JacobPointMont_Dbl(&Y_tmp, &Y_tmp);
+                i--;
+            }
+
+            SM2JacobPointMont_Add(&Y_tmp, table + (wvalue >> 1), &Y_tmp);
         }
     }
 
     *Y = Y_tmp;
 }
 
+void SM2JacobPointMont_Mul(const UInt256* k, const SM2JacobPointMont* X, SM2JacobPointMont* Y)
+{
+    _SM2JacobPointMont_Mul_SlidingWindow(k, X, Y);
+}
+
 void SM2JacobPointMont_Neg(const SM2JacobPointMont* X, SM2JacobPointMont* Y)
 {
     Y->x = X->x;
     SM2ModP_MontNeg(&X->y, &Y->y);
     Y->z = X->z;
 }
```

### Comparing `gmalglib-0.5.6/src/gmalglib/core/sm2table.c` & `gmalglib-0.5.7/src/gmalglib/core/sm2table.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/sm3.c` & `gmalglib-0.5.7/src/gmalglib/core/sm3.c`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 {
     bytes[0] = (uint8_t)(word >> 24);
     bytes[1] = (uint8_t)(word >> 16);
     bytes[2] = (uint8_t)(word >> 8);
     bytes[3] = (uint8_t)(word);
 }
 
-static inline
-uint32_t T(uint32_t i)
-{
-    return i <= 15 ? 0x79cc4519 : 0x7a879d8a;
-}
+//static inline
+//uint32_t T(uint32_t i)
+//{
+//    return i <= 15 ? 0x79cc4519 : 0x7a879d8a;
+//}
 
 static inline
 uint32_t FF(uint32_t i, uint32_t X, uint32_t Y, uint32_t Z)
 {
     return i <= 15 ? (X ^ Y ^ Z) : ((X & Y) | (X & Z) | (Y & Z));
 }
```

### Comparing `gmalglib-0.5.6/src/gmalglib/core/sm4.c` & `gmalglib-0.5.7/src/gmalglib/core/sm4.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/core/zuc.c` & `gmalglib-0.5.7/src/gmalglib/core/zuc.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/coremodule.c` & `gmalglib-0.5.7/src/gmalglib/coremodule.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/sm2.pyi` & `gmalglib-0.5.7/src/gmalglib/sm2.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/sm3.pyi` & `gmalglib-0.5.7/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/wrapped.py` & `gmalglib-0.5.7/src/gmalglib/wrapped.py`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib/zuc.pyi` & `gmalglib-0.5.7/src/gmalglib/zuc.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.5.6/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.5.7/src/gmalglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.5.6
+Version: 0.5.7
 Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gmalglib-0.5.6/src/gmalglib.egg-info/SOURCES.txt` & `gmalglib-0.5.7/src/gmalglib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

