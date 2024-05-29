# Comparing `tmp/scipion-em-aretomo-3.9.0.tar.gz` & `tmp/scipion-em-aretomo-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-aretomo-3.9.0.tar", last modified: Mon Mar  4 13:26:44 2024, max compression
+gzip compressed data, was "scipion-em-aretomo-3.9.1.tar", last modified: Wed May 29 07:54:44 2024, max compression
```

## Comparing `scipion-em-aretomo-3.9.0.tar` & `scipion-em-aretomo-3.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/aretomo/
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/aretomo/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/convert/dataimport.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/aretomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40949 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/protocols/protocol_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/aretomo/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14005 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/aretomo/tests/test_protocols_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-04 13:26:44.000000 scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 13:26:44.529925 scipion-em-aretomo-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-03-04 13:26:16.000000 scipion-em-aretomo-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.052127 scipion-em-aretomo-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-29 07:54:44.052127 scipion-em-aretomo-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.048127 scipion-em-aretomo-3.9.1/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.048127 scipion-em-aretomo-3.9.1/aretomo/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5466 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/convert/dataimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.048127 scipion-em-aretomo-3.9.1/aretomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43057 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/protocols/protocol_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.048127 scipion-em-aretomo-3.9.1/aretomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/aretomo/tests/test_protocols_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:54:44.052127 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-29 07:54:43.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-29 07:54:44.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:54:43.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 07:54:43.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 07:54:43.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 07:54:43.000000 scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:54:44.052127 scipion-em-aretomo-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-05-29 07:54:15.000000 scipion-em-aretomo-3.9.1/setup.py
```

### Comparing `scipion-em-aretomo-3.9.0/CHANGES.txt` & `scipion-em-aretomo-3.9.1/CHANGES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+3.9.1:
+  Users:
+   - Add aretomo2 1.1.2
+   - Fix backwards compatibility.
+   - Add an option to specify AlignZ per TS.
+   - fix dose weighting bug related to the tilt angle file (aretomo2 only)
+  Developers:
+   - The tests now use the Test Centralization Layer update and expansion of the used test set definition
+     from em-tomo v3.6.0.
+   - Update the acquisition order in the CTFTomo objects (field added to that class in scipion-em-tomo v3.7.0).
 3.9.0:
   Users:
     - The protocol form now present CTF-related parameters, to choose if estimate it or
       not and phase plate acquisition related params (estimate the phase shift).
     - Generates the output SetOfCtfTomoSeries if the CTF files are found
     - Add dataimport module to parse the CTF generated so it can be called from the
       centralized protocol for importing CTFs.
```

### Comparing `scipion-em-aretomo-3.9.0/LICENSE` & `scipion-em-aretomo-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/PKG-INFO` & `scipion-em-aretomo-3.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.9.0
+Version: 3.9.1
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
@@ -56,39 +56,39 @@
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-aretomo --devel
         
         * AreTomo binaries will be installed automatically with the plugin, but you can also link an existing installation.
-        * Default installation path assumed is ``software/em/aretomo2-1.0.0``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
-        * Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.0.0_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
+        * Default installation path assumed is ``software/em/aretomo2-1.1.2``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
+        * Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.1.2_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
         * If you need to use CUDA different from the one used during Scipion installation (defined by CUDA_LIB), you can add *ARETOMO_CUDA_LIB* variable to the config file. Various binaries can be downloaded from the official website.
         
         To check the installation, simply run the following Scipion test:
         
         ``scipion test aretomo.tests.test_protocols_aretomo.TestAreTomo``
         
         Licensing
         ---------
         
-        AreTomo2 is available under BSD-3 license
+        AreTomo2 binaries is available under BSD-3 license
         
         Supported versions
         ------------------
         
-        aretomo2: 1.0.0
+        aretomo2: 1.0.0, 1.1.2
         aretomo: 1.3.4
         
         Protocols
         ---------
         
             * tilt-series align and reconstruct
         
