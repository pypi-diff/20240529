# Comparing `tmp/py-seal-0.0.6.tar.gz` & `tmp/py-seal-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-seal-0.0.6.tar", last modified: Tue May 28 09:38:30 2024, max compression
+gzip compressed data, was "py-seal-0.0.7.tar", last modified: Wed May 29 10:34:21 2024, max compression
```

## Comparing `py-seal-0.0.6.tar` & `py-seal-0.0.7.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.314368 py-seal-0.0.6/
--rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.6/LICENSE
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-28 09:38:30.314216 py-seal-0.0.6/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      772 2024-05-28 06:36:48.000000 py-seal-0.0.6/README.md
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309059 py-seal-0.0.6/py_seal.egg-info/
--rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/PKG-INFO
--rw-r--r--   0 yehao      (501) staff       (20)      745 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/SOURCES.txt
--rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/dependency_links.txt
--rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-28 09:38:30.000000 py-seal-0.0.6/py_seal.egg-info/top_level.txt
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309207 py-seal-0.0.6/seal/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/__init__.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309406 py-seal-0.0.6/seal/config/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/config/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      272 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/config/configuration.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.309762 py-seal-0.0.6/seal/context/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/context/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      626 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/context/context.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.310081 py-seal-0.0.6/seal/db/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.6/seal/db/connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.311073 py-seal-0.0.6/seal/db/mysql/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/mysql/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)    10004 2024-05-28 08:22:36.000000 py-seal-0.0.6/seal/db/mysql/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6593 2024-05-28 08:22:36.000000 py-seal-0.0.6/seal/db/mysql/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      774 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/db/mysql/mysql_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.311856 py-seal-0.0.6/seal/db/sqlite/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/db/sqlite/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     9437 2024-05-28 08:28:54.000000 py-seal-0.0.6/seal/db/sqlite/base_mapper.py
--rw-r--r--   0 yehao      (501) staff       (20)     6325 2024-05-28 08:29:03.000000 py-seal-0.0.6/seal/db/sqlite/chained_query.py
--rw-r--r--   0 yehao      (501) staff       (20)      369 2024-05-28 09:21:01.000000 py-seal-0.0.6/seal/db/sqlite/sqlite_connector.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.312345 py-seal-0.0.6/seal/model/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/model/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.6/seal/model/base_entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.6/seal/model/response.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.312698 py-seal-0.0.6/seal/router/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/router/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)     2204 2024-05-27 14:07:17.000000 py-seal-0.0.6/seal/router/router.py
-drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-28 09:38:30.313975 py-seal-0.0.6/seal/wrapper/
--rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 08:46:17.000000 py-seal-0.0.6/seal/wrapper/__init__.py
--rw-r--r--   0 yehao      (501) staff       (20)      735 2024-05-28 09:09:22.000000 py-seal-0.0.6/seal/wrapper/entity.py
--rw-r--r--   0 yehao      (501) staff       (20)      767 2024-05-28 09:38:16.000000 py-seal-0.0.6/seal/wrapper/singleton.py
--rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-28 09:38:30.314412 py-seal-0.0.6/setup.cfg
--rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-28 08:34:13.000000 py-seal-0.0.6/setup.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.565684 py-seal-0.0.7/
+-rw-r--r--   0 yehao      (501) staff       (20)    35148 2024-05-27 11:31:04.000000 py-seal-0.0.7/LICENSE
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-29 10:34:21.565578 py-seal-0.0.7/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      772 2024-05-29 01:33:36.000000 py-seal-0.0.7/README.md
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.558841 py-seal-0.0.7/py_seal.egg-info/
+-rw-r--r--   0 yehao      (501) staff       (20)      130 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/PKG-INFO
+-rw-r--r--   0 yehao      (501) staff       (20)      792 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/SOURCES.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        1 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/dependency_links.txt
+-rw-r--r--   0 yehao      (501) staff       (20)        5 2024-05-29 10:34:21.000000 py-seal-0.0.7/py_seal.egg-info/top_level.txt
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.558944 py-seal-0.0.7/seal/
+-rw-r--r--   0 yehao      (501) staff       (20)      516 2024-05-29 10:22:23.000000 py-seal-0.0.7/seal/__init__.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.559348 py-seal-0.0.7/seal/config/
+-rw-r--r--   0 yehao      (501) staff       (20)       41 2024-05-29 02:01:44.000000 py-seal-0.0.7/seal/config/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      376 2024-05-29 10:26:19.000000 py-seal-0.0.7/seal/config/configuration.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.559800 py-seal-0.0.7/seal/context/
+-rw-r--r--   0 yehao      (501) staff       (20)       45 2024-05-29 02:01:44.000000 py-seal-0.0.7/seal/context/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      623 2024-05-29 02:01:22.000000 py-seal-0.0.7/seal/context/context.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.560239 py-seal-0.0.7/seal/db/
+-rw-r--r--   0 yehao      (501) staff       (20)       35 2024-05-29 02:17:30.000000 py-seal-0.0.7/seal/db/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-26 00:07:28.000000 py-seal-0.0.7/seal/db/connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.561260 py-seal-0.0.7/seal/db/mysql/
+-rw-r--r--   0 yehao      (501) staff       (20)      120 2024-05-29 02:32:50.000000 py-seal-0.0.7/seal/db/mysql/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9966 2024-05-29 02:21:34.000000 py-seal-0.0.7/seal/db/mysql/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6570 2024-05-29 02:30:49.000000 py-seal-0.0.7/seal/db/mysql/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      728 2024-05-29 10:25:26.000000 py-seal-0.0.7/seal/db/mysql/mysql_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.562254 py-seal-0.0.7/seal/db/sqlite/
+-rw-r--r--   0 yehao      (501) staff       (20)      122 2024-05-29 02:34:53.000000 py-seal-0.0.7/seal/db/sqlite/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     9399 2024-05-29 02:33:53.000000 py-seal-0.0.7/seal/db/sqlite/base_mapper.py
+-rw-r--r--   0 yehao      (501) staff       (20)     6301 2024-05-29 02:34:35.000000 py-seal-0.0.7/seal/db/sqlite/chained_query.py
+-rw-r--r--   0 yehao      (501) staff       (20)      320 2024-05-29 10:25:31.000000 py-seal-0.0.7/seal/db/sqlite/sqlite_connector.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.562889 py-seal-0.0.7/seal/model/
+-rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 02:16:41.000000 py-seal-0.0.7/seal/model/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      292 2024-05-25 14:35:24.000000 py-seal-0.0.7/seal/model/base_entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      563 2024-04-03 02:38:36.000000 py-seal-0.0.7/seal/model/response.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.564389 py-seal-0.0.7/seal/router/
+-rw-r--r--   0 yehao      (501) staff       (20)       67 2024-05-29 02:13:15.000000 py-seal-0.0.7/seal/router/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)     2269 2024-05-29 10:25:19.000000 py-seal-0.0.7/seal/router/router.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.564678 py-seal-0.0.7/seal/utils/
+-rw-r--r--   0 yehao      (501) staff       (20)        0 2024-05-28 10:25:13.000000 py-seal-0.0.7/seal/utils/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      165 2024-05-29 01:31:15.000000 py-seal-0.0.7/seal/utils/str_utils.py
+drwxr-xr-x   0 yehao      (501) staff       (20)        0 2024-05-29 10:34:21.565315 py-seal-0.0.7/seal/wrapper/
+-rw-r--r--   0 yehao      (501) staff       (20)       60 2024-05-29 02:13:15.000000 py-seal-0.0.7/seal/wrapper/__init__.py
+-rw-r--r--   0 yehao      (501) staff       (20)      730 2024-05-29 01:32:54.000000 py-seal-0.0.7/seal/wrapper/entity.py
+-rw-r--r--   0 yehao      (501) staff       (20)      767 2024-05-28 09:45:30.000000 py-seal-0.0.7/seal/wrapper/singleton.py
+-rw-r--r--   0 yehao      (501) staff       (20)       38 2024-05-29 10:34:21.565722 py-seal-0.0.7/setup.cfg
+-rw-r--r--   0 yehao      (501) staff       (20)      314 2024-05-29 10:34:07.000000 py-seal-0.0.7/setup.py
```

### Comparing `py-seal-0.0.6/LICENSE` & `py-seal-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.6/README.md` & `py-seal-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.6/py_seal.egg-info/SOURCES.txt` & `py-seal-0.0.7/py_seal.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -21,10 +21,12 @@
 seal/db/sqlite/chained_query.py
 seal/db/sqlite/sqlite_connector.py
 seal/model/__init__.py
 seal/model/base_entity.py
 seal/model/response.py
 seal/router/__init__.py
 seal/router/router.py
