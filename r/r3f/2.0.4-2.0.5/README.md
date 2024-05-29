# Comparing `tmp/r3f-2.0.4.tar.gz` & `tmp/r3f-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3f-2.0.4.tar", last modified: Tue May 28 16:17:50 2024, max compression
+gzip compressed data, was "r3f-2.0.5.tar", last modified: Wed May 29 19:53:52 2024, max compression
```

## Comparing `r3f-2.0.4.tar` & `r3f-2.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.670345 r3f-2.0.4/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.4/LICENSE.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-28 16:17:50.670288 r3f-2.0.4/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.4/README.md
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.4/pyproject.toml
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2024-05-28 16:17:50.670578 r3f-2.0.4/setup.cfg
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.668245 r3f-2.0.4/src/
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.669360 r3f-2.0.4/src/r3f/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.4/src/r3f/__init__.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)   102708 2024-05-28 16:08:59.000000 r3f-2.0.4/src/r3f/r3f.py
--rw-r--r--   0 davidwoodburn   (501) staff       (20)    19909 2024-05-28 16:07:59.000000 r3f-2.0.4/src/r3f/test_r3f.py
-drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-28 16:17:50.670111 r3f-2.0.4/src/r3f.egg-info/
--rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/PKG-INFO
--rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/SOURCES.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/dependency_links.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/requires.txt
--rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-28 16:17:50.000000 r3f-2.0.4/src/r3f.egg-info/top_level.txt
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-29 19:53:52.328079 r3f-2.0.5/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     1059 2022-05-06 23:09:16.000000 r3f-2.0.5/LICENSE.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-29 19:53:52.328020 r3f-2.0.5/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4320 2023-10-19 22:37:17.000000 r3f-2.0.5/README.md
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       85 2022-10-17 18:56:07.000000 r3f-2.0.5/pyproject.toml
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      607 2024-05-29 19:53:52.328316 r3f-2.0.5/setup.cfg
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-29 19:53:52.325881 r3f-2.0.5/src/
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-29 19:53:52.327011 r3f-2.0.5/src/r3f/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)       50 2022-05-27 17:40:46.000000 r3f-2.0.5/src/r3f/__init__.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)   104098 2024-05-29 19:42:23.000000 r3f-2.0.5/src/r3f/r3f.py
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)    20421 2024-05-29 19:51:33.000000 r3f-2.0.5/src/r3f/test_r3f.py
+drwxr-xr-x   0 davidwoodburn   (501) staff       (20)        0 2024-05-29 19:53:52.327814 r3f-2.0.5/src/r3f.egg-info/
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)     4805 2024-05-29 19:53:52.000000 r3f-2.0.5/src/r3f.egg-info/PKG-INFO
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)      255 2024-05-29 19:53:52.000000 r3f-2.0.5/src/r3f.egg-info/SOURCES.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        1 2024-05-29 19:53:52.000000 r3f-2.0.5/src/r3f.egg-info/dependency_links.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        6 2024-05-29 19:53:52.000000 r3f-2.0.5/src/r3f.egg-info/requires.txt
+-rw-r--r--   0 davidwoodburn   (501) staff       (20)        4 2024-05-29 19:53:52.000000 r3f-2.0.5/src/r3f.egg-info/top_level.txt
```

### Comparing `r3f-2.0.4/LICENSE.txt` & `r3f-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `r3f-2.0.4/PKG-INFO` & `r3f-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.4
+Version: 2.0.5
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `r3f-2.0.4/README.md` & `r3f-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `r3f-2.0.4/setup.cfg` & `r3f-2.0.5/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = r3f
-version = 2.0.4
+version = 2.0.5
 author = David Woodburn
 author_email = david.woodburn@icloud.com
 description = A library for three-dimensional, reference-frame conversions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/davidwoodburn/r3f
 classifiers =
```

### Comparing `r3f-2.0.4/src/r3f/r3f.py` & `r3f-2.0.5/src/r3f/r3f.py`

 * *Files 2% similar despite different names*