-        Detailed manual can be found in ``software/em/aretomo2-1.0.0/bin/AreTomo2Manual_1.0.0_10-26-2023.pdf``
+        Detailed manual can be found in ``software/em/aretomo2-1.1.2/bin/AreTomo2_Manual_1.1.pdf``
         
         References
         ----------
         
             * AreTomo: An integrated software package for automated marker-free, motion-corrected cryo-electron tomographic alignment and reconstruction. Shawn Zheng, Georg Wolff, Garrett Greenan, Zhen Chen, Frank G. A. Faas, Montserrat Bárcena, Abraham J. Koster, Yifan Cheng, David Agard. JSB vol. 6, 2022, 100068.
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
```

### Comparing `scipion-em-aretomo-3.9.0/README.rst` & `scipion-em-aretomo-3.9.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -46,37 +46,37 @@
     * install
 
     .. code-block::
 
         scipion installp -p /path/to/scipion-em-aretomo --devel
 
 * AreTomo binaries will be installed automatically with the plugin, but you can also link an existing installation.
-* Default installation path assumed is ``software/em/aretomo2-1.0.0``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
-* Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.0.0_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
+* Default installation path assumed is ``software/em/aretomo2-1.1.2``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
+* Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.1.2_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
 * If you need to use CUDA different from the one used during Scipion installation (defined by CUDA_LIB), you can add *ARETOMO_CUDA_LIB* variable to the config file. Various binaries can be downloaded from the official website.
 
 To check the installation, simply run the following Scipion test:
 
 ``scipion test aretomo.tests.test_protocols_aretomo.TestAreTomo``
 
 Licensing
 ---------
 
-AreTomo2 is available under BSD-3 license
+AreTomo2 binaries is available under BSD-3 license
 
 Supported versions
 ------------------
 
-aretomo2: 1.0.0
+aretomo2: 1.0.0, 1.1.2
 aretomo: 1.3.4
 
 Protocols
 ---------
 
     * tilt-series align and reconstruct
 
-Detailed manual can be found in ``software/em/aretomo2-1.0.0/bin/AreTomo2Manual_1.0.0_10-26-2023.pdf``
+Detailed manual can be found in ``software/em/aretomo2-1.1.2/bin/AreTomo2_Manual_1.1.pdf``
 
 References
 ----------
 
     * AreTomo: An integrated software package for automated marker-free, motion-corrected cryo-electron tomographic alignment and reconstruction. Shawn Zheng, Georg Wolff, Garrett Greenan, Zhen Chen, Frank G. A. Faas, Montserrat Bárcena, Abraham J. Koster, Yifan Cheng, David Agard. JSB vol. 6, 2022, 100068.
```

### Comparing `scipion-em-aretomo-3.9.0/aretomo/__init__.py` & `scipion-em-aretomo-3.9.1/aretomo/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,34 +28,41 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.9.0'
+__version__ = '3.9.1'
 _logo = "aretomo_logo.png"
 _references = ['Zheng2022']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = ARETOMO_HOME
     _pathVars = [ARETOMO_HOME, ARETOMO_CUDA_LIB]
-    _supportedVersions = [V1_0_0, V1_3_4]
+    _supportedVersions = [V1_0_0, V1_1_2, V1_3_4]
     _url = "https://github.com/scipion-em/scipion-em-aretomo"
 
     @classmethod
     def _defineVariables(cls):
-        cls._defineEmVar(ARETOMO_HOME, f'aretomo2-{V1_0_0}')
+        cls._defineEmVar(ARETOMO_HOME, f'aretomo2-{V1_1_2}')
         cls._defineVar(ARETOMO_CUDA_LIB, pwem.Config.CUDA_LIB)
 
         # Define the variable default value based on the guessed cuda version
-        cudaVersion = cls.guessCudaVersion(ARETOMO_CUDA_LIB)
-        cls._defineVar(ARETOMO_BIN,
-                       f'AreTomo2_{V1_0_0}_Cuda{cudaVersion.major}{cudaVersion.minor}')
+        cudaVersion = cls.guessCudaVersion(ARETOMO_CUDA_LIB,
+                                           default="11.8")
+
+        if cls.getVar(ARETOMO_HOME).endswith(V1_3_4):
+            binaryName = f'AreTomo_{V1_3_4}_Cuda{cudaVersion.major}{cudaVersion.minor}_Feb22_2023'
+        else:
+            binaryStr = V1_0_0 if cls.getVar(ARETOMO_HOME).endswith(V1_0_0) else V1_1_2
+            binaryName = f'AreTomo2_{binaryStr}_Cuda{cudaVersion.major}{cudaVersion.minor}'
+
+        cls._defineVar(ARETOMO_BIN, binaryName)
 
     @classmethod
     def getEnviron(cls):
         """ Return the environment to run AreTomo. """
         environ = pwutils.Environ(os.environ)
         # Get AreTomo CUDA library path if defined
         cudaLib = cls.getVar(ARETOMO_CUDA_LIB, pwem.Config.CUDA_LIB)
