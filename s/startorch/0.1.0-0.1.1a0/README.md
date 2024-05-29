# Comparing `tmp/startorch-0.1.0.tar.gz` & `tmp/startorch-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startorch-0.1.0.tar", max compression
+gzip compressed data, was "startorch-0.1.1a0.tar", max compression
```

## Comparing `startorch-0.1.0.tar` & `startorch-0.1.1a0.tar`

### file list

```diff
@@ -1,107 +1,136 @@
--rw-r--r--   0        0        0     1501 2024-03-19 02:21:34.830344 startorch-0.1.0/LICENSE
--rw-r--r--   0        0        0     7031 2024-03-19 02:21:34.830344 startorch-0.1.0/README.md
--rw-r--r--   0        0        0     6488 2024-03-19 02:21:34.882344 startorch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       85 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/__init__.py
--rw-r--r--   0        0        0      357 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/constants.py
--rw-r--r--   0        0        0     3830 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/example/__init__.py
--rw-r--r--   0        0        0     3884 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/example/base.py
--rw-r--r--   0        0        0     7792 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/example/blobs.py
--rw-r--r--   0        0        0     2282 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/example/cache.py
--rw-r--r--   0        0        0     6148 2024-03-19 02:21:34.882344 startorch-0.1.0/src/startorch/example/circles.py
--rw-r--r--   0        0        0    13681 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/friedman.py
--rw-r--r--   0        0        0     5499 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/hypercube.py
--rw-r--r--   0        0        0     5448 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/moons.py
--rw-r--r--   0        0        0     7359 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/regression.py
--rw-r--r--   0        0        0     2453 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/sparse_uncorrelated.py
--rw-r--r--   0        0        0     5097 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/swissroll.py
--rw-r--r--   0        0        0     2687 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/example/timeseries.py
--rw-r--r--   0        0        0       41 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/__init__.py
--rw-r--r--   0        0        0      848 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/sequence/__init__.py
--rw-r--r--   0        0        0     4696 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/sequence/base.py
--rw-r--r--   0        0        0     2011 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/sequence/repeat.py
--rw-r--r--   0        0        0     3462 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/sequence/wave.py
--rw-r--r--   0        0        0      612 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/timeseries/__init__.py
--rw-r--r--   0        0        0     5715 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/timeseries/base.py
--rw-r--r--   0        0        0     2299 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/periodic/timeseries/repeat.py
--rw-r--r--   0        0        0       53 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/__init__.py
--rw-r--r--   0        0        0      307 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/matplotlib/__init__.py
--rw-r--r--   0        0        0     2783 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/matplotlib/feature.py
--rw-r--r--   0        0        0     3856 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/matplotlib/sequence.py
--rw-r--r--   0        0        0      295 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/plotly/__init__.py
--rw-r--r--   0        0        0     2900 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/plotly/feature.py
--rw-r--r--   0        0        0     3760 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/plot/plotly/sequence.py
--rw-r--r--   0        0        0     1582 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/random/__init__.py
--rw-r--r--   0        0        0    33276 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/random/bounded.py
--rw-r--r--   0        0        0     1239 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/random/discrete.py
--rw-r--r--   0        0        0     5300 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/random/infinite.py
--rw-r--r--   0        0        0     9294 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/random/semi_infinite.py
--rw-r--r--   0        0        0    14227 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/__init__.py
--rw-r--r--   0        0        0     4984 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/ar.py
--rw-r--r--   0        0        0     3868 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/base.py
--rw-r--r--   0        0        0     6027 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/categorical.py
--rw-r--r--   0        0        0     9359 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/cauchy.py
--rw-r--r--   0        0        0     2860 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/choice.py
--rw-r--r--   0        0        0     2801 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/constant.py
--rw-r--r--   0        0        0     1821 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/dtype.py
--rw-r--r--   0        0        0    10313 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/exponential.py
--rw-r--r--   0        0        0     7267 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/halfcauchy.py
--rw-r--r--   0        0        0     7121 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/halfnormal.py
--rw-r--r--   0        0        0     2945 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/joining.py
--rw-r--r--   0        0        0     2797 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/linear.py
--rw-r--r--   0        0        0     9708 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/lognormal.py
--rw-r--r--   0        0        0    19835 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/math.py
--rw-r--r--   0        0        0     9400 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/normal.py
--rw-r--r--   0        0        0     2690 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/periodic.py
--rw-r--r--   0        0        0     4684 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/poisson.py
--rw-r--r--   0        0        0     1462 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/range.py
--rw-r--r--   0        0        0     1654 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/sort.py
--rw-r--r--   0        0        0     1909 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/tensor.py
--rw-r--r--   0        0        0    12422 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/time.py
--rw-r--r--   0        0        0     5102 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/trigo.py
--rw-r--r--   0        0        0    12629 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/uniform.py
--rw-r--r--   0        0        0     3674 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/wave.py
--rw-r--r--   0        0        0     2891 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/wiener.py
--rw-r--r--   0        0        0     1097 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/sequence/wrapper.py
--rw-r--r--   0        0        0    11412 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/__init__.py
--rw-r--r--   0        0        0     3422 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/base.py
--rw-r--r--   0        0        0     6112 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/categorical.py
--rw-r--r--   0        0        0     8104 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/cauchy.py
--rw-r--r--   0        0        0     2957 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/choice.py
--rw-r--r--   0        0        0     1352 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/constant.py
--rw-r--r--   0        0        0     1575 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/dtype.py
--rw-r--r--   0        0        0     6304 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/exponential.py
--rw-r--r--   0        0        0     6227 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/halfcauchy.py
--rw-r--r--   0        0        0     6110 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/halfnormal.py
--rw-r--r--   0        0        0     8434 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/lognormal.py
--rw-r--r--   0        0        0    17516 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/math.py
--rw-r--r--   0        0        0     8154 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/normal.py
--rw-r--r--   0        0        0     2838 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/poisson.py
--rw-r--r--   0        0        0     4405 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/trigo.py
--rw-r--r--   0        0        0    10075 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/uniform.py
--rw-r--r--   0        0        0     1096 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/tensor/wrapper.py
--rw-r--r--   0        0        0      596 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/testing.py
--rw-r--r--   0        0        0       39 2024-03-19 02:21:34.886344 startorch-0.1.0/src/startorch/th3rd/__init__.py
--rw-r--r--   0        0        0       48 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/th3rd/iden/__init__.py
--rw-r--r--   0        0        0       53 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/th3rd/iden/data/__init__.py
--rw-r--r--   0        0        0      213 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/th3rd/iden/data/generator/__init__.py
--rw-r--r--   0        0        0     1902 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/th3rd/iden/data/generator/example.py
--rw-r--r--   0        0        0     1354 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/__init__.py
--rw-r--r--   0        0        0     4760 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/base.py
--rw-r--r--   0        0        0     3787 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/choice.py
--rw-r--r--   0        0        0     1949 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/generic.py
--rw-r--r--   0        0        0     2888 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/merge.py
--rw-r--r--   0        0        0     2585 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/mixed.py
--rw-r--r--   0        0        0     3113 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/periodic.py
--rw-r--r--   0        0        0      251 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/utils/__init__.py
--rw-r--r--   0        0        0     3318 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/utils/merge.py
--rw-r--r--   0        0        0     1407 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/timeseries/utils/mixed.py
--rw-r--r--   0        0        0       34 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/__init__.py
--rw-r--r--   0        0        0     1032 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/batch.py
--rw-r--r--   0        0        0     1956 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/conversion.py
--rw-r--r--   0        0        0     2221 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/format.py
--rw-r--r--   0        0        0     3043 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/imports.py
--rw-r--r--   0        0        0     2328 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/seed.py
--rw-r--r--   0        0        0     1131 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/tensor.py
--rw-r--r--   0        0        0     4221 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/validation.py
--rw-r--r--   0        0        0     3326 2024-03-19 02:21:34.890344 startorch-0.1.0/src/startorch/utils/weight.py
--rw-r--r--   0        0        0     8452 1970-01-01 00:00:00.000000 startorch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-29 07:03:02.079477 startorch-0.1.1a0/LICENSE
+-rw-r--r--   0        0        0     7243 2024-05-29 07:03:02.079477 startorch-0.1.1a0/README.md
+-rw-r--r--   0        0        0     6852 2024-05-29 07:03:02.147477 startorch-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/__init__.py
+-rw-r--r--   0        0        0      357 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/constants.py
+-rw-r--r--   0        0        0     4417 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/__init__.py
+-rw-r--r--   0        0        0     3825 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/base.py
+-rw-r--r--   0        0        0     7704 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/blobs.py
+-rw-r--r--   0        0        0     2273 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/cache.py
+-rw-r--r--   0        0        0     6176 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/circles.py
+-rw-r--r--   0        0        0     2404 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/concatenate.py
+-rw-r--r--   0        0        0    13735 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/friedman.py
+-rw-r--r--   0        0        0     5421 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/hypercube.py
+-rw-r--r--   0        0        0     5456 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/moons.py
+-rw-r--r--   0        0        0     7291 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/regression.py
+-rw-r--r--   0        0        0     2462 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/sparse_uncorrelated.py
+-rw-r--r--   0        0        0     5099 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/swissroll.py
+-rw-r--r--   0        0        0     2268 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/tensor.py
+-rw-r--r--   0        0        0     2722 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/timeseries.py
+-rw-r--r--   0        0        0     2351 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/transform.py
+-rw-r--r--   0        0        0     2057 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/example/vanilla.py
+-rw-r--r--   0        0        0       39 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/integration/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/integration/iden/__init__.py
+-rw-r--r--   0        0        0       53 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/integration/iden/data/__init__.py
+-rw-r--r--   0        0        0      219 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/integration/iden/data/generator/__init__.py
+-rw-r--r--   0        0        0     1902 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/integration/iden/data/generator/example.py
+-rw-r--r--   0        0        0       41 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/__init__.py
+-rw-r--r--   0        0        0      848 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/sequence/__init__.py
+-rw-r--r--   0        0        0     4639 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/sequence/base.py
+-rw-r--r--   0        0        0     2003 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/sequence/repeat.py
+-rw-r--r--   0        0        0     3433 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/sequence/wave.py
+-rw-r--r--   0        0        0      612 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/timeseries/__init__.py
+-rw-r--r--   0        0        0     5800 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/timeseries/base.py
+-rw-r--r--   0        0        0     2354 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/periodic/timeseries/repeat.py
+-rw-r--r--   0        0        0       53 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/plot/__init__.py
+-rw-r--r--   0        0        0      307 2024-05-29 07:03:02.147477 startorch-0.1.1a0/src/startorch/plot/matplotlib/__init__.py
+-rw-r--r--   0        0        0     2744 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/plot/matplotlib/feature.py
+-rw-r--r--   0        0        0     3700 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/plot/matplotlib/sequence.py
+-rw-r--r--   0        0        0      295 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/plot/plotly/__init__.py
+-rw-r--r--   0        0        0     2861 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/plot/plotly/feature.py
+-rw-r--r--   0        0        0     3588 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/plot/plotly/sequence.py
+-rw-r--r--   0        0        0     1582 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/random/__init__.py
+-rw-r--r--   0        0        0    32543 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/random/bounded.py
+-rw-r--r--   0        0        0     1210 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/random/discrete.py
+-rw-r--r--   0        0        0     5165 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/random/infinite.py
+-rw-r--r--   0        0        0     9093 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/random/semi_infinite.py
+-rw-r--r--   0        0        0    14431 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/__init__.py
+-rw-r--r--   0        0        0     4925 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/ar.py
+-rw-r--r--   0        0        0     3821 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/base.py
+-rw-r--r--   0        0        0     5978 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/categorical.py
+-rw-r--r--   0        0        0     9223 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/cauchy.py
+-rw-r--r--   0        0        0     2851 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/choice.py
+-rw-r--r--   0        0        0     3022 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/constant.py
+-rw-r--r--   0        0        0     1823 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/dtype.py
+-rw-r--r--   0        0        0    10187 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/exponential.py
+-rw-r--r--   0        0        0     7191 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/halfcauchy.py
+-rw-r--r--   0        0        0     7045 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/halfnormal.py
+-rw-r--r--   0        0        0     2916 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/joining.py
+-rw-r--r--   0        0        0     2768 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/linear.py
+-rw-r--r--   0        0        0     9572 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/lognormal.py
+-rw-r--r--   0        0        0     4817 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/markov.py
+-rw-r--r--   0        0        0    19689 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/math.py
+-rw-r--r--   0        0        0     9263 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/normal.py
+-rw-r--r--   0        0        0     2671 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/periodic.py
+-rw-r--r--   0        0        0     4626 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/poisson.py
+-rw-r--r--   0        0        0     1453 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/range.py
+-rw-r--r--   0        0        0     1633 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/sort.py
+-rw-r--r--   0        0        0     1890 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/tensor.py
+-rw-r--r--   0        0        0    12323 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/time.py
+-rw-r--r--   0        0        0     5108 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/trigo.py
+-rw-r--r--   0        0        0    12457 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/uniform.py
+-rw-r--r--   0        0        0     3635 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/wave.py
+-rw-r--r--   0        0        0     2843 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/wiener.py
+-rw-r--r--   0        0        0     1087 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/sequence/wrapper.py
+-rw-r--r--   0        0        0    11412 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/__init__.py
+-rw-r--r--   0        0        0     3385 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/base.py
+-rw-r--r--   0        0        0     6054 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/categorical.py
+-rw-r--r--   0        0        0     7988 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/cauchy.py
+-rw-r--r--   0        0        0     2948 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/choice.py
+-rw-r--r--   0        0        0     1333 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/constant.py
+-rw-r--r--   0        0        0     1577 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/dtype.py
+-rw-r--r--   0        0        0     6248 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/exponential.py
+-rw-r--r--   0        0        0     6171 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/halfcauchy.py
+-rw-r--r--   0        0        0     6054 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/halfnormal.py
+-rw-r--r--   0        0        0     8318 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/lognormal.py
+-rw-r--r--   0        0        0    17369 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/math.py
+-rw-r--r--   0        0        0     8038 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/normal.py
+-rw-r--r--   0        0        0     2820 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/poisson.py
+-rw-r--r--   0        0        0      924 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/transformer/__init__.py
+-rw-r--r--   0        0        0     3774 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/transformer/base.py
+-rw-r--r--   0        0        0     1396 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/transformer/identity.py
+-rw-r--r--   0        0        0     2674 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/transformer/math.py
+-rw-r--r--   0        0        0     4411 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/trigo.py
+-rw-r--r--   0        0        0     9941 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/uniform.py
+-rw-r--r--   0        0        0     1086 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/tensor/wrapper.py
+-rw-r--r--   0        0        0      596 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/testing.py
+-rw-r--r--   0        0        0     1847 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/__init__.py
+-rw-r--r--   0        0        0     4833 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/base.py
+-rw-r--r--   0        0        0     3910 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/choice.py
+-rw-r--r--   0        0        0     2541 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/concatenate.py
+-rw-r--r--   0        0        0     2936 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/merge.py
+-rw-r--r--   0        0        0     2580 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/mixed.py
+-rw-r--r--   0        0        0     3131 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/periodic.py
+-rw-r--r--   0        0        0     2078 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/sequence.py
+-rw-r--r--   0        0        0     2175 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/tensor.py
+-rw-r--r--   0        0        0      251 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/utils/__init__.py
+-rw-r--r--   0        0        0     3299 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/utils/merge.py
+-rw-r--r--   0        0        0     1388 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/timeseries/utils/mixed.py
+-rw-r--r--   0        0        0     2522 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/__init__.py
+-rw-r--r--   0        0        0     5943 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/base.py
+-rw-r--r--   0        0        0     2111 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/exponential.py
+-rw-r--r--   0        0        0     1451 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/identity.py
+-rw-r--r--   0        0        0     2151 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/lut.py
+-rw-r--r--   0        0        0     3830 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/math.py
+-rw-r--r--   0        0        0     1974 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/poisson.py
+-rw-r--r--   0        0        0     2219 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/sequential.py
+-rw-r--r--   0        0        0     7782 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/trigo.py
+-rw-r--r--   0        0        0     1348 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transformer/utils.py
+-rw-r--r--   0        0        0     1482 2024-05-29 07:03:02.151477 startorch-0.1.1a0/src/startorch/transition/__init__.py
+-rw-r--r--   0        0        0     3976 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/base.py
+-rw-r--r--   0        0        0     1788 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/diag.py
+-rw-r--r--   0        0        0     1929 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/mask.py
+-rw-r--r--   0        0        0     1914 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/normalize.py
+-rw-r--r--   0        0        0     1544 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/tensor.py
+-rw-r--r--   0        0        0     2186 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/transition/transform.py
+-rw-r--r--   0        0        0       34 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/__init__.py
+-rw-r--r--   0        0        0     1013 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/batch.py
+-rw-r--r--   0        0        0     1929 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/conversion.py
+-rw-r--r--   0        0        0     2183 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/format.py
+-rw-r--r--   0        0        0     3049 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/imports.py
+-rw-r--r--   0        0        0     3299 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/mask.py
+-rw-r--r--   0        0        0     2291 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/seed.py
+-rw-r--r--   0        0        0     2331 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/tensor.py
+-rw-r--r--   0        0        0     4106 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/validation.py
+-rw-r--r--   0        0        0     3308 2024-05-29 07:03:02.155477 startorch-0.1.1a0/src/startorch/utils/weight.py
+-rw-r--r--   0        0        0     8758 1970-01-01 00:00:00.000000 startorch-0.1.1a0/PKG-INFO
```

### Comparing `startorch-0.1.0/LICENSE` & `startorch-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/README.md` & `startorch-0.1.1a0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # startorch
 
 <p align="center">
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="CI" src="https://github.com/durandtibo/startorch/workflows/CI/badge.svg">
     </a>
-    <a href="https://durandtibo.github.io/startorch/">
-        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation/badge.svg">
-    </a>
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="Nightly Tests" src="https://github.com/durandtibo/startorch/workflows/Nightly%20Tests/badge.svg">
     </a>
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="Nightly Package Tests" src="https://github.com/durandtibo/startorch/workflows/Nightly%20Package%20Tests/badge.svg">
     </a>
     <br/>
+    <a href="https://durandtibo.github.io/startorch/">
+        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation%20(stable)/badge.svg">
+    </a>
+    <a href="https://durandtibo.github.io/startorch/">
+        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation%20(unstable)/badge.svg">
+    </a>
+    <br/>
     <a href="https://codecov.io/gh/durandtibo/startorch">
         <img alt="Codecov" src="https://codecov.io/gh/durandtibo/startorch/branch/main/graph/badge.svg">
     </a>
     <a href="https://codeclimate.com/github/durandtibo/startorch/maintainability">
         <img src="https://api.codeclimate.com/v1/badges/05a12c503bf3be80a00b/maintainability" />
     </a>
     <a href="https://codeclimate.com/github/durandtibo/startorch/test_coverage">
