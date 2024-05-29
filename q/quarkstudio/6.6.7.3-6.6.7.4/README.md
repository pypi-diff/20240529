# Comparing `tmp/quarkstudio-6.6.7.3-cp312-none-win_amd64.whl.zip` & `tmp/quarkstudio-6.6.7.4-cp311-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 132897 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     1084 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3201 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       37 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        1 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      517 b- defN 24-May-28 12:43 quarkstudio-6.6.7.3.dist-info/RECORD
--rw-rw-rw-  2.0 fat   220672 b- defN 24-May-28 12:43 quark/__init__.pyd
--rw-rw-rw-  2.0 fat    76800 b- defN 24-May-28 12:43 quark/setting.pyd
-8 files, 302412 bytes uncompressed, 131727 bytes compressed:  56.4%
+Zip file size: 778680 bytes, number of entries: 8
+-rwxrwxrwx  2.0 unx     1084 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3173 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      111 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       37 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/entry_points.txt
+-rwxrwxrwx  2.0 unx        1 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      517 b- defN 24-May-29 01:57 quarkstudio-6.6.7.4.dist-info/RECORD
+-rwxr-xr-x  2.0 unx  1426792 b- defN 24-May-29 01:57 quark/__init__.so
+-rwxr-xr-x  2.0 unx   518328 b- defN 24-May-29 01:57 quark/setting.so
+8 files, 1950043 bytes uncompressed, 777514 bytes compressed:  60.1%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: quarkstudio-6.6.7.3.dist-info/LICENSE
+Filename: quarkstudio-6.6.7.4.dist-info/LICENSE
 Comment: 
 
-Filename: quarkstudio-6.6.7.3.dist-info/METADATA
+Filename: quarkstudio-6.6.7.4.dist-info/METADATA
 Comment: 
 
-Filename: quarkstudio-6.6.7.3.dist-info/WHEEL
+Filename: quarkstudio-6.6.7.4.dist-info/WHEEL
 Comment: 
 
-Filename: quarkstudio-6.6.7.3.dist-info/entry_points.txt
+Filename: quarkstudio-6.6.7.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: quarkstudio-6.6.7.3.dist-info/top_level.txt
+Filename: quarkstudio-6.6.7.4.dist-info/top_level.txt
 Comment: 
 
-Filename: quarkstudio-6.6.7.3.dist-info/RECORD
+Filename: quarkstudio-6.6.7.4.dist-info/RECORD
 Comment: 
 
-Filename: quark/__init__.pyd
+Filename: quark/__init__.so
 Comment: 
 
-Filename: quark/setting.pyd
+Filename: quark/setting.so
 Comment: 
 
 Zip file comment:
```

## Comparing `quarkstudio-6.6.7.3.dist-info/LICENSE` & `quarkstudio-6.6.7.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `quarkstudio-6.6.7.3.dist-info/METADATA` & `quarkstudio-6.6.7.4.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-Metadata-Version: 2.1
-Name: quarkstudio
-Version: 6.6.7.3
-Summary: description
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL Feng
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: srpc >=4.2.8
-Requires-Dist: zee >=0.0.2
-Provides-Extra: full
-Requires-Dist: vios >=2.0.0 ; extra == 'full'
-Requires-Dist: anyon >=4.1.0 ; extra == 'full'
-Requires-Dist: axion >=4.0.0 ; extra == 'full'
-Requires-Dist: qwark >=1.0.0 ; extra == 'full'
-Requires-Dist: pyside6 >=6.4.2 ; extra == 'full'
-Requires-Dist: pyqtgraph >=0.12.4 ; extra == 'full'
-Requires-Dist: matplotlib >=3.6.3 ; extra == 'full'
-Requires-Dist: vispy >=0.12.0 ; extra == 'full'
-Requires-Dist: qtconsole >=0.12.0 ; extra == 'full'
-Provides-Extra: server
-Requires-Dist: vios >=2.0.0 ; extra == 'server'
-Requires-Dist: anyon >=4.1.0 ; extra == 'server'
-Requires-Dist: axion >=4.0.0 ; extra == 'server'
-Provides-Extra: studio
-Requires-Dist: qwark >=1.0.0 ; extra == 'studio'
-Requires-Dist: pyside6 >=6.4.2 ; extra == 'studio'
-Requires-Dist: pyqtgraph >=0.12.4 ; extra == 'studio'
-Requires-Dist: matplotlib >=3.6.3 ; extra == 'studio'
-Requires-Dist: vispy >=0.12.0 ; extra == 'studio'
-Requires-Dist: qtconsole >=0.12.0 ; extra == 'studio'
-
-123
+Metadata-Version: 2.1
+Name: quarkstudio
+Version: 6.6.7.4
+Summary: description
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL Feng
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: srpc (>=4.2.8)
+Requires-Dist: zee (>=0.0.2)
+Provides-Extra: full
+Requires-Dist: vios (>=2.0.0) ; extra == 'full'
+Requires-Dist: anyon (>=4.1.0) ; extra == 'full'
+Requires-Dist: axion (>=4.0.0) ; extra == 'full'
+Requires-Dist: qwark (>=1.0.0) ; extra == 'full'
+Requires-Dist: pyside6 (>=6.4.2) ; extra == 'full'
+Requires-Dist: pyqtgraph (>=0.12.4) ; extra == 'full'
+Requires-Dist: matplotlib (>=3.6.3) ; extra == 'full'
+Requires-Dist: vispy (>=0.12.0) ; extra == 'full'
+Requires-Dist: qtconsole (>=0.12.0) ; extra == 'full'
+Provides-Extra: server
+Requires-Dist: vios (>=2.0.0) ; extra == 'server'
+Requires-Dist: anyon (>=4.1.0) ; extra == 'server'
+Requires-Dist: axion (>=4.0.0) ; extra == 'server'
+Provides-Extra: studio
+Requires-Dist: qwark (>=1.0.0) ; extra == 'studio'
+Requires-Dist: pyside6 (>=6.4.2) ; extra == 'studio'
+Requires-Dist: pyqtgraph (>=0.12.4) ; extra == 'studio'
+Requires-Dist: matplotlib (>=3.6.3) ; extra == 'studio'
+Requires-Dist: vispy (>=0.12.0) ; extra == 'studio'
+Requires-Dist: qtconsole (>=0.12.0) ; extra == 'studio'
+
+123
```