@@ -81,12 +88,14 @@
     @classmethod
     def getProgram(cls) -> str:
         """ Return the program binary that will be used. """
         return cls.getHome('bin', cls.getVar(ARETOMO_BIN))
 
     @classmethod
     def defineBinaries(cls, env):
-        env.addPackage('aretomo2', version=V1_0_0,
-                       tar=f"aretomo2-{V1_0_0}.tgz",
-                       default=True)
+        for v in [V1_0_0, V1_1_2]:
+            env.addPackage('aretomo2', version=v,
+                           tar=f"aretomo2-{v}.tgz",
+                           default=v == V1_1_2)
+
         env.addPackage('aretomo', version=V1_3_4,
                        tar=f"aretomo_v{V1_3_4}.tgz")
```

### Comparing `scipion-em-aretomo-3.9.0/aretomo/bibtex.py` & `scipion-em-aretomo-3.9.1/aretomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/constants.py` & `scipion-em-aretomo-3.9.1/aretomo/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 ARETOMO_BIN = 'ARETOMO_BIN'
 ARETOMO_HOME = 'ARETOMO_HOME'
 ARETOMO_CUDA_LIB = 'ARETOMO_CUDA_LIB'
 
 # Supported versions
 V1_0_0 = '1.0.0'
+V1_1_2 = '1.1.2'
 V1_3_4 = '1.3.4'  # TODO: delete old aretomo
 
 RECON_SART = 0
 RECON_WBP = 1
 
 LOCAL_MOTION_DISABLE = 0
 LOCAL_MOTION_COORDS = 1
```

### Comparing `scipion-em-aretomo-3.9.0/aretomo/convert/__init__.py` & `scipion-em-aretomo-3.9.1/aretomo/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/convert/convert.py` & `scipion-em-aretomo-3.9.1/aretomo/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/convert/dataimport.py` & `scipion-em-aretomo-3.9.1/aretomo/convert/dataimport.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
             # The enabled attribute has to be managed here because the method ctfModelToCtfTomo can't copy that
             # attribute as it is a python boolean instead of a Scipion Boolean object. This is because that attribute
             # belongs to the class Object, which is above in the hierarchy than the Scipion types, so it can't follow
             # their setters and getters logic, failing when trying to copy the mentioned attribute
             if not ti.isEnabled():
                 newCtfTomo.setEnabled(False)
             newCtfTomo.setIndex(i + 1)
