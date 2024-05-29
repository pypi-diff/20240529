# Comparing `tmp/lessweb-1.3.0.tar.gz` & `tmp/lessweb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.3.0.tar", last modified: Wed May 15 03:12:47 2024, max compression
+gzip compressed data, was "lessweb-1.4.0.tar", last modified: Wed May 29 03:46:02 2024, max compression
```

## Comparing `lessweb-1.3.0.tar` & `lessweb-1.4.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.165947 lessweb-1.3.0/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.156158 lessweb-1.3.0/.github/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.158430 lessweb-1.3.0/.github/workflows/
--rw-r--r--   0 zhangji    (502) staff       (20)     1014 2024-04-12 12:13:03.000000 lessweb-1.3.0/.github/workflows/python-package.yml
--rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.3.0/.gitignore
--rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.3.0/LICENSE.txt
--rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-15 03:12:47.165722 lessweb-1.3.0/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.3.0/README.md
--rw-r--r--   0 zhangji    (502) staff       (20)      797 2024-05-15 03:11:45.000000 lessweb-1.3.0/changelog.md
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.156903 lessweb-1.3.0/examples/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.158684 lessweb-1.3.0/examples/100_hello_world/
--rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159365 lessweb-1.3.0/examples/100_hello_world_config/
--rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world_config/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/100_hello_world_config/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159748 lessweb-1.3.0/examples/101_handle_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/101_handle_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.159988 lessweb-1.3.0/examples/102_response/
--rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/102_response/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160116 lessweb-1.3.0/examples/103_get_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/103_get_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160371 lessweb-1.3.0/examples/205_mysql_crud/
--rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.160581 lessweb-1.3.0/examples/205_mysql_crud/myapp/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/__init__.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161035 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
--rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
--rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
--rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/myapp/mapper.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161167 lessweb-1.3.0/examples/205_mysql_crud/schema/
--rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/205_mysql_crud/schema/pet.sql
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161317 lessweb-1.3.0/examples/302_cookie/
--rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/302_cookie/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161563 lessweb-1.3.0/examples/303_middleware/
--rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/303_middleware/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.161743 lessweb-1.3.0/examples/304_websocket/
--rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/304_websocket/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.162064 lessweb-1.3.0/examples/305_schedule_task/
--rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.3.0/examples/305_schedule_task/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.162795 lessweb-1.3.0/lessweb/
--rw-r--r--   0 zhangji    (502) staff       (20)      202 2024-04-09 15:15:43.000000 lessweb-1.3.0/lessweb/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)    17522 2024-04-18 15:19:24.000000 lessweb-1.3.0/lessweb/bridge.py
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.3.0/lessweb/py.typed
--rw-r--r--   0 zhangji    (502) staff       (20)    11750 2024-04-11 08:10:34.000000 lessweb-1.3.0/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.164735 lessweb-1.3.0/lessweb.egg-info/
--rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1209 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (502) staff       (20)      137 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-05-15 03:12:47.000000 lessweb-1.3.0/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.3.0/mypy.ini
--rw-r--r--   0 zhangji    (502) staff       (20)      724 2024-04-12 14:18:18.000000 lessweb-1.3.0/pyproject.toml
--rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-05-15 03:12:47.165992 lessweb-1.3.0/setup.cfg
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.163868 lessweb-1.3.0/tests/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.3.0/tests/__init__.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-15 03:12:47.164390 lessweb-1.3.0/tests/e2e/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-04-11 09:53:36.000000 lessweb-1.3.0/tests/e2e/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)     1708 2024-04-12 13:07:13.000000 lessweb-1.3.0/tests/e2e/test_request_stack.py
--rw-r--r--   0 zhangji    (502) staff       (20)      453 2024-04-12 12:12:38.000000 lessweb-1.3.0/tests/test_bridge.py
--rw-r--r--   0 zhangji    (502) staff       (20)     6075 2024-04-10 06:59:02.000000 lessweb-1.3.0/tests/test_typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.025258 lessweb-1.4.0/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.013540 lessweb-1.4.0/.github/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.016121 lessweb-1.4.0/.github/workflows/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1014 2024-04-12 12:13:03.000000 lessweb-1.4.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.4.0/.gitignore
+-rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.4.0/LICENSE.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-29 03:46:02.025020 lessweb-1.4.0/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.4.0/README.md
+-rw-r--r--   0 zhangji    (502) staff       (20)      934 2024-05-29 03:41:52.000000 lessweb-1.4.0/changelog.md
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.014350 lessweb-1.4.0/examples/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.016351 lessweb-1.4.0/examples/100_hello_world/
+-rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/100_hello_world/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.017012 lessweb-1.4.0/examples/100_hello_world_config/
+-rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/100_hello_world_config/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/100_hello_world_config/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.017383 lessweb-1.4.0/examples/101_handle_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/101_handle_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.017580 lessweb-1.4.0/examples/102_response/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/102_response/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.017770 lessweb-1.4.0/examples/103_get_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/103_get_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.018271 lessweb-1.4.0/examples/205_mysql_crud/
+-rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.018481 lessweb-1.4.0/examples/205_mysql_crud/myapp/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.018996 lessweb-1.4.0/examples/205_mysql_crud/myapp/endpoint/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/myapp/mapper.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.019132 lessweb-1.4.0/examples/205_mysql_crud/schema/
+-rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/205_mysql_crud/schema/pet.sql
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.019255 lessweb-1.4.0/examples/302_cookie/
+-rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/302_cookie/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.019598 lessweb-1.4.0/examples/303_middleware/
+-rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/303_middleware/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.019770 lessweb-1.4.0/examples/304_websocket/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/304_websocket/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.020147 lessweb-1.4.0/examples/305_schedule_task/
+-rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.4.0/examples/305_schedule_task/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.020984 lessweb-1.4.0/lessweb/
+-rw-r--r--   0 zhangji    (502) staff       (20)      202 2024-04-09 15:15:43.000000 lessweb-1.4.0/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)    17562 2024-05-29 03:35:05.000000 lessweb-1.4.0/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.4.0/lessweb/py.typed
+-rw-r--r--   0 zhangji    (502) staff       (20)    11832 2024-05-29 03:22:10.000000 lessweb-1.4.0/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.023911 lessweb-1.4.0/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (502) staff       (20)     2479 2024-05-29 03:46:01.000000 lessweb-1.4.0/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1209 2024-05-29 03:46:02.000000 lessweb-1.4.0/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-05-29 03:46:01.000000 lessweb-1.4.0/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)      137 2024-05-29 03:46:01.000000 lessweb-1.4.0/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-05-29 03:46:01.000000 lessweb-1.4.0/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.4.0/mypy.ini
+-rw-r--r--   0 zhangji    (502) staff       (20)      724 2024-05-29 03:38:37.000000 lessweb-1.4.0/pyproject.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-05-29 03:46:02.025380 lessweb-1.4.0/setup.cfg
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.022963 lessweb-1.4.0/tests/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.4.0/tests/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-05-29 03:46:02.023356 lessweb-1.4.0/tests/e2e/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-04-11 09:53:36.000000 lessweb-1.4.0/tests/e2e/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1708 2024-04-12 13:07:13.000000 lessweb-1.4.0/tests/e2e/test_request_stack.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      453 2024-04-12 12:12:38.000000 lessweb-1.4.0/tests/test_bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     6313 2024-05-29 03:23:56.000000 lessweb-1.4.0/tests/test_typecast.py
```

### Comparing `lessweb-1.3.0/.github/workflows/python-package.yml` & `lessweb-1.4.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/.gitignore` & `lessweb-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/LICENSE.txt` & `lessweb-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/PKG-INFO` & `lessweb-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `lessweb-1.3.0/README.md` & `lessweb-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/changelog.md` & `lessweb-1.4.0/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## version 1.4.0
+1. Feature: support data type UUID for the request parameters.
+2. Feature: optimize endpoint name compatibility check.
+
 ## version 1.3.0
 1. Deprecated: `getdoc()`;
 2. Feature: support app['lessweb.routes'];
 3. Feature: support multiple positional-only parameters;
 4. Feature: add e2e test (new tests/e2e/ dir);
 5. Feature: when incorrectly used, raise TypeError as the standard specification;
 6. Feature: add autopep8 linter;
```

