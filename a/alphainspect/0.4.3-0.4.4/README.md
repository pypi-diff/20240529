# Comparing `tmp/alphainspect-0.4.3.tar.gz` & `tmp/alphainspect-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphainspect-0.4.3.tar", last modified: Mon May 20 07:13:56 2024, max compression
+gzip compressed data, was "alphainspect-0.4.4.tar", last modified: Wed May 29 04:21:10 2024, max compression
```

## Comparing `alphainspect-0.4.3.tar` & `alphainspect-0.4.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:13:56.353816 alphainspect-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 07:13:49.000000 alphainspect-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-20 07:13:56.353816 alphainspect-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-20 07:13:49.000000 alphainspect-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:13:56.353816 alphainspect-0.4.3/alphainspect/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/_nb.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/dtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/ic.py
--rw-r--r--   0 runner    (1001) docker     (127)     8845 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/turnover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2024-05-20 07:13:49.000000 alphainspect-0.4.3/alphainspect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:13:56.353816 alphainspect-0.4.3/alphainspect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-20 07:13:56.000000 alphainspect-0.4.3/alphainspect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-20 07:13:56.000000 alphainspect-0.4.3/alphainspect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:13:56.000000 alphainspect-0.4.3/alphainspect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 07:13:56.000000 alphainspect-0.4.3/alphainspect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-20 07:13:56.000000 alphainspect-0.4.3/alphainspect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-20 07:13:49.000000 alphainspect-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:13:56.353816 alphainspect-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:21:10.504953 alphainspect-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 04:21:02.000000 alphainspect-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-29 04:21:10.504953 alphainspect-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-29 04:21:02.000000 alphainspect-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:21:10.504953 alphainspect-0.4.4/alphainspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/_nb.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/dtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/ic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/turnover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10035 2024-05-29 04:21:02.000000 alphainspect-0.4.4/alphainspect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 04:21:10.504953 alphainspect-0.4.4/alphainspect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-29 04:21:10.000000 alphainspect-0.4.4/alphainspect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-29 04:21:10.000000 alphainspect-0.4.4/alphainspect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 04:21:10.000000 alphainspect-0.4.4/alphainspect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 04:21:10.000000 alphainspect-0.4.4/alphainspect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 04:21:10.000000 alphainspect-0.4.4/alphainspect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 04:21:02.000000 alphainspect-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 04:21:10.504953 alphainspect-0.4.4/setup.cfg
```

### Comparing `alphainspect-0.4.3/LICENSE` & `alphainspect-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/PKG-INFO` & `alphainspect-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.4.3
+Version: 0.4.4
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.4.3/README.md` & `alphainspect-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/_nb.py` & `alphainspect-0.4.4/alphainspect/_nb.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/dtree.py` & `alphainspect-0.4.4/alphainspect/dtree.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/events.py` & `alphainspect-0.4.4/alphainspect/events.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/ic.py` & `alphainspect-0.4.4/alphainspect/ic.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from matplotlib import pyplot as plt
 from polars import Expr
 from scipy import stats
 from sklearn.feature_selection import mutual_info_regression
 from statsmodels import api as sm
 
 from alphainspect import _DATE_
-from alphainspect.utils import plot_heatmap, get_row_col, select_by_suffix, plot_hist
+from alphainspect.utils import plot_heatmap, get_row_col, select_by_suffix, plot_hist, index_split_unstack
 
 
 def rank_ic(a: str, b: str) -> Expr:
     """RankIC"""
     return pl.corr(a, b, method='spearman', ddof=0, propagate_nans=False)
 
 
@@ -73,20 +73,14 @@
 
 
 def calc_ic_corr(df_pl: pl.DataFrame) -> pd.DataFrame:
     """由于numpy版不能很好的处理空值，所以用pandas版"""
     return df_pl.to_pandas().corr(method="pearson")
 
 