+            newCtfTomo.setAcquisitionOrder(ti.getAcquisitionOrder())
             output.append(newCtfTomo)
 
     @staticmethod
     def _getCtfTi(ctfModel, ctfArray, item=0, psdFile=None):
         """ Set values for the ctfModel from an input list.
         :param ctfModel: output CTF model
         :param ctfArray: array with CTF values
```

### Comparing `scipion-em-aretomo-3.9.0/aretomo/protocols/__init__.py` & `scipion-em-aretomo-3.9.1/aretomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/protocols/protocol_aretomo.py` & `scipion-em-aretomo-3.9.1/aretomo/protocols/protocol_aretomo.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
                           SetOfTomograms, SetOfTiltSeries, SetOfCTFTomoSeries, CTFTomoSeries)
 
 from .. import Plugin
 from ..convert.convert import getTransformationMatrix, readAlnFile
 from ..convert.dataimport import AretomoCtfParser
 from ..constants import RECON_SART, LOCAL_MOTION_COORDS, LOCAL_MOTION_PATCHES, V1_3_4
 
-
 OUT_TS = "TiltSeries"
 OUT_TS_ALN = "InterpolatedTiltSeries"
 OUT_TOMO = "Tomograms"
 OUT_CTFS = "CTFTomoSeries"
 
 
 class ProtAreTomoAlignRecon(EMProtocol, ProtTomoBase, ProtStreamingBase):
@@ -130,15 +129,26 @@
                       help='Specifies Z height (*unbinned*) of the temporary volume '
                            'reconstructed for projection matching as part '
                            'of the alignment process. This value plays '
                            'an important role in alignment accuracy. This '
                            'Z height should be always smaller than tomogram '
                            'thickness and should be close to the sample '
                            'thickness.')
-
+        
+        form.addParam('alignZfile', params.FileParam,
+                      expertLevel=params.LEVEL_ADVANCED,
+                      condition='not skipAlign and not useInputProt',
+                      label='File with volume height for alignment per tilt-series',
+                      help='Specifies a text file containing the Z height (*unbinned*) '
+                           'to be used for alignment of individual tilt-series. '
+                           'The file should have two columns, the first '
+                           'containing the tsId and the second containing the AlignZ value '
+                           'for that tilt-series. You can specify one tilt-series '
+                           'per line.')
+        
         form.addParam('tomoThickness', params.IntParam,
                       condition='makeTomo', important=True,
                       default=1200, label='Tomogram thickness unbinned (voxels)',
                       help='Z height of the reconstructed volume in '
                            '*unbinned* voxels.')
 
         form.addParam('refineTiltAngles',
@@ -284,15 +294,15 @@
                       expertLevel=params.LEVEL_ADVANCED,
                       label='Additional parameters',
                       help="Extra command line parameters. See AreTomo help.")
 
         form.addHidden(params.GPU_LIST, params.StringParam,
                        default='0', label="Choose GPU IDs")
 
-        form.addParallelSection(threads=2)
+        form.addParallelSection(threads=2, mpi=0)
 
     # --------------------------- INSERT steps functions ----------------------
     def stepsGeneratorStep(self) -> None:
         """
         This step should be implemented by any streaming protocol.
         It should check its input and when ready conditions are met
         call the self._insertFunctionStep method.
@@ -343,14 +353,19 @@
         doSwap = 45 < abs(rotationAngle) < 135
         ts.applyTransform(outputTsFileName, swapXY=doSwap)
 
         # Generate angle file
         angleFilePath = self.getFilePath(tsFn, tmpPrefix, ".tlt")
         self._generateTltFile(ts, angleFilePath)
 
+        if not self.skipAlign and self.alignZfile.hasValue():
+            alignZfile = self.alignZfile.get()
+            if os.path.exists(alignZfile):
+                self.perTsAlignZ = self.readThicknessFile(alignZfile)
+
         if self.useInputProt:
             # Find and copy aln file
             protExtra = self.inputProt.get()._getExtraPath(tsId)
             protAlnBase = self.getFilePath(tsFn, protExtra, ".aln").replace(
                 "_even", "*").replace("_odd", "*")
             protAln = glob(protAlnBase)
             if protAln:
@@ -381,14 +396,17 @@
             '-FlipVol': 1 if self.makeTomo and self.flipVol else 0,
             '-PixSize': tsSet.getSamplingRate(),
             '-Kv': tsSet.getAcquisition().getVoltage(),
             '-DarkTol': self.darkTol.get(),
             '-Gpu': '%(GPU)s'
         }
 
+        if Plugin.getActiveVersion() != V1_3_4 and self.doDW:
+            args['-ImgDose'] = tsSet.getAcquisition().getDosePerFrame()
+
         if Plugin.getActiveVersion() != V1_3_4 and self.doEstimateCtf.get():
             # Manage the CTF estimation:
             # In AreTomo2, parameters PixSize, Kv and Cs are required to estimate the CTF. Since the first two are
             # also used for the dose weighting and the third is only used for the CTF estimation, we'll use it as
             # doEstimateCtf flag parameter.
             args['-Cs'] = tsSet.getAcquisition().getSphericalAberration()
             if self.doPhaseShiftSearch.get():
@@ -401,15 +419,18 @@
             if ts.hasAlignment():
                 # in this case we already used ts.applyTransform()
                 tiltAxisAngle = 0.0
 
             args['-TiltAxis'] = f"{tiltAxisAngle} {self.refineTiltAxis.get() - 1}"
             args['-TiltCor'] = self.refineTiltAngles.get() - 1
 
-            if not self.skipAlign:
+            if self.alignZfile.get():
+                # Check if we have AlignZ information per tilt-series
+                args['-AlignZ'] = self.perTsAlignZ.get(tsId, self.alignZ)
+            else:
                 args['-AlignZ'] = self.alignZ
 
             if self.sampleType.get() == LOCAL_MOTION_COORDS:
                 args['-RoiFile'] = self.coordsFn
             elif self.sampleType.get() == LOCAL_MOTION_PATCHES:
                 args['-Patch'] = f"{self.patchX} {self.patchY}"
 
