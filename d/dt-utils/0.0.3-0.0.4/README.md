# Comparing `tmp/dt_utils-0.0.3.tar.gz` & `tmp/dt_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dt_utils-0.0.3.tar", last modified: Sat Jun 15 09:22:50 2019, max compression
+gzip compressed data, was "dt_utils-0.0.4.tar", last modified: Tue May 28 10:31:27 2024, max compression
```

## Comparing `dt_utils-0.0.3.tar` & `dt_utils-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2019-06-15 09:22:50.000000 dt_utils-0.0.3/
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       66 2018-07-09 10:00:38.000000 dt_utils-0.0.3/dt_utils/__init__.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      865 2018-12-05 06:33:18.000000 dt_utils-0.0.3/dt_utils/timers.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     6002 2019-06-15 09:21:39.000000 dt_utils-0.0.3/dt_utils/parsers.py
--rw-rw-r--   0 dodo      (1000) dodo      (1000)      417 2019-06-15 09:22:50.000000 dt_utils-0.0.3/PKG-INFO
--rw-rw-r--   0 dodo      (1000) dodo      (1000)       38 2019-06-15 09:22:50.000000 dt_utils-0.0.3/setup.cfg
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/
--rw-r--r--   0 dodo      (1000) dodo      (1000)       15 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/top_level.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      417 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 dodo      (1000) dodo      (1000)       20 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/requires.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)        1 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/dependency_links.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)      284 2019-06-15 09:22:50.000000 dt_utils-0.0.3/dt_utils.egg-info/SOURCES.txt
--rw-r--r--   0 dodo      (1000) dodo      (1000)       26 2018-06-22 08:56:39.000000 dt_utils-0.0.3/README.md
-drwxrwxr-x   0 dodo      (1000) dodo      (1000)        0 2019-06-15 09:22:50.000000 dt_utils-0.0.3/tests/
--rw-r--r--   0 dodo      (1000) dodo      (1000)        0 2018-07-09 10:01:02.000000 dt_utils-0.0.3/tests/__init__.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)     2231 2018-07-09 10:31:11.000000 dt_utils-0.0.3/tests/test_parse_datetime.py
--rw-r--r--   0 dodo      (1000) dodo      (1000)      739 2019-06-15 09:22:34.000000 dt_utils-0.0.3/setup.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     1210 2018-06-22 08:56:39.000000 dt_utils-0.0.4/LICENSE
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-28 10:31:27.701625 dt_utils-0.0.4/PKG-INFO
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       26 2018-06-22 08:56:39.000000 dt_utils-0.0.4/README.md
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/dt_utils/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       88 2024-05-28 10:30:39.000000 dt_utils-0.0.4/dt_utils/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     2439 2024-05-28 10:25:08.000000 dt_utils-0.0.4/dt_utils/neat.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     6798 2024-05-28 09:50:00.000000 dt_utils-0.0.4/dt_utils/parsers.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      865 2018-12-05 06:33:18.000000 dt_utils-0.0.4/dt_utils/timers.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/dt_utils.egg-info/
+-rw-r--r--   0 dodo      (1000) dodo      (1000)      433 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/PKG-INFO
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      355 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/SOURCES.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)        1 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/dependency_links.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       20 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/requires.txt
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)       15 2024-05-28 10:31:27.000000 dt_utils-0.0.4/dt_utils.egg-info/top_level.txt
+-rw-r--r--   0 dodo      (1000) dodo      (1000)       38 2024-05-28 10:31:27.701625 dt_utils-0.0.4/setup.cfg
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)      739 2024-05-28 10:30:39.000000 dt_utils-0.0.4/setup.py
+drwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2024-05-28 10:31:27.701625 dt_utils-0.0.4/tests/
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)        0 2018-07-09 10:01:02.000000 dt_utils-0.0.4/tests/__init__.py
+-rw-r--r--   0 dodo      (1000) dodo      (1000)     1204 2024-05-28 10:30:13.000000 dt_utils-0.0.4/tests/test_neat.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2791 2024-05-28 09:52:08.000000 dt_utils-0.0.4/tests/test_parse_datetime.py
+-rwxr-xr-x   0 dodo      (1000) dodo      (1000)     2729 2024-05-28 09:05:09.000000 dt_utils-0.0.4/tests/test_parse_tdelta.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dt_utils-0.0.3/dt_utils/timers.py` & `dt_utils-0.0.4/dt_utils/timers.py`

 * *Files identical despite different names*

### Comparing `dt_utils-0.0.3/dt_utils/parsers.py` & `dt_utils-0.0.4/dt_utils/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,19 +54,28 @@
                 res_list.append(datetime.fromordinal(timestr.toordinal()))
             else:
                 res_list.append(timestr)
             continue
         if isinstance(timestr, six.integer_types + (np.integer, )):
             timestr = str(timestr)
 
+        # handle year or year-month format like YYYY, YYYY-mm etc
+        if re.match(r'^\d{4}$', timestr):  # year
+            timestr = timestr + '0101'
+        else:
+            month_m = re.match(r'^(\d{4})([\t\n\r\f-/]*)(\d{2})$', timestr)
+            if month_m:
+                timestr = '{}{}01'.format(month_m.group(1), month_m.group(3))
+
         if len(timestr) == 10:
             if re.match(r'^\d{10}$', timestr):
                 timestr = timestr + '00'
             elif re.match(r'^\d{4}.\d{2}.\d{2}$', timestr):
                 timestr = timestr + ' 00:00:00'