### Comparing `lessweb-1.3.0/examples/101_handle_request/index.py` & `lessweb-1.4.0/examples/101_handle_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/102_response/index.py` & `lessweb-1.4.0/examples/102_response/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/103_get_request/index.py` & `lessweb-1.4.0/examples/103_get_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/205_mysql_crud/myapp/mapper.py` & `lessweb-1.4.0/examples/205_mysql_crud/myapp/mapper.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/302_cookie/index.py` & `lessweb-1.4.0/examples/302_cookie/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/303_middleware/index.py` & `lessweb-1.4.0/examples/303_middleware/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/304_websocket/index.py` & `lessweb-1.4.0/examples/304_websocket/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/examples/305_schedule_task/index.py` & `lessweb-1.4.0/examples/305_schedule_task/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/lessweb/bridge.py` & `lessweb-1.4.0/lessweb/bridge.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,16 +325,17 @@
 def assert_endpoint_name_compatible(sp_endpoint: ENDPOINT_TYPE, method: str, path: str) -> None:
     """
     限制endpoint函数名必须字面上包含method+path。
     作用：1.避免无谓的思考;2.杜绝在endpoint上滥用修饰器。
 
     :raise: NameError
     """
+    path = re.sub(r':.*?\}', '}', path.lower())
     method_path_slug = f'{method.lower()}_' + \