@@ -461,15 +482,15 @@
             #    10   -10.6414    1.00000     24.338     -5.868     1.00     1.00     1.00     0.00  1567301525373690323140608.00
             #
             # Hence, the output tilt angles will be checked before storing the corresponding outputs
             inTiltAngles = np.array([ti.getTiltAngle() for ti in ts if ti.getIndex() - 1 in AretomoAln.sections])
             aretomoTiltAngles = np.array([AretomoAln.tilt_angles])
             if not np.allclose(inTiltAngles, aretomoTiltAngles, atol=45):
                 msg = 'tsId = %s. Bad tilt angle values detected.' % tsId
-                self.info(msg + ' Skipping...')
+                self.warning(msg + ' Skipping...')
                 outMsg = self.badTsAliMsg.get() + '\n' + msg if self.badTsAliMsg.get() else '\n' + msg
                 self.badTsAliMsg.set(outMsg)
                 self._store(self.badTsAliMsg)
                 return
 
             alignmentMatrix = getTransformationMatrix(AretomoAln.imod_matrix)
 
@@ -491,15 +512,15 @@
             # values, see comment above).
             #
             # Hence, the output tilt angles will be checked before storing the corresponding outputs
             tomoFileName = self.getFilePath(tsFn, extraPrefix, ".mrc")
             tomoDims = self._getOutputDim(tomoFileName)
             if np.any(np.array(tomoDims) == len(ts)):
                 msg = 'tsId = %s. Generated tomogram dims = %s' % (tsId, str(tomoDims))
-                self.info('Tilt series skipped because of a bad reconstruction. ' + msg)
+                self.warning('Tilt series skipped because of a bad reconstruction. ' + msg)
                 outMsg = self.badTomoRecMsg.get() + '\n' + msg if self.badTomoRecMsg.get() else '\n' + msg
                 self.badTomoRecMsg.set(outMsg)
                 self._store(self.badTomoRecMsg)
                 return
             outputSetOfTomograms = self.getOutputSetOfTomograms()
             # Tomogram attributes
             newTomogram = Tomogram()
@@ -529,15 +550,14 @@
                     if secNum in AretomoAln.sections:
                         newTi = TiltImage()
                         newTi.copyInfo(tiltImage, copyId=False, copyTM=False)
 
                         acqTi = tiltImage.getAcquisition()
                         acqTi.setTiltAxisAngle(0.)
 
-
                         secIndex = AretomoAln.sections.index(secNum)
                         newTi.setTiltAngle(AretomoAln.tilt_angles[secIndex])
                         newTi.setLocation(secIndex + 1,
                                           (self.getFilePath(tsFn, extraPrefix, ".mrc")))
                         newTi.setSamplingRate(self._getOutputSampling())
                         newTs.append(newTi)
                         # If the interpolated TS was generated considering the dose weighting, it's accumulated dose
@@ -547,19 +567,21 @@
                             acqTi.setAccumDose(0.)
                             newTi.setAcquisition(acqTi)
                         else:
                             initialDoseList.append(acqTi.getDoseInitial())
                             accumDoseList.append(acqTi.getAccumDose())
 
                     else:
-                        excludedViewsList.append(secNum)
+                        excludedViewsList.append(secNum + 1)
                 if excludedViewsList:
                     newTs.setAnglesCount(len(newTs))
                     prevMsg = self.excludedViewsMsg.get() if self.excludedViewsMsg.get() else ''
-                    self.excludedViewsMsg.set(prevMsg + f'\n{tsId}: {excludedViewsList}')
+                    newMsg = f'\n{tsId}: {excludedViewsList}'
+                    self.warning('Some views were excluded:' + prevMsg)
+                    self.excludedViewsMsg.set(prevMsg + newMsg)
                     self._store(self.excludedViewsMsg)
 
                 acq = newTs.getAcquisition()
                 if self.doDW.get():
                     acq.setDoseInitial(0.)
                     acq.setAccumDose(0.)
                 else:
@@ -726,14 +748,33 @@
                     self.TS_read.append(ts.getObjId())
             self.info(f'Tomograms calculated for this TS_ID : {self.TS_read}')
             self.outputSOTSList_objID = self.TS_read
 
         except AttributeError:  # There is no outputSetOfTiltSeries
             pass
 
+    def readThicknessFile(self, filePath: os.PathLike):
+        """ Reads a text file with thickness information per tilt-series.
+        Example of how the file should look like:
+        Position_112 700
+        Position_35  650
+        Position_18  500
+        Position_114 1000
+        """
+        thickPerTs = {}
+        with open(filePath, "r") as f:
+            lines = f.readlines()
+            lines = filter(lambda x: x.strip(), lines)
+
+            for line in lines:
+                values = line.split()
+                thickPerTs[values[0]] = values[1]
+
+        return thickPerTs
+
     def getFilePath(self,
                     tsFn: Union[str, os.PathLike],
                     prefix: str,
                     ext: Optional[str] = None) -> Union[str, os.PathLike]:
         fileName, fileExtension = os.path.splitext(os.path.basename(tsFn))
         if ext is not None:
             fileExtension = ext
@@ -812,21 +853,23 @@
         x, y, z, _ = ih.getDimensions(fn)
         return x, y, z
 
     def _generateTltFile(self, ts: TiltSeries,
                          outputFn: os.PathLike) -> None:
         """ Generate .tlt file with tilt angles and accumulated dose. """
         angleList = []
+        aretomo2 = Plugin.getActiveVersion() != V1_3_4
 
         for ti in ts.iterItems(orderBy="_index"):
+            acqOrder = ti.getAcquisitionOrder()
             accDose = ti.getAcquisition().getAccumDose()
             tAngle = ti.getTiltAngle()
-            angleList.append((tAngle, accDose))
+            angleList.append((tAngle, acqOrder if aretomo2 else accDose))
 
         with open(outputFn, 'w') as f:
             if self.doDW:
-                f.writelines(f"{i[0]:0.3f} {i[1]:0.3f}\n" for i in angleList)
+                f.writelines(f"{i[0]:0.3f} {i[1]}\n" for i in angleList)
             else:
                 f.writelines(f"{i[0]:0.3f}\n" for i in angleList)
 
     def _saveInterpolated(self) -> bool:
         return self.saveStack
```

### Comparing `scipion-em-aretomo-3.9.0/aretomo/protocols.conf` & `scipion-em-aretomo-3.9.1/aretomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/tests/__init__.py` & `scipion-em-aretomo-3.9.1/aretomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/aretomo/tests/test_protocols_aretomo.py` & `scipion-em-aretomo-3.9.1/aretomo/tests/test_protocols_aretomo.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,96 +24,54 @@
 # *
 # **************************************************************************
 import numpy as np
 
 from pwem import ALIGN_2D
 from pyworkflow.utils import magentaStr
 from pyworkflow.tests import DataSet, setupTestProject
-
-from tomo.objects import TomoAcquisition
 from tomo.protocols import ProtImportTs
 from tomo.tests import RE4_STA_TUTO, DataSetRe4STATuto
 from tomo.tests.test_base_centralized_layer import TestBaseCentralizedLayer
 
 from ..protocols.protocol_aretomo import (ProtAreTomoAlignRecon, OUT_TS, OUT_TOMO,
                                           OUT_TS_ALN, OUT_CTFS)
 
 TS_54 = 'TS_54'
 TS_03 = 'TS_03'
 
 
 class TestAreTomoBase(TestBaseCentralizedLayer):
-    nAnglesDict = None
     ds = None
     importedTs = None
-    particlesUnbinnedBoxSize = 256
-    particlesExtractedBoxSize = 64
+    unbinnedSRate = DataSetRe4STATuto.unbinnedPixSize.value
+    nAnglesDict = DataSetRe4STATuto.nAnglesDict.value
+    nTiltSeries = len(nAnglesDict)
+    expectedDimsTs = DataSetRe4STATuto.dimsTsBin1Dict.value
+    tsAcqDict = DataSetRe4STATuto.tsAcqDict.value
     alignZ = 900
-    nTiltSeries = 2
     binFactor = 4
-    unbinnedSRate = DataSetRe4STATuto.unbinnedPixSize.value
     unbinnedThk = 1200
