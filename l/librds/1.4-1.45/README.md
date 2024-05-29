# Comparing `tmp/librds-1.4.tar.gz` & `tmp/librds-1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "librds-1.4.tar", last modified: Tue May 28 19:26:46 2024, max compression
+gzip compressed data, was "librds-1.45.tar", last modified: Wed May 29 14:26:56 2024, max compression
```

## Comparing `librds-1.4.tar` & `librds-1.45.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:26:46.615634 librds-1.4/
--rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.4/LICENCE
--rw-r--r--   0 root         (0) root         (0)     1830 2024-05-28 19:26:46.615634 librds-1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1173 2024-05-28 19:16:17.000000 librds-1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:26:46.607634 librds-1.4/librds/
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-05-28 19:16:17.000000 librds-1.4/librds/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.4/librds/af.py
--rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.4/librds/charset.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2024-05-28 19:16:17.000000 librds-1.4/librds/comfort.py
--rw-rw-rw-   0 root         (0) root         (0)     3878 2024-05-28 19:16:17.000000 librds-1.4/librds/decoder.py
--rw-rw-rw-   0 root         (0) root         (0)     6396 2024-05-28 19:16:17.000000 librds-1.4/librds/generator.py
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.4/librds/group.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-28 19:16:17.000000 librds-1.4/librds/interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:26:46.615634 librds-1.4/librds.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1830 2024-05-28 19:26:46.000000 librds-1.4/librds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      364 2024-05-28 19:26:46.000000 librds-1.4/librds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 19:26:46.000000 librds-1.4/librds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-28 19:26:46.000000 librds-1.4/librds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 19:26:46.615634 librds-1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      999 2024-05-28 19:16:17.000000 librds-1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 19:26:46.611634 librds-1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4796 2024-05-28 16:54:30.000000 librds-1.4/tests/test_decoder.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-28 16:54:30.000000 librds-1.4/tests/test_groupsequencer.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2024-05-28 19:16:17.000000 librds-1.4/tests/test_interfaces.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:26:56.544695 librds-1.45/
+-rw-rw-rw-   0 root         (0) root         (0)    35187 2024-05-27 16:08:02.000000 librds-1.45/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-05-29 14:26:56.544695 librds-1.45/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1173 2024-05-28 19:16:17.000000 librds-1.45/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:26:56.540695 librds-1.45/librds/
+-rw-rw-rw-   0 root         (0) root         (0)      293 2024-05-29 14:26:04.000000 librds-1.45/librds/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2024-05-27 16:08:02.000000 librds-1.45/librds/af.py
+-rw-rw-rw-   0 root         (0) root         (0)    17334 2024-05-27 16:08:02.000000 librds-1.45/librds/charset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2035 2024-05-29 14:26:04.000000 librds-1.45/librds/comfort.py
+-rw-rw-rw-   0 root         (0) root         (0)     3874 2024-05-29 14:26:04.000000 librds-1.45/librds/decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6626 2024-05-29 14:26:04.000000 librds-1.45/librds/generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-27 16:08:02.000000 librds-1.45/librds/group.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-28 19:16:17.000000 librds-1.45/librds/interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:26:56.544695 librds-1.45/librds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1831 2024-05-29 14:26:56.000000 librds-1.45/librds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      364 2024-05-29 14:26:56.000000 librds-1.45/librds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:26:56.000000 librds-1.45/librds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-29 14:26:56.000000 librds-1.45/librds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 14:26:56.544695 librds-1.45/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-29 14:26:04.000000 librds-1.45/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:26:56.544695 librds-1.45/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4796 2024-05-28 16:54:30.000000 librds-1.45/tests/test_decoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-28 16:54:30.000000 librds-1.45/tests/test_groupsequencer.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2024-05-28 19:16:17.000000 librds-1.45/tests/test_interfaces.py
```

### Comparing `librds-1.4/LICENCE` & `librds-1.45/LICENCE`

 * *Files identical despite different names*

### Comparing `librds-1.4/PKG-INFO` & `librds-1.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.4
+Version: 1.45
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `librds-1.4/README.md` & `librds-1.45/README.md`

 * *Files identical despite different names*

### Comparing `librds-1.4/librds/af.py` & `librds-1.45/librds/af.py`

 * *Files identical despite different names*

### Comparing `librds-1.4/librds/charset.py` & `librds-1.45/librds/charset.py`

 * *Files identical despite different names*

### Comparing `librds-1.4/librds/comfort.py` & `librds-1.45/librds/comfort.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,14 +18,34 @@
             ((year - 1900) - l) * 365.25
         ) +
         int(
             (month + 2 + l * 12) * 30.6001
         )
     )
 
