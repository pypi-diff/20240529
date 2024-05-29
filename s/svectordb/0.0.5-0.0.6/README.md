# Comparing `tmp/svectordb-0.0.5.tar.gz` & `tmp/svectordb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svectordb-0.0.5.tar", last modified: Wed Mar 27 09:08:10 2024, max compression
+gzip compressed data, was "svectordb-0.0.6.tar", last modified: Wed May 29 11:30:43 2024, max compression
```

## Comparing `svectordb-0.0.5.tar` & `svectordb-0.0.6.tar`

### file list

```diff
@@ -1,73 +1,87 @@
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.668269 svectordb-0.0.5/
--rw-r--r--   0 jacksen    (501) staff       (20)      922 2024-03-27 09:08:10.668049 svectordb-0.0.5/PKG-INFO
--rw-r--r--   0 jacksen    (501) staff       (20)      104 2024-03-27 09:05:09.000000 svectordb-0.0.5/README.md
--rw-r--r--   0 jacksen    (501) staff       (20)     1245 2024-03-27 09:04:21.000000 svectordb-0.0.5/pyproject.toml
--rw-r--r--   0 jacksen    (501) staff       (20)       38 2024-03-27 09:08:10.668313 svectordb-0.0.5/setup.cfg
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.657782 svectordb-0.0.5/smithy_aws_core/
--rw-r--r--   0 jacksen    (501) staff       (20)      584 2024-03-13 22:13:18.000000 svectordb-0.0.5/smithy_aws_core/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1977 2024-03-13 22:13:18.000000 svectordb-0.0.5/smithy_aws_core/identity.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.657984 svectordb-0.0.5/smithy_aws_core/interfaces/
--rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-03-13 22:13:18.000000 svectordb-0.0.5/smithy_aws_core/interfaces/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)        7 2024-03-13 22:13:18.000000 svectordb-0.0.5/smithy_aws_core/py.typed
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.659766 svectordb-0.0.5/smithy_core/
--rw-r--r--   0 jacksen    (501) staff       (20)     3876 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/__init__.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.660522 svectordb-0.0.5/smithy_core/aio/
--rw-r--r--   0 jacksen    (501) staff       (20)      803 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/aio/__init__.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.660875 svectordb-0.0.5/smithy_core/aio/interfaces/
--rw-r--r--   0 jacksen    (501) staff       (20)      659 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/aio/interfaces/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)      750 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/aio/interfaces/identity.py
--rw-r--r--   0 jacksen    (501) staff       (20)     9350 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/aio/types.py
--rw-r--r--   0 jacksen    (501) staff       (20)      425 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/aio/utils.py
--rw-r--r--   0 jacksen    (501) staff       (20)      751 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/exceptions.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1018 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/identity.py
--rw-r--r--   0 jacksen    (501) staff       (20)    28262 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/interceptors.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.661426 svectordb-0.0.5/smithy_core/interfaces/
--rw-r--r--   0 jacksen    (501) staff       (20)     1615 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/interfaces/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1198 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/interfaces/identity.py
--rw-r--r--   0 jacksen    (501) staff       (20)     4291 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/interfaces/retries.py
--rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/py.typed
--rw-r--r--   0 jacksen    (501) staff       (20)     9444 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/retries.py
--rw-r--r--   0 jacksen    (501) staff       (20)     4253 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/rfc3986.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1170 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/types.py
--rw-r--r--   0 jacksen    (501) staff       (20)     9023 2024-03-13 22:13:13.000000 svectordb-0.0.5/smithy_core/utils.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.662462 svectordb-0.0.5/smithy_http/
--rw-r--r--   0 jacksen    (501) staff       (20)     7495 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/__init__.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.663282 svectordb-0.0.5/smithy_http/aio/
--rw-r--r--   0 jacksen    (501) staff       (20)     1923 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     3912 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/aiohttp.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.663608 svectordb-0.0.5/smithy_http/aio/auth/
--rw-r--r--   0 jacksen    (501) staff       (20)      109 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/auth/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     4182 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/auth/apikey.py
--rw-r--r--   0 jacksen    (501) staff       (20)    10998 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/crt.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1389 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/endpoints.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.663945 svectordb-0.0.5/smithy_http/aio/identity/
--rw-r--r--   0 jacksen    (501) staff       (20)      109 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/identity/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1334 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/identity/apikey.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.664299 svectordb-0.0.5/smithy_http/aio/interfaces/
--rw-r--r--   0 jacksen    (501) staff       (20)     2526 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/interfaces/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)     3737 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/interfaces/auth.py
--rw-r--r--   0 jacksen    (501) staff       (20)     1786 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/aio/restjson.py
--rw-r--r--   0 jacksen    (501) staff       (20)      502 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/endpoints.py
--rw-r--r--   0 jacksen    (501) staff       (20)      279 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/exceptions.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.664464 svectordb-0.0.5/smithy_http/interfaces/
--rw-r--r--   0 jacksen    (501) staff       (20)     3775 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/interfaces/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/py.typed
--rw-r--r--   0 jacksen    (501) staff       (20)      871 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/restjson.py
--rw-r--r--   0 jacksen    (501) staff       (20)     4500 2024-03-13 22:13:08.000000 svectordb-0.0.5/smithy_http/utils.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.666504 svectordb-0.0.5/svectordb/
--rw-r--r--   0 jacksen    (501) staff       (20)       55 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/__init__.py
--rw-r--r--   0 jacksen    (501) staff       (20)      927 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/auth.py
--rw-r--r--   0 jacksen    (501) staff       (20)    23112 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/client.py
--rw-r--r--   0 jacksen    (501) staff       (20)     4766 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/config.py
--rw-r--r--   0 jacksen    (501) staff       (20)    22934 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/deserialize.py
--rw-r--r--   0 jacksen    (501) staff       (20)    14456 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/errors.py
--rw-r--r--   0 jacksen    (501) staff       (20)    32966 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/models.py
--rw-r--r--   0 jacksen    (501) staff       (20)     7872 2024-03-27 08:52:26.000000 svectordb-0.0.5/svectordb/serialize.py
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.667460 svectordb-0.0.5/svectordb.egg-info/
--rw-r--r--   0 jacksen    (501) staff       (20)      922 2024-03-27 09:08:10.000000 svectordb-0.0.5/svectordb.egg-info/PKG-INFO
--rw-r--r--   0 jacksen    (501) staff       (20)     1491 2024-03-27 09:08:10.000000 svectordb-0.0.5/svectordb.egg-info/SOURCES.txt
--rw-r--r--   0 jacksen    (501) staff       (20)        1 2024-03-27 09:08:10.000000 svectordb-0.0.5/svectordb.egg-info/dependency_links.txt
--rw-r--r--   0 jacksen    (501) staff       (20)       84 2024-03-27 09:08:10.000000 svectordb-0.0.5/svectordb.egg-info/requires.txt
--rw-r--r--   0 jacksen    (501) staff       (20)       55 2024-03-27 09:08:10.000000 svectordb-0.0.5/svectordb.egg-info/top_level.txt
-drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-03-27 09:08:10.667259 svectordb-0.0.5/tests/
--rw-r--r--   0 jacksen    (501) staff       (20)     1588 2024-03-27 08:52:26.000000 svectordb-0.0.5/tests/test_protocol.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.601647 svectordb-0.0.6/
+-rw-r--r--   0 jacksen    (501) staff       (20)      922 2024-05-29 11:30:43.601400 svectordb-0.0.6/PKG-INFO
+-rw-r--r--   0 jacksen    (501) staff       (20)      104 2024-05-29 11:21:05.000000 svectordb-0.0.6/README.md
+-rw-r--r--   0 jacksen    (501) staff       (20)     1271 2024-05-29 11:25:48.000000 svectordb-0.0.6/pyproject.toml
+-rw-r--r--   0 jacksen    (501) staff       (20)       38 2024-05-29 11:30:43.601688 svectordb-0.0.6/setup.cfg
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.589748 svectordb-0.0.6/smithy_aws_core/
+-rw-r--r--   0 jacksen    (501) staff       (20)      584 2024-05-29 11:27:02.000000 svectordb-0.0.6/smithy_aws_core/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1989 2024-05-29 11:27:02.000000 svectordb-0.0.6/smithy_aws_core/identity.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.589930 svectordb-0.0.6/smithy_aws_core/interfaces/
+-rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-05-29 11:27:02.000000 svectordb-0.0.6/smithy_aws_core/interfaces/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)        7 2024-05-29 11:27:02.000000 svectordb-0.0.6/smithy_aws_core/py.typed
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.593116 svectordb-0.0.6/smithy_core/
+-rw-r--r--   0 jacksen    (501) staff       (20)     4166 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/__init__.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.593762 svectordb-0.0.6/smithy_core/aio/
+-rw-r--r--   0 jacksen    (501) staff       (20)      107 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/aio/__init__.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.594036 svectordb-0.0.6/smithy_core/aio/interfaces/
+-rw-r--r--   0 jacksen    (501) staff       (20)     1651 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/aio/interfaces/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      754 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/aio/interfaces/identity.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     9369 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/aio/types.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1650 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/aio/utils.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     5642 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/deserializers.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    17977 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/documents.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      901 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/exceptions.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1022 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/identity.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    28327 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/interceptors.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.594589 svectordb-0.0.6/smithy_core/interfaces/
+-rw-r--r--   0 jacksen    (501) staff       (20)     1584 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/interfaces/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      398 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/interfaces/exceptions.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1198 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/interfaces/identity.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4297 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/interfaces/retries.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     2702 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/prelude.py
+-rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/py.typed
+-rw-r--r--   0 jacksen    (501) staff       (20)     9444 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/retries.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4252 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/rfc3986.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     7385 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/schemas.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    11382 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/serializers.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     3383 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/shapes.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      492 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/traits.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     3887 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/types.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     9026 2024-05-29 11:27:09.000000 svectordb-0.0.6/smithy_core/utils.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.595731 svectordb-0.0.6/smithy_http/
+-rw-r--r--   0 jacksen    (501) staff       (20)     8353 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/__init__.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.596493 svectordb-0.0.6/smithy_http/aio/
+-rw-r--r--   0 jacksen    (501) staff       (20)     2031 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4400 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/aiohttp.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.596756 svectordb-0.0.6/smithy_http/aio/auth/
+-rw-r--r--   0 jacksen    (501) staff       (20)      109 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/auth/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4184 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/auth/apikey.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    11369 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/crt.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1389 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/endpoints.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.597048 svectordb-0.0.6/smithy_http/aio/identity/
+-rw-r--r--   0 jacksen    (501) staff       (20)      109 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/identity/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1338 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/identity/apikey.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.597328 svectordb-0.0.6/smithy_http/aio/interfaces/
+-rw-r--r--   0 jacksen    (501) staff       (20)     3278 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/interfaces/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     3435 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/interfaces/auth.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     1968 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/aio/restjson.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      502 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/endpoints.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      279 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/exceptions.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.597458 svectordb-0.0.6/smithy_http/interfaces/
+-rw-r--r--   0 jacksen    (501) staff       (20)     4026 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/interfaces/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)        0 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/py.typed
+-rw-r--r--   0 jacksen    (501) staff       (20)      885 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/restjson.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4500 2024-05-29 11:27:13.000000 svectordb-0.0.6/smithy_http/utils.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.597766 svectordb-0.0.6/smithy_json/
+-rw-r--r--   0 jacksen    (501) staff       (20)      131 2024-05-29 11:27:18.000000 svectordb-0.0.6/smithy_json/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)        7 2024-05-29 11:27:18.000000 svectordb-0.0.6/smithy_json/py.typed
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.599388 svectordb-0.0.6/svectordb/
+-rw-r--r--   0 jacksen    (501) staff       (20)       55 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/__init__.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.600355 svectordb-0.0.6/svectordb/_private/
+-rw-r--r--   0 jacksen    (501) staff       (20)       55 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/_private/__init__.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    16604 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/_private/schemas.py
+-rw-r--r--   0 jacksen    (501) staff       (20)      934 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/auth.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    24334 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/client.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4766 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/config.py
+-rw-r--r--   0 jacksen    (501) staff       (20)    25195 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/deserialize.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     2855 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/errors.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     4117 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/models.py
+-rw-r--r--   0 jacksen    (501) staff       (20)     9125 2024-05-29 08:31:14.000000 svectordb-0.0.6/svectordb/serialize.py
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.600816 svectordb-0.0.6/svectordb.egg-info/
+-rw-r--r--   0 jacksen    (501) staff       (20)      922 2024-05-29 11:30:43.000000 svectordb-0.0.6/svectordb.egg-info/PKG-INFO
+-rw-r--r--   0 jacksen    (501) staff       (20)     1805 2024-05-29 11:30:43.000000 svectordb-0.0.6/svectordb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacksen    (501) staff       (20)        1 2024-05-29 11:30:43.000000 svectordb-0.0.6/svectordb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacksen    (501) staff       (20)       84 2024-05-29 11:30:43.000000 svectordb-0.0.6/svectordb.egg-info/requires.txt
+-rw-r--r--   0 jacksen    (501) staff       (20)       67 2024-05-29 11:30:43.000000 svectordb-0.0.6/svectordb.egg-info/top_level.txt
+drwxr-xr-x   0 jacksen    (501) staff       (20)        0 2024-05-29 11:30:43.600602 svectordb-0.0.6/tests/
+-rw-r--r--   0 jacksen    (501) staff       (20)     1909 2024-05-29 08:31:14.000000 svectordb-0.0.6/tests/test_protocol.py
```

### Comparing `svectordb-0.0.5/PKG-INFO` & `svectordb-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: svectordb
-Version: 0.0.5
+Version: 0.0.6
 Summary: svectordb client
 License: Apache-2.0
 Keywords: smithy,svectordb
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp<3.10.0,>=3.8.6
 Provides-Extra: tests
 Requires-Dist: pytest<8.0.0,>=7.2.0; extra == "tests"
 Requires-Dist: pytest-asyncio<0.21.0,>=0.20.3; extra == "tests"
 
 ## SvectorDB Client