-    expectedDimsTs = {TS_03: [3710, 3838, 40],
-                      TS_54: [3710, 3838, 41]}
     expectedTomoDims = [958, 926, 300]
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.ds = DataSet.getDataSet(RE4_STA_TUTO)
         cls.expectedOriginShifts = list(np.array(cls.expectedTomoDims) / -2 * cls.unbinnedSRate * cls.binFactor)
         cls.inTsSet = cls._runImportTs()
-        # Angles count dict
-        cls.nAnglesDict = {
-            TS_03: 40,
-            TS_54: 41
-        }
-        # Acquisition common parameters
-        dosePerTiltImg = DataSetRe4STATuto.dosePerTiltImgWithTltFile.value
-        testAcq = TomoAcquisition(voltage=DataSetRe4STATuto.voltage.value,
-                                  sphericalAberration=DataSetRe4STATuto.sphericalAb.value,
-                                  amplitudeContrast=DataSetRe4STATuto.amplitudeContrast.value,
-                                  magnification=DataSetRe4STATuto.magnification.value,
-                                  doseInitial=DataSetRe4STATuto.initialDose.value,
-                                  dosePerFrame=dosePerTiltImg,
-                                  angleMax=60,
-                                  step=3)
-        # Acquisition of TS_03
-        testAcq03 = testAcq.clone()
-        testAcq03.setAngleMin(-57)
-        testAcq03.setAccumDose(dosePerTiltImg * cls.nAnglesDict[TS_03])
-        # Acquisition of TS_54
-        testAcq54 = testAcq.clone()
-        testAcq54.setAngleMin(-60)
-        testAcq54.setAccumDose(dosePerTiltImg * cls.nAnglesDict[TS_54])
-        # Tilt series acq dict
-        cls.tsAcqDict = {
-            TS_03: testAcq03,
-            TS_54: testAcq54
-        }
+
         # Acquisition of the interpolated TS: aretomo allows to dose-weight the TS, so if the interpolated TS is
         # generated and the dose-weight option is active, then the dose is set to 0 to avoid double dose correction
         # if using the interpolated TS for the PPPT. Also, the tilt axis angle should be 0 as the tilt series is
         # aligned
-        # Acquisition of TS_03 interpolated
-        testAcq03Interp = testAcq03.clone()
-        testAcq03Interp.setTiltAxisAngle(0)
-        # Acquisition of TS_54 interpolated
-        testAcq54Interp = testAcq54.clone()
-        testAcq54Interp.setTiltAxisAngle(0)
-        # Tilt series interpolated acq dict
-        cls.tsAcqInterpDict = {
-            TS_03: testAcq03Interp,
-            TS_54: testAcq54Interp
-        }
         # Acquisition of TS_03 interpolated with DW
-        testAcq03InterpDw = testAcq03Interp.clone()
+        testAcq03InterpDw = DataSetRe4STATuto.testAcq03Interp.value.clone()
         testAcq03InterpDw.setAccumDose(0)
         # Acquisition of TS_54 interpolated with DW
-        testAcq54InterpDw = testAcq54Interp.clone()
+        testAcq54InterpDw = DataSetRe4STATuto.testAcq54Interp.value.clone()
         testAcq54InterpDw.setAccumDose(0)
         # Tilt series interpolated acq dict wih DW
         cls.tsAcqInterpDwDict = {
             TS_03: testAcq03InterpDw,
             TS_54: testAcq54InterpDw
         }
 
@@ -148,16 +106,15 @@
                          "\n\t- Dose weighting"
                          "\n\t- No views are excluded"
                          "\n\t- CTF not generated"))
 
         # Expected values
         expectedDimsTsInterp = {TS_03: [958, 926, 40],
                                 TS_54: [958, 926, 41]}
