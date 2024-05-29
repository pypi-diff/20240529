# Comparing `tmp/dt_utils-0.0.4.tar.gz` & `tmp/dt_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt_utils-0.0.4.tar", last modified: Tue May 28 10:31:27 2024, max compression
+gzip compressed data, was "dt_utils-0.0.5.tar", last modified: Wed May 29 02:11:47 2024, max compression
```

## Comparing `dt_utils-0.0.4.tar` & `dt_utils-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)     1210 2018-06-22 08:56:39.000000 dt_utils-0.0.4/LICENSE
--rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-28 10:31:27.701625 dt_utils-0.0.4/PKG-INFO
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)       26 2018-06-22 08:56:39.000000 dt_utils-0.0.4/README.md
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/dt_utils/
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)       88 2024-05-28 10:30:39.000000 dt_utils-0.0.4/dt_utils/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     2439 2024-05-28 10:25:08.000000 dt_utils-0.0.4/dt_utils/neat.py
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)     6798 2024-05-28 09:50:00.000000 dt_utils-0.0.4/dt_utils/parsers.py
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)      865 2018-12-05 06:33:18.000000 dt_utils-0.0.4/dt_utils/timers.py
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/dt_utils.egg-info/
--rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/PKG-INFO
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)      355 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/SOURCES.txt
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)        1 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/dependency_links.txt
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)       20 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/requires.txt
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)       15 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/top_level.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2024-05-28 10:31:27.701625 dt_utils-0.0.4/setup.cfg
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)      739 2024-05-28 10:30:39.000000 dt_utils-0.0.4/setup.py
-drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/tests/
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-07-09 10:01:02.000000 dt_utils-0.0.4/tests/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     1204 2024-05-28 10:30:13.000000 dt_utils-0.0.4/tests/test_neat.py
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2791 2024-05-28 09:52:08.000000 dt_utils-0.0.4/tests/test_parse_datetime.py
--rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2729 2024-05-28 09:05:09.000000 dt_utils-0.0.4/tests/test_parse_tdelta.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-29 02:11:47.864809 dt_utils-0.0.5/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     1210 2018-06-22 08:56:39.000000 dt_utils-0.0.5/LICENSE
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-29 02:11:47.864809 dt_utils-0.0.5/PKG-INFO
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       26 2018-06-22 08:56:39.000000 dt_utils-0.0.5/README.md
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-29 02:11:47.864809 dt_utils-0.0.5/dt_utils/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      110 2024-05-29 02:10:56.000000 dt_utils-0.0.5/dt_utils/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      240 2024-05-29 01:39:57.000000 dt_utils-0.0.5/dt_utils/common.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1471 2024-05-29 02:10:24.000000 dt_utils-0.0.5/dt_utils/format.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     2439 2024-05-28 10:25:08.000000 dt_utils-0.0.5/dt_utils/neat.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     6031 2024-05-29 02:10:34.000000 dt_utils-0.0.5/dt_utils/parsers.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      865 2018-12-05 06:33:18.000000 dt_utils-0.0.5/dt_utils/timers.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-29 02:11:47.864809 dt_utils-0.0.5/dt_utils.egg-info/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-29 02:11:47.000000 dt_utils-0.0.5/dt_utils.egg-info/PKG-INFO
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      414 2024-05-29 02:11:47.000000 dt_utils-0.0.5/dt_utils.egg-info/SOURCES.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)        1 2024-05-29 02:11:47.000000 dt_utils-0.0.5/dt_utils.egg-info/dependency_links.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       20 2024-05-29 02:11:47.000000 dt_utils-0.0.5/dt_utils.egg-info/requires.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       15 2024-05-29 02:11:47.000000 dt_utils-0.0.5/dt_utils.egg-info/top_level.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2024-05-29 02:11:47.864809 dt_utils-0.0.5/setup.cfg
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      739 2024-05-29 02:10:56.000000 dt_utils-0.0.5/setup.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-29 02:11:47.864809 dt_utils-0.0.5/tests/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-07-09 10:01:02.000000 dt_utils-0.0.5/tests/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      946 2024-05-29 02:06:28.000000 dt_utils-0.0.5/tests/test_format.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1204 2024-05-28 10:30:13.000000 dt_utils-0.0.5/tests/test_neat.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2791 2024-05-28 09:52:08.000000 dt_utils-0.0.5/tests/test_parse_datetime.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2729 2024-05-28 09:05:09.000000 dt_utils-0.0.5/tests/test_parse_tdelta.py
```

### Comparing `dt_utils-0.0.4/LICENSE` & `dt_utils-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.4/dt_utils/neat.py` & `dt_utils-0.0.5/dt_utils/neat.py`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.4/dt_utils/parsers.py` & `dt_utils-0.0.5/dt_utils/parsers.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,17 @@
 
 import six
 import re
 from datetime import datetime, timedelta, date
 from dateutil.relativedelta import relativedelta
 from dateutil.parser import parse
 import numpy as np
+from .common import return_as_type
 
-__all__ = ['parse_datetime', 'parse_timedelta', 'datetime_range', 'T', 'TD', 'TR', 'TT', 'datetime', 'timedelta', 'date', 'relativedelta']
-
-
-def _return_as_type(seq, return_type=None):
-    if return_type == 'scalar':
-        return seq[0]
-    elif return_type == 'np_arr':
-        return np.array(seq)
-    else:
-        return seq
+__all__ = ['parse_datetime', 'parse_timedelta', 'datetime_range', 'T', 'TD', 'TR', 'datetime', 'timedelta', 'date', 'relativedelta']
 
 
 def parse_datetime(timestr, force_datetime=True):
     """Try parse timestr or integer or list of str/integer into datetimes
     timestr: single value or seq of:
                 int/str: YYYYMMDD[HH[MM[SS]]] , delimiters are also allowed,
                     e.g.: YYYY-MM-DD HH:MM:SS.
@@ -86,15 +78,15 @@
                     res = datetime.strptime(numonly_str, fmtstr)
                 else:
                     res = parse(numonly_str)
             except Exception:
                 res = None
         res_list.append(res)
 
-    return _return_as_type(res_list, return_type)
+    return return_as_type(res_list, return_type)
 
 
 _tdelta_dict = {
     'd': 'days', 'h': 'hours', 'm': 'minutes', 's': 'seconds',  # legacy formats
     # pandas freq compatible
     'T': 'minutes', 'min': 'minutes',
     'H': 'hours', 'D': 'days', 'S': 'seconds',
@@ -159,15 +151,15 @@
                 key = _tdelta_dict.get(symbol)
                 if key is None:
                     res = None
                 else:
                     res = timedelta(**{key: value})
         res_list.append(res)
 
-    return _return_as_type(res_list, return_type)
+    return return_as_type(res_list, return_type)
 
 
 def datetime_range(beg, end=None, tdelta='1h'):
     """Returns a list of datetimes from beg to end with tdelta.
     """
     if end is None:
         tokens = beg.split(':')
@@ -189,32 +181,7 @@
         now = now + tdelta
     return result
 
 
 T = parse_datetime
 TD = parse_timedelta
 TR = datetime_range
-
-
-def TT(dt):
-    if isinstance(dt, (list, tuple)):
-        dts = dt
-        return_type = 'list'
-    elif isinstance(dt, np.ndarray):
-        dts = dt
-        return_type = 'np_arr'
-    else:
-        dts = [dt]
-        return_type = 'scalar'
-
-    result = []
-    for item in dts:
-        if isinstance(item, datetime):
-            result.append(item.strftime("%Y-%m-%d %H:%M:%S"))
-        elif isinstance(item, date):
-            result.append(item.strftime("%Y-%m-%d"))
-        else:
-            result.append(T(item).strftime("%Y-%m-%d %H:%M:%S"))
-
-    return _return_as_type(result, return_type)
-
-
```

### Comparing `dt_utils-0.0.4/dt_utils/timers.py` & `dt_utils-0.0.5/dt_utils/timers.py`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.4/setup.py` & `dt_utils-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 
 setuptools.setup(
     name="dt_utils",
-    version="0.0.4",
+    version="0.0.5",
     author="claydodo and his little friends (xiao huo ban)",
     author_email="claydodo@foxmail.com",
     description="Datetime utils",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/claydodo/dt_utils",
     packages=setuptools.find_packages(),
```

### Comparing `dt_utils-0.0.4/tests/test_neat.py` & `dt_utils-0.0.5/tests/test_neat.py`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.4/tests/test_parse_datetime.py` & `dt_utils-0.0.5/tests/test_parse_datetime.py`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.4/tests/test_parse_tdelta.py` & `dt_utils-0.0.5/tests/test_parse_tdelta.py`

 * *Files identical despite different names*