```

### Comparing `svectordb-0.0.5/smithy_aws_core/__init__.py` & `svectordb-0.0.6/smithy_aws_core/__init__.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/smithy_aws_core/identity.py` & `svectordb-0.0.6/smithy_aws_core/identity.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,19 @@
         session_token: str | None = None,
         expiration: datetime | None = None,
     ) -> None:
         """Initialize the AWSCredentialIdentity.
 
         :param access_key_id: A unique identifier for an AWS user or role.
         :param secret_access_key: A secret key used in conjunction with the access key
-        ID to authenticate programmatic access to AWS services.
+            ID to authenticate programmatic access to AWS services.
         :param session_token: A temporary token used to specify the current session for
-        the supplied credentials.
-        :param expiration: The expiration time of the identity. If time zone is provided,
-        it is updated to UTC. The value must always be in UTC.
+            the supplied credentials.
+        :param expiration: The expiration time of the identity. If time zone is
+            provided, it is updated to UTC. The value must always be in UTC.
         """
         super().__init__(expiration=expiration)
         self._access_key_id: str = access_key_id
         self._secret_access_key: str = secret_access_key
         self._session_token: str | None = session_token
 
     @property
```

### Comparing `svectordb-0.0.5/smithy_core/__init__.py` & `svectordb-0.0.6/smithy_core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,22 +56,28 @@
     def __post_init__(self) -> None:
         """Validate host component."""
         if not rfc3986.HOST_MATCHER.match(self.host) and not rfc3986.IPv6_MATCHER.match(
             f"[{self.host}]"
         ):
             raise SmithyException(f"Invalid host: {self.host}")
 
-    @cached_property
+    @property
     def netloc(self) -> str:
         """Construct netloc string in format ``{username}:{password}@{host}:{port}``
 
         ``username``, ``password``, and ``port`` are only included if set. ``password``
         is ignored, unless ``username`` is also set. Add square brackets around the host
         if it is a valid IPv6 endpoint URI per :rfc:`3986#section-3.2.2`.
         """
+        return self._netloc
+
+    # cached_property does NOT behave like property, it actually allows for setting.
+    # Therefore we need a layer of indirection.
+    @cached_property
+    def _netloc(self) -> str:
         if self.username is not None:
             password = "" if self.password is None else f":{self.password}"
             userinfo = f"{self.username}{password}@"
         else:
             userinfo = ""
 
         if self.port is not None:
@@ -82,17 +88,21 @@
         if self.host_type == HostType.IPv6:
             host = f"[{self.host}]"
         else:
             host = self.host
 
         return f"{userinfo}{host}{port}"
 
-    @cached_property
+    @property
     def host_type(self) -> HostType:
         """Return the type of host."""
+        return self._host_type
+
+    @cached_property
+    def _host_type(self) -> HostType:
         if rfc3986.IPv6_MATCHER.match(f"[{self.host}]"):
             return HostType.IPv6
         if rfc3986.IPv4_MATCHER.match(self.host):
             return HostType.IPv4
         if rfc3986.HOST_MATCHER.match(self.host):
             return HostType.DOMAIN
         return HostType.UNKNOWN
```

### Comparing `svectordb-0.0.5/smithy_core/aio/__init__.py` & `svectordb-0.0.6/smithy_core/aio/interfaces/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,55 @@
-# Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
-# SPDX-License-Identifier: Apache-2.0
+#  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
+#  SPDX-License-Identifier: Apache-2.0
 from collections.abc import AsyncIterable
-from typing import Protocol
+from typing import Protocol, runtime_checkable
 
-from ..interfaces import URI
+from ...interfaces import URI
+from ...interfaces import StreamingBlob as SyncStreamingBlob
+
+
+@runtime_checkable
+class AsyncByteStream(Protocol):
+    """A file-like object with an async read method."""
+
+    async def read(self, size: int = -1) -> bytes: ...
+
+
+# A union of all acceptable streaming blob types. Deserialized payloads will
+# always return a ByteStream, or AsyncByteStream if async is enabled.
+type StreamingBlob = SyncStreamingBlob | AsyncByteStream | AsyncIterable[bytes]
 
 
 class Request(Protocol):
-    """Protocol-agnostic representation of a request."""
+    """Protocol-agnostic representation of a request.
+
+    :param destination: The URI where the request should be sent to.
+    :param body: The request payload as iterable of chunks of bytes.
+    """
 
     destination: URI
-    body: AsyncIterable[bytes]
+    body: StreamingBlob = b""
 