+seal/utils/__init__.py
+seal/utils/str_utils.py
 seal/wrapper/__init__.py
 seal/wrapper/entity.py
 seal/wrapper/singleton.py
```

### Comparing `py-seal-0.0.6/seal/context/context.py` & `py-seal-0.0.7/seal/context/context.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextvars import ContextVar
 
-from seal.wrapper.singleton import singleton
+from ..wrapper.singleton import singleton
 
 page_ctx = ContextVar('page')
 
 
 @singleton
 class PageContext:
```

### Comparing `py-seal-0.0.6/seal/db/mysql/base_mapper.py` & `py-seal-0.0.7/seal/db/mysql/base_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+import abc
 from datetime import datetime
-from seal.model.base_entity import BaseEntity
 from builtins import list as _list
-from seal.context.context import WebContext
-import abc
-
-from seal.db.mysql.mysql_connector import MysqlConnector
+from ...context import WebContext
+from ...model import BaseEntity
+from .mysql_connector import MysqlConnector
 
 
 class BaseMapper(metaclass=abc.ABCMeta):
 
     def __init__(self, entity_clz):
         self.clz = entity_clz
         self.placeholder = '%s'
```

### Comparing `py-seal-0.0.6/seal/db/mysql/chained_query.py` & `py-seal-0.0.7/seal/db/mysql/chained_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
-from seal.context.context import PageContext, WebContext
-from seal.db.mysql.mysql_connector import MysqlConnector
+from ...context import PageContext, WebContext
+from .mysql_connector import MysqlConnector
 
 
 class ChainedQuery:
     def __init__(self, entity_clz, logic_delete_col: str = None):
         self.clz = entity_clz
         self.__conditions = [(logic_delete_col if logic_delete_col is not None else 'deleted', 0, '=')]
         self.__select_cols = ()
