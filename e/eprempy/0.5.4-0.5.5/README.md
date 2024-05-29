# Comparing `tmp/eprempy-0.5.4.tar.gz` & `tmp/eprempy-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eprempy-0.5.4.tar", max compression
+gzip compressed data, was "eprempy-0.5.5.tar", max compression
```

## Comparing `eprempy-0.5.4.tar` & `eprempy-0.5.5.tar`

### file list

```diff
@@ -1,98 +1,178 @@
--rwxr-xr-x   0        0        0     1513 2023-12-18 17:25:57.411106 eprempy-0.5.4/LICENSE
--rw-r--r--   0        0        0    10899 2024-03-27 21:41:55.392748 eprempy-0.5.4/README.md
--rw-r--r--   0        0        0      769 2024-03-27 21:44:08.161033 eprempy-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      298 2024-01-16 19:17:26.814570 eprempy-0.5.4/src/eprempy/__init__.py
--rw-r--r--   0        0        0     2513 2024-02-09 20:00:09.547665 eprempy-0.5.4/src/eprempy/__main__.py
--rw-r--r--   0        0        0     4067 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/_project_main.py
--rw-r--r--   0        0        0    38096 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/aliased.py
--rw-r--r--   0        0        0    10750 2024-02-01 21:56:36.730088 eprempy-0.5.4/src/eprempy/atomic.py
--rw-r--r--   0        0        0     3068 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/__init__.py
--rw-r--r--   0        0        0    11541 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/_abcs.py
--rw-r--r--   0        0        0     9699 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/_protocols.py
--rw-r--r--   0        0        0     1291 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/_types.py
--rw-r--r--   0        0        0      379 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/abc.py
--rw-r--r--   0        0        0     3558 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/base/mixins.py
--rw-r--r--   0        0        0     6643 2024-02-16 21:43:35.579405 eprempy-0.5.4/src/eprempy/cli.py
--rw-r--r--   0        0        0    37520 2024-02-19 22:23:32.972106 eprempy-0.5.4/src/eprempy/container.py
--rw-r--r--   0        0        0      872 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/datafile/__init__.py
--rw-r--r--   0        0        0     3038 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/datafile/_core.py
--rw-r--r--   0        0        0    13619 2024-02-01 21:56:36.730088 eprempy-0.5.4/src/eprempy/datafile/_interfaces.py
--rw-r--r--   0        0        0      838 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/datafile/_reference.py
--rw-r--r--   0        0        0     8597 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/datafile/_viewers.py
--rw-r--r--   0        0        0    14024 2024-03-27 21:35:17.659905 eprempy-0.5.4/src/eprempy/eprem.py
--rw-r--r--   0        0        0    19560 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/etc.py
--rw-r--r--   0        0        0     6421 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/exceptions.py
--rw-r--r--   0        0        0     2535 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/interfaces.py
--rw-r--r--   0        0        0      452 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measurable/__init__.py
--rw-r--r--   0        0        0     1649 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/measured/__init__.py
--rw-r--r--   0        0        0     3554 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_context.py
--rw-r--r--   0        0        0      843 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_convert.py
--rw-r--r--   0        0        0     1881 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_factories.py
--rw-r--r--   0        0        0      872 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_object.py
--rw-r--r--   0        0        0        0 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_operators.py
--rw-r--r--   0        0        0     2499 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_sequence.py
--rw-r--r--   0        0        0     2710 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_types.py
--rw-r--r--   0        0        0      530 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_units.py
--rw-r--r--   0        0        0      781 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/measured/_value.py
--rw-r--r--   0        0        0     4334 2024-01-22 22:28:21.800484 eprempy-0.5.4/src/eprempy/metric/__init__.py
--rw-r--r--   0        0        0    19397 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/metric/_conversions.py
--rw-r--r--   0        0        0    26244 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/metric/_defined.py
--rw-r--r--   0        0        0     3013 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/metric/_dimensions.py
--rw-r--r--   0        0        0      804 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/metric/_exceptions.py
--rw-r--r--   0        0        0    20947 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/metric/_reference.py
--rw-r--r--   0        0        0    13685 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/metric/_systems.py
--rw-r--r--   0        0        0     1011 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/metric/_types.py
--rw-r--r--   0        0        0    20543 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/metric/_units.py
--rw-r--r--   0        0        0     1893 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/numeric/__init__.py
--rw-r--r--   0        0        0    27098 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/numeric/_array.py
--rw-r--r--   0        0        0     3999 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_data.py
--rw-r--r--   0        0        0     2944 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_factory.py
--rw-r--r--   0        0        0     2105 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_implementation.py
--rw-r--r--   0        0        0    22263 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/numeric/_index.py
--rw-r--r--   0        0        0    16116 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_mixins.py
--rw-r--r--   0        0        0     7169 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_objects.py
--rw-r--r--   0        0        0    12011 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/numeric/_operations.py
--rw-r--r--   0        0        0     4363 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/numeric/_operators.py
--rw-r--r--   0        0        0      637 2023-12-18 17:25:57.415106 eprempy-0.5.4/src/eprempy/observable/__init__.py
--rw-r--r--   0        0        0    66067 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/observable/_interfaces.py
--rw-r--r--   0        0        0    20418 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/observable/_objects.py
--rw-r--r--   0        0        0     5829 2024-02-16 16:58:53.068415 eprempy-0.5.4/src/eprempy/parameter/__init__.py
--rw-r--r--   0        0        0    13237 2024-02-16 16:58:53.068415 eprempy-0.5.4/src/eprempy/parameter/_config.py
--rw-r--r--   0        0        0    12922 2024-03-27 21:35:17.659905 eprempy-0.5.4/src/eprempy/parameter/_metadata.py
--rw-r--r--   0        0        0     7762 2024-02-16 21:43:35.579405 eprempy-0.5.4/src/eprempy/parameter/_runtime.py
--rw-r--r--   0        0        0    15954 2024-02-16 21:43:35.579405 eprempy-0.5.4/src/eprempy/parameter/_src.py
--rw-r--r--   0        0        0    20943 2024-03-27 19:22:59.867663 eprempy-0.5.4/src/eprempy/parameter/reference.json
--rw-r--r--   0        0        0    27683 2024-03-27 19:25:57.511816 eprempy-0.5.4/src/eprempy/parameter/reference.py
--rw-r--r--   0        0        0     7210 2024-01-17 20:28:37.607261 eprempy-0.5.4/src/eprempy/paths.py
--rw-r--r--   0        0        0    18010 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/physical/__init__.py
--rw-r--r--   0        0        0     6544 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/physical/_array.py
--rw-r--r--   0        0        0    17721 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/physical/_axes.py
--rw-r--r--   0        0        0    13547 2024-03-27 21:35:17.659905 eprempy-0.5.4/src/eprempy/physical/_axis.py
--rw-r--r--   0        0        0     2249 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_axis_factories.py
--rw-r--r--   0        0        0      150 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/physical/_exceptions.py
--rw-r--r--   0        0        0     4163 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_object.py
--rw-r--r--   0        0        0     5868 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_object_factories.py
--rw-r--r--   0        0        0    21876 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/physical/_operations.py
--rw-r--r--   0        0        0     2658 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/physical/_scalar.py
--rw-r--r--   0        0        0     2030 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_tensor.py
--rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_types.py
--rw-r--r--   0        0        0     1696 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/physical/_vector.py
--rw-r--r--   0        0        0    40811 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/project.py
--rw-r--r--   0        0        0     4789 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/quantity/__init__.py
--rw-r--r--   0        0        0      400 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/quantity/_exceptions.py
--rw-r--r--   0        0        0     9972 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/quantity/_functions.py
--rw-r--r--   0        0        0     2093 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/quantity/_measurement.py
--rw-r--r--   0        0        0     3790 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/real/__init__.py
--rw-r--r--   0        0        0    11506 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/real/_array.py
--rw-r--r--   0        0        0     4891 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/real/_objects.py
--rw-r--r--   0        0        0      707 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/real/_types.py
--rw-r--r--   0        0        0     5785 2024-01-22 22:28:21.804484 eprempy-0.5.4/src/eprempy/reference.py
--rw-r--r--   0        0        0     1756 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/symbolic/__init__.py
--rw-r--r--   0        0        0    13984 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/symbolic/_expression.py
--rw-r--r--   0        0        0    31307 2024-01-24 16:54:00.366890 eprempy-0.5.4/src/eprempy/symbolic/_operand.py
--rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/symbolic/_operator.py
--rw-r--r--   0        0        0     8534 2024-01-17 20:28:37.611261 eprempy-0.5.4/src/eprempy/symbolic/_parser.py
--rw-r--r--   0        0        0     3018 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/symbolic/_part.py
--rw-r--r--   0        0        0      647 2023-12-18 17:25:57.419106 eprempy-0.5.4/src/eprempy/typehelp.py
--rw-r--r--   0        0        0     9023 2024-02-01 21:56:36.734088 eprempy-0.5.4/src/eprempy/universal.py
--rw-r--r--   0        0        0    11598 1970-01-01 00:00:00.000000 eprempy-0.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1513 2023-12-18 17:25:57.411106 eprempy-0.5.5/LICENSE
+-rw-r--r--   0        0        0    10899 2024-03-27 21:41:55.392748 eprempy-0.5.5/README.md
+-rw-r--r--   0        0        0      769 2024-05-29 14:54:01.233232 eprempy-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-01-16 19:17:26.814570 eprempy-0.5.5/src/eprempy/__init__.py
+-rw-r--r--   0        0        0     2513 2024-02-09 20:00:09.547665 eprempy-0.5.5/src/eprempy/__main__.py
+-rw-r--r--   0        0        0     4067 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/_project_main.py
+-rw-r--r--   0        0        0    38096 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/aliased.py
+-rw-r--r--   0        0        0    10750 2024-02-01 21:56:36.730088 eprempy-0.5.5/src/eprempy/atomic.py
+-rw-r--r--   0        0        0     3068 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/__init__.py
+-rw-r--r--   0        0        0     4939 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/base/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    19155 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_abcs.cpython-311.pyc
+-rw-r--r--   0        0        0    17932 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_protocols.cpython-311.pyc
+-rw-r--r--   0        0        0     1217 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/_types.cpython-311.pyc
+-rw-r--r--   0        0        0      576 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/base/__pycache__/abc.cpython-311.pyc
+-rw-r--r--   0        0        0     5768 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/base/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    11541 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_abcs.py
+-rw-r--r--   0        0        0     9699 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_protocols.py
+-rw-r--r--   0        0        0     1291 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/_types.py
+-rw-r--r--   0        0        0      379 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/abc.py
+-rw-r--r--   0        0        0     3558 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/base/mixins.py
+-rw-r--r--   0        0        0     6643 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/cli.py
+-rw-r--r--   0        0        0    37520 2024-02-19 22:23:32.972106 eprempy-0.5.5/src/eprempy/container.py
+-rw-r--r--   0        0        0      872 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/__init__.py
+-rw-r--r--   0        0        0     1306 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7386 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_core.cpython-311.pyc
+-rw-r--r--   0        0        0    22272 2024-02-01 22:21:06.982000 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_interfaces.cpython-311.pyc
+-rw-r--r--   0        0        0      472 2024-01-23 15:12:07.528662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_reference.cpython-311.pyc
+-rw-r--r--   0        0        0    15878 2024-01-23 15:12:07.532662 eprempy-0.5.5/src/eprempy/datafile/__pycache__/_viewers.cpython-311.pyc
+-rw-r--r--   0        0        0     3038 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_core.py
+-rw-r--r--   0        0        0    13619 2024-02-01 21:56:36.730088 eprempy-0.5.5/src/eprempy/datafile/_interfaces.py
+-rw-r--r--   0        0        0      838 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_reference.py
+-rw-r--r--   0        0        0     8597 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/datafile/_viewers.py
+-rw-r--r--   0        0        0    14024 2024-05-07 18:59:06.063479 eprempy-0.5.5/src/eprempy/eprem.py
+-rw-r--r--   0        0        0    19560 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/etc.py
+-rw-r--r--   0        0        0     6421 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/exceptions.py
+-rw-r--r--   0        0        0     2535 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/interfaces.py
+-rw-r--r--   0        0        0      452 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measurable/__init__.py
+-rw-r--r--   0        0        0     1138 2023-12-18 17:27:18.215239 eprempy-0.5.5/src/eprempy/measurable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1649 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/measured/__init__.py
+-rw-r--r--   0        0        0     3214 2024-01-23 15:12:06.724663 eprempy-0.5.5/src/eprempy/measured/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     6881 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_context.cpython-311.pyc
+-rw-r--r--   0        0        0     1828 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_convert.cpython-311.pyc
+-rw-r--r--   0        0        0     3866 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_factories.cpython-311.pyc
+-rw-r--r--   0        0        0     2022 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_object.cpython-311.pyc
+-rw-r--r--   0        0        0     3798 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_sequence.cpython-311.pyc
+-rw-r--r--   0        0        0     5551 2023-12-18 17:27:18.195239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_types.cpython-311.pyc
+-rw-r--r--   0        0        0     1336 2023-12-18 17:27:18.235239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_units.cpython-311.pyc
+-rw-r--r--   0        0        0     1966 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/measured/__pycache__/_value.cpython-311.pyc
+-rw-r--r--   0        0        0     3554 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_context.py
+-rw-r--r--   0        0        0      843 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_convert.py
+-rw-r--r--   0        0        0     1881 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_factories.py
+-rw-r--r--   0        0        0      872 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_object.py
+-rw-r--r--   0        0        0        0 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_operators.py
+-rw-r--r--   0        0        0     2499 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_sequence.py
+-rw-r--r--   0        0        0     2710 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_types.py
+-rw-r--r--   0        0        0      530 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_units.py
+-rw-r--r--   0        0        0      781 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/measured/_value.py
+-rw-r--r--   0        0        0     4334 2024-01-22 22:28:21.800484 eprempy-0.5.5/src/eprempy/metric/__init__.py
+-rw-r--r--   0        0        0     5988 2024-01-23 15:12:06.728663 eprempy-0.5.5/src/eprempy/metric/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    28262 2024-01-23 15:12:06.736663 eprempy-0.5.5/src/eprempy/metric/__pycache__/_conversions.cpython-311.pyc
+-rw-r--r--   0        0        0    41607 2024-01-17 20:32:10.271816 eprempy-0.5.5/src/eprempy/metric/__pycache__/_defined.cpython-311.pyc
+-rw-r--r--   0        0        0     6425 2023-12-18 17:27:18.187239 eprempy-0.5.5/src/eprempy/metric/__pycache__/_dimensions.cpython-311.pyc
+-rw-r--r--   0        0        0     2176 2024-01-17 20:32:10.275816 eprempy-0.5.5/src/eprempy/metric/__pycache__/_exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0    15038 2024-02-01 22:21:06.218000 eprempy-0.5.5/src/eprempy/metric/__pycache__/_reference.cpython-311.pyc
+-rw-r--r--   0        0        0    23126 2024-01-17 20:32:10.483817 eprempy-0.5.5/src/eprempy/metric/__pycache__/_systems.cpython-311.pyc
+-rw-r--r--   0        0        0     2358 2023-12-18 17:27:18.191239 eprempy-0.5.5/src/eprempy/metric/__pycache__/_types.cpython-311.pyc
+-rw-r--r--   0        0        0    25561 2024-01-17 20:32:10.495817 eprempy-0.5.5/src/eprempy/metric/__pycache__/_units.cpython-311.pyc
+-rw-r--r--   0        0        0    19397 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/metric/_conversions.py
+-rw-r--r--   0        0        0    26244 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_defined.py
+-rw-r--r--   0        0        0     3013 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/metric/_dimensions.py
+-rw-r--r--   0        0        0      804 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_exceptions.py
+-rw-r--r--   0        0        0    20947 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/metric/_reference.py
+-rw-r--r--   0        0        0    13685 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_systems.py
+-rw-r--r--   0        0        0     1011 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/metric/_types.py
+-rw-r--r--   0        0        0    20543 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/metric/_units.py
+-rw-r--r--   0        0        0     1893 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/numeric/__init__.py
+-rw-r--r--   0        0        0     3045 2024-01-23 15:12:06.896663 eprempy-0.5.5/src/eprempy/numeric/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    45019 2024-02-01 22:21:06.398000 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_array.cpython-311.pyc
+-rw-r--r--   0        0        0     6502 2023-12-18 17:27:18.199239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_data.cpython-311.pyc
+-rw-r--r--   0        0        0     4973 2023-12-18 17:27:18.223239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_factory.cpython-311.pyc
+-rw-r--r--   0        0        0     4242 2023-12-18 17:27:18.203239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_implementation.cpython-311.pyc
+-rw-r--r--   0        0        0    39216 2024-02-01 22:21:06.390000 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_index.cpython-311.pyc
+-rw-r--r--   0        0        0    20506 2023-12-18 17:27:18.215239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    12801 2023-12-18 17:27:18.199239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_objects.cpython-311.pyc
+-rw-r--r--   0        0        0    16208 2024-01-17 20:32:10.503817 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_operations.cpython-311.pyc
+-rw-r--r--   0        0        0     8024 2023-12-18 17:27:18.203239 eprempy-0.5.5/src/eprempy/numeric/__pycache__/_operators.cpython-311.pyc
+-rw-r--r--   0        0        0    27098 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/numeric/_array.py
+-rw-r--r--   0        0        0     3999 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_data.py
+-rw-r--r--   0        0        0     2944 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_factory.py
+-rw-r--r--   0        0        0     2105 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_implementation.py
+-rw-r--r--   0        0        0    22263 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/numeric/_index.py
+-rw-r--r--   0        0        0    16116 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_mixins.py
+-rw-r--r--   0        0        0     7169 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_objects.py
+-rw-r--r--   0        0        0    12011 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/numeric/_operations.py
+-rw-r--r--   0        0        0     4363 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/numeric/_operators.py
+-rw-r--r--   0        0        0      637 2023-12-18 17:25:57.415106 eprempy-0.5.5/src/eprempy/observable/__init__.py
+-rw-r--r--   0        0        0     1235 2023-12-18 17:27:18.547240 eprempy-0.5.5/src/eprempy/observable/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    89743 2024-02-01 22:22:10.929996 eprempy-0.5.5/src/eprempy/observable/__pycache__/_interfaces.cpython-311.pyc
+-rw-r--r--   0        0        0    31847 2024-02-01 22:21:06.722000 eprempy-0.5.5/src/eprempy/observable/__pycache__/_objects.cpython-311.pyc
+-rw-r--r--   0        0        0    66067 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/observable/_interfaces.py
+-rw-r--r--   0        0        0    20418 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/observable/_objects.py
+-rw-r--r--   0        0        0     5829 2024-02-16 16:58:53.068415 eprempy-0.5.5/src/eprempy/parameter/__init__.py
+-rw-r--r--   0        0        0     7713 2024-02-16 17:07:35.148203 eprempy-0.5.5/src/eprempy/parameter/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    22264 2024-02-16 17:07:35.148203 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_config.cpython-311.pyc
+-rw-r--r--   0        0        0      174 2024-02-09 16:09:39.704090 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_interface.cpython-311.pyc
+-rw-r--r--   0        0        0    10077 2024-05-24 16:41:42.827676 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_metadata.cpython-311.pyc
+-rw-r--r--   0        0        0     9967 2024-01-26 15:55:06.544039 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_reference.cpython-311.pyc
+-rw-r--r--   0        0        0    14379 2024-02-16 21:45:52.775370 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_runtime.cpython-311.pyc
+-rw-r--r--   0        0        0    28158 2024-02-16 21:45:52.743369 eprempy-0.5.5/src/eprempy/parameter/__pycache__/_src.cpython-311.pyc
+-rw-r--r--   0        0        0    13524 2024-02-09 16:09:08.524083 eprempy-0.5.5/src/eprempy/parameter/__pycache__/default.cpython-311.pyc
+-rw-r--r--   0        0        0    13439 2024-03-27 19:39:17.007480 eprempy-0.5.5/src/eprempy/parameter/__pycache__/reference.cpython-311.pyc
+-rw-r--r--   0        0        0    13237 2024-02-16 16:58:53.068415 eprempy-0.5.5/src/eprempy/parameter/_config.py
+-rw-r--r--   0        0        0    12922 2024-03-27 21:35:17.659905 eprempy-0.5.5/src/eprempy/parameter/_metadata.py
+-rw-r--r--   0        0        0     7762 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/parameter/_runtime.py
+-rw-r--r--   0        0        0    15954 2024-02-16 21:43:35.579405 eprempy-0.5.5/src/eprempy/parameter/_src.py
+-rw-r--r--   0        0        0    20943 2024-03-27 19:22:59.867663 eprempy-0.5.5/src/eprempy/parameter/reference.json
+-rw-r--r--   0        0        0    27683 2024-03-27 19:25:57.511816 eprempy-0.5.5/src/eprempy/parameter/reference.py
+-rw-r--r--   0        0        0      447 2024-03-27 19:22:59.875663 eprempy-0.5.5/src/eprempy/parameter/sources.log
+-rw-r--r--   0        0        0     7210 2024-01-17 20:28:37.607261 eprempy-0.5.5/src/eprempy/paths.py
+-rw-r--r--   0        0        0    18010 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/physical/__init__.py
+-rw-r--r--   0        0        0    23629 2024-01-23 15:12:06.724663 eprempy-0.5.5/src/eprempy/physical/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12627 2024-02-01 22:21:06.414000 eprempy-0.5.5/src/eprempy/physical/__pycache__/_array.cpython-311.pyc
+-rw-r--r--   0        0        0    26899 2024-01-17 20:32:10.583817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axes.cpython-311.pyc
+-rw-r--r--   0        0        0    20617 2024-05-24 17:02:27.395843 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axis.cpython-311.pyc
+-rw-r--r--   0        0        0     4355 2023-12-18 17:27:18.531240 eprempy-0.5.5/src/eprempy/physical/__pycache__/_axis_factories.cpython-311.pyc
+-rw-r--r--   0        0        0      552 2024-01-17 20:32:10.587817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0     8714 2023-12-18 17:27:18.239239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_object.cpython-311.pyc
+-rw-r--r--   0        0        0     9947 2023-12-18 17:27:18.247239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_object_factories.cpython-311.pyc
+-rw-r--r--   0        0        0    42022 2024-02-01 22:21:06.706000 eprempy-0.5.5/src/eprempy/physical/__pycache__/_operations.cpython-311.pyc
+-rw-r--r--   0        0        0     5448 2024-01-17 20:32:10.587817 eprempy-0.5.5/src/eprempy/physical/__pycache__/_scalar.cpython-311.pyc
+-rw-r--r--   0        0        0     4504 2023-12-18 17:27:18.251239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_tensor.cpython-311.pyc
+-rw-r--r--   0        0        0     3431 2023-12-18 17:27:18.243239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_types.cpython-311.pyc
+-rw-r--r--   0        0        0     4116 2023-12-18 17:27:18.251239 eprempy-0.5.5/src/eprempy/physical/__pycache__/_vector.cpython-311.pyc
+-rw-r--r--   0        0        0     6544 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/physical/_array.py
+-rw-r--r--   0        0        0    17721 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_axes.py
+-rw-r--r--   0        0        0    13647 2024-05-24 17:02:24.651820 eprempy-0.5.5/src/eprempy/physical/_axis.py
+-rw-r--r--   0        0        0     2249 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_axis_factories.py
+-rw-r--r--   0        0        0      150 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_exceptions.py
+-rw-r--r--   0        0        0     4163 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_object.py
+-rw-r--r--   0        0        0     5868 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_object_factories.py
+-rw-r--r--   0        0        0    21876 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/physical/_operations.py
+-rw-r--r--   0        0        0     2658 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/physical/_scalar.py
+-rw-r--r--   0        0        0     2030 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_tensor.py
+-rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_types.py
+-rw-r--r--   0        0        0     1696 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/physical/_vector.py
+-rw-r--r--   0        0        0    40811 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/project.py
+-rw-r--r--   0        0        0     4789 2024-05-24 16:51:09.576354 eprempy-0.5.5/src/eprempy/quantity/__init__.py
+-rw-r--r--   0        0        0     6632 2024-05-24 16:53:00.804523 eprempy-0.5.5/src/eprempy/quantity/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1303 2024-01-17 20:32:10.571817 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_exceptions.cpython-311.pyc
+-rw-r--r--   0        0        0    17103 2024-05-24 16:53:00.804523 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_functions.cpython-311.pyc
+-rw-r--r--   0        0        0     4164 2023-12-18 17:27:18.239239 eprempy-0.5.5/src/eprempy/quantity/__pycache__/_measurement.cpython-311.pyc
+-rw-r--r--   0        0        0      400 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/quantity/_exceptions.py
+-rw-r--r--   0        0        0     9972 2024-05-24 16:50:50.316326 eprempy-0.5.5/src/eprempy/quantity/_functions.py
+-rw-r--r--   0        0        0     2093 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/quantity/_measurement.py
+-rw-r--r--   0        0        0     3790 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/real/__init__.py
+-rw-r--r--   0        0        0     8573 2024-01-23 15:12:06.912663 eprempy-0.5.5/src/eprempy/real/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    23275 2024-01-23 15:12:06.916663 eprempy-0.5.5/src/eprempy/real/__pycache__/_array.cpython-311.pyc
+-rw-r--r--   0        0        0    10049 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/real/__pycache__/_objects.cpython-311.pyc
+-rw-r--r--   0        0        0      745 2023-12-18 17:27:18.227239 eprempy-0.5.5/src/eprempy/real/__pycache__/_types.cpython-311.pyc
+-rw-r--r--   0        0        0    11506 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/real/_array.py
+-rw-r--r--   0        0        0     4891 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/real/_objects.py
+-rw-r--r--   0        0        0      707 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/real/_types.py
+-rw-r--r--   0        0        0     5785 2024-01-22 22:28:21.804484 eprempy-0.5.5/src/eprempy/reference.py
+-rw-r--r--   0        0        0     1756 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/symbolic/__init__.py
+-rw-r--r--   0        0        0     3097 2024-01-17 20:32:10.255816 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    21446 2023-12-18 17:27:17.999239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_expression.cpython-311.pyc
+-rw-r--r--   0        0        0    42853 2024-01-24 19:12:48.936383 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_operand.cpython-311.pyc
+-rw-r--r--   0        0        0     3246 2023-12-18 17:27:18.015239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_operator.cpython-311.pyc
+-rw-r--r--   0        0        0    13036 2024-01-17 20:32:10.267816 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_parser.cpython-311.pyc
+-rw-r--r--   0        0        0     6480 2023-12-18 17:27:18.011239 eprempy-0.5.5/src/eprempy/symbolic/__pycache__/_part.cpython-311.pyc
+-rw-r--r--   0        0        0    13984 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_expression.py
+-rw-r--r--   0        0        0    31307 2024-01-24 16:54:00.366890 eprempy-0.5.5/src/eprempy/symbolic/_operand.py
+-rw-r--r--   0        0        0     1689 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_operator.py
+-rw-r--r--   0        0        0     8534 2024-01-17 20:28:37.611261 eprempy-0.5.5/src/eprempy/symbolic/_parser.py
+-rw-r--r--   0        0        0     3018 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/symbolic/_part.py
+-rw-r--r--   0        0        0      647 2023-12-18 17:25:57.419106 eprempy-0.5.5/src/eprempy/typehelp.py
+-rw-r--r--   0        0        0     9023 2024-02-01 21:56:36.734088 eprempy-0.5.5/src/eprempy/universal.py
+-rw-r--r--   0        0        0    11598 1970-01-01 00:00:00.000000 eprempy-0.5.5/PKG-INFO
```

### Comparing `eprempy-0.5.4/LICENSE` & `eprempy-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/README.md` & `eprempy-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/pyproject.toml` & `eprempy-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eprempy"
-version = "0.5.4"
+version = "0.5.5"
 description = "Tools for working with EPREM simulation runs"
 authors = ["Matt Young"]
 license = "BSD 3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
