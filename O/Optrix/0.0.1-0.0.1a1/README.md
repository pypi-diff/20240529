# Comparing `tmp/optrix-0.0.1.tar.gz` & `tmp/optrix-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optrix-0.0.1.tar", last modified: Tue May 28 23:14:18 2024, max compression
+gzip compressed data, was "optrix-0.0.1a1.tar", last modified: Tue Nov 21 16:03:39 2023, max compression
```

## Comparing `optrix-0.0.1.tar` & `optrix-0.0.1a1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 joaobiu    (501) staff       (20)        0 2024-05-28 23:14:18.700355 optrix-0.0.1/
--rw-r--r--   0 joaobiu    (501) staff       (20)     1065 2024-05-28 23:08:05.000000 optrix-0.0.1/LICENSE
-drwxr-xr-x   0 joaobiu    (501) staff       (20)        0 2024-05-28 23:14:18.700055 optrix-0.0.1/Optrix.egg-info/
--rw-r--r--   0 joaobiu    (501) staff       (20)      459 2024-05-28 23:14:18.000000 optrix-0.0.1/Optrix.egg-info/PKG-INFO
--rw-r--r--   0 joaobiu    (501) staff       (20)      212 2024-05-28 23:14:18.000000 optrix-0.0.1/Optrix.egg-info/SOURCES.txt
--rw-r--r--   0 joaobiu    (501) staff       (20)        1 2024-05-28 23:14:18.000000 optrix-0.0.1/Optrix.egg-info/dependency_links.txt
--rw-r--r--   0 joaobiu    (501) staff       (20)        7 2024-05-28 23:14:18.000000 optrix-0.0.1/Optrix.egg-info/top_level.txt
--rw-r--r--   0 joaobiu    (501) staff       (20)      459 2024-05-28 23:14:18.700194 optrix-0.0.1/PKG-INFO
--rw-r--r--   0 joaobiu    (501) staff       (20)       93 2024-05-28 23:08:05.000000 optrix-0.0.1/README.md
-drwxr-xr-x   0 joaobiu    (501) staff       (20)        0 2024-05-28 23:14:18.699814 optrix-0.0.1/optrix/
--rw-r--r--   0 joaobiu    (501) staff       (20)       96 2024-05-28 23:08:05.000000 optrix-0.0.1/optrix/__init__.py
--rw-r--r--   0 joaobiu    (501) staff       (20)     7911 2024-05-28 23:08:05.000000 optrix-0.0.1/optrix/_objects.py
--rw-r--r--   0 joaobiu    (501) staff       (20)      439 2024-05-28 23:12:21.000000 optrix-0.0.1/pyproject.toml
--rw-r--r--   0 joaobiu    (501) staff       (20)       38 2024-05-28 23:14:18.700396 optrix-0.0.1/setup.cfg
-drwxr-xr-x   0 joaobiu    (501) staff       (20)        0 2024-05-28 23:14:18.699923 optrix-0.0.1/tests/
--rw-r--r--   0 joaobiu    (501) staff       (20)     2521 2024-05-28 23:08:05.000000 optrix-0.0.1/tests/test_objects.py
+drwxr-xr-x   0 joaobiu   (1000) joaobiu   (1000)        0 2023-11-21 16:03:39.217138 optrix-0.0.1a1/
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)     1237 2023-11-21 16:03:39.217138 optrix-0.0.1a1/PKG-INFO
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)       93 2023-11-20 23:18:51.000000 optrix-0.0.1a1/README.md
+drwxr-xr-x   0 joaobiu   (1000) joaobiu   (1000)        0 2023-11-21 16:03:39.217138 optrix-0.0.1a1/optrix/
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)       82 2023-11-21 00:16:47.000000 optrix-0.0.1a1/optrix/__init__.py
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)     6923 2023-11-21 15:50:40.000000 optrix-0.0.1a1/optrix/_objects.py
+drwxr-xr-x   0 joaobiu   (1000) joaobiu   (1000)        0 2023-11-21 16:03:39.217138 optrix-0.0.1a1/optrix.egg-info/
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)     1237 2023-11-21 16:03:39.000000 optrix-0.0.1a1/optrix.egg-info/PKG-INFO
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)      252 2023-11-21 16:03:39.000000 optrix-0.0.1a1/optrix.egg-info/SOURCES.txt
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)        1 2023-11-21 16:03:39.000000 optrix-0.0.1a1/optrix.egg-info/dependency_links.txt
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)       43 2023-11-21 16:03:39.000000 optrix-0.0.1a1/optrix.egg-info/requires.txt
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)        7 2023-11-21 16:03:39.000000 optrix-0.0.1a1/optrix.egg-info/top_level.txt
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)       86 2023-11-20 23:31:06.000000 optrix-0.0.1a1/pyproject.toml
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)       78 2023-11-21 16:03:39.217138 optrix-0.0.1a1/setup.cfg
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)     1708 2023-11-20 23:32:37.000000 optrix-0.0.1a1/setup.py
+drwxr-xr-x   0 joaobiu   (1000) joaobiu   (1000)        0 2023-11-21 16:03:39.217138 optrix-0.0.1a1/tests/
+-rw-r--r--   0 joaobiu   (1000) joaobiu   (1000)     2521 2023-11-21 15:56:15.000000 optrix-0.0.1a1/tests/test_objects.py
```

### Comparing `optrix-0.0.1/optrix/_objects.py` & `optrix-0.0.1a1/optrix/_objects.py`

 * *Files 14% similar despite different names*

```diff
@@ -264,44 +264,8 @@
 
     @property
     def distance(self):
         return self._distance
     
     @distance.setter
     def distance(self, value):
-        self._distance = value
-
-class GaussianBeam:
-    def __init__(self, wavelength, w0, A0):
-        self.wavelength = wavelength
-        self.w0 = w0
-        self.A0 = A0
-
-    def z0(self):
-        return np.pi*self.w0**2/self.wavelength
-
-    def w(self, z):   
-        return self.w0*np.sqrt(1+(z/self.z0())**2)
-        
-    def R(self, z):
-        return z*(1+(self.z0()/(z + 1e-15))**2)
-        
-    def zeta(self, z):
-        return np.arctan(z/self.z0())
-
-    def wavefunction(self, x, y, z):
-        rho = np.sqrt(x**2 + y**2)
-        A0 = self.A0
-        w0 = self.w0
-        w = self.w(z)
-        k = 2*np.pi/self.wavelength
-        R = self.R(z)
-        zeta = self.zeta(z)
-        return A0*(w0/w)*np.exp(-rho**2/(w**2 + 1e-15))*np.exp(-1j*k*(rho**2)/(2*R + 1e-15))*np.exp(1j*zeta)
-
-    def wavefunction_in_0(self, x, y):
-        A0 = self.A0
-        w0 = self.w0
-        return A0*np.exp(-(x**2+y**2)/w0**2 + 1e-15)
-
-    def intensity(self, x, y, z):
-        return np.abs(self.wavefunction(x, y, z))**2
+        self._distance = value
```

### Comparing `optrix-0.0.1/tests/test_objects.py` & `optrix-0.0.1a1/tests/test_objects.py`

 * *Files identical despite different names*