-def row_unstack(df_pl: pl.DataFrame, factors: Sequence[str], forward_returns: Sequence[str]) -> pd.DataFrame:
-    """一行值堆叠成一个矩阵"""
-    return pd.DataFrame(df_pl.to_numpy().reshape(len(factors), len(forward_returns)),
-                        index=factors, columns=forward_returns)
-
-
 def plot_ic_ts(df_pl: pl.DataFrame, col: str,
                *,
                axvlines=(), ax=None) -> Dict[str, float]:
     """IC时序图
 
     Examples
     --------
@@ -178,18 +172,20 @@
                      *,
                      axvlines=(), ) -> pl.DataFrame:
     """生成IC图表。多因子多收益率。
 
     用于分析相似因子在不同持有期下的IC信息
     """
     df_pl = calc_ic(df_pl, factors, forward_returns)
-    df_ic = calc_ic_mean(df_pl)
-    df_ir = calc_ic_ir(df_pl)
-    df_ic = row_unstack(df_ic, factors, forward_returns)
-    df_ir = row_unstack(df_ir, factors, forward_returns)
+    df_ic = calc_ic_mean(df_pl).to_pandas().iloc[0]
+    df_ir = calc_ic_ir(df_pl).to_pandas().iloc[0]
+
+    df_ic = index_split_unstack(df_ic)
+    df_ir = index_split_unstack(df_ir)
+
     logger.info('Mean IC: {} \n{}', '=' * 60, df_ic)
     logger.info('IC_IR: {} \n{}', '=' * 60, df_ir)
 
     # 画ic与ir的热力图
     fig, axes = plt.subplots(1, 2, figsize=(12, 9))
     plot_heatmap(df_ic, title='Mean IC', ax=axes[0])
     plot_heatmap(df_ir, title='IR', ax=axes[1])
```

### Comparing `alphainspect-0.4.3/alphainspect/portfolio.py` & `alphainspect-0.4.4/alphainspect/portfolio.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def plot_quantile_portfolio(df_pd: pd.DataFrame, fwd_ret_1: str,
                             long_short=None,
                             *,
                             axvlines=None, ax=None) -> None:
     ax = df_pd.plot(ax=ax, title=f'{fwd_ret_1}', cmap='coolwarm', lw=1, grid=True)
     if long_short is not None:
-        long_short.plot(ax=ax, c="g", ls="--", lw=1, label='L-S')
+        long_short.plot(ax=ax, c="g", ls="--", lw=1, label='L-S', grid=True)
     ax.legend(loc='upper left')
     ax.set_xlabel('')
     for v in axvlines:
         ax.axvline(x=v, c="b", ls="--", lw=1)
 
 
 def plot_portfolio_heatmap_monthly(df_pd: pd.DataFrame,
```

### Comparing `alphainspect-0.4.3/alphainspect/reports.py` & `alphainspect-0.4.4/alphainspect/reports.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/returns.py` & `alphainspect-0.4.4/alphainspect/returns.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Sequence
 
 import matplotlib.pyplot as plt
 import polars as pl
 import seaborn as sns
 
 from alphainspect import _QUANTILE_
+from alphainspect.utils import plot_heatmap
 
 
 def plot_quantile_returns_bar(df_pl: pl.DataFrame, factor: str, forward_returns: Sequence[str],
                               *,
                               factor_quantile: str = _QUANTILE_,
                               ax=None):
     """分组收益柱状图
@@ -50,7 +51,36 @@
 
     # 一定要过滤null才能用
     df_pl = df_pl.filter(pl.col(factor_quantile).is_not_null())
     plot_quantile_returns_bar(df_pl, factor, forward_returns, factor_quantile=factor_quantile, ax=axes[0])
     plot_quantile_returns_box(df_pl, factor, forward_returns, factor_quantile=factor_quantile, ax=axes[1])
 
     fig.tight_layout()
