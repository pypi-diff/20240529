# Comparing `tmp/remfile-0.1.8.tar.gz` & `tmp/remfile-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remfile-0.1.8.tar", last modified: Fri Oct  6 23:35:00 2023, max compression
+gzip compressed data, was "remfile-0.1.9.tar", last modified: Wed Nov  1 13:34:42 2023, max compression
```

## Comparing `remfile-0.1.8.tar` & `remfile-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-10-06 23:35:00.143684 remfile-0.1.8/
--rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.8/LICENSE
--rw-r--r--   0 magland   (1000) magland   (1000)     3576 2023-10-06 23:35:00.143684 remfile-0.1.8/PKG-INFO
--rw-rw-r--   0 magland   (1000) magland   (1000)     3203 2023-10-06 23:34:15.000000 remfile-0.1.8/README.md
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-10-06 23:35:00.143684 remfile-0.1.8/remfile/
--rw-rw-r--   0 magland   (1000) magland   (1000)      917 2023-08-08 18:43:06.000000 remfile-0.1.8/remfile/DiskCache.py
--rw-rw-r--   0 magland   (1000) magland   (1000)    13636 2023-10-06 23:27:11.000000 remfile-0.1.8/remfile/RemFile.py
--rw-r--r--   0 magland   (1000) magland   (1000)      148 2023-08-08 18:43:38.000000 remfile-0.1.8/remfile/__init__.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-10-06 23:35:00.143684 remfile-0.1.8/remfile.egg-info/
--rw-r--r--   0 magland   (1000) magland   (1000)     3576 2023-10-06 23:35:00.000000 remfile-0.1.8/remfile.egg-info/PKG-INFO
--rw-r--r--   0 magland   (1000) magland   (1000)      259 2023-10-06 23:35:00.000000 remfile-0.1.8/remfile.egg-info/SOURCES.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-10-06 23:35:00.000000 remfile-0.1.8/remfile.egg-info/dependency_links.txt
--rw-r--r--   0 magland   (1000) magland   (1000)       20 2023-10-06 23:35:00.000000 remfile-0.1.8/remfile.egg-info/requires.txt
--rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-10-06 23:35:00.000000 remfile-0.1.8/remfile.egg-info/top_level.txt
--rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-10-06 23:35:00.143684 remfile-0.1.8/setup.cfg
--rw-rw-r--   0 magland   (1000) magland   (1000)      764 2023-10-06 23:34:21.000000 remfile-0.1.8/setup.py
-drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-10-06 23:35:00.143684 remfile-0.1.8/tests/
--rw-rw-r--   0 magland   (1000) magland   (1000)     2961 2023-08-17 11:22:32.000000 remfile-0.1.8/tests/test_main.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-11-01 13:34:42.979996 remfile-0.1.9/
+-rw-rw-r--   0 magland   (1000) magland   (1000)    11357 2023-08-07 12:41:38.000000 remfile-0.1.9/LICENSE
+-rw-r--r--   0 magland   (1000) magland   (1000)     3576 2023-11-01 13:34:42.979996 remfile-0.1.9/PKG-INFO
+-rw-rw-r--   0 magland   (1000) magland   (1000)     3203 2023-11-01 13:33:07.000000 remfile-0.1.9/README.md
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-11-01 13:34:42.979996 remfile-0.1.9/remfile/
+-rw-rw-r--   0 magland   (1000) magland   (1000)      917 2023-08-08 18:43:06.000000 remfile-0.1.9/remfile/DiskCache.py
+-rw-rw-r--   0 magland   (1000) magland   (1000)    13900 2023-11-01 13:33:07.000000 remfile-0.1.9/remfile/RemFile.py
+-rw-r--r--   0 magland   (1000) magland   (1000)      148 2023-08-08 18:43:38.000000 remfile-0.1.9/remfile/__init__.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-11-01 13:34:42.979996 remfile-0.1.9/remfile.egg-info/
+-rw-r--r--   0 magland   (1000) magland   (1000)     3576 2023-11-01 13:34:42.000000 remfile-0.1.9/remfile.egg-info/PKG-INFO
+-rw-r--r--   0 magland   (1000) magland   (1000)      259 2023-11-01 13:34:42.000000 remfile-0.1.9/remfile.egg-info/SOURCES.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        1 2023-11-01 13:34:42.000000 remfile-0.1.9/remfile.egg-info/dependency_links.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)       20 2023-11-01 13:34:42.000000 remfile-0.1.9/remfile.egg-info/requires.txt
+-rw-r--r--   0 magland   (1000) magland   (1000)        8 2023-11-01 13:34:42.000000 remfile-0.1.9/remfile.egg-info/top_level.txt
+-rw-rw-r--   0 magland   (1000) magland   (1000)       38 2023-11-01 13:34:42.979996 remfile-0.1.9/setup.cfg
+-rw-rw-r--   0 magland   (1000) magland   (1000)      764 2023-11-01 13:34:17.000000 remfile-0.1.9/setup.py
+drwxrwxr-x   0 magland   (1000) magland   (1000)        0 2023-11-01 13:34:42.979996 remfile-0.1.9/tests/
+-rw-rw-r--   0 magland   (1000) magland   (1000)     2961 2023-08-17 11:22:32.000000 remfile-0.1.9/tests/test_main.py
```

### Comparing `remfile-0.1.8/LICENSE` & `remfile-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `remfile-0.1.8/PKG-INFO` & `remfile-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.8
+Version: 0.1.9
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Home-page: https://github.com/magland/remfile
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -33,29 +33,29 @@
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
-Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## Installation
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
 The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
-Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## How?
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Disk caching
```