+def calculate_ymd(mjd:int):
+    """Returns the same format as calculate_mjd, so you can encode and decode without any conversions"""
+    jd = mjd + 2_400_001
+    ljd = jd + 68569
+    
+    njd = int((4 * ljd / 146097))
+    ljd = ljd - int(((146097 * njd + 3) / 4))
+    
+    year = int((4000 * (ljd + 1) / 1461001))
+    ljd = ljd - int(((1461 * year / 4))) + 31
+    
+    month = int((80 * ljd / 2447))
+    
+    day = ljd - int((2447 * month / 80))
+    
+    ljd = int((month / 11));
+    month = int((month + 2 - 12 * ljd))
+    year = int((100 * (njd - 49) + year + ljd))
+    return year, (month-1), day
+
 class Groups(Enum):
     PS = 0
     PS_B = 1
     RT = 2
     RT_B = 3
     PTYN = 4
     ECC = 5
```

### Comparing `librds-1.4/librds/decoder.py` & `librds-1.45/librds/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     is_lic:bool
 @dataclass
 class DecodedGroup:
     raw_group:Group
     pi: int
     tp: bool
     pty: int
-    group: IntEnum
+    group: int
     details:Details
 class GroupDecoder:
     def _decode_0(self, group: Group, dgroup: DecodedGroup):
         segment = group.b & 3
         ta = (group.b >> 4) & 1
         ms = (group.b >> 3) & 1
         if segment == 3:
```

### Comparing `librds-1.4/librds/generator.py` & `librds-1.45/librds/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -112,21 +112,25 @@
         return Group(
             blocks.a & 0xFFFF,
             (blocks.b | 10 << 12 | (int(ab) << 4) | segment) & 0xFFFF,
             (RDSCharset.translate(get_from_list(ptyn_text,segment*4+0," "))<<8 | RDSCharset.translate(get_from_list(ptyn_text,segment*4+1," "))) & 0xFFFF,
             (RDSCharset.translate(get_from_list(ptyn_text,segment*4+2," "))<<8 | RDSCharset.translate(get_from_list(ptyn_text,segment*4+3," "))) & 0xFFFF,
             False
         )
-    def ct(basic:Group, mjd: int, hour: int, min: int, local_hour:int=None):
+    def ct(basic:Group, mjd: int, hour: int, minute: int, local_hour:int=None,local_minute:int=None):
         """This function should generator a 4A group (can't test properly, you have been warned)"""
         group = Group(
             basic.a & 0xFFFF,
             (basic.b | 4 << 12 | (mjd>>15)) & 0xffff,
             ((mjd<<1) | (hour >> 4)) & 0xffff,
-            ((hour & 0xF)<<12 | min << 6) & 0xffff,
+            ((hour & 0xF)<<12 | minute << 6) & 0xffff,
             False
         )
         if local_hour:
-            offset = local_hour - hour
+            offset_h = local_hour - hour
+            if offset_h < 0: group.d |= (1 << 5) #set the time sense bit to 1
+            if local_minute:
+                offset_m = local_minute - minute
+            else: offset_m = 0
+            offset = int((offset_m + (offset_h * 60)) / 30)
             group.d |= abs(offset)
-            if offset < 0: group.d |= (1 << 5)
         return group
```

### Comparing `librds-1.4/librds/interface.py` & `librds-1.45/librds/interface.py`

 * *Files identical despite different names*

### Comparing `librds-1.4/librds.egg-info/PKG-INFO` & `librds-1.45/librds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librds
-Version: 1.4
+Version: 1.45
 Summary: RDS Group Generator
 Home-page: https://flerken.zapto.org:1115/kuba/librds
 Author: kuba201
 Project-URL: Source, https://flerken.zapto.org:1115/kuba/librds
 Keywords: radiodatasystem,rds,broadcast_fm
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Telecommunications Industry
```

### Comparing `librds-1.4/setup.py` & `librds-1.45/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
         name="librds", 
-        version="1.4",
+        version="1.45",
         author="kuba201",
         description='RDS Group Generator',
         long_description=readme,
         long_description_content_type='text/markdown',
         packages=find_packages(),
         url="https://flerken.zapto.org:1115/kuba/librds",
         install_requires=[],
```

### Comparing `librds-1.4/tests/test_decoder.py` & `librds-1.45/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `librds-1.4/tests/test_interfaces.py` & `librds-1.45/tests/test_interfaces.py`

 * *Files identical despite different names*

