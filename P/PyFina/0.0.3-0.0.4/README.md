# Comparing `tmp/PyFina-0.0.3.tar.gz` & `tmp/pyfina-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyFina-0.0.3.tar", last modified: Sat Sep  4 16:29:18 2021, max compression
+gzip compressed data, was "pyfina-0.0.4.tar", last modified: Wed May 29 07:56:04 2024, max compression
```

## Comparing `PyFina-0.0.3.tar` & `pyfina-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 alexandrecuer  (1000) alexandrecuer  (1000)        0 2021-09-04 16:29:18.000000 PyFina-0.0.3/
-drwxrwxr-x   0 alexandrecuer  (1000) alexandrecuer  (1000)        0 2021-09-04 16:29:18.000000 PyFina-0.0.3/PyFina/
--rw-r--r--   0 alexandrecuer  (1000) alexandrecuer  (1000)       22 2021-05-22 15:43:27.000000 PyFina-0.0.3/PyFina/__init__.py
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)     4660 2021-09-04 16:21:54.000000 PyFina-0.0.3/PyFina/PyFina.py
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)     3573 2021-09-04 16:29:18.000000 PyFina-0.0.3/PKG-INFO
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)      890 2021-09-04 16:25:26.000000 PyFina-0.0.3/setup.py
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)       38 2021-09-04 16:29:18.000000 PyFina-0.0.3/setup.cfg
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)     2265 2021-05-24 09:38:42.000000 PyFina-0.0.3/README.md
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)      104 2021-05-22 10:34:16.000000 PyFina-0.0.3/pyproject.toml
-drwxrwxr-x   0 alexandrecuer  (1000) alexandrecuer  (1000)        0 2021-09-04 16:29:18.000000 PyFina-0.0.3/PyFina.egg-info/
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)      218 2021-09-04 16:29:17.000000 PyFina-0.0.3/PyFina.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)     3573 2021-09-04 16:29:17.000000 PyFina-0.0.3/PyFina.egg-info/PKG-INFO
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)       17 2021-09-04 16:29:17.000000 PyFina-0.0.3/PyFina.egg-info/requires.txt
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)        1 2021-09-04 16:29:17.000000 PyFina-0.0.3/PyFina.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandrecuer  (1000) alexandrecuer  (1000)        7 2021-09-04 16:29:17.000000 PyFina-0.0.3/PyFina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:04.900739 pyfina-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-29 07:56:00.000000 pyfina-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-29 07:56:04.900739 pyfina-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:04.900739 pyfina-0.0.4/PyFina/
+-rw-r--r--   0 runner    (1001) docker     (127)     4999 2024-05-29 07:56:00.000000 pyfina-0.0.4/PyFina/PyFina.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-29 07:56:00.000000 pyfina-0.0.4/PyFina/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:04.900739 pyfina-0.0.4/PyFina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-05-29 07:56:04.000000 pyfina-0.0.4/PyFina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-29 07:56:04.000000 pyfina-0.0.4/PyFina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:56:04.000000 pyfina-0.0.4/PyFina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 07:56:04.000000 pyfina-0.0.4/PyFina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 07:56:04.000000 pyfina-0.0.4/PyFina.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-29 07:56:00.000000 pyfina-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 07:56:00.000000 pyfina-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:56:04.900739 pyfina-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-29 07:56:00.000000 pyfina-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:56:04.900739 pyfina-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-29 07:56:00.000000 pyfina-0.0.4/tests/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PyFina-0.0.3/PyFina/PyFina.py` & `pyfina-0.0.4/PyFina/PyFina.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,135 +1,137 @@
-import numpy as np
+"""pyfina module"""
+
 import struct
 import os
 import math
 
-def trim(id, dir, limit=100):
+import numpy as np
+
+def trim(feed_id, data_dir, limit=100):
     """
     checks and removes anomalies (values above a threshold limit, eg 100)
-    id: feed number
-    dir: feed path (eg /var/opt/emoncms/phpfina)
+    feed_id: feed number
+    data_dir: feed path (eg /var/opt/emoncms/phpfina)
     limit: threshold we don't want to exceed
     """
