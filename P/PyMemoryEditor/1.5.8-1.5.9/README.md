# Comparing `tmp/pymemoryeditor-1.5.8.tar.gz` & `tmp/pymemoryeditor-1.5.9.tar.gz`

## Comparing `pymemoryeditor-1.5.8.tar` & `pymemoryeditor-1.5.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/requirements.txt
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/enums.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/errors.py
--rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/linux/functions.py
--rw-r--r--   0        0        0     5586 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/linux/process.py
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/linux/types.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/linux/ptrace/__init__.py
--rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/linux/ptrace/enums.py
--rw-r--r--   0        0        0     5176 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/process/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/process/errors.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/process/info.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/process/util.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/sample/application.py
--rw-r--r--   0        0        0    17280 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/sample/main_application_window.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/sample/open_process_window.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/util/__init__.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/util/scan.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/util/search/abstract.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/util/search/kmp.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/functions.py
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/process.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/types.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/__init__.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_allocation_states.py
--rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_protections.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/process_operations.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/standard_access_rights.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/__init__.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/open_process.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/__init__.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/errors.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/util.py
--rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/functions.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/types.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/util.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/__init__.py
--rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_allocation_states.py
--rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_protections.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_types.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/process_operations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/scan_types.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/standard_access_rights.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/tests/package.py
--rw-r--r--   0        0        0    10006 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/tests/test_editor.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/LICENSE
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/README.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/pyproject.toml
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/requirements.txt
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/__init__.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/enums.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/errors.py
+-rw-r--r--   0        0        0     8532 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/linux/functions.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/linux/process.py
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/linux/types.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/linux/ptrace/__init__.py
+-rw-r--r--   0        0        0     5327 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/linux/ptrace/enums.py
+-rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/process/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/process/errors.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/process/info.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/process/util.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/sample/application.py
+-rw-r--r--   0        0        0    17113 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/sample/main_application_window.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/sample/open_process_window.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/util/__init__.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/util/scan.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/util/search/abstract.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/util/search/kmp.py
+-rw-r--r--   0        0        0    11006 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/functions.py
+-rw-r--r--   0        0        0     8510 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/process.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/types.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/__init__.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_allocation_states.py
+-rw-r--r--   0        0        0     6742 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_protections.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_types.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/process_operations.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/standard_access_rights.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/__init__.py
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/open_process.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/errors.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/util.py
+-rw-r--r--   0        0        0     8302 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/functions.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/types.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/util.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/__init__.py
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_allocation_states.py
+-rw-r--r--   0        0        0     6600 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_protections.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_types.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/process_operations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/scan_types.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/standard_access_rights.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/tests/package.py
+-rw-r--r--   0        0        0    12275 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/tests/test_editor.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/LICENSE
+-rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/README.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0     6725 2020-02-02 00:00:00.000000 pymemoryeditor-1.5.9/PKG-INFO
```

### Comparing `pymemoryeditor-1.5.8/.github/workflows/python-package.yml` & `pymemoryeditor-1.5.9/.github/workflows/python-package.yml`

 * *Files 11% similar despite different names*

```diff
@@ -30,11 +30,11 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -r requirements.txt
     - name: Test with pytest
       run: |
-        pytest tests -v -s
+        pytest tests -v -s -x
     - name: Install package
       run: |
         pip install PyMemoryEditor
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/__init__.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Multi-platform library developed with ctypes for reading, writing and
 searching process memory, in a simple and friendly way with Python 3.
 
 The package supports Windows and Linux (32-bit and 64-bit).
 """
 
 __author__ = "Jean Loui Bernard Silva de Jesus"
-__version__ = "1.5.8"
+__version__ = "1.5.9"
 
 
 from .enums import ScanTypesEnum
 import sys
 
 # For Windows.
 if "win" in sys.platform:
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/linux/functions.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/linux/functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # Read more about process_vm_(read/write)v here:
 # https://man7.org/linux/man-pages/man2/process_vm_readv.2.html
 
 # Read more about proc and memory mapping here:
 # https://man7.org/linux/man-pages/man5/proc.5.html
 
 from ctypes import addressof, sizeof
-from typing import Generator, Tuple, Type, TypeVar, Union
+from typing import Dict, Generator, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 from ..enums import ScanTypesEnum
-from ..util import get_c_type_of, scan_memory, scan_memory_for_exact_value
+from ..util import convert_from_bytearray, get_c_type_of, scan_memory, scan_memory_for_exact_value
 from .ptrace import libc
 from .types import MEMORY_BASIC_INFORMATION, iovec
 
 import ctypes
 
 
 T = TypeVar("T")
@@ -63,18 +63,18 @@
 
     data = get_c_type_of(pytype, bufflength)
 
     libc.process_vm_readv(
         pid, (iovec * 1)(iovec(addressof(data), sizeof(data))),
         1, (iovec * 1)(iovec(address, sizeof(data))), 1, 0
     )
-    return str(data.value) if pytype is str else data.value
+    return data.value.decode() if pytype is str else data.value
 
 
-def search_all_memory(
+def search_addresses_by_value(
     pid: int,
     pytype: Type[T],
     bufflength: int,
     value: Union[bool, int, float, str, bytes, tuple],
     scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
     progress_information: bool = False,
     writeable_only: bool = False,
@@ -143,14 +143,78 @@
             }
             yield (found_address, extra_information) if progress_information else found_address
 
         # Compute the region size to the checked memory size.
         checked_memory_size += size
 
 
+def search_values_by_addresses(
+    pid: int,
+    pytype: Type[T],
+    bufflength: int,
+    addresses: Sequence[int],
+    *,
+    memory_regions: Optional[Sequence[Dict]] = None,
+    raise_error: bool = False,
+) -> Generator[Tuple[int, Optional[T]], None, None]:
+    """
+    Search the whole memory space, accessible to the process,
+    for the provided list of addresses, returning their values.
+    """
+    if pytype not in [bool, int, float, str, bytes]:
+        raise ValueError("The type must be bool, int, float, str or bytes.")
+
+    memory_regions = list(memory_regions) if memory_regions else list()
+    addresses = sorted(addresses)
+
+    # If no memory page has been given, get all readable memory pages.
+    if not memory_regions:
+        for region in get_memory_regions(pid):
+            if not b"r" in region["struct"].Privileges: continue
+            memory_regions.append(region)
+
+    memory_regions.sort(key=lambda region: region["address"])
+    address_index = 0
+
+    # Walk by each memory region.
+    for region in memory_regions:
+        if address_index >= len(addresses): continue
+
+        target_address = addresses[address_index]
+
+        # Check if the memory region contains the target address.
+        base_address, size = region["address"], region["size"]
+        if not (base_address <= target_address < base_address + size): continue
+
+        region_data = (ctypes.c_byte * size)()
+
+        # Get data from the region.
+        libc.process_vm_readv(
+            pid, (iovec * 1)(iovec(addressof(region_data), sizeof(region_data))),
+            1, (iovec * 1)(iovec(base_address, sizeof(region_data))), 1, 0
+        )
+
+        # Get the value of each address.
+        while base_address <= target_address < base_address + size:
+            offset = target_address - base_address
+            address_index += 1
+
+            try:
+                data = region_data[offset: offset + bufflength]
+                data = (ctypes.c_byte * bufflength)(*data)
+                yield target_address, convert_from_bytearray(data, pytype, bufflength)
+
+            except Exception as error:
+                if raise_error: raise error
+                yield target_address, None
+
+            if address_index >= len(addresses): break
+            target_address = addresses[address_index]
+
+
 def write_process_memory(
     pid: int,
     address: int,
     pytype: Type[T],
     bufflength: int,
     value: Union[bool, int, float, str, bytes]
 ) -> T:
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/linux/process.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/linux/process.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # -*- coding: utf-8 -*-
 
 from ..enums import ScanTypesEnum
 from ..errors import ClosedProcess
 from ..process import AbstractProcess
-from .functions import get_memory_regions, read_process_memory, search_all_memory, write_process_memory
-from typing import Generator, Optional, Tuple, Type, TypeVar, Union
+from .functions import (
+    get_memory_regions,
+    read_process_memory,
+    search_addresses_by_value,
+    search_values_by_addresses,
+    write_process_memory
+)
+from typing import Generator, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 
 T = TypeVar("T")
 
 
 class LinuxProcess(AbstractProcess):
     """
