# Comparing `tmp/pykinml-1.0.1.tar.gz` & `tmp/pykinml-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykinml-1.0.1.tar", last modified: Tue May 28 22:00:10 2024, max compression
+gzip compressed data, was "pykinml-1.0.2.tar", last modified: Tue May 28 22:33:05 2024, max compression
```

## Comparing `pykinml-1.0.1.tar` & `pykinml-1.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:00:10.071878 pykinml-1.0.1/
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)      198 2024-05-15 16:19:47.000000 pykinml-1.0.1/LICENSE
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     2059 2024-05-28 22:00:10.071878 pykinml-1.0.1/PKG-INFO
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)      883 2024-04-03 21:38:47.000000 pykinml-1.0.1/README.md
-drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:00:10.070878 pykinml-1.0.1/pykinml/
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)        0 2024-02-13 00:47:19.000000 pykinml-1.0.1/pykinml/__init__.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    12813 2024-05-15 16:18:21.000000 pykinml-1.0.1/pykinml/aev.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     8334 2024-05-15 16:18:30.000000 pykinml-1.0.1/pykinml/daev.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)   107962 2024-05-15 16:18:36.000000 pykinml-1.0.1/pykinml/data.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    21079 2024-05-15 16:18:45.000000 pykinml-1.0.1/pykinml/hdf5_handler.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     6026 2024-05-15 16:18:54.000000 pykinml-1.0.1/pykinml/model_calculator.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    17144 2024-05-15 16:19:06.000000 pykinml-1.0.1/pykinml/nnpes.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    25015 2024-05-15 16:19:14.000000 pykinml-1.0.1/pykinml/rdb.py
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)   140080 2024-05-15 16:19:22.000000 pykinml-1.0.1/pykinml/trainer.py
-drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:00:10.071878 pykinml-1.0.1/pykinml.egg-info/
--rw-r--r--   0 cjdever  (136073) cjdever  (136073)     2059 2024-05-28 22:00:10.000000 pykinml-1.0.1/pykinml.egg-info/PKG-INFO
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)      356 2024-05-28 22:00:10.000000 pykinml-1.0.1/pykinml.egg-info/SOURCES.txt
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)        1 2024-05-28 22:00:10.000000 pykinml-1.0.1/pykinml.egg-info/dependency_links.txt
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       58 2024-05-28 22:00:10.000000 pykinml-1.0.1/pykinml.egg-info/requires.txt
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       22 2024-05-28 22:00:10.000000 pykinml-1.0.1/pykinml.egg-info/top_level.txt
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     1379 2024-05-28 21:59:34.000000 pykinml-1.0.1/pyproject.toml
--rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       38 2024-05-28 22:00:10.071878 pykinml-1.0.1/setup.cfg
+drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:33:05.990949 pykinml-1.0.2/
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     1439 2024-05-28 22:29:53.000000 pykinml-1.0.2/LICENSE
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     3364 2024-05-28 22:33:05.990949 pykinml-1.0.2/PKG-INFO
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)      883 2024-04-03 21:38:47.000000 pykinml-1.0.2/README.md
+drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:33:05.989949 pykinml-1.0.2/pykinml/
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)        0 2024-02-13 00:47:19.000000 pykinml-1.0.2/pykinml/__init__.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    14054 2024-05-28 22:22:36.000000 pykinml-1.0.2/pykinml/aev.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     9575 2024-05-28 22:22:47.000000 pykinml-1.0.2/pykinml/daev.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)   109203 2024-05-28 22:22:58.000000 pykinml-1.0.2/pykinml/data.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    22320 2024-05-28 22:23:07.000000 pykinml-1.0.2/pykinml/hdf5_handler.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     7267 2024-05-28 22:23:15.000000 pykinml-1.0.2/pykinml/model_calculator.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    18385 2024-05-28 22:23:23.000000 pykinml-1.0.2/pykinml/nnpes.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)    26256 2024-05-28 22:23:33.000000 pykinml-1.0.2/pykinml/rdb.py
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)   141321 2024-05-28 22:23:41.000000 pykinml-1.0.2/pykinml/trainer.py
+drwxrwxr-x   0 cjdever  (136073) cjdever  (136073)        0 2024-05-28 22:33:05.989949 pykinml-1.0.2/pykinml.egg-info/
+-rw-r--r--   0 cjdever  (136073) cjdever  (136073)     3364 2024-05-28 22:33:05.000000 pykinml-1.0.2/pykinml.egg-info/PKG-INFO
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)      356 2024-05-28 22:33:05.000000 pykinml-1.0.2/pykinml.egg-info/SOURCES.txt
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)        1 2024-05-28 22:33:05.000000 pykinml-1.0.2/pykinml.egg-info/dependency_links.txt
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       58 2024-05-28 22:33:05.000000 pykinml-1.0.2/pykinml.egg-info/requires.txt
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       22 2024-05-28 22:33:05.000000 pykinml-1.0.2/pykinml.egg-info/top_level.txt
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)     1379 2024-05-28 22:33:03.000000 pykinml-1.0.2/pyproject.toml
+-rw-rw-r--   0 cjdever  (136073) cjdever  (136073)       38 2024-05-28 22:33:05.990949 pykinml-1.0.2/setup.cfg
```

### Comparing `pykinml-1.0.1/README.md` & `pykinml-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pykinml-1.0.1/pykinml/aev.py` & `pykinml-1.0.2/pykinml/aev.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 import math
 import numpy as np
 import matplotlib.pyplot as plt
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/daev.py` & `pykinml-1.0.2/pykinml/daev.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 import timeit
 import numpy as np
 import torch
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/data.py` & `pykinml-1.0.2/pykinml/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 import math
 import sys
 import time
 import os
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/hdf5_handler.py` & `pykinml-1.0.2/pykinml/hdf5_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 import sys
 import os
 import timeit
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/nnpes.py` & `pykinml-1.0.2/pykinml/nnpes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 import torch
 import torch.nn as nn
 from torch_scatter import segment_coo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/rdb.py` & `pykinml-1.0.2/pykinml/rdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 # utility library for sqlite relational database functionality
 # use these functions to create meta, xyz, aev, and energy data tables
 # and to write to or read from them
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pykinml/trainer.py` & `pykinml-1.0.2/pykinml/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 #=====================================================================================
 """
 Copyright 2024 National Technology & Engineering Solutions of Sandia, LLC (NTESS). 
 Under the terms of Contract DE-NA0003525 with NTESS, the U.S. Government retains certain rights in this software.
+
+Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS “AS IS” AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 #=====================================================================================
 
 from pathlib import Path
 import math
 import sys
 import argparse
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pykinml-1.0.1/pyproject.toml` & `pykinml-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 exclude = ["build", "dist", "ensemble", "examples"]
 
 [tool.setuptools.package-data]
 "pykinml.tpl" = []
 
 [project]
 name = "pykinml"
-version = "1.0.1"
+version = "1.0.2"
 description = "Neural Net Potential Energy Surface"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 # keywords = []
 authors = [
     {name="cjdever", email="cjdever@sandia.gov"},
```