+
+
+def create_returns2_sheet(df_pl: pl.DataFrame,
+                          forward_return: str,
+                          factor_quantiles: Sequence[str]):
+    """双重排序法。灵活使用分组方法能实现独立双重排序和条件双重排序
+
+    例如，将两个因子划分成5*5，查看两因子组合效果
+
+    Parameters
+    ----------
+    df_pl
+    forward_return
+    factor_quantiles
+
+    """
+    fig, axes = plt.subplots(1, 2, figsize=(12, 9))
+
+    df_pl = df_pl.filter([pl.col(q).is_not_null() for q in factor_quantiles])
+
+    df_mean = df_pl.group_by(factor_quantiles).agg(pl.mean(forward_return)).sort(factor_quantiles).to_pandas()
+    df_std = df_pl.group_by(factor_quantiles).agg(pl.std(forward_return, ddof=0)).sort(factor_quantiles).to_pandas()
+    df_mean = df_mean.set_index(factor_quantiles)[forward_return].unstack()
+    df_std = df_std.set_index(factor_quantiles)[forward_return].unstack()
+
+    plot_heatmap(df_mean, title='Mean', ax=axes[0])
+    plot_heatmap(df_std, title='Std', ax=axes[1])
+
+    fig.tight_layout()
```

### Comparing `alphainspect-0.4.3/alphainspect/selection.py` & `alphainspect-0.4.4/alphainspect/selection.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/turnover.py` & `alphainspect-0.4.4/alphainspect/turnover.py`

 * *Files identical despite different names*

### Comparing `alphainspect-0.4.3/alphainspect/utils.py` & `alphainspect-0.4.4/alphainspect/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,116 @@
 import math
-from typing import Dict
+from typing import Dict, Sequence, Optional
 
 import numpy as np
 import pandas as pd
 import polars as pl
 import seaborn as sns
 from loguru import logger
 from polars import selectors as cs
 
-from alphainspect import _QUANTILE_, _DATE_, _GROUP_
+from alphainspect import _QUANTILE_, _DATE_
 from alphainspect._nb import _sub_portfolio_returns
 
 
 def rank_qcut(x: pl.Expr, q: int = 10) -> pl.Expr:
-    """结果与qcut基本一样，速度快三倍"""
+    """结果与qcut基本一样，速度快三倍。取值范围0~1"""
     # TODO 等官方提供原生功能
     a = x.rank(method='min') - 1.001
     b = pl.max_horizontal(x.count() - 1, 1)
     return (a / b * q).cast(pl.Int16)
 
 
-def with_factor_quantile(df_pl: pl.DataFrame, factor: str, quantiles: int = 10, by_group: bool = False, factor_quantile: str = _QUANTILE_) -> pl.DataFrame:
-    """添加因子分位数信息
+def rank_top(x: pl.Expr, k: int = 10) -> pl.Expr:
+    """前K后K, 取值范围0、1、2
+    0表示做空
+    2表示做多
+    1表示即不做多也不做空。如果数量<2K很大，导致某支即分到多也分到空，那就对冲成1
+    """
+    # 使用min是因为因子值可能一样，如果按dense可能导致结果随机。
+    # 由于重复值，组内数量可能大于k
+
+    # 值越大排第一,用来做多
+    a = x.rank(method='min', descending=True) <= k
+    # 值越小排第一，用来做空
+    b = x.rank(method='min', descending=False) <= k
+    return a.cast(pl.Int8) - b.cast(pl.Int8) + 1
+
+
+def with_factor_quantile(df_pl: pl.DataFrame, factor: str, quantiles: int = 10, group_name: Optional[str] = None, factor_quantile: str = _QUANTILE_) -> pl.DataFrame:
+    """添加因子分位数信息。隐含了按日期分组
 
     Parameters
     ----------
     df_pl
     factor: str
         因子名
     quantiles: int
         分层数