@@ -94,15 +98,15 @@
 - [API stability](#api-stability)
 - [License](#license)
 
 ## Dependencies
 
 | `startorch` | `batchtensor`  | `coola`      | `objectory`  | `numpy`       | `torch`      | `iden`<sup>*</sup> | `matplotlib`<sup>*</sup> | `plotly`<sup>*</sup> | `python`      |
 |-------------|----------------|--------------|--------------|---------------|--------------|--------------------|--------------------------|----------------------|---------------|
-| `main`      | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
+| `main`      | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.23,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
 | `0.1.0`     | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
 
 <sup>*</sup> indicates an optional dependency
 
 <details>
     <summary>older versions</summary>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 # startorch
-           _[_C_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
+                  _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
+                        _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_0_5_a_1_2_c_5_0_3_b_f_3_b_e_8_0_a_0_0_b_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_0_5_a_1_2_c_5_0_3_b_f_3_b_e_8_0_a_0_0_b_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_M_o_n_t_h_l_y_ _d_o_w_n_l_o_a_d_s_]
 --- ## Overview Collecting datasets to train Machine Learning models can be
@@ -22,15 +23,15 @@
 - [Documentation](https://durandtibo.github.io/startorch/) - [Installation]
 (https://durandtibo.github.io/startorch/get_started/) - [Contributing]
 (#contributing) - [API stability](#api-stability) - [License](#license) ##
 Dependencies | `startorch` | `batchtensor` | `coola` | `objectory` | `numpy` |
 `torch` | `iden`* | `matplotlib`* | `plotly`* | `python` | |-------------|-----
 -----------|--------------|--------------|---------------|--------------|------
 --------------|--------------------------|----------------------|--------------
--| | `main` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
+-| | `main` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.23,<2.0` |
 `>=2.0,<3.0` | `>=0.0.2,<0.1` | `>=3.6,<4.0` | `>=5.0,<6.0` | `>=3.9,<3.12` | |
 `0.1.0` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
 `>=2.0,<3.0` | `>=0.0.2,<0.1` | `>=3.6,<4.0` | `>=5.0,<6.0` | `>=3.9,<3.12` | *
 indicates an optional dependency older versions | `startorch` | `coola` |
 `objectory` | `redcat` | `torch` | `matplotlib`* | `plotly`* | `python` | |----
 ---------|--------------------|------------------|--------------------|--------
 ------|--------------------------|----------------------|---------------| |
```

### Comparing `startorch-0.1.0/pyproject.toml` & `startorch-0.1.1a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "startorch"
-version = "0.1.0"
+version = "0.1.1a0"
 description = "synthetic time-series generator in PyTorch"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/startorch"
 repository = "https://github.com/durandtibo/startorch"
 keywords = ["synthetic", "time-series", "pytorch"]
 license = "BSD-3-Clause"
 
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -28,18 +28,21 @@
     { include = "startorch", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
 batchtensor = ">=0.0.2,<0.1"
 coola = ">=0.2,<1.0"
-numpy = ">=1.21,<2.0"
+numpy = ">=1.23,<2.0"
 objectory = ">=0.1,<1.0"
 python = ">=3.9,<3.13"
-torch = ">=2.0,<3.0"
+torch = [
+    { version = ">=2.0,<2.3", markers="sys_platform == 'darwin' and platform_machine != 'arm64'" },
+    { version = ">=2.0,<3.0" }
+]
 
 # Optional dependencies
 iden = { version = ">=0.0.2,<0.1", optional = true }
 matplotlib = { version = ">=3.6,<4.0", optional = true }
 plotly = { version = ">=5.0,<6.0", optional = true }
 
 [tool.poetry.extras]
@@ -48,32 +51,34 @@
 [tool.poetry.group.exp]
 optional = true
 
 [tool.poetry.group.exp.dependencies]
 jupyterlab = "^4.0"
 safetensors = ">=0.4,<1.0"
 seaborn = "^0.13"
+scikit-learn = "^1.4"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
+mike = "^2.1"
 mkdocs-material = "^9.5"
-mkdocstrings = "^0.24"
+mkdocstrings = { extras = ["python"], version = "^0.25" }
 
 [tool.poetry.group.dev.dependencies]
-black = ">=24.3"
-coverage = { extras = ["toml"], version = "^7.4" }
+black = ">=24.4"
+coverage = { extras = ["toml"], version = "^7.5" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
-pre-commit = "^3.6"
-pygments = "^2.17"
-pytest = "^8.1"
-pytest-cov = "^4.1"
+pre-commit = "^3.7"
+pygments = "^2.18"
+pytest = "^8.2"
+pytest-cov = "^5.0"
 pytest-timeout = "^2.3"
-ruff = ">=0.3.0,<1.0"
+ruff = ">=0.4.0,<1.0"
 xdoctest = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
@@ -112,29 +117,27 @@
 [tool.docformatter]
 recursive = true
 wrap-summaries = 72
 wrap-descriptions = 72
 syntax = "google"
 
 [tool.ruff]
-line-length = 100
-target-version = "py39"
-src = ["src"]
-
 # List of rules: https://docs.astral.sh/ruff/rules/
 lint.select = [
     "A", # builtins
     "ANN", # annotations
     "ARG", # flake8-unused-arguments
     "B", # bugbear
     "BLE", # flake8-blind-except
     "C4", # flake8-comprehensions
     "D", # pydocstyle
+    "DTZ", # flake8-datetimez
     "E", # pycodestyle (Error)
     "EM", # flake8-errmsg
+    "EXE", # flake8-executable
     "F", # pyflakes
     "FA", # flake8-future-annotations
     "FURB", # refurb
     "ICN", # flake8-import-conventions
     "INP", # flake8-no-pep420
     "ISC", # flake8-implicit-str-concat
     "LOG", # logging
@@ -146,14 +149,15 @@
     "PL", # Pylint
     "PT", # flake8-pytest-style
     "PTH", # pathlib
     "PYI", # flake8-pyi
     "Q", # flake8-quotes
     "RET", # flake8-return
     "RSE", # flake8-raise
+    "RUF", # Ruff-specific rules
     "S", # flake8-bandit
     "SIM", # flake8-simplify
     "T20", # flake8-print
     "TCH", # flake8-type-checking
     "TD", # flake8-todos
     "TID", # flake8-tidy-imports
     "TRY", # tryceratops
@@ -184,16 +188,18 @@
     "A",
     "ANN",
     "ARG",
     "B",
     "BLE",
     "C4",
     "D",
+    "DTZ",
     "E",
     "EM",
+    "EXE",
     "F",
     "FA",
     "FURB",
     "ICN",
     "INP",
     "ISC",
     "LOG",
@@ -204,14 +210,15 @@
     "PL",
     "PT",
     "PTH",
     "PYI",
     "Q",
     "RET",
     "RSE",
+    "RUF",
     "S",
     "SIM",
     "T20",
     "TCH",
     "TD",
     "TID",
     "TRY",
@@ -240,21 +247,28 @@
     "node_modules",
     "venv",
 ]
 
 # Enable on top of the Google convention.
 lint.extend-select = ["D400", "D401", "D404"]
 
+line-length = 100
+target-version = "py39"
+src = ["src"]
+
 [tool.ruff.lint.per-file-ignores]
 # Ignore all directories named `tests`.
 "tests/**" = [
     "D", # pydocstyle
     "PL", # Pylint
     "S101", # flake8-bandit
 ]
+"**.ipynb" = [
+    "T20", # flake8-print
+]
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `startorch-0.1.0/src/startorch/example/__init__.py` & `startorch-0.1.1a0/src/startorch/example/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,36 @@
     "BaseExampleGenerator",
     "BlobsClassification",
     "BlobsClassificationExampleGenerator",
     "Cache",
     "CacheExampleGenerator",
     "CirclesClassification",
     "CirclesClassificationExampleGenerator",
+    "Concatenate",
+    "ConcatenateExampleGenerator",
     "Friedman1Regression",
     "Friedman1RegressionExampleGenerator",
     "Friedman2Regression",
     "Friedman2RegressionExampleGenerator",
     "Friedman3Regression",
     "Friedman3RegressionExampleGenerator",
     "HypercubeClassification",
     "HypercubeClassificationExampleGenerator",
     "LinearRegression",
     "LinearRegressionExampleGenerator",
     "MoonsClassification",
     "MoonsClassificationExampleGenerator",
     "SwissRoll",
     "SwissRollExampleGenerator",
+    "TensorExampleGenerator",
     "TimeSeries",
     "TimeSeriesExampleGenerator",
+    "Transform",
+    "TransformExampleGenerator",
+    "VanillaExampleGenerator",
     "is_example_generator_config",
     "make_blobs_classification",
     "make_circles_classification",
     "make_friedman1_regression",
     "make_friedman2_regression",
     "make_friedman3_regression",
     "make_hypercube_classification",
@@ -53,14 +59,16 @@
 from startorch.example.cache import CacheExampleGenerator
 from startorch.example.cache import CacheExampleGenerator as Cache
 from startorch.example.circles import CirclesClassificationExampleGenerator
 from startorch.example.circles import (
     CirclesClassificationExampleGenerator as CirclesClassification,
 )
 from startorch.example.circles import make_circles_classification
+from startorch.example.concatenate import ConcatenateExampleGenerator
+from startorch.example.concatenate import ConcatenateExampleGenerator as Concatenate
 from startorch.example.friedman import Friedman1RegressionExampleGenerator
 from startorch.example.friedman import (
     Friedman1RegressionExampleGenerator as Friedman1Regression,
 )
 from startorch.example.friedman import Friedman2RegressionExampleGenerator
 from startorch.example.friedman import (
     Friedman2RegressionExampleGenerator as Friedman2Regression,
@@ -89,9 +97,13 @@
     LinearRegressionExampleGenerator as LinearRegression,
 )
 from startorch.example.regression import make_linear_regression
 from startorch.example.sparse_uncorrelated import make_sparse_uncorrelated_regression
 from startorch.example.swissroll import SwissRollExampleGenerator
 from startorch.example.swissroll import SwissRollExampleGenerator as SwissRoll
 from startorch.example.swissroll import make_swiss_roll
+from startorch.example.tensor import TensorExampleGenerator
 from startorch.example.timeseries import TimeSeriesExampleGenerator
 from startorch.example.timeseries import TimeSeriesExampleGenerator as TimeSeries
+from startorch.example.transform import TransformExampleGenerator
+from startorch.example.transform import TransformExampleGenerator as Transform
+from startorch.example.vanilla import VanillaExampleGenerator
```

### Comparing `startorch-0.1.0/src/startorch/example/base.py` & `startorch-0.1.1a0/src/startorch/example/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
 class BaseExampleGenerator(Generic[T], ABC, metaclass=AbstractFactory):
     r"""Define the base class to generate examples.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import HypercubeClassification
     >>> generator = HypercubeClassification(num_classes=5, feature_size=6)
     >>> generator
     HypercubeClassificationExampleGenerator(num_classes=5, feature_size=6, noise_std=0.2)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -47,16 +48,16 @@
     @abstractmethod
     def generate(
         self, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
         r"""Generate a batch of examples.
 
         Args:
-            batch_size: Specifies the batch size.
-            rng: Specifies an optional random number generator.
+            batch_size: The batch size.
+            rng: An optional random number generator.
 
         Returns:
             A batch of examples.
 
         Example usage:
 
         ```pycon
@@ -76,15 +77,15 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration for a
             ``BaseExampleGenerator`` object.
 
     Example usage:
 
@@ -96,29 +97,29 @@
     """
     return is_object_config(config, BaseExampleGenerator)
 
 
 def setup_example_generator(
     generator: BaseExampleGenerator | dict,
 ) -> BaseExampleGenerator:
-    r"""Set up a time series generator.
+    r"""Set up an example generator.
 
     The time series generator is instantiated from its configuration
     by using the ``BaseExampleGenerator`` factory function.
 
     Args:
-        generator: Specifies a time series generator or its
-            configuration.
+        generator: An example generator or its configuration.
 
     Returns:
-        A time series generator.
+        An example generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import setup_example_generator
     >>> generator = setup_example_generator(
     ...     {"_target_": "startorch.example.HypercubeClassification"}
     ... )
     >>> generator
     HypercubeClassificationExampleGenerator(num_classes=50, feature_size=64, noise_std=0.2)
```

### Comparing `startorch-0.1.0/src/startorch/example/blobs.py` & `startorch-0.1.1a0/src/startorch/example/blobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,28 +22,29 @@
     r"""Implement a binary classification example generator where the
     data are generated from isotropic Gaussian blobs.
 
     The implementation is based on
     https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_blobs.html
 
     Args:
-        centers: Specifies the cluster centers used to generate the
+        centers: The cluster centers used to generate the
             examples. It must be a float tensor of shape
             ``(num_clusters, feature_size)``.
-        cluster_std: Specifies the standard deviation of the clusters.
+        cluster_std: The standard deviation of the clusters.
             It must be a float tensor of shape
             ``(num_clusters, feature_size)``.
 
     Raises:
         TypeError: if one of the parameters has an invalid type.
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.example import BlobsClassification
     >>> generator = BlobsClassification(torch.rand(5, 4))
     >>> generator
     BlobsClassificationExampleGenerator(num_clusters=5, feature_size=4)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
@@ -110,17 +111,17 @@
         feature_size: int = 2,
         random_seed: int = 17532042831661189422,
     ) -> BlobsClassificationExampleGenerator:
         r"""Instantiate a ``BlobsClassificationExampleGenerator`` where
         the centers are sampled from a uniform distribution.
 
         Args:
-            num_clusters: Specifies the number of clusters.
-            feature_size: Specifies the feature size.
-            random_seed: Specifies the random seed used to generate
+            num_clusters: The number of clusters.
+            feature_size: The feature size.
+            random_seed: The random seed used to generate
                 the cluster centers.
 
         Returns:
             An instantiated example generator.
 
         Example usage:
 
@@ -155,22 +156,22 @@
     r"""Generate a classification dataset where the data are gnerated
     from isotropic Gaussian blobs for clustering.
 
     The implementation is based on
     https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_blobs.html
 
     Args:
-        num_examples: Specifies the number of examples.
-        centers: Specifies the cluster centers used to generate the
+        num_examples: The number of examples.
+        centers: The cluster centers used to generate the
             examples. It must be a float tensor of shape
             ``(num_clusters, feature_size)``.
-        cluster_std: Specifies the standard deviation of the clusters.
+        cluster_std: The standard deviation of the clusters.
             It must be a float tensor of shape
             ``(num_clusters, feature_size)``.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type long and
@@ -179,14 +180,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.example import make_blobs_classification
     >>> batch = make_blobs_classification(num_examples=10, centers=torch.rand(5, 2))
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
```

### Comparing `startorch-0.1.0/src/startorch/example/cache.py` & `startorch-0.1.1a0/src/startorch/example/cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 class CacheExampleGenerator(BaseExampleGenerator):
     r"""Implement an example generator that caches the last batch and
     returns it everytime a batch is generated.
 
     A new batch is generated only if the batch size changes.
 
     Args:
-        generator: Specifies the example generator or its
+        generator: The example generator or its
             configuration.
         deepcopy: If ``True``, the cached batch is deepcopied before to
             be return.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import Cache, SwissRoll
     >>> generator = Cache(SwissRoll())
     >>> generator
     CacheExampleGenerator(
       (generator): SwissRollExampleGenerator(noise_std=0.0, spin=1.5, hole=False)
       (deepcopy): False
     )
```

### Comparing `startorch-0.1.0/src/startorch/example/circles.py` & `startorch-0.1.1a0/src/startorch/example/circles.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,32 +19,33 @@
 
 class CirclesClassificationExampleGenerator(BaseExampleGenerator):
     r"""Implements a binary classification example generator where the
     data are generated with a large circle containing a smaller circle
     in 2d.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html
+    [`sklearn.datasets.make_circles`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html).
 
     Args:
         shuffle: If ``True``, the examples are shuffled.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        factor: Specifies the scale factor between inner and outer
+        factor: The scale factor between inner and outer
             circle in the range ``[0, 1)``.
-        ratio: Specifies the ratio between the number of examples in
+        ratio: The ratio between the number of examples in
             outer circle and inner circle.
 
     Raises:
-        TypeError or RuntimeError if one of the parameters is not
-            valid.
+        TypeError: if one of the parameters is not valid.
+        RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import CirclesClassification
     >>> generator = CirclesClassification()
     >>> generator
     CirclesClassificationExampleGenerator(shuffle=True, noise_std=0.0, factor=0.8, ratio=0.5)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -112,26 +113,26 @@
     ratio: float = 0.5,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate a binary classification dataset where the data are
     generated with a large circle containing a smaller circle in 2d.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html
+    [`sklearn.datasets.make_circles`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html).
 
     Args:
-        num_examples: Specifies the number of examples.
+        num_examples: The number of examples.
         shuffle: If ``True``, the examples are shuffled.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        factor: Specifies the scale factor between inner and outer
+        factor: The scale factor between inner and outer
             circle in the range ``[0, 1)``.
-        ratio: Specifies the ratio between the number of examples in
+        ratio: The ratio between the number of examples in
             outer circle and inner circle.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, 2)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type long and
@@ -140,14 +141,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_circles_classification
     >>> batch = make_circles_classification(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/friedman.py` & `startorch-0.1.1a0/src/startorch/example/friedman.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,30 +22,31 @@
 from startorch.utils.validation import check_feature_size, check_num_examples, check_std
 
 
 class Friedman1RegressionExampleGenerator(BaseExampleGenerator):
     r"""Implement the "Friedman #1" regression example generator.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman1.html
+    [`sklearn.datasets.make_friedman1`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman1.html).
 
     Args:
-        feature_size: Specifies the feature size. The feature size has
+        feature_size: The feature size. The feature size has
             to be greater than or equal to 5. Out of all features,
             only 5 are actually used to compute the targets.
             The remaining features are independent of targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import Friedman1Regression
     >>> generator = Friedman1Regression(feature_size=6)
     >>> generator
     Friedman1RegressionExampleGenerator(feature_size=6, noise_std=0.0)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -88,31 +89,32 @@
         )
 
 
 class Friedman2RegressionExampleGenerator(BaseExampleGenerator):
     r"""Implement the "Friedman #2" regression example generator.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman2.html
+    [`sklearn.datasets.make_friedman2`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman2.html).
 
     Args:
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
             The feature size has to be greater than or equal to 4.
             Out of all features, only 4 are actually used to compute
             the targets. The remaining features are independent of
             targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import Friedman2Regression
     >>> generator = Friedman2Regression(feature_size=6)
     >>> generator
     Friedman2RegressionExampleGenerator(feature_size=6, noise_std=0.0)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -155,31 +157,32 @@
         )
 
 
 class Friedman3RegressionExampleGenerator(BaseExampleGenerator):
     r"""Implement the "Friedman #3" regression example generator.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman3.html
+    [`sklearn.datasets.make_friedman3`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman3.html).
 
     Args:
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
             The feature size has to be greater than or equal to 4.
             Out of all features, only 4 are actually used to compute
             the targets. The remaining features are independent of
             targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import Friedman3Regression
     >>> generator = Friedman3Regression(feature_size=6)
     >>> generator
     Friedman3RegressionExampleGenerator(feature_size=6, noise_std=0.0)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -227,25 +230,25 @@
     feature_size: int = 10,
     noise_std: float = 0.0,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate the "Friedman #1" regression data.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman1.html
+    [`sklearn.datasets.make_friedman1`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman1.html).
 
     Args:
-        num_examples: Specifies the number of examples.
-        feature_size: Specifies the feature size. The feature size has
+        num_examples: The number of examples.
+        feature_size: The feature size. The feature size has
             to be greater than or equal to 5. Out of all features,
             only 5 are actually used to compute the targets.
             The remaining features are independent of targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -254,14 +257,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_friedman1_regression
     >>> batch = make_friedman1_regression(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
@@ -286,26 +290,26 @@
     feature_size: int = 4,
     noise_std: float = 0.0,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate the "Friedman #2" regression data.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman2.html
+    [`sklearn.datasets.make_friedman2`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman2.html).
 
     Args:
-        num_examples: Specifies the number of examples.
-        feature_size: Specifies the feature size.
+        num_examples: The number of examples.
+        feature_size: The feature size.
             The feature size has to be greater than or equal to 4.
             Out of all features, only 4 are actually used to compute
             the targets. The remaining features are independent of
             targets.
-        noise_std: Specifies the standard deviation
+        noise_std: The standard deviation
             of the Gaussian noise.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -314,14 +318,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_friedman2_regression
     >>> batch = make_friedman2_regression(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
@@ -350,26 +355,26 @@
     feature_size: int = 4,
     noise_std: float = 0.0,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate the "Friedman #3" regression problem.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman3.html
+    [`sklearn.datasets.make_friedman3`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_friedman3.html).
 
     Args:
-        num_examples: Specifies the number of examples.
-        feature_size: Specifies the feature size.
+        num_examples: The number of examples.
+        feature_size: The feature size.
             The feature size has to be greater than or equal to 4.
             Out of all features, only 4 are actually used to compute
             the targets. The remaining features are independent of
             targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        generator: Specifies an optional random number generator.
+        generator: An optional random number generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -378,14 +383,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_friedman3_regression
     >>> batch = make_friedman3_regression(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/hypercube.py` & `startorch-0.1.1a0/src/startorch/example/hypercube.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,26 +23,27 @@
 
     The data are generated by using a hypercube. The targets are some
     vertices of the hypercube. Each input feature is a 1-hot
     representation of the target plus a Gaussian noise. These data can
     be used for a multi-class classification task.
 
     Args:
-        num_classes: Specifies the number of classes.
-        feature_size: Specifies the feature size. The feature size has
+        num_classes: The number of classes.
+        feature_size: The feature size. The feature size has
             to be greater than the number of classes.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import HypercubeClassification
     >>> generator = HypercubeClassification(num_classes=5, feature_size=6)
     >>> generator
     HypercubeClassificationExampleGenerator(num_classes=5, feature_size=6, noise_std=0.2)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -112,21 +113,21 @@
 
     The data are generated by using a hypercube. The targets are some
     vertices of the hypercube. Each input feature is a 1-hot
     representation of the target plus a Gaussian noise. These data can
     be used for a multi-class classification task.
 
     Args:
-        num_examples: Specifies the number of examples.
-        num_classes: Specifies the number of classes.
-        feature_size: Specifies the feature size. The feature size has
+        num_examples: The number of examples.
+        num_classes: The number of classes.
+        feature_size: The feature size. The feature size has
             to be greater than the number of classes.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``torch.Tensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``torch.Tensor`` of type long and
@@ -135,14 +136,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example.hypercube import make_hypercube_classification
     >>> batch = make_hypercube_classification(num_examples=10, num_classes=5, feature_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/moons.py` & `startorch-0.1.1a0/src/startorch/example/moons.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,31 @@
 
 class MoonsClassificationExampleGenerator(BaseExampleGenerator):
     r"""Implements a binary classification example generator where the
     data are generated with a large circle containing a smaller circle
     in 2d.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_circles.html
+    [`sklearn.datasets.make_moons`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_moons.html).
 
     Args:
         shuffle: If ``True``, the examples are shuffled.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        ratio: Specifies the ratio between the number of examples in
+        ratio: The ratio between the number of examples in
             outer circle and inner circle.
 
     Raises:
         TypeError: if one of the parameters has an invalid type.
         RuntimeError: if one of the parameters has an invalid value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import MoonsClassification
     >>> generator = MoonsClassification()
     >>> generator
     MoonsClassificationExampleGenerator(shuffle=True, noise_std=0.0, ratio=0.5)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -94,24 +95,24 @@
     ratio: float = 0.5,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate a binary classification dataset where the data are two
     interleaving half circles in 2d.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_moons.html
+    [`sklearn.datasets.make_moons`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_moons.html).
 
     Args:
-        num_examples: Specifies the number of examples.
+        num_examples: The number of examples.
         shuffle: If ``True``, the examples are shuffled.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        ratio: Specifies the ratio between the number of examples in
+        ratio: The ratio between the number of examples in
             outer circle and inner circle.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, 2)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type long and
@@ -120,14 +121,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_moons_classification
     >>> batch = make_moons_classification(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/regression.py` & `startorch-0.1.1a0/src/startorch/example/regression.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 
 
 class LinearRegressionExampleGenerator(BaseExampleGenerator):
     r"""Implement a regression example generator where the data are
     generated with an underlying linear model.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html
+    [`sklearn.datasets.make_regression`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_regression.html).
 
     Args:
-        weights: Specifies the linear weights in the underlying linear
+        weights: The linear weights in the underlying linear
             model. It must be a float tensor of shape
             ``(feature_size,)``.
-        bias: Specifies the bias term in the underlying linear model.
-        noise_std: Specifies the standard deviation of the Gaussian
+        bias: The bias term in the underlying linear model.
+        noise_std: The standard deviation of the Gaussian
             noise.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import LinearRegression
     >>> generator = LinearRegression.create_uniform_weights()
     >>> generator
     LinearRegressionExampleGenerator(feature_size=100, bias=0.0, noise_std=0.0)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -138,22 +139,22 @@
     an underlying linear model.
 
     The features are sampled from a Normal distribution.
     Then, the targets are generated by applying a random linear
     regression model.
 
     Args:
-        weights: Specifies the linear weights in the underlying linear
+        weights: The linear weights in the underlying linear
             model. It must be a float tensor of shape
             ``(feature_size,)``.
-        bias: Specifies the bias term in the underlying linear model.
-        num_examples: Specifies the number of examples to generate.
-        noise_std: Specifies the standard deviation of the Gaussian
+        bias: The bias term in the underlying linear model.
+        num_examples: The number of examples to generate.
+        noise_std: The standard deviation of the Gaussian
             noise.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A dictionary with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -162,14 +163,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_linear_regression
     >>> batch = make_linear_regression(weights=torch.rand(10), num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
@@ -195,27 +197,28 @@
 
     The weights of the informative features are sampled from a uniform
     distribution. The other weights are set to 0.
     This function was designed to be used with
     ``make_normal_regression``.
 
     Args:
-        feature_size: Specifies the feature size i.e. the number of
+        feature_size: The feature size i.e. the number of
             features.
-        informative_feature_size: Specifies the number of informative
+        informative_feature_size: The number of informative
             features.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         The generated weights as a float tensor of shape
             ``(feature_size,)``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example.regression import get_uniform_weights
     >>> weights = get_uniform_weights(feature_size=10, informative_feature_size=5)
     >>> weights
     tensor([...])
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/sparse_uncorrelated.py` & `startorch-0.1.1a0/src/startorch/example/sparse_uncorrelated.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,25 @@
     noise_std: float = 0.0,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate a random regression problem with sparse uncorrelated
     design.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_sparse_uncorrelated.html
+    [`sklearn.datasets.make_sparse_uncorrelated`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_sparse_uncorrelated.html).
 
     Args:
-        num_examples: Specifies the number of examples.
-        feature_size: Specifies the feature size. The feature size has
+        num_examples: The number of examples.
+        feature_size: The feature size. The feature size has
             to be greater than or equal to 4. Out of all features,
             only 4 are actually used to compute the targets.
             The remaining features are independent of targets.
-        noise_std: Specifies the standard deviation of the Gaussian
+        noise_std: The standard deviation of the Gaussian
             noise.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A batch with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, feature_size)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -46,14 +46,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_sparse_uncorrelated_regression
     >>> data = make_sparse_uncorrelated_regression(num_examples=10)
     >>> data
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/swissroll.py` & `startorch-0.1.1a0/src/startorch/example/swissroll.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 
 
 class SwissRollExampleGenerator(BaseExampleGenerator):
     r"""Implements a manifold example generator based on the Swiss roll
     pattern.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_swiss_roll.html
+    [`sklearn.datasets.make_swiss_roll`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_swiss_roll.html).
 
     Args:
-        noise_std: Specifies the standard deviation of the Gaussian
-            noise.
-        spin: Specifies the number of spins of the Swiss roll.
-        hole: If ``True`` generates the Swiss roll with hole dataset.
+        noise_std: The standard deviation of the Gaussian noise.
+        spin: The number of spins of the Swiss roll.
+        hole: If ``True`` generates the Swiss roll with a hole.
 
     Raises:
         ValueError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import SwissRoll
     >>> generator = SwissRoll()
     >>> generator
     SwissRollExampleGenerator(noise_std=0.0, spin=1.5, hole=False)
     >>> batch = generator.generate(batch_size=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
@@ -92,23 +92,23 @@
     spin: float = 1.5,
     hole: bool = False,
     generator: torch.Generator | None = None,
 ) -> dict[str, torch.Tensor]:
     r"""Generate a toy manifold dataset based on Swiss roll pattern.
 
     The implementation is based on
-    https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_swiss_roll.html
+    [`sklearn.datasets.make_swiss_roll`](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.make_swiss_roll.html).
 
     Args:
-        num_examples: Specifies the number of examples.
-        noise_std: Specifies the standard deviation of the Gaussian
+        num_examples: The number of examples.
+        noise_std: The standard deviation of the Gaussian
             noise.
-        spin: Specifies the number of spins of the Swiss roll.
+        spin: The number of spins of the Swiss roll.
         hole: If ``True`` generates the Swiss roll with hole dataset.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A batch with two items:
             - ``'input'``: a ``BatchedTensor`` of type float and
                 shape ``(num_examples, 3)``. This
                 tensor represents the input features.
             - ``'target'``: a ``BatchedTensor`` of type float and
@@ -117,14 +117,15 @@
 
     Raises:
         RuntimeError: if one of the parameters is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.example import make_swiss_roll
     >>> batch = make_swiss_roll(num_examples=10)
     >>> batch
     {'target': tensor([...]), 'feature': tensor([[...]])}
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/example/timeseries.py` & `startorch-0.1.1a0/src/startorch/timeseries/periodic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,80 +1,87 @@
-r"""Contain the implementation of example generator that generates
-sequences from a time series generator."""
+r"""Implement a time series generator to generate periodic time series
+from a regular time series generator."""
 
 from __future__ import annotations
 
-__all__ = ["TimeSeriesExampleGenerator"]
-
+__all__ = ["PeriodicTimeSeriesGenerator"]
 
+import math
 from typing import TYPE_CHECKING
 
+from batchtensor.nested import repeat_along_seq, slice_along_seq
 from coola.utils import str_indent, str_mapping
 
-from startorch.example.base import BaseExampleGenerator
-from startorch.tensor.base import setup_tensor_generator
+from startorch.periodic.timeseries.base import BasePeriodicTimeSeriesGenerator
+from startorch.tensor.base import BaseTensorGenerator, setup_tensor_generator
 from startorch.timeseries.base import (
     BaseTimeSeriesGenerator,
     setup_timeseries_generator,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Hashable
 
     import torch
 
-    from startorch.tensor.base import BaseTensorGenerator
-
 
-class TimeSeriesExampleGenerator(BaseExampleGenerator):
-    r"""Implement an example generator to generate time series.
+class PeriodicTimeSeriesGenerator(BaseTimeSeriesGenerator):
+    r"""Implement a time series generator to generate periodic time
+    series from a regular time series generator.
 
     Args:
-        timeseries: Specifies a time series generator or its
-            configuration.
-        seq_len: Specifies the sequence length sampler or its
-            configuration. This sampler is used to sample the
-            sequence length at each batch.
+        timeseries: A time series generator or its
+            configuration that is used to generate the periodic
+            pattern.
+        period: The period length sampler or its
+            configuration. This sampler is used to sample the period
+            length at each batch.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.example import TimeSeriesExampleGenerator
-    >>> from startorch.timeseries import TimeSeriesGenerator
-    >>> from startorch.sequence import Periodic, RandUniform
+
+    >>> from startorch.timeseries import Periodic, SequenceTimeSeries
+    >>> from startorch.sequence import RandUniform
     >>> from startorch.tensor import RandInt
-    >>> generator = TimeSeriesExampleGenerator(
-    ...     timeseries=TimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()}),
-    ...     seq_len=RandInt(2, 5),
+    >>> generator = Periodic(
+    ...     SequenceTimeSeries({"value": RandUniform(), "time": RandUniform()}),
+    ...     period=RandInt(2, 5),
     ... )
     >>> generator
-    TimeSeriesExampleGenerator(
-      (timeseries): TimeSeriesGenerator(
+    PeriodicTimeSeriesGenerator(
+      (sequence): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
-      (seq_len): RandIntTensorGenerator(low=2, high=5)
+      (period): RandIntTensorGenerator(low=2, high=5)
     )
-    >>> generator.generate(batch_size=10)
+    >>> generator.generate(seq_len=10, batch_size=2)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
 
     ```
     """
 
     def __init__(
         self,
-        timeseries: BaseTimeSeriesGenerator | dict,
-        seq_len: BaseTensorGenerator | dict,
+        timeseries: BaseTimeSeriesGenerator | BasePeriodicTimeSeriesGenerator | dict,
+        period: BaseTensorGenerator | dict,
     ) -> None:
         super().__init__()
         self._timeseries = setup_timeseries_generator(timeseries)
-        self._seq_len = setup_tensor_generator(seq_len)
+        self._period = setup_tensor_generator(period)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"timeseries": self._timeseries, "seq_len": self._seq_len}))
+        args = str_indent(str_mapping({"sequence": self._timeseries, "period": self._period}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
-        self, batch_size: int = 1, rng: torch.Generator | None = None
+        self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
-        seq_len = int(self._seq_len.generate((1,), rng=rng).item())
-        return self._timeseries.generate(seq_len=seq_len, batch_size=batch_size, rng=rng)
+        period = int(self._period.generate((1,), rng=rng).item())
+        if isinstance(self._timeseries, BasePeriodicTimeSeriesGenerator):
+            return self._timeseries.generate(
+                seq_len=seq_len, period=period, batch_size=batch_size, rng=rng
+            )
+        data = self._timeseries.generate(seq_len=period, batch_size=batch_size, rng=rng)
+        data = repeat_along_seq(data, math.ceil(seq_len / period))
+        return slice_along_seq(data, stop=seq_len)
```

### Comparing `startorch-0.1.0/src/startorch/periodic/sequence/__init__.py` & `startorch-0.1.1a0/src/startorch/periodic/sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/periodic/sequence/base.py` & `startorch-0.1.1a0/src/startorch/periodic/sequence/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     r"""Define the base class to generate periodic sequences.
 
     A child class has to implement the ``generate`` method.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.periodic.sequence import Repeat
     >>> from startorch.sequence import RandUniform
     >>> generator = Repeat(RandUniform())
     >>> generator
     RepeatPeriodicSequenceGenerator(
       (generator): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
@@ -51,18 +52,18 @@
         self, seq_len: int, period: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         r"""Generate a batch of periodic sequences.
 
         All the sequences in the batch have the same length.
 
         Args:
-            seq_len: Specifies the sequence length.
-            period: Specifies the period.
-            batch_size: Specifies the batch size.
-            rng: Specifies an optional random number generator.
+            seq_len: The sequence length.
+            period: The period.
+            batch_size: The batch size.
+            rng: An optional random number generator.
 
         Returns:
             A batch of sequences represented as a tensor of shape
                 ``(batch_size, sequence_length, *)`` where `*` means
                 any number of dimensions.
 
         Example usage:
@@ -85,23 +86,24 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration
             for a ``BasePeriodicSequenceGenerator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.sequence import is_periodic_sequence_generator_config
     >>> is_periodic_sequence_generator_config(
     ...     {
     ...         "_target_": "startorch.periodic.sequence.Repeat",
     ...         "generator": {"_target_": "startorch.sequence.RandUniform"},
     ...     }
     ... )
@@ -117,23 +119,24 @@
 ) -> BasePeriodicSequenceGenerator:
     r"""Set up a periodic sequence generator.
 
     The sequence generator is instantiated from its configuration by
     using the ``BasePeriodicSequenceGenerator`` factory function.
 
     Args:
-        generator: Specifies a periodic sequence generator or its
+        generator: A periodic sequence generator or its
             configuration.
 
     Returns:
         A periodic sequence generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.sequence import setup_periodic_sequence_generator
     >>> setup_periodic_sequence_generator(
     ...     {
     ...         "_target_": "startorch.periodic.sequence.Repeat",
     ...         "generator": {"_target_": "startorch.sequence.RandUniform"},
     ...     }
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/periodic/sequence/repeat.py` & `startorch-0.1.1a0/src/startorch/periodic/sequence/repeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,20 @@
 
 class RepeatPeriodicSequenceGenerator(BasePeriodicSequenceGenerator):
     r"""Implement a class to generate periodic sequences by using a
     ``BaseSequenceGenerator`` object and repeating the generated
     sequence.
 
     Args:
-        sequence: Specifies a sequence generator or its configuration.
+        generator: A sequence generator or its configuration.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.periodic.sequence import Repeat
     >>> from startorch.sequence import RandUniform
     >>> generator = Repeat(RandUniform())
     >>> generator
     RepeatPeriodicSequenceGenerator(
       (generator): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
```

### Comparing `startorch-0.1.0/src/startorch/periodic/sequence/wave.py` & `startorch-0.1.1a0/src/startorch/periodic/sequence/wave.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,25 @@
     sequence by sampling values with a sine wave pattern.
 
     The sequences are generated by using the following formula:
 
     ``output = amplitude * sin(2 * pi * frequency * value + phase)``
 
     Args:
-        value: Specifies a sequence generator (or its configuration)
+        value: A sequence generator (or its configuration)
             to generate the sequence values.
-        phase: Specifies a sequence generator (or its configuration)
+        phase: A sequence generator (or its configuration)
             to generate the phase values.
-        amplitude: Specifies a sequence generator (or its
+        amplitude: A sequence generator (or its
             configuration) to generate the amplitude values.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.periodic.sequence import Repeat, SineWave
     >>> from startorch.sequence import RandUniform
     >>> generator = SineWave(
     ...     value=Repeat(RandUniform(low=-1.0, high=1.0)),
     ...     phase=Repeat(RandUniform(low=-1.0, high=1.0)),
     ...     amplitude=Repeat(RandUniform(low=-1.0, high=1.0)),
```

### Comparing `startorch-0.1.0/src/startorch/periodic/timeseries/__init__.py` & `startorch-0.1.1a0/src/startorch/periodic/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/periodic/timeseries/base.py` & `startorch-0.1.1a0/src/startorch/periodic/timeseries/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,21 +31,24 @@
     r"""Define the base class to generate periodic time series.
 
     A child class has to implement the ``generate`` method.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.timeseries import Repeat
-    >>> from startorch.timeseries import TimeSeries
+    >>> from startorch.timeseries import SequenceTimeSeriesGenerator
     >>> from startorch.sequence import RandUniform
-    >>> generator = Repeat(TimeSeries({"value": RandUniform(), "time": RandUniform()}))
+    >>> generator = Repeat(
+    ...     SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()})
+    ... )
     >>> generator
     RepeatPeriodicTimeSeriesGenerator(
-      (generator): TimeSeriesGenerator(
+      (generator): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
     )
     >>> generator.generate(seq_len=12, period=4, batch_size=4)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
 
@@ -57,29 +60,29 @@
         self, seq_len: int, period: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
         r"""Generate a batch of periodic time series.
 
         All the time series in the batch have the same length.
 
         Args:
-            seq_len: Specifies the sequence length.
-            period: Specifies the period.
-            batch_size: Specifies the batch size.
-            rng: Specifies an optional random number generator.
+            seq_len: The sequence length.
+            period: The period.
+            batch_size: The batch size.
+            rng: An optional random number generator.
 
         Returns:
             A batch of periodic time series.
 
         Example usage:
 
         ```pycon
         >>> from startorch.periodic.timeseries import Repeat
-        >>> from startorch.timeseries import TimeSeries
+        >>> from startorch.timeseries import SequenceTimeSeriesGenerator
         >>> from startorch.sequence import RandUniform
-        >>> generator = Repeat(TimeSeries({"value": RandUniform(), "time": RandUniform()}))
+        >>> generator = Repeat(SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()}))
         >>> generator.generate(seq_len=12, period=4, batch_size=4)
         {'value': tensor([[...]]), 'time': tensor([[...]])}
 
         ```
         """
 
 
@@ -89,30 +92,31 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration
             for a ``BasePeriodicTimeSeriesGenerator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.timeseries import is_periodic_timeseries_generator_config
     >>> is_periodic_timeseries_generator_config(
     ...     {
     ...         "_target_": "startorch.periodic.timeseries.Repeat",
     ...         "generator": {
-    ...             "_target_": "startorch.timeseries.TimeSeries",
-    ...             "sequences": {
+    ...             "_target_": "startorch.timeseries.SequenceTimeSeriesGenerator",
+    ...             "generators": {
     ...                 "value": {"_target_": "startorch.sequence.RandUniform"},
     ...                 "time": {"_target_": "startorch.sequence.RandUniform"},
     ...             },
     ...         },
     ...     }
     ... )
     True
@@ -127,38 +131,39 @@
 ) -> BasePeriodicTimeSeriesGenerator:
     r"""Set up a periodic time series generator.
 
     The time series generator is instantiated from its configuration by
     using the ``BasePeriodicTimeSeriesGenerator`` factory function.
 
     Args:
-        generator: Specifies a periodic time series generator or its
+        generator: A periodic time series generator or its
             configuration.
 
     Returns:
         A periodic time series generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.timeseries import setup_periodic_timeseries_generator
     >>> setup_periodic_timeseries_generator(
     ...     {
     ...         "_target_": "startorch.periodic.timeseries.Repeat",
     ...         "generator": {
-    ...             "_target_": "startorch.timeseries.TimeSeries",
-    ...             "sequences": {
+    ...             "_target_": "startorch.timeseries.SequenceTimeSeriesGenerator",
+    ...             "generators": {
     ...                 "value": {"_target_": "startorch.sequence.RandUniform"},
     ...                 "time": {"_target_": "startorch.sequence.RandUniform"},
     ...             },
     ...         },
     ...     }
     ... )
     RepeatPeriodicTimeSeriesGenerator(
-      (generator): TimeSeriesGenerator(
+      (generator): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
     )
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/periodic/timeseries/repeat.py` & `startorch-0.1.1a0/src/startorch/periodic/timeseries/repeat.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
 class RepeatPeriodicTimeSeriesGenerator(BasePeriodicTimeSeriesGenerator):
     r"""Implement a class to generate periodic sequences by using a
     ``BaseTimeSeriesGenerator`` object and repeating the generated
     sequence.
 
     Args:
-        generator: Specifies a sequence generator or its configuration.
+        generator: A sequence generator or its configuration.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.periodic.timeseries import Repeat
-    >>> from startorch.timeseries import TimeSeries
+    >>> from startorch.timeseries import SequenceTimeSeriesGenerator
     >>> from startorch.sequence import RandUniform
-    >>> generator = Repeat(TimeSeries({"value": RandUniform(), "time": RandUniform()}))
+    >>> generator = Repeat(
+    ...     SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()})
+    ... )
     >>> generator
     RepeatPeriodicTimeSeriesGenerator(
-      (generator): TimeSeriesGenerator(
+      (generator): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
     )
     >>> generator.generate(seq_len=12, period=4, batch_size=4)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
```

### Comparing `startorch-0.1.0/src/startorch/plot/matplotlib/feature.py` & `startorch-0.1.1a0/src/startorch/plot/matplotlib/feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 ) -> plt.Figure:
     r"""Plot the distribution of each feature.
 
     If the input has ``n`` features, this function returns a figure
     with ``n`` histograms: one for each features.
 
     Args:
-        features: Specifies the features. It must be a tensor of shape
+        features: The features. It must be a tensor of shape
             ``(d0, d1, ..., dn)``.
-        feature_names: Specifies the feature names. If ``None``,
+        feature_names: The feature names. If ``None``,
             the feature names are generated automatically.
-        ncols: Specifies the number of columns.
-        figsize: Specifies the individual figure size in pixels.
+        ncols: The number of columns.
+        figsize: The individual figure size in pixels.
             The first dimension is the width and the second is the
             height.
         **kwargs: Additional keyword arguments for ``plt.hist``.
 
     Returns:
         ``matplotlib.pyplot.Figure``: The generated figure.
 
@@ -54,14 +54,15 @@
         RuntimeError: if the ``features`` shape is invalid
         RuntimeError: if ``features`` and ``feature_names`` are not
             consistent
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.matplotlib import hist_feature
     >>> import numpy as np
     >>> fig = hist_feature(np.random.rand(10, 5))
 
     ```
     """
     check_matplotlib()
```

### Comparing `startorch-0.1.0/src/startorch/plot/matplotlib/sequence.py` & `startorch-0.1.1a0/src/startorch/plot/matplotlib/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,30 +36,31 @@
     figsize: tuple[float, float] = (16, 5),
     scale: str = "identity",
     **kwargs: Any,
 ) -> plt.Figure:
     r"""Plot the distribution from a sequence generator.
 
     Args:
-        sequence: Specifies the sequence generator.
-        bins: Specifies the number of histogram bins.
-        seq_len: Specifies the sequence length.
-        batch_size: Specifies the batch size.
-        num_batches: Specifies the number of batches to generate.
-        rng: Specifies a random number generator or a random seed.
-        figsize: Specifies the figure size.
-        scale: Specifies a scale transformation of the features.
+        sequence: The sequence generator.
+        bins: The number of histogram bins.
+        seq_len: The sequence length.
+        batch_size: The batch size.
+        num_batches: The number of batches to generate.
+        rng: A random number generator or a random seed.
+        figsize: The figure size.
+        scale: The transformation scale of the features.
         **kwargs: Additional keyword arguments for ``plt.hist``.
 
     Returns:
         The generated figure.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.matplotlib import hist_sequence
     >>> from startorch.sequence import RandUniform
     >>> fig = hist_sequence(RandUniform(low=-5, high=5))
 
     ```
     """
     check_matplotlib()
@@ -87,30 +88,31 @@
     xscale: str = "linear",
     yscale: str = "linear",
     **kwargs: Any,
 ) -> plt.Figure:
     r"""Plot some sequences generated from a sequence generator.
 
     Args:
-        sequence: Specifies the sequence generator.
-        seq_len: Specifies the sequence length.
-        batch_size: Specifies the batch size.
-        num_batches: Specifies the number of batches.
-        rng: Specifies a random number generator or a random seed.
-        figsize: Specifies the figure size.
-        xscale: Specifies the x-axis scale.
-        yscale: Specifies the y-axis scale.
+        sequence: The sequence generator.
+        seq_len: The sequence length.
+        batch_size: The batch size.
+        num_batches: The number of batches.
+        rng: A random number generator or a random seed.
+        figsize: The figure size.
+        xscale: The x-axis scale.
+        yscale: The y-axis scale.
         **kwargs: Additional keyword arguments for ``plt.plot``.
 
     Returns:
         The generated figure.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.matplotlib import plot_sequence
     >>> from startorch.sequence import RandUniform
     >>> fig = plot_sequence(RandUniform(low=-5, high=5), batch_size=4)
 
     ```
     """
     check_matplotlib()
```

### Comparing `startorch-0.1.0/src/startorch/plot/plotly/feature.py` & `startorch-0.1.1a0/src/startorch/plot/plotly/feature.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,20 @@
 ) -> go.Figure:
     r"""Plot the distribution of each feature.
 
     If the input has ``n`` features, this function returns a figure
     with ``n`` histograms: one for each feature.
 
     Args:
-        features: Specifies the features. It must be a tensor of shape
+        features: The features. It must be a tensor of shape
             ``(d0, d1, ..., dn)``.
-        feature_names: Specifies the feature names. If ``None``,
+        feature_names: The feature names. If ``None``,
             the feature names are generated automatically.
-        ncols: Specifies the number of columns.
-        figsize: Specifies the individual figure size in pixels.
+        ncols: The number of columns.
+        figsize: The individual figure size in pixels.
             The first dimension is the width and the second is the
             height.
         **kwargs: Additional keyword arguments for
             ``plotly.graph_objects.Histogram``.
 
     Returns:
         The generated figure.
@@ -56,14 +56,15 @@
         RuntimeError: if the ``features`` shape is invalid
         RuntimeError: if ``features`` and ``feature_names`` are not
             consistent
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.plotly import hist_feature
     >>> import numpy as np
     >>> fig = hist_feature(np.random.rand(10, 5))
 
     ```
     """
     check_plotly()
```

### Comparing `startorch-0.1.0/src/startorch/plot/plotly/sequence.py` & `startorch-0.1.1a0/src/startorch/plot/plotly/sequence.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,31 +39,32 @@
     figsize: tuple[int, int] = (800, 600),
     scale: str = "identity",
     **kwargs: Any,
 ) -> go.Figure:
     r"""Plot the distribution from a sequence generator.
 
     Args:
-        sequence: Specifies the sequence generator.
-        bins: Specifies the number of histogram bins.
-        seq_len: Specifies the sequence length.
-        batch_size: Specifies the batch size.
-        num_batches: Specifies the number of batches to generate.
-        rng: Specifies a random number generator or a random seed.
-        figsize: Specifies the figure size.
-        scale: Specifies a scale transformation of the features.
+        sequence: The sequence generator.
+        bins: The number of histogram bins.
+        seq_len: The sequence length.
+        batch_size: The batch size.
+        num_batches: The number of batches to generate.
+        rng: A random number generator or a random seed.
+        figsize: The figure size.
+        scale: A scale transformation of the features.
         **kwargs: Additional keyword arguments for
             ``plotly.graph_objects.Histogram``.
 
     Returns:
         The generated figure.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.plotly import hist_sequence
     >>> from startorch.sequence import RandUniform
     >>> fig = hist_sequence(RandUniform(low=-5, high=5))
 
     ```
     """
     check_plotly()
@@ -88,28 +89,28 @@
     num_batches: int = 1,
     rng: int | torch.Generator = 13683624337160779813,
     **kwargs: Any,
 ) -> go.Figure:
     r"""Plot some sequences generated from a sequence generator.
 
     Args:
-        sequence: Specifies the sequence generator.
-        seq_len: Specifies the sequence length.
-        batch_size: Specifies the batch size.
-        num_batches: Specifies the number of batches.
-        rng: Specifies a random number generator or a random seed.
-        figsize: Specifies the figure size.
+        sequence: The sequence generator.
+        seq_len: The sequence length.
+        batch_size: The batch size.
+        num_batches: The number of batches.
+        rng: A random number generator or a random seed.
         **kwargs: Additional keyword arguments for ``plt.plot``.
 
     Returns:
         The generated figure.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.plot.plotly import plot_sequence
     >>> from startorch.sequence import RandUniform
     >>> fig = plot_sequence(RandUniform(low=-5, high=5), batch_size=4)
 
     ```
     """
     check_plotly()
```

### Comparing `startorch-0.1.0/src/startorch/random/__init__.py` & `startorch-0.1.1a0/src/startorch/random/__init__.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/random/bounded.py` & `startorch-0.1.1a0/src/startorch/random/bounded.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,32 +47,33 @@
     max_value: float = 2.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Cauchy distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        loc: Specifies the location of the Cauchy distribution.
-        scale: Specifies the scale of the Cauchy distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        size: The tensor shape.
+        loc: The location of the Cauchy distribution.
+        scale: The scale of the Cauchy distribution.
+        min_value: The minimum value.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated Cauchy
             distribution
 
     Raises:
         ValueError: if the ``max_value`` and ``min_value`` parameters
             are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_cauchy
     >>> rand_trunc_cauchy((2, 3), loc=1.0, scale=2.0, min_value=-3.0, max_value=3.0)
     tensor([[...]])
 
     ```
     """
@@ -96,35 +97,36 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Cauchy distribution.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
+        loc: The location/median of the Cauchy distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        scale: Specifies the scale of the Cauchy distribution.
+        scale: The scale of the Cauchy distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        min_value: Specifies the minimum value. It must be a float
+        min_value: The minimum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated Cauchy distribution
 
     Raises:
         ValueError: if the ``loc``, ``scale``, ``max_value`` and
             ``min_value`` parameters are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import trunc_cauchy
     >>> trunc_cauchy(
     ...     loc=torch.tensor([1.0, 0.0, -1.0]),
     ...     scale=torch.tensor([1.0, 3.0, 5.0]),
     ...     min_value=torch.tensor([-5.0, -10.0, -15.0]),
     ...     max_value=torch.tensor([5.0, 10.0, 15.0]),
@@ -164,29 +166,30 @@
     max_value: float = 5.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Exponential distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        rate: Specifies the rate of the Exponential distribution.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        size: The tensor shape.
+        rate: The rate of the Exponential distribution.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated
             Exponential distribution
 
     Raises:
         ValueError: if the ``max_value`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_exponential
     >>> rand_trunc_exponential((2, 3), rate=1.0, max_value=3.0)
     tensor([[...]])
 
     ```
     """
@@ -208,31 +211,32 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Exponential distribution.
 
     Args:
-        rate: Specifies the rate of the Exponential distribution.
+        rate: The rate of the Exponential distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated Exponential distribution.
 
     Raises:
         ValueError: if the ``rate`` and ``max_value`` parameter are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import trunc_exponential
     >>> trunc_exponential(
     ...     rate=torch.tensor([1.0, 3.0, 5.0]),
     ...     max_value=torch.tensor([5.0, 10.0, 15.0]),
     ... )
     tensor([...])
@@ -267,29 +271,30 @@
     max_value: float = 4.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated half-
     Cauchy distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        scale: Specifies the scale of the half-Cauchy distribution.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        size: The tensor shape.
+        scale: The scale of the half-Cauchy distribution.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated
             half-Cauchy distribution.
 
     Raises:
         ValueError: if the ``max_value`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_half_cauchy
     >>> rand_trunc_half_cauchy((2, 3), scale=1.0, max_value=3.0)
     tensor([[...]])
 
     ```
     """
@@ -311,31 +316,32 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated half-
     Cauchy distribution.
 
     Args:
-        scale: Specifies the scale of the half-Cauchy distribution.
+        scale: The scale of the half-Cauchy distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated Cauchy distribution.
 
     Raises:
         ValueError: if the ``scale`` and ``max_value`` parameter are
             not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import trunc_half_cauchy
     >>> trunc_half_cauchy(
     ...     scale=torch.tensor([1.0, 3.0, 5.0]),
     ...     max_value=torch.tensor([5.0, 10.0, 15.0]),
     ... )
     tensor([...])
@@ -370,30 +376,31 @@
     max_value: float = 5.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated half-
     Normal distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        std: Specifies the standard deviation of the half-Normal
+        size: The tensor shape.
+        std: The standard deviation of the half-Normal
             distribution.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated
             half-Normal distribution.
 
     Raises:
         ValueError: if the ``max_value`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_half_normal
     >>> rand_trunc_half_normal((2, 3), std=1.0, max_value=3.0)
     tensor([[...]])
 
     ```
     """
@@ -415,32 +422,33 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated half-
     Normal distribution.
 
     Args:
-        std: Specifies the standard deviation of the half-Normal
+        std: The standard deviation of the half-Normal
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated half-Normal distribution.
 
     Raises:
         ValueError: if the ``std`` and ``max_value`` parameters are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import trunc_half_normal
     >>> trunc_half_normal(
     ...     std=torch.tensor([1.0, 3.0, 5.0]), max_value=torch.tensor([5.0, 10.0, 15.0])
     ... )
     tensor([...])
 
@@ -474,33 +482,34 @@
     max_value: float = 5.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated log-
     Normal distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        mean: Specifies the mean of the underlying Normal distribution.
-        std: Specifies the standard deviation of the underlying Normal
+        size: The tensor shape.
+        mean: The mean of the underlying Normal distribution.
+        std: The standard deviation of the underlying Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        min_value: The minimum value.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated log-Normal
             distribution.
 
     Raises:
         ValueError: if the ``min_value`` and ``max_value`` parameters
             are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_log_normal
     >>> rand_trunc_log_normal((2, 3), mean=0.0, std=1.0, min_value=1.0, max_value=4.0)
     tensor([[...]])
 
     ```
     """
@@ -524,24 +533,24 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated log-
     Normal distribution.
 
     Args:
-        mean: Specifies the mean of the underlying Normal distribution.
+        mean: The mean of the underlying Normal distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        std: Specifies the standard deviation of the underlying Normal
+        std: The standard deviation of the underlying Normal
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        min_value: Specifies the minimum value. It must be a float
+        min_value: The minimum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated log-Normal distribution.
 
     Raises:
         ValueError: if the ``mean``, ``std``, ``min_value`` and
@@ -597,33 +606,34 @@
     max_value: float = 3.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Normal distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        size: The tensor shape.
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
-        generator: Specifies an optional random generator.
+        min_value: The minimum value.
+        max_value: The maximum value.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a truncated Normal
             distribution.
 
     Raises:
         ValueError: if the ``min_value`` and  ``max_value`` parameters
             are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_trunc_normal
     >>> rand_trunc_normal((2, 3), mean=1.0, std=2.0, min_value=-5.0, max_value=5.0)
     tensor([[...]])
 
     ```
     """
@@ -647,36 +657,37 @@
     max_value: torch.Tensor,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a truncated
     Normal distribution.
 
     Args:
-        mean: Specifies the mean of the Normal distribution.
+        mean: The mean of the Normal distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        std: Specifies the standard deviation of the Normal
+        std: The standard deviation of the Normal
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        min_value: Specifies the minimum value. It must be a float
+        min_value: The minimum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        max_value: Specifies the maximum value. It must be a float
+        max_value: The maximum value. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a truncated Normal distribution.
 
     Raises:
         ValueError: if the ``min_value`` and  ``max_value`` parameters
             are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import trunc_normal
     >>> trunc_normal(
     ...     mean=torch.tensor([1.0, 0.0, -1.0]),
     ...     std=torch.tensor([1.0, 3.0, 5.0]),
     ...     min_value=torch.tensor([-5.0, -10.0, -15.0]),
     ...     max_value=torch.tensor([5.0, 10.0, 15.0]),
@@ -717,30 +728,31 @@
     high: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a uniform
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
-        generator: Specifies an optional random generator.
+        size: The tensor shape.
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a uniform
             distribution.
 
     Raises:
         ValueError: if the ``low`` and  ``high`` parameters  are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_uniform
     >>> rand_uniform((2, 3), low=-1.0, high=2.0)
     tensor([[...]])
 
     ```
     """
@@ -760,33 +772,34 @@
 
     Unlike ``rand_uniform``, this function allows to sample values
     from different uniform distributions at the same time.
     The shape of the ``low`` and ``high`` tensors are used to infer
     the output size.
 
     Args:
-        low: Specifies the minimum values (inclusive). It must be a
+        low: The minimum values (inclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        high: Specifies the maximum values (exclusive). It must be a
+        high: The maximum values (exclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a uniform distribution where the minimum and
             maximum values are given as input.
 
     Raises:
         ValueError: if the input tensor shapes do not match or if at
             least one value in ``low`` tensor is higher than its
             associated high value in ``high``
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import uniform
     >>> uniform(low=torch.tensor([-1.0, 0.0, 1.0]), high=torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
@@ -816,31 +829,32 @@
     high: float,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a uniform
     distribution in the log space.
 
     Args:
-        size: Specifies the tensor shape.
-        low: Specifies the minimum value (inclusive).
+        size: The tensor shape.
+        low: The minimum value (inclusive).
             This value needs to be positive.
-        high: Specifies the maximum value (exclusive).
-        generator: Specifies an optional random generator.
+        high: The maximum value (exclusive).
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a uniform distribution
             in the log space.
 
     Raises:
         ValueError: if the ``low`` and  ``high`` parameters  are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.random import rand_log_uniform
     >>> rand_log_uniform((2, 3), low=0.1, high=1000.0)
     tensor([[...]])
 
     ```
     """
     if high < low:
@@ -859,32 +873,33 @@
 def log_uniform(
     low: torch.Tensor, high: torch.Tensor, generator: torch.Generator | None = None
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a uniform
     distribution in the log space.
 
     Args:
-        low: Specifies the minimum values (inclusive). It must be a
+        low: The minimum values (inclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        high: Specifies the maximum values (exclusive). It must be a
+        high: The maximum values (exclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a uniform distribution in the log space where
             the minimum and maximum values are given as input.
 
     Raises:
         ValueError: if the ``low`` and  ``high`` parameters  are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.random import log_uniform
     >>> log_uniform(low=torch.tensor([0.01, 0.1, 1.0]), high=torch.tensor([1.0, 10.0, 100.0]))
     tensor([...])
 
     ```
     """
     if low.shape != high.shape:
@@ -915,31 +930,32 @@
     high: float,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a uniform
     distribution in the inverse hyperbolic sine space.
 
     Args:
-        size: Specifies the tensor shape.
-        low: Specifies the minimum value (inclusive).
+        size: The tensor shape.
+        low: The minimum value (inclusive).
             This value needs to be positive.
-        high: Specifies the maximum value (exclusive).
-        generator: Specifies an optional random generator.
+        high: The maximum value (exclusive).
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a uniform distribution
             in the inverse hyperbolic sine space.
 
     Raises:
         ValueError: if the ``low`` and  ``high`` parameters  are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.random import rand_asinh_uniform
     >>> rand_asinh_uniform((2, 3), low=-1000.0, high=1000.0)
     tensor([[...]])
 
     ```
     """
     if high < low:
@@ -958,33 +974,34 @@
 def asinh_uniform(
     low: torch.Tensor, high: torch.Tensor, generator: torch.Generator | None = None
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a uniform
     distribution in the inverse hyperbolic sine space.
 
     Args:
-        low: Specifies the minimum values (inclusive). It must be a
+        low: The minimum values (inclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        high: Specifies the maximum values (exclusive). It must be a
+        high: The maximum values (exclusive). It must be a
             float tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a uniform distribution in the inverse
             hyperbolic sine space where the minimum and maximum values
             are given as input.
 
     Raises:
         ValueError: if the ``low`` and  ``high`` parameters  are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.random import asinh_uniform
     >>> asinh_uniform(
     ...     low=torch.tensor([-10.0, 0.0, 1.0]),
     ...     high=torch.tensor([1.0, 10.0, 100.0]),
     ... )
     tensor([...])
```

### Comparing `startorch-0.1.0/src/startorch/random/discrete.py` & `startorch-0.1.1a0/src/startorch/random/discrete.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,29 +14,30 @@
     rate: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a Poisson
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        rate: Specifies the rate of the Poisson distribution.
+        size: The tensor shape.
+        rate: The rate of the Poisson distribution.
             This value has to be greater than 0.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         ``torch.Tensor`` of type float: A tensor filled with values
             sampled from a Poisson distribution.
 
     Raises:
         ValueError: if the ``rate`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_poisson
     >>> rand_poisson(size=(2, 3), rate=2.0)
     tensor([...])
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/random/infinite.py` & `startorch-0.1.1a0/src/startorch/random/infinite.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,30 @@
     scale: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a sequence of continuous variables sampled from a Cauchy
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        loc: Specifies the location/median of the Cauchy distribution.
-        scale: Specifies the scale of the Cauchy distribution.
+        size: The tensor shape.
+        loc: The location/median of the Cauchy distribution.
+        scale: The scale of the Cauchy distribution.
             This value has to be greater than 0.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a Cauchy distribution.
 
     Raises:
-        ValueError if the ``scale`` parameter is not valid.
+        ValueError: if the ``scale`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_cauchy
     >>> rand_cauchy((2, 3), loc=1.0, scale=2.0)
     tensor([[...]])
 
     ```
     """
@@ -57,32 +58,33 @@
 
     Unlike ``rand_cauchy``, this function allows to sample values
     from different Cauchy distributions at the same time.
     The shape of the ``loc`` and ``scale`` tensors are used to infer
     the output size.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
+        loc: The location/median of the Cauchy distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        scale: Specifies the standard deviation of the Cauchy
+        scale: The standard deviation of the Cauchy
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a Cauchy distribution.
 
     Raises:
         ValueError: if the ``loc`` and ``scale`` parameters are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import cauchy
     >>> cauchy(loc=torch.tensor([-1.0, 0.0, 1.0]), scale=torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
@@ -101,29 +103,30 @@
     std: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a Normal
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        size: The tensor shape.
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a Normal distribution.
 
     Raises:
         ValueError: if the ``std`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_normal
     >>> rand_normal((2, 3), mean=1.0, std=2.0)
     tensor([[...]])
 
     ```
     """
@@ -136,31 +139,32 @@
 def normal(
     mean: torch.Tensor, std: torch.Tensor, generator: torch.Generator | None = None
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a Normal
     distribution.
 
     Args:
-        mean: Specifies the mean. It must be a float tensor of shape
+        mean: The mean. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        std: Specifies the standard deviation. It must be a float
+        std: The standard deviation. It must be a float
             tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a Normal distribution.
 
     Raises:
         ValueError: if the ``mean`` and ``std`` parameters are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import normal
     >>> normal(mean=torch.tensor([-1.0, 0.0, 1.0]), std=torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/random/semi_infinite.py` & `startorch-0.1.1a0/src/startorch/random/semi_infinite.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,28 +25,29 @@
     rate: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from an Exponential
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        rate: Specifies the rate of the Exponential distribution.
-        generator: Specifies an optional random generator.
+        size: The tensor shape.
+        rate: The rate of the Exponential distribution.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from an Exponential
             distribution.
 
     Raises:
         ValueError: if the ``rate`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_exponential
     >>> rand_exponential((2, 3), rate=1.0)
     tensor([[...]])
 
     ```
     """
@@ -63,28 +64,29 @@
     distribution.
 
     Unlike ``rand_exponential``, this function allows to sample values
     from different Exponential distributions at the same time.
     The shape of the ``rate`` tensor is used to infer the output size.
 
     Args:
-        rate: Specifies the rates of the Exponential distribution.
+        rate: The rates of the Exponential distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from an Exponential distribution.
 
     Raises:
         ValueError: if the ``rate`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import exponential
     >>> exponential(torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
@@ -100,29 +102,30 @@
     scale: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a half-Cauchy
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        scale: Specifies the scale of the half-Cauchy distribution.
+        size: The tensor shape.
+        scale: The scale of the half-Cauchy distribution.
             This value has to be greater than 0.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a half-Cauchy
             distribution.
 
     Raises:
         ValueError: if the ``scale`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_half_cauchy
     >>> rand_half_cauchy((2, 3), scale=1.0)
     tensor([[...]])
 
     ```
     """
@@ -135,28 +138,29 @@
 
     Unlike ``rand_half_cauchy``, this function allows to sample values
     from different half-Cauchy distributions at the same time.
     The shape of the ``scale`` tensor is used to infer
     the output size.
 
     Args:
-        scale: Specifies the scale of the half-Cauchy distribution.
+        scale: The scale of the half-Cauchy distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a half-Cauchy distribution.
 
     Raises:
-        ValueError if the ``scale`` parameter is not valid.
+        ValueError: if the ``scale`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import half_cauchy
     >>> half_cauchy(torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
@@ -168,29 +172,30 @@
     std: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a half-Normal
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        std: Specifies the standard deviation of the half-Normal
+        size: The tensor shape.
+        std: The standard deviation of the half-Normal
             distribution.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor filled with values sampled from a half-Normal
             distribution.
 
     Raises:
         ValueError: if the ``std`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_half_normal
     >>> rand_half_normal((2, 3), std=1.0)
     tensor([[...]])
 
     ```
     """
@@ -206,15 +211,15 @@
 
     Unlike ``rand_half_normal``, this function allows to sample values
     from different half-Normal distributions at the same time.
     The shape of the ``std`` tensor is used to infer
     the output size.
 
     Args:
-        std: Specifies the standard deviation of the half-Normal
+        std: The standard deviation of the half-Normal
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
         generator: Specifies
             an optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
@@ -222,14 +227,15 @@
 
     Raises:
         ValueError: if the ``std`` parameter is not valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import half_normal
     >>> half_normal(torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
@@ -242,31 +248,32 @@
     std: float = 1.0,
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a tensor filled with values sampled from a log-Normal
     distribution.
 
     Args:
-        size: Specifies the tensor shape.
-        mean: Specifies the mean of the underlying Normal distribution.
-        std: Specifies the standard deviation of the underlying
+        size: The tensor shape.
+        mean: The mean of the underlying Normal distribution.
+        std: The standard deviation of the underlying
             Normal distribution.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a log-Normal distribution.
 
     Raises:
         ValueError: if the ``mean`` and ``std`` parametera are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import rand_log_normal
     >>> rand_log_normal((2, 3), mean=1.0, std=2.0)
     tensor([[...]])
 
     ```
     """
@@ -286,32 +293,33 @@
 
     Unlike ``rand_log_normal``, this function allows to sample values
     from different log-Normal distributions at the same time.
     The shape of the ``mean`` and ``std`` tensors are used to infer
     the output size.
 
     Args:
-        mean: Specifies the mean of the log-Normal distribution.
+        mean: The mean of the log-Normal distribution.
             It must be a float tensor of shape ``(d0, d1, ..., dn)``.
-        std: Specifies the standard deviation of the log-Normal
+        std: The standard deviation of the log-Normal
             distribution. It must be a float tensor of shape
             ``(d0, d1, ..., dn)``.
-        generator: Specifies an optional random generator.
+        generator: An optional random generator.
 
     Returns:
         A tensor of shape ``(d0, d1, ..., dn)`` filled with values
             sampled from a log-Normal distribution.
 
     Raises:
         ValueError: if the ``mean`` and ``std`` parametera are not
             valid.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.random import log_normal
     >>> log_normal(torch.tensor([-1.0, 0.0, 1.0]), torch.tensor([1.0, 3.0, 5.0]))
     tensor([...])
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/sequence/__init__.py` & `startorch-0.1.1a0/src/startorch/sequence/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
     "LogNormal",
     "LogNormalSequenceGenerator",
     "LogSequenceGenerator",
     "LogUniform",
     "LogUniformSequenceGenerator",
     "Long",
     "LongSequenceGenerator",
+    "MarkovChain",
+    "MarkovChainSequenceGenerator",
     "Mul",
     "MulScalar",
     "MulScalarSequenceGenerator",
     "MulSequenceGenerator",
     "Multinomial",
     "MultinomialChoice",
     "MultinomialChoiceSequenceGenerator",
@@ -237,14 +239,16 @@
 from startorch.sequence.lognormal import (
     RandTruncLogNormalSequenceGenerator as RandTruncLogNormal,
 )
 from startorch.sequence.lognormal import TruncLogNormalSequenceGenerator
 from startorch.sequence.lognormal import (
     TruncLogNormalSequenceGenerator as TruncLogNormal,
 )
+from startorch.sequence.markov import MarkovChainSequenceGenerator
+from startorch.sequence.markov import MarkovChainSequenceGenerator as MarkovChain
 from startorch.sequence.math import AbsSequenceGenerator
 from startorch.sequence.math import AbsSequenceGenerator as Abs
 from startorch.sequence.math import AddScalarSequenceGenerator
 from startorch.sequence.math import AddScalarSequenceGenerator as AddScalar
 from startorch.sequence.math import AddSequenceGenerator
 from startorch.sequence.math import AddSequenceGenerator as Add
 from startorch.sequence.math import ClampSequenceGenerator
```

### Comparing `startorch-0.1.0/src/startorch/sequence/ar.py` & `startorch-0.1.1a0/src/startorch/sequence/ar.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 
 
 class AutoRegressiveSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from an
     autoregressive process.
 
     Args:
-        value: Specifies a sequence generator (or its configuration)
+        value: A sequence generator (or its configuration)
             used to generate the initial sequence values. These values
             are used to start the AR.
-        coefficient: Specifies a sequence generator (or its
+        coefficient: A sequence generator (or its
             configuration) used to generate the coefficients.
-        noise: Specifies a sequence generator (or its configuration)
+        noise: A sequence generator (or its configuration)
             used to generate the noise values.
-        order: Specifies a tensor generator (or its configuration)
+        order: A tensor generator (or its configuration)
             used to generate the order of the AR.
-        max_abs_value: Specifies the maximum absolute value.
+        max_abs_value: The maximum absolute value.
             This argument ensures the values stay in the range
             ``[-max_abs_value, max_abs_value]``.
-        warmup: Specifies the number of cycles used to
+        warmup: The number of cycles used to
             initiate the AR. The initial value sampled do not follow
             an AR, so using warmup allows to initialize the AR so each
             value follows an AR.
 
     Raises:
         ValueError: if ``max_abs_value`` is not a positive number.
         ValueError: if ``warmup`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import AutoRegressive, RandUniform, RandNormal, Full
     >>> from startorch.tensor import RandInt
     >>> generator = AutoRegressive(
     ...     value=RandNormal(),
     ...     coefficient=RandUniform(low=-1.0, high=1.0),
     ...     noise=Full(0.0),
```

### Comparing `startorch-0.1.0/src/startorch/sequence/base.py` & `startorch-0.1.1a0/src/startorch/sequence/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     r"""Define the base class to generate sequences.
 
     A child class has to implement the ``generate`` method.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform
     >>> generator = RandUniform()
     >>> generator
     RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -43,17 +44,17 @@
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         r"""Generate a batch of sequences.
 
         All the sequences in the batch must have the same length.
 
         Args:
-            seq_len: Specifies the sequence length.
-            batch_size: Specifies the batch size.
-            rng: Specifies an optional random number generator.
+            seq_len: The sequence length.
+            batch_size: The batch size.
+            rng: An optional random number generator.
 
         Returns:
             A batch of sequences. The data in the batch are
                 represented as a ``torch.Tensor`` of shape
                 ``(batch_size, sequence_length, *)`` where `*` means
                 any number of dimensions.
 
@@ -76,23 +77,24 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration
             for a ``BaseSequenceGenerator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import is_sequence_generator_config
     >>> is_sequence_generator_config({"_target_": "startorch.sequence.RandUniform"})
     True
 
     ```
     """
     return is_object_config(config, BaseSequenceGenerator)
@@ -101,22 +103,23 @@
 def setup_sequence_generator(generator: BaseSequenceGenerator | dict) -> BaseSequenceGenerator:
     r"""Set up a sequence generator.
 
     The sequence generator is instantiated from its configuration by
     using the ``BaseSequenceGenerator`` factory function.
 
     Args:
-        generator: Specifies a sequence generator or its configuration.
+        generator: A sequence generator or its configuration.
 
     Returns:
         A sequence generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import setup_sequence_generator
     >>> setup_sequence_generator({"_target_": "startorch.sequence.RandUniform"})
     RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
 
     ```
     """
     if isinstance(generator, dict):
```

### Comparing `startorch-0.1.0/src/startorch/sequence/categorical.py` & `startorch-0.1.1a0/src/startorch/sequence/categorical.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 
 
 class MultinomialSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequences of categorical variables
     where each value is sampled from a multinomial distribution.
 
     Args:
-        weights (``torch.Tensor`` of shape ``(num_categories,)`` and
-            type float): Specifies the vector of weights associated
-            at each category. The weights have to be positive but do
-            not need to sum to 1.
-        feature_size: Specifies the feature size.
+        weights: The vector of weights associated at each category.
+            The weights have to be positive but do not need to sum
+            to 1. The input is expected to be a ``torch.Tensor`` of
+            shape ``(num_categories,)`` and type float.
+        feature_size: The feature size.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Multinomial
     >>> generator = Multinomial(weights=torch.ones(5))
     >>> generator
     MultinomialSequenceGenerator(num_categories=5, feature_size=(1,))
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -73,15 +74,15 @@
         r"""Instantiate the weights with a uniform pattern.
 
         All the categories have the same probability.
         The weight of the ``i``-th category (``w_i``) is generated
         with the rule: ``w_i = 1``
 
         Args:
-            num_categories: Specifies the number of categories.
+            num_categories: The number of categories.
 
         Returns:
             A sequence generator where the weights of the multinomial
                 distribution follow a uniform pattern.
         """
         return cls(weights=torch.ones(num_categories))
 
@@ -89,15 +90,15 @@
     def create_linear_weights(cls, num_categories: int) -> MultinomialSequenceGenerator:
         r"""Instantiate the weights with a linear pattern.
 
         The weight of the ``i``-th category (``w_i``) is generated
         with the rule: ``w_i = num_categories - i``
 
         Args:
-            num_categories: Specifies the number of categories.
+            num_categories: The number of categories.
 
         Returns:
             A sequence generator where the weights of the multinomial
                 distribution follow a linear pattern.
         """
         return cls(
             weights=num_categories * torch.ones(num_categories) - torch.arange(num_categories)
@@ -109,16 +110,16 @@
     ) -> MultinomialSequenceGenerator:
         r"""Instantiate the weights with an exponential pattern.
 
         The weight of the ``i``-th category (``w_i``) is generated with
         the rule: ``w_i = exp(-scale * i)``
 
         Args:
-            num_categories: Specifies the number of categories.
-            scale: Specifies the scale parameter that controls the
+            num_categories: The number of categories.
+            scale: The scale parameter that controls the
                 exponential function.
 
         Returns:
             A sequence generator where the weights of the multinomial
                 distribution follow an exponential pattern.
         """
         return cls(weights=torch.arange(num_categories).float().mul(-scale).exp())
@@ -131,23 +132,24 @@
     All the categories have the same probability.
 
     Note:
         It is a more efficient implementation of
         ``Multinomial.generate_uniform_weights``.
 
     Args:
-        num_categories: Specifies the number of categories.
-        feature_size: Specifies the feature size.
+        num_categories: The number of categories.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``num_categories`` is negative.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import UniformCategorical
     >>> generator = UniformCategorical(10)
     >>> generator
     UniformCategoricalSequenceGenerator(num_categories=10, feature_size=())
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -175,10 +177,10 @@
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return torch.randint(
             low=0,
             high=self._num_categories,
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             generator=rng,
         )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/cauchy.py` & `startorch-0.1.1a0/src/startorch/sequence/cauchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
 
 class CauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies a sequence generator (or its configuration) to
+        loc: A sequence generator (or its configuration) to
             generate the location.
-        scale: Specifies a sequence generator (or its configuration)
+        scale: A sequence generator (or its configuration)
             to generate the scale.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Cauchy, RandUniform
     >>> generator = Cauchy(
     ...     loc=RandUniform(low=-1.0, high=1.0),
     ...     scale=RandUniform(low=1.0, high=2.0),
     ... )
     >>> generator
     CauchySequenceGenerator(
@@ -75,24 +76,25 @@
 
 
 class RandCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
-        scale: Specifies the scale of the distribution.
-        feature_size: Specifies the feature size.
+        loc: The location/median of the Cauchy distribution.
+        scale: The scale of the distribution.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``scale`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandCauchy
     >>> generator = RandCauchy(loc=0.0, scale=1.0)
     >>> generator
     RandCauchySequenceGenerator(loc=0.0, scale=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -119,39 +121,40 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_cauchy(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             loc=self._loc,
             scale=self._scale,
             generator=rng,
         )
 
 
 class RandTruncCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     truncated Cauchy distribution.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
-        scale: Specifies the scale of the distribution.
-        min_value: Specifies the minimum value (included).
-        max_value: Specifies the maximum value (excluded).
-        feature_size: Specifies the feature size.
+        loc: The location/median of the Cauchy distribution.
+        scale: The scale of the distribution.
+        min_value: The minimum value (included).
+        max_value: The maximum value (excluded).
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandTruncCauchy
     >>> generator = RandTruncCauchy(loc=0.0, scale=1.0, min_value=-5.0, max_value=5.0)
     >>> generator
     RandTruncCauchySequenceGenerator(loc=0.0, scale=1.0, min_value=-5.0, max_value=5.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -187,40 +190,41 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_trunc_cauchy(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             loc=self._loc,
             scale=self._scale,
             min_value=self._min_value,
             max_value=self._max_value,
             generator=rng,
         )
 
 
 class TruncCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies a sequence generator (or its configuration) to
+        loc: A sequence generator (or its configuration) to
             generate the location.
-        scale: Specifies a sequence generator (or its configuration)
+        scale: A sequence generator (or its configuration)
             to generate the scale.
-        min_value: Specifies a sequence generator (or its
+        min_value: A sequence generator (or its
             configuration) to generate the minimum value (included).
-        max_value: Specifies a sequence generator (or its
+        max_value: A sequence generator (or its
             configuration) to generate the  maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandUniform, TruncCauchy
     >>> generator = TruncCauchy(
     ...     loc=RandUniform(low=-1.0, high=1.0),
     ...     scale=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=-10.0, high=-5.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/choice.py` & `startorch-0.1.1a0/src/startorch/sequence/choice.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,21 @@
         - a key ``'generator'`` which indicates the sequence generator
             or its configuration.
         - an optional key ``'weight'`` with a float value which
             indicates the weight of the sequence generator.
             If this key is absent, the weight is set to ``1.0``.
 
     Args:
-        sequences: Specifies the sequence generators and their weights.
+        sequences: The sequence generators and their weights.
             See above to learn about the expected format.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import MultinomialChoice, RandUniform, RandNormal
     >>> generator = MultinomialChoice(
     ...     (
     ...         {"weight": 2.0, "generator": RandUniform()},
     ...         {"weight": 1.0, "generator": RandNormal()},
     ...     )
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/constant.py` & `startorch-0.1.1a0/src/startorch/sequence/constant.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     r"""Implement a sequence generator to generate a batch of sequences
     with constant values where the values for each sequence are sampled
     from another sequence generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Constant, RandUniform
     >>> generator = Constant(RandUniform())
     >>> generator
     ConstantSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
@@ -45,20 +46,21 @@
     r"""Implement a sequence generator to generate sequences filled with
     a given value.
 
     This sequence generator is fully deterministic and the random
     seed has no effect.
 
     Args:
-        value: Specifies the value.
-        feature_size: Specifies the feature size.
+        value: The value.
+        feature_size: The feature size.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Full
     >>> generator = Full(42.0)
     >>> generator
     FullSequenceGenerator(value=42.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[[42.],
              [42.],
@@ -68,33 +70,39 @@
              [42.]],
             [[42.],
              [42.],
              [42.],
              [42.],
              [42.],
              [42.]]])
+    >>> generator = Full(42, feature_size=())
+    >>> generator
+    FullSequenceGenerator(value=42, feature_size=())
+    >>> generator.generate(seq_len=6, batch_size=2)
+    tensor([[42, 42, 42, 42, 42, 42],
+            [42, 42, 42, 42, 42, 42]])
 
     ```
     """
 
     def __init__(
         self,
         value: float,
         feature_size: tuple[int, ...] | list[int] | int = 1,
     ) -> None:
         super().__init__()
-        self._value = float(value)
+        self._value = value
         self._feature_size = to_tuple(feature_size)
 
     def __repr__(self) -> str:
         return (
             f"{self.__class__.__qualname__}(value={self._value}, "
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self,
         seq_len: int,
         batch_size: int = 1,
         rng: torch.Generator | None = None,  # noqa: ARG002
     ) -> torch.Tensor:
-        return torch.full((batch_size, seq_len) + self._feature_size, self._value)
+        return torch.full((batch_size, seq_len, *self._feature_size), self._value)
```

### Comparing `startorch-0.1.0/src/startorch/sequence/dtype.py` & `startorch-0.1.1a0/src/startorch/sequence/dtype.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class FloatSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that converts a batch of sequences
     to float type.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Float, RandInt
     >>> generator = Float(RandInt(low=0, high=10))
     >>> generator
     FloatSequenceGenerator(
       (sequence): RandIntSequenceGenerator(low=0, high=10, feature_size=())
     )
     >>> generator.generate(seq_len=6, batch_size=2)
@@ -41,14 +42,15 @@
 class LongSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that converts a batch of sequences
     to long type.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Long, RandUniform
     >>> generator = Long(RandUniform(low=0, high=10))
     >>> generator
     LongSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=10.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
```

### Comparing `startorch-0.1.0/src/startorch/sequence/exponential.py` & `startorch-0.1.1a0/src/startorch/sequence/exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,20 +33,21 @@
     Exponential distribution.
 
     The rates of the Exponential distribution are generated by the
     rate generator. The rate generator should return the rate for each
     value in the sequence.
 
     Args:
-        rate: Specifies the rate generator or its configuration.
+        rate: The rate generator or its configuration.
             The rate generator should return valid rate values.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Exponential, RandUniform
     >>> generator = Exponential(rate=RandUniform(low=1.0, high=10.0))
     >>> generator
     ExponentialSequenceGenerator(
       (rate): RandUniformSequenceGenerator(low=1.0, high=10.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
@@ -75,16 +76,16 @@
     def create_fixed_rate(
         cls, rate: float = 1.0, feature_size: tuple[int, ...] | list[int] | int = 1
     ) -> ExponentialSequenceGenerator:
         r"""Implement a sequence generator where the values are sampled
         from an Exponential distribution with a fixed rate.
 
         Args:
-            rate: Specifies the rate of the Exponential distribution.
-            feature_size: Specifies the feature size.
+            rate: The rate of the Exponential distribution.
+            feature_size: The feature size.
 
         Returns:
             A sequence generator where the rates of the Exponential
                 distribution are a fixed given value.
 
         Example usage:
 
@@ -112,17 +113,17 @@
         r"""Implement a sequence generator where the rates of the
         Exponential distribution are sampled from a uniform
         distribution.
 
         One rate is sampled per sequence.
 
         Args:
-            min_rate: Specifies the minimum rate value.
-            max_rate: Specifies the maximum rate value.
-            feature_size: Specifies the feature size.
+            min_rate: The minimum rate value.
+            max_rate: The maximum rate value.
+            feature_size: The feature size.
 
         Returns:
             A sequence generator where the rates for each sequence are
                 sampled from a uniform distribution.
 
         Example usage:
 
@@ -155,23 +156,24 @@
 
 
 class RandExponentialSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequences by sampling values from
     an Exponential distribution.
 
     Args:
-        rate: Specifies the rate of the Exponential distribution.
-        feature_size: Specifies the feature size.
+        rate: The rate of the Exponential distribution.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandExponential
     >>> generator = RandExponential(rate=1.0)
     >>> generator
     RandExponentialSequenceGenerator(rate=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -196,36 +198,37 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_exponential(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             rate=self._rate,
             generator=rng,
         )
 
 
 class RandTruncExponentialSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequences by sampling values from a
     truncated Exponential distribution.
 
     Args:
-        rate: Specifies the rate of the Exponential distribution.
-        max_value: Specifies the maximum value.
-        feature_size: Specifies the feature size.
+        rate: The rate of the Exponential distribution.
+        max_value: The maximum value.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandTruncExponential
     >>> generator = RandTruncExponential(rate=1.0, max_value=3.0)
     >>> generator
     RandTruncExponentialSequenceGenerator(rate=1.0, max_value=3.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -255,34 +258,35 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_trunc_exponential(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             rate=self._rate,
             max_value=self._max_value,
             generator=rng,
         )
 
 
 class TruncExponentialSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from an
     Exponential distribution.
 
     Args:
-        rate: Specifies a sequence generator (or its configuration)
+        rate: A sequence generator (or its configuration)
             to generate the rate.
-        max_value: Specifies a sequence generator (or its
+        max_value: A sequence generator (or its
             configuration) to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandUniform, TruncExponential
     >>> generator = TruncExponential(
     ...     rate=RandUniform(low=1.0, high=10.0),
     ...     max_value=RandUniform(low=1.0, high=100.0),
     ... )
     >>> generator
     TruncExponentialSequenceGenerator(
```

### Comparing `startorch-0.1.0/src/startorch/sequence/halfcauchy.py` & `startorch-0.1.1a0/src/startorch/sequence/halfnormal.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,229 +1,228 @@
 r"""Contain the implementation of sequence generators where the values
-are sampled from a half-Cauchy distribution."""
+are sampled from a half-Normal distribution."""
 
 from __future__ import annotations
 
 __all__ = [
-    "HalfCauchySequenceGenerator",
-    "RandHalfCauchySequenceGenerator",
-    "RandTruncHalfCauchySequenceGenerator",
-    "TruncHalfCauchySequenceGenerator",
+    "HalfNormalSequenceGenerator",
+    "RandHalfNormalSequenceGenerator",
+    "RandTruncHalfNormalSequenceGenerator",
+    "TruncHalfNormalSequenceGenerator",
 ]
 
 from typing import TYPE_CHECKING
 
 from coola.utils.format import str_indent, str_mapping
 
 from startorch.random import (
-    half_cauchy,
-    rand_half_cauchy,
-    rand_trunc_half_cauchy,
-    trunc_half_cauchy,
+    half_normal,
+    rand_half_normal,
+    rand_trunc_half_normal,
+    trunc_half_normal,
 )
 from startorch.sequence.base import BaseSequenceGenerator, setup_sequence_generator
 from startorch.utils.conversion import to_tuple
 
 if TYPE_CHECKING:
     import torch
 
 
-class HalfCauchySequenceGenerator(BaseSequenceGenerator):
+class HalfNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Cauchy distribution.
+    half-Normal distribution.
 
     Args:
-        scale: Specifies a sequence generator (or its configuration)
-            to generate the scale.
+        std: A sequence generator (or its configuration)
+            to generate the standard deviation.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import HalfCauchy, RandUniform
-    >>> generator = HalfCauchy(scale=RandUniform(low=1.0, high=2.0))
+
+    >>> from startorch.sequence import HalfNormal, RandUniform
+    >>> generator = HalfNormal(std=RandUniform(low=1.0, high=2.0))
     >>> generator
-    HalfCauchySequenceGenerator(
-      (scale): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
+    HalfNormalSequenceGenerator(
+      (std): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
-    def __init__(self, scale: BaseSequenceGenerator | dict) -> None:
+    def __init__(self, std: BaseSequenceGenerator | dict) -> None:
         super().__init__()
-        self._scale = setup_sequence_generator(scale)
+        self._std = setup_sequence_generator(std)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"scale": self._scale}))
+        args = str_indent(str_mapping({"std": self._std}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
-    ) -> torch.tensor:
-        return half_cauchy(
-            scale=self._scale.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
+    ) -> torch.Tensor:
+        return half_normal(
+            std=self._std.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             generator=rng,
         )
 
 
-class RandHalfCauchySequenceGenerator(BaseSequenceGenerator):
+class RandHalfNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Cauchy distribution.
+    half-Normal distribution.
 
     Args:
-        scale: Specifies the scale of the distribution.
-        feature_size: Specifies the feature size.
+        std: The std of the distribution.
+        feature_size: The feature size.
 
     Raises:
-        ValueError: if ``scale`` is not a positive number.
+        ValueError: if ``std`` is not a positive number.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandHalfCauchy
-    >>> generator = RandHalfCauchy(scale=1.0)
+
+    >>> from startorch.sequence import RandHalfNormal
+    >>> generator = RandHalfNormal(std=1.0)
     >>> generator
-    RandHalfCauchySequenceGenerator(scale=1.0, feature_size=(1,))
+    RandHalfNormalSequenceGenerator(std=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
-        self,
-        scale: float = 1.0,
-        feature_size: tuple[int, ...] | list[int] | int = 1,
+        self, std: float = 1.0, feature_size: tuple[int, ...] | list[int] | int = 1
     ) -> None:
         super().__init__()
-        if scale <= 0:
-            msg = f"scale has to be greater than 0 (received: {scale})"
+        if std <= 0:
+            msg = f"std has to be greater than 0 (received: {std})"
             raise ValueError(msg)
-        self._scale = float(scale)
+        self._std = float(std)
         self._feature_size = to_tuple(feature_size)
 
     def __repr__(self) -> str:
-        return (
-            f"{self.__class__.__qualname__}(scale={self._scale}, "
-            f"feature_size={self._feature_size})"
-        )
+        return f"{self.__class__.__qualname__}(std={self._std}, feature_size={self._feature_size})"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return rand_half_cauchy(
-            size=(batch_size, seq_len) + self._feature_size,
-            scale=self._scale,
+        return rand_half_normal(
+            size=(batch_size, seq_len, *self._feature_size),
+            std=self._std,
             generator=rng,
         )
 
 
-class RandTruncHalfCauchySequenceGenerator(BaseSequenceGenerator):
+class RandTruncHalfNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    truncated half-Cauchy distribution.
+    truncated half-Normal distribution.
 
     Args:
-        scale: Specifies the scale of the distribution.
-        max_value: Specifies the maximum value.
-        feature_size: Specifies the feature size.
+        std: The std of the distribution.
+        max_value: The maximum value.
+        feature_size: The feature size.
 
     Raises:
-        ValueError: if ``scale`` is not a positive number.
+        ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandTruncHalfCauchy
-    >>> generator = RandTruncHalfCauchy(scale=1.0, max_value=5.0)
+
+    >>> from startorch.sequence import RandTruncHalfNormal
+    >>> generator = RandTruncHalfNormal(std=1.0, max_value=1.0)
     >>> generator
-    RandTruncHalfCauchySequenceGenerator(scale=1.0, max_value=5.0, feature_size=(1,))
+    RandTruncHalfNormalSequenceGenerator(std=1.0, max_value=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
         self,
-        scale: float = 1.0,
-        max_value: float = 4.0,
+        std: float = 1.0,
+        max_value: float = 3.0,
         feature_size: tuple[int, ...] | list[int] | int = 1,
     ) -> None:
         super().__init__()
-        if scale <= 0:
-            msg = f"scale has to be greater than 0 (received: {scale})"
+        if std <= 0:
+            msg = f"std has to be greater than 0 (received: {std})"
             raise ValueError(msg)
-        self._scale = float(scale)
+        self._std = float(std)
         if max_value <= 0:
             msg = f"max_value has to be greater than 0 (received: {max_value})"
             raise ValueError(msg)
         self._max_value = float(max_value)
         self._feature_size = to_tuple(feature_size)
 
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__qualname__}(scale={self._scale}, max_value={self._max_value}, "
+            f"{self.__class__.__qualname__}(std={self._std}, max_value={self._max_value}, "
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return rand_trunc_half_cauchy(
-            size=(batch_size, seq_len) + self._feature_size,
-            scale=self._scale,
+        return rand_trunc_half_normal(
+            size=(batch_size, seq_len, *self._feature_size),
+            std=self._std,
             max_value=self._max_value,
             generator=rng,
         )
 
 
-class TruncHalfCauchySequenceGenerator(BaseSequenceGenerator):
+class TruncHalfNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Cauchy distribution.
+    half-Normal distribution.
 
     Args:
-        scale: Specifies a sequence generator (or its configuration)
-            to generate the scale.
-        max_value: Specifies a sequence generator (or its
+        std: A sequence generator (or its configuration) to
+            generate the std.
+        max_value: A sequence generator (or its
             configuration) to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandUniform, TruncHalfCauchy
-    >>> generator = TruncHalfCauchy(
-    ...     scale=RandUniform(low=1.0, high=2.0),
+
+    >>> from startorch.sequence import RandUniform, TruncHalfNormal
+    >>> generator = TruncHalfNormal(
+    ...     std=RandUniform(low=1.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
     >>> generator
-    TruncHalfCauchySequenceGenerator(
-      (scale): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
+    TruncHalfNormalSequenceGenerator(
+      (std): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
       (max_value): RandUniformSequenceGenerator(low=5.0, high=10.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
-        self, scale: BaseSequenceGenerator | dict, max_value: BaseSequenceGenerator | dict
+        self, std: BaseSequenceGenerator | dict, max_value: BaseSequenceGenerator | dict
     ) -> None:
         super().__init__()
-        self._scale = setup_sequence_generator(scale)
+        self._std = setup_sequence_generator(std)
         self._max_value = setup_sequence_generator(max_value)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"scale": self._scale, "max_value": self._max_value}))
+        args = str_indent(str_mapping({"std": self._std, "max_value": self._max_value}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return trunc_half_cauchy(
-            scale=self._scale.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
+        return trunc_half_normal(
+            std=self._std.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             max_value=self._max_value.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             generator=rng,
         )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/halfnormal.py` & `startorch-0.1.1a0/src/startorch/sequence/halfcauchy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,224 +1,233 @@
 r"""Contain the implementation of sequence generators where the values
-are sampled from a half-Normal distribution."""
+are sampled from a half-Cauchy distribution."""
 
 from __future__ import annotations
 
 __all__ = [
-    "HalfNormalSequenceGenerator",
-    "RandHalfNormalSequenceGenerator",
-    "RandTruncHalfNormalSequenceGenerator",
-    "TruncHalfNormalSequenceGenerator",
+    "HalfCauchySequenceGenerator",
+    "RandHalfCauchySequenceGenerator",
+    "RandTruncHalfCauchySequenceGenerator",
+    "TruncHalfCauchySequenceGenerator",
 ]
 
 from typing import TYPE_CHECKING
 
 from coola.utils.format import str_indent, str_mapping
 
 from startorch.random import (
-    half_normal,
-    rand_half_normal,
-    rand_trunc_half_normal,
-    trunc_half_normal,
+    half_cauchy,
+    rand_half_cauchy,
+    rand_trunc_half_cauchy,
+    trunc_half_cauchy,
 )
 from startorch.sequence.base import BaseSequenceGenerator, setup_sequence_generator
 from startorch.utils.conversion import to_tuple
 
 if TYPE_CHECKING:
     import torch
 
 
-class HalfNormalSequenceGenerator(BaseSequenceGenerator):
+class HalfCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Normal distribution.
+    half-Cauchy distribution.
 
     Args:
-        std: Specifies a sequence generator (or its configuration)
-            to generate the standard deviation.
+        scale: A sequence generator (or its configuration)
+            to generate the scale.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import HalfNormal, RandUniform
-    >>> generator = HalfNormal(std=RandUniform(low=1.0, high=2.0))
+
+    >>> from startorch.sequence import HalfCauchy, RandUniform
+    >>> generator = HalfCauchy(scale=RandUniform(low=1.0, high=2.0))
     >>> generator
-    HalfNormalSequenceGenerator(
-      (std): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
+    HalfCauchySequenceGenerator(
+      (scale): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
-    def __init__(self, std: BaseSequenceGenerator | dict) -> None:
+    def __init__(self, scale: BaseSequenceGenerator | dict) -> None:
         super().__init__()
-        self._std = setup_sequence_generator(std)
+        self._scale = setup_sequence_generator(scale)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"std": self._std}))
+        args = str_indent(str_mapping({"scale": self._scale}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
-    ) -> torch.Tensor:
-        return half_normal(
-            std=self._std.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
+    ) -> torch.tensor:
+        return half_cauchy(
+            scale=self._scale.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             generator=rng,
         )
 
 
-class RandHalfNormalSequenceGenerator(BaseSequenceGenerator):
+class RandHalfCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Normal distribution.
+    half-Cauchy distribution.
 
     Args:
-        std: Specifies the std of the distribution.
-        feature_size: Specifies the feature size.
+        scale: The scale of the distribution.
+        feature_size: The feature size.
 
     Raises:
-        ValueError: if ``std`` is not a positive number.
+        ValueError: if ``scale`` is not a positive number.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandHalfNormal
-    >>> generator = RandHalfNormal(std=1.0)
+
+    >>> from startorch.sequence import RandHalfCauchy
+    >>> generator = RandHalfCauchy(scale=1.0)
     >>> generator
-    RandHalfNormalSequenceGenerator(std=1.0, feature_size=(1,))
+    RandHalfCauchySequenceGenerator(scale=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
-        self, std: float = 1.0, feature_size: tuple[int, ...] | list[int] | int = 1
+        self,
+        scale: float = 1.0,
+        feature_size: tuple[int, ...] | list[int] | int = 1,
     ) -> None:
         super().__init__()
-        if std <= 0:
-            msg = f"std has to be greater than 0 (received: {std})"
+        if scale <= 0:
+            msg = f"scale has to be greater than 0 (received: {scale})"
             raise ValueError(msg)
-        self._std = float(std)
+        self._scale = float(scale)
         self._feature_size = to_tuple(feature_size)
 
     def __repr__(self) -> str:
-        return f"{self.__class__.__qualname__}(std={self._std}, feature_size={self._feature_size})"
+        return (
+            f"{self.__class__.__qualname__}(scale={self._scale}, "
+            f"feature_size={self._feature_size})"
+        )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return rand_half_normal(
-            size=(batch_size, seq_len) + self._feature_size,
-            std=self._std,
+        return rand_half_cauchy(
+            size=(batch_size, seq_len, *self._feature_size),
+            scale=self._scale,
             generator=rng,
         )
 
 
-class RandTruncHalfNormalSequenceGenerator(BaseSequenceGenerator):
+class RandTruncHalfCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    truncated half-Normal distribution.
+    truncated half-Cauchy distribution.
 
     Args:
-        std: Specifies the std of the distribution.
-        max_value: Specifies the maximum value.
-        feature_size: Specifies the feature size.
+        scale: The scale of the distribution.
+        max_value: The maximum value.
+        feature_size: The feature size.
 
     Raises:
-        ValueError: if ``std`` is not a positive number.
+        ValueError: if ``scale`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandTruncHalfNormal
-    >>> generator = RandTruncHalfNormal(std=1.0, max_value=1.0)
+
+    >>> from startorch.sequence import RandTruncHalfCauchy
+    >>> generator = RandTruncHalfCauchy(scale=1.0, max_value=5.0)
     >>> generator
-    RandTruncHalfNormalSequenceGenerator(std=1.0, max_value=1.0, feature_size=(1,))
+    RandTruncHalfCauchySequenceGenerator(scale=1.0, max_value=5.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
         self,
-        std: float = 1.0,
-        max_value: float = 3.0,
+        scale: float = 1.0,
+        max_value: float = 4.0,
         feature_size: tuple[int, ...] | list[int] | int = 1,
     ) -> None:
         super().__init__()
-        if std <= 0:
-            msg = f"std has to be greater than 0 (received: {std})"
+        if scale <= 0:
+            msg = f"scale has to be greater than 0 (received: {scale})"
             raise ValueError(msg)
-        self._std = float(std)
+        self._scale = float(scale)
         if max_value <= 0:
             msg = f"max_value has to be greater than 0 (received: {max_value})"
             raise ValueError(msg)
         self._max_value = float(max_value)
         self._feature_size = to_tuple(feature_size)
 
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__qualname__}(std={self._std}, max_value={self._max_value}, "
+            f"{self.__class__.__qualname__}(scale={self._scale}, max_value={self._max_value}, "
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return rand_trunc_half_normal(
-            size=(batch_size, seq_len) + self._feature_size,
-            std=self._std,
+        return rand_trunc_half_cauchy(
+            size=(batch_size, seq_len, *self._feature_size),
+            scale=self._scale,
             max_value=self._max_value,
             generator=rng,
         )
 
 
-class TruncHalfNormalSequenceGenerator(BaseSequenceGenerator):
+class TruncHalfCauchySequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
-    half-Normal distribution.
+    half-Cauchy distribution.
 
     Args:
-        std: Specifies a sequence generator (or its configuration) to
-            generate the std.
-        max_value: Specifies a sequence generator (or its
+        scale: A sequence generator (or its configuration)
+            to generate the scale.
+        max_value: A sequence generator (or its
             configuration) to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
-    >>> from startorch.sequence import RandUniform, TruncHalfNormal
-    >>> generator = TruncHalfNormal(
-    ...     std=RandUniform(low=1.0, high=2.0),
+
+    >>> from startorch.sequence import RandUniform, TruncHalfCauchy
+    >>> generator = TruncHalfCauchy(
+    ...     scale=RandUniform(low=1.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
     >>> generator
-    TruncHalfNormalSequenceGenerator(
-      (std): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
+    TruncHalfCauchySequenceGenerator(
+      (scale): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
       (max_value): RandUniformSequenceGenerator(low=5.0, high=10.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
     ```
     """
 
     def __init__(
-        self, std: BaseSequenceGenerator | dict, max_value: BaseSequenceGenerator | dict
+        self, scale: BaseSequenceGenerator | dict, max_value: BaseSequenceGenerator | dict
     ) -> None:
         super().__init__()
-        self._std = setup_sequence_generator(std)
+        self._scale = setup_sequence_generator(scale)
         self._max_value = setup_sequence_generator(max_value)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"std": self._std, "max_value": self._max_value}))
+        args = str_indent(str_mapping({"scale": self._scale, "max_value": self._max_value}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return trunc_half_normal(
-            std=self._std.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
+        return trunc_half_cauchy(
+            scale=self._scale.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             max_value=self._max_value.generate(seq_len=seq_len, batch_size=batch_size, rng=rng),
             generator=rng,
         )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/joining.py` & `startorch-0.1.1a0/src/startorch/sequence/joining.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,24 +20,25 @@
 class Cat2SequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator that concatenate two sequences
     along the sequence dimension.
 
     ``ouput = [sequence1, sequence2]``
 
     Args:
-        generator1: Specifies the first sequence generator or its
+        generator1: The first sequence generator or its
             configuration.
-        generator2: Specifies the second sequence generator or its
+        generator2: The second sequence generator or its
             configuration.
-        changepoint: Specifies the change point generator or its
+        changepoint: The change point generator or its
             configuration.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Cat2, RandUniform, RandNormal
     >>> from startorch.tensor import RandInt
     >>> generator = Cat2(
     ...     generator1=RandUniform(), generator2=RandNormal(), changepoint=RandInt(0, 12)
     ... )
     >>> generator
```

### Comparing `startorch-0.1.0/src/startorch/sequence/linear.py` & `startorch-0.1.1a0/src/startorch/sequence/linear.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,25 +20,26 @@
     linear pattern.
 
     The sequences are generated by using the following formula:
 
     ``output = slope * value + intercept``
 
     Args:
-        value: Specifies a sequence generator (or its configuration)
+        value: A sequence generator (or its configuration)
             to generate the sequence values. The linear transformation
             is applied on these values.
-        slope: Specifies a sequence generator (or its configuration)
+        slope: A sequence generator (or its configuration)
             to generate the slope values.
-        intercept: Specifies a sequence generator (or its
+        intercept: A sequence generator (or its
             configuration) to generate the intercept values.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Linear, RandUniform
     >>> generator = Linear(
     ...     value=RandUniform(low=-1.0, high=1.0),
     ...     slope=RandUniform(low=1.0, high=2.0),
     ...     intercept=RandUniform(low=-10.0, high=-5.0),
     ... )
     >>> generator
```

### Comparing `startorch-0.1.0/src/startorch/sequence/lognormal.py` & `startorch-0.1.1a0/src/startorch/sequence/lognormal.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,23 +28,24 @@
 
 
 class LogNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     log-Normal distribution.
 
     Args:
-        mean: Specifies a sequence generator (or its configuration) to
+        mean: A sequence generator (or its configuration) to
             generate the mean of the underlying Normal distribution.
-        std: Specifies a sequence generator (or its configuration) to
+        std: A sequence generator (or its configuration) to
             generate the standard deviation of the underlying Normal
             distribution.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import LogNormal, RandUniform
     >>> generator = LogNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0), std=RandUniform(low=1.0, high=2.0)
     ... )
     >>> generator
     LogNormalSequenceGenerator(
       (mean): RandUniformSequenceGenerator(low=-1.0, high=1.0, feature_size=(1,))
@@ -78,25 +79,26 @@
 
 
 class RandLogNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     log-Normal distribution.
 
     Args:
-        mean: Specifies the mean of the underlying Normal distribution.
-        std: Specifies the standard deviation of the underlying Normal
+        mean: The mean of the underlying Normal distribution.
+        std: The standard deviation of the underlying Normal
             distribution.
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandLogNormal
     >>> generator = RandLogNormal(mean=0.0, std=1.0)
     >>> generator
     RandLogNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -123,40 +125,41 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_log_normal(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             mean=self._mean,
             std=self._std,
             generator=rng,
         )
 
 
 class RandTruncLogNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate cyclic sequences by
     sampling values from a truncated log-Normal distribution.
 
     Args:
-        mean: Specifies the mean of the log-Normal distribution.
-        std: Specifies the standard deviation of the log-Normal
+        mean: The mean of the log-Normal distribution.
+        std: The standard deviation of the log-Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
-        feature_size: Specifies the feature size.
+        min_value: The minimum value.
+        max_value: The maximum value.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandTruncLogNormal
     >>> generator = RandTruncLogNormal(mean=0.0, std=1.0, min_value=0.0, max_value=1.0)
     >>> generator
     RandTruncLogNormalSequenceGenerator(mean=0.0, std=1.0, min_value=0.0, max_value=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -191,44 +194,45 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_trunc_log_normal(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             mean=self._mean,
             std=self._std,
             min_value=self._min_value,
             max_value=self._max_value,
             generator=rng,
         )
 
 
 class TruncLogNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     truncated log-Normal distribution.
 
     Args:
-        mean: Specifies a sequence
+        mean: A sequence
             generator (or its configuration) to generate the mean of
             the underlying Normal distribution.
-        std: Specifies a sequence
+        std: A sequence
             generator (or its configuration) to generate the standard
             deviation of the underlying Normal distribution.
-        min_value: Specifies a
+        min_value: A
             sequence generator (or its configuration) to generate the
             minimum value (included).
-        max_value: Specifies a
+        max_value: A
             sequence generator (or its configuration) to generate the
             maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandUniform, TruncLogNormal
     >>> generator = TruncLogNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0),
     ...     std=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=0.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/math.py` & `startorch-0.1.1a0/src/startorch/sequence/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 class AbsSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the absolute value
     of a generated sequence.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Abs, RandNormal
     >>> generator = Abs(RandNormal())
     >>> generator
     AbsSequenceGenerator(
       (sequence): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
     )
@@ -63,23 +64,24 @@
 
 class AddSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator that adds multiple sequences.
 
     ``sequence = sequence_1 + sequence_2 + ... + sequence_n``
 
     Args:
-        sequences: Specifies the sequence generators or
+        sequences: The sequence generators or
             their configuration.
 
     Raises:
         ValueError: if no sequence generator is provided.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Add, RandUniform, RandNormal
     >>> generator = Add([RandUniform(), RandNormal()])
     >>> generator
     AddSequenceGenerator(
       (0): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (1): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
@@ -110,21 +112,22 @@
 
 
 class AddScalarSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that adds a scalar value to a
     generated batch of sequences.
 
     Args:
-        generator: Specifies the sequence generator or its
+        generator: The sequence generator or its
             configuration.
-        value: Specifies the scalar value to add.
+        value: The scalar value to add.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import AddScalar, RandUniform, RandNormal
     >>> generator = AddScalar(RandUniform(), 42.0)
     >>> generator
     AddScalarSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (value): 42.0
@@ -158,27 +161,28 @@
 class ClampSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator to generate a batch of sequences
     where the values are clamped.
 
     Note: ``min_value`` and ``max_value`` cannot be both ``None``.
 
     Args:
-        generator: Specifies the sequence generator or its
+        generator: The sequence generator or its
             configuration.
-        min: Specifies the lower bound. If ``min_value`` is ``None``,
+        min: The lower bound. If ``min_value`` is ``None``,
             there is no lower bound.
-        max: Specifies the upper bound. If ``max_value`` is ``None``,
+        max: The upper bound. If ``max_value`` is ``None``,
             there is no upper bound.
 
     Raises:
         ValueError: if both ``min`` and ``max`` are ``None``
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Clamp, RandNormal
     >>> generator = Clamp(RandNormal(), -1.0, 1.0)
     >>> generator
     ClampSequenceGenerator(
       (sequence): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
       (min): -1.0
@@ -220,14 +224,15 @@
 class CumsumSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the cumulative sum
     of a generated sequence.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Cumsum, RandUniform
     >>> generator = Cumsum(RandUniform())
     >>> generator
     CumsumSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -248,29 +253,30 @@
 class DivSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator that divides one sequence by
     another one.
 
     ``sequence = dividend / divisor`` (a.k.a. true division)
 
     Args:
-        dividend: Specifies the dividend sequence generator or its
+        dividend: The dividend sequence generator or its
             configuration.
-        divisor: Specifies the divisor sequence generator or its
+        divisor: The divisor sequence generator or its
             configuration.
-        rounding_mode: Specifies the type of rounding applied to the
+        rounding_mode: The type of rounding applied to the
             result:
                 - ``None``: true division.
                 - ``"trunc"``: rounds the results of the division
                     towards zero.
                 - ``"floor"``: floor division.
 
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Div, RandUniform, RandNormal
     >>> generator = Div(RandNormal(), RandUniform(1.0, 10.0))
     >>> generator
     DivSequenceGenerator(
       (dividend): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
       (divisor): RandUniformSequenceGenerator(low=1.0, high=10.0, feature_size=(1,))
@@ -317,14 +323,15 @@
 class ExpSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the exponential of a
     batch of sequences.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Exp, RandUniform, RandNormal
     >>> generator = Exp(RandUniform())
     >>> generator
     ExpSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -341,21 +348,22 @@
 
 
 class FmodSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a tensor generator that computes the element-wise
     remainder of division.
 
     Args:
-        dividend: Specifies the sequence generator (or its
+        dividend: The sequence generator (or its
             configuration) that generates the dividend values.
-        divisor: Specifies the divisor.
+        divisor: The divisor.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Fmod, RandUniform
     >>> generator = Fmod(dividend=RandUniform(low=-100, high=100), divisor=10.0)
     >>> generator
     FmodSequenceGenerator(
       (dividend): RandUniformSequenceGenerator(low=-100.0, high=100.0, feature_size=(1,))
       (divisor): 10.0
     )
@@ -402,14 +410,15 @@
 class LogSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the logarithm of a
     batch of sequences.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Log, RandUniform, RandNormal
     >>> generator = Log(RandUniform(1.0, 10.0))
     >>> generator
     LogSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=1.0, high=10.0, feature_size=(1,))
     )
@@ -428,22 +437,23 @@
 class MulSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator that multiplies multiple
     sequences.
 
     ``sequence = sequence_1 * sequence_2 * ... * sequence_n``
 
     Args:
-        sequences: Specifies the sequence generators.
+        sequences: The sequence generators.
 
     Raises:
         ValueError: if no sequence generator is provided.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Mul, RandUniform, RandNormal
     >>> generator = Mul([RandUniform(), RandNormal()])
     >>> generator
     MulSequenceGenerator(
       (0): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (1): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
@@ -477,21 +487,22 @@
 
 
 class MulScalarSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that multiplies a scalar value to
     a generated batch of sequences.
 
     Args:
-        generator: Specifies the sequence generator or its
+        generator: The sequence generator or its
             configuration.
-        value: Specifies the scalar value to multiply.
+        value: The scalar value to multiply.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import MulScalar, RandUniform, RandNormal
     >>> generator = MulScalar(RandUniform(), 2.0)
     >>> generator
     MulScalarSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (value): 2.0
@@ -525,14 +536,15 @@
 class NegSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the negation of a
     generated sequence.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Neg, RandUniform, RandNormal
     >>> generator = Neg(RandUniform())
     >>> generator
     NegSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -551,14 +563,15 @@
 class SqrtSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the squared root of
     a batch of sequences.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Sqrt, RandUniform, RandNormal
     >>> generator = Sqrt(RandUniform(1.0, 4.0))
     >>> generator
     SqrtSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=1.0, high=4.0, feature_size=(1,))
     )
@@ -576,22 +589,23 @@
 
 class SubSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator that subtracts sequences.
 
     ``sequence = sequence_1 - sequence_2``
 
     Args:
-        sequence1: Specifies the first sequence generator or its
+        sequence1: The first sequence generator or its
             configuration.
-        sequence2: Specifies the second sequence generator or its
+        sequence2: The second sequence generator or its
             configuration.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Sub, RandUniform, RandNormal
     >>> generator = Sub(RandUniform(), RandNormal())
     >>> generator
     SubSequenceGenerator(
       (sequence1): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (sequence2): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
```

### Comparing `startorch-0.1.0/src/startorch/sequence/normal.py` & `startorch-0.1.1a0/src/startorch/sequence/normal.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,22 +23,23 @@
 
 
 class NormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Normal distribution.
 
     Args:
-        mean: Specifies a sequence generator (or its configuration)
+        mean: A sequence generator (or its configuration)
             to generate the mean.
-        std: Specifies a sequence generator (or its configuration) to
+        std: A sequence generator (or its configuration) to
             generate the standard deviation.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Normal, RandUniform
     >>> generator = Normal(
     ...     mean=RandUniform(low=-1.0, high=1.0), std=RandUniform(low=1.0, high=2.0)
     ... )
     >>> generator
     NormalSequenceGenerator(
       (mean): RandUniformSequenceGenerator(low=-1.0, high=1.0, feature_size=(1,))
@@ -72,25 +73,26 @@
 
 
 class RandNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate cyclic sequences by
     sampling values from a Normal distribution.
 
     Args:
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandNormal
     >>> generator = RandNormal(mean=0.0, std=1.0)
     >>> generator
     RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -117,32 +119,32 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_normal(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             mean=self._mean,
             std=self._std,
             generator=rng,
         )
 
 
 class RandTruncNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate cyclic sequences by
     sampling values from a truncated Normal distribution.
 
     Args:
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
-        feature_size: Specifies the feature size.
+        min_value: The minimum value.
+        max_value: The maximum value.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
@@ -186,43 +188,44 @@
             f"feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_trunc_normal(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             mean=self._mean,
             std=self._std,
             min_value=self._min_value,
             max_value=self._max_value,
             generator=rng,
         )
 
 
 class TruncNormalSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     truncated Normal distribution.
 
     Args:
-        mean: Specifies a sequence
+        mean: A sequence
             generator (or its configuration) to generate the mean.
-        std: Specifies a sequence
+        std: A sequence
             generator (or its configuration) to generate the standard
             deviation.
-        min_value: Specifies a
+        min_value: A
             sequence generator (or its configuration) to generate the
             minimum value (included).
-        max_value: Specifies a
+        max_value: A
             sequence generator (or its configuration) to generate the
             maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandUniform, TruncNormal
     >>> generator = TruncNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0),
     ...     std=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=-10.0, high=-5.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/periodic.py` & `startorch-0.1.1a0/src/startorch/sequence/periodic.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,23 +20,24 @@
 
 
 class PeriodicSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate periodic sequence from
     a regular sequence generator.
 
     Args:
-        sequence: Specifies a sequence generator or its configuration
+        sequence: A sequence generator or its configuration
             that is used to generate the periodic pattern.
-        period: Specifies the period length sampler or its
+        period: The period length sampler or its
             configuration. This sampler is used to sample the period
             length at each batch.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Periodic, RandUniform
     >>> from startorch.tensor import RandInt
     >>> generator = Periodic(sequence=RandUniform(), period=RandInt(2, 5))
     >>> generator
     PeriodicSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (period): RandIntTensorGenerator(low=2, high=5)
```

### Comparing `startorch-0.1.0/src/startorch/sequence/poisson.py` & `startorch-0.1.1a0/src/startorch/sequence/poisson.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,20 +20,21 @@
     Poisson distribution.
 
     The rates of the Poisson distribution are generated by the rate
     generator. The rate generator should return the rate for each value
     in the sequence. The rate values should be greater than 0.
 
     Args:
-        rate: Specifies the rate generator or its configuration.
+        rate: The rate generator or its configuration.
             The rate generator should return valid rate values.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandUniform, Poisson
     >>> generator = Poisson(rate=RandUniform(low=1.0, high=2.0))
     >>> generator
     PoissonSequenceGenerator(
       (rate): RandUniformSequenceGenerator(low=1.0, high=2.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=6, batch_size=2)
@@ -65,17 +66,17 @@
         max_rate: float = 1.0,
         feature_size: tuple[int, ...] | list[int] | int = 1,
     ) -> PoissonSequenceGenerator:
         r"""Implement a sequence generator where the rates of the Poisson
         distribution are sampled from a uniform distribution.
 
         Args:
-            min_rate: Specifies the minimum rate value.
-            max_rate: Specifies the maximum rate value.
-            feature_size: Specifies the feature size.
+            min_rate: The minimum rate value.
+            max_rate: The maximum rate value.
+            feature_size: The feature size.
 
         Returns:
             A sequence generator where the rates of the Poisson
                 distribution are sampled from a uniform distribution
                 (``UniformConstantSequenceGenerator``).
         """
         # The import is here to do not generate circular dependencies
@@ -93,24 +94,25 @@
 
 
 class RandPoissonSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Poisson distribution.
 
     Args:
-        rate: Specifies the rate of the Poisson distribution.
+        rate: The rate of the Poisson distribution.
             This value has to be greater than 0.
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandPoisson
     >>> generator = RandPoisson(rate=1.0)
     >>> generator
     RandPoissonSequenceGenerator(rate=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -134,11 +136,11 @@
             f"{self.__class__.__qualname__}(rate={self._rate}, feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_poisson(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             rate=self._rate,
             generator=rng,
         )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/range.py` & `startorch-0.1.1a0/src/startorch/sequence/range.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 
 
 class ArangeSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequence of consecutive integer
     values between ``0`` and ``seq_len-1``.
 
     Args:
-        feature_size: Specifies the feature size.
+        feature_size: The feature size.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import Arange
     >>> generator = Arange(feature_size=())
     >>> generator
     ArangeSequenceGenerator(feature_size=())
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[0, 1, 2, 3, 4, 5],
             [0, 1, 2, 3, 4, 5]])
```

### Comparing `startorch-0.1.0/src/startorch/sequence/sort.py` & `startorch-0.1.1a0/src/startorch/sequence/sort.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     from startorch.sequence.base import BaseSequenceGenerator
 
 
 class SortSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that sorts a generated sequence.
 
     Args:
-        sequence: Specifies the sequence generator or its
-            configuration.
-        descending: Controls the sorting order. If ``True``,
+        generator: The sequence generator or its configuration.
+        descending: Control the sorting order. If ``True``,
             the elements are sorted in descending order by value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform, Sort
     >>> generator = Sort(RandUniform())
     >>> generator
     SortSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/tensor.py` & `startorch-0.1.1a0/src/startorch/sequence/tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,21 @@
 
 
 class TensorSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences from a
     tensor generator.
 
     Args:
-        tensor: Specifies a tensor generator (or its configuration).
-        feature_size: Specifies the feature size.
+        tensor: A tensor generator (or its configuration).
+        feature_size: The feature size.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import TensorSequence
     >>> from startorch.tensor import RandUniform
     >>> generator = TensorSequence(RandUniform())
     >>> generator
     TensorSequenceGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
@@ -55,8 +56,8 @@
     def __repr__(self) -> str:
         args = str_indent(str_mapping({"tensor": self._tensor, "feature_size": self._feature_size}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
-        return self._tensor.generate(size=(batch_size, seq_len) + self._feature_size, rng=rng)
+        return self._tensor.generate(size=(batch_size, seq_len, *self._feature_size), rng=rng)
```

### Comparing `startorch-0.1.0/src/startorch/sequence/time.py` & `startorch-0.1.1a0/src/startorch/sequence/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
        - ``1.2`` -> ``00:00:01.200``
        - ``61.2`` -> ``00:01:01.200``
        - ``3661.2`` -> ``01:01:01.200``
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform, Time
     >>> generator = Time(RandUniform())
     >>> generator
     TimeSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -53,15 +54,15 @@
     @classmethod
     def create_exponential_constant_time_diff(cls, rate: float = 1.0) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps is constant and is sampled from an
         exponential distribution.
 
         Args:
-            rate: Specifies the rate of the exponential distribution.
+            rate: The rate of the exponential distribution.
 
         Returns:
             A time sequence generator where the time difference
                 between two consecutive steps is constant and is
                 sampled from an exponential distribution.
 
         Example usage:
@@ -102,15 +103,15 @@
     @classmethod
     def create_exponential_time_diff(cls, rate: float = 1.0) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps follows an exponential
         distribution.
 
         Args:
-            rate: Specifies the rate of the exponential distribution.
+            rate: The rate of the exponential distribution.
 
         Returns:
             A time sequence generator where the time difference between
                 two consecutive steps follows an exponential
                 distribution.
 
         Example usage:
@@ -147,15 +148,15 @@
     @classmethod
     def create_poisson_constant_time_diff(cls, rate: float = 1.0) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps is constant and is sampled from a
         Poisson distribution.
 
         Args:
-            rate: Specifies the rate of the Poisson distribution.
+            rate: The rate of the Poisson distribution.
 
         Returns:
             A time sequence generator where the time difference
                 between two consecutive steps is constant and is
                 sampled from a Poisson distribution.
 
         Example usage:
@@ -185,15 +186,15 @@
 
     @classmethod
     def create_poisson_time_diff(cls, rate: float = 1.0) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps follows a Poisson distribution.
 
         Args:
-            rate: Specifies the rate of the Poisson distribution.
+            rate: The rate of the Poisson distribution.
 
         Returns:
             A time sequence generator where the time difference
                 between two consecutive steps follows a Poisson
                 distribution.
 
         Example usage:
@@ -222,17 +223,17 @@
         max_time_diff: float = 1.0,
     ) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps is constant and is sampled from a
         uniform distribution.
 
         Args:
-            min_time_diff: Specifies the minimum time difference
+            min_time_diff: The minimum time difference
                 between two consecutive steps.
-            max_time_diff: Specifies the maximum time difference
+            max_time_diff: The maximum time difference
                 between two consecutive steps.
 
         Returns:
             A time sequence generator where the time difference
                 between two consecutive steps is constant and is
                 sampled from a uniform distribution.
 
@@ -279,17 +280,17 @@
         min_time_diff: float = 0.0,
         max_time_diff: float = 1.0,
     ) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time difference
         between two consecutive steps follows a uniform distribution.
 
         Args:
-            min_time_diff: Specifies the minimum time difference
+            min_time_diff: The minimum time difference
                 between two consecutive steps.
-            max_time_diff: Specifies the maximum time difference
+            max_time_diff: The maximum time difference
                 between two consecutive steps.
 
         Returns:
             A time sequence generator where the time difference
                 between two consecutive steps follows a uniform
                 distribution.
 
@@ -332,16 +333,16 @@
         min_time: float = 0.0,
         max_time: float = 1.0,
     ) -> TimeSequenceGenerator:
         r"""Create a time sequence generator where the time is sampled
         from a uniform distribution.
 
         Args:
-            min_time: Specifies the minimum time.
-            max_time: Specifies the maximum time.
+            min_time: The minimum time.
+            max_time: The maximum time.
 
         Returns:
             A time sequence generator where the time is sampled from a
                 uniform distribution.
 
         Raises:
             ValueError: if ``min_time`` is lower than 0.
```

### Comparing `startorch-0.1.0/src/startorch/sequence/trigo.py` & `startorch-0.1.1a0/src/startorch/sequence/trigo.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 class AcoshSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the inverse
     hyperbolic cosine (arccosh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Acosh, RandUniform
     >>> generator = Acosh(RandUniform())
     >>> generator
     AcoshSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -49,14 +50,15 @@
 class AsinhSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the inverse
     hyperbolic sine (arcsinh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Asinh, RandUniform
     >>> generator = Asinh(RandUniform())
     >>> generator
     AsinhSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -75,14 +77,15 @@
 class AtanhSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the inverse
     hyperbolic tangent (arctanh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Atanh, RandUniform
     >>> generator = Atanh(RandUniform())
     >>> generator
     AtanhSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -101,14 +104,15 @@
 class CoshSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the hyperbolic
     cosine (cosh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Cosh, RandUniform
     >>> generator = Cosh(RandUniform())
     >>> generator
     CoshSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -127,14 +131,15 @@
 class SinhSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the hyperbolic sine
     (sinh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Sinh, RandUniform
     >>> generator = Sinh(RandUniform())
     >>> generator
     SinhSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
@@ -153,14 +158,15 @@
 class TanhSequenceGenerator(BaseWrapperSequenceGenerator):
     r"""Implement a sequence generator that computes the hyperbolic
     tangent (tanh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Tanh, RandUniform
     >>> generator = Tanh(RandUniform())
     >>> generator
     TanhSequenceGenerator(
       (sequence): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
```

### Comparing `startorch-0.1.0/src/startorch/sequence/uniform.py` & `startorch-0.1.1a0/src/startorch/sequence/uniform.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,22 +30,23 @@
 
 
 class AsinhUniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from an asinh-uniform distribution.
 
     Args:
-        low: Specifies a sequence generator (or its configuration) to
+        low: A sequence generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a sequence generator (or its configuration) to
+        high: A sequence generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import AsinhUniform, RandUniform
     >>> generator = AsinhUniform(low=RandUniform(-1.0, 0.0), high=RandUniform(0.0, 1.0))
     >>> generator
     AsinhUniformSequenceGenerator(
       (low): RandUniformSequenceGenerator(low=-1.0, high=0.0, feature_size=(1,))
       (high): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
@@ -78,22 +79,23 @@
 
 
 class LogUniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from a log-uniform distribution.
 
     Args:
-        low: Specifies a sequence generator (or its configuration) to
+        low: A sequence generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a sequence generator (or its configuration) to
+        high: A sequence generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import LogUniform, RandUniform
     >>> generator = LogUniform(low=RandUniform(0.0, 1.0), high=RandUniform(5.0, 10.0))
     >>> generator
     LogUniformSequenceGenerator(
       (low): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (high): RandUniformSequenceGenerator(low=5.0, high=10.0, feature_size=(1,))
@@ -126,24 +128,25 @@
 
 
 class RandAsinhUniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from an asinh-uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
-        feature_size: Specifies the feature size.
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``high`` is lower than ``low``.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandAsinhUniform
     >>> generator = RandAsinhUniform(low=1.0, high=10.0)
     >>> generator
     RandAsinhUniformSequenceGenerator(low=1.0, high=10.0, feature_size=(1,))
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -171,36 +174,37 @@
             f"high={self._high}, feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_asinh_uniform(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             low=self._low,
             high=self._high,
             generator=rng,
         )
 
 
 class RandIntSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a class to generate sequences of uniformly distributed
     integers.
 
     Args:
-        low: Specifies the minimum value (included).
-        high: Specifies the maximum value (excluded).
-        feature_size: Specifies the feature size.
+        low: The minimum value (included).
+        high: The maximum value (excluded).
+        feature_size: The feature size.
 
     Raises:
-        ValueError if ``high`` is lower than ``low``.
+        ValueError: if ``high`` is lower than ``low``.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandInt
     >>> generator = RandInt(0, 100)
     >>> generator
     RandIntSequenceGenerator(low=0, high=100, feature_size=())
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -230,34 +234,35 @@
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return torch.randint(
             low=self._low,
             high=self._high,
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             generator=rng,
         )
 
 
 class RandLogUniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from a log-uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
-        feature_size: Specifies the feature size.
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``high`` is lower than ``low``.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandLogUniform
     >>> generator = RandLogUniform(low=1.0, high=10.0)
     >>> generator
     RandLogUniformSequenceGenerator(low=1.0, high=10.0, feature_size=(1,))
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -285,36 +290,37 @@
             f"high={self._high}, feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_log_uniform(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             low=self._low,
             high=self._high,
             generator=rng,
         )
 
 
 class RandUniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from a uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
-        feature_size: Specifies the feature size.
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
+        feature_size: The feature size.
 
     Raises:
         ValueError: if ``high`` is lower than ``low``.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform
     >>> generator = RandUniform()
     >>> generator
     RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     >>> generator.generate(seq_len=12, batch_size=4)
     tensor([[...]])
@@ -342,34 +348,35 @@
             f"high={self._high}, feature_size={self._feature_size})"
         )
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> torch.Tensor:
         return rand_uniform(
-            size=(batch_size, seq_len) + self._feature_size,
+            size=(batch_size, seq_len, *self._feature_size),
             low=self._low,
             high=self._high,
             generator=rng,
         )
 
 
 class UniformSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences by sampling
     values from a uniform distribution.
 
     Args:
-        low: Specifies a sequence generator (or its configuration) to
+        low: A sequence generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a sequence generator (or its configuration) to
+        high: A sequence generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Uniform, RandUniform
     >>> generator = Uniform(low=RandUniform(-1.0, 0.0), high=RandUniform(0.0, 1.0))
     >>> generator
     UniformSequenceGenerator(
       (low): RandUniformSequenceGenerator(low=-1.0, high=0.0, feature_size=(1,))
       (high): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
```

### Comparing `startorch-0.1.0/src/startorch/sequence/wave.py` & `startorch-0.1.1a0/src/startorch/sequence/wave.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,27 @@
     sine wave pattern.
 
     The sequences are generated by using the following formula:
 
     ``output = amplitude * sin(2 * pi * frequency * value + phase)``
 
     Args:
-        value: Specifies a sequence generator (or its configuration) to
+        value: A sequence generator (or its configuration) to
             generate the sequence values.
-        frequency: Specifies a sequence generator (or its
+        frequency: A sequence generator (or its
             configuration) to generate the frequency values.
-        phase: Specifies a sequence generator (or its configuration)
+        phase: A sequence generator (or its configuration)
             to generate the phase values.
-        amplitude: Specifies a sequence generator (or its
+        amplitude: A sequence generator (or its
             configuration) to generate the amplitude values.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import Arange, SineWave, RandUniform, Constant, RandLogUniform
     >>> generator = SineWave(
     ...     value=Arange(),
     ...     frequency=Constant(RandLogUniform(low=0.01, high=0.1)),
     ...     phase=Constant(RandUniform(low=-1.0, high=1.0)),
     ...     amplitude=Constant(RandLogUniform(low=0.1, high=1.0)),
```

### Comparing `startorch-0.1.0/src/startorch/sequence/wiener.py` & `startorch-0.1.1a0/src/startorch/sequence/wiener.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 class RandWienerProcessSequenceGenerator(BaseSequenceGenerator):
     r"""Implement a sequence generator to generate sequences where the
     values are generated by a Wiener process.
 
     Useful link: https://en.wikipedia.org/wiki/Wiener_process
 
     Args:
-        step_size: Specifies the time step size.
+        step_size: The time step size.
 
     Raises:
         ValueError: if ``step_size`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence import RandWienerProcess
     >>> generator = RandWienerProcess()
     >>> generator
     RandWienerProcessSequenceGenerator(step_size=1.0)
     >>> generator.generate(seq_len=6, batch_size=2)
     tensor([[...]])
 
@@ -65,30 +66,31 @@
     generator: torch.Generator | None = None,
 ) -> torch.Tensor:
     r"""Create a batch of sequences generated by a Wiener process.
 
     Useful link: https://en.wikipedia.org/wiki/Wiener_process
 
     Args:
-        seq_len: Specifies the sequence length.
-        step_size: Specifies the time step size.
-        batch_size: Specifies the batch size.
-        generator: Specifies an optional random generator.
+        seq_len: The sequence length.
+        step_size: The time step size.
+        batch_size: The batch size.
+        generator: An optional random generator.
 
     Returns:
         A batch of sequences generated with a Wiener process.
             It is a tensor of type float and shape
             ``(batch size, sequence length)``.
 
     Raises:
         ValueError: if ``step_size`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.sequence.wiener import wiener_process
     >>> wiener_process(seq_len=12, batch_size=4)
     tensor([[...]])
 
     ```
     """
     if step_size < 0:
```

### Comparing `startorch-0.1.0/src/startorch/sequence/wrapper.py` & `startorch-0.1.1a0/src/startorch/sequence/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Note:
         It is possible to wrap a sequence generator into another
         sequence generator without using this base class. This class
         makes it more convenient and reduce duplicate code.
 
     Args:
-        generator: Specifies the sequence generator or its
+        generator: The sequence generator or its
             configuration.
     """
 
     def __init__(self, generator: BaseSequenceGenerator | dict) -> None:
         super().__init__()
         self._generator = setup_sequence_generator(generator)
```

### Comparing `startorch-0.1.0/src/startorch/tensor/__init__.py` & `startorch-0.1.1a0/src/startorch/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/tensor/base.py` & `startorch-0.1.1a0/src/startorch/tensor/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     r"""Define the base class to generate tensor.
 
     A child class has to implement the ``generate`` method.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import RandUniform
     >>> generator = RandUniform()
     >>> generator
     RandUniformTensorGenerator(low=0.0, high=1.0)
     >>> generator.generate(size=(4, 12))
     tensor([[...]])
@@ -39,16 +40,16 @@
     """
 
     @abstractmethod
     def generate(self, size: tuple[int, ...], rng: torch.Generator | None = None) -> torch.Tensor:
         r"""Generate a tensor.
 
         Args:
-            size: Specifies the size of the tensor to generate.
-            rng: Specifies an optional random number generator.
+            size: The size of the tensor to generate.
+            rng: An optional random number generator.
 
         Returns:
             The generated tensor with the specified size.
 
         Example usage:
 
         ```pycon
@@ -68,23 +69,24 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration for a
             ``BaseTensorGenerator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import is_tensor_generator_config
     >>> is_tensor_generator_config({"_target_": "startorch.tensor.RandUniform"})
     True
 
     ```
     """
     return is_object_config(config, BaseTensorGenerator)
@@ -93,22 +95,23 @@
 def setup_tensor_generator(generator: BaseTensorGenerator | dict) -> BaseTensorGenerator:
     r"""Set up a tensor generator.
 
     The tensor generator is instantiated from its configuration by
     using the ``BaseTensorGenerator`` factory function.
 
     Args:
-        generator: Specifies a tensor generator or its configuration.
+        generator: A tensor generator or its configuration.
 
     Returns:
         A tensor generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import setup_tensor_generator
     >>> setup_tensor_generator({"_target_": "startorch.tensor.RandUniform"})
     RandUniformTensorGenerator(low=0.0, high=1.0)
 
     ```
     """
     if isinstance(generator, dict):
```

### Comparing `startorch-0.1.0/src/startorch/tensor/categorical.py` & `startorch-0.1.1a0/src/startorch/tensor/categorical.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,22 +18,23 @@
 
 
 class MultinomialTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensors of categorical variables
     where each value is sampled from a multinomial distribution.
 
     Args:
-        weights: Specifies the vector of weights associated at each
+        weights: The vector of weights associated at each
             category. It must be a float tensor of shape
             ``(num_categories,)``. The weights have to be positive but
             do not need to sum to 1.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import Multinomial
     >>> generator = Multinomial(torch.ones(10))
     >>> generator
     MultinomialTensorGenerator(num_categories=10)
     >>> generator.generate(size=(4, 12))
     tensor([[...]])
@@ -58,15 +59,15 @@
         r"""Instantiate the weights with a uniform pattern.
 
         All the categories have the same probability.
         The weight of the ``i``-th category (``w_i``) is generated
         with the rule: ``w_i = 1``
 
         Args:
-            num_categories: Specifies the number of categories.
+            num_categories: The number of categories.
 
         Returns:
             A tensor generator where the weights of the multinomial
                 distribution follow a uniform pattern.
 
         Example usage:
 
@@ -90,15 +91,15 @@
     ) -> MultinomialTensorGenerator:
         r"""Instantiate the weights with a linear pattern.
 
         The weight of the ``i``-th category (``w_i``) is generated
         with the rule: ``w_i = num_categories - i``
 
         Args:
-            num_categories: Specifies the number of categories.
+            num_categories: The number of categories.
 
         Returns:
             A tensor generator where the weights of the multinomial
                 distribution follow a linear pattern.
 
         Example usage:
 
@@ -123,16 +124,16 @@
     ) -> MultinomialTensorGenerator:
         r"""Instantiate the weights with an exponential pattern.
 
         The weight of the ``i``-th category (``w_i``) is generated with
         the rule: ``w_i = exp(-scale * i)``
 
         Args:
-            num_categories: Specifies the number of categories.
-            scale: Specifies the scale parameter that controls the
+            num_categories: The number of categories.
+            scale: The scale parameter that controls the
                 exponential function.
 
         Returns:
             A tensor generator where the weights of the multinomial
                 distribution follow an exponential pattern.
 
         Example usage:
@@ -157,22 +158,23 @@
 
     All the categories have the same probability.
 
     Note: it is a more efficient implementation of
     ``Multinomial.generate_uniform_weights``.
 
     Args:
-        num_categories: Specifies the number of categories.
+        num_categories: The number of categories.
 
     Raises:
         ValueError: if ``num_categories`` is negative.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import UniformCategorical
     >>> generator = UniformCategorical(10)
     >>> generator
     UniformCategoricalTensorGenerator(num_categories=10)
     >>> generator.generate(size=(4, 12))
     tensor([[...]])
```

### Comparing `startorch-0.1.0/src/startorch/tensor/cauchy.py` & `startorch-0.1.1a0/src/startorch/tensor/cauchy.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
 
 class CauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies a tensor generator (or its configuration) to
+        loc: A tensor generator (or its configuration) to
             generate the location.
-        scale: Specifies a tensor generator (or its configuration) to
+        scale: A tensor generator (or its configuration) to
             generate the scale.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Cauchy, RandUniform
     >>> generator = Cauchy(
     ...     loc=RandUniform(low=-1.0, high=1.0), scale=RandUniform(low=1.0, high=2.0)
     ... )
     >>> generator
     CauchyTensorGenerator(
       (loc): RandUniformTensorGenerator(low=-1.0, high=1.0)
@@ -67,23 +68,24 @@
 
 
 class RandCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
-        scale: Specifies the scale of the distribution.
+        loc: The location/median of the Cauchy distribution.
+        scale: The scale of the distribution.
 
     Raises:
         ValueError: if ``scale`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandCauchy
     >>> generator = RandCauchy(loc=0.0, scale=1.0)
     >>> generator
     RandCauchyTensorGenerator(loc=0.0, scale=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -111,26 +113,27 @@
 
 
 class RandTruncCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     truncated Cauchy distribution.
 
     Args:
-        loc: Specifies the location/median of the Cauchy distribution.
-        scale: Specifies the scale of the distribution.
-        min_value: Specifies the minimum value (included).
-        max_value: Specifies the maximum value (excluded).
+        loc: The location/median of the Cauchy distribution.
+        scale: The scale of the distribution.
+        min_value: The minimum value (included).
+        max_value: The maximum value (excluded).
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncCauchy
     >>> generator = RandTruncCauchy(loc=0.0, scale=1.0, min_value=-1.0, max_value=1.0)
     >>> generator
     RandTruncCauchyTensorGenerator(loc=0.0, scale=1.0, min_value=-1.0, max_value=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -174,26 +177,27 @@
 
 
 class TruncCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     Cauchy distribution.
 
     Args:
-        loc: Specifies a tensor generator (or its configuration) to
+        loc: A tensor generator (or its configuration) to
             generate the location.
-        scale: Specifies a tensor generator (or its configuration) to
+        scale: A tensor generator (or its configuration) to
             generate the scale.
-        min_value: Specifies a tensor generator (or its configuration)
+        min_value: A tensor generator (or its configuration)
             to generate the minimum value (included).
-        max_value: Specifies a tensor generator (or its configuration)
+        max_value: A tensor generator (or its configuration)
             to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncCauchy
     >>> generator = TruncCauchy(
     ...     loc=RandUniform(low=-1.0, high=1.0),
     ...     scale=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=-10.0, high=-5.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/tensor/choice.py` & `startorch-0.1.1a0/src/startorch/tensor/choice.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,20 +33,21 @@
         - a key ``'generator'`` which indicates the tensor generator
             or its configuration.
         - an optional key ``'weight'`` with a float value which
             indicates the weight of the tensor generator.
             If this key is absent, the weight is set to ``1.0``.
 
     Args:
-        generators: Specifies the tensor generators and their weights.
+        generators: The tensor generators and their weights.
             See above to learn about the expected format.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import MultinomialChoice, RandUniform, RandNormal
     >>> generator = MultinomialChoice(
     ...     (
     ...         {"weight": 2.0, "generator": RandUniform()},
     ...         {"weight": 1.0, "generator": RandNormal()},
     ...     )
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/tensor/constant.py` & `startorch-0.1.1a0/src/startorch/tensor/constant.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,21 +12,22 @@
 
 
 class FullTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator that fills the tensor with a given
     value.
 
     Args:
-        value: Specifies the fill value.
-        dtype: Specifies the target dtype. ``None`` means the data type
+        value: The fill value.
+        dtype: The target dtype. ``None`` means the data type
             is infered from the value type.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Full
     >>> generator = Full(value=42)
     >>> generator
     FullTensorGenerator(value=42, dtype=None)
     >>> generator.generate((2, 6))
     tensor([[42, 42, 42, 42, 42, 42],
             [42, 42, 42, 42, 42, 42]])
```

### Comparing `startorch-0.1.0/src/startorch/tensor/dtype.py` & `startorch-0.1.1a0/src/startorch/tensor/dtype.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 class FloatTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a sequence generator that converts tensor values to
     float.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Float, RandInt
     >>> generator = Float(RandInt(low=0, high=10))
     >>> generator
     FloatTensorGenerator(
       (tensor): RandIntTensorGenerator(low=0, high=10)
     )
     >>> generator.generate((2, 6))
@@ -39,14 +40,15 @@
 class LongTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a sequence generator that converts a tensor values to
     long.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Long, RandUniform
     >>> generator = Long(RandUniform(low=0, high=10))
     >>> generator
     LongTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=10.0)
     )
     >>> generator.generate((2, 6))
```

### Comparing `startorch-0.1.0/src/startorch/tensor/exponential.py` & `startorch-0.1.1a0/src/startorch/tensor/exponential.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,21 @@
     Exponential distribution.
 
     The rates of the Exponential distribution are generated by the
     rate generator. The rate generator should return the rate for each
     value in the sequence.
 
     Args:
-        rate: Specifies the rate generator or its configuration.
+        rate: The rate generator or its configuration.
             The rate generator should return valid rate values.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Exponential, RandUniform
     >>> generator = Exponential(rate=RandUniform(low=1.0, high=100.0))
     >>> generator
     ExponentialTensorGenerator(
       (rate): RandUniformTensorGenerator(low=1.0, high=100.0)
     )
     >>> generator.generate((2, 6))
@@ -66,22 +67,23 @@
 
 
 class RandExponentialTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate sequences by sampling values from
     an Exponential distribution.
 
     Args:
-        rate: Specifies the rate of the Exponential distribution.
+        rate: The rate of the Exponential distribution.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandExponential
     >>> generator = RandExponential(rate=1.0)
     >>> generator
     RandExponentialTensorGenerator(rate=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -103,24 +105,25 @@
 
 
 class RandTruncExponentialTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate sequences by sampling values from a
     truncated Exponential distribution.
 
     Args:
-        rate: Specifies the rate of the Exponential distribution.
-        max_value: Specifies the maximum value.
+        rate: The rate of the Exponential distribution.
+        max_value: The maximum value.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncExponential
     >>> generator = RandTruncExponential(rate=1.0, max_value=3.0)
     >>> generator
     RandTruncExponentialTensorGenerator(rate=1.0, max_value=3.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -151,22 +154,23 @@
 
 
 class TruncExponentialTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate sequence by sampling values from an
     Exponential distribution.
 
     Args:
-        rate: Specifies a sequence generator (or its configuration) to
+        rate: A sequence generator (or its configuration) to
             generate the rate.
-        max_value: Specifies a sequence generator (or its
+        max_value: A sequence generator (or its
             configuration) to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncExponential
     >>> generator = TruncExponential(
     ...     rate=RandUniform(low=1.0, high=10.0),
     ...     max_value=RandUniform(low=1.0, high=100.0),
     ... )
     >>> generator
     TruncExponentialTensorGenerator(
```

### Comparing `startorch-0.1.0/src/startorch/tensor/halfcauchy.py` & `startorch-0.1.1a0/src/startorch/tensor/halfcauchy.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 
 
 class HalfCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Cauchy distribution.
 
     Args:
-        scale: Specifies a tensor generator (or its configuration) to
+        scale: A tensor generator (or its configuration) to
             generate the scale.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import HalfCauchy, RandUniform
     >>> generator = HalfCauchy(scale=RandUniform(low=1.0, high=2.0))
     >>> generator
     HalfCauchyTensorGenerator(
       (scale): RandUniformTensorGenerator(low=1.0, high=2.0)
     )
     >>> generator.generate((2, 6))
@@ -65,22 +66,23 @@
 
 
 class RandHalfCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Cauchy distribution.
 
     Args:
-        scale: Specifies the scale of the distribution.
+        scale: The scale of the distribution.
 
     Raises:
         ValueError: if ``scale`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandHalfCauchy
     >>> generator = RandHalfCauchy(scale=1.0)
     >>> generator
     RandHalfCauchyTensorGenerator(scale=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -106,24 +108,25 @@
 
 
 class RandTruncHalfCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     truncated half-Cauchy distribution.
 
     Args:
-        scale: Specifies the scale of the distribution.
-        max_value: Specifies the maximum value.
+        scale: The scale of the distribution.
+        max_value: The maximum value.
 
     Raises:
         ValueError: if ``scale`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncHalfCauchy
     >>> generator = RandTruncHalfCauchy(scale=1.0, max_value=5.0)
     >>> generator
     RandTruncHalfCauchyTensorGenerator(scale=1.0, max_value=5.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -158,22 +161,23 @@
 
 
 class TruncHalfCauchyTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Cauchy distribution.
 
     Args:
-        scale: Specifies a tensor generator (or its configuration) to
+        scale: A tensor generator (or its configuration) to
             generate the scale.
-        max_value: Specifies a tensor generator (or its configuration)
+        max_value: A tensor generator (or its configuration)
             to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncHalfCauchy
     >>> generator = TruncHalfCauchy(
     ...     scale=RandUniform(low=1.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
     >>> generator
     TruncHalfCauchyTensorGenerator(
```

### Comparing `startorch-0.1.0/src/startorch/tensor/halfnormal.py` & `startorch-0.1.1a0/src/startorch/tensor/halfnormal.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 
 
 class HalfNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Normal distribution.
 
     Args:
-        std: Specifies a tensor generator (or its configuration) to
+        std: A tensor generator (or its configuration) to
             generate the standard deviation.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import HalfNormal, RandUniform
     >>> generator = HalfNormal(std=RandUniform(low=1.0, high=2.0))
     >>> generator
     HalfNormalTensorGenerator(
       (std): RandUniformTensorGenerator(low=1.0, high=2.0)
     )
     >>> generator.generate(size=(2, 6))
@@ -65,22 +66,23 @@
 
 
 class RandHalfNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Normal distribution.
 
     Args:
-        std: Specifies the std of the distribution.
+        std: The std of the distribution.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandHalfNormal
     >>> generator = RandHalfNormal(std=1.0)
     >>> generator
     RandHalfNormalTensorGenerator(std=1.0)
     >>> generator.generate(size=(2, 6))
     tensor([[...]])
 
@@ -106,24 +108,25 @@
 
 
 class RandTruncHalfNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     truncated half-Normal distribution.
 
     Args:
-        std: Specifies the std of the distribution.
-        max_value: Specifies the maximum value.
+        std: The std of the distribution.
+        max_value: The maximum value.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncHalfNormal
     >>> generator = RandTruncHalfNormal(std=1.0, max_value=1.0)
     >>> generator
     RandTruncHalfNormalTensorGenerator(std=1.0, max_value=1.0)
     >>> generator.generate(size=(2, 6))
     tensor([[...]])
 
@@ -154,22 +157,23 @@
 
 
 class TruncHalfNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     half-Normal distribution.
 
     Args:
-        std: Specifies a tensor generator (or its configuration) to
+        std: A tensor generator (or its configuration) to
             generate the std.
-        max_value: Specifies a tensor generator (or its configuration)
+        max_value: A tensor generator (or its configuration)
             to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncHalfNormal
     >>> generator = TruncHalfNormal(
     ...     std=RandUniform(low=1.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
     >>> generator
     TruncHalfNormalTensorGenerator(
```

### Comparing `startorch-0.1.0/src/startorch/tensor/lognormal.py` & `startorch-0.1.1a0/src/startorch/tensor/lognormal.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,23 +27,24 @@
 
 
 class LogNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     log-Normal distribution.
 
     Args:
-        mean: Specifies a tensor generator (or its configuration) to
+        mean: A tensor generator (or its configuration) to
             generate the mean of the underlying Normal distribution.
-        std: Specifies a tensor generator (or its configuration) to
+        std: A tensor generator (or its configuration) to
             generate the standard deviation of the underlying Normal
             distribution.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import LogNormal, RandUniform
     >>> generator = LogNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0), std=RandUniform(low=1.0, high=2.0)
     ... )
     >>> generator
     LogNormalTensorGenerator(
       (mean): RandUniformTensorGenerator(low=-1.0, high=1.0)
@@ -73,24 +74,25 @@
 
 
 class RandLogNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     log-Normal distribution.
 
     Args:
-        mean: Specifies the mean of the underlying Normal distribution.
-        std: Specifies the standard deviation of the underlying Normal
+        mean: The mean of the underlying Normal distribution.
+        std: The standard deviation of the underlying Normal
             distribution.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandLogNormal
     >>> generator = RandLogNormal(mean=0.0, std=1.0)
     >>> generator
     RandLogNormalTensorGenerator(mean=0.0, std=1.0)
     >>> generator.generate(size=(2, 6))
     tensor([[...]])
 
@@ -118,27 +120,28 @@
 
 
 class RandTruncLogNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator to generate cyclic tensors by
     sampling values from a truncated log-Normal distribution.
 
     Args:
-        mean: Specifies the mean of the log-Normal distribution.
-        std: Specifies the standard deviation of the log-Normal
+        mean: The mean of the log-Normal distribution.
+        std: The standard deviation of the log-Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
+        min_value: The minimum value.
+        max_value: The maximum value.
 
     Raises:
         ValueError: if ``std`` is not a positive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncLogNormal
     >>> generator = RandTruncLogNormal(mean=0.0, std=1.0, min_value=0.0, max_value=1.0)
     >>> generator
     RandTruncLogNormalTensorGenerator(mean=0.0, std=1.0, min_value=0.0, max_value=1.0)
     >>> generator.generate(size=(2, 6))
     tensor([[...]])
 
@@ -178,27 +181,28 @@
 
 
 class TruncLogNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensor by sampling values from a
     truncated log-Normal distribution.
 
     Args:
-        mean: Specifies a tensor generator (or its configuration) to
+        mean: A tensor generator (or its configuration) to
             generate the mean of the underlying Normal distribution.
-        std: Specifies a tensor generator (or its configuration) to
+        std: A tensor generator (or its configuration) to
             generate the standard deviation of the underlying Normal
             distribution.
-        min_value: Specifies a tensor generator (or its configuration)
+        min_value: A tensor generator (or its configuration)
             to generate the minimum value (included).
-        max_value: Specifies a tensor generator (or its configuration)
+        max_value: A tensor generator (or its configuration)
             to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncLogNormal
     >>> generator = TruncLogNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0),
     ...     std=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=0.0, high=2.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/tensor/math.py` & `startorch-0.1.1a0/src/startorch/tensor/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     a tensor.
 
     This tensor generator is equivalent to: ``output = abs(tensor)``
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Abs, RandNormal
     >>> generator = Abs(RandNormal())
     >>> generator
     AbsTensorGenerator(
       (tensor): RandNormalTensorGenerator(mean=0.0, std=1.0)
     )
     >>> generator.generate((2, 6))
@@ -61,20 +62,21 @@
     r"""Implement a tensor generator that adds a scalar value to a
     generated batch of tensors.
 
     This tensor generator is equivalent to:
     ``output = tensor + scalar``
 
     Args:
-        generator: Specifies the tensor generator or its configuration.
-        value: Specifies the scalar value to add.
+        generator: The tensor generator or its configuration.
+        value: The scalar value to add.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import AddScalar, RandUniform
     >>> generator = AddScalar(RandUniform(), 10.0)
     >>> generator
     AddScalarTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
       (value): 10.0
     )
@@ -105,22 +107,23 @@
 class AddTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator that adds several tensor.
 
     This tensor generator is equivalent to:
     ``output = tensor_1 + tensor_2 + ... + tensor_n``
 
     Args:
-        generators: Specifies the tensor generators.
+        generators: The tensor generators.
 
     Raises:
         ValueError: if no sequence generator is provided.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Add, RandNormal, RandUniform
     >>> generator = Add([RandUniform(), RandNormal()])
     >>> generator
     AddTensorGenerator(
       (0): RandUniformTensorGenerator(low=0.0, high=1.0)
       (1): RandNormalTensorGenerator(mean=0.0, std=1.0)
     )
@@ -150,26 +153,27 @@
 class ClampTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator to generate tensors where the values
     are clamped.
 
     Note: ``min_value`` and ``max_value`` cannot be both ``None``.
 
     Args:
-        generator: Specifies the tensor generator or its configuration.
-        min_value: Specifies the lower bound. If ``min_value`` is
+        generator: The tensor generator or its configuration.
+        min_value: The lower bound. If ``min_value`` is
             ``None``, there is no lower bound.
-        max_value: Specifies the upper bound. If ``max_value`` is
+        max_value: The upper bound. If ``max_value`` is
             ``None``, there is no upper bound.
 
     Raises:
         ValueError: if both ``min`` and ``max`` are ``None``
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Clamp, RandUniform
     >>> generator = Clamp(RandUniform(low=1.0, high=50.0), min_value=2.0, max_value=10.0)
     >>> generator
     ClampTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=1.0, high=50.0)
       (min_value): 2.0
       (max_value): 10.0
@@ -214,28 +218,29 @@
     one.
 
     This tensor generator is equivalent to:
         - ``output = dividend / divisor`` (a.k.a. true division)
         - ``output = dividend // divisor`` (a.k.a. floor division)
 
     Args:
-        dividend: Specifies the dividend tensor generator or its
+        dividend: The dividend tensor generator or its
             configuration.
-        divisor: Specifies the divisor tensor generator or its
+        divisor: The divisor tensor generator or its
             configuration.
-        rounding_mode: Specifies the
+        rounding_mode: The
             type of rounding applied to the result.
             - ``None``: true division.
             - ``"trunc"``: rounds the results of the division
                 towards zero.
             - ``"floor"``: floor division.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Div, RandUniform
     >>> generator = Div(RandUniform(), RandUniform(low=1.0, high=10.0))
     >>> generator
     DivTensorGenerator(
       (dividend): RandUniformTensorGenerator(low=0.0, high=1.0)
       (divisor): RandUniformTensorGenerator(low=1.0, high=10.0)
     )
@@ -272,14 +277,15 @@
     tensor.
 
     This tensor generator is equivalent to: ``output = exp(tensor)``
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Exp, RandUniform
     >>> generator = Exp(RandUniform(low=1.0, high=5.0))
     >>> generator
     ExpTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=1.0, high=5.0)
     )
     >>> generator.generate((2, 6))
@@ -296,21 +302,22 @@
     r"""Implement a tensor generator that computes the element-wise
     remainder of division.
 
     This tensor generator is equivalent to:
     ``output = dividend % divisor``
 
     Args:
-        dividend: Specifies the tensor generator (or its configuration)
+        dividend: The tensor generator (or its configuration)
             that generates the dividend values.
-        divisor: Specifies the divisor.
+        divisor: The divisor.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Fmod, RandUniform
     >>> generator = Fmod(dividend=RandUniform(low=-100, high=100), divisor=10.0)
     >>> generator
     FmodTensorGenerator(
       (dividend): RandUniformTensorGenerator(low=-100.0, high=100.0)
       (divisor): 10.0
     )
@@ -357,14 +364,15 @@
     tensor.
 
     This tensor generator is equivalent to: ``output = log(tensor)``
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Log, RandUniform
     >>> generator = Log(RandUniform(low=1.0, high=100.0))
     >>> generator
     LogTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=1.0, high=100.0)
     )
     >>> generator.generate((2, 6))
@@ -380,22 +388,23 @@
 class MulTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator that multiplies multiple tensors.
 
     This tensor generator is equivalent to:
     ``output = tensor_1 * tensor_2 * ... * tensor_n``
 
     Args:
-        generators: Specifies the tensor generators.
+        generators: The tensor generators.
 
     Raises:
         ValueError: if no sequence generator is provided.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import Mul, RandUniform, RandNormal
     >>> generator = Mul([RandUniform(), RandNormal()])
     >>> generator
     MulTensorGenerator(
       (0): RandUniformTensorGenerator(low=0.0, high=1.0)
       (1): RandNormalTensorGenerator(mean=0.0, std=1.0)
@@ -427,20 +436,21 @@
     r"""Implement a tensor generator that multiplies a scalar value to a
     generated batch of tensors.
 
     This tensor generator is equivalent to:
     ``output = tensor * scalar``
 
     Args:
-        generator: Specifies the tensor generator or its configuration.
-        value: Specifies the scalar value to multiply.
+        generator: The tensor generator or its configuration.
+        value: The scalar value to multiply.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import MulScalar, RandUniform, RandNormal
     >>> generator = MulScalar(RandUniform(), 42)
     >>> generator
     MulScalarTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
     )
@@ -473,14 +483,15 @@
     generated tensor.
 
     This tensor generator is equivalent to: ``output = -tensor``
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.tensor import Neg, RandNormal
     >>> generator = Neg(RandNormal())
     >>> generator
     NegTensorGenerator(
       (tensor): RandNormalTensorGenerator(mean=0.0, std=1.0)
     )
@@ -499,14 +510,15 @@
     tensor.
 
     This tensor generator is equivalent to: ``output = sqrt(tensor)``
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, Sqrt
     >>> generator = Sqrt(RandUniform(low=1.0, high=100.0))
     >>> generator
     SqrtTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=1.0, high=100.0)
     )
     >>> generator.generate((2, 6))
@@ -522,22 +534,23 @@
 class SubTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator that subtracts two tensors.
 
     This tensor generator is equivalent to:
     ``output = tensor_1 - tensor_2``
 
     Args:
-        tensor1: Specifies the first tensor generator or its
+        tensor1: The first tensor generator or its
             configuration.
-        tensor2: Specifies the second tensor generator or its
+        tensor2: The second tensor generator or its
             configuration.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandNormal, RandUniform, Sub
     >>> generator = Sub(RandUniform(), RandNormal())
     >>> generator
     SubTensorGenerator(
       (tensor1): RandUniformTensorGenerator(low=0.0, high=1.0)
       (tensor2): RandNormalTensorGenerator(mean=0.0, std=1.0)
     )
```

### Comparing `startorch-0.1.0/src/startorch/tensor/normal.py` & `startorch-0.1.1a0/src/startorch/tensor/normal.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 
 
 class NormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     Normal distribution.
 
     Args:
-        mean: Specifies a tensor generator (or its configuration) to
+        mean: A tensor generator (or its configuration) to
             generate the mean.
-        std: Specifies a tensor generator (or its configuration) to
+        std: A tensor generator (or its configuration) to
             generate the standard deviation.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Normal, RandUniform
     >>> generator = Normal(
     ...     mean=RandUniform(low=-1.0, high=1.0), std=RandUniform(low=1.0, high=2.0)
     ... )
     >>> generator
     NormalTensorGenerator(
       (mean): RandUniformTensorGenerator(low=-1.0, high=1.0)
@@ -67,24 +68,25 @@
 
 
 class RandNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a sequence generator to generate cyclic sequences by
     sampling values from a Normal distribution.
 
     Args:
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
 
     Raises:
         ValueError: if ``std`` is not a postive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandNormal
     >>> generator = RandNormal(mean=0.0, std=1.0)
     >>> generator
     RandNormalTensorGenerator(mean=0.0, std=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -112,27 +114,28 @@
 
 
 class RandTruncNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a sequence generator to generate cyclic sequences by
     sampling values from a truncated Normal distribution.
 
     Args:
-        mean: Specifies the mean of the Normal distribution.
-        std: Specifies the standard deviation of the Normal
+        mean: The mean of the Normal distribution.
+        std: The standard deviation of the Normal
             distribution.
-        min_value: Specifies the minimum value.
-        max_value: Specifies the maximum value.
+        min_value: The minimum value.
+        max_value: The maximum value.
 
     Raises:
         ValueError: if ``std`` is not a postive number.
         ValueError: if ``max_value`` is lower than ``min_value``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandTruncNormal
     >>> generator = RandTruncNormal(mean=0.0, std=1.0, min_value=-1.0, max_value=1.0)
     >>> generator
     RandTruncNormalTensorGenerator(mean=0.0, std=1.0, min_value=-1.0, max_value=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -176,26 +179,27 @@
 
 
 class TruncNormalTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate sequence by sampling values from a
     truncated Normal distribution.
 
     Args:
-        mean: Specifies a sequence generator (or its configuration) to
+        mean: A sequence generator (or its configuration) to
             generate the mean.
-        std: Specifies a sequence generator (or its configuration) to
+        std: A sequence generator (or its configuration) to
             generate the standard deviation.
-        min_value: Specifies a sequence generator (or its
+        min_value: A sequence generator (or its
             configuration) to generate the minimum value (included).
-        max_value: Specifies a sequence generator (or its
+        max_value: A sequence generator (or its
             configuration) to generate the maximum value (excluded).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, TruncNormal
     >>> generator = TruncNormal(
     ...     mean=RandUniform(low=-1.0, high=1.0),
     ...     std=RandUniform(low=1.0, high=2.0),
     ...     min_value=RandUniform(low=-10.0, high=-5.0),
     ...     max_value=RandUniform(low=5.0, high=10.0),
     ... )
```

### Comparing `startorch-0.1.0/src/startorch/tensor/poisson.py` & `startorch-0.1.1a0/src/startorch/tensor/poisson.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     Poisson distribution.
 
     The rates of the Poisson distribution are generated by the rate
     generator. The rate generator should return the rate for each value
     in the tensor. The rate values should be greater than 0.
 
     Args:
-        rate: Specifies the rate generator or its configuration.
+        rate: The rate generator or its configuration.
             The rate generator should return valid rate values.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, Poisson
     >>> generator = Poisson(rate=RandUniform(low=1.0, high=2.0))
     >>> generator
     PoissonTensorGenerator(
       (rate): RandUniformTensorGenerator(low=1.0, high=2.0)
     )
     >>> generator.generate((2, 6))
@@ -53,23 +54,24 @@
 
 
 class RandPoissonTensorGenerator(BaseTensorGenerator):
     r"""Implement a class to generate tensors by sampling values from a
     Poisson distribution.
 
     Args:
-        rate: Specifies the rate of the Poisson distribution.
+        rate: The rate of the Poisson distribution.
             This value has to be greater than 0.
 
     Raises:
         ValueError: if ``rate`` is not a positive number.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandPoisson
     >>> generator = RandPoisson(rate=1.0)
     >>> generator
     RandPoissonTensorGenerator(rate=1.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
```

### Comparing `startorch-0.1.0/src/startorch/tensor/trigo.py` & `startorch-0.1.1a0/src/startorch/tensor/trigo.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 class AcoshTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the inverse hyperbolic
     cosine (arccosh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Acosh, RandUniform
     >>> generator = Acosh(RandUniform(low=1.0, high=5.0))
     >>> generator
     AcoshTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=1.0, high=5.0)
     )
     >>> generator.generate((2, 6))
@@ -46,14 +47,15 @@
 class AsinhTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the inverse hyperbolic
     sine (arcsinh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Asinh, RandUniform
     >>> generator = Asinh(RandUniform(low=0.0, high=1000.0))
     >>> generator
     AsinhTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1000.0)
     )
     >>> generator.generate((2, 6))
@@ -69,14 +71,15 @@
 class AtanhTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the inverse hyperbolic
     tangent (arctanh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Atanh, RandUniform
     >>> generator = Atanh(RandUniform(low=-0.5, high=0.5))
     >>> generator
     AtanhTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=-0.5, high=0.5)
     )
     >>> generator.generate((2, 6))
@@ -92,14 +95,15 @@
 class CoshTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the hyperbolic cosine
     (cosh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import Cosh, RandUniform
     >>> generator = Cosh(RandUniform())
     >>> generator
     CoshTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
     )
     >>> generator.generate((2, 6))
@@ -115,14 +119,15 @@
 class SinhTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the hyperbolic sine
     (sinh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, Sinh
     >>> generator = Sinh(RandUniform(low=0.0, high=1.0))
     >>> generator
     SinhTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
     )
     >>> generator.generate((2, 6))
@@ -138,14 +143,15 @@
 class TanhTensorGenerator(BaseWrapperTensorGenerator):
     r"""Implement a tensor generator that computes the hyperbolic tangent
     (tanh) of each value.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, Tanh
     >>> generator = Tanh(RandUniform(low=0.0, high=1.0))
     >>> generator
     TanhTensorGenerator(
       (tensor): RandUniformTensorGenerator(low=0.0, high=1.0)
     )
     >>> generator.generate((2, 6))
```

### Comparing `startorch-0.1.0/src/startorch/tensor/uniform.py` & `startorch-0.1.1a0/src/startorch/tensor/uniform.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,22 +28,23 @@
 
 
 class AsinhUniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator to generate tensors by sampling
     values from an asinh-uniform distribution.
 
     Args:
-        low : Specifies a tensor generator (or its configuration) to
+        low: A tensor generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a tensor generator (or its configuration) to
+        high: A tensor generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, AsinhUniform
     >>> generator = AsinhUniform(
     ...     low=RandUniform(low=-1000, high=-100), high=RandUniform(low=100, high=1000)
     ... )
     >>> generator
     AsinhUniformTensorGenerator(
       (low): RandUniformTensorGenerator(low=-1000.0, high=-100.0)
@@ -73,22 +74,23 @@
 
 
 class LogUniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator to generate tensors by sampling
     values from a log-uniform distribution.
 
     Args:
-        low: Specifies a tensor generator (or its configuration) to
+        low: A tensor generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a tensor generator (or its configuration) to
+        high: A tensor generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, LogUniform
     >>> generator = LogUniform(
     ...     low=RandUniform(low=0.1, high=1.0), high=RandUniform(low=100, high=1000)
     ... )
     >>> generator
     LogUniformTensorGenerator(
       (low): RandUniformTensorGenerator(low=0.1, high=1.0)
@@ -118,20 +120,21 @@
 
 
 class RandAsinhUniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator by sampling values from an asinh-
     uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandAsinhUniform
     >>> generator = RandAsinhUniform(low=-1000, high=1000)
     >>> generator
     RandAsinhUniformTensorGenerator(low=-1000.0, high=1000.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -159,20 +162,21 @@
 
 
 class RandIntTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator by sampling integer values from a
     uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandInt
     >>> generator = RandInt(low=0, high=10)
     >>> generator
     RandIntTensorGenerator(low=0, high=10)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -195,20 +199,21 @@
 
 
 class RandLogUniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator to generate tensors by sampling
     values from a log-uniform distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandLogUniform
     >>> generator = RandLogUniform(low=0.1, high=100.0)
     >>> generator
     RandLogUniformTensorGenerator(low=0.1, high=100.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -236,20 +241,21 @@
 
 
 class RandUniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator by sampling values from a uniform
     distribution.
 
     Args:
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform
     >>> generator = RandUniform(low=0, high=10)
     >>> generator
     RandUniformTensorGenerator(low=0.0, high=10.0)
     >>> generator.generate((2, 6))
     tensor([[...]])
 
@@ -272,22 +278,23 @@
 
 
 class UniformTensorGenerator(BaseTensorGenerator):
     r"""Implement a tensor generator by sampling values from a uniform
     distribution.
 
     Args:
-        low: Specifies a tensor generator (or its configuration) to
+        low: A tensor generator (or its configuration) to
             generate the minimum value (inclusive).
-        high: Specifies a tensor generator (or its configuration) to
+        high: A tensor generator (or its configuration) to
             generate the maximum value (exclusive).
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.tensor import RandUniform, Uniform
     >>> generator = UniformTensorGenerator(
     ...     low=RandUniform(low=0, high=2), high=RandUniform(low=8, high=10)
     ... )
     >>> generator
     UniformTensorGenerator(
       (low): RandUniformTensorGenerator(low=0.0, high=2.0)
```

### Comparing `startorch-0.1.0/src/startorch/tensor/wrapper.py` & `startorch-0.1.1a0/src/startorch/tensor/wrapper.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
     Note:
         It is possible to wrap a tensor generator into another tensor
         generator without using this base class. This class makes it
         more convenient and reduce duplicate code.
 
     Args:
-        generator: Specifies the tensor generator or its configuration.
+        generator: The tensor generator or its configuration.
     """
 
     def __init__(self, generator: BaseTensorGenerator | dict) -> None:
         super().__init__()
         self._generator = setup_tensor_generator(generator)
 
     def __repr__(self) -> str:
```

### Comparing `startorch-0.1.0/src/startorch/testing.py` & `startorch-0.1.1a0/src/startorch/testing.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/th3rd/iden/data/generator/example.py` & `startorch-0.1.1a0/src/startorch/integration/iden/data/generator/example.py`

 * *Files identical despite different names*

### Comparing `startorch-0.1.0/src/startorch/timeseries/__init__.py` & `startorch-0.1.1a0/src/startorch/timeseries/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,49 @@
 r"""Contain time series generators."""
 
 from __future__ import annotations
 
 __all__ = [
     "BaseTimeSeriesGenerator",
+    "Concatenate",
+    "ConcatenateTimeSeriesGenerator",
     "Merge",
     "MergeTimeSeriesGenerator",
     "MixedTimeSeries",
     "MixedTimeSeriesGenerator",
     "MultinomialChoice",
     "MultinomialChoiceTimeSeriesGenerator",
     "Periodic",
     "PeriodicTimeSeriesGenerator",
-    "TimeSeries",
-    "TimeSeriesGenerator",
+    "SequenceTimeSeries",
+    "SequenceTimeSeriesGenerator",
+    "TensorTimeSeries",
+    "TensorTimeSeriesGenerator",
     "is_timeseries_generator_config",
     "setup_timeseries_generator",
 ]
 
 from startorch.timeseries.base import (
     BaseTimeSeriesGenerator,
     is_timeseries_generator_config,
     setup_timeseries_generator,
 )
 from startorch.timeseries.choice import MultinomialChoiceTimeSeriesGenerator
 from startorch.timeseries.choice import (
     MultinomialChoiceTimeSeriesGenerator as MultinomialChoice,
 )
-from startorch.timeseries.generic import TimeSeriesGenerator
-from startorch.timeseries.generic import TimeSeriesGenerator as TimeSeries
+from startorch.timeseries.concatenate import ConcatenateTimeSeriesGenerator
+from startorch.timeseries.concatenate import (
+    ConcatenateTimeSeriesGenerator as Concatenate,
+)
 from startorch.timeseries.merge import MergeTimeSeriesGenerator
 from startorch.timeseries.merge import MergeTimeSeriesGenerator as Merge
 from startorch.timeseries.mixed import MixedTimeSeriesGenerator
 from startorch.timeseries.mixed import MixedTimeSeriesGenerator as MixedTimeSeries
 from startorch.timeseries.periodic import PeriodicTimeSeriesGenerator
 from startorch.timeseries.periodic import PeriodicTimeSeriesGenerator as Periodic
+from startorch.timeseries.sequence import SequenceTimeSeriesGenerator
+from startorch.timeseries.sequence import (
+    SequenceTimeSeriesGenerator as SequenceTimeSeries,
+)
+from startorch.timeseries.tensor import TensorTimeSeriesGenerator
+from startorch.timeseries.tensor import TensorTimeSeriesGenerator as TensorTimeSeries
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/base.py` & `startorch-0.1.1a0/src/startorch/timeseries/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 
 class BaseTimeSeriesGenerator(ABC, metaclass=AbstractFactory):
     r"""Define the base class to implement a time series generator.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform
-    >>> from startorch.timeseries import TimeSeries
-    >>> generator = TimeSeries({"value": RandUniform(), "time": RandUniform()})
+    >>> from startorch.timeseries import SequenceTimeSeriesGenerator
+    >>> generator = SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()})
     >>> generator
-    TimeSeriesGenerator(
+    SequenceTimeSeriesGenerator(
       (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=12, batch_size=4)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
 
     ```
@@ -49,28 +50,28 @@
     @abstractmethod
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
         r"""Generate a time series.
 
         Args:
-            seq_len: Specifies the sequence length.
-            batch_size: Specifies the batch size.
-            rng: Specifies an optional random number generator.
+            seq_len: The sequence length.
+            batch_size: The batch size.
+            rng: An optional random number generator.
 
         Returns:
             A batch of time series.
 
         Example usage:
 
         ```pycon
         >>> import torch
         >>> from startorch.sequence import RandUniform
-        >>> from startorch.timeseries import TimeSeries
-        >>> generator = TimeSeries({"value": RandUniform(), "time": RandUniform()})
+        >>> from startorch.timeseries import SequenceTimeSeriesGenerator
+        >>> generator = SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()})
         >>> generator.generate(seq_len=12, batch_size=4)
         {'value': tensor([[...]]), 'time': tensor([[...]])}
 
         ```
         """
 
 
@@ -80,28 +81,29 @@
 
     This function only checks if the value of the key  ``_target_``
     is valid. It does not check the other values. If ``_target_``
     indicates a function, the returned type hint is used to check
     the class.
 
     Args:
-        config: Specifies the configuration to check.
+        config: The configuration to check.
 
     Returns:
         ``True`` if the input configuration is a configuration for a
             ``BaseTimeSeriesGenerator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.timeseries import is_timeseries_generator_config
     >>> is_timeseries_generator_config(
     ...     {
-    ...         "_target_": "startorch.timeseries.TimeSeries",
-    ...         "sequences": {
+    ...         "_target_": "startorch.timeseries.SequenceTimeSeriesGenerator",
+    ...         "generators": {
     ...             "value": {"_target_": "startorch.sequence.RandUniform"},
     ...             "time": {"_target_": "startorch.sequence.RandUniform"},
     ...         },
     ...     }
     ... )
     True
 
@@ -115,34 +117,35 @@
 ) -> BaseTimeSeriesGenerator:
     r"""Set up a time series generator.
 
     The time series generator is instantiated from its configuration
     by using the ``BaseTimeSeriesGenerator`` factory function.
 
     Args:
-        generator: Specifies a time series generator or its
+        generator: A time series generator or its
             configuration.
 
     Returns:
         A time series generator.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.timeseries import setup_timeseries_generator
     >>> setup_timeseries_generator(
     ...     {
-    ...         "_target_": "startorch.timeseries.TimeSeries",
-    ...         "sequences": {
+    ...         "_target_": "startorch.timeseries.SequenceTimeSeriesGenerator",
+    ...         "generators": {
     ...             "value": {"_target_": "startorch.sequence.RandUniform"},
     ...             "time": {"_target_": "startorch.sequence.RandUniform"},
     ...         },
     ...     }
     ... )
-    TimeSeriesGenerator(
+    SequenceTimeSeriesGenerator(
       (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
 
     ```
     """
     if isinstance(generator, dict):
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/choice.py` & `startorch-0.1.1a0/src/startorch/timeseries/choice.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,41 +37,46 @@
         - a key ``'generator'`` which indicates the time series
             generator or its configuration.
         - an optional key ``'weight'`` with a float value which
             indicates the weight of the time series generator.
             If this key is absent, the weight is set to ``1.0``.
 
     Args:
-        generators: Specifies the time series generators and their
+        generators: The time series generators and their
             weights. See above to learn about the expected format.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.timeseries import MultinomialChoice, TimeSeries
+
+    >>> from startorch.timeseries import MultinomialChoice, SequenceTimeSeries
     >>> from startorch.sequence import RandUniform, RandNormal
     >>> generator = MultinomialChoice(
     ...     (
     ...         {
     ...             "weight": 2.0,
-    ...             "generator": TimeSeries({"value": RandUniform(), "time": RandUniform()}),
+    ...             "generator": SequenceTimeSeries(
+    ...                 {"value": RandUniform(), "time": RandUniform()}
+    ...             ),
     ...         },
     ...         {
     ...             "weight": 1.0,
-    ...             "generator": TimeSeries({"value": RandNormal(), "time": RandNormal()}),
+    ...             "generator": SequenceTimeSeries(
+    ...                 {"value": RandNormal(), "time": RandNormal()}
+    ...             ),
     ...         },
     ...     )
     ... )
     >>> generator
     MultinomialChoiceTimeSeriesGenerator(
-      (0) [weight=2.0] TimeSeriesGenerator(
+      (0) [weight=2.0] SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
-      (1) [weight=1.0] TimeSeriesGenerator(
+      (1) [weight=1.0] SequenceTimeSeriesGenerator(
           (value): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
           (time): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
         )
     )
     >>> generator.generate(seq_len=12, batch_size=4)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/generic.py` & `startorch-0.1.1a0/src/startorch/timeseries/sequence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-r"""Contain the implementation of a generic time series generator."""
+r"""Contain the implementation of a time series generator that generates
+time series with sequence generators."""
 
 from __future__ import annotations
 
-__all__ = ["TimeSeriesGenerator"]
+__all__ = ["SequenceTimeSeriesGenerator"]
 
 
 from typing import TYPE_CHECKING
 
 from coola.utils import str_indent, str_mapping
 
 from startorch.sequence.base import BaseSequenceGenerator, setup_sequence_generator
@@ -14,49 +15,51 @@
 
 if TYPE_CHECKING:
     from collections.abc import Hashable, Mapping
 
     import torch
 
 
-class TimeSeriesGenerator(BaseTimeSeriesGenerator):
-    r"""Implement a generic time series generator.
+class SequenceTimeSeriesGenerator(BaseTimeSeriesGenerator):
+    r"""Implement a time series generator that generates time series with
+    sequence generators.
 
     Args:
-        sequences: Specifies the sequence generators or their
+        generators: The sequence generators or their
             configurations.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform
-    >>> from startorch.timeseries import TimeSeries
-    >>> generator = TimeSeries({"value": RandUniform(), "time": RandUniform()})
+    >>> from startorch.timeseries import SequenceTimeSeries
+    >>> generator = SequenceTimeSeries({"value": RandUniform(), "time": RandUniform()})
     >>> generator
-    TimeSeriesGenerator(
+    SequenceTimeSeriesGenerator(
       (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
       (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
     )
     >>> generator.generate(seq_len=12, batch_size=4)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
 
     ```
     """
 
-    def __init__(self, sequences: Mapping[str, BaseSequenceGenerator | dict]) -> None:
+    def __init__(self, generators: Mapping[str, BaseSequenceGenerator | dict]) -> None:
         super().__init__()
-        self._sequences = {
-            key: setup_sequence_generator(generator) for key, generator in sequences.items()
+        self._generators = {
+            key: setup_sequence_generator(generator) for key, generator in generators.items()
         }
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping(self._sequences))
+        args = str_indent(str_mapping(self._generators))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
         self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
         return {
             key: generator.generate(seq_len=seq_len, batch_size=batch_size, rng=rng)
-            for key, generator in self._sequences.items()
+            for key, generator in self._generators.items()
         }
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/merge.py` & `startorch-0.1.1a0/src/startorch/timeseries/merge.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,38 +25,39 @@
 class MergeTimeSeriesGenerator(BaseTimeSeriesGenerator):
     r"""Implement a time series creator that creates time series by
     combining several time series.
 
     The time series are combined by using the time information.
 
     Args:
-        generators: Specifies the time series generators or their
+        generators: The time series generators or their
             configuration.
-        time_key: Specifies the key used to merge the time series by
+        time_key: The key used to merge the time series by
             time.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.timeseries import Merge, TimeSeries
+
+    >>> from startorch.timeseries import Merge, SequenceTimeSeriesGenerator
     >>> from startorch.sequence import RandUniform, RandNormal
     >>> generator = Merge(
     ...     (
-    ...         TimeSeries({"value": RandUniform(), "time": RandUniform()}),
-    ...         TimeSeries({"value": RandNormal(), "time": RandNormal()}),
+    ...         SequenceTimeSeriesGenerator({"value": RandUniform(), "time": RandUniform()}),
+    ...         SequenceTimeSeriesGenerator({"value": RandNormal(), "time": RandNormal()}),
     ...     )
     ... )
     >>> generator
     MergeTimeSeriesGenerator(
       (time_key): time
-      (0): TimeSeriesGenerator(
+      (0): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
-      (1): TimeSeriesGenerator(
+      (1): SequenceTimeSeriesGenerator(
           (value): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
           (time): RandNormalSequenceGenerator(mean=0.0, std=1.0, feature_size=(1,))
         )
     )
     >>> batch = generator.generate(seq_len=12, batch_size=10)
     >>> batch
     {'value': tensor([[...]]), 'time': tensor([[...]])}
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/mixed.py` & `startorch-0.1.1a0/src/startorch/timeseries/mixed.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 
 
 class MixedTimeSeriesGenerator(BaseTimeSeriesGenerator):
     r"""Implement a time series generator that generates time series by
     mixing two sequences of a time series.
 
     Args:
-        generator: Specifies the time series generator or its
+        generator: The time series generator or its
             configuration.
-        key1: Specifies the key of the first sequence to mix.
-        key2: Specifies the key of the second sequence to mix.
+        key1: The key of the first sequence to mix.
+        key2: The key of the second sequence to mix.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.sequence import RandUniform
-    >>> from startorch.timeseries import MixedTimeSeries, TimeSeries
+    >>> from startorch.timeseries import MixedTimeSeries, SequenceTimeSeries
     >>> generator = MixedTimeSeries(
-    ...     TimeSeries({"key1": RandUniform(), "key2": RandUniform()}),
+    ...     SequenceTimeSeries({"key1": RandUniform(), "key2": RandUniform()}),
     ...     key1="key1",
     ...     key2="key2",
     ... )
     >>> generator
     MixedTimeSeriesGenerator(
-      (generator): TimeSeriesGenerator(
+      (generator): SequenceTimeSeriesGenerator(
           (key1): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (key2): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
       (key1): key1
       (key2): key2
     )
     >>> generator.generate(seq_len=12, batch_size=10)
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/periodic.py` & `startorch-0.1.1a0/src/startorch/example/timeseries.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-r"""Implement a time series generator to generate periodic time series
-from a regular time series generator."""
+r"""Contain the implementation of example generator that generates
+sequences from a time series generator."""
 
 from __future__ import annotations
 
-__all__ = ["PeriodicTimeSeriesGenerator"]
+__all__ = ["TimeSeriesExampleGenerator"]
+
 
-import math
 from typing import TYPE_CHECKING
 
-from batchtensor.nested import repeat_along_seq, slice_along_seq
 from coola.utils import str_indent, str_mapping
 
-from startorch.periodic.timeseries.base import BasePeriodicTimeSeriesGenerator
-from startorch.tensor.base import BaseTensorGenerator, setup_tensor_generator
+from startorch.example.base import BaseExampleGenerator
+from startorch.tensor.base import setup_tensor_generator
 from startorch.timeseries.base import (
     BaseTimeSeriesGenerator,
     setup_timeseries_generator,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Hashable
 
     import torch
 
+    from startorch.tensor.base import BaseTensorGenerator
+
 
-class PeriodicTimeSeriesGenerator(BaseTimeSeriesGenerator):
-    r"""Implement a time series generator to generate periodic time
-    series from a regular time series generator.
+class TimeSeriesExampleGenerator(BaseExampleGenerator):
+    r"""Implement an example generator to generate time series.
 
     Args:
-        timeseries: Specifies a time series generator or its
-            configuration that is used to generate the periodic
-            pattern.
-        period: Specifies the period length sampler or its
-            configuration. This sampler is used to sample the period
-            length at each batch.
+        generators: A time series generator or its
+            configuration.
+        seq_len: The sequence length sampler or its
+            configuration. This sampler is used to sample the
+            sequence length at each batch.
 
     Example usage:
 
     ```pycon
-    >>> from startorch.timeseries import Periodic, TimeSeries
-    >>> from startorch.sequence import RandUniform
+
+    >>> from startorch.example import TimeSeriesExampleGenerator
+    >>> from startorch.timeseries import SequenceTimeSeriesGenerator
+    >>> from startorch.sequence import Periodic, RandUniform
     >>> from startorch.tensor import RandInt
-    >>> generator = Periodic(
-    ...     TimeSeries({"value": RandUniform(), "time": RandUniform()}), period=RandInt(2, 5)
+    >>> generator = TimeSeriesExampleGenerator(
+    ...     generators=SequenceTimeSeriesGenerator(
+    ...         {"value": RandUniform(), "time": RandUniform()}
+    ...     ),
+    ...     seq_len=RandInt(2, 5),
     ... )
     >>> generator
-    PeriodicTimeSeriesGenerator(
-      (sequence): TimeSeriesGenerator(
+    TimeSeriesExampleGenerator(
+      (generators): SequenceTimeSeriesGenerator(
           (value): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
           (time): RandUniformSequenceGenerator(low=0.0, high=1.0, feature_size=(1,))
         )
-      (period): RandIntTensorGenerator(low=2, high=5)
+      (seq_len): RandIntTensorGenerator(low=2, high=5)
     )
-    >>> generator.generate(seq_len=10, batch_size=2)
+    >>> generator.generate(batch_size=10)
     {'value': tensor([[...]]), 'time': tensor([[...]])}
 
     ```
     """
 
     def __init__(
         self,
-        timeseries: BaseTimeSeriesGenerator | BasePeriodicTimeSeriesGenerator | dict,
-        period: BaseTensorGenerator | dict,
+        generators: BaseTimeSeriesGenerator | dict,
+        seq_len: BaseTensorGenerator | dict,
     ) -> None:
         super().__init__()
-        self._timeseries = setup_timeseries_generator(timeseries)
-        self._period = setup_tensor_generator(period)
+        self._generators = setup_timeseries_generator(generators)
+        self._seq_len = setup_tensor_generator(seq_len)
 
     def __repr__(self) -> str:
-        args = str_indent(str_mapping({"sequence": self._timeseries, "period": self._period}))
+        args = str_indent(str_mapping({"generators": self._generators, "seq_len": self._seq_len}))
         return f"{self.__class__.__qualname__}(\n  {args}\n)"
 
     def generate(
-        self, seq_len: int, batch_size: int = 1, rng: torch.Generator | None = None
+        self, batch_size: int = 1, rng: torch.Generator | None = None
     ) -> dict[Hashable, torch.Tensor]:
-        period = int(self._period.generate((1,), rng=rng).item())
-        if isinstance(self._timeseries, BasePeriodicTimeSeriesGenerator):
-            return self._timeseries.generate(
-                seq_len=seq_len, period=period, batch_size=batch_size, rng=rng
-            )
-        data = self._timeseries.generate(seq_len=period, batch_size=batch_size, rng=rng)
-        data = repeat_along_seq(data, math.ceil(seq_len / period))
-        return slice_along_seq(data, stop=seq_len)
+        seq_len = int(self._seq_len.generate((1,), rng=rng).item())
+        return self._generators.generate(seq_len=seq_len, batch_size=batch_size, rng=rng)
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/utils/merge.py` & `startorch-0.1.1a0/src/startorch/timeseries/utils/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,27 +37,28 @@
     batches in each dictionary should have a shape
     ``(batch_size, sequence_length, *)`` where `*` means any
     number of dimensions. Only the sequence dimension can change
     between the time series. This function works for a variable
     number of features.
 
     Args:
-        timeseries: Specifies the list of time series to merge.
+        timeseries: The list of time series to merge.
             See the description above to know the format of the time
             series.
-        time_key: Specifies the key that contains the time data used
+        time_key: The key that contains the time data used
             to merge the time series.
 
     Returns:
         The merged time series. The dictionary has the same structure
             that the input time series.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch import constants as ct
     >>> from startorch.timeseries.utils import merge_by_time
     >>> batch = merge_by_time(
     ...     [
     ...         {
     ...             ct.TIME: torch.tensor([[[5], [10], [15], [20], [25]]], dtype=torch.float),
```

### Comparing `startorch-0.1.0/src/startorch/timeseries/utils/mixed.py` & `startorch-0.1.1a0/src/startorch/timeseries/utils/mixed.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,24 +16,25 @@
     If the input batches are
     ``x = [x[0], x[1], x[2], x[3], x[4], ...]`` and
     ``y = [y[0], y[1], y[2], y[3], y[4], ...]``, the output batches
     are: ``x = [x[0], y[1], x[2], y[3], x[4], ...]`` and
     ``y = [y[0], x[1], y[2], x[3], y[4], ...]``
 
     Args:
-        x: Specifies the first batch.
-        y: Specifies the second batch. It must have the same shape
+        x: The first batch.
+        y: The second batch. It must have the same shape
             as ``x``.
 
     Returns:
         The batches with mixed values along the sequence dimension.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.timeseries.utils import mix2sequences
     >>> mix2sequences(
     ...     torch.arange(10).view(2, 5),
     ...     torch.arange(10, 20).view(2, 5),
     ... )
     (tensor([[ 0, 11,  2, 13,  4], [ 5, 16,  7, 18,  9]]),
```

### Comparing `startorch-0.1.0/src/startorch/utils/batch.py` & `startorch-0.1.1a0/src/startorch/utils/batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,24 @@
     import torch
 
 
 def scale_batch(batch: torch.Tensor, scale: str = "identity") -> torch.Tensor:
     r"""Scale a batch.
 
     Args:
-        batch: Specifies the batch to scale.
-        scale: Specifies the scaling transformation.
+        batch: The batch to scale.
+        scale: The scaling transformation.
 
     Returns:
         The scaled batch.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.batch import scale_batch
     >>> batch = torch.arange(10).view(2, 5)
     >>> scale_batch(batch, scale="asinh")
     tensor([[0.0000, 0.8814, 1.4436, 1.8184, 2.0947],
             [2.3124, 2.4918, 2.6441, 2.7765, 2.8934]])
```

### Comparing `startorch-0.1.0/src/startorch/utils/conversion.py` & `startorch-0.1.1a0/src/startorch/utils/conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,22 +14,23 @@
     from collections.abc import Sequence
 
 
 def to_array(data: Sequence | torch.Tensor | np.ndarray) -> np.ndarray:
     r"""Convert the input to a ``numpy.ndarray``.
 
     Args:
-        data: Specifies the data to convert to an array.
+        data: The data to convert to an array.
 
     Returns:
         A NumPy array.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.conversion import to_array
     >>> x = to_array([1, 2, 3, 4, 5])
     >>> x
     array([1, 2, 3, 4, 5])
 
     ```
     """
@@ -40,22 +41,23 @@
     return np.asarray(data)
 
 
 def to_tensor(data: torch.Tensor | np.ndarray | Sequence) -> torch.Tensor:
     r"""Convert the input to a ``torch.Tensor``.
 
     Args:
-        data: Specifies the data to convert to a tensor.
+        data: The data to convert to a tensor.
 
     Returns:
         A tensor.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.conversion import to_tensor
     >>> x = to_tensor([1, 2, 3, 4, 5])
     >>> x
     tensor([1, 2, 3, 4, 5])
 
     ```
     """
@@ -68,22 +70,23 @@
 
 def to_tuple(value: Any) -> tuple:
     r"""Convert a value to a tuple.
 
     This function is a no-op if the input is a tuple.
 
     Args:
-        value: Specifies the value to convert.
+        value: The value to convert.
 
     Returns:
         The input value in a tuple.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.conversion import to_tuple
     >>> to_tuple(1)
     (1,)
     >>> to_tuple("abc")
     ('abc',)
 
     ```
```

### Comparing `startorch-0.1.0/src/startorch/utils/format.py` & `startorch-0.1.1a0/src/startorch/utils/format.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,24 +13,25 @@
     from collections.abc import Sequence
 
 
 def str_target_object(config: dict) -> str:
     r"""Get a string that indicates the target object in the config.
 
     Args:
-        config: Specifies a config using the ``object_factory``
+        config: A config using the ``object_factory``
             library. This dict is expected to have a key
             ``'_target_'`` to indicate the target object.
 
     Returns:
         A string with the target object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.format import str_target_object
     >>> str_target_object({OBJECT_TARGET: "something.MyClass"})
     [_target_: something.MyClass]
     >>> str_target_object({})
     [_target_: N/A]
 
     ```
@@ -39,26 +40,27 @@
 
 
 def str_weighted_modules(modules: Sequence, weights: Sequence, num_spaces: int = 2) -> str:
     r"""Compute a pretty representation of a sequence of modules where
     each module is associated to a weight.
 
     Args:
-        modules: Specifies the modules.
-        weights: Specifies the weights. The ``weights`` should have
+        modules: The modules.
+        weights: The weights. The ``weights`` should have
             the same length that ``modules``.
-        num_spaces: Specifies the number of spaces used for the
+        num_spaces: The number of spaces used for the
             indentation.
 
     Returns:
         The string representation of the modules.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.format import str_weighted_modules
     >>> print(str_weighted_modules(modules=["abc", "something\nelse"], weights=[1, 2]))
     (0) [weight=1] abc
     (1) [weight=2] something
       else
 
     ```
```

### Comparing `startorch-0.1.0/src/startorch/utils/imports.py` & `startorch-0.1.1a0/src/startorch/utils/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     Raises:
         RuntimeError: if the ``iden`` package is not installed.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import check_iden
     >>> check_iden()
 
     ```
     """
     if not is_iden_available():
         msg = (
@@ -43,14 +44,15 @@
 
 def is_iden_available() -> bool:
     r"""Indicate if the ``iden`` package is installed or not.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import is_iden_available
     >>> is_iden_available()
 
     ```
     """
     return find_spec("iden") is not None
 
@@ -65,14 +67,15 @@
 
     Raises:
         RuntimeError: if the ``matplotlib`` package is not installed.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import check_matplotlib
     >>> check_matplotlib()
 
     ```
     """
     if not is_matplotlib_available():
         msg = (
@@ -85,14 +88,15 @@
 
 def is_matplotlib_available() -> bool:
     r"""Indicate if the ``matplotlib`` package is installed or not.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import is_matplotlib_available
     >>> is_matplotlib_available()
 
     ```
     """
     return find_spec("matplotlib") is not None
 
@@ -107,14 +111,15 @@
 
     Raises:
         RuntimeError: if the ``plotly`` package is not installed.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import check_plotly
     >>> check_plotly()
 
     ```
     """
     if not is_plotly_available():
         msg = (
@@ -127,13 +132,14 @@
 
 def is_plotly_available() -> bool:
     r"""Indicate if the ``plotly`` package is installed or not.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.imports import is_plotly_available
     >>> is_plotly_available()
 
     ```
     """
     return find_spec("plotly") is not None
```

### Comparing `startorch-0.1.0/src/startorch/utils/seed.py` & `startorch-0.1.1a0/src/startorch/utils/seed.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 import torch
 
 
 def get_random_seed(seed: int) -> int:
     r"""Get a random seed.
 
     Args:
-        seed: Specifies a random seed to make the process
+        seed: A random seed to make the process
             reproducible.
 
     Returns:
         int: A random seed. The value is between ``-2 ** 63`` and
             ``2 ** 63 - 1``.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.seed import get_random_seed
     >>> get_random_seed(44)
     6176747449835261347
 
     ```
     """
     return torch.randint(-(2**63), 2**63 - 1, size=(1,), generator=get_torch_generator(seed)).item()
@@ -33,23 +34,24 @@
 
 def get_torch_generator(
     random_seed: int = 1, device: torch.device | str | None = "cpu"
 ) -> torch.Generator:
     r"""Create a ``torch.Generator`` initialized with a given seed.
 
     Args:
-        random_seed: Specifies a random seed.
-        device: Specifies the desired device for the generator.
+        random_seed: A random seed.
+        device: The desired device for the generator.
 
     Returns:
         A ``torch.Generator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.seed import get_torch_generator
     >>> generator = get_torch_generator(42)
     >>> torch.rand(2, 4, generator=generator)
     tensor([[0.8823, 0.9150, 0.3829, 0.9593],
             [0.3904, 0.6009, 0.2566, 0.7936]])
     >>> generator = get_torch_generator(42)
@@ -64,23 +66,24 @@
     return generator
 
 
 def setup_torch_generator(generator_or_seed: int | torch.Generator) -> torch.Generator:
     r"""Set up a ``torch.Generator`` object.
 
     Args:
-        generator_or_seed: Specifies a ``torch.Generator`` object or
+        generator_or_seed: A ``torch.Generator`` object or
             a random seed.
 
     Returns:
         A ``torch.Generator`` object.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.seed import setup_torch_generator
     >>> generator = setup_torch_generator(42)
     >>> generator
     <torch._C.Generator object at 0x...>
 
     ```
     """
```

### Comparing `startorch-0.1.0/src/startorch/utils/validation.py` & `startorch-0.1.1a0/src/startorch/utils/validation.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,49 +14,51 @@
 
 
 def check_feature_size(value: int | Any, low: int = 1) -> None:
     r"""Check if the given value is a valid feature size i.e. number of
     features.
 
     Args:
-        value: Specifies the value to check.
-        low: Specifies the minimum value (inclusive).
+        value: The value to check.
+        low: The minimum value (inclusive).
 
     Raises:
         TypeError: if the input is not an integer.
         RuntimeError: if the value is not greater than 0
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.validation import check_feature_size
     >>> check_feature_size(5)
 
     ```
     """
     check_integer_ge(value, name="feature_size", low=low)
 
 
 def check_interval(value: float | Any, low: float, high: float, name: str) -> None:
     r"""Check if the given value is an interval.
 
     Args:
-        value: Specifies the value to check.
-        low: Specifies the minimum value (inclusive).
-        high: Specifies the maximum value (exclusive).
-        name: Specifies the variable name.
+        value: The value to check.
+        low: The minimum value (inclusive).
+        high: The maximum value (exclusive).
+        name: The variable name.
 
     Raises:
         TypeError: if the input is not an integer or float.
         RuntimeError: if the value is not in the interval
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.validation import check_interval
     >>> check_interval(1, low=-1.0, high=2.0, name="my_variable")
 
     ```
     """
     if not isinstance(value, (int, float)):
@@ -70,47 +72,49 @@
         raise RuntimeError(msg)
 
 
 def check_num_examples(value: int | Any) -> None:
     r"""Check if the given value is a valid number of examples.
 
     Args:
-        value: Specifies the value to check.
+        value: The value to check.
 
     Raises:
         TypeError: if the input is not an integer.
         RuntimeError: if the value is not greater than 0
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.validation import check_num_examples
     >>> check_num_examples(5)
 
     ```
     """
     check_integer_ge(value, low=1, name="num_examples")
 
 
 def check_integer_ge(value: int | Any, low: int, name: str) -> None:
     r"""Check if the given value is a valid positive integer.
 
     Args:
-        value: Specifies the value to check.
-        low: Specifies the minimum value (inclusive).
-        name: Specifies the variable name.
+        value: The value to check.
+        low: The minimum value (inclusive).
+        name: The variable name.
 
     Raises:
         TypeError: if the input is not an integer.
         RuntimeError: if the value is not greater than 0
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.validation import check_integer_ge
     >>> check_integer_ge(5, low=0, name="feature_size")
 
     ```
     """
     if not isinstance(value, int):
@@ -124,24 +128,25 @@
         raise RuntimeError(msg)
 
 
 def check_std(value: float | Any, name: str = "std") -> None:
     r"""Check if the given value is a valid standard deviation.
 
     Args:
-        value: Specifies the value to check.
-        name: Specifies the variable name.
+        value: The value to check.
+        name: The variable name.
 
     Raises:
         TypeError: if the input is not an integer or float.
         RuntimeError: if the value is not greater than 0
 
     Example usage:
 
     ```pycon
+
     >>> import torch
     >>> from startorch.utils.validation import check_std
     >>> check_std(1.2)
 
     ```
     """
     if not isinstance(value, (int, float)):
```

### Comparing `startorch-0.1.0/src/startorch/utils/weight.py` & `startorch-0.1.1a0/src/startorch/utils/weight.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     import torch
 
 
 def prepare_probabilities(weights: torch.Tensor | Sequence[float]) -> torch.Tensor:
     r"""Convert un-normalized positive weights to probabilities.
 
     Args:
-        weights: Specifies the vector of weights associated to each
+        weights: The vector of weights associated to each
             category. The weights have to be positive. It must be a
             float tensor of shape ``(num_categories,)`` or a
             ``Sequence``.
 
     Returns:
         The vector of probability associated at each category.
             The output is a ``torch.Tensor`` of type float and
@@ -35,14 +35,15 @@
 
     Raises:
         ValueError: if the weights are not valid.
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.weight import prepare_probabilities
     >>> prepare_probabilities([1, 1, 1, 1])
     tensor([0.2500, 0.2500, 0.2500, 0.2500])
 
     ```
     """
     weights = to_tensor(weights)
@@ -74,25 +75,26 @@
         - a key ``'generator'`` which indicates the tensor generator
             or its configuration.
         - an optional key ``'weight'`` with a float value which
             indicates the weight of the tensor generator.
             If this key is absent, the weight is set to ``1.0``.
 
     Args:
-        generators: Specifies the tensor generators and their weights.
+        generators: The tensor generators and their weights.
             See above to learn about the expected format.
 
     Returns:
         A tuple with two items:
             - a tuple of generators or their configurations
             - a tuple of generator weights
 
     Example usage:
 
     ```pycon
+
     >>> from startorch.utils.weight import prepare_weighted_generators
     >>> from startorch.tensor import RandUniform, RandNormal
     >>> prepare_weighted_generators(
     ...     (
     ...         {"weight": 2.0, "generator": RandUniform()},
     ...         {"weight": 1.0, "generator": RandNormal()},
     ...     )
```

### Comparing `startorch-0.1.0/PKG-INFO` & `startorch-0.1.1a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: startorch
-Version: 0.1.0
+Version: 0.1.1a0
 Summary: synthetic time-series generator in PyTorch
 Home-page: https://github.com/durandtibo/startorch
 License: BSD-3-Clause
 Keywords: synthetic,time-series,pytorch
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -22,37 +22,42 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: all
 Requires-Dist: batchtensor (>=0.0.2,<0.1)
 Requires-Dist: coola (>=0.2,<1.0)
 Requires-Dist: iden (>=0.0.2,<0.1) ; extra == "all"
 Requires-Dist: matplotlib (>=3.6,<4.0) ; extra == "all"
-Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: objectory (>=0.1,<1.0)
 Requires-Dist: plotly (>=5.0,<6.0) ; extra == "all"
+Requires-Dist: torch (>=2.0,<2.3) ; sys_platform == "darwin" and platform_machine != "arm64"
 Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/durandtibo/startorch
 Description-Content-Type: text/markdown
 
 # startorch
 
 <p align="center">
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="CI" src="https://github.com/durandtibo/startorch/workflows/CI/badge.svg">
     </a>
-    <a href="https://durandtibo.github.io/startorch/">
-        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation/badge.svg">
-    </a>
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="Nightly Tests" src="https://github.com/durandtibo/startorch/workflows/Nightly%20Tests/badge.svg">
     </a>
     <a href="https://github.com/durandtibo/startorch/actions">
         <img alt="Nightly Package Tests" src="https://github.com/durandtibo/startorch/workflows/Nightly%20Package%20Tests/badge.svg">
     </a>
     <br/>
+    <a href="https://durandtibo.github.io/startorch/">
+        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation%20(stable)/badge.svg">
+    </a>
+    <a href="https://durandtibo.github.io/startorch/">
+        <img alt="Documentation" src="https://github.com/durandtibo/startorch/workflows/Documentation%20(unstable)/badge.svg">
+    </a>
+    <br/>
     <a href="https://codecov.io/gh/durandtibo/startorch">
         <img alt="Codecov" src="https://codecov.io/gh/durandtibo/startorch/branch/main/graph/badge.svg">
     </a>
     <a href="https://codeclimate.com/github/durandtibo/startorch/maintainability">
         <img src="https://api.codeclimate.com/v1/badges/05a12c503bf3be80a00b/maintainability" />
     </a>
     <a href="https://codeclimate.com/github/durandtibo/startorch/test_coverage">
@@ -129,15 +134,15 @@
 - [API stability](#api-stability)
 - [License](#license)
 
 ## Dependencies
 
 | `startorch` | `batchtensor`  | `coola`      | `objectory`  | `numpy`       | `torch`      | `iden`<sup>*</sup> | `matplotlib`<sup>*</sup> | `plotly`<sup>*</sup> | `python`      |
 |-------------|----------------|--------------|--------------|---------------|--------------|--------------------|--------------------------|----------------------|---------------|
-| `main`      | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
+| `main`      | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.23,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
 | `0.1.0`     | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` | `>=2.0,<3.0` | `>=0.0.2,<0.1`     | `>=3.6,<4.0`             | `>=5.0,<6.0`         | `>=3.9,<3.12` |
 
 <sup>*</sup> indicates an optional dependency
 
 <details>
     <summary>older versions</summary>
```

#### html2text {}

```diff
@@ -1,27 +1,29 @@
-Metadata-Version: 2.1 Name: startorch Version: 0.1.0 Summary: synthetic time-
+Metadata-Version: 2.1 Name: startorch Version: 0.1.1a0 Summary: synthetic time-
 series generator in PyTorch Home-page: https://github.com/durandtibo/startorch
 License: BSD-3-Clause Keywords: synthetic,time-series,pytorch Author: Thibaut
 Durand Author-email: durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
+Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Software Development :: Libraries Provides-Extra: all Requires-Dist:
 batchtensor (>=0.0.2,<0.1) Requires-Dist: coola (>=0.2,<1.0) Requires-Dist:
 iden (>=0.0.2,<0.1) ; extra == "all" Requires-Dist: matplotlib (>=3.6,<4.0) ;
-extra == "all" Requires-Dist: numpy (>=1.21,<2.0) Requires-Dist: objectory
+extra == "all" Requires-Dist: numpy (>=1.23,<2.0) Requires-Dist: objectory
 (>=0.1,<1.0) Requires-Dist: plotly (>=5.0,<6.0) ; extra == "all" Requires-Dist:
-torch (>=2.0,<3.0) Project-URL: Repository, https://github.com/durandtibo/
-startorch Description-Content-Type: text/markdown # startorch
-           _[_C_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
+torch (>=2.0,<2.3) ; sys_platform == "darwin" and platform_machine != "arm64"
+Requires-Dist: torch (>=2.0,<3.0) Project-URL: Repository, https://github.com/
+durandtibo/startorch Description-Content-Type: text/markdown # startorch
+                  _[_C_I_]_[_N_i_g_h_t_l_y_ _T_e_s_t_s_]_[_N_i_g_h_t_l_y_ _P_a_c_k_a_g_e_ _T_e_s_t_s_]
+                        _[_D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_]
      _[_C_o_d_e_c_o_v_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_0_5_a_1_2_c_5_0_3_b_f_3_b_e_8_0_a_0_0_b_/
  _m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_]_[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_0_5_a_1_2_c_5_0_3_b_f_3_b_e_8_0_a_0_0_b_/
                                 _t_e_s_t___c_o_v_e_r_a_g_e_]
         _[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]_[_R_u_f_f_]_[_D_o_c_ _s_t_y_l_e_:_ _g_o_o_g_l_e_]
                      _[_P_Y_P_I_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]_[_B_S_D_-_3_-_C_l_a_u_s_e_]
                         _[_D_o_w_n_l_o_a_d_s_]_[_M_o_n_t_h_l_y_ _d_o_w_n_l_o_a_d_s_]
 --- ## Overview Collecting datasets to train Machine Learning models can be
@@ -40,15 +42,15 @@
 - [Documentation](https://durandtibo.github.io/startorch/) - [Installation]
 (https://durandtibo.github.io/startorch/get_started/) - [Contributing]
 (#contributing) - [API stability](#api-stability) - [License](#license) ##
 Dependencies | `startorch` | `batchtensor` | `coola` | `objectory` | `numpy` |
 `torch` | `iden`* | `matplotlib`* | `plotly`* | `python` | |-------------|-----
 -----------|--------------|--------------|---------------|--------------|------
 --------------|--------------------------|----------------------|--------------
--| | `main` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
+-| | `main` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.23,<2.0` |
 `>=2.0,<3.0` | `>=0.0.2,<0.1` | `>=3.6,<4.0` | `>=5.0,<6.0` | `>=3.9,<3.12` | |
 `0.1.0` | `>=0.0.1,<0.1` | `>=0.2,<1.0` | `>=0.1,<1.0` | `>=1.22,<2.0` |
 `>=2.0,<3.0` | `>=0.0.2,<0.1` | `>=3.6,<4.0` | `>=5.0,<6.0` | `>=3.9,<3.12` | *
 indicates an optional dependency older versions | `startorch` | `coola` |
 `objectory` | `redcat` | `torch` | `matplotlib`* | `plotly`* | `python` | |----
 ---------|--------------------|------------------|--------------------|--------
 ------|--------------------------|----------------------|---------------| |
```

