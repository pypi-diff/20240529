# Comparing `tmp/vnpy_ctabacktester-1.1.2.tar.gz` & `tmp/vnpy_ctabacktester-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_ctabacktester-1.1.2.tar", last modified: Mon Sep  4 01:27:15 2023, max compression
+gzip compressed data, was "vnpy_ctabacktester-1.1.3.tar", last modified: Wed May 29 13:05:39 2024, max compression
```

## Comparing `vnpy_ctabacktester-1.1.2.tar` & `vnpy_ctabacktester-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-09-04 01:27:14.993368 vnpy_ctabacktester-1.1.2/
--rw-rw-rw-   0        0        0     1107 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     1889 2023-09-04 01:27:14.993368 vnpy_ctabacktester-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      926 2023-09-04 01:21:27.000000 vnpy_ctabacktester-1.1.2/README.md
--rw-rw-rw-   0        0        0     1063 2023-09-04 01:27:15.031244 vnpy_ctabacktester-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0       43 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-04 01:27:14.957181 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/
--rw-rw-rw-   0        0        0     1810 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/__init__.py
--rw-rw-rw-   0        0        0    14499 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/engine.py
-drwxrwxrwx   0        0        0        0 2023-09-04 01:27:14.992344 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/
--rw-rw-rw-   0        0        0       39 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/__init__.py
--rw-rw-rw-   0        0        0    64478 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/backtester.ico
--rw-rw-rw-   0        0        0    50717 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/widget.py
-drwxrwxrwx   0        0        0        0 2023-09-04 01:27:14.965901 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/
--rw-rw-rw-   0        0        0     1889 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      449 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-09-04 01:27:14.000000 vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:05:39.233173 vnpy_ctabacktester-1.1.3/
+-rw-rw-rw-   0        0        0     1107 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1893 2024-05-29 13:05:39.234222 vnpy_ctabacktester-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      928 2024-05-29 13:04:28.000000 vnpy_ctabacktester-1.1.3/README.md
+-rw-rw-rw-   0        0        0     1065 2024-05-29 13:05:39.235812 vnpy_ctabacktester-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       43 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:05:39.158605 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/
+-rw-rw-rw-   0        0        0     1810 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/__init__.py
+-rw-rw-rw-   0        0        0    14545 2024-05-29 13:02:44.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/engine.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:05:39.232123 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/
+-rw-rw-rw-   0        0        0       39 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/__init__.py
+-rw-rw-rw-   0        0        0    64478 2023-09-04 01:20:48.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/backtester.ico
+-rw-rw-rw-   0        0        0    50848 2024-05-29 13:02:44.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/widget.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:05:39.227930 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/
+-rw-rw-rw-   0        0        0     1893 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 13:05:38.000000 vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/top_level.txt
```

### Comparing `vnpy_ctabacktester-1.1.2/LICENSE` & `vnpy_ctabacktester-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.2/PKG-INFO` & `vnpy_ctabacktester-1.1.3/vnpy_ctabacktester.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: vnpy_ctabacktester
-Version: 1.1.2
+Name: vnpy-ctabacktester
+Version: 1.1.3
 Summary: CTA strategy backtesting application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,27 +24,27 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.2-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 图形化CTA策略回测模块，基于用户友好的图形界面实现简洁易用的数据下载、历史回测和参数优化等投研功能。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_ctabacktester
 ```
```

### Comparing `vnpy_ctabacktester-1.1.2/README.md` & `vnpy_ctabacktester-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.2-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 图形化CTA策略回测模块，基于用户友好的图形界面实现简洁易用的数据下载、历史回测和参数优化等投研功能。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_ctabacktester
 ```
```

### Comparing `vnpy_ctabacktester-1.1.2/setup.cfg` & `vnpy_ctabacktester-1.1.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6e70 795f 6374 6162 6163 6b74   = vnpy_ctabackt
 00000020: 6573 7465 720d 0a76 6572 7369 6f6e 203d  ester..version =
-00000030: 2031 2e31 2e32 0d0a 7572 6c20 3d20 6874   1.1.2..url = ht
+00000030: 2031 2e31 2e33 0d0a 7572 6c20 3d20 6874   1.1.3..url = ht
 00000040: 7470 733a 2f2f 7777 772e 766e 7079 2e63  tps://www.vnpy.c
 00000050: 6f6d 0d0a 6c69 6365 6e73 6520 3d20 4d49  om..license = MI
 00000060: 540d 0a61 7574 686f 7220 3d20 5869 616f  T..author = Xiao
 00000070: 796f 7520 4368 656e 0d0a 6175 7468 6f72  you Chen..author
 00000080: 5f65 6d61 696c 203d 2078 6961 6f79 6f75  _email = xiaoyou
 00000090: 2e63 6865 6e40 6d61 696c 2e76 6e70 792e  .chen@mail.vnpy.
 000000a0: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