-    by_group:bool
-        是否分组
+    group_name:str
+        条件分组
     factor_quantile:str
         分组名
 
     Returns
     -------
     pl.DataFrame
 
     """
+    F = pl.col(factor)
 
     def _func_cs(df: pl.DataFrame):
         return df.with_columns([
-            rank_qcut(pl.col(factor), quantiles).alias(factor_quantile),
+            rank_qcut(F, quantiles).alias(factor_quantile),
         ])
 
     # 将nan改成null
-    df_pl = df_pl.with_columns(pl.col(factor).fill_nan(None))
+    df_pl = df_pl.with_columns(F.fill_nan(None))
 
-    if by_group:
-        return df_pl.group_by(by=[_DATE_, _GROUP_]).map_groups(_func_cs)
+    if group_name is None:
+        return df_pl.group_by(_DATE_).map_groups(_func_cs)
     else:
+        return df_pl.group_by(by=[_DATE_, group_name]).map_groups(_func_cs)
+
+
+def with_factor_top_k(df_pl: pl.DataFrame, factor: str, top_k: int = 10, group_name: Optional[str] = None, factor_quantile: str = _QUANTILE_) -> pl.DataFrame:
+    """前K后K的分组方法。一般用于截面股票数不多无法分位数分层的情况。
+
+    输出范围为0、1、2，分别为做空、对冲、做多
+    输出数量并不等于top_k，
+        - 遇到重复时会出现数量大于top_k，
+        - 遇到top_k>数量/2时，即在做多组又在做空组会划分到对冲组
+
+    Parameters
+    ----------
+    df_pl
+    factor
+    top_k:int
+    group_name
+    factor_quantile
+
+    Returns
+    -------
+    pl.DataFrame
+
+    """
+    F = pl.col(factor)
+
+    def _func_cs(df: pl.DataFrame):
+        return df.with_columns(
+            rank_top(F, top_k).alias(factor_quantile)
+        )
+
+    # 将nan改成null
+    df_pl = df_pl.with_columns(F.fill_nan(None))
+
+    if group_name is None:
         return df_pl.group_by(_DATE_).map_groups(_func_cs)
+    else:
+        return df_pl.group_by(by=[_DATE_, group_name]).map_groups(_func_cs)
 
 
 def with_quantile_tradable(df_pl: pl.DataFrame, factor_quantile: str, next_doji: str = 'NEXT_DOJI') -> pl.DataFrame:
     """是否可以交易，将不可产易的分到其它分组
 
     Parameters
     ----------
@@ -241,7 +295,18 @@
     sorted_indices = np.argsort(eigenvalues)[::-1]
     sorted_eigenvectors = eigenvectors[:, sorted_indices]
 
     # 正交化矩阵
     orthogonal_matrix = np.linalg.qr(sorted_eigenvectors)[0]
 
     return orthogonal_matrix
+
+
+def row_unstack(df_pl: pl.DataFrame, index: Sequence[str], columns: Sequence[str]) -> pd.DataFrame:
+    """一行值堆叠成一个矩阵"""
+    return pd.DataFrame(df_pl.to_numpy().reshape(len(index), len(columns)),
+                        index=index, columns=columns)
+
+
+def index_split_unstack(s: pd.Series, split_by: str = '__'):
+    s.index = pd.MultiIndex.from_tuples(map(lambda x: tuple(x.split(split_by)), s.index))
+    return s.unstack()
```

### Comparing `alphainspect-0.4.3/alphainspect.egg-info/PKG-INFO` & `alphainspect-0.4.4/alphainspect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphainspect
-Version: 0.4.3
+Version: 0.4.4
 Summary: factor performance visualization
 Author-email: wukan <wu-kan@163.com>
 License: MIT License
         
         Copyright (c) 2024 wukan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `alphainspect-0.4.3/pyproject.toml` & `alphainspect-0.4.4/pyproject.toml`

 * *Files identical despite different names*

