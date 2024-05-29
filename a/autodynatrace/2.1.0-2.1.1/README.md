# Comparing `tmp/autodynatrace-2.1.0.tar.gz` & `tmp/autodynatrace-2.1.1.tar.gz`

## Comparing `autodynatrace-2.1.0.tar` & `autodynatrace-2.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/__about__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/__init__.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/log.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/sdk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/utils.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/aiohttp/__init__.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/aiohttp/wrapper.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/asyncio/__init__.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/asyncio/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/bottle/__init__.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/bottle/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/celery/__init__.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/celery/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/concurrent/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/concurrent/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/confluent_kafka/__init__.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/custom/__init__.py
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/custom/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/cx_Oracle/__init__.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/dbapi/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/apps.py
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/db.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/middlewares.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/utils.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/django/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/fastapi/__init__.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/fastapi/middleware.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/fastapi/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/flask/__init__.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/flask/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/grpc/__init__.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/grpc/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/paramiko/__init__.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/paramiko/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pika/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pika/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/psycopg2/__init__.py
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/psycopg2/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pymongo/__init__.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pymongo/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pysnmp/__init__.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/pysnmp/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/redis/__init__.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/redis/utils.py
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/redis/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/ruxit/__init__.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/ruxit/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/starlette/__init__.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/starlette/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/subprocess/__init__.py
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/subprocess/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/suds/__init__.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/suds/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/tornado/__init__.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/tornado/wrapper.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/urllib/__init__.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/autodynatrace/wrappers/urllib/wrapper.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/.gitignore
--rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/LICENSE
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/README.md
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 autodynatrace-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/__about__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/__init__.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/log.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/sdk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/utils.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/aiohttp/__init__.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/aiohttp/wrapper.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/asyncio/__init__.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/asyncio/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/bottle/__init__.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/bottle/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/celery/__init__.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/celery/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/concurrent/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/concurrent/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/confluent_kafka/__init__.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/custom/__init__.py
+-rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/custom/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/cx_Oracle/__init__.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/dbapi/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/__init__.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/apps.py
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/db.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/middlewares.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/utils.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/django/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/fastapi/__init__.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/fastapi/middleware.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/fastapi/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/flask/__init__.py
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/flask/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/grpc/__init__.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/grpc/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/paramiko/__init__.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/paramiko/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pika/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pika/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/psycopg2/__init__.py
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/psycopg2/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pymongo/__init__.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pymongo/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pysnmp/__init__.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/pysnmp/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/redis/__init__.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/redis/utils.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/redis/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/ruxit/__init__.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/ruxit/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/starlette/__init__.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/starlette/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/subprocess/__init__.py
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/subprocess/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/suds/__init__.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/suds/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/tornado/__init__.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/tornado/wrapper.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/urllib/__init__.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/autodynatrace/wrappers/urllib/wrapper.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/.gitignore
+-rw-r--r--   0        0        0    13107 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/README.md
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 autodynatrace-2.1.1/PKG-INFO
```

### Comparing `autodynatrace-2.1.0/autodynatrace/__init__.py` & `autodynatrace-2.1.1/autodynatrace/__init__.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/sdk.py` & `autodynatrace-2.1.1/autodynatrace/sdk.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/aiohttp/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/aiohttp/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/asyncio/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/asyncio/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/bottle/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/bottle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/celery/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/celery/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/concurrent/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/concurrent/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/confluent_kafka/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/confluent_kafka/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/custom/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/custom/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/cx_Oracle/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/cx_Oracle/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/dbapi/__init__.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/django/db.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/django/db.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/django/middlewares.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/django/middlewares.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/django/utils.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/django/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/django/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/django/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/fastapi/middleware.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/fastapi/middleware.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/fastapi/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/fastapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/flask/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/flask/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/grpc/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/grpc/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/paramiko/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/paramiko/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/pika/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/pika/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/psycopg2/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/psycopg2/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/pymongo/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/pymongo/wrapper.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,16 +37,14 @@
 
         def end(self, failed, event, message=""):
             tracer = self._tracer_dict.get(_get_tracer_dict_key(event))
             if tracer is not None:
                 if event and not isinstance(event, monitoring.CommandSucceededEvent):
                     logger.debug("Got bad pymongo event: {}".format(event))
                     tracer.mark_failed("MongoDB Command", message)
-
-                logger.debug("Ending Mongo call: {}({})@{}:{}".format(event.command_name, event.database_name, event.connection_id[0], event.connection_id[1]))
                 tracer.end()
                 self._tracer_dict.pop(_get_tracer_dict_key(event))
 
     monitoring.register(DynatraceMongoListener())
 
     def _get_tracer_dict_key(event):
         if event.connection_id is not None:
```

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/pysnmp/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/pysnmp/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/redis/utils.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/redis/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/redis/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/sqlalchemy/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/sqlalchemy/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/starlette/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/starlette/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/subprocess/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/subprocess/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/suds/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/suds/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/tornado/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/tornado/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/autodynatrace/wrappers/urllib/wrapper.py` & `autodynatrace-2.1.1/autodynatrace/wrappers/urllib/wrapper.py`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/LICENSE` & `autodynatrace-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/README.md` & `autodynatrace-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/pyproject.toml` & `autodynatrace-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autodynatrace-2.1.0/PKG-INFO` & `autodynatrace-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: autodynatrace
-Version: 2.1.0
+Version: 2.1.1
 Summary: Auto instrumentation for the OneAgent SDK
 Project-URL: Homepage, https://github.com/dlopes7/autodynatrace
 Project-URL: Issue Tracker, https://github.com/dlopes7/autodynatrace/issues
 Author-email: David Lopes <david.lopes@dynatrace.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