-        '_'.join(re.findall('[a-z0-9]+', path.lower()))
+        '_'.join(re.findall('[a-z0-9]+', path))
     if not contains_sub_string(sp_endpoint.__name__,  method_path_slug):
         raise NameError(
             f'endpoint name "{sp_endpoint.__name__}" should contain "{method_path_slug}" to compatible with [{method} {path}]')
 
 
 def rest_mapping(method: str, paths: list) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
```

### Comparing `lessweb-1.3.0/lessweb/typecast.py` & `lessweb-1.4.0/lessweb/typecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum
 import inspect
 import json
 import re
 import sys
 from typing import (Any, Dict, List, Literal, NewType, Type, Union,
                     get_type_hints)
+from uuid import UUID
 
 import typing_inspect
 
 
 class TypeCastError(Exception):
     pass
 
@@ -169,14 +170,16 @@
         return tp(data)
     elif issubclass_safe(tp, datetime.datetime):
         return datetime.datetime.fromisoformat(data)
     elif issubclass_safe(tp, datetime.date):
         return datetime.date.fromisoformat(data)
     elif issubclass_safe(tp, datetime.time):
         return datetime.time.fromisoformat(data)
+    elif issubclass_safe(tp, UUID):
+        return tp(data)
     elif isinstance(data, str):
         if issubclass_safe(tp, str):
             return tp(data)
         elif is_list_type(tp):
             data = parse_csv(data)
             return typecast(data, tp)
         else:
```

### Comparing `lessweb-1.3.0/lessweb.egg-info/PKG-INFO` & `lessweb-1.4.0/lessweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.3.0
+Version: 1.4.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `lessweb-1.3.0/lessweb.egg-info/SOURCES.txt` & `lessweb-1.4.0/lessweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/pyproject.toml` & `lessweb-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lessweb"
-version = "1.3.0"
+version = "1.4.0"
 description = 'A pythonic web framework'
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ['lessweb', 'web', 'web.py', 'aiohttp']
 authors = [
     {name = "qorzj", email = "goodhorsezxj@gmail.com"},
 ]
```

### Comparing `lessweb-1.3.0/tests/e2e/test_request_stack.py` & `lessweb-1.4.0/tests/e2e/test_request_stack.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.3.0/tests/test_typecast.py` & `lessweb-1.4.0/tests/test_typecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 import unittest
 from datetime import date, datetime, time
 from enum import Enum
 from typing import (Any, Dict, Generator, List, Literal, NewType, Optional,
                     TypedDict, Union)
+from uuid import UUID
 
 from lessweb.typecast import (TypeCastError, inspect_type,
                               semi_json_schema_type, typecast)
 
 NoneType = type(None)
 
 
@@ -83,14 +84,20 @@
 
     def test_typecast_time(self):
         data = "12:00:00"
         tp = time
         result = typecast(data, tp)
         self.assertEqual(result, time.fromisoformat(data))
 
+    def test_typecast_uuid(self):
+        data = 'f81d4fae-7dec-11d0-a765-00a0c91e6bf6'
+        tp = UUID
+        result = typecast(data, tp)
+        self.assertEqual(result.hex, 'f81d4fae7dec11d0a76500a0c91e6bf6')
+
     def test_typecast_str(self):
         data = "Hello"
         tp = str
         result = typecast(data, tp)
         self.assertEqual(result, data)
 
     def test_typecast_list(self):
```

