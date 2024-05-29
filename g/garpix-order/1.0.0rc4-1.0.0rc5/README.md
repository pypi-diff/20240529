# Comparing `tmp/garpix_order-1.0.0rc4.tar.gz` & `tmp/garpix_order-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_order-1.0.0rc4.tar", last modified: Tue May  7 10:32:24 2024, max compression
+gzip compressed data, was "garpix_order-1.0.0rc5.tar", last modified: Wed May 29 09:59:28 2024, max compression
```

## Comparing `garpix_order-1.0.0rc4.tar` & `garpix_order-1.0.0rc5.tar`

### file list

```diff
@@ -1,72 +1,107 @@
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.649078 garpix_order-1.0.0rc4/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       64 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/MANIFEST.in
--rw-r--r--   0 crusat    (1000) crusat    (1000)      638 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/PKG-INFO
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       64 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/MANIFEST.in
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      462 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/README.rst
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       59 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/__init__.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/admin/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       77 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/home_page.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      207 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/admin/recurring.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      184 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/apps.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      531 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/exceptions.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/logging/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       23 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/__init__.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.637078 garpix_order-1.0.0rc4/garpix_order/logging/filters/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       60 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/filters/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      365 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/logging/filters/payment_auth_data_filter.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/migrations/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     6932 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0001_initial.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     2607 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0002_auto_20230703_1624.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      803 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/0003_robokassainvoice.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/migrations/__init__.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/models/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      257 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      468 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/config.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     4210 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/order.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      789 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/order_item.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     5279 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payment.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/models/payments/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      206 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      241 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/bank_card.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      207 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/cash.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1338 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/cloudpayments.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1874 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/recurring.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1589 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/robokassa.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1612 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/models/payments/sber.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      100 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/pyproject.toml
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.641078 garpix_order-1.0.0rc4/garpix_order/serializers/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       77 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/serializers/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      419 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/serializers/robokassa.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/services/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     3577 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/robokassa.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     9124 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/services/sber.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1154 2024-05-07 10:28:21.000000 garpix_order-1.0.0rc4/garpix_order/setup.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     7708 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/tests.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/types/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       20 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/types/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1285 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/types/sber.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      515 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/urls.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      219 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/utils.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       37 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/__init__.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     5754 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1239 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/default_view.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       98 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/fail.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       97 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/pay.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)      710 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/payment_data.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order/views/robokassa/
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       35 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/robokassa/__init__.py
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1553 2024-05-07 10:04:32.000000 garpix_order-1.0.0rc4/garpix_order/views/robokassa/payment.py
-drwxrwxr-x   0 crusat    (1000) crusat    (1000)        0 2024-05-07 10:32:24.645078 garpix_order-1.0.0rc4/garpix_order.egg-info/
--rw-r--r--   0 crusat    (1000) crusat    (1000)      638 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/PKG-INFO
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1884 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/SOURCES.txt
--rw-rw-r--   0 crusat    (1000) crusat    (1000)        1 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/dependency_links.txt
--rw-rw-r--   0 crusat    (1000) crusat    (1000)        1 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/not-zip-safe
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       38 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/requires.txt
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       13 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/garpix_order.egg-info/top_level.txt
--rw-rw-r--   0 crusat    (1000) crusat    (1000)       38 2024-05-07 10:32:24.649078 garpix_order-1.0.0rc4/setup.cfg
--rw-rw-r--   0 crusat    (1000) crusat    (1000)     1154 2024-05-07 10:32:24.000000 garpix_order-1.0.0rc4/setup.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.301928 garpix_order-1.0.0rc5/
+-rw-r--r--   0 anatoly    (501) staff       (20)       64 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/MANIFEST.in
+-rw-r--r--   0 anatoly    (501) staff       (20)      527 2024-05-29 09:59:28.301785 garpix_order-1.0.0rc5/PKG-INFO
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.292082 garpix_order-1.0.0rc5/garpix_order/
+-rw-r--r--   0 anatoly    (501) staff       (20)       64 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/MANIFEST.in
+-rw-r--r--   0 anatoly    (501) staff       (20)      462 2024-05-29 09:56:57.000000 garpix_order-1.0.0rc5/garpix_order/README.md
+-rw-r--r--   0 anatoly    (501) staff       (20)      462 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/README.rst
+-rw-r--r--   0 anatoly    (501) staff       (20)       59 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.293333 garpix_order-1.0.0rc5/garpix_order/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      262 2024-05-29 09:56:26.000000 garpix_order-1.0.0rc5/garpix_order/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      665 2024-05-29 09:56:26.000000 garpix_order-1.0.0rc5/garpix_order/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1010 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      753 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/__pycache__/utils.cpython-311.pyc
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.293689 garpix_order-1.0.0rc5/garpix_order/admin/
+-rw-r--r--   0 anatoly    (501) staff       (20)        0 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/admin/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.293826 garpix_order-1.0.0rc5/garpix_order/admin/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      208 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/admin/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)       77 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/admin/home_page.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      207 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/admin/recurring.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      184 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/apps.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      712 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/exceptions.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.293949 garpix_order-1.0.0rc5/garpix_order/logging/
+-rw-r--r--   0 anatoly    (501) staff       (20)       23 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/logging/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.294195 garpix_order-1.0.0rc5/garpix_order/logging/filters/
+-rw-r--r--   0 anatoly    (501) staff       (20)       60 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/logging/filters/__init__.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      365 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/logging/filters/payment_auth_data_filter.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.294951 garpix_order-1.0.0rc5/garpix_order/migrations/
+-rw-r--r--   0 anatoly    (501) staff       (20)     6932 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/migrations/0001_initial.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     2607 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/migrations/0002_auto_20230703_1624.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      803 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/migrations/0003_robokassainvoice.py
+-rw-r--r--   0 anatoly    (501) staff       (20)        0 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/migrations/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.295672 garpix_order-1.0.0rc5/garpix_order/models/
+-rw-r--r--   0 anatoly    (501) staff       (20)      257 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.296426 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      660 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1134 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     7341 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/order.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1934 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/order_item.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     8583 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/__pycache__/payment.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      468 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/config.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     4210 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/order.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      789 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/order_item.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     5279 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payment.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.297306 garpix_order-1.0.0rc5/garpix_order/models/payments/
+-rw-r--r--   0 anatoly    (501) staff       (20)      206 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.298286 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      567 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      909 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/bank_card.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      866 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/cash.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     2196 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/cloudpayments.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     3763 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/recurring.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     3565 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/robokassa.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     2651 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/__pycache__/sber.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      241 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/bank_card.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      207 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/cash.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1338 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/cloudpayments.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1874 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/recurring.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1589 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/robokassa.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1612 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/models/payments/sber.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      100 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/pyproject.toml
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.298894 garpix_order-1.0.0rc5/garpix_order/serializers/
+-rw-r--r--   0 anatoly    (501) staff       (20)       77 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/serializers/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.299169 garpix_order-1.0.0rc5/garpix_order/serializers/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      330 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/serializers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1342 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/serializers/__pycache__/robokassa.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)      419 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/serializers/robokassa.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.299502 garpix_order-1.0.0rc5/garpix_order/services/
+-rw-r--r--   0 anatoly    (501) staff       (20)        0 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/services/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.299765 garpix_order-1.0.0rc5/garpix_order/services/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      211 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/services/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     6621 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/services/__pycache__/robokassa.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     3577 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/services/robokassa.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     9372 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/services/sber.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1284 2024-05-29 09:59:07.000000 garpix_order-1.0.0rc5/garpix_order/setup.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     7708 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/tests.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.300054 garpix_order-1.0.0rc5/garpix_order/types/
+-rw-r--r--   0 anatoly    (501) staff       (20)       20 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/types/__init__.py
+-rw-r--r--   0 anatoly    (501) staff       (20)     1285 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/types/sber.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      515 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/urls.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      219 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/utils.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.300188 garpix_order-1.0.0rc5/garpix_order/views/
+-rw-r--r--   0 anatoly    (501) staff       (20)       37 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.300323 garpix_order-1.0.0rc5/garpix_order/views/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      269 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/views/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.300986 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/
+-rw-r--r--   0 anatoly    (501) staff       (20)     5754 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.301105 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)     9070 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1673 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/default_view.py
+-rw-r--r--   0 anatoly    (501) staff       (20)       98 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/fail.py
+-rw-r--r--   0 anatoly    (501) staff       (20)       97 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/pay.py
+-rw-r--r--   0 anatoly    (501) staff       (20)      710 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/payment_data.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.301354 garpix_order-1.0.0rc5/garpix_order/views/robokassa/
+-rw-r--r--   0 anatoly    (501) staff       (20)       35 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/robokassa/__init__.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.301596 garpix_order-1.0.0rc5/garpix_order/views/robokassa/__pycache__/
+-rw-r--r--   0 anatoly    (501) staff       (20)      277 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/views/robokassa/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     3240 2024-05-29 09:56:28.000000 garpix_order-1.0.0rc5/garpix_order/views/robokassa/__pycache__/payment.cpython-311.pyc
+-rw-r--r--   0 anatoly    (501) staff       (20)     1553 2024-05-29 09:46:53.000000 garpix_order-1.0.0rc5/garpix_order/views/robokassa/payment.py
+drwxr-xr-x   0 anatoly    (501) staff       (20)        0 2024-05-29 09:59:28.292808 garpix_order-1.0.0rc5/garpix_order.egg-info/
+-rw-r--r--   0 anatoly    (501) staff       (20)      527 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/PKG-INFO
+-rw-r--r--   0 anatoly    (501) staff       (20)     3396 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/SOURCES.txt
+-rw-r--r--   0 anatoly    (501) staff       (20)        1 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/dependency_links.txt
+-rw-r--r--   0 anatoly    (501) staff       (20)        1 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/not-zip-safe
+-rw-r--r--   0 anatoly    (501) staff       (20)       56 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/requires.txt
+-rw-r--r--   0 anatoly    (501) staff       (20)       13 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/garpix_order.egg-info/top_level.txt
+-rw-r--r--   0 anatoly    (501) staff       (20)       38 2024-05-29 09:59:28.301974 garpix_order-1.0.0rc5/setup.cfg
+-rw-r--r--   0 anatoly    (501) staff       (20)     1284 2024-05-29 09:59:28.000000 garpix_order-1.0.0rc5/setup.py
```

### Comparing `garpix_order-1.0.0rc4/garpix_order/exceptions.py` & `garpix_order-1.0.0rc5/garpix_order/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 class BasePaymentException(Exception):
     pass
 
 