-    meta = getMeta(id, dir)
+    meta = getMeta(feed_id, data_dir)
     pos = 0
     i = 0
-    nbn =0
-    with open("{}/{}.dat".format(dir, id), "rb+") as ts:
+    nbn = 0
+    with open(f"{data_dir}/{feed_id}.dat", "rb+") as ts:
         while pos <= meta["npoints"]:
             ts.seek(pos*4, 0)
             hexa = ts.read(4)
             aa = bytearray(hexa)
             if len(aa) == 4:
                 value = struct.unpack('<f', aa)[0]
                 if math.isnan(value):
                     nbn +=1
                 elif value > limit:
-                    print("anomaly detected at {} : {}".format(pos, value))
+                    print(f"anomaly detected at {pos} : {value}")
                     i += 1
                     nv = struct.pack('<f', float('nan'))
                     try:
-                        ts.seek(pos*4,0)
+                        ts.seek(pos*4, 0)
                         ts.write(nv)
                     except Exception as e:
                         print(e)
                     finally:
                         print("4 bytes written")
             pos +=1
-        print("{} anomaly(ies)".format(i))
-        print("{} nan".format(nbn))
+        print(f"{i} anomaly(ies)")
+        print(f"{nbn} nan")
 
-def getMeta(id, dir):
+def getMeta(feed_id, data_dir):
     """
     decoding the .meta file
-
-    id (4 bytes, Unsigned integer)
+    feed_id (4 bytes, Unsigned integer)
     npoints (4 bytes, Unsigned integer, Legacy : use instead filesize//4 )
     interval (4 bytes, Unsigned integer)
     start_time (4 bytes, Unsigned integer)
-
     """
-    with open("{}/{}.meta".format(dir,id),"rb") as f:
+    with open(f"{data_dir}/{feed_id}.meta","rb") as f:
         f.seek(8,0)
         hexa = f.read(8)
         aa= bytearray(hexa)
         if len(aa)==8:
             decoded=struct.unpack('<2I', aa)
         else:
             print("corrupted meta - aborting")
             return False
     meta = {
-             "interval":decoded[0],
-             "start_time":decoded[1],
-             "npoints":os.path.getsize("{}/{}.dat".format(dir,id))//4
-           }
+        "interval": decoded[0],
+        "start_time": decoded[1],
+        "npoints": os.path.getsize(f"{data_dir}/{feed_id}.dat") // 4
+    }
     return meta
 
 class PyFina(np.ndarray):
-
-    def __new__(cls, id, dir, start, step, npts):
-        meta = getMeta(id, dir)
+    """ pyfina class."""
+    def __new__(cls, feed_id, data_dir, start, step, npts, remove_nan=True):
+        meta = getMeta(feed_id, data_dir)
         if not meta:
-            return
-        """
-        decoding and sampling the .dat file
-        values are 32 bit floats, stored on 4 bytes
-        to estimate value(time), position in the dat file is calculated as follow :
-        pos = (time - meta["start_time"]) // meta["interval"]
-        Nota : no NAN value - if a NAN is detected, the algorithm will fetch the first non NAN value in the future
-        """
-        verbose = False
+            return None
+        # decoding and sampling the .dat file
+        # values are 32 bit floats, stored on 4 bytes
+        # to estimate value(time), position in the dat file is calculated as follow :
+        # pos = (time - meta["start_time"]) // meta["interval"]
+        # Nota : if remove_nan is True and a NAN is detected, the algorithm takes previous value
         obj = np.zeros(npts).view(cls)
+        raw_obj = np.empty(npts)
 
         end = start + (npts-1) * step
         time = start
         i = 0
-        with open("{}/{}.dat".format(dir,id), "rb") as ts:
+        nb_nan = 0
+        with open(f"{data_dir}/{feed_id}.dat", "rb") as ts:
             while time < end:
                 time = start + step * i
                 pos = (time - meta["start_time"]) // meta["interval"]