```diff
@@ -1212,15 +1212,15 @@
 
     # Check input.
     if isinstance(rpy, (list, tuple)):
         rpy = np.array(rpy)
     trs = (rpy.ndim == 2 and rpy.shape[0] != 3)
     s = np.pi/180 if degs else 1.0
 
-    # Tranpose.
+    # Transpose.
     if trs:
         rpy = rpy.T
 
     if rpy.ndim == 1:
         # Get the cosine and sine functions.
         r, p, y = rpy
         cr = math.cos(s*r)
@@ -1327,14 +1327,62 @@
 
         # Pre-multiply the old rotation matrix by the new.
         C = C_n @ C
 
     return C
 
 
+def rotate(C, vec):
+    """
+    Rotate a vector over time. `C` should be a 3d array, a stack of rotation
+    matrices, and `vec` should be a matrix of vectors. Each layer of the stack
+    and each column of the vector correspond to a different moment in time.
+
+    Parameters
+    ----------
+    vec : (3, K) or (K, 3) list, tuple, or np.ndarray
+        Matrix of vectors in which each column (or row) is a vector.
+    C : (K, 3, 3) np.ndarray
+        Rotation matrix or stack of K rotation matrices.
+
+    Returns
+    -------
+    out : (3, K) or (K, 3) np.ndarray
+        Matrix of rotated vectors in which each column (or row) is a vector.
+    """
+
+    # Check input.
+    if isinstance(vec, (list, tuple)):
+        vec = np.array(vec)
+    if np.ndim(vec) != 2:
+        raise ValueError("vec must be a 2d array.")
+    if np.ndim(C) != 3:
+        raise ValueError("C must be a 3d array.")
+    trs = (vec.shape[0] != 3)
+
+    # Transpose input.
+    if trs:
+        vec = vec.T
+
+    # Initialize the output.
+    K = vec.shape[1]
+    out = np.zeros((3, K))
+
+    # Perform the matrix-vector multiplication.
+    out[0] = C[:, 0, 0]*vec[0] + C[:, 0, 1]*vec[1] + C[:, 0, 2]*vec[2]
+    out[1] = C[:, 1, 0]*vec[0] + C[:, 1, 1]*vec[1] + C[:, 1, 2]*vec[2]
+    out[2] = C[:, 2, 0]*vec[0] + C[:, 2, 1]*vec[1] + C[:, 2, 2]*vec[2]
+
+    # Transpose output.
+    if trs:
+        out = out.T
+
+    return out
+
+
 def quat_to_rpy(q, degs=False):
     """
     Convert from a quaternion right-handed frame rotation to a roll, pitch, and
     yaw, z, y, x sequence of right-handed frame rotations. If frame 1 is rotated
     in a z, y, x sequence to become frame 2, then the quaternion `q` would also
     rotate a vector in frame 1 into frame 2.
 
@@ -2056,15 +2104,15 @@
 
     # Get the longitude.
     lon = np.arctan2(ye, xe)
 
     # Assemble the matrix.
     llh = np.array([hlat/s, lon/s, hhae])
 
-    # Tranpose output.
+    # Transpose output.
     if trs:
         llh = llh.T
 
     return llh
 
 
 def tangent_to_ecef(pt, pe0, ned=True):
```

### Comparing `r3f-2.0.4/src/r3f/test_r3f.py` & `r3f-2.0.5/src/r3f/test_r3f.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,36 @@
 
     # preserve units
     ang = np.array([45, 45, 45])
     ax = np.array([2, 1, 0])
     R = r3f.rot(ang, ax, True)
     assert np.allclose(ang, np.array([45, 45, 45]))
 
+
+def test_rotate():
+    # Generate the random inputs.
+    N = 10
+    R = np.random.uniform(-np.pi, np.pi, N)
+    P = np.random.uniform(-np.pi/2 + r3f.TOL, np.pi/2 - r3f.TOL, N)
+    Y = np.random.uniform(-np.pi, np.pi, N)
+    C = r3f.rpy_to_dcm([R, P, Y])
+    a = np.random.randn(3, N)
+
+    # Rotate with the single function.
+    b1 = r3f.rotate(C, a)
+
+    # Rotate with a for loop.
+    b2 = np.zeros((3, N))
+    for n in range(N):
+        b2[:, n] = C[n, :, :] @ a[:, n]
+
+    # Check the results.
+    assert np.allclose(b1, b2)
+
+
 # -------------------------
 # Reference-frame Rotations
 # -------------------------
 
 def test_dcm_inertial_to_ecef():
     # Test single time.
     t = np.pi/r3f.W_EI
@@ -631,9 +653,7 @@
     assert np.allclose(delta, Delta)
     try:
         theta = r3f.inverse_rodrigues_rotation(Delta)
         assert False
     except:
         assert True
 
-
-test_rodrigues()
```

### Comparing `r3f-2.0.4/src/r3f.egg-info/PKG-INFO` & `r3f-2.0.5/src/r3f.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3f
-Version: 2.0.4
+Version: 2.0.5
 Summary: A library for three-dimensional, reference-frame conversions
 Home-page: https://gitlab.com/davidwoodburn/r3f
 Author: David Woodburn
 Author-email: david.woodburn@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