```

### Comparing `eprempy-0.5.4/src/eprempy/__main__.py` & `eprempy-0.5.5/src/eprempy/__main__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/_project_main.py` & `eprempy-0.5.5/src/eprempy/_project_main.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/aliased.py` & `eprempy-0.5.5/src/eprempy/aliased.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/atomic.py` & `eprempy-0.5.5/src/eprempy/atomic.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/base/__init__.py` & `eprempy-0.5.5/src/eprempy/base/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/base/_abcs.py` & `eprempy-0.5.5/src/eprempy/base/_abcs.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/base/_protocols.py` & `eprempy-0.5.5/src/eprempy/base/_protocols.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/base/_types.py` & `eprempy-0.5.5/src/eprempy/base/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/base/mixins.py` & `eprempy-0.5.5/src/eprempy/base/mixins.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/cli.py` & `eprempy-0.5.5/src/eprempy/cli.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/container.py` & `eprempy-0.5.5/src/eprempy/container.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/datafile/__init__.py` & `eprempy-0.5.5/src/eprempy/datafile/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/datafile/_core.py` & `eprempy-0.5.5/src/eprempy/datafile/_core.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/datafile/_interfaces.py` & `eprempy-0.5.5/src/eprempy/datafile/_interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/datafile/_reference.py` & `eprempy-0.5.5/src/eprempy/datafile/_reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/datafile/_viewers.py` & `eprempy-0.5.5/src/eprempy/datafile/_viewers.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/eprem.py` & `eprempy-0.5.5/src/eprempy/eprem.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/etc.py` & `eprempy-0.5.5/src/eprempy/etc.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/exceptions.py` & `eprempy-0.5.5/src/eprempy/exceptions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/interfaces.py` & `eprempy-0.5.5/src/eprempy/interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/__init__.py` & `eprempy-0.5.5/src/eprempy/measured/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_context.py` & `eprempy-0.5.5/src/eprempy/measured/_context.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_convert.py` & `eprempy-0.5.5/src/eprempy/measured/_convert.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_factories.py` & `eprempy-0.5.5/src/eprempy/measured/_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_object.py` & `eprempy-0.5.5/src/eprempy/measured/_object.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_sequence.py` & `eprempy-0.5.5/src/eprempy/measured/_sequence.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_types.py` & `eprempy-0.5.5/src/eprempy/measured/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_units.py` & `eprempy-0.5.5/src/eprempy/measured/_units.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/measured/_value.py` & `eprempy-0.5.5/src/eprempy/measured/_value.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/__init__.py` & `eprempy-0.5.5/src/eprempy/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_conversions.py` & `eprempy-0.5.5/src/eprempy/metric/_conversions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_defined.py` & `eprempy-0.5.5/src/eprempy/metric/_defined.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_dimensions.py` & `eprempy-0.5.5/src/eprempy/metric/_dimensions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_exceptions.py` & `eprempy-0.5.5/src/eprempy/metric/_exceptions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_reference.py` & `eprempy-0.5.5/src/eprempy/metric/_reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_systems.py` & `eprempy-0.5.5/src/eprempy/metric/_systems.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_types.py` & `eprempy-0.5.5/src/eprempy/metric/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/metric/_units.py` & `eprempy-0.5.5/src/eprempy/metric/_units.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/__init__.py` & `eprempy-0.5.5/src/eprempy/numeric/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_array.py` & `eprempy-0.5.5/src/eprempy/numeric/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_data.py` & `eprempy-0.5.5/src/eprempy/numeric/_data.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_factory.py` & `eprempy-0.5.5/src/eprempy/numeric/_factory.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_implementation.py` & `eprempy-0.5.5/src/eprempy/numeric/_implementation.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_index.py` & `eprempy-0.5.5/src/eprempy/numeric/_index.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_mixins.py` & `eprempy-0.5.5/src/eprempy/numeric/_mixins.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_objects.py` & `eprempy-0.5.5/src/eprempy/numeric/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_operations.py` & `eprempy-0.5.5/src/eprempy/numeric/_operations.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/numeric/_operators.py` & `eprempy-0.5.5/src/eprempy/numeric/_operators.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/observable/__init__.py` & `eprempy-0.5.5/src/eprempy/observable/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/observable/_interfaces.py` & `eprempy-0.5.5/src/eprempy/observable/_interfaces.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/observable/_objects.py` & `eprempy-0.5.5/src/eprempy/observable/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/__init__.py` & `eprempy-0.5.5/src/eprempy/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/_config.py` & `eprempy-0.5.5/src/eprempy/parameter/_config.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/_metadata.py` & `eprempy-0.5.5/src/eprempy/parameter/_metadata.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/_runtime.py` & `eprempy-0.5.5/src/eprempy/parameter/_runtime.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/_src.py` & `eprempy-0.5.5/src/eprempy/parameter/_src.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/reference.json` & `eprempy-0.5.5/src/eprempy/parameter/reference.json`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/parameter/reference.py` & `eprempy-0.5.5/src/eprempy/parameter/reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/paths.py` & `eprempy-0.5.5/src/eprempy/paths.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/__init__.py` & `eprempy-0.5.5/src/eprempy/physical/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_array.py` & `eprempy-0.5.5/src/eprempy/physical/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_axes.py` & `eprempy-0.5.5/src/eprempy/physical/_axes.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_axis.py` & `eprempy-0.5.5/src/eprempy/physical/_axis.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,14 +322,16 @@
 
     def _measure(self, targets: typing.Sequence):
         """Create a measured sequence, if possible."""
         if len(targets) == 1:
             target = targets[0]
             if isinstance(target, quantity.Measurement):
                 return target
+            if isinstance(target, measured.Object):
+                return quantity.measure(target)
             if quantity.ismeasurable(target):
                 return quantity.measure(target)
         with contextlib.suppress(quantity.ParsingTypeError):
             return quantity.measure(targets)
 
     def __eq__(self, other):
         if isinstance(other, Coordinates):
```