-                if pos >=0 and pos < meta["npoints"]:
-                    #print("trying to find point {} going to index {}".format(i,pos))
-                    ts.seek(pos*4, 0)
-                    hexa = ts.read(4)
-                    aa= bytearray(hexa)
-                    if len(aa)==4:
-                      value=struct.unpack('<f', aa)[0]
-                      if not math.isnan(value):
-                          obj[i] = value
-                      else:
-                          if verbose:
-                              print("NAN at pos {} uts {}".format(pos, meta["start_time"]+pos*meta["interval"]))
-                          j=1
-                          while True:
-                              #print(j)
-                              ramble=(pos+j)*4
-                              ts.seek(ramble, 0)
-                              hexa = ts.read(4)
-                              aa= bytearray(hexa)
-                              value=struct.unpack('<f', aa)[0]
-                              if math.isnan(value):
-                                  j+=1
-                              else:
-                                  break
-                          obj[i] = value
+                if 0 <= pos < meta["npoints"]:
+                    try:
+                        #print(f"trying to find point {i} going to index {pos}")
+                        ts.seek(pos*4, 0)
+                        hexa = ts.read(4)
+                        aa= bytearray(hexa)
+                    except Exception as e:
+                        print(f"error during file operation {e}")
                     else:
-                      print("unpacking problem {} len is {} position is {}".format(i,len(aa),position))
+                        if len(aa)==4:
+                            value = struct.unpack('<f', aa)[0]
+                            obj[i] = value
+                            raw_obj[i] = value
+                            if remove_nan and np.isnan(value):
+                                nb_nan += 1
+                                obj[i] = obj[i-1]
+                        else:
+                            print(f"unpacking problem {i} len is {len(aa)} position is {pos}")
                 i += 1
-        """
-        storing the "signature" of the "sampled" feed
-        """
+        first_non_nan_value = -1
+        first_non_nan_index = -1
+        starting_by_nan = np.isnan(raw_obj[0])
+        if nb_nan < npts:
+            finiteness_obj = np.isfinite(raw_obj)
+            first_non_nan_index = np.where(finiteness_obj)[0][0]
+            first_non_nan_value = raw_obj[finiteness_obj][0]
+            if starting_by_nan and remove_nan:
+                obj[:first_non_nan_index] = np.ones(first_non_nan_index) * first_non_nan_value
+        # storing the "signature" of the "sampled" feed
         obj.start = start
         obj.step = step
-
+        obj.nb_nan = nb_nan
+        obj.first_non_nan_value = first_non_nan_value
+        obj.first_non_nan_index = first_non_nan_index
+        obj.starting_by_nan = starting_by_nan
         return obj
 
     def __array_finalize__(self, obj):
-        if obj is None: return
-        self.start = getattr(obj, 'start', None)
-        self.step = getattr(obj, 'step', None)
+        if obj is None:
+            return
+        self.start = getattr(obj, 'start', None)   # pylint: disable=W0201
+        self.step = getattr(obj, 'step', None)  # pylint: disable=W0201
 
     def timescale(self):
         """
         return the time scale of the feed as a numpy array
         """
         return np.arange(0,self.step*self.shape[0],self.step)
```

### Comparing `PyFina-0.0.3/setup.py` & `pyfina-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+"""setup."""
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyFina",
-    version="0.0.3",
+    version="0.0.4",
     author="Alexandre CUER",
     author_email="alexandre.cuer@wanadoo.fr",
     description="A numpy subclass to read emoncms PHPFINA feeds as numpy array",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Open-Building-Management/PyFina",
     project_urls={
```

### Comparing `PyFina-0.0.3/README.md` & `pyfina-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 ## Getting Started
 
 To retrieve metadatas for feed number 1 :
 
 ```
 from PyFina import getMeta, PyFina
-import matplotlib.pylab as plt
+import matplotlib.pyplot as plt
 # classic emoncms feed storage on linux
 dir = "/var/opt/emoncms/phpfina"
 meta = getMeta(1,dir)
 print(meta)
 ```
 To import the first 8 days of datas, with a sampling interval of 3600 s :
```