-class UndefinedModelForSberPaymentException(BasePaymentException):
+class UndefinedModelPaymentException(BasePaymentException):
     def __init__(self, message="Не задана модель-наследник BaseSberPayment в settings.py."):
         super().__init__(message)
 
 
-class InvalidModelForSberPaymentException(BasePaymentException):
+class InvalidModelPaymentException(BasePaymentException):
     def __init__(self, message="Заданная модель для платежей Сбера не является наследником BaseSberPayment."):
         super().__init__(message)
+
+
+class InvalidOrderStatusPaymentException(BasePaymentException):
+    def __init__(self, message="Неподдерживаемый статус заказа."):
+        super().__init__(message)
```

### Comparing `garpix_order-1.0.0rc4/garpix_order/migrations/0001_initial.py` & `garpix_order-1.0.0rc5/garpix_order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/migrations/0002_auto_20230703_1624.py` & `garpix_order-1.0.0rc5/garpix_order/migrations/0002_auto_20230703_1624.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/migrations/0003_robokassainvoice.py` & `garpix_order-1.0.0rc5/garpix_order/migrations/0003_robokassainvoice.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/order.py` & `garpix_order-1.0.0rc5/garpix_order/models/order.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/order_item.py` & `garpix_order-1.0.0rc5/garpix_order/models/order_item.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/payment.py` & `garpix_order-1.0.0rc5/garpix_order/models/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/payments/cloudpayments.py` & `garpix_order-1.0.0rc5/garpix_order/models/payments/cloudpayments.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/payments/recurring.py` & `garpix_order-1.0.0rc5/garpix_order/models/payments/recurring.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/payments/robokassa.py` & `garpix_order-1.0.0rc5/garpix_order/models/payments/robokassa.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/models/payments/sber.py` & `garpix_order-1.0.0rc5/garpix_order/models/payments/sber.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/services/robokassa.py` & `garpix_order-1.0.0rc5/garpix_order/services/robokassa.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/services/sber.py` & `garpix_order-1.0.0rc5/garpix_order/services/sber.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from rest_framework.response import Response
 from rest_framework.status import HTTP_200_OK, HTTP_400_BAD_REQUEST
 
 from ..models import BaseOrder, BasePayment, SberPaymentStatus, AbstractSberPayment
 from ..types.sber import (
     CreatePaymentData, GetPaymentData, PaymentCreationData
 )