-        nAnglesDict = {TS_03: 40,
-                       TS_54: 41}
+
         # Update the corresponding acquisition dictionary with the refined tilt axis angle values
         tsAcqDict = self.tsAcqDict
         tsAcqDict[TS_03].setTiltAxisAngle(85.13)
         tsAcqDict[TS_54].setTiltAxisAngle(85.3)
 
         # Run the protocol
         prot = self.newProtocol(ProtAreTomoAlignRecon,
@@ -184,15 +141,15 @@
         # Interpolated TS
         self.checkTiltSeries(getattr(prot, OUT_TS_ALN, None),
                              expectedSetSize=self.nTiltSeries,
                              expectedSRate=self.unbinnedSRate * self.binFactor,
                              # Protocol sets the bin factor to 2 by default
                              expectedDimensions=expectedDimsTsInterp,
                              testAcqObj=self.tsAcqInterpDwDict,
-                             anglesCount=nAnglesDict,
+                             anglesCount=self.nAnglesDict,
                              isInterpolated=True)
         # CTFs
         self.assertIsNone(getattr(prot, OUT_CTFS, None))
 
     def test_align_02(self):
         print(magentaStr("\n==> Testing AreTomo:"
                          "\n\t- Align only"
@@ -211,15 +168,15 @@
         # Update the corresponding acquisition dictionary with the refined tilt axis angle values
         # Note: they're different from in the previous test because of the views exclusion
         tsAcqDict = self.tsAcqDict
         tsAcqDict[TS_03].setTiltAxisAngle(84.9)
         tsAcqDict[TS_54].setTiltAxisAngle(85.19)
         # Because some of the excluded views are at the end of the stack and DW is not applied in this test, the TS
         # accumulated values will be updated in the interpolated TS
-        tsAcqDictInterp = self.tsAcqInterpDict
+        tsAcqDictInterp = DataSetRe4STATuto.tsAcqInterpDict.value
         tsAcqDictInterp[TS_03].setAccumDose(96)
         tsAcqDictInterp[TS_54].setAccumDose(111)
 
         # Run the protocol
         prot = self.newProtocol(ProtAreTomoAlignRecon,
                                 inputSetOfTiltSeries=self.inTsSet,
                                 makeTomo=False,
```

### Comparing `scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/PKG-INFO` & `scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.9.0
+Version: 3.9.1
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
@@ -56,39 +56,39 @@
             * install
         
             .. code-block::
         
                 scipion installp -p /path/to/scipion-em-aretomo --devel
         
         * AreTomo binaries will be installed automatically with the plugin, but you can also link an existing installation.
-        * Default installation path assumed is ``software/em/aretomo2-1.0.0``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
-        * Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.0.0_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
+        * Default installation path assumed is ``software/em/aretomo2-1.1.2``, if you want to change it, set *ARETOMO_HOME* in ``scipion.conf`` file to the folder where the AreTomo is installed.
+        * Depending on your CUDA version this plugin will guess the right default binary from ``AreTomo2_1.1.2_CudaXY`` (X is for cuda major version, Y for the minor). You can always set a different one by explicitly setting ARETOMO_BIN variable.
         * If you need to use CUDA different from the one used during Scipion installation (defined by CUDA_LIB), you can add *ARETOMO_CUDA_LIB* variable to the config file. Various binaries can be downloaded from the official website.
         
         To check the installation, simply run the following Scipion test:
         
         ``scipion test aretomo.tests.test_protocols_aretomo.TestAreTomo``
         
         Licensing
         ---------
         
-        AreTomo2 is available under BSD-3 license
+        AreTomo2 binaries is available under BSD-3 license
         
         Supported versions
         ------------------
         
-        aretomo2: 1.0.0
+        aretomo2: 1.0.0, 1.1.2
         aretomo: 1.3.4
         
         Protocols
         ---------
         
             * tilt-series align and reconstruct
         
-        Detailed manual can be found in ``software/em/aretomo2-1.0.0/bin/AreTomo2Manual_1.0.0_10-26-2023.pdf``
+        Detailed manual can be found in ``software/em/aretomo2-1.1.2/bin/AreTomo2_Manual_1.1.pdf``
         
         References
         ----------
         
             * AreTomo: An integrated software package for automated marker-free, motion-corrected cryo-electron tomographic alignment and reconstruction. Shawn Zheng, Georg Wolff, Garrett Greenan, Zhen Chen, Frank G. A. Faas, Montserrat Bárcena, Abraham J. Koster, Yifan Cheng, David Agard. JSB vol. 6, 2022, 100068.
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
```

### Comparing `scipion-em-aretomo-3.9.0/scipion_em_aretomo.egg-info/SOURCES.txt` & `scipion-em-aretomo-3.9.1/scipion_em_aretomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.9.0/setup.py` & `scipion-em-aretomo-3.9.1/setup.py`

 * *Files identical despite different names*

