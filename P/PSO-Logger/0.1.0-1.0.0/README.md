# Comparing `tmp/pso_logger-0.1.0.tar.gz` & `tmp/pso_logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pso_logger-0.1.0.tar", max compression
+gzip compressed data, was "pso_logger-1.0.0.tar", max compression
```

## Comparing `pso_logger-0.1.0.tar` & `pso_logger-1.0.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      302 2024-05-27 13:22:13.099552 pso_logger-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-27 13:22:48.330509 pso_logger-0.1.0/src/pso_logger/__init__.py
--rw-r--r--   0        0        0     2220 2024-05-27 13:23:19.270708 pso_logger-0.1.0/src/pso_logger/pso_logging.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 pso_logger-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      302 2024-05-28 11:49:47.723937 pso_logger-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-27 13:22:48.330509 pso_logger-1.0.0/src/pso_logger/__init__.py
+-rw-r--r--   0        0        0     1550 2024-05-28 11:48:15.220161 pso_logger-1.0.0/src/pso_logger/pso_logging.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 pso_logger-1.0.0/PKG-INFO
```