```

### Comparing `py-seal-0.0.6/seal/db/sqlite/base_mapper.py` & `py-seal-0.0.7/seal/db/sqlite/base_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+import abc
 from datetime import datetime
-from seal.model.base_entity import BaseEntity
 from builtins import list as _list
-from seal.context.context import WebContext
-from seal.db.sqlite.sqlite_connector import SqliteConnector
-import abc
+from ...context import WebContext
+from .sqlite_connector import SqliteConnector
+from ...model import BaseEntity
 
 
 class BaseMapper(metaclass=abc.ABCMeta):
 
     def __init__(self, entity_clz):
         self.clz = entity_clz
         self.placeholder = '?'
```

### Comparing `py-seal-0.0.6/seal/db/sqlite/chained_query.py` & `py-seal-0.0.7/seal/db/sqlite/chained_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
-from seal.context.context import PageContext, WebContext
-from seal.db.sqlite.sqlite_connector import SqliteConnector
+from ...context import PageContext, WebContext
+from .sqlite_connector import SqliteConnector
 
 
 class ChainedQuery:
     def __init__(self, entity_clz, logic_delete_col: str = None):
         self.clz = entity_clz
         self.__conditions = [(logic_delete_col if logic_delete_col is not None else 'deleted', 0, '=')]
         self.__select_cols = ()
```

### Comparing `py-seal-0.0.6/seal/model/response.py` & `py-seal-0.0.7/seal/model/response.py`

 * *Files identical despite different names*

### Comparing `py-seal-0.0.6/seal/router/router.py` & `py-seal-0.0.7/seal/router/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import time
 from functools import wraps
 
 import jwt
 from fastapi import FastAPI, Request, Response, HTTPException, Depends
 from starlette.middleware.cors import CORSMiddleware
-from seal.context.context import WebContext
-from seal.model.response import Response as ResponseModel
-
-jwt_key = 'melon'
+from ..context import WebContext
+from ..model import Response as ResponseModel
+from .. import get_seal
 
 
 async def verify_token(request: Request = Request):
     if request.method == 'OPTIONS' or request.url.path in ['/login/submit']:
         return None
     try:
-        payload = jwt.decode(request.headers['Authorization'], jwt_key, algorithms=["HS256"])
+        payload = jwt.decode(request.headers['Authorization'],
+                             get_seal().get_config('jwt_key'),
+                             algorithms=["HS256"])
         WebContext().set({'uid': payload['uid']})
     except Exception as e:
         print(e)
         raise HTTPException(status_code=401, detail=f"Token is invalid: {e}")
 
 
 app = FastAPI(dependencies=[Depends(verify_token)])
```

### Comparing `py-seal-0.0.6/seal/wrapper/entity.py` & `py-seal-0.0.7/seal/wrapper/entity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from boltons import strutils
+from ..utils.str_utils import snake_case
 
 
 def parametrized(decorator):
     def layer(*args, **kwargs):
         def repl(cls):
             return decorator(cls, *args, **kwargs)
 
         return repl
 
     return layer
 
 
 @parametrized
-def entity(cls, table: str = None, ignore: list[str] = None):
+def entity(cls, table: str, ignore: list[str] = None):
     def columns(exclude: list[str] = None):
         cs = [key for key in cls.model_fields if
               (exclude is None or key not in exclude) and (ignore is None or key not in ignore)]
         # print(cs)
         return cs
 
     def table_name():
         if table is not None:
             return table
-        return strutils.camel2under(cls.__name__)
+        return snake_case(cls.__name__)
 
     setattr(cls, 'columns', columns)
     setattr(cls, 'table_name', table_name)
     return cls
```

### Comparing `py-seal-0.0.6/seal/wrapper/singleton.py` & `py-seal-0.0.7/seal/wrapper/singleton.py`

 * *Files identical despite different names*