+
         try:
             res = parse(timestr)
         except ValueError:
             try:
                 numonly_str = re.sub(numonly_pattern, '', timestr)
                 nl = len(numonly_str)
                 if nl >= 7:
@@ -80,39 +89,47 @@
             except Exception:
                 res = None
         res_list.append(res)
 
     return _return_as_type(res_list, return_type)
 
 
-_tdelta_dict = {'d':'days', 'h':'hours', 'm':'minutes', 's':'seconds'}
-_rel_tdelta_dict = {'Y':'years', 'M':'months', 'W':'weeks'}
+_tdelta_dict = {
+    'd': 'days', 'h': 'hours', 'm': 'minutes', 's': 'seconds',  # legacy formats
+    # pandas freq compatible
+    'T': 'minutes', 'min': 'minutes',
+    'H': 'hours', 'D': 'days', 'S': 'seconds',
+}
+_rel_tdelta_dict = {'Y': 'years', 'M': 'months', 'W': 'weeks'}
 def parse_timedelta(timestr):
     """Try parse single value or seq of timestr/integer/timedelta into timedeltas.
     e.g. parse_timedelta(['30m', '2h', '1d', '15s', '2:30', '1:12:25']).
     Y: years
     M: months
     W: weeks
-    d: days
-    h: hours
-    m: minutes
-    s: seconds (default)
+    d, D: days
+    h, H: hours
+    m, min, T: minutes
+    s, S: seconds (default)
     """
     if isinstance(timestr, (list, tuple)):
         timestrs = timestr
         return_type = 'list'
     elif isinstance(timestr, np.ndarray):
         timestrs = timestr
         return_type = 'np_arr'
     else:
         timestrs = [timestr]
         return_type = 'scalar'
 
     res_list = []
     for timestr in timestrs:
+        if timestr is None:
+            res_list.append(None)
+            continue
         if isinstance(timestr, (timedelta, relativedelta)):
             res_list.append(timestr)
             continue
         if isinstance(timestr, six.integer_types + (np.integer, )):
             timestr = str(timestr)
         timestr = timestr.strip()
 
@@ -121,26 +138,33 @@
             seconds = 0
             for i, tk in enumerate(reversed(tokens)):
                 seconds += int(tk) * (60 ** i)
             res = timedelta(seconds=seconds)
             res_list.append(res)
             continue
 
-        m = re.match(r'([-+0-9]+)([dhmsYMW]*)', timestr)
+        m = re.match(r'([-+0-9]*)([A-Za-z]*)', timestr)
         if not m:
             res = None
         else:
-            value = int(m.group(1))
+            if m.group(1) == '':
+                value = 1
+            else:
+                value = int(m.group(1))
             symbol = m.group(2)
             if symbol in _rel_tdelta_dict:
-                res = relativedelta(**{_rel_tdelta_dict[symbol]:value})
+                res = relativedelta(**{_rel_tdelta_dict[symbol]: value})
             else:
                 if symbol == '':
                     symbol = 's'
-                res = timedelta(**{_tdelta_dict[symbol]:value})
+                key = _tdelta_dict.get(symbol)
+                if key is None:
+                    res = None
+                else:
+                    res = timedelta(**{key: value})
         res_list.append(res)
 
     return _return_as_type(res_list, return_type)
 
 
 def datetime_range(beg, end=None, tdelta='1h'):
     """Returns a list of datetimes from beg to end with tdelta.
```

### Comparing `dt_utils-0.0.3/tests/test_parse_datetime.py` & `dt_utils-0.0.4/tests/test_parse_datetime.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,10 +48,19 @@
             raw_list = [dt.strftime(fmt) for dt in raw_dts]
             raw_array = np.array(raw_list)
             parsed = T(raw_array)
             self.assertEqual(type(parsed), np.ndarray)
             parsed_strlist = [dt.strftime(fmt) for dt in parsed]
             self.assertListEqual(raw_list, parsed_strlist)
 
+    def test_year_and_yearmonth(self):
+        self.assertEqual(T('2024'), datetime(year=2024, month=1, day=1))
+        self.assertEqual(T('202405'), datetime(year=2024, month=5, day=1))
+        self.assertEqual(T('2024 05'), datetime(year=2024, month=5, day=1))
+        self.assertEqual(T('2024-05'), datetime(year=2024, month=5, day=1))
+        self.assertEqual(T('2024/05'), datetime(year=2024, month=5, day=1))
+        self.assertEqual(T(2024), datetime(year=2024, month=1, day=1))
+        self.assertEqual(T(202405), datetime(year=2024, month=5, day=1))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `dt_utils-0.0.3/setup.py` & `dt_utils-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # with open("README.md", "r") as fh:
 #     long_description = fh.read()
 
 
 setuptools.setup(
     name="dt_utils",
-    version="0.0.3",
+    version="0.0.4",
     author="claydodo and his little friends (xiao huo ban)",
     author_email="claydodo@foxmail.com",
     description="Datetime utils",
     # long_description=long_description,
     # long_description_content_type="text/markdown",
     url="https://github.com/claydodo/dt_utils",
     packages=setuptools.find_packages(),
```