-    async def consume_body(self) -> bytes:
+    async def consume_body_async(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        ...
+
+    def consume_body(self) -> bytes:
         """Iterate over request body and return as bytes."""
         ...
 
 
 class Response(Protocol):
     """Protocol-agnostic representation of a response."""
 
     @property
-    def body(self) -> AsyncIterable[bytes]:
+    def body(self) -> StreamingBlob:
         """The response payload as iterable of chunks of bytes."""
         ...
 
-    async def consume_body(self) -> bytes:
+    async def consume_body_async(self) -> bytes:
         """Iterate over response body and return as bytes."""
         ...
+
+    def consume_body(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        ...
```

### Comparing `svectordb-0.0.5/smithy_core/aio/interfaces/identity.py` & `svectordb-0.0.6/smithy_core/aio/interfaces/identity.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,11 +12,11 @@
     """
 
     async def get_identity(
         self, *, identity_properties: IdentityPropertiesType_contra
     ) -> IdentityType_cov:
         """Load the user's identity from this resolver.
 
-        :param identity_properties: Properties used to help determine the
-        identity to return.
+        :param identity_properties: Properties used to help determine the identity to
+            return.
         """
         ...
```

### Comparing `svectordb-0.0.5/smithy_core/aio/types.py` & `svectordb-0.0.6/smithy_core/aio/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
             self._data = BytesIO(data)
         else:
             self._data = data
 
     async def read(self, size: int = -1) -> bytes:
         """Read a number of bytes from the stream.
 
-        :param size: The maximum number of bytes to read. If less than 0, all bytes
-        will be read.
+        :param size: The maximum number of bytes to read. If less than 0, all bytes will
+            be read.
         """
         if self._closed or not self._data:
             raise ValueError("I/O operation on closed file.")
 
         if isinstance(self._data, ByteStream) and not iscoroutinefunction(
             self._data.read
         ):
@@ -83,15 +83,15 @@
 
     def iter_chunks(
         self, chunk_size: int = _DEFAULT_CHUNK_SIZE
     ) -> AsyncIterator[bytes]:
         """Iterate over the reader in chunks of a given size.
 
         :param chunk_size: The maximum size of each chunk. If less than 0, the entire
-        reader will be read into one chunk.
+            reader will be read into one chunk.
         """
         return _AsyncByteStreamIterator(self.read, chunk_size)
 
     def readable(self) -> bool:
         """Returns whether the stream is readable."""
         return True
 
@@ -139,16 +139,16 @@
         else:
             self._buffer = BytesIO()
             self._data_source = AsyncBytesReader(data)
 
     async def read(self, size: int = -1) -> bytes:
         """Read a number of bytes from the stream.
 
-        :param size: The maximum number of bytes to read. If less than 0, all bytes
-        will be read.
+        :param size: The maximum number of bytes to read. If less than 0, all bytes will
+            be read.
         """
         if self._data_source is None or size == 0:
             return self._buffer.read(size)
 
         start = self._buffer.tell()
         current_buffer_size = self._buffer.seek(0, 2)
 
@@ -217,15 +217,15 @@
 
     def iter_chunks(
         self, chunk_size: int = _DEFAULT_CHUNK_SIZE
     ) -> AsyncIterator[bytes]:
         """Iterate over the reader in chunks of a given size.
 
         :param chunk_size: The maximum size of each chunk. If less than 0, the entire
-        reader will be read into one chunk.
+            reader will be read into one chunk.
         """
         return _AsyncByteStreamIterator(self.read, chunk_size)
 
     def readable(self) -> bool:
         """Returns whether the stream is readable."""
         return True
 
@@ -253,16 +253,15 @@
 class _AsyncByteStreamIterator:
     """An async bytes iterator that operates over an async read method."""
 
     def __init__(self, read: Callable[[int], Awaitable[bytes]], chunk_size: int):
         """Initializes self.
 
         :param read: An async callable that reads a given number of bytes from some
-        source.
-
+            source.
         :param chunk_size: The number of bytes to read in each iteration.
         """
         self._read = read
         self._chunk_size = chunk_size
 
     def __aiter__(self) -> Self:
         return self
```

### Comparing `svectordb-0.0.5/smithy_core/exceptions.py` & `svectordb-0.0.6/smithy_core/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,7 +15,12 @@
 class SmithyIdentityException(SmithyException):
     """Base exception type for all exceptions raised in identity resolution."""
 
 
 class MissingDependencyException(SmithyException):
     """Exception type raised when a feature that requires a missing optional dependency
     is called."""
+
+
+class AsyncBodyException(SmithyException):
+    """Exception indicating that a request with an async body type was created in a sync
+    context."""
```

### Comparing `svectordb-0.0.5/smithy_core/identity.py` & `svectordb-0.0.6/smithy_core/identity.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self,
         *,
         expiration: datetime | None = None,
     ) -> None:
         """Initialize an identity.
 
         :param expiration: The expiration time of the identity. If time zone is
-        provided, it is updated to UTC. The value must always be in UTC.
+            provided, it is updated to UTC. The value must always be in UTC.
         """
         if expiration is not None:
             expiration = ensure_utc(expiration)
         self.expiration: datetime | None = expiration
 
     @property
     def is_expired(self) -> bool:
```

### Comparing `svectordb-0.0.5/smithy_core/interceptors.py` & `svectordb-0.0.6/smithy_core/interceptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 from copy import copy, deepcopy
-from typing import Any, Generic, TypeVar
+from typing import Any, TypeVar
 
 Request = TypeVar("Request")
 Response = TypeVar("Response")
 TransportRequest = TypeVar("TransportRequest")
 TransportResponse = TypeVar("TransportResponse")
 
 
-class InterceptorContext(
-    Generic[Request, Response, TransportRequest, TransportResponse]
-):
+class InterceptorContext[Request, Response, TransportRequest, TransportResponse]:
     def __init__(
         self,
         *,
         request: Request,
         response: Response | Exception,
         transport_request: TransportRequest,
         transport_response: TransportResponse,
@@ -97,25 +95,27 @@
         """Copy the context object, optionally overriding certain properties."""
         if transport_request is None:
             transport_request = copy(self._transport_request)
 
         if transport_response is None:
             transport_response = copy(self._transport_response)
 
-        context = InterceptorContext(
+        context: InterceptorContext[
+            Request, Response, TransportRequest, TransportResponse
+        ] = InterceptorContext(
             request=request if request is not None else self._request,
             response=response if response is not None else self._response,
             transport_request=transport_request,
             transport_response=transport_response,
         )
         context._properties = deepcopy(self._properties)
         return context
 
 
-class Interceptor(Generic[Request, Response, TransportRequest, TransportResponse]):
+class Interceptor[Request, Response, TransportRequest, TransportResponse]:
     """Allows injecting code into the SDK's request execution pipeline.
 
     Terminology:
 
     * execution - An execution is one end-to-end invocation against a client.
     * attempt - An attempt is an attempt at performing an execution. By default,
         executions are retried multiple times based on the client's retry strategy.
```

### Comparing `svectordb-0.0.5/smithy_core/interfaces/__init__.py` & `svectordb-0.0.6/smithy_core/interfaces/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from typing import Protocol, Union, runtime_checkable
+from typing import Protocol, runtime_checkable
 
 
 class URI(Protocol):
     """Universal Resource Identifier, target location for a :py:class:`Request`."""
 
     scheme: str
     """For example ``http`` or ``mqtts``."""
@@ -44,18 +44,13 @@
         ...
 
 
 @runtime_checkable
 class ByteStream(Protocol):
     """A file-like object with a read method that returns bytes."""
 
-    def read(self, size: int = -1) -> bytes:
-        pass
+    def read(self, size: int = -1) -> bytes: ...
 
 
 # A union of all acceptable streaming blob types. Deserialized payloads will
 # always return a ByteStream, or AsyncByteStream if async is enabled.
-StreamingBlob = Union[
-    ByteStream,
-    bytes,
-    bytearray,
-]
+type StreamingBlob = ByteStream | bytes | bytearray
```

### Comparing `svectordb-0.0.5/smithy_core/interfaces/identity.py` & `svectordb-0.0.6/smithy_core/interfaces/identity.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/smithy_core/interfaces/retries.py` & `svectordb-0.0.6/smithy_core/interfaces/retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,17 @@
 
     def acquire_initial_retry_token(
         self, *, token_scope: str | None = None
     ) -> RetryToken:
         """Called before any retries (for the first attempt at the operation).
 
         :param token_scope: An arbitrary string accepted by the retry strategy to
-        separate tokens into scopes.
-
+            separate tokens into scopes.
         :returns: A retry token, to be used for determining the retry delay, refreshing
-        the token after a failure, and recording success after success.
-
+            the token after a failure, and recording success after success.
         :raises SmithyRetryException: If the retry strategy has no available tokens.
         """
         ...
 
     def refresh_retry_token_for_retry(
         self, *, token_to_renew: RetryToken, error_info: RetryErrorInfo
     ) -> RetryToken:
@@ -109,13 +107,13 @@
         :raises SmithyRetryException: If no further retry attempts are allowed.
         """
         ...
 
     def record_success(self, *, token: RetryToken) -> None:
         """Return token after successful completion of an operation.
 
-        Upon successful completion of the operation, a user calls this function
-        to record that the operation was successful.
+        Upon successful completion of the operation, a user calls this function to
+        record that the operation was successful.
 
         :param token: The token used for the previous successful attempt.
         """
         ...
```

### Comparing `svectordb-0.0.5/smithy_core/retries.py` & `svectordb-0.0.6/smithy_core/retries.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/smithy_core/rfc3986.py` & `svectordb-0.0.6/smithy_core/rfc3986.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 """Module vended from rfc3986 ``abnf_rexexp.py`` and ``misc.py``.
 
 https://github.com/python-hyper/rfc3986/blob/main/src/rfc3986/abnf_regexp.py
 https://github.com/python-hyper/rfc3986/blob/main/src/rfc3986/misc.py
 """
 import re
```

### Comparing `svectordb-0.0.5/smithy_core/utils.py` & `svectordb-0.0.6/smithy_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # Same as RFC3339, but with microsecond precision.
 RFC3339_MICRO = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 def ensure_utc(value: datetime) -> datetime:
     """Ensures that the given datetime is a UTC timezone-aware datetime.
 
-    If the datetime isn't timezone-aware, its timezone is set to UTC. If it is
-    aware, it's replaced with the equivalent datetime under UTC.
+    If the datetime isn't timezone-aware, its timezone is set to UTC. If it is aware,
+    it's replaced with the equivalent datetime under UTC.
 
     :param value: A datetime object that may or may not be timezone-aware.
     :returns: A UTC timezone-aware equivalent datetime.
     """
     if value.tzinfo is None:
         return value.replace(tzinfo=timezone.utc)
     else:
@@ -67,25 +67,23 @@
         return epoch_zero + timedelta(seconds=value)
 
 
 _T = TypeVar("_T")
 
 
 @overload
-def expect_type(typ: type[_T], value: Any) -> _T:
-    ...
+def expect_type(typ: type[_T], value: Any) -> _T: ...
 
 
 # For some reason, mypy and other type checkers don't treat Union like a full type
 # despite it being checkable with isinstance and other methods. This essentially means
 # we can't pass back the given type when we're given a union. So instead we have to
 # return Any.
 @overload
-def expect_type(typ: UnionType, value: Any) -> Any:
-    ...
+def expect_type(typ: UnionType, value: Any) -> Any: ...
 
 
 def expect_type(typ: UnionType | type, value: Any) -> Any:
     """Asserts a value is of the given type and returns it unchanged.
 
     This performs both a runtime assertion and type narrowing during type checking
     similar to ``typing.cast``. If the runtime assertion is not needed, ``typing.cast``
@@ -154,16 +152,16 @@
     re.VERBOSE,
 )
 
 
 def strict_parse_float(given: str) -> float:
     """Strictly parses a float from a string.
 
-    Unlike float(), this forbids the use of "inf" and case-sensitively matches
-    Infinity and NaN.
+    Unlike float(), this forbids the use of "inf" and case-sensitively matches Infinity
+    and NaN.
 
     :param given: A string that is expected to contain a float.
     :returns: The given string parsed to a float.
     :raises ExpectationNotMetException: If the given string isn't a float.
     """
     if _FLOAT_REGEX.fullmatch(given):
         return float(given)
@@ -242,15 +240,15 @@
 
     Optionally removes consecutive slashes.
 
     :param path: The path to modify.
     :param remove_consecutive_slashes: Whether to remove consecutive slashes.
     :returns: The path with dot segments removed.
     """
-    output = []
+    output: list[str] = []
     for segment in path.split("/"):
         if segment == ".":
             continue
         elif segment != "..":
             output.append(segment)
         elif output:
             output.pop()
```

### Comparing `svectordb-0.0.5/smithy_http/__init__.py` & `svectordb-0.0.6/smithy_http/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         self,
         initial: Iterable[interfaces.Field] | None = None,
         *,
         encoding: str = "utf-8",
     ):
         """Collection of header and trailer entries mapped by name.
 
-        :param initial: Initial list of ``Field`` objects. ``Field``s can alse be added
-        with :func:`set_field` and later removed with :func:`remove_field`.
+        :param initial: Initial list of ``Field`` objects. ``Field``s can also be added
+        and later removed.
         :param encoding: The string encoding to be used when converting the ``Field``
         name and value from ``str`` to ``bytes`` for transmission.
         """
         init_fields = [fld for fld in initial] if initial is not None else []
         init_field_names = [self._normalize_field_name(fld.name) for fld in init_fields]
         fname_counter = Counter(init_field_names)
         repeated_names_exist = (
@@ -113,24 +113,39 @@
                 f"{', '.join(non_unique_names)}."
             )
         init_tuples = zip(init_field_names, init_fields)
         self.entries: OrderedDict[str, interfaces.Field] = OrderedDict(init_tuples)
         self.encoding: str = encoding
 
     def set_field(self, field: interfaces.Field) -> None:
-        """Set entry for a Field name."""
-        normalized_name = self._normalize_field_name(field.name)
+        """Alias for __setitem__ to utilize the field.name for the entry key."""
+        self.__setitem__(field.name, field)
+
+    def __setitem__(self, name: str, field: interfaces.Field) -> None:
+        """Set or override entry for a Field name."""
+        normalized_name = self._normalize_field_name(name)
+        normalized_field_name = self._normalize_field_name(field.name)
+        if normalized_name != normalized_field_name:
+            raise ValueError(
+                f"Supplied key {name} does not match Field.name "
+                f"provided: {normalized_field_name}"
+            )
         self.entries[normalized_name] = field
 
-    def get_field(self, name: str) -> interfaces.Field:
+    def get(
+        self, key: str, default: interfaces.Field | None = None
+    ) -> interfaces.Field | None:
+        return self[key] if key in self else default
+
+    def __getitem__(self, name: str) -> interfaces.Field:
         """Retrieve Field entry."""
         normalized_name = self._normalize_field_name(name)
         return self.entries[normalized_name]
 
-    def remove_field(self, name: str) -> None:
+    def __delitem__(self, name: str) -> None:
         """Delete entry from collection."""
         normalized_name = self._normalize_field_name(name)
         del self.entries[normalized_name]
 
     def get_by_type(self, kind: FieldPosition) -> list[interfaces.Field]:
         """Helper function for retrieving specific types of fields.
 
@@ -143,19 +158,19 @@
 
         For every `Field` in the ``entries`` of ``other``: If the normalized name
         already exists in the current ``entries``, the values from ``other`` are
         appended. Otherwise, the ``Field`` is added to the list of ``entries``.
         """
         for other_field in other:
             try:
-                cur_field = self.get_field(name=other_field.name)
+                cur_field = self.__getitem__(other_field.name)
                 for other_value in other_field.values:
                     cur_field.add(other_value)
             except KeyError:
-                self.set_field(other_field)
+                self.__setitem__(other_field.name, other_field)
 
     def _normalize_field_name(self, name: str) -> str:
         """Normalize field names.
 
         For use as key in ``entries``.
         """
         return name.lower()
@@ -168,14 +183,23 @@
         if not isinstance(other, Fields):
             return False
         return self.encoding == other.encoding and self.entries == other.entries
 
     def __iter__(self) -> Iterator[interfaces.Field]:
         yield from self.entries.values()
 
+    def __len__(self) -> int:
+        return len(self.entries)
+
+    def __repr__(self) -> str:
+        return f"Fields({self.entries})"
+
+    def __contains__(self, key: str) -> bool:
+        return self._normalize_field_name(key) in self.entries
+
 
 def quote_and_escape_field_value(value: str) -> str:
     """Escapes and quotes a single :class:`Field` value if necessary.
 
     See :func:`Field.as_string` for quoting and escaping logic.
     """
     chars_to_quote = (",", '"')
@@ -193,14 +217,14 @@
     one Field value.
 
     :param kind: The Field kind to define for all tuples.
     """
     fields = Fields()
     for name, value in tuples:
         try:
-            fields.get_field(name).add(value)
+            fields[name].add(value)
         except KeyError:
-            fields.set_field(
-                Field(name=name, values=[value], kind=kind or FieldPosition.HEADER)
+            fields[name] = Field(
+                name=name, values=[value], kind=kind or FieldPosition.HEADER
             )
 
     return fields
```

### Comparing `svectordb-0.0.5/smithy_http/aio/__init__.py` & `svectordb-0.0.6/smithy_http/aio/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 # SPDX-License-Identifier: Apache-2.0
-from collections.abc import AsyncIterable
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 
 from smithy_core import interfaces as core_interfaces
+from smithy_core.aio import interfaces as core_aio_interfaces
+from smithy_core.aio.utils import read_streaming_blob, read_streaming_blob_async
 
 from .. import interfaces as http_interfaces
 from . import interfaces as http_aio_interfaces
 
 
 @dataclass(kw_only=True)
 class HTTPRequest(http_aio_interfaces.HTTPRequest):
     """HTTP primitives for an Exchange to construct a version agnostic HTTP message."""
 
     destination: core_interfaces.URI
-    body: AsyncIterable[bytes]
+    body: core_aio_interfaces.StreamingBlob = field(repr=False, default=b"")
     method: str
     fields: http_interfaces.Fields
 
-    async def consume_body(self) -> bytes:
-        """Iterate over request body and return as bytes."""
-        body = b""
-        async for chunk in self.body:
-            body += chunk
-        return body
-
 
 # HTTPResponse implements http_interfaces.HTTPResponse but cannot be explicitly
 # annotated to reflect this because doing so causes Python to raise an AttributeError.
 # See https://github.com/python/typing/discussions/903#discussioncomment-4866851 for
 # details.
 @dataclass(kw_only=True)
 class HTTPResponse:
     """Basic implementation of :py:class:`.interfaces.HTTPResponse`.
 
     Implementations of :py:class:`.interfaces.HTTPClient` may return instances of this
     class or of custom response implementations.
     """
 
-    body: AsyncIterable[bytes]
+    body: core_aio_interfaces.StreamingBlob = field(repr=False, default=b"")
     """The response payload as iterable of chunks of bytes."""
 
     status: int
     """The 3 digit response status code (1xx, 2xx, 3xx, 4xx, 5xx)."""
 
     fields: http_interfaces.Fields
     """HTTP header and trailer fields."""
 
     reason: str | None = None
     """Optional string provided by the server explaining the status."""
 
-    async def consume_body(self) -> bytes:
+    async def consume_body_async(self) -> bytes:
         """Iterate over response body and return as bytes."""
-        body = b""
-        async for chunk in self.body:
-            body += chunk
-        return body
+        return await read_streaming_blob_async(body=self.body)
+
+    def consume_body(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        return read_streaming_blob(body=self.body)
```

### Comparing `svectordb-0.0.5/smithy_http/aio/aiohttp.py` & `svectordb-0.0.6/smithy_http/aio/aiohttp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 from copy import copy, deepcopy
 from itertools import chain
-from typing import Any
+from typing import TYPE_CHECKING, Any
 from urllib.parse import parse_qs, urlunparse
 
-try:
+if TYPE_CHECKING:
+    # pyright doesn't like optional imports. This is reasonable because if we use these
+    # in type hints then they'd result in runtime errors.
+    # TODO: add integ tests that import these without the dependendency installed
     import aiohttp
 
+try:
+    import aiohttp  # noqa: F811
+
     HAS_AIOHTTP = True
 except ImportError:
-    HAS_AIOHTTP = False
+    HAS_AIOHTTP = False  # type: ignore
 
+from smithy_core.aio.interfaces import StreamingBlob
+from smithy_core.aio.types import AsyncBytesReader
 from smithy_core.aio.utils import async_list
 from smithy_core.exceptions import MissingDependencyException
 from smithy_core.interfaces import URI
 
 from .. import Field, Fields
 from ..interfaces import (
     FieldPosition,
@@ -42,15 +50,15 @@
 class AIOHTTPClient(HTTPClient):
     """Implementation of :py:class:`.interfaces.HTTPClient` using aiohttp."""
 
     def __init__(
         self,
         *,
         client_config: AIOHTTPClientConfig | None = None,
-        _session: aiohttp.ClientSession | None = None,
+        _session: "aiohttp.ClientSession | None" = None,
     ) -> None:
         """
         :param client_config: Configuration that applies to all requests made with this
         client.
         """
         _assert_aiohttp()
         self._config = client_config or AIOHTTPClientConfig()
@@ -72,43 +80,45 @@
         headers_list = list(
             chain.from_iterable(
                 fld.as_tuples()
                 for fld in request.fields.get_by_type(FieldPosition.HEADER)
             )
         )
 
+        body: StreamingBlob = request.body
+        if not isinstance(body, AsyncBytesReader):
+            body = AsyncBytesReader(body)
+
         async with self._session.request(
             method=request.method,
             url=self._serialize_uri_without_query(request.destination),
             params=parse_qs(request.destination.query),
             headers=headers_list,
-            data=request.body,
+            data=body,
         ) as resp:
             return await self._marshal_response(resp)
 
     def _serialize_uri_without_query(self, uri: URI) -> str:
         """Serialize all parts of the URI up to and including the path."""
         components = (uri.scheme, uri.netloc, uri.path or "", "", "", "")
         return urlunparse(components)
 
     async def _marshal_response(
-        self, aiohttp_resp: aiohttp.ClientResponse
+        self, aiohttp_resp: "aiohttp.ClientResponse"
     ) -> HTTPResponseInterface:
         """Convert a ``aiohttp.ClientResponse`` to a ``smithy_http.aio.HTTPResponse``"""
         headers = Fields()
         for header_name, header_val in aiohttp_resp.headers.items():
             try:
-                headers.get_field(header_name).add(header_val)
+                headers[header_name].add(header_val)
             except KeyError:
-                headers.set_field(
-                    Field(
-                        name=header_name,
-                        values=[header_val],
-                        kind=FieldPosition.HEADER,
-                    )
+                headers[header_name] = Field(
+                    name=header_name,
+                    values=[header_val],
+                    kind=FieldPosition.HEADER,
                 )
 
         return HTTPResponse(
             status=aiohttp_resp.status,
             fields=headers,
             body=async_list([await aiohttp_resp.read()]),
             reason=aiohttp_resp.reason,
```

### Comparing `svectordb-0.0.5/smithy_http/aio/auth/apikey.py` & `svectordb-0.0.6/smithy_http/aio/auth/apikey.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     """The :rfc:`9110#section-11.4` scheme to prefix a header value with."""
 
     location: ApiKeyLocation
     """Where the key is serialized."""
 
 
 class ApiKeyConfig(Protocol):
-    api_key_identity_resolver: IdentityResolver[
-        ApiKeyIdentity, IdentityProperties
-    ] | None
+    api_key_identity_resolver: (
+        IdentityResolver[ApiKeyIdentity, IdentityProperties] | None
+    )
 
 
 @dataclass(init=False)
 class ApiKeyAuthScheme(
     HTTPAuthScheme[
         ApiKeyIdentity, ApiKeyConfig, IdentityProperties, ApiKeySigningProperties
     ]
```

### Comparing `svectordb-0.0.5/smithy_http/aio/crt.py` & `svectordb-0.0.6/smithy_http/aio/crt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
+#  pyright: reportMissingTypeStubs=false,reportUnknownMemberType=false
+#  flake8: noqa: F811
 import asyncio
 from collections.abc import AsyncGenerator, AsyncIterable, Awaitable
 from concurrent.futures import Future
 from io import BytesIO
 from threading import Lock
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
-try:
+if TYPE_CHECKING:
+    # pyright doesn't like optional imports. This is reasonable because if we use these
+    # in type hints then they'd result in runtime errors.
+    # TODO: add integ tests that import these without the dependendency installed
     from awscrt import http as crt_http
     from awscrt import io as crt_io
 
+try:
+    from awscrt import http as crt_http  # noqa: F811
+    from awscrt import io as crt_io  # noqa: F811
+
     HAS_CRT = True
 except ImportError:
-    HAS_CRT = False
+    HAS_CRT = False  # type: ignore
 
 from smithy_core import interfaces as core_interfaces
 from smithy_core.exceptions import MissingDependencyException
 
 from .. import Field, Fields
 from .. import interfaces as http_interfaces
 from ..exceptions import SmithyHTTPException
@@ -33,51 +42,49 @@
 
 
 class _AWSCRTEventLoop:
     def __init__(self) -> None:
         _assert_crt()
         self.bootstrap = self._initialize_default_loop()
 
-    def _initialize_default_loop(self) -> crt_io.ClientBootstrap:
+    def _initialize_default_loop(self) -> "crt_io.ClientBootstrap":
         event_loop_group = crt_io.EventLoopGroup(1)
         host_resolver = crt_io.DefaultHostResolver(event_loop_group)
         return crt_io.ClientBootstrap(event_loop_group, host_resolver)
 
 
 class AWSCRTHTTPResponse(http_aio_interfaces.HTTPResponse):
     def __init__(self) -> None:
         _assert_crt()
-        self._stream: crt_http.HttpClientStream | None = None
+        self._stream: "crt_http.HttpClientStream | None" = None
         self._status_code_future: Future[int] = Future()
         self._headers_future: Future[Fields] = Future()
         self._chunk_futures: list[Future[bytes]] = []
         self._received_chunks: list[bytes] = []
         self._chunk_lock: Lock = Lock()
 
-    def _set_stream(self, stream: crt_http.HttpClientStream) -> None:
+    def _set_stream(self, stream: "crt_http.HttpClientStream") -> None:
         if self._stream is not None:
             raise SmithyHTTPException("Stream already set on AWSCRTHTTPResponse object")
         self._stream = stream
         self._stream.completion_future.add_done_callback(self._on_complete)
         self._stream.activate()
 
     def _on_headers(
         self, status_code: int, headers: list[tuple[str, str]], **kwargs: Any
     ) -> None:  # pragma: crt-callback
         fields = Fields()
         for header_name, header_val in headers:
             try:
-                fields.get_field(header_name).add(header_val)
+                fields[header_name].add(header_val)
             except KeyError:
-                fields.set_field(
-                    Field(
-                        name=header_name,
-                        values=[header_val],
-                        kind=FieldPosition.HEADER,
-                    )
+                fields[header_name] = Field(
+                    name=header_name,
+                    values=[header_val],
+                    kind=FieldPosition.HEADER,
                 )
         self._status_code_future.set_result(status_code)
         self._headers_future.set_result(fields)
 
     def _on_body(self, chunk: bytes, **kwargs: Any) -> None:  # pragma: crt-callback
         with self._chunk_lock:
             # TODO: update back pressure window once CRT supports it
@@ -142,24 +149,17 @@
         while True:
             chunk = await self.get_chunk()
             if chunk:
                 yield chunk
             else:
                 break
 
-    async def consume_body(self) -> bytes:
-        """Iterate over request body and return as bytes."""
-        body = b""
-        async for chunk in self.body:
-            body += chunk
-        return body
-
 
 ConnectionPoolKey = tuple[str, str, int | None]
-ConnectionPoolDict = dict[ConnectionPoolKey, crt_http.HttpClientConnection]
+ConnectionPoolDict = dict[ConnectionPoolKey, "crt_http.HttpClientConnection"]
 
 
 class AWSCRTHTTPClientConfig(http_interfaces.HTTPClientConfiguration):
     def __post_init__(self) -> None:
         _assert_crt()
 
 
@@ -186,58 +186,59 @@
         self._client_bootstrap = self._eventloop.bootstrap
         self._tls_ctx = crt_io.ClientTlsContext(crt_io.TlsContextOptions())
         self._socket_options = crt_io.SocketOptions()
         self._connections: ConnectionPoolDict = {}
 
     async def send(
         self,
+        *,
         request: http_aio_interfaces.HTTPRequest,
-        request_config: http_interfaces.HTTPRequestConfiguration | None = None,
+        request_config: http_aio_interfaces.HTTPRequestConfiguration | None = None,
     ) -> AWSCRTHTTPResponse:
         """Send HTTP request using awscrt client.
 
         :param request: The request including destination URI, fields, payload.
         :param request_config: Configuration specific to this request.
         """
         crt_request = await self._marshal_request(request)
         connection = await self._get_connection(request.destination)
         crt_response = AWSCRTHTTPResponse()
         crt_stream = connection.request(
             crt_request,
-            crt_response._on_headers,
-            crt_response._on_body,
+            crt_response._on_headers,  # pyright: ignore[reportPrivateUsage]
+            crt_response._on_body,  # pyright: ignore[reportPrivateUsage]
         )
-        crt_response._set_stream(crt_stream)
+        crt_response._set_stream(crt_stream)  # pyright: ignore[reportPrivateUsage]
         return crt_response
 
     async def _create_connection(
         self, url: core_interfaces.URI
-    ) -> crt_http.HttpClientConnection:
+    ) -> "crt_http.HttpClientConnection":
         """Builds and validates connection to ``url``, returns it as
         ``asyncio.Future``"""
         connect_future = self._build_new_connection(url)
         connection = await asyncio.wrap_future(connect_future)
         self._validate_connection(connection)
         return connection
 
     async def _get_connection(
         self, url: core_interfaces.URI
-    ) -> crt_http.HttpClientConnection:
+    ) -> "crt_http.HttpClientConnection":
         # TODO: Use CRT connection pooling instead of this basic kind
         connection_key = (url.scheme, url.host, url.port)
         if connection_key in self._connections:
             return self._connections[connection_key]
         else:
             connection = await self._create_connection(url)
             self._connections[connection_key] = connection
             return connection
 
     def _build_new_connection(
         self, url: core_interfaces.URI
-    ) -> Future[crt_http.HttpClientConnection]:
+    ) -> Future["crt_http.HttpClientConnection"]:
         if url.scheme == "http":
             port = self._HTTP_PORT
             tls_connection_options = None
         elif url.scheme == "https":
             port = self._HTTPS_PORT
             tls_connection_options = self._tls_ctx.new_connection_options()
             tls_connection_options.set_server_name(url.host)
@@ -246,26 +247,26 @@
         else:
             raise SmithyHTTPException(
                 f"AWSCRTHTTPClient does not support URL scheme {url.scheme}"
             )
         if url.port is not None:
             port = url.port
 
-        connect_future: Future[
-            crt_http.HttpClientConnection
-        ] = crt_http.HttpClientConnection.new(
-            bootstrap=self._client_bootstrap,
-            host_name=url.host,
-            port=port,
-            socket_options=self._socket_options,
-            tls_connection_options=tls_connection_options,
+        connect_future: Future[crt_http.HttpClientConnection] = (
+            crt_http.HttpClientConnection.new(
+                bootstrap=self._client_bootstrap,
+                host_name=url.host,
+                port=port,
+                socket_options=self._socket_options,
+                tls_connection_options=tls_connection_options,
+            )
         )
         return connect_future
 
-    def _validate_connection(self, connection: crt_http.HttpClientConnection) -> None:
+    def _validate_connection(self, connection: "crt_http.HttpClientConnection") -> None:
         """Validates an existing connection against the client config.
 
         Checks performed:
         * If ``force_http_2`` is enabled: Is the connection HTTP/2?
         """
         force_http_2 = self._config.force_http_2
         if force_http_2 and connection.version is not crt_http.HttpVersion.Http2:
@@ -276,29 +277,27 @@
     def _render_path(self, url: core_interfaces.URI) -> str:
         path = url.path if url.path is not None else "/"
         query = f"?{url.query}" if url.query is not None else ""
         return f"{path}{query}"
 
     async def _marshal_request(
         self, request: http_aio_interfaces.HTTPRequest
-    ) -> crt_http.HttpRequest:
-        """
-        Create :py:class:`awscrt.http.HttpRequest` from
-        :py:class:`smithy_http.aio.HTTPRequest`
-        """
+    ) -> "crt_http.HttpRequest":
+        """Create :py:class:`awscrt.http.HttpRequest` from
+        :py:class:`smithy_http.aio.HTTPRequest`"""
         headers_list = []
         for fld in request.fields.entries.values():
             if fld.kind != FieldPosition.HEADER:
                 continue
             for val in fld.values:
                 headers_list.append((fld.name, val))
 
         path = self._render_path(request.destination)
         headers = crt_http.HttpHeaders(headers_list)
-        body = BytesIO(await request.consume_body())
+        body = BytesIO(await request.consume_body_async())
 
         crt_request = crt_http.HttpRequest(
             method=request.method,
             path=path,
             headers=headers,
             body_stream=body,
         )
```

### Comparing `svectordb-0.0.5/smithy_http/aio/endpoints.py` & `svectordb-0.0.6/smithy_http/aio/endpoints.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/smithy_http/aio/identity/apikey.py` & `svectordb-0.0.6/smithy_http/aio/identity/apikey.py`

 * *Files 17% similar despite different names*

```diff
@@ -27,12 +27,12 @@
                 self._identity = api_key
 
     async def get_identity(
         self, *, identity_properties: IdentityProperties
     ) -> ApiKeyIdentity:
         """Load the user's api key identity from this resolver.
 
-        :param identity_properties: Properties used to help determine the
-        identity to return.
+        :param identity_properties: Properties used to help determine the identity to
+            return.
         :returns: The api key identity.
         """
         return self._identity
```

### Comparing `svectordb-0.0.5/smithy_http/aio/interfaces/__init__.py` & `svectordb-0.0.6/smithy_http/aio/interfaces/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 from typing import Protocol, TypeVar
 
-from smithy_core.aio import Request, Response
+from smithy_core.aio.interfaces import Request, Response
+from smithy_core.aio.utils import read_streaming_blob, read_streaming_blob_async
 
 from ...interfaces import (
     Endpoint,
     Fields,
     HTTPClientConfiguration,
     HTTPRequestConfiguration,
 )
@@ -33,14 +34,22 @@
     :param fields: ``Fields`` object containing HTTP headers and trailers.
     :param body: A streamable collection of bytes.
     """
 
     method: str
     fields: Fields
 
+    async def consume_body_async(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        return await read_streaming_blob_async(self.body)
+
+    def consume_body(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        return read_streaming_blob(self.body)
+
 
 class HTTPResponse(Response, Protocol):
     """HTTP primitives returned from an Exchange, used to construct a client
     response."""
 
     @property
     def status(self) -> int:
@@ -53,27 +62,38 @@
         ...
 
     @property
     def reason(self) -> str | None:
         """Optional string provided by the server explaining the status."""
         ...
 
+    async def consume_body_async(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        return await read_streaming_blob_async(self.body)
+
+    def consume_body(self) -> bytes:
+        """Iterate over request body and return as bytes."""
+        return read_streaming_blob(self.body)
+
 
 class HTTPClient(Protocol):
     """An asynchronous HTTP client interface."""
 
     def __init__(self, *, client_config: HTTPClientConfiguration | None) -> None:
         """
         :param client_config: Configuration that applies to all requests made with this
         client.
         """
         ...
 
     async def send(
-        self, *, request: HTTPRequest, request_config: HTTPRequestConfiguration | None
+        self,
+        *,
+        request: HTTPRequest,
+        request_config: HTTPRequestConfiguration | None = None,
     ) -> HTTPResponse:
         """Send HTTP request over the wire and return the response.
 
         :param request: The request including destination URI, fields, payload.
         :param request_config: Configuration specific to this request.
         """
         ...
```

### Comparing `svectordb-0.0.5/smithy_http/aio/interfaces/auth.py` & `svectordb-0.0.6/smithy_http/aio/interfaces/auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,15 @@
 # ANY KIND, either express or implied. See the License for the specific
 # language governing permissions and limitations under the License.
 
 from dataclasses import dataclass
 from typing import Any, Protocol, TypedDict, TypeVar
 
 from smithy_core.aio.interfaces.identity import IdentityResolver
-from smithy_core.interfaces.identity import (
-    IdentityConfig_contra,
-    IdentityPropertiesType_contra,
-    IdentityType,
-    IdentityType_contra,
-)
+from smithy_core.interfaces.identity import Identity, IdentityProperties
 
 from . import HTTPRequest
 
 
 class SigningProperties(TypedDict):
     """Additional properties loaded to modify the signing process."""
 
@@ -33,55 +28,46 @@
 
 SigningPropertiesType = TypeVar("SigningPropertiesType", bound=SigningProperties)
 SigningPropertiesType_contra = TypeVar(
     "SigningPropertiesType_contra", bound=SigningProperties, contravariant=True
 )
 
 
-class HTTPSigner(Protocol[IdentityType_contra, SigningPropertiesType_contra]):
+class HTTPSigner[I: Identity, SP: SigningProperties](Protocol):
     """An interface for generating a signed HTTP request."""
 
     async def sign(
         self,
         *,
         http_request: HTTPRequest,
-        identity: IdentityType_contra,
-        signing_properties: SigningPropertiesType_contra,
+        identity: I,
+        signing_properties: SP,
     ) -> HTTPRequest:
         """Generate a new signed HTTPRequest based on the one provided.
 
         :param http_request: The HTTP request to sign.
-
         :param identity: The signing identity.
-
-        :param signing_properties: Additional properties loaded to modify the
-        signing process.
+        :param signing_properties: Additional properties loaded to modify the signing
+            process.
         """
         ...
 
 
-class HTTPAuthScheme(
-    Protocol[
-        IdentityType,
-        IdentityConfig_contra,
-        IdentityPropertiesType_contra,
-        SigningPropertiesType,
-    ]
+class HTTPAuthScheme[I: Identity, C, IP: IdentityProperties, SP: SigningProperties](
+    Protocol
 ):
     """Represents a way a service will authenticate the user's identity."""
 
     # A unique identifier for the authentication scheme.
     scheme_id: str
 
     # An API that can be used to sign HTTP requests.
-    signer: HTTPSigner[IdentityType, SigningPropertiesType]
+    signer: HTTPSigner[I, SP]
 
-    def identity_resolver(
-        self, *, config: IdentityConfig_contra
-    ) -> IdentityResolver[IdentityType, IdentityPropertiesType_contra]:
+    def identity_resolver(self, *, config: C) -> IdentityResolver[I, IP]:
         """An API that can be queried to resolve identity."""
         ...
 
 
 @dataclass(kw_only=True)
 class HTTPAuthOption:
     """Auth scheme used for signing and identity resolution."""
@@ -114,10 +100,10 @@
 
     def resolve_auth_scheme(
         self, *, auth_parameters: AuthSchemeParameters
     ) -> list[HTTPAuthOption]:
         """Resolve an ordered list of applicable auth schemes.
 
         :param auth_parameters: The parameters required for determining which
-        authentication schemes to potentially use.
+            authentication schemes to potentially use.
         """
         ...
```

### Comparing `svectordb-0.0.5/smithy_http/aio/restjson.py` & `svectordb-0.0.6/smithy_http/aio/restjson.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 import json
 
-from smithy_core.types import Document
+from smithy_core.documents import DocumentValue
 from smithy_core.utils import expect_type
 
-from ..restjson import (
-    _REST_JSON_CODE_HEADER,
-    _REST_JSON_CODE_KEYS,
-    _REST_JSON_MESSAGE_KEYS,
-    RestJsonErrorInfo,
-)
+from ..restjson import _REST_JSON_CODE_HEADER  # pyright: ignore[reportPrivateUsage]
+from ..restjson import _REST_JSON_CODE_KEYS  # pyright: ignore[reportPrivateUsage]
+from ..restjson import _REST_JSON_MESSAGE_KEYS  # pyright: ignore[reportPrivateUsage]
+from ..restjson import RestJsonErrorInfo
 from .interfaces import HTTPResponse
 
 
 async def parse_rest_json_error_info(
     http_response: HTTPResponse, check_body: bool = True
 ) -> RestJsonErrorInfo:
     """Parses generic RestJson error info from an HTTP response.
 
     :param http_response: The HTTP response to parse.
     :param check_body: Whether to check the body for the code / message.
     :returns: The parsed error information.
     """
     code: str | None = None
     message: str | None = None
-    json_body: dict[str, Document] | None = None
+    json_body: dict[str, DocumentValue] | None = None
 
     for field in http_response.fields:
         if field.name.lower() == _REST_JSON_CODE_HEADER:
             code = field.values[0]
 
     if check_body:
-        if body := await http_response.consume_body():
+        if body := await http_response.consume_body_async():
             json_body = json.loads(body)
 
         if json_body:
             for key, value in json_body.items():
                 key_lower = key.lower()
                 if not code and key_lower in _REST_JSON_CODE_KEYS:
                     code = expect_type(str, value)
```

### Comparing `svectordb-0.0.5/smithy_http/interfaces/__init__.py` & `svectordb-0.0.6/smithy_http/interfaces/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,25 +71,37 @@
     fields."""
 
     # Entries are keyed off the name of a provided Field
     entries: dict[str, Field]
     encoding: str | None = "utf-8"
 
     def set_field(self, field: Field) -> None:
+        """Alias for __setitem__ to utilize the field.name for the entry key."""
+        ...
+
+    def __setitem__(self, name: str, field: Field) -> None:
         """Set entry for a Field name."""
         ...
 
-    def get_field(self, name: str) -> Field:
+    def __getitem__(self, name: str) -> Field:
         """Retrieve Field entry."""
         ...
 
-    def remove_field(self, name: str) -> None:
+    def __delitem__(self, name: str) -> None:
         """Delete entry from collection."""
         ...
 
+    def __iter__(self) -> Iterator[Field]:
+        """Allow iteration over entries."""
+        ...
+
+    def __len__(self) -> int:
+        """Get total number of Field entries."""
+        ...
+
     def get_by_type(self, kind: FieldPosition) -> list[Field]:
         """Helper function for retrieving specific types of fields.
 
         Used to grab all headers or all trailers.
         """
         ...
 
@@ -98,18 +110,14 @@
 
         For every `Field` in the ``entries`` of ``other``: If the normalized name
         already exists in the current ``entries``, the values from ``other`` are
         appended. Otherwise, the ``Field`` is added to the list of ``entries``.
         """
         ...
 
-    def __iter__(self) -> Iterator[Field]:
-        """Allow iteration over entries."""
-        ...
-
 
 QueryParamsList = list[tuple[str, str]]
 
 
 class Endpoint(Protocol):
     uri: URI
     headers: Fields
@@ -125,12 +133,12 @@
     force_http_2: bool = False
 
 
 @dataclass(kw_only=True)
 class HTTPRequestConfiguration:
     """Request-level HTTP configuration.
 
-    :param read_timeout: How long, in seconds, the client will attempt to read the
-    first byte over an established, open connection before timing out.
+    :param read_timeout: How long, in seconds, the client will attempt to read the first
+        byte over an established, open connection before timing out.
     """
 
     read_timeout: float | None = None
```

### Comparing `svectordb-0.0.5/smithy_http/restjson.py` & `svectordb-0.0.6/smithy_http/restjson.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #  Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 #  SPDX-License-Identifier: Apache-2.0
 from typing import NamedTuple
 
-from smithy_core.types import Document
+from smithy_core.documents import DocumentValue
 
 _REST_JSON_CODE_HEADER = "x-amzn-errortype"
 
 _REST_JSON_CODE_KEYS = {"__type", "code"}
 
 _REST_JSON_MESSAGE_KEYS = {"message", "errormessage", "error_message"}
 
@@ -21,9 +21,9 @@
     """The generic error message.
 
     A modeled error may have the error bound somewhere else. This is based off of
     checking the most common locations and is intended for use with excpetions that
     either didn't model the message or which are unknown.
     """
 
-    json_body: dict[str, Document] | None = None
+    json_body: dict[str, DocumentValue] | None = None
     """The HTTP response body parsed as JSON."""
```

### Comparing `svectordb-0.0.5/smithy_http/utils.py` & `svectordb-0.0.6/smithy_http/utils.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/svectordb/auth.py` & `svectordb-0.0.6/svectordb/auth.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         auth_options: list[HTTPAuthOption] = []
 
         if ((option := _generate_api_key_option(auth_parameters)) is not None):
             auth_options.append(option)
 
         return auth_options
 
-def _generate_api_key_option(auth_params: HTTPAuthParams) -> HTTPAuthOption:
+def _generate_api_key_option(auth_params: HTTPAuthParams) -> HTTPAuthOption | None:
     return HTTPAuthOption(
         scheme_id="smithy.api#httpApiKeyAuth",
         identity_properties={},
         signer_properties={
             "name": "Authorization",
             "location": ApiKeyLocation("header"),
             "scheme": "ApiKey",
```

### Comparing `svectordb-0.0.5/svectordb/client.py` & `svectordb-0.0.6/svectordb/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Code generated by smithy-python-codegen DO NOT EDIT.
 
 from asyncio import sleep
 from copy import deepcopy
+import logging
 from typing import Any, Awaitable, Callable, TypeVar, cast
 
 from smithy_core import URI
 from smithy_core.exceptions import SmithyRetryException
 from smithy_core.interceptors import Interceptor, InterceptorContext
+from smithy_core.interfaces.exceptions import HasFault
 from smithy_core.interfaces.identity import Identity
 from smithy_core.interfaces.retries import RetryErrorInfo, RetryErrorType
 from smithy_http.aio.interfaces import HTTPRequest, HTTPResponse
 from smithy_http.aio.interfaces.auth import HTTPAuthOption, HTTPSigner
 from smithy_http.endpoints import StaticEndpointParams
 from smithy_http.interfaces import HTTPRequestConfiguration
 
@@ -45,14 +47,17 @@
     _serialize_get_item,
     _serialize_list_items,
     _serialize_query,
     _serialize_set_item,
 )
 
 
+
+logger = logging.getLogger(__name__)
+
 Input = TypeVar("Input")
 Output = TypeVar("Output")
 
 class DatabaseService:
     """Client for DatabaseService
 
     :param config: Optional configuration for the client. Here you can set things like the
@@ -70,23 +75,23 @@
         if plugins:
             client_plugins.extend(plugins)
 
         for plugin in client_plugins:
             plugin(self._config)
 
     async def delete_item(self, input: DeleteItemInput, plugins: list[Plugin] | None = None) -> DeleteItemOutput:
-        """Invokes the DeleteItem operation.
+        """Deletes an item from the database.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
@@ -94,23 +99,23 @@
             serialize=_serialize_delete_item,
             deserialize=_deserialize_delete_item,
             config=self._config,
             operation_name="DeleteItem",
         )
 
     async def embed(self, input: EmbedInput, plugins: list[Plugin] | None = None) -> EmbedOutput:
-        """Invokes the Embed operation.
+        """Embeds input into a vector.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
@@ -118,23 +123,23 @@
             serialize=_serialize_embed,
             deserialize=_deserialize_embed,
             config=self._config,
             operation_name="Embed",
         )
 
     async def get_item(self, input: GetItemInput, plugins: list[Plugin] | None = None) -> GetItemOutput:
-        """Invokes the GetItem operation.
+        """Retrieves a single item from the database.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
@@ -142,23 +147,23 @@
             serialize=_serialize_get_item,
             deserialize=_deserialize_get_item,
             config=self._config,
             operation_name="GetItem",
         )
 
     async def list_items(self, input: ListItemsInput, plugins: list[Plugin] | None = None) -> ListItemsOutput:
-        """Invokes the ListItems operation.
+        """Lists items in the database.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
@@ -166,23 +171,23 @@
             serialize=_serialize_list_items,
             deserialize=_deserialize_list_items,
             config=self._config,
             operation_name="ListItems",
         )
 
     async def query(self, input: QueryInput, plugins: list[Plugin] | None = None) -> QueryOutput:
-        """Invokes the Query operation.
+        """Queries the database for items.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
@@ -190,37 +195,64 @@
             serialize=_serialize_query,
             deserialize=_deserialize_query,
             config=self._config,
             operation_name="Query",
         )
 
     async def set_item(self, input: SetItemInput, plugins: list[Plugin] | None = None) -> SetItemOutput:
-        """Invokes the SetItem operation.
+        """Inserts or overwrites an item in the database.
 
         :param input: The operation's input.
 
         :param plugins: A list of callables that modify the configuration dynamically.
         Changes made by these plugins only apply for the duration of the operation
         execution and will not affect any other operation invocations.
         """
-        operation_plugins = [
+        operation_plugins: list[Plugin] = [
 
         ]
         if plugins:
             operation_plugins.extend(plugins)
 
         return await self._execute_operation(
             input=input,
             plugins=operation_plugins,
             serialize=_serialize_set_item,
             deserialize=_deserialize_set_item,
             config=self._config,
             operation_name="SetItem",
         )
 
+    def _classify_error(
+        self,
+        *,
+        error: Exception,
+        context: InterceptorContext[Input, Output, HTTPRequest, HTTPResponse | None]
+    ) -> RetryErrorInfo:
+
+        if not isinstance(error, HasFault) and not context.transport_response:
+            return RetryErrorInfo(error_type=RetryErrorType.TRANSIENT)
+
+        if context.transport_response:
+            if context.transport_response.status in [429, 503]:
+                retry_after = None
+                retry_header = context.transport_response.fields["retry-after"]
+                if retry_header and retry_header.values:
+                    retry_after = float(retry_header.values[0])
+                return RetryErrorInfo(error_type=RetryErrorType.THROTTLING, retry_after_hint=retry_after)
+
+            if context.transport_response.status >= 500:
+                return RetryErrorInfo(error_type=RetryErrorType.SERVER_ERROR)
+
+        error_type = RetryErrorType.CLIENT_ERROR
+        if isinstance(error, HasFault) and error.fault == "server":
+            error_type = RetryErrorType.SERVER_ERROR
+
+        return RetryErrorInfo(error_type=error_type)
+
     async def _execute_operation(
         self,
         input: Input,
         plugins: list[Plugin],
         serialize: Callable[[Input, Config], Awaitable[HTTPRequest]],
         deserialize: Callable[[HTTPResponse, Config], Awaitable[Output]],
         config: Config,
@@ -242,14 +274,15 @@
         input: Input,
         plugins: list[Plugin],
         serialize: Callable[[Input, Config], Awaitable[HTTPRequest]],
         deserialize: Callable[[HTTPResponse, Config], Awaitable[Output]],
         config: Config,
         operation_name: str,
     ) -> Output:
+        logger.debug(f"Making request for operation {operation_name} with parameters: {input}")
         context: InterceptorContext[Input, None, None, None] = InterceptorContext(
             request=input,
             response=None,
             transport_request=None,
             transport_response=None,
         )
         _client_interceptors = config.interceptors
@@ -331,29 +364,29 @@
                 context = context_with_response  # type: ignore
 
                 if isinstance(context_with_response.response, Exception):
                     # Step 7u: Reacquire retry token if the attempt failed
                     try:
                         retry_token = retry_strategy.refresh_retry_token_for_retry(
                             token_to_renew=retry_token,
-                            error_info=RetryErrorInfo(
-                                # TODO: Determine the error type.
-                                error_type=RetryErrorType.CLIENT_ERROR,
+                            error_info=self._classify_error(
+                                error=context_with_response.response,
+                                context=context_with_response,
                             )
                         )
                     except SmithyRetryException:
                         raise context_with_response.response
                     await sleep(retry_token.retry_delay)
                 else:
                     # Step 8: Invoke record_success
                     retry_strategy.record_success(token=retry_token)
                     break
         except Exception as e:
             if context.response is not None:
-                # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                logger.exception(f"Exception occurred while handling: {context.response}")
                 pass
             context._response = e
 
         # At this point, the context's request will have been definitively set, and
         # The response will be set either with the modeled output or an exception. The
         # transport_request and transport_response may be set or None.
         execution_context = cast(
@@ -403,18 +436,14 @@
 
                 # Step 7e: Invoke identity_resolver.get_identity
                 identity = await identity_resolver.get_identity(
                     identity_properties=auth_option.identity_properties
                 )
 
             # Step 7f: Invoke endpoint_resolver.resolve_endpoint
-            if config.endpoint_resolver is None:
-                raise ServiceError(
-                    "No endpoint_resolver found on the operation config."
-                )
             if config.endpoint_uri is None:
                 raise ServiceError(
                     "No endpoint_uri found on the operation config."
                 )
 
             endpoint = await config.endpoint_resolver.resolve_endpoint(
                 StaticEndpointParams(uri=config.endpoint_uri)
@@ -498,15 +527,15 @@
             )
 
             # Step 7r: Invoke read_after_deserialization
             for interceptor in interceptors:
                 interceptor.read_after_deserialization(context_with_output)
         except Exception as e:
             if context.response is not None:
-                # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                logger.exception(f"Exception occurred while handling: {context.response}")
                 pass
             context._response = e
 
         # At this point, the context's request and transport_request have definitively been set,
         # the response is either set or an exception, and the transport_resposne is either set or
         # None. This will also be true after _finalize_attempt because there is no opportunity
         # there to set the transport_response.
@@ -524,25 +553,25 @@
         try:
             for interceptor in interceptors:
                 context._response = interceptor.modify_before_attempt_completion(
                     context
                 )
         except Exception as e:
             if context.response is not None:
-                # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                logger.exception(f"Exception occurred while handling: {context.response}")
                 pass
             context._response = e
 
         # Step 7t: Invoke read_after_attempt
         for interceptor in interceptors:
             try:
                 interceptor.read_after_attempt(context)
             except Exception as e:
                 if context.response is not None:
-                    # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                    logger.exception(f"Exception occurred while handling: {context.response}")
                     pass
                 context._response = e
 
         return context
 
     async def _finalize_execution(
         self,
@@ -555,29 +584,29 @@
                 context._response = interceptor.modify_before_completion(context)
 
             # Step 10: Invoke trace_probe.dispatch_events
             try:
                 pass
             except Exception as e:
                 # log and ignore exceptions
-                # config.logger.exception(f"Exception occurred while dispatching trace events: {e}")
+                logger.exception(f"Exception occurred while dispatching trace events: {e}")
                 pass
         except Exception as e:
             if context.response is not None:
-                # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                logger.exception(f"Exception occurred while handling: {context.response}")
                 pass
             context._response = e
 
         # Step 11: Invoke read_after_execution
         for interceptor in interceptors:
             try:
                 interceptor.read_after_execution(context)
             except Exception as e:
                 if context.response is not None:
-                    # config.logger.exception(f"Exception occurred while handling: {context.response}")
+                    logger.exception(f"Exception occurred while handling: {context.response}")
                     pass
                 context._response = e
 
         # Step 12: Return / throw
         if isinstance(context.response, Exception):
             raise context.response
```

### Comparing `svectordb-0.0.5/svectordb/config.py` & `svectordb-0.0.6/svectordb/config.py`

 * *Files identical despite different names*

### Comparing `svectordb-0.0.5/svectordb/deserialize.py` & `svectordb-0.0.6/svectordb/deserialize.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Code generated by smithy-python-codegen DO NOT EDIT.
 
 from base64 import b64decode
 import json
-from typing import Any, cast
+from typing import Any
 
-from smithy_core.types import Document
+from smithy_core.documents import DocumentValue
 from smithy_core.utils import expect_type, limited_parse_float
 from smithy_http.aio.interfaces import HTTPResponse
 from smithy_http.aio.restjson import parse_rest_json_error_info
 
 from .config import Config
 from .errors import (
     AccessDeniedException,
@@ -25,14 +25,20 @@
 )
 from .models import (
     DeleteItemOutput,
     EmbedOutput,
     GetItemOutput,
     Item,
     ListItemsOutput,
+    MetadataValue,
+    MetadataValueNumber,
+    MetadataValueNumberArray,
+    MetadataValueString,
+    MetadataValueStringArray,
+    MetadataValueUnknown,
     QueryOutput,
     QueryResultItem,
     SetItemOutput,
     ValidationExceptionField,
 )
 
 
@@ -40,15 +46,15 @@
     if http_response.status != 204 and http_response.status >= 300:
         raise await _deserialize_error_delete_item(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
     return DeleteItemOutput(**kwargs)
 
-async def _deserialize_error_delete_item(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_delete_item(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -77,28 +83,28 @@
 
 async def _deserialize_embed(http_response: HTTPResponse, config: Config) -> EmbedOutput:
     if http_response.status != 200 and http_response.status >= 300:
         raise await _deserialize_error_embed(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
-    output: dict[str, Document] = {}
-    if (body := await http_response.consume_body()):
+    output: dict[str, DocumentValue] = {}
+    if (body := await http_response.consume_body_async()):
         output = json.loads(body)
 
     if (_consumed_embedding_units := output.get("consumedEmbeddingUnits")) is not None:
         kwargs["consumed_embedding_units"] = expect_type(int, _consumed_embedding_units)
 
     if "vector" not in output:
         raise ServiceError('Expected to find "vector" in the operation output, but it was not present.')
     kwargs["vector"] = _deserialize_vector(output['vector'], config)
 
     return EmbedOutput(**kwargs)
 
-async def _deserialize_error_embed(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_embed(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -127,33 +133,35 @@
 
 async def _deserialize_get_item(http_response: HTTPResponse, config: Config) -> GetItemOutput:
     if http_response.status != 200 and http_response.status >= 300:
         raise await _deserialize_error_get_item(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
-    output: dict[str, Document] = {}
-    if (body := await http_response.consume_body()):
+    output: dict[str, DocumentValue] = {}
+    if (body := await http_response.consume_body_async()):
         output = json.loads(body)
 
-    if "key" not in output:
-        raise ServiceError('Expected to find "key" in the operation output, but it was not present.')
-    kwargs["key"] = expect_type(str, output['key'])
-
-    if "value" not in output:
-        raise ServiceError('Expected to find "value" in the operation output, but it was not present.')
-    kwargs["value"] = b64decode(expect_type(str, output['value']))
+    if (_value := output.get("value")) is not None:
+        kwargs["value"] = b64decode(expect_type(str, _value))
 
     if "vector" not in output:
         raise ServiceError('Expected to find "vector" in the operation output, but it was not present.')
     kwargs["vector"] = _deserialize_vector(output['vector'], config)
 
+    if (_metadata := output.get("metadata")) is not None:
+        kwargs["metadata"] = _deserialize_metadata(_metadata, config)
+
+    if "key" not in output:
+        raise ServiceError('Expected to find "key" in the operation output, but it was not present.')
+    kwargs["key"] = expect_type(str, output['key'])
+
     return GetItemOutput(**kwargs)
 
-async def _deserialize_error_get_item(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_get_item(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -182,28 +190,28 @@
 
 async def _deserialize_list_items(http_response: HTTPResponse, config: Config) -> ListItemsOutput:
     if http_response.status != 200 and http_response.status >= 300:
         raise await _deserialize_error_list_items(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
-    output: dict[str, Document] = {}
-    if (body := await http_response.consume_body()):
+    output: dict[str, DocumentValue] = {}
+    if (body := await http_response.consume_body_async()):
         output = json.loads(body)
 
     if "items" not in output:
         raise ServiceError('Expected to find "items" in the operation output, but it was not present.')
     kwargs["items"] = _deserialize_item_list(output['items'], config)
 
     if (_next_token := output.get("nextToken")) is not None:
         kwargs["next_token"] = expect_type(str, _next_token)
 
     return ListItemsOutput(**kwargs)
 
-async def _deserialize_error_list_items(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_list_items(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -232,25 +240,25 @@
 
 async def _deserialize_query(http_response: HTTPResponse, config: Config) -> QueryOutput:
     if http_response.status != 200 and http_response.status >= 300:
         raise await _deserialize_error_query(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
-    output: dict[str, Document] = {}
-    if (body := await http_response.consume_body()):
+    output: dict[str, DocumentValue] = {}
+    if (body := await http_response.consume_body_async()):
         output = json.loads(body)
 
     if "results" not in output:
         raise ServiceError('Expected to find "results" in the operation output, but it was not present.')
     kwargs["results"] = _deserialize_query_result(output['results'], config)
 
     return QueryOutput(**kwargs)
 
-async def _deserialize_error_query(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_query(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -281,15 +289,15 @@
     if http_response.status != 204 and http_response.status >= 300:
         raise await _deserialize_error_set_item(http_response, config)
 
     kwargs: dict[str, Any] = {}
 
     return SetItemOutput(**kwargs)
 
-async def _deserialize_error_set_item(http_response: HTTPResponse, config: Config) -> ApiError[Any]:
+async def _deserialize_error_set_item(http_response: HTTPResponse, config: Config) -> ApiError:
     code, message, parsed_body = await parse_rest_json_error_info(http_response)
 
     match code.lower():
         case "internalservererror":
             return await _deserialize_error_internal_server_error(http_response, config, parsed_body, message)
 
         case "serviceunavailableerror":
@@ -315,167 +323,167 @@
 
         case _:
             return UnknownApiError(message)
 
 async def _deserialize_error_validation_exception(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> ValidationException:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
+
+    if (_field_list := output.get("fieldList")) is not None:
+        kwargs["field_list"] = _deserialize_validation_exception_field_list(_field_list, config)
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
-    if (_field_list := output.get("fieldList")) is not None:
-        kwargs["field_list"] = _deserialize_validation_exception_field_list(_field_list, config)
-
     return ValidationException(**kwargs)
 
 async def _deserialize_error_access_denied_exception(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> AccessDeniedException:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return AccessDeniedException(**kwargs)
 
 async def _deserialize_error_insufficient_funds_exception(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> InsufficientFundsException:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return InsufficientFundsException(**kwargs)
 
 async def _deserialize_error_internal_server_error(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> InternalServerError:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return InternalServerError(**kwargs)
 
 async def _deserialize_error_not_found_exception(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> NotFoundException:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return NotFoundException(**kwargs)
 
 async def _deserialize_error_quota_exceeded_exception(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> QuotaExceededException:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return QuotaExceededException(**kwargs)
 
 async def _deserialize_error_service_unavailable_error(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> ServiceUnavailableError:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return ServiceUnavailableError(**kwargs)
 
 async def _deserialize_error_throttling_error(
     http_response: HTTPResponse,
     config: Config,
-    parsed_body: dict[str, Document] | None,
+    parsed_body: dict[str, DocumentValue] | None,
     default_message: str,
 ) -> ThrottlingError:
     kwargs: dict[str, Any] = {"message": default_message}
 
-    if (parsed_body is None) and (body := await http_response.consume_body()):
+    if (parsed_body is None) and (body := await http_response.consume_body_async()):
         parsed_body = json.loads(body)
 
-    output: dict[str, Document] = parsed_body if parsed_body is not None else {}
+    output: dict[str, DocumentValue] = parsed_body if parsed_body is not None else {}
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return ThrottlingError(**kwargs)
 
-def _deserialize_validation_exception_field(output: Document, config: Config) -> ValidationExceptionField:
+def _deserialize_validation_exception_field(output: DocumentValue, config: Config) -> ValidationExceptionField:
     if not isinstance(output, dict):
         raise ServiceError(f"Expected dict, found {type(output)}")
 
     kwargs: dict[str, Any] = {}
 
     if "path" not in output:
         raise ServiceError('Expected to find "path" in the operation output, but it was not present.')
@@ -483,50 +491,88 @@
 
     if "message" not in output:
         raise ServiceError('Expected to find "message" in the operation output, but it was not present.')
     kwargs["message"] = expect_type(str, output['message'])
 
     return ValidationExceptionField(**kwargs)
 
-def _deserialize_validation_exception_field_list(output: Document, config: Config) -> list[ValidationExceptionField]:
+def _deserialize_validation_exception_field_list(output: DocumentValue, config: Config) -> list[ValidationExceptionField]:
     if not isinstance(output, list):
         raise ServiceError(f"Expected list, found {type(output)}")
     return [_deserialize_validation_exception_field(e, config) for e in output]
 
-def _deserialize_item(output: Document, config: Config) -> Item:
+def _deserialize_item(output: DocumentValue, config: Config) -> Item:
     if not isinstance(output, dict):
         raise ServiceError(f"Expected dict, found {type(output)}")
 
     kwargs: dict[str, Any] = {}
 
     if "key" not in output:
         raise ServiceError('Expected to find "key" in the operation output, but it was not present.')
     kwargs["key"] = expect_type(str, output['key'])
 
-    if "value" not in output:
-        raise ServiceError('Expected to find "value" in the operation output, but it was not present.')
-    kwargs["value"] = b64decode(expect_type(str, output['value']))
+    if (_value := output.get("value")) is not None:
+        kwargs["value"] = b64decode(expect_type(str, _value))
 
     if "vector" not in output:
         raise ServiceError('Expected to find "vector" in the operation output, but it was not present.')
     kwargs["vector"] = _deserialize_vector(output['vector'], config)
 
+    if (_metadata := output.get("metadata")) is not None:
+        kwargs["metadata"] = _deserialize_metadata(_metadata, config)
+
     return Item(**kwargs)
 
-def _deserialize_item_list(output: Document, config: Config) -> list[Item]:
+def _deserialize_item_list(output: DocumentValue, config: Config) -> list[Item]:
     if not isinstance(output, list):
         raise ServiceError(f"Expected list, found {type(output)}")
     return [_deserialize_item(e, config) for e in output]
 
-def _deserialize_query_result(output: Document, config: Config) -> list[QueryResultItem]:
+def _deserialize_metadata(output: DocumentValue, config: Config) -> dict[str, MetadataValue]:
+    if not isinstance(output, dict):
+        raise ServiceError(f"Expected dict, found { type(output) }")
+
+    return {k: _deserialize_metadata_value(v, config) for k, v in output.items() if v is not None}
+
+def _deserialize_metadata_value(output: DocumentValue, config: Config) -> MetadataValue:
+    if not isinstance(output, dict):
+        raise ServiceError(f"Expected dict, found {type(output)}")
+
+    if (count := len(output)) != 1:
+        raise ServiceError(f"Unions must have exactly one member set, found {count}.")
+
+    tag, value = list(output.items())[0]
+
+    match tag:
+        case "string":
+            return MetadataValueString(expect_type(str, value))
+
+        case "stringArray":
+            return MetadataValueStringArray(_deserialize_string_array(value, config))
+
+        case "number":
+            return MetadataValueNumber(limited_parse_float(value))
+
+        case "numberArray":
+            return MetadataValueNumberArray(_deserialize_number_array(value, config))
+
+        case _:
+            return MetadataValueUnknown(tag)
+
+def _deserialize_number_array(output: DocumentValue, config: Config) -> list[float]:
+    if not isinstance(output, list):
+        raise ServiceError(f"Expected list, found {type(output)}")
+    return [limited_parse_float(e) for e in output]
+
+def _deserialize_query_result(output: DocumentValue, config: Config) -> list[QueryResultItem]:
     if not isinstance(output, list):
         raise ServiceError(f"Expected list, found {type(output)}")
     return [_deserialize_query_result_item(e, config) for e in output]
 
-def _deserialize_query_result_item(output: Document, config: Config) -> QueryResultItem:
+def _deserialize_query_result_item(output: DocumentValue, config: Config) -> QueryResultItem:
     if not isinstance(output, dict):
         raise ServiceError(f"Expected dict, found {type(output)}")
 
     kwargs: dict[str, Any] = {}
 
     if "key" not in output:
         raise ServiceError('Expected to find "key" in the operation output, but it was not present.')
@@ -536,17 +582,26 @@
         raise ServiceError('Expected to find "value" in the operation output, but it was not present.')
     kwargs["value"] = b64decode(expect_type(str, output['value']))
 
     if "vector" not in output:
         raise ServiceError('Expected to find "vector" in the operation output, but it was not present.')
     kwargs["vector"] = _deserialize_vector(output['vector'], config)
 
+    if "metadata" not in output:
+        raise ServiceError('Expected to find "metadata" in the operation output, but it was not present.')
+    kwargs["metadata"] = _deserialize_metadata(output['metadata'], config)
+
     if "distance" not in output:
         raise ServiceError('Expected to find "distance" in the operation output, but it was not present.')
     kwargs["distance"] = limited_parse_float(output['distance'])
 
     return QueryResultItem(**kwargs)
 
-def _deserialize_vector(output: Document, config: Config) -> list[float]:
+def _deserialize_string_array(output: DocumentValue, config: Config) -> list[str]:
+    if not isinstance(output, list):
+        raise ServiceError(f"Expected list, found {type(output)}")
+    return [expect_type(str, e) for e in output]
+
+def _deserialize_vector(output: DocumentValue, config: Config) -> list[float]:
     if not isinstance(output, list):
         raise ServiceError(f"Expected list, found {type(output)}")
     return [limited_parse_float(e) for e in output]
```

### Comparing `svectordb-0.0.5/svectordb/serialize.py` & `svectordb-0.0.6/svectordb/serialize.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from base64 import b64encode
 import json
 from typing import AsyncIterable
 from urllib.parse import quote as urlquote
 
 from smithy_core import URI as _URI
 from smithy_core.aio.types import AsyncBytesReader
-from smithy_core.types import Document
+from smithy_core.documents import DocumentValue
 from smithy_core.utils import limited_serialize_float
 from smithy_http import Field, Fields
 from smithy_http.aio import HTTPRequest as _HTTPRequest
 from smithy_http.aio.interfaces import HTTPRequest
 
 from .config import Config
 from .errors import ServiceError
@@ -19,14 +19,19 @@
     DeleteItemInput,
     EmbedInput,
     EmbeddingInput,
     EmbeddingInputImage,
     EmbeddingInputText,
     GetItemInput,
     ListItemsInput,
+    MetadataValue,
+    MetadataValueNumber,
+    MetadataValueNumberArray,
+    MetadataValueString,
+    MetadataValueStringArray,
     QueryInput,
     QueryType,
     QueryTypeKey,
     QueryTypeVector,
     SetItemInput,
 )
 
@@ -73,15 +78,15 @@
     path = "/db/{database_id}/embed/{model}".format(
         database_id=urlquote(input.database_id, safe=''),
         model=urlquote(input.model, safe=''),
     )
     query: str = f''
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b'')
-    result: dict[str, Document] = {}
+    result: dict[str, DocumentValue] = {}
 
     if input.input is not None:
         result["input"] = _serialize_embedding_input(input.input, config)
 
     content = json.dumps(result).encode('utf-8')
     content_length = len(content)
     body = AsyncBytesReader(content)
@@ -144,22 +149,22 @@
 
     path = "/db/{database_id}/items".format(
         database_id=urlquote(input.database_id, safe=''),
     )
     query: str = f''
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b'')
-    result: dict[str, Document] = {}
-
-    if input.next_token is not None:
-        result["nextToken"] = input.next_token
+    result: dict[str, DocumentValue] = {}
 
     if input.page_size is not None:
         result["pageSize"] = input.page_size
 
+    if input.next_token is not None:
+        result["nextToken"] = input.next_token
+
     content = json.dumps(result).encode('utf-8')
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -186,21 +191,24 @@
 
     path = "/db/{database_id}/query".format(
         database_id=urlquote(input.database_id, safe=''),
     )
     query: str = f''
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b'')
-    result: dict[str, Document] = {}
+    result: dict[str, DocumentValue] = {}
+
+    if input.query is not None:
+        result["query"] = _serialize_query_type(input.query, config)
 
     if input.max_results is not None:
         result["maxResults"] = input.max_results
 
-    if input.query is not None:
-        result["query"] = _serialize_query_type(input.query, config)
+    if input.filter is not None:
+        result["filter"] = input.filter
 
     content = json.dumps(result).encode('utf-8')
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
@@ -232,22 +240,25 @@
     path = "/db/{database_id}/item/{key}".format(
         database_id=urlquote(input.database_id, safe=''),
         key=urlquote(input.key, safe=''),
     )
     query: str = f''
 
     body: AsyncIterable[bytes] = AsyncBytesReader(b'')
-    result: dict[str, Document] = {}
+    result: dict[str, DocumentValue] = {}
 
     if input.vector is not None:
         result["vector"] = input.vector
 
     if input.value is not None:
         result["value"] = b64encode(input.value).decode('utf-8')
 
+    if input.metadata is not None:
+        result["metadata"] = _serialize_metadata(input.metadata, config)
+
     content = json.dumps(result).encode('utf-8')
     content_length = len(content)
     body = AsyncBytesReader(content)
 
     headers = Fields(
         [
             Field(name="Content-Type", values=["application/json"]),
@@ -264,31 +275,54 @@
             query=query,
         ),
         method="PUT",
         fields=headers,
         body=body,
     )
 
-def _serialize_embedding_input(input: EmbeddingInput, config: Config) -> dict[str, Document]:
+def _serialize_embedding_input(input: EmbeddingInput, config: Config) -> dict[str, DocumentValue]:
     match input:
         case EmbeddingInputText():
             return {"text": input.value}
 
         case EmbeddingInputImage():
             return {"image": b64encode(input.value).decode('utf-8')}
 
         case _:
             raise ServiceError(f"Unexpected union variant: {type(input)}")
 
-def _serialize_query_type(input: QueryType, config: Config) -> dict[str, Document]:
+def _serialize_metadata(input: dict[str, MetadataValue], config: Config) -> dict[str, DocumentValue]:
+    return {k: _serialize_metadata_value(v, config) for k, v in input.items()}
+
+def _serialize_metadata_value(input: MetadataValue, config: Config) -> dict[str, DocumentValue]:
+    match input:
+        case MetadataValueString():
+            return {"string": input.value}
+
+        case MetadataValueStringArray():
+            return {"stringArray": input.value}
+
+        case MetadataValueNumber():
+            return {"number": limited_serialize_float(input.value)}
+
+        case MetadataValueNumberArray():
+            return {"numberArray": input.value}
+
+        case _:
+            raise ServiceError(f"Unexpected union variant: {type(input)}")
+
+def _serialize_number_array(input: list[float], config: Config) -> list[DocumentValue]:
+    return [limited_serialize_float(e) for e in input]
+
+def _serialize_query_type(input: QueryType, config: Config) -> dict[str, DocumentValue]:
     match input:
         case QueryTypeKey():
             return {"key": input.value}
 
         case QueryTypeVector():
             return {"vector": input.value}
 
         case _:
             raise ServiceError(f"Unexpected union variant: {type(input)}")
 
-def _serialize_vector(input: list[float], config: Config) -> list[Document]:
+def _serialize_vector(input: list[float], config: Config) -> list[DocumentValue]:
     return [limited_serialize_float(e) for e in input]
```

### Comparing `svectordb-0.0.5/svectordb.egg-info/PKG-INFO` & `svectordb-0.0.6/svectordb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: svectordb
-Version: 0.0.5
+Version: 0.0.6
 Summary: svectordb client
 License: Apache-2.0
 Keywords: smithy,svectordb
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp<3.10.0,>=3.8.6
 Provides-Extra: tests
 Requires-Dist: pytest<8.0.0,>=7.2.0; extra == "tests"
 Requires-Dist: pytest-asyncio<0.21.0,>=0.20.3; extra == "tests"
 
 ## SvectorDB Client
```

### Comparing `svectordb-0.0.5/svectordb.egg-info/SOURCES.txt` & `svectordb-0.0.6/svectordb.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 README.md
 pyproject.toml
 smithy_aws_core/__init__.py
 smithy_aws_core/identity.py
 smithy_aws_core/py.typed
 smithy_aws_core/interfaces/__init__.py
 smithy_core/__init__.py
+smithy_core/deserializers.py
+smithy_core/documents.py
 smithy_core/exceptions.py
 smithy_core/identity.py
 smithy_core/interceptors.py
+smithy_core/prelude.py
 smithy_core/py.typed
 smithy_core/retries.py
 smithy_core/rfc3986.py
+smithy_core/schemas.py
+smithy_core/serializers.py
+smithy_core/shapes.py
+smithy_core/traits.py
 smithy_core/types.py
 smithy_core/utils.py
 smithy_core/aio/__init__.py
 smithy_core/aio/types.py
 smithy_core/aio/utils.py
 smithy_core/aio/interfaces/__init__.py
 smithy_core/aio/interfaces/identity.py
 smithy_core/interfaces/__init__.py
+smithy_core/interfaces/exceptions.py
 smithy_core/interfaces/identity.py
 smithy_core/interfaces/retries.py
 smithy_http/__init__.py
 smithy_http/endpoints.py
 smithy_http/exceptions.py
 smithy_http/py.typed
 smithy_http/restjson.py
@@ -35,21 +43,25 @@
 smithy_http/aio/auth/__init__.py
 smithy_http/aio/auth/apikey.py
 smithy_http/aio/identity/__init__.py
 smithy_http/aio/identity/apikey.py
 smithy_http/aio/interfaces/__init__.py
 smithy_http/aio/interfaces/auth.py
 smithy_http/interfaces/__init__.py
+smithy_json/__init__.py
+smithy_json/py.typed
 svectordb/__init__.py
 svectordb/auth.py
 svectordb/client.py
 svectordb/config.py
 svectordb/deserialize.py
 svectordb/errors.py
 svectordb/models.py
 svectordb/serialize.py
 svectordb.egg-info/PKG-INFO
 svectordb.egg-info/SOURCES.txt
 svectordb.egg-info/dependency_links.txt
 svectordb.egg-info/requires.txt
 svectordb.egg-info/top_level.txt
+svectordb/_private/__init__.py
+svectordb/_private/schemas.py
 tests/test_protocol.py
```

### Comparing `svectordb-0.0.5/tests/test_protocol.py` & `svectordb-0.0.6/tests/test_protocol.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 # Code generated by smithy-python-codegen DO NOT EDIT.
 
-from typing import Any
-
 from smithy_core.aio.utils import async_list
-from smithy_http import Fields, tuples_to_fields
+from smithy_http import tuples_to_fields
 from smithy_http.aio import HTTPResponse as _HTTPResponse
 from smithy_http.aio.interfaces import HTTPRequest, HTTPResponse
-from smithy_http.interfaces import HTTPRequestConfiguration
+from smithy_http.interfaces import HTTPClientConfiguration, HTTPRequestConfiguration
 
 from svectordb.errors import ServiceError
 
 
 class TestHttpServiceError(ServiceError):
     """A test error that subclasses the service-error for protocol tests."""
 
     def __init__(self, request: HTTPRequest):
         self.request = request
 
 class RequestTestHTTPClient:
     """An asynchronous HTTP client solely for testing purposes."""
 
+    def __init__(self, *, client_config: HTTPClientConfiguration | None = None):
+        self._client_config = client_config
+
     async def send(
-        self, *, request: HTTPRequest, request_config: HTTPRequestConfiguration | None
+        self, *, request: HTTPRequest, request_config: HTTPRequestConfiguration | None = None
     ) -> HTTPResponse:
         # Raise the exception with the request object to bypass actual request handling
         raise TestHttpServiceError(request)
 
 class ResponseTestHTTPClient:
     """An asynchronous HTTP client solely for testing purposes."""
 
-    def __init__(self, status: int, headers: list[tuple[str, str]], body: bytes):
+    def __init__(
+        self,
+        *,
+        client_config: HTTPClientConfiguration | None = None,
+        status: int = 200,
+        headers: list[tuple[str, str]] | None = None,
+        body: bytes = b"",
+    ):
+        self._client_config = client_config
         self.status = status
-        self.fields = tuples_to_fields(headers)
+        self.fields = tuples_to_fields(headers or [])
         self.body = body
 
     async def send(
-        self, *, request: HTTPRequest, request_config: HTTPRequestConfiguration | None
+        self, *, request: HTTPRequest, request_config: HTTPRequestConfiguration | None = None
     ) -> _HTTPResponse:
         # Pre-construct the response from the request and return it
         return _HTTPResponse(
             status=self.status,
             fields=self.fields,
             body=async_list([self.body]),
         )
```