-from ..exceptions import UndefinedModelForSberPaymentException, InvalidModelForSberPaymentException
+from ..exceptions import (
+    UndefinedModelPaymentException, InvalidModelPaymentException, InvalidOrderStatusPaymentException
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 # Sber REST Docs - https://securecardpayment.ru/wiki/doku.php/integration:api:rest:start
 
@@ -38,20 +40,20 @@
     def __init__(self) -> None:
         super().__init__()
 
     def get_payment_model(self):
         payment_model_path = getattr(settings, 'SBER_PAYMENT_MODEL', None)
 
         if payment_model_path is None:
-            raise UndefinedModelForSberPaymentException
+            raise UndefinedModelPaymentException
 
         payment_model = import_string(payment_model_path)
 
         if not issubclass(payment_model, AbstractSberPayment):
-            raise InvalidModelForSberPaymentException
+            raise InvalidModelPaymentException
 
         return payment_model
 
     def _make_params_for_create_payment(self, order: BaseOrder, **kwargs) -> CreatePaymentData:
         """
         Возвращает params для запроса при создании платежа.
         """
@@ -76,24 +78,28 @@
             language='ru',
         )
 
     def _change_payment_status(self, payment: BasePayment, order_status: int) -> None:
         """
         Изменяет статус модели SberPayment в зависимости от полученного от Сбера статуса.
         """