### Comparing `eprempy-0.5.4/src/eprempy/physical/_axis_factories.py` & `eprempy-0.5.5/src/eprempy/physical/_axis_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_object.py` & `eprempy-0.5.5/src/eprempy/physical/_object.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_object_factories.py` & `eprempy-0.5.5/src/eprempy/physical/_object_factories.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_operations.py` & `eprempy-0.5.5/src/eprempy/physical/_operations.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_scalar.py` & `eprempy-0.5.5/src/eprempy/physical/_scalar.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_tensor.py` & `eprempy-0.5.5/src/eprempy/physical/_tensor.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_types.py` & `eprempy-0.5.5/src/eprempy/physical/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/physical/_vector.py` & `eprempy-0.5.5/src/eprempy/physical/_vector.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/project.py` & `eprempy-0.5.5/src/eprempy/project.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/quantity/__init__.py` & `eprempy-0.5.5/src/eprempy/quantity/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/quantity/_functions.py` & `eprempy-0.5.5/src/eprempy/quantity/_functions.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/quantity/_measurement.py` & `eprempy-0.5.5/src/eprempy/quantity/_measurement.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/real/__init__.py` & `eprempy-0.5.5/src/eprempy/real/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/real/_array.py` & `eprempy-0.5.5/src/eprempy/real/_array.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/real/_objects.py` & `eprempy-0.5.5/src/eprempy/real/_objects.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/real/_types.py` & `eprempy-0.5.5/src/eprempy/real/_types.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/reference.py` & `eprempy-0.5.5/src/eprempy/reference.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/__init__.py` & `eprempy-0.5.5/src/eprempy/symbolic/__init__.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/_expression.py` & `eprempy-0.5.5/src/eprempy/symbolic/_expression.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/_operand.py` & `eprempy-0.5.5/src/eprempy/symbolic/_operand.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/_operator.py` & `eprempy-0.5.5/src/eprempy/symbolic/_operator.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/_parser.py` & `eprempy-0.5.5/src/eprempy/symbolic/_parser.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/symbolic/_part.py` & `eprempy-0.5.5/src/eprempy/symbolic/_part.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/typehelp.py` & `eprempy-0.5.5/src/eprempy/typehelp.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/src/eprempy/universal.py` & `eprempy-0.5.5/src/eprempy/universal.py`

 * *Files identical despite different names*

### Comparing `eprempy-0.5.4/PKG-INFO` & `eprempy-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprempy
-Version: 0.5.4
+Version: 0.5.5
 Summary: Tools for working with EPREM simulation runs
 License: BSD 3-Clause
 Author: Matt Young
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

