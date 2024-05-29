# Comparing `tmp/cirq-1.4.0.dev20240523223409-py3-none-any.whl.zip` & `tmp/cirq-1.4.0.dev20240529181723-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 8322 bytes, number of entries: 6
--rw-r--r--  2.0 unx      292 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/AUTHORS
--rw-r--r--  2.0 unx    11357 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/LICENSE
--rw-r--r--  2.0 unx     7712 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 24-May-23 22:34 cirq-1.4.0.dev20240523223409.dist-info/RECORD
-6 files, 20017 bytes uncompressed, 7284 bytes compressed:  63.6%
+Zip file size: 8351 bytes, number of entries: 6
+-rw-r--r--  2.0 unx      292 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/AUTHORS
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7864 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 24-May-29 18:17 cirq-1.4.0.dev20240529181723.dist-info/RECORD
+6 files, 20169 bytes uncompressed, 7313 bytes compressed:  63.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: cirq-1.4.0.dev20240523223409.dist-info/AUTHORS
+Filename: cirq-1.4.0.dev20240529181723.dist-info/AUTHORS
 Comment: 
 
-Filename: cirq-1.4.0.dev20240523223409.dist-info/LICENSE
+Filename: cirq-1.4.0.dev20240529181723.dist-info/LICENSE
 Comment: 
 
-Filename: cirq-1.4.0.dev20240523223409.dist-info/METADATA
+Filename: cirq-1.4.0.dev20240529181723.dist-info/METADATA
 Comment: 
 
-Filename: cirq-1.4.0.dev20240523223409.dist-info/WHEEL
+Filename: cirq-1.4.0.dev20240529181723.dist-info/WHEEL
 Comment: 
 
-Filename: cirq-1.4.0.dev20240523223409.dist-info/top_level.txt
+Filename: cirq-1.4.0.dev20240529181723.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq-1.4.0.dev20240523223409.dist-info/RECORD
+Filename: cirq-1.4.0.dev20240529181723.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `cirq-1.4.0.dev20240523223409.dist-info/LICENSE` & `cirq-1.4.0.dev20240529181723.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq-1.4.0.dev20240523223409.dist-info/METADATA` & `cirq-1.4.0.dev20240529181723.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cirq
-Version: 1.4.0.dev20240523223409
+Version: 1.4.0.dev20240529181723
 Summary: A framework for creating, editing, and invoking Noisy Intermediate Scale Quantum (NISQ) circuits.
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Requires-Python: >=3.10.0
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: cirq-aqt ==1.4.0.dev20240523223409
-Requires-Dist: cirq-core ==1.4.0.dev20240523223409
-Requires-Dist: cirq-google ==1.4.0.dev20240523223409
-Requires-Dist: cirq-ionq ==1.4.0.dev20240523223409
-Requires-Dist: cirq-pasqal ==1.4.0.dev20240523223409
-Requires-Dist: cirq-rigetti ==1.4.0.dev20240523223409
-Requires-Dist: cirq-web ==1.4.0.dev20240523223409
+Requires-Dist: cirq-aqt ==1.4.0.dev20240529181723
+Requires-Dist: cirq-core ==1.4.0.dev20240529181723
+Requires-Dist: cirq-google ==1.4.0.dev20240529181723
+Requires-Dist: cirq-ionq ==1.4.0.dev20240529181723
+Requires-Dist: cirq-pasqal ==1.4.0.dev20240529181723
+Requires-Dist: cirq-rigetti ==1.4.0.dev20240529181723
+Requires-Dist: cirq-web ==1.4.0.dev20240529181723
 Provides-Extra: dev_env
 Requires-Dist: mypy ==1.2.0 ; extra == 'dev_env'
 Requires-Dist: types-backports ==0.1.3 ; extra == 'dev_env'
 Requires-Dist: types-cachetools ; extra == 'dev_env'
 Requires-Dist: types-protobuf ~=3.20 ; extra == 'dev_env'
 Requires-Dist: types-requests ==2.28.1 ; extra == 'dev_env'
 Requires-Dist: types-setuptools ==62.6.1 ; extra == 'dev_env'
@@ -35,29 +35,32 @@
 Requires-Dist: virtualenv ~=20.23 ; extra == 'dev_env'
 Requires-Dist: virtualenv-clone ; extra == 'dev_env'
 Requires-Dist: black ==24.3.0 ; extra == 'dev_env'
 Requires-Dist: pylint ~=2.13.0 ; extra == 'dev_env'
 Requires-Dist: grpcio-tools ~=1.59.0 ; extra == 'dev_env'
 Requires-Dist: mypy-protobuf ==3.4 ; extra == 'dev_env'
 Requires-Dist: ipython >=7.34.0 ; extra == 'dev_env'
-Requires-Dist: notebook <=6.4.7,>=6.4.1 ; extra == 'dev_env'
-Requires-Dist: ipykernel ==5.3.4 ; extra == 'dev_env'
-Requires-Dist: papermill ~=2.3.2 ; extra == 'dev_env'
+Requires-Dist: notebook ~=7.0 ; extra == 'dev_env'
+Requires-Dist: ipykernel ~=6.29 ; extra == 'dev_env'
+Requires-Dist: papermill ~=2.6 ; extra == 'dev_env'
 Requires-Dist: ply >=3.6 ; extra == 'dev_env'
 Requires-Dist: pylatex ~=1.4 ; extra == 'dev_env'
 Requires-Dist: quimb ~=1.7 ; extra == 'dev_env'
 Requires-Dist: opt-einsum ; extra == 'dev_env'
 Requires-Dist: seaborn ~=0.12 ; extra == 'dev_env'
+Requires-Dist: jupyterlab ~=4.0.13 ; extra == 'dev_env'
+Requires-Dist: jupyterlab-server ~=2.24.0 ; extra == 'dev_env'
+Requires-Dist: nbformat ~=5.10.4 ; extra == 'dev_env'
 Requires-Dist: virtualenv ; extra == 'dev_env'
 Requires-Dist: setuptools ; extra == 'dev_env'
 Requires-Dist: wheel ; extra == 'dev_env'
 Requires-Dist: twine ; extra == 'dev_env'
 Requires-Dist: asv ; extra == 'dev_env'
 Requires-Dist: qiskit-aer ~=0.12.0 ; extra == 'dev_env'
-Requires-Dist: rstcheck ~=3.3.1 ; extra == 'dev_env'
+Requires-Dist: rstcheck ; extra == 'dev_env'
 Requires-Dist: codeowners ; (platform_system != "Windows") and extra == 'dev_env'
 
 **This is a development version of Cirq and may be unstable.**
 
 **For the latest stable release of Cirq see**
 `here <https://pypi.org/project/cirq>`__.
```