-        if order_status == SberPaymentStatus.WAITING_FOR_CAPTURE:
+        if order_status == SberPaymentStatus.PENDING:
+            payment.pending()
+        elif order_status == SberPaymentStatus.WAITING_FOR_CAPTURE:
             payment.waiting_for_capture()
         elif order_status == SberPaymentStatus.FULL_PAID:
             payment.succeeded()
         elif order_status == SberPaymentStatus.CANCELLED:
             payment.canceled()
         elif order_status == SberPaymentStatus.REFUNDED:
             payment.refunded()
         elif order_status == SberPaymentStatus.DECLINED:
             payment.failed()
+        else:
+            raise InvalidOrderStatusPaymentException
 
         payment.save()
 
     def _compute_my_checksum(self, secret_key: bytes, callback_data: str) -> str:
         """
         Вычисляет чексумму из данных полученных в callback-уведомлении.
         """
@@ -116,15 +122,16 @@
 
     def _request(self, url: str, params: Type[TypedDict]) -> dict:
         """
         Отправляет GET-запрос и возвращает полученные данные в виде словаря.
         Логирует url запроса и ошибку в случае возникновения.
         """
         try:
-            response = requests.get(url=url, params=params, timeout=self.TIMEOUT)
+            cert_path = settings.SBER.get('cert_path', None)
+            response = requests.get(url=url, params=params, timeout=self.TIMEOUT, verify=cert_path)
             logger.info(f'Request URL: {response.request.url}')
             response.raise_for_status()
             return json.loads(response.content)
         except RequestException as e:
             logger.error(f'Error processing request: {e}')
             raise e
```

### Comparing `garpix_order-1.0.0rc4/garpix_order/setup.py` & `garpix_order-1.0.0rc5/garpix_order/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
-from os import path
-#from m2r import convert
-from django.conf import settings
+# from os import path
+# from m2r import convert
+# from django.conf import settings
 
+# here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
-#with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
-#    long_description = convert(f.read())
+
+# with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
+#     long_description = convert(f.read())
+
+# with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+#     long_description = f.read()
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc4',
+    version='1.0.0-rc5',
     description='',
-#    long_description=long_description,
-    long_description='https://github.com/garpixcms/garpix_order',
+    long_description='',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -29,9 +33,10 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
+        'django-fsm == 3.0.0',
     ],
-)
+)
```

### Comparing `garpix_order-1.0.0rc4/garpix_order/tests.py` & `garpix_order-1.0.0rc5/garpix_order/tests.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/types/sber.py` & `garpix_order-1.0.0rc5/garpix_order/types/sber.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/urls.py` & `garpix_order-1.0.0rc5/garpix_order/urls.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/__init__.py` & `garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/views/cloudpayments/payment_data.py` & `garpix_order-1.0.0rc5/garpix_order/views/cloudpayments/payment_data.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/garpix_order/views/robokassa/payment.py` & `garpix_order-1.0.0rc5/garpix_order/views/robokassa/payment.py`

 * *Files identical despite different names*

### Comparing `garpix_order-1.0.0rc4/setup.py` & `garpix_order-1.0.0rc5/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from setuptools import setup, find_packages
-from os import path
-#from m2r import convert
-from django.conf import settings
+# from os import path
+# from m2r import convert
+# from django.conf import settings
 
+# here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
-#with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
-#    long_description = convert(f.read())
+
+# with open(path.join(settings.BASE_DIR, '..', 'README.md'), encoding='utf-8') as f:
+#     long_description = convert(f.read())
+
+# with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+#     long_description = f.read()
 
 setup(
     name='garpix_order',
-    version='1.0.0-rc4',
+    version='1.0.0-rc5',
     description='',
-#    long_description=long_description,
-    long_description='https://github.com/garpixcms/garpix_order',
+    long_description='',
     url='https://github.com/garpixcms/garpix_order',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
     packages=find_packages(exclude=['testproject', 'testproject.*']),
     classifiers=[
         'Development Status :: 4 - Beta',
@@ -29,9 +33,10 @@
         'Programming Language :: Python :: 3.8',
     ],
     include_package_data=True,
     zip_safe=False,
     install_requires=[
         'Django >= 1.11',
         'djangorestframework >= 3.8',
+        'django-fsm == 3.0.0',
     ],
-)
+)
```