@@ -64,14 +70,29 @@
         :param pytype: type of the value to be received (bool, int, float, str or bytes).
         :param bufflength: value size in bytes (1, 2, 4, 8).
         """
         if self.__closed: raise ClosedProcess()
 
         return read_process_memory(self.pid, address, pytype, bufflength)
 
+    def search_by_addresses(
+        self,
+        pytype: Type[T],
+        bufflength: int,
+        addresses: Sequence[int],
+        *,
+        raise_error: bool = False,
+    ) -> Generator[Tuple[int, Optional[T]], None, None]:
+        """
+        Search the whole memory space, accessible to the process,
+        for the provided list of addresses, returning their values.
+        """
+        if self.__closed: raise ClosedProcess()
+        return search_values_by_addresses(self.pid, pytype, bufflength, addresses, raise_error=raise_error)
+
     def search_by_value(
         self,
         pytype: Type[T],
         bufflength: int,
         value: Union[bool, int, float, str, bytes],
         scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
         *,
@@ -90,15 +111,15 @@
         :param writeable_only: if True, search only at writeable memory regions.
         """
         if self.__closed: raise ClosedProcess()
 
         if scan_type in [ScanTypesEnum.VALUE_BETWEEN, ScanTypesEnum.NOT_VALUE_BETWEEN]:
             raise ValueError("Use the method search_by_value_between(...) to search within a range of values.")
 