### Comparing `remfile-0.1.8/README.md` & `remfile-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
-Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## Installation
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
 The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
-Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## How?
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Disk caching
```

### Comparing `remfile-0.1.8/remfile/DiskCache.py` & `remfile-0.1.9/remfile/DiskCache.py`

 * *Files identical despite different names*

### Comparing `remfile-0.1.8/remfile/RemFile.py` & `remfile-0.1.9/remfile/RemFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union, Any
 import time
 from concurrent.futures import ThreadPoolExecutor
 import requests
 from .DiskCache import DiskCache
 
 default_min_chunk_size = 100 * 1024
-default_max_cache_size = 1e8
+default_max_cache_size = 1e9
 default_chunk_increment_factor = 1.7
 default_bytes_per_thread = 4 * 1024 * 1024
 default_max_threads = 3
 
 class RemFile:
     def __init__(self,
         url: Union[str, Any], *,
@@ -109,15 +109,19 @@
         self._position += size
 
         # clean up the cache
         if len(self._chunk_indices) > self._max_chunks_in_cache:
             if self._verbose:
                 print("Cleaning up cache")
             for chunk_index in self._chunk_indices[:int(self._max_chunks_in_cache * 0.5)]:
-                del self._chunks[chunk_index]
+                if chunk_index in self._chunks:
+                    del self._chunks[chunk_index]
+                else:
+                    # it is possible that the chunk was already deleted (repeated chunk index in the list)
+                    pass
             self._chunk_indices = self._chunk_indices[int(self._max_chunks_in_cache * 0.5):]
 
         return ret
     
     def _load_chunk(self, chunk_index: int):
         """Load a chunk of the file.
 
@@ -145,15 +149,15 @@
             # make sure the chunk sequence length is valid
             for j in range(1, self._smart_loader_chunk_sequence_length):
                 if chunk_index + j in self._chunks:
                     # already loaded this chunk
                     self._smart_loader_chunk_sequence_length = j
                     break
         else:
-            self._smart_loader_chunk_sequence_length = 1
+            self._smart_loader_chunk_sequence_length = round(self._smart_loader_chunk_sequence_length / 1.7 + 0.5)
         data_start = chunk_index * self._min_chunk_size
         data_end = data_start + self._min_chunk_size * self._smart_loader_chunk_sequence_length - 1
         if self._verbose:
             print(f"Loading {self._smart_loader_chunk_sequence_length} chunks starting at {chunk_index} ({(data_end - data_start + 1)/1e6} million bytes)")
         if data_end >= self.length:
             data_end = self.length - 1
         x = _get_bytes(
```

### Comparing `remfile-0.1.8/remfile.egg-info/PKG-INFO` & `remfile-0.1.9/remfile.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remfile
-Version: 0.1.8
+Version: 0.1.9
 Summary: File-like object from url of remote file, optimized for use with h5py.
 Home-page: https://github.com/magland/remfile
 Author: Jeremy Magland
 Author-email: jmagland@flatironinstitute.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
@@ -33,29 +33,29 @@
 
 with h5py.File(file, 'r') as f:
     print(f['/'].keys())
 ```
 
 See [examples/example1.py](examples/example1.py) for a more complete example.
 
-Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Note: url can either be a string or an object that has a get_url() method. The latter is useful if the url is a presigned AWS URL that expires after a certain amount of time. However, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## Installation
 
 ```bash
 pip install remfile
 ```
 
 ## Why?
 
 The conventional way of reading a remote hdf5 file is to use the fsspec library as in [examples/example1_compare_fsspec.py](examples/example1_compare_fsspec.py). However, this approach is empirically much slower than using remfile. I am not familiar with the inner workings of fsspec, but it does not seem to be optimized for reading hdf5 files. Efficient access of remote hdf5 files requires reading small chunks of data to obtain meta information, and then large chunks of data, and parallelization, to obtain the larger data arrays.
 
 See a timing comparison betweeen remfile and fsspec in the examples directory.
 
-Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary!
+Furthermore, since the url can be an object with a get_url() method, it is possible to use remfile in a context where presigned URLs need to be renewed. As mentioned above, if you implement your own get_url() method, make sure it renews the signed URL only when necessary.
 
 ## How?
 
 A file-like object is created that reads the remote file in chunks using the requests library. A relatively small default chunk size is used, but when the system detects that a large data array is being accessed, it switches to a larger chunk size. For very large data arrays, the system will use multiple threads to read the data in parallel.
 
 ## Disk caching
```

### Comparing `remfile-0.1.8/setup.py` & `remfile-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README.md
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 setup(
     name='remfile',
     version=__version__,
     author="Jeremy Magland",
     author_email="jmagland@flatironinstitute.org",
     url="https://github.com/magland/remfile",
```

### Comparing `remfile-0.1.8/tests/test_main.py` & `remfile-0.1.9/tests/test_main.py`

 * *Files identical despite different names*