@@ -30,38 +30,38 @@
 000001d0: 5374 6162 6c65 0d0a 094f 7065 7261 7469  Stable...Operati
 000001e0: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
 000001f0: 496e 6465 7065 6e64 656e 740d 0a09 5072  Independent...Pr
 00000200: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
 00000210: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
 00000220: 330d 0a09 5072 6f67 7261 6d6d 696e 6720  3...Programming 
 00000230: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000240: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
-00000250: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000260: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000270: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
-00000280: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000290: 6f6e 203a 3a20 332e 3130 0d0a 0954 6f70  on :: 3.10...Top
-000002a0: 6963 203a 3a20 4f66 6669 6365 2f42 7573  ic :: Office/Bus
-000002b0: 696e 6573 7320 3a3a 2046 696e 616e 6369  iness :: Financi
-000002c0: 616c 203a 3a20 496e 7665 7374 6d65 6e74  al :: Investment
-000002d0: 0d0a 0950 726f 6772 616d 6d69 6e67 204c  ...Programming L
-000002e0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000002f0: 6e20 3a3a 2049 6d70 6c65 6d65 6e74 6174  n :: Implementat
-00000300: 696f 6e20 3a3a 2043 5079 7468 6f6e 0d0a  ion :: CPython..
-00000310: 094c 6963 656e 7365 203a 3a20 4f53 4920  .License :: OSI 
-00000320: 4170 7072 6f76 6564 203a 3a20 4d49 5420  Approved :: MIT 
-00000330: 4c69 6365 6e73 650d 0a09 4e61 7475 7261  License...Natura
-00000340: 6c20 4c61 6e67 7561 6765 203a 3a20 4368  l Language :: Ch
-00000350: 696e 6573 6520 2853 696d 706c 6966 6965  inese (Simplifie
-00000360: 6429 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  d)....[options].
-00000370: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
-00000380: 3a0d 0a7a 6970 5f73 6166 6520 3d20 4661  :..zip_safe = Fa
-00000390: 6c73 650d 0a70 7974 686f 6e5f 7265 7175  lse..python_requ
-000003a0: 6972 6573 203d 203e 3d33 2e37 0d0a 696e  ires = >=3.7..in
-000003b0: 7374 616c 6c5f 7265 7175 6972 6573 203d  stall_requires =
-000003c0: 200d 0a09 766e 7079 5f63 7461 7374 7261   ...vnpy_ctastra
-000003d0: 7465 6779 0d0a 0d0a 5b6f 7074 696f 6e73  tegy....[options
-000003e0: 2e70 6163 6b61 6765 5f64 6174 615d 0d0a  .package_data]..
-000003f0: 2a20 3d20 2a2e 6963 6f0d 0a0d 0a5b 6567  * = *.ico....[eg
-00000400: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-00000410: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000420: 3d20 300d 0a0d 0a                        = 0....
+00000240: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000250: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000260: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000270: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000280: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000290: 7468 6f6e 203a 3a20 332e 3132 0d0a 0954  thon :: 3.12...T
+000002a0: 6f70 6963 203a 3a20 4f66 6669 6365 2f42  opic :: Office/B
+000002b0: 7573 696e 6573 7320 3a3a 2046 696e 616e  usiness :: Finan
+000002c0: 6369 616c 203a 3a20 496e 7665 7374 6d65  cial :: Investme
+000002d0: 6e74 0d0a 0950 726f 6772 616d 6d69 6e67  nt...Programming
+000002e0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000002f0: 686f 6e20 3a3a 2049 6d70 6c65 6d65 6e74  hon :: Implement
+00000300: 6174 696f 6e20 3a3a 2043 5079 7468 6f6e  ation :: CPython
+00000310: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
+00000320: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
+00000330: 5420 4c69 6365 6e73 650d 0a09 4e61 7475  T License...Natu
+00000340: 7261 6c20 4c61 6e67 7561 6765 203a 3a20  ral Language :: 
+00000350: 4368 696e 6573 6520 2853 696d 706c 6966  Chinese (Simplif
+00000360: 6965 6429 0d0a 0d0a 5b6f 7074 696f 6e73  ied)....[options
+00000370: 5d0d 0a70 6163 6b61 6765 7320 3d20 6669  ]..packages = fi
+00000380: 6e64 3a0d 0a7a 6970 5f73 6166 6520 3d20  nd:..zip_safe = 
+00000390: 4661 6c73 650d 0a70 7974 686f 6e5f 7265  False..python_re
+000003a0: 7175 6972 6573 203d 203e 3d33 2e37 0d0a  quires = >=3.7..
+000003b0: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
+000003c0: 203d 200d 0a09 766e 7079 5f63 7461 7374   = ...vnpy_ctast
+000003d0: 7261 7465 6779 0d0a 0d0a 5b6f 7074 696f  rategy....[optio
+000003e0: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+000003f0: 0d0a 2a20 3d20 2a2e 6963 6f0d 0a0d 0a5b  ..* = *.ico....[
+00000400: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+00000410: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+00000420: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/__init__.py` & `vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/engine.py` & `vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,16 @@
             strategy_class,
             setting
         )
 
         engine.load_data()
         if not engine.history_data:
             self.write_log("策略回测失败，历史数据为空")
+            
+            self.thread = None
             return
 
         try:
             engine.run_backtesting()
         except Exception:
             msg: str = f"策略回测失败，触发异常：\n{traceback.format_exc()}"
             self.write_log(msg)
```

### Comparing `vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/backtester.ico` & `vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/backtester.ico`

 * *Files identical despite different names*

### Comparing `vnpy_ctabacktester-1.1.2/vnpy_ctabacktester/ui/widget.py` & `vnpy_ctabacktester-1.1.3/vnpy_ctabacktester/ui/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -564,14 +564,15 @@
         "daily_slippage": "日均滑点",
         "daily_turnover": "日均成交额",
         "daily_trade_count": "日均成交笔数",
 
         "daily_return": "日均收益率",
         "return_std": "收益标准差",
         "sharpe_ratio": "夏普比率",
+        "ewm_sharpe": "EWM夏普",
         "return_drawdown_ratio": "收益回撤比"
     }
 
     def __init__(self) -> None:
         """"""
         super().__init__()
 
@@ -617,14 +618,15 @@
         data["daily_commission"] = f"{data['daily_commission']:,.2f}"
         data["daily_slippage"] = f"{data['daily_slippage']:,.2f}"
         data["daily_turnover"] = f"{data['daily_turnover']:,.2f}"
         data["daily_trade_count"] = f"{data['daily_trade_count']:,.2f}"
         data["daily_return"] = f"{data['daily_return']:,.2f}%"
         data["return_std"] = f"{data['return_std']:,.2f}%"
         data["sharpe_ratio"] = f"{data['sharpe_ratio']:,.2f}"
+        data["ewm_sharpe"] = f"{data['ewm_sharpe']:,.2f}"
         data["return_drawdown_ratio"] = f"{data['return_drawdown_ratio']:,.2f}"
 
         for key, cell in self.cells.items():
             value = data.get(key, "")
             cell.setText(str(value))
 
 
@@ -833,14 +835,15 @@
 class OptimizationSettingEditor(QtWidgets.QDialog):
     """
     For setting up parameters for optimization.
     """
     DISPLAY_NAME_MAP: dict = {
         "总收益率": "total_return",
         "夏普比率": "sharpe_ratio",
+        "EWM夏普": "ewm_sharpe",
         "收益回撤比": "return_drawdown_ratio",
         "日均盈亏": "daily_net_pnl"
     }
 
     def __init__(
         self, class_name: str, parameters: dict
     ) -> None:
```

### Comparing `vnpy_ctabacktester-1.1.2/vnpy_ctabacktester.egg-info/PKG-INFO` & `vnpy_ctabacktester-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
-Name: vnpy-ctabacktester
-Version: 1.1.2
+Name: vnpy_ctabacktester
+Version: 1.1.3
 Summary: CTA strategy backtesting application for VeighNa quant trading framework.
 Home-page: https://www.vnpy.com
 Author: Xiaoyou Chen
 Author-email: xiaoyou.chen@mail.vnpy.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: Chinese (Simplified)
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,27 +24,27 @@
 # VeighNa框架的CTA投研模块
 
 <p align="center">
   <img src ="https://vnpy.oss-cn-shanghai.aliyuncs.com/vnpy-logo.png"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-1.1.2-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-1.1.3-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.8|3.9|3.10-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
     <img src ="https://img.shields.io/github/license/vnpy/vnpy.svg?color=orange"/>
 </p>
 
 ## 说明
 
 图形化CTA策略回测模块，基于用户友好的图形界面实现简洁易用的数据下载、历史回测和参数优化等投研功能。
 
 ## 安装
 
-安装环境推荐基于3.7.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
+安装环境推荐基于3.9.0版本以上的【[**VeighNa Studio**](https://www.vnpy.com)】。
 
 直接使用pip命令：
 
 ```
 pip install vnpy_ctabacktester
 ```
```