-        return search_all_memory(self.pid, pytype, bufflength, value, scan_type, progress_information, writeable_only)
+        return search_addresses_by_value(self.pid, pytype, bufflength, value, scan_type, progress_information, writeable_only)
 
     def search_by_value_between(
         self,
         pytype: Type[T],
         bufflength: int,
         start: Union[bool, int, float, str, bytes],
         end: Union[bool, int, float, str, bytes],
@@ -118,15 +139,15 @@
         :param not_between: if True, return only addresses of values that are NOT within the range.
         :param progress_information: if True, a dictionary with the progress information will be return.
         :param writeable_only: if True, search only at writeable memory regions.
         """
         if self.__closed: raise ClosedProcess()
 
         scan_type = ScanTypesEnum.NOT_VALUE_BETWEEN if not_between else ScanTypesEnum.VALUE_BETWEEN
-        return search_all_memory(self.pid, pytype, bufflength, (start, end), scan_type, progress_information, writeable_only)
+        return search_addresses_by_value(self.pid, pytype, bufflength, (start, end), scan_type, progress_information, writeable_only)
 
     def write_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int,
         value: Union[bool, int, float, str, bytes]
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/linux/types.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/linux/types.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/linux/ptrace/__init__.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/linux/ptrace/__init__.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/linux/ptrace/enums.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/linux/ptrace/enums.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/process/__init__.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/process/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from abc import ABC, abstractmethod
-from typing import Generator, Optional, Tuple, Type, TypeVar, Union
+from typing import Generator, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 from ..enums import ScanTypesEnum
 from ..process.info import ProcessInfo
 
 
 T = TypeVar("T")
 
@@ -58,14 +58,29 @@
         """
         Generates dictionaries with the address, size and other
         information of each memory region used by the process.
         """
         raise NotImplementedError()
 
     @abstractmethod
+    def search_by_addresses(
+        self,
+        pytype: Type[T],
+        bufflength: int,
+        addresses: Sequence[int],
+        *,
+        raise_error: bool = False,
+    ) -> Generator[Tuple[int, Optional[T]], None, None]:
+        """
+        Search the whole memory space, accessible to the process,
+        for the provided list of addresses, returning their values.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
     def search_by_value(
         self,
         pytype: Type[T],
         bufflength: int,
         value: Union[bool, int, float, str, bytes],
         scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
         *,
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/process/errors.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/process/info.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/process/info.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/process/util.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/sample/main_application_window.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/sample/main_application_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     }
 
     def __init__(self, process: AbstractProcess):
         super().__init__()
         self.__process = process
 
         self.__scan_type = ScanTypesEnum.EXACT_VALUE
-        self.__value = 0
         self.__value_type = int
         self.__value_length = 4
         self.__addresses = []
 
         self.__updating = False  # Indicate the application is updating the values of the found addresses.
         self.__scanning = False  # Indicate a scan has started.
 
@@ -207,17 +206,15 @@
                 raise ValueError()
         except:
             self.__value_entry.delete(0, "end")
             return self.__value_entry.insert(0, "Invalid value")
 
         # Start the scan.
         value = pytype(value)
-
         self.__value_length = length
-        self.__value = value
 
         self.after(100, lambda: self.__start_scan(pytype, length, value, scan_type))
 
     def __next_scan(self):
         """
         Filter the found addresses.
         """
@@ -284,22 +281,24 @@
         self.__scanning = True
         self.__addresses = []
 
         for address, info in self.__process.search_by_value(pytype, length, value, scan_type, progress_information=True):
             if self.__close: break
 
             self.__address_list.insert("end", f"Addr: {hex(address)[2:].upper()}")
-            self.__value_list.insert("end", f"Value: {value}")
+            self.__value_list.insert("end", f"Value: loading...")
 
             self.__progress_var.set(info["progress"] * 100)
             self.__addresses.append(address)
             self.update()
 
             self.__count_label.config(text=f"Found {len(self.__addresses)} addresses.")
 
+        self.__update_values()
+
         self.__new_scan_button.config(text="New Scan")
         self.__next_scan_button.config(text="Next Scan")
         self.__progress_var.set(100)
 
     def __set_scan_type(self, scan_type: int):
         """
         Method for the Menubutton to select a scan type.
@@ -340,81 +339,75 @@
         """
         Method to validate if an input is hexadecimal.
         """
         for char in string.upper():
             if char not in "0123456789ABCDEF": return False
         return True
 
-    def __update_values(self, index = 0, *, remove = False, first_call = True):
+    def __update_values(self, *, remove: bool = False):
         """
         Update the values of the found addresses. If "remove" is True, it will
         compare the current value in memory and remove the address from the
         results if the comparison is False.
         """
-        if self.__updating and first_call: return  # Allow call the method once.
+        if self.__updating: return
 
-        # Return if user asked for closing the application.
-        if self.__close:
-            self.__updating = False
-            return
+        if not self.__addresses: return self.__progress_var.set(100)
 
         # Get the value to compare.
-        if first_call:
-            value = self.__value_entry.get().strip()
+        value = self.__value_entry.get().strip()
+        total = len(self.__addresses)
 
-            try:
-                if str(self.__value_type(value)) != value:
-                    raise ValueError()
-            except:
-                self.__value_entry.delete(0, "end")
-                return self.__value_entry.insert(0, "Invalid value")
+        try:
+            if str(self.__value_type(value)) != value:
+                raise ValueError()
+        except:
+            self.__value_entry.delete(0, "end")
+            return self.__value_entry.insert(0, "Invalid value")
 
-            self.__value = self.__value_type(value)
-            self.__progress_var.set(0)
+        self.__value = self.__value_type(value)
+        self.__progress_var.set(0)
 
         # Indicate the application is updating the values.
         self.__updating = True
 
-        if index % 10 == 0: self.update()
+        new_scan_button_text = self.__new_scan_button["text"]
+        self.__new_scan_button.config(text="Updating")
 
-        # Get the address from the list.
-        try:
-            address = self.__addresses[index]
-        except:
-            self.__updating = False
+        # Get the address and its current value in memory.
+        total, count = len(self.__addresses), 0
 
-            self.__count_label.config(text=f"Found {len(self.__addresses)} addresses.")
-            return self.__progress_var.set(100 if not first_call else 0)
-
-        # Get the current value of the address.
-        corrupted = False
-        value = None
+        for address, value in self.__process.search_by_addresses(self.__value_type, self.__value_length, self.__addresses):
+            self.__progress_var.set((count / total) * 100)
+            self.update()
 
-        try: value = self.__process.read_process_memory(address, self.__value_type, self.__value_length)
-        except: corrupted = True
+            index = self.__addresses.index(address)
+            count += 1
 
-        # If "remove" is True, compare the value.
-        if remove or corrupted:
-            compare = self.__comp_methods[self.__scan_type]
+            # Return if user asked for closing the application.
+            if self.__close:
+                self.__updating = False
+                return
 
-            # Remove the address from the results.
-            if corrupted or not compare(value, self.__value):
+            # If value is corrupted or "remove" is True and comparison is False, remove the value from the results.
+            if value is None or (remove and not self.__comp_methods[self.__scan_type](value, self.__value)):
                 self.__address_list.delete(index)
                 self.__value_list.delete(index)
                 self.__addresses.remove(address)
-                index -= 1
 
-        # Update the value at the listbox.
-        else:
-            self.__value_list.delete(index)
-            self.__value_list.insert(index, f"Value: {value}")
-
-        # Call the method again recursively
-        if index % 10 == 0: self.__progress_var.set((index / len(self.__addresses)) * 100)
-        self.after(5, lambda: self.__update_values(index + 1, remove=remove, first_call=False))
+            # Update the value at the listbox.
+            else:
+                self.__value_list.delete(index)
+                self.__value_list.insert(index, f"Value: {value}")
+
+        self.__new_scan_button.config(text=new_scan_button_text)
+        self.__updating = False
+
+        self.__count_label.config(text=f"Found {len(self.__addresses)} addresses.")
+        self.__progress_var.set(100)
 
     def __write_value(self):
         """
         Change the value in memory of an address of the result list.
         """
         try:
             address = int(self.__address_entry.get().strip(), 16)
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/sample/open_process_window.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/sample/open_process_window.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/util/__init__.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 
-from .scan import scan_memory, scan_memory_for_exact_value
 from typing import Type
 import ctypes
 
 
 def get_c_type_of(pytype: Type, length: int = 1) -> ctypes._SimpleCData:
     """
     Return a C type of a primitive type of the Python language.
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/util/scan.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/util/scan.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/util/search/kmp.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/util/search/kmp.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/functions.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/functions.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 
 # Read more about operations with processes by win32 api here:
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
-from ..enums import ScanTypesEnum
-from ..util import get_c_type_of, scan_memory, scan_memory_for_exact_value
-
-from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum
+from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum, ScanTypesEnum
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
-
-from typing import Generator, Tuple, Type, TypeVar, Union
+from .util import get_c_type_of
+from typing import Generator, Optional, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
+import sys
 
 # Load the libraries.
 kernel32 = ctypes.windll.LoadLibrary("kernel32.dll")
 user32 = ctypes.windll.LoadLibrary("user32.dll")
 
 # Set the argtypes to prevent ArgumentError.
 kernel32.VirtualQueryEx.argtypes = (
@@ -123,86 +121,81 @@
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
     data = get_c_type_of(pytype, bufflength)
     kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(data), bufflength, None)
 
-    return data.value.decode() if pytype is str else data.value
+    return str(data.value) if pytype is str else data.value
 
 
 def SearchAllMemory(
     process_handle: int,
     pytype: Type[T],
     bufflength: int,
-    value: Union[bool, int, float, str, bytes, tuple],
+    value: Union[bool, int, float, str, bytes],
     scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
-    progress_information: bool = False,
-    writeable_only: bool = False,
+    progress_information: Optional[bool] = False,
 ) -> Generator[Union[int, Tuple[int, dict]], None, None]:
     """
     Search the whole memory space, accessible to the process,
     for the provided value, returning the found addresses.
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
-    # Convert the target value, or all values of a tuple, as bytes.
-    target_values = value if isinstance(value, tuple) else (value,)
-
-    conversion_buffer = list()
+    # Get the target value as bytes.
+    target_value = get_c_type_of(pytype, bufflength)
+    target_value.value = value
 
-    for v in target_values:
-        target_value = get_c_type_of(pytype, bufflength)
-        target_value.value = v.encode() if isinstance(v, str) else v
+    target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
+    target_value_bytes = int.from_bytes(bytes(target_value_bytes.contents), sys.byteorder)
 
-        target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
-        conversion_buffer.append(bytes(target_value_bytes.contents))
-
-    target_value_bytes = tuple(conversion_buffer) if isinstance(value, tuple) else conversion_buffer[0]
-
-    # Get the memory regions, computing the total amount of memory to be scanned.
-    checked_memory_size = 0
-    memory_total = 0
     regions = list()
+    memory_total = 0
 
+    # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
         # Only committed, non-shared and readable memory pages.
         if region["struct"].State != MemoryAllocationStatesEnum.MEM_COMMIT.value: continue
         if region["struct"].Type != MemoryTypesEnum.MEM_PRIVATE.value: continue
         if region["struct"].Protect & MemoryProtectionsEnum.PAGE_READABLE.value == 0: continue
 
-        # If writeable_only is True, checks if the memory page is writeable.
-        if writeable_only and region["struct"].Protect & MemoryProtectionsEnum.PAGE_READWRITEABLE.value == 0: continue
-
         memory_total += region["size"]
         regions.append(region)
 
+    checked_memory_size = 0
+
     # Check each memory region used by the process.
     for region in regions:
         address, size = region["address"], region["size"]
         region_data = (ctypes.c_byte * size)()
 
         # Get data from the region.
         kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(region_data), size, None)
 
-        # Choose the searching method.
-        searching_method = scan_memory
-
-        if scan_type in [ScanTypesEnum.EXACT_VALUE, ScanTypesEnum.NOT_EXACT_VALUE]:
-            searching_method = scan_memory_for_exact_value
+        # Walk by the returned bytes, searching for the target value.
+        for index in range(size - bufflength):
+            data = region_data[index: index + bufflength]
+            data = int.from_bytes(bytes((ctypes.c_byte * bufflength)(*data)), sys.byteorder)
+
+            # Compare the values.
+            if scan_type is ScanTypesEnum.EXACT_VALUE and data != target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.NOT_EXACT_VALUE and data == target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.BIGGER_THAN and data <= target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.SMALLER_THAN and data >= target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.BIGGER_THAN_OR_EXACT_VALUE and data < target_value_bytes: continue
+            elif scan_type is ScanTypesEnum.SMALLER_THAN_OR_EXACT_VALUE and data > target_value_bytes: continue
 
-        # Search the value and return the found addresses.
-        for offset in searching_method(region_data, size, target_value_bytes, bufflength, scan_type, pytype is str):
-            found_address = address + offset
+            found_address = address + index
 
             extra_information = {
                 "memory_total": memory_total,
-                "progress": (checked_memory_size + offset) / memory_total,
+                "progress": (checked_memory_size + index) / memory_total,
             }
             yield (found_address, extra_information) if progress_information else found_address
 
         # Compute the region size to the checked memory size.
         checked_memory_size += size
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/process.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/process.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 from .enums import ProcessOperationsEnum
 
 from .functions import (
     CloseProcessHandle,
     GetMemoryRegions,
     GetProcessHandle,
     ReadProcessMemory,
-    SearchAllMemory,
+    SearchAddressesByValue,
+    SearchValuesByAddresses,
     WriteProcessMemory
 )
 
-from typing import Generator, Optional, Tuple, Type, TypeVar, Union
+from typing import Generator, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 
 T = TypeVar("T")
 
 
 class WindowsProcess(AbstractProcess):
     """
@@ -66,14 +67,37 @@
         Generates dictionaries with the address, size and other
         information of each memory region used by the process.
         """
         if self.__closed: raise ClosedProcess()
 
         return GetMemoryRegions(self.__process_handle)
 
+    def search_by_addresses(
+        self,
+        pytype: Type[T],
+        bufflength: int,
+        addresses: Sequence[int],
+        *,
+        raise_error: bool = False,
+    ) -> Generator[Tuple[int, Optional[T]], None, None]:
+        """
+        Search the whole memory space, accessible to the process,
+        for the provided list of addresses, returning their values.
+        """
+        if self.__closed: raise ClosedProcess()
+
+        valid_permissions = [
+            ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
+            ProcessOperationsEnum.PROCESS_VM_READ.value
+        ]
+        if self.__permission.value not in valid_permissions:
+            raise PermissionError("The handle does not have permission to read the process memory.")
+
+        return SearchValuesByAddresses(self.__process_handle, pytype, bufflength, addresses, raise_error=raise_error)
+
     def search_by_value(
         self,
         pytype: Type[T],
         bufflength: int,
         value: Union[bool, int, float, str, bytes],
         scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
         *,
@@ -99,15 +123,15 @@
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
         if scan_type in [ScanTypesEnum.VALUE_BETWEEN, ScanTypesEnum.NOT_VALUE_BETWEEN]:
             raise ValueError("Use the method search_by_value_between(...) to search within a range of values.")
 
-        return SearchAllMemory(self.__process_handle, pytype, bufflength, value, scan_type, progress_information, writeable_only)
+        return SearchAddressesByValue(self.__process_handle, pytype, bufflength, value, scan_type, progress_information, writeable_only)
 
     def search_by_value_between(
         self,
         pytype: Type[T],
         bufflength: int,
         start: Union[bool, int, float, str, bytes],
         end: Union[bool, int, float, str, bytes],
@@ -134,15 +158,15 @@
             ProcessOperationsEnum.PROCESS_ALL_ACCESS.value,
             ProcessOperationsEnum.PROCESS_VM_READ.value
         ]
         if self.__permission.value not in valid_permissions:
             raise PermissionError("The handle does not have permission to read the process memory.")
 
         scan_type = ScanTypesEnum.NOT_VALUE_BETWEEN if not_between else ScanTypesEnum.VALUE_BETWEEN
-        return SearchAllMemory(self.__process_handle, pytype, bufflength, (start, end), scan_type, progress_information, writeable_only)
+        return SearchAddressesByValue(self.__process_handle, pytype, bufflength, (start, end), scan_type, progress_information, writeable_only)
 
     def read_process_memory(
         self,
         address: int,
         pytype: Type[T],
         bufflength: int
     ) -> T:
```

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/types.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_allocation_states.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_allocation_states.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_protections.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_protections.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/memory_types.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/memory_types.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/process_operations.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/process_operations.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PyMemoryEditor/win32/enums/standard_access_rights.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/enums/standard_access_rights.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/open_process.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/open_process.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/__init__.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/__init__.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/errors.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/errors.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/process/util.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/process/util.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/functions.py` & `pymemoryeditor-1.5.9/PyMemoryEditor/win32/functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,22 +2,24 @@
 
 # Read more about operations with processes by win32 api here:
 # https://learn.microsoft.com/en-us/windows/win32/api/memoryapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/processthreadsapi/
 # https://learn.microsoft.com/en-us/windows/win32/api/psapi/
 # ...
 
-from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum, ScanTypesEnum
+from ..enums import ScanTypesEnum
+from ..util import convert_from_bytearray, get_c_type_of, scan_memory, scan_memory_for_exact_value
+
+from .enums import MemoryAllocationStatesEnum, MemoryProtectionsEnum, MemoryTypesEnum
 from .types import MEMORY_BASIC_INFORMATION, SYSTEM_INFO, WNDENUMPROC
-from .util import get_c_type_of
-from typing import Generator, Optional, Tuple, Type, TypeVar, Union
+
+from typing import Dict, Generator, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 import ctypes
 import ctypes.wintypes
-import sys
 
 # Load the libraries.
 kernel32 = ctypes.windll.LoadLibrary("kernel32.dll")
 user32 = ctypes.windll.LoadLibrary("user32.dll")
 
 # Set the argtypes to prevent ArgumentError.
 kernel32.VirtualQueryEx.argtypes = (
@@ -121,88 +123,157 @@
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
     data = get_c_type_of(pytype, bufflength)
     kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(data), bufflength, None)
 
-    return str(data.value) if pytype is str else data.value
+    return data.value.decode() if pytype is str else data.value
 
 
-def SearchAllMemory(
+def SearchAddressesByValue(
     process_handle: int,
     pytype: Type[T],
     bufflength: int,
-    value: Union[bool, int, float, str, bytes],
+    value: Union[bool, int, float, str, bytes, tuple],
     scan_type: ScanTypesEnum = ScanTypesEnum.EXACT_VALUE,
-    progress_information: Optional[bool] = False,
+    progress_information: bool = False,
+    writeable_only: bool = False,
 ) -> Generator[Union[int, Tuple[int, dict]], None, None]:
     """
     Search the whole memory space, accessible to the process,
     for the provided value, returning the found addresses.
     """
     if pytype not in [bool, int, float, str, bytes]:
         raise ValueError("The type must be bool, int, float, str or bytes.")
 
-    # Get the target value as bytes.
-    target_value = get_c_type_of(pytype, bufflength)
-    target_value.value = value
+    # Convert the target value, or all values of a tuple, as bytes.
+    target_values = value if isinstance(value, tuple) else (value,)
+
+    conversion_buffer = list()
+
+    for v in target_values:
+        target_value = get_c_type_of(pytype, bufflength)
+        target_value.value = v.encode() if isinstance(v, str) else v
 
-    target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
-    target_value_bytes = int.from_bytes(bytes(target_value_bytes.contents), sys.byteorder)
+        target_value_bytes = ctypes.cast(ctypes.byref(target_value), ctypes.POINTER(ctypes.c_byte * bufflength))
+        conversion_buffer.append(bytes(target_value_bytes.contents))
 
-    regions = list()
+    target_value_bytes = tuple(conversion_buffer) if isinstance(value, tuple) else conversion_buffer[0]
+
+    # Get the memory regions, computing the total amount of memory to be scanned.
+    checked_memory_size = 0
     memory_total = 0
+    memory_regions = list()
 
-    # Get the memory regions, computing the space size.
     for region in GetMemoryRegions(process_handle):
 
         # Only committed, non-shared and readable memory pages.
         if region["struct"].State != MemoryAllocationStatesEnum.MEM_COMMIT.value: continue
         if region["struct"].Type != MemoryTypesEnum.MEM_PRIVATE.value: continue
         if region["struct"].Protect & MemoryProtectionsEnum.PAGE_READABLE.value == 0: continue
 
-        memory_total += region["size"]
-        regions.append(region)
+        # If writeable_only is True, checks if the memory page is writeable.
+        if writeable_only and region["struct"].Protect & MemoryProtectionsEnum.PAGE_READWRITEABLE.value == 0: continue
 
-    checked_memory_size = 0
+        memory_total += region["size"]
+        memory_regions.append(region)
 
     # Check each memory region used by the process.
-    for region in regions:
+    for region in memory_regions:
         address, size = region["address"], region["size"]
         region_data = (ctypes.c_byte * size)()
 
         # Get data from the region.
         kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(address), ctypes.byref(region_data), size, None)
 
-        # Walk by the returned bytes, searching for the target value.
-        for index in range(size - bufflength):
-            data = region_data[index: index + bufflength]
-            data = int.from_bytes(bytes((ctypes.c_byte * bufflength)(*data)), sys.byteorder)
-
-            # Compare the values.
-            if scan_type is ScanTypesEnum.EXACT_VALUE and data != target_value_bytes: continue
-            elif scan_type is ScanTypesEnum.NOT_EXACT_VALUE and data == target_value_bytes: continue
-            elif scan_type is ScanTypesEnum.BIGGER_THAN and data <= target_value_bytes: continue
-            elif scan_type is ScanTypesEnum.SMALLER_THAN and data >= target_value_bytes: continue
-            elif scan_type is ScanTypesEnum.BIGGER_THAN_OR_EXACT_VALUE and data < target_value_bytes: continue
-            elif scan_type is ScanTypesEnum.SMALLER_THAN_OR_EXACT_VALUE and data > target_value_bytes: continue
+        # Choose the searching method.
+        searching_method = scan_memory
 
-            found_address = address + index
+        if scan_type in [ScanTypesEnum.EXACT_VALUE, ScanTypesEnum.NOT_EXACT_VALUE]:
+            searching_method = scan_memory_for_exact_value
+
+        # Search the value and return the found addresses.
+        for offset in searching_method(region_data, size, target_value_bytes, bufflength, scan_type, pytype is str):
+            found_address = address + offset
 
             extra_information = {
                 "memory_total": memory_total,
-                "progress": (checked_memory_size + index) / memory_total,
+                "progress": (checked_memory_size + offset) / memory_total,
             }
             yield (found_address, extra_information) if progress_information else found_address
 
         # Compute the region size to the checked memory size.
         checked_memory_size += size
 
 
+def SearchValuesByAddresses(
+    process_handle: int,
+    pytype: Type[T],
+    bufflength: int,
+    addresses: Sequence[int],
+    *,
+    memory_regions: Optional[Sequence[Dict]] = None,
+    raise_error: bool = False,
+) -> Generator[Tuple[int, Optional[T]], None, None]:
+    """
+    Search the whole memory space, accessible to the process,
+    for the provided list of addresses, returning their values.
+    """
+    if pytype not in [bool, int, float, str, bytes]:
+        raise ValueError("The type must be bool, int, float, str or bytes.")
+
+    memory_regions = list(memory_regions) if memory_regions else list()
+    addresses = sorted(addresses)
+
+    # If no memory page has been given, get all committed, non-shared and readable memory pages.
+    if not memory_regions:
+        for region in GetMemoryRegions(process_handle):
+            if region["struct"].State != MemoryAllocationStatesEnum.MEM_COMMIT.value: continue
+            if region["struct"].Type != MemoryTypesEnum.MEM_PRIVATE.value: continue
+            if region["struct"].Protect & MemoryProtectionsEnum.PAGE_READABLE.value == 0: continue
+
+            memory_regions.append(region)
+
+    memory_regions.sort(key=lambda region: region["address"])
+    address_index = 0
+
+    # Walk by each memory region.
+    for region in memory_regions:
+        if address_index >= len(addresses): continue
+
+        target_address = addresses[address_index]
+
+        # Check if the memory region contains the target address.
+        base_address, size = region["address"], region["size"]
+        if not (base_address <= target_address < base_address + size): continue
+
+        region_data = (ctypes.c_byte * size)()
+
+        # Get data from the region.
+        kernel32.ReadProcessMemory(process_handle, ctypes.c_void_p(base_address), ctypes.byref(region_data), size, None)
+
+        # Get the value of each address.
+        while base_address <= target_address < base_address + size:
+            offset = target_address - base_address
+            address_index += 1
+
+            try:
+                data = region_data[offset: offset + bufflength]
+                data = (ctypes.c_byte * bufflength)(*data)
+                yield target_address, convert_from_bytearray(data, pytype, bufflength)
+
+            except Exception as error:
+                if raise_error: raise error
+                yield target_address, None
+
+            if address_index >= len(addresses): break
+            target_address = addresses[address_index]
+
+
 def WriteProcessMemory(
     process_handle: int,
     address: int,
     pytype: Type[T],
     bufflength: int,
     value: Union[bool, int, float, str, bytes]
 ) -> T:
```

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/types.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/types.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_allocation_states.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_allocation_states.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_protections.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_protections.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/memory_types.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/memory_types.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/process_operations.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/process_operations.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/build/lib/PyMemoryEditor/win32/enums/standard_access_rights.py` & `pymemoryeditor-1.5.9/build/lib/PyMemoryEditor/win32/enums/standard_access_rights.py`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/tests/test_editor.py` & `pymemoryeditor-1.5.9/tests/test_editor.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,21 +64,23 @@
     # Read the process memory and compare the result.
     result = process.read_process_memory(address, int, data_length)
     assert type(result) is int and result == target_value.value
 
 
 def test_read_string():
     # Get a random text to compare the result.
-    target_value = ctypes.create_string_buffer(generate_text(20).encode())
+    target_value = ctypes.create_string_buffer(20)
+    target_value.value = generate_text(20).encode()
+
     address = ctypes.addressof(target_value)
     data_length = ctypes.sizeof(target_value)
 
     # Read the process memory and compare the result.
     result = process.read_process_memory(address, str, data_length)
-    assert type(result) is str and result == str(target_value.value)
+    assert type(result) is str and result == target_value.value.decode()
 
 
 def test_write_bool():
     # Compare with True and False values.
     original_value_1 = True
     original_value_2 = False
 
@@ -130,28 +132,77 @@
 
 
 def test_write_string():
     # Get a random text to compare the result.
     original_value = generate_text(20).encode()
     new_value = generate_text(20).encode()
 
-    target_value = ctypes.create_string_buffer(original_value)
+    target_value = ctypes.create_string_buffer(20)
+    target_value.value = original_value
+
     address = ctypes.addressof(target_value)
     data_length = ctypes.sizeof(target_value)
 
     # Write to the process memory and compare the result.
-    process.write_process_memory(address, str, data_length, new_value)
+    process.write_process_memory(address, str, data_length, new_value.decode())
     assert target_value.value != original_value and target_value.value == new_value
 
 
+def test_search_by_int_addresses():
+    # Get random values to compare the result.
+    test_length = 10
+
+    target_values = [ctypes.c_int(random.randint(0, 10000)) for i in range(test_length)]
+    data_length = ctypes.sizeof(target_values[0])
+
+    target_values = {ctypes.addressof(v): v for v in target_values}
+    addresses = list(target_values.keys())
+
+    for address, value in process.search_by_addresses(int, data_length, addresses):
+        assert target_values[address].value == value and type(value) is int
+
+def test_search_by_float_addresses():
+    # Get random values to compare the result.
+    test_length = 10
+
+    target_values = [ctypes.c_double(random.randint(0, 10000) / random.randint(0, 10000)) for i in range(test_length)]
+    data_length = ctypes.sizeof(target_values[0])
+
+    target_values = {ctypes.addressof(v): v for v in target_values}
+    addresses = list(target_values.keys())
+
+    for address, value in process.search_by_addresses(float, data_length, addresses):
+        assert target_values[address].value == value and type(value) is float
+
+
+def test_search_by_string_addresses():
+    # Get random values to compare the result.
+    string_length, test_length = 20, 10
+
+    target_values = list()
+
+    for i in range(test_length):
+        value = ctypes.create_string_buffer(string_length)
+        value.value = generate_text(string_length).encode()
+        target_values.append(value)
+
+    data_length = ctypes.sizeof(target_values[0])
+
+    target_values = {ctypes.addressof(v): v for v in target_values}
+    addresses = list(target_values.keys())
+
+    for address, value in process.search_by_addresses(str, data_length, addresses):
+        assert target_values[address].value.decode() == value and type(value) is str
+
+
 def test_search_by_int():
     # Get random values to compare the result.
-    length = 10
+    test_length = 10
 
-    target_values = [ctypes.c_int(random.randint(0, 10000)) for i in range(length)]
+    target_values = [ctypes.c_int(random.randint(0, 10000)) for i in range(test_length)]
     addresses = [ctypes.addressof(v) for v in target_values]
     data_length = ctypes.sizeof(target_values[0])
 
     min_value = min([v.value for v in target_values])
     max_value = max([v.value for v in target_values])
 
     total = 0
@@ -168,23 +219,23 @@
 
         total += 1
 
         # Check if the address really points to a valid value.
         value = process.read_process_memory(found_address, int, data_length)
         if min_value <= value <= max_value: correct += 1
 
-    assert found / length >= 0.7
+    assert found / test_length >= 0.7
     assert correct / total >= 0.7  # Some of the addresses are beyond our control and may have their values changed.
 
 
 def test_search_by_float():
     # Get random values to compare the result.
-    length = 10
+    test_length = 10
 
-    target_values = [ctypes.c_double(random.randint(0, 10000)) for i in range(length)]
+    target_values = [ctypes.c_double(random.randint(0, 10000)) for i in range(test_length)]
     addresses = [ctypes.addressof(v) for v in target_values]
     data_length = ctypes.sizeof(target_values[0])
 
     min_value = min([v.value for v in target_values])
     max_value = max([v.value for v in target_values])
 
     total = 0
@@ -201,23 +252,29 @@
 
         total += 1
 
         # Check if the address really points to a valid value.
         value = process.read_process_memory(found_address, float, data_length)
         if min_value <= value <= max_value: correct += 1
 
-    assert found / length >= 0.7
+    assert found / test_length >= 0.7
     assert correct / total >= 0.7  # Some of the addresses are beyond our control and may have their values changed.
 
 
 def test_search_by_string():
     # Get random values to compare the result.
-    length = 10
+    string_length, test_length = 20, 10
+
+    target_values = list()
+
+    for i in range(test_length):
+        value = ctypes.create_string_buffer(string_length)
+        value.value = generate_text(string_length).encode()
+        target_values.append(value)
 
-    target_values = [ctypes.create_string_buffer(generate_text(20).encode()) for i in range(length)]
     data_length = ctypes.sizeof(target_values[0])
 
     total = 0
     found = 0
     correct = 0
 
     # Get addresses of values exact or smaller than max_value.
@@ -227,30 +284,38 @@
             # Check if the found address is the target address.
             if found_address == ctypes.addressof(target_value):
                 found += 1
 
             total += 1
 
             # Check if the address really points to a valid value.
-            value = process.read_process_memory(found_address, str, data_length)
-            if value == str(target_value.value): correct += 1
+            try:
+                value = process.read_process_memory(found_address, str, data_length)
+                if value == target_value.value.decode(): correct += 1
+            except: pass
 
-    assert found / length >= 0.7
+    assert found / test_length >= 0.7
     assert correct / total >= 0.7  # Some of the addresses are beyond our control and may have their values changed.
 
 
 def test_search_by_string_between():
     # Get random values to compare the result.
-    length = 10
+    string_length, test_length = 20, 10
+
+    values = list()
+
+    for i in range(test_length * 2):
+        value = ctypes.create_string_buffer(string_length)
+        value.value = generate_text(string_length).encode()
+        values.append(value)
 
-    values = [ctypes.create_string_buffer(generate_text(20).encode()) for i in range(length * 2)]
     values.sort(key = lambda target_value: target_value.value)
 
     # Half of the set of strings is the target and the other half contains string that should be ignored by the scanner.
-    target_values = [target_value for target_value in values[length // 4: length - length // 4]]
+    target_values = [target_value for target_value in values[test_length // 4: test_length - test_length // 4]]
 
     addresses = [ctypes.addressof(v) for v in values]
     target_addresses = [ctypes.addressof(v) for v in target_values]
 
     data_length = ctypes.sizeof(target_values[0])
 
     min_value = target_values[0].value
@@ -265,13 +330,13 @@
         if found_address in target_addresses:
             addresses.remove(found_address)
             found += 1
 
         elif found_address in addresses:
             raise ValueError("Scanner returned the address of a clearly invalid string.")
 
-    assert found / length >= 0.5
+    assert found / test_length >= 0.5
 
 
 def test_close_process():
     # Try to close the process handle.
     assert process.close()
```

### Comparing `pymemoryeditor-1.5.8/LICENSE` & `pymemoryeditor-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/README.md` & `pymemoryeditor-1.5.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/pymemoryeditor?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/PyMemoryEditor/)
 
 # Installing PyMemoryEditor:
 ```
 pip3 install PyMemoryEditor
 ```
 
+### Tkinter application sample:
+You can run a simple tkinter application to scan the memory of a process by typing `pymemoryeditor` at the CLI.
+
 # Basic Usage:
 Import `PyMemoryEditor` and open a process using the `OpenProcess` class, passing a window title, process name <br>
 or PID as an argument. You can use the context manager to do this.
 ```py
 from PyMemoryEditor import OpenProcess
 
 with OpenProcess(process_name = "example.exe") as process:
@@ -67,26 +70,31 @@
 ```
 
 All methods described above work even for strings, including the method `search_by_value_between` — however, `bytes` comparison may work differently than `str` comparison, depending on the `byteorder` of your system.
 
 ## Progress information on searching:
 These methods has the `progress_information` parameter that returns a dictionary containing the search progress information.
 ```py
-for address, info process.search_by_value(..., progress_information = True):
+for address, info in process.search_by_value(..., progress_information = True):
     template = "Address: 0x{:<10X} | Progress: {:.1f}%"
     progress = info["progress"] * 100
     
     print(template.format(address, progress))
 ```
 
+# Reading multiple addresses efficiently:
+If you have a large number of addresses where their values need to be read from memory, using the `search_by_addresses` method is much more efficient than reading the value of each address one by one.
+```py
+for address, value in process.search_by_addresses(int, 4, addresses_list):
+    print(f"Address", address, "holds the value", value)
+```
+The key advantage of this method is that it reads a memory page just once, obtaining the values of the addresses within the page. This approach reduces the frequency of system calls.
+
 ## Getting memory regions:
 Use the method `get_memory_regions()` to get the base address, size and more information of all memory regions used by the process.
 
 ```py
 for memory_region in process.get_memory_regions():
     base_address = memory_region["address"]
     size = memory_region["size"]
     information = memory_region["struct"]
 ```
-
-# Tkinter application sample:
-You can run a simple tkinter application to scan the memory of a process by typing `pymemoryeditor` at the CLI.
```

### Comparing `pymemoryeditor-1.5.8/pyproject.toml` & `pymemoryeditor-1.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pymemoryeditor-1.5.8/PKG-INFO` & `pymemoryeditor-1.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMemoryEditor
-Version: 1.5.8
+Version: 1.5.9
 Summary: Multi-platform library developed with ctypes for reading, writing and searching process memory, in a simple and friendly way with Python 3.
 Project-URL: Homepage, https://github.com/JeanExtreme002/PyMemoryEditor
 Author-email: Jean Loui Bernard Silva de Jesus <jeanextreme002@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: address,api,cheat,ctypes,debug,editor,linux,memory,override,pointer,process,ptrace,reader,readprocessmemory,scanner,track,virtual,win32,writeprocessmemory,writer
 Classifier: Intended Audience :: Developers
@@ -43,14 +43,17 @@
 [![Downloads](https://static.pepy.tech/personalized-badge/pymemoryeditor?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads)](https://pypi.org/project/PyMemoryEditor/)
 
 # Installing PyMemoryEditor:
 ```
 pip3 install PyMemoryEditor
 ```
 
+### Tkinter application sample:
+You can run a simple tkinter application to scan the memory of a process by typing `pymemoryeditor` at the CLI.
+
 # Basic Usage:
 Import `PyMemoryEditor` and open a process using the `OpenProcess` class, passing a window title, process name <br>
 or PID as an argument. You can use the context manager to do this.
 ```py
 from PyMemoryEditor import OpenProcess
 
 with OpenProcess(process_name = "example.exe") as process:
@@ -99,26 +102,31 @@
 ```
 
 All methods described above work even for strings, including the method `search_by_value_between` — however, `bytes` comparison may work differently than `str` comparison, depending on the `byteorder` of your system.
 
 ## Progress information on searching:
 These methods has the `progress_information` parameter that returns a dictionary containing the search progress information.
 ```py
-for address, info process.search_by_value(..., progress_information = True):
+for address, info in process.search_by_value(..., progress_information = True):
     template = "Address: 0x{:<10X} | Progress: {:.1f}%"
     progress = info["progress"] * 100
     
     print(template.format(address, progress))
 ```
 
+# Reading multiple addresses efficiently:
+If you have a large number of addresses where their values need to be read from memory, using the `search_by_addresses` method is much more efficient than reading the value of each address one by one.
+```py
+for address, value in process.search_by_addresses(int, 4, addresses_list):
+    print(f"Address", address, "holds the value", value)
+```
+The key advantage of this method is that it reads a memory page just once, obtaining the values of the addresses within the page. This approach reduces the frequency of system calls.
+
 ## Getting memory regions:
 Use the method `get_memory_regions()` to get the base address, size and more information of all memory regions used by the process.
 
 ```py
 for memory_region in process.get_memory_regions():
     base_address = memory_region["address"]
     size = memory_region["size"]
     information = memory_region["struct"]
 ```
-
-# Tkinter application sample:
-You can run a simple tkinter application to scan the memory of a process by typing `pymemoryeditor` at the CLI.
```

