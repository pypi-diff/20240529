# Comparing `tmp/pyscsp-0.9.9.tar.gz` & `tmp/pyscsp-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscsp-0.9.9.tar", max compression
+gzip compressed data, was "pyscsp-1.0.0.tar", max compression
```

## Comparing `pyscsp-0.9.9.tar` & `pyscsp-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0      750 2023-10-02 10:54:01.268119 pyscsp-0.9.9/LICENSE.md
--rw-r--r--   0        0        0     7656 2023-10-11 04:49:06.962721 pyscsp-0.9.9/README.md
--rw-r--r--   0        0        0     1592 2023-10-13 15:16:17.887790 pyscsp-0.9.9/pyproject.toml
--rw-r--r--   0        0        0      284 2023-10-10 13:31:29.845153 pyscsp-0.9.9/pyscsp/__init__.py
--rw-r--r--   0        0        0    64814 2023-10-04 09:04:52.622575 pyscsp-0.9.9/pyscsp/discscsp.py
--rw-r--r--   0        0        0    11972 2023-10-04 09:49:41.613785 pyscsp-0.9.9/pyscsp/torchscsp.py
--rw-r--r--   0        0        0     8384 1970-01-01 00:00:00.000000 pyscsp-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0      750 2023-10-02 10:54:01.268119 pyscsp-1.0.0/LICENSE.md
+-rw-r--r--   0        0        0    14763 2024-05-29 05:45:45.731076 pyscsp-1.0.0/README.md
+-rw-r--r--   0        0        0     1592 2024-05-29 05:47:22.772843 pyscsp-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      307 2023-10-16 05:58:42.529400 pyscsp-1.0.0/pyscsp/__init__.py
+-rw-r--r--   0        0        0    20052 2024-05-29 05:17:08.158121 pyscsp-1.0.0/pyscsp/affscsp.py
+-rw-r--r--   0        0        0    86423 2024-05-29 05:16:54.410914 pyscsp-1.0.0/pyscsp/discscsp.py
+-rw-r--r--   0        0        0    34583 2024-05-29 05:17:41.892330 pyscsp-1.0.0/pyscsp/gaussders.py
+-rw-r--r--   0        0        0    23140 2024-05-29 05:17:19.101075 pyscsp-1.0.0/pyscsp/torchscsp.py
+-rw-r--r--   0        0        0    15542 1970-01-01 00:00:00.000000 pyscsp-1.0.0/PKG-INFO
```

### Comparing `pyscsp-0.9.9/LICENSE.md` & `pyscsp-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyscsp-0.9.9/pyproject.toml` & `pyscsp-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyscsp"
-version = "0.9.9"
+version = "1.0.0"
 description = "Scale-Space Toolbox for Python."
 authors = ["Tony Lindeberg <tony@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tonylindeberg/pyscsp"
 
 [tool.poetry.dependencies]
```

### Comparing `pyscsp-0.9.9/pyscsp/discscsp.py` & `pyscsp-1.0.0/pyscsp/discscsp.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """Discrete Scale Space and Scale-Space Derivative Toolbox for Python
 
 For computing discrete scale-space smoothing by convolution with the discrete
 analogue of the Gaussian kernel and for computing discrete derivative approximations
 by applying central difference operators to the smoothed data. Then, different
-types of feature detectors can be defined by combining discrete analogues of the
+types of feature detectors can be defined, by combining discrete analogues of the
 Gaussian derivative operators into differential expressions.
 
 This code is the result of porting a subset of the routines in the Matlab packages
-discscsp and discscspders to Python.
+discscsp and discscspders to Python, however, with different interfaces for some
+of the functions.
 
 Note: The scale normalization does not explicitly compensate for the additional 
 variance 1/12 for the integrated Gaussian kernel or the additional variance 1/6
 for the linearly integrated Gaussian kernel at coarser scales.
 
 References:
 
 Lindeberg (1990) "Scale-space for discrete signals", IEEE Transactions on
-Pattern Analysis and Machine Intelligence, 12(3): 234--254.
+Pattern Analysis and Machine Intelligence, 12(3): 234-254.
 
 Lindeberg (1993a) "Discrete derivative approximations with scale-space properties: 
 A basis for low-level feature detection", Journal of Mathematical Imaging and 
 Vision, 3(4): 349-376.
 
 Lindeberg (1993b) Scale-Space Theory in Computer Vision, Springer.
 
@@ -32,74 +33,76 @@
 
 Lindeberg (2009) "Scale-space". In: B. Wah (Ed.) Wiley Encyclopedia of Computer 
 Science and Engineering, John Wiley & Sons, pp. 2495-2504.
 
 Lindeberg (2015) "Image matching using generalized scale-space interest points", 
 Journal of Mathematical Imaging and Vision, 52(1): 3-36.
 
+Limitations:
+
 Compared to the original Matlab code, the following implementation is reduced 
 in the following ways:
-- there is no handling of scale normalization powers gamma that are not equal to one
-- Lp-normalization is only implemented for p = 1
-- much fewer functions of the N-jet have so far been implemented
-- there is no passing of additional parameters to functions of the N-jet
-- this reimplementation has not yet been thoroughly tested
+
+- much fewer functions of the N-jet have so far been implemented,
+- there is no passing of additional parameters to functions of the N-jet,
+- this reimplementation has not been thoroughly tested.
 """
-from math import sqrt, exp, ceil, pi
+
+
+from math import sqrt, exp, ceil, pi, cos, sin
 from typing import NamedTuple, Union, List
 import numpy as np
 from scipy.ndimage import correlate1d, correlate
 from scipy.special import ive, erf, erfcinv
 
 
 class ScSpMethod(NamedTuple):
     """Object for storing the parameters of a scale-space discretization method, 
     which can be of either of the types  'discgauss', 'samplgauss', 'normsamplgauss', 
-    'intgauss' or 'linintgauss
+    'intgauss' or 'linintgauss'
     """
     methodname: str
     epsilon: float
 
 
 class ScSpNormDerMethod(NamedTuple):
     """Object for storing the parameters of a discretization method for computing
     scale-normalized derivatives, including also the necessary parameters of the
     underlying method for discrete approximation of the Gaussian smoothing operation.
     """
     scspmethod: ScSpMethod
-    normdermethod: str # either 'nonormalization', 'varnorm' or 'Lpnorm'
-    gamma: float
+    normdermethod: str # either 'nonormalization' or 'varnorm'
 
 
 def scspnormdermethodobject(
         scspmethod : str = 'discgauss',
-        normdermethod : str = 'Lpnorm',
-        gamma : float = 1.0,
+        normdermethod : str = 'varnorm',
         epsilon : float = 0.00000001
-) -> ScSpNormDerMethod :
+    ) -> ScSpNormDerMethod :
     """Creates an object that contains the parameters of discretization method
     for computing scale-normalized derivatives, with default values for a preferred 
     choice.
     """
-    return ScSpNormDerMethod(ScSpMethod(scspmethod, epsilon), normdermethod, gamma)
+    return ScSpNormDerMethod(ScSpMethod(scspmethod, epsilon), normdermethod)
 
 
 def scspconv(
         inpic,
         sigma : float,
         scspmethod : Union[str, ScSpMethod] = 'discgauss',
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Computes the scale-space representation of the 2-D image inpic (or a 1-D signal) 
-    at scale level sigma in units of the standard deviation of the Gaussian kernel that 
-    is approximated discretely with the method scspmethod and with the formally 
+    at scale level sigma in units of the standard deviation of the Gaussian kernel, 
+    that is approximated discretely with the method scspmethod, and with the formally 
     infinite convolution operation truncated at the tails with a relative approximation 
     error less than epsilon.
 
     The following discrete approximation methods have been implemented:
+
       'discgauss' - the discrete analogue of the Gaussian kernel
       'samplgauss' - the sampled Gaussian kernel
       'normsamplgauss' - the normalized sampled Gaussian kernel
       'intgauss' - the integrated Gaussian kernel
       'linintgauss' - the linearily interpolated and integrated Gaussian kernel
 
     The discrete analogue of the Gaussian kernel has the best theoretical properties 
@@ -115,25 +118,27 @@
     'discgauss' + guarantees non-enhancement of local extrema over a 2-D image domain
                 + guarantees non-creation of new extrema from any finer to any
                   coarser level of scale over a 1-D signal domain
                 + the kernel values are guaranteed to be in the interval [0, 1]
                 + the kernel values are guaranteed to sum to 1 over an infinite domain
                 + no scale offset at all in the spatial discretization
 
-    'samplgauss' + no added scale offset in the spatial discretization
+    'samplgauss' + good approx of continuous model for sufficiently large scale values
+                 + no added scale offset in the spatial discretization
                  - the kernel values may become greater than 1 for small values of sigma
                  - the kernel values do not sum up to one
-                 - for very small values of sigma the kernels have too narrow shape
+                 - for very small values of sigma, the kernels have a too narrow shape
 
     'normsamplgauss' + no added scale offset in the spatial discretization
                      + formally the kernel values are guaranteed to be in the 
                        interval [0, 1]
                      + formally the kernel values are guaranteed to sum up to 1 
                      - the complementary normalization of the kernel is ad hoc
-                     - for very small values of sigma the kernels have too narrow shape
+                     - for very small values of sigma, the kernels have a too narrow 
+                       shape
 
     'intgauss' + the kernel values are guaranteed to be in the interval [0, 1]
                + the kernel values are guaranteed to sum up to 1 over an infinite domain
                - the box integration introduces a scale offset of 1/12 at coarser scales
 
     'linintgauss' + the kernel values are guaranteed to be in the interval [0, 1]
                   - the triangular window integration introduces a scale offset of 1/6
@@ -173,15 +178,15 @@
 
 
 def scspconv_mult(
         inpic,
         sigmavec : List[float],
         scspmethod : Union[str, ScSpMethod] = 'discgauss',
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Performs a similar function as the function scscpconv, with the 
     difference that an array of sigma values can be provided instead of a 
     single value, and that the cascade smoothing property of Gaussian 
     convolution is then made use of to perform the computational more
     efficiently than if applying the scspconv function for each
     scale level separately.
 
@@ -232,15 +237,15 @@
         raise ValueError(f'Cannot handle images of dimensionality {ndim}')
 
     return outpic
 
 
 def scaleoffset_variance(
         scspmethod : Union[str, ScSpMethod] = 'discgauss'
-) -> float :
+    ) -> float :
     """Returns the scale offset that the scale-space discretization method
     scspmethod gives rise to at coarser scales. At finer scales, however, 
     the added offset may be lower.
 
     Note that this scale offset is given in units of the variance s = sigma^2
     of the kernel, as opposed to the standard deviation sigma, motivated by
     the additive property of variances under convolution of non-negative kernels.
@@ -266,15 +271,15 @@
     return scaleoffset
 
 
 def discgaussconv(
         inpic,
         sigma : float,
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Convolves the 2-D image inpic (or a 1-D signal) with the discrete analogue of 
     the Gaussian kernel with standard deviation sigma and relative truncation error 
     less than epsilon.
 
     Convolution with this kernel corresponds to solving a spatially discretized version
     of the diffusion equation with the time variable = sigma^2 being continuous.
 
@@ -288,16 +293,16 @@
     extrema in the smoothed signal is guaranteed to not increase with scale.
 
     The spatial standard deviation of the resulting kernel is exactly equal
     to the scale parameter sigma over an infinite spatial domain. These kernel 
     values do also in the ideal infinite case exactly sum up to one, and are
     also confined in the interval [0, 1].
 
-    Reference: Lindeberg (1990) "Scale-space for discrete signals", IEEE Transactions on
-    Pattern Analysis and Machine Intelligence, 12(3): 234--254.
+    Reference: Lindeberg (1990) "Scale-space for discrete signals", IEEE Transactions 
+    on Pattern Analysis and Machine Intelligence, 12(3): 234-254.
     """
     ndim = inpic.ndim
     sep1Dfilter = make1Ddiscgaussfilter(sigma, epsilon, ndim)
 
     if ndim == 1:
         outpic = correlate1d(np.array(inpic).astype('float'), sep1Dfilter)
 
@@ -317,19 +322,19 @@
     return outpic
 
 
 def make1Ddiscgaussfilter(
         sigma : float,
         epsilon : float = 0.00000001,
         D : int = 1
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Generates a 1-D discrete analogue of the Gaussian kernel at scale level sigma
     in units of the standard deviation of the kernel and with relative truncation error
     not exceeding epsilon as a relative number over a D-dimensional spatial domain.
-"""
+    """
     s = sigma*sigma
     tmpvecsize = ceil(1 + 1.5*gaussfiltsize(sigma, epsilon, D))
 
     # Generate filter coefficients from the modified Bessel functions
     longhalffiltvec = ive(np.arange(0, tmpvecsize+1), s)
     halffiltvec = truncfilter(longhalffiltvec, truncerrtransf(epsilon, D))
     filtvec = mirrorhfilter(halffiltvec)
@@ -337,32 +342,34 @@
     return filtvec
 
 
 def samplgaussconv(
         inpic,
         sigma : float,
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Convolves the 2-D image inpic (or a 1-D signal) with the sampled Gaussian 
     kernel with standard deviation sigma and relative truncation error less than 
     epsilon.
 
     The transformation from the input image will always be a scale-space transformation,
     in the sense that for a 1-D signal the number of local extrema in the smoothed
     signal are guaranteed to not exceed the number of local extrema in the input image.
     The transformation between adjacent scale levels is, however, not guaranteed to
     be a scale-space transformation.
 
-    Note also that for smaller values of sigma, the kernel values may go outside the
-    interval [0, 1], which is not a desirable property.
+    For sufficiently large values of the scale parameter, the sampled Gaussian kernel
+    leads to good approximations of the continuous scale-space model. For smaller values 
+    of sigma, the kernel values do not, however, sum to one, and they may even go 
+    outside the interval [0, 1], which are not a desirable properties.
 
     For a theoretical explanations of these properties, see Section VII.A in
 
     Lindeberg (1990) "Scale-space for discrete signals", IEEE Transactions on
-    Pattern Analysis and Machine Intelligence, 12(3): 234--254.
+    Pattern Analysis and Machine Intelligence, 12(3): 234-254.
 
     or Section 3.6.1 in
 
     Lindeberg (1993b) Scale-Space Theory in Computer Vision, Springer.
     """
     ndim = inpic.ndim
     sep1Dfilter = make1Dsamplgaussfilter(sigma, epsilon, ndim)
@@ -386,15 +393,15 @@
     return outpic
 
 
 def make1Dsamplgaussfilter(
         sigma : float,
         epsilon : float = 0.00000001,
         D : int = 1
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Generates a sampled Gaussian kernel with standard deviation sigma, given an
     upper bound on the relative truncation error epsilon over a D-dimensional domain.
     """
     vecsize = ceil(1.1*gaussfiltsize(sigma, epsilon, D))
     x = np.linspace(-vecsize, vecsize, 1+2*vecsize)
 
     return gauss(x, sigma)
@@ -407,15 +414,15 @@
     return 1/(sqrt(2*pi)*sigma)*np.exp(-(x**2/(2*sigma**2)))
 
 
 def normsamplgaussconv(
         inpic,
         sigma : float,
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Convolves the 2-D image inpic (or a 1-D signal) with the normalized 
     sampled Gaussian kernel with standard deviation sigma and relative truncation 
     error less than epsilon.
 
     The transformation from the input image will always be a scale-space transformation,
     in the sense that for a 1-D signal the number of local extrema in the smoothed
     signal are guaranteed to not exceed the number of local extrema in the input image.
@@ -429,15 +436,15 @@
     fine scale, meaning that the normalization does not really solve the
     real problems with the sampled Gaussian kernel at very fine scales.
 
     For a theoretical explanations of the properties of the regular sampled
     Gaussian kernel, see Section VII.A in
 
     Lindeberg (1990) "Scale-space for discrete signals", IEEE Transactions on
-    Pattern Analysis and Machine Intelligence, 12(3): 234--254.
+    Pattern Analysis and Machine Intelligence, 12(3): 234-254.
 
     or Section 3.6.1 in
 
     Lindeberg (1993b) Scale-Space Theory in Computer Vision, Springer.
     """
     ndim = inpic.ndim
     sep1Dfilter = make1Dnormsamplgaussfilter(sigma, epsilon, ndim)
@@ -461,29 +468,29 @@
     return outpic
 
 
 def make1Dnormsamplgaussfilter(
         sigma : float,
         epsilon : float = 0.00000001,
         D : int = 1
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Generates a normalized sampled Gaussian kernel with standard deviation sigma, 
     given an upper bound on the relative truncation error epsilon over a D-dimensional 
     domain.
     """
     prelfilter = make1Dsamplgaussfilter(sigma, epsilon, D)
 
     return prelfilter/np.sum(prelfilter)
 
 
 def intgaussconv(
         inpic,
         sigma : float,
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Convolves the 2-D image inpic (or a 1-D signal) with the box integrated 
     Gaussian kernel with standard deviation sigma and relative truncation error less 
     than epsilon, according to Equation (3.89) on page 97 in Lindeberg (1993) 
     Scale-Space Theory  in Computer Vision, published by Springer.
 
     The transformation from the input image will always be a scale-space transformation,
     in the sense that for a 1-D signal the number of local extrema in the smoothed
@@ -526,15 +533,15 @@
     return outpic
 
 
 def make1Dintgaussfilter(
         sigma : float,
         epsilon : float = 0.00000001,
         D : int = 1
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Generates a box integrated Gaussian kernel with standard deviation sigma, 
     according to Equation (3.89) on page 97 in Lindeberg (1993) Scale-Space Theory 
     in Computer Vision (published by Springer), given an upper bound on the 
     relative truncation error epsilon over a D-dimensional domain.
 
     Remark: Adds additional spatial variance 1/12 to the kernel at coarser scales.
     """
@@ -551,15 +558,15 @@
     return 1/2*(1 + erf(x/(sqrt(2)*sigma)))
 
 
 def linintgaussconv(
         inpic,
         sigma : float,
         epsilon : float = 0.00000001
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Convolves the 2-D image inpic (or a 1-D signal) with the linearily 
     integrated Gaussian kernel with standard deviation sigma and relative 
     truncation error less than epsilon, according to Equation (3.89) on 
     page 97 in Lindeberg (1993) Scale-Space Theory  in Computer Vision, 
     published by Springer.
 
     The transformation from the input image will always be a scale-space transformation,
@@ -605,15 +612,15 @@
     return outpic
 
 
 def make1Dlinintgaussfilter(
         sigma : float,
         epsilon : float = 0.00000001,
         D : int = 1
-) -> np.ndarray :
+    ) -> np.ndarray :
     """Generates a linearily integrated Gaussian kernel with standard deviation 
     sigma, given an upper bound on the relative truncation error epsilon over a 
     D-dimensional domain.
 
     Remark: Adds additional spatial variance 1/6 to the kernel at coarser scales.
     """
     vecsize = ceil(1.1*gaussfiltsize(sigma, epsilon, D))
@@ -697,152 +704,154 @@
 
     pic[xc, yc] = 1.0
 
     return pic
 
 
 def dxmask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the first-order derivative 
-    in the x-direction.
+    """Defines a (minimal) mask for discrete approximation of the first-order 
+    derivative in the x-direction.
     """
-    return np.array([[-1/2, 0, 1/2]])
+    return np.array([[-1/2, 0, +1/2]])
 
 
 def dymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the first-order derivative 
-    in the y-direction.
+    """Defines a (minimal) mask for discrete approximation of the first-order 
+    derivative in the y-direction.
     """
     return np.array([[+1/2], \
                      [   0], \
                      [-1/2]])
 
 
 def dxxmask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the second-order derivative 
-    in the x-direction.
+    """Defines a (minimal) mask for discrete approximation of the second-order 
+    derivative in the x-direction.
     """
     return np.array([[1, -2, 1]])
 
 
 def dxymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed second-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed second-order 
     derivative in the x- and y-directions.
     """
     return np.array([[-1/4, 0, +1/4], \
                      [   0, 0,    0], \
                      [+1/4, 0, -1/4]])
 
 
 def dyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the second-order derivative 
-    in the y-direction.
+    """Defines a (minimal) mask for discrete approximation of the second-order 
+    derivative in the y-direction.
     """
     return np.array([[+1], \
                      [-2], \
                      [+1]])
 
 
 def dxxxmask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the third-order derivative 
-    in the x-direction.
+    """Defines a (minimal) mask for discrete approximation of the third-order 
+    derivative in the x-direction.
     """
-    return np.array([[-1/2, 1, 0, -1, 1/2]])
+    return np.array([[-1/2, +1, 0, -1, 1/2]])
 
 
 def dxxymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed third-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed third-order 
     derivative corresponding to a second-order derivative in the x-direction 
     and a first-order derivative in the y-direction.
     """
     return np.array([[+1/2, -1, +1/2], \
                      [   0,  0,    0], \
                      [-1/2, +1, -1/2]])
 
 
 def dxyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed third-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed third-order 
     derivative corresponding to a first-order derivative in the x-direction 
     and a second-order derivative in the y-direction.
     """
     return np.array([[-1/2, 0, +1/2], \
                      [  +1, 0,   -1], \
                      [-1/2, 0, +1/2]])
 
 
 def dyyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the third-order derivative 
-    in the y-direction.
+    """Defines a (minimal) mask for discrete approximation of the third-order 
+    derivative in the y-direction.
     """
     return np.array([[+1/2], \
                      [  -1], \
                      [   0], \
                      [  +1], \
                      [-1/2]])
 
 
 def dxxxxmask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the fourth-order derivative 
-    in the x-direction.
+    """Defines a (minimal) mask for discrete approximation of the fourth-order 
+    derivative in the x-direction.
     """
     return np.array([[1, -4, 6, -4, 1]])
 
 
 def dxxxymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed fourth-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed fourth-order 
     derivative corresponding to a third-order derivative in the x-direction and 
     a first-order derivative in the y-direction.
     """
     return np.array([[-1/4, +1/2, 0, -1/2, +1/4], \
                      [   0,    0, 0,    0,    0], \
                      [+1/4, -1/2, 0, +1/2, -1/4]])
 
 
 def dxxyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed fourth-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed fourth-order 
     derivative corresponding to a second-order derivatives in the x- and y-directions.
     """
     return np.array([[+1, -2, +1], \
                      [-2, +4, -2], \
                      [+1, -2, +1]])
 
 
 def dxyyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the mixed fourth-order 
+    """Defines a (minimal) mask for discrete approximation of the mixed fourth-order 
     derivative corresponding to a first-order derivative in the x-direction and 
     a third-order derivative in the y-direction.
     """
     return np.array([[-1/4, 0, +1/4], \
                      [+1/2, 0, -1/2], \
                      [   0, 0,    0], \
                      [-1/2, 0, +1/2], \
                      [+1/4, 0, -1/4]])
 
 
 def dyyyymask() -> np.ndarray :
-    """Defines a mask for discrete approximation of the fourth-order derivative 
-    in the y-direction.
+    """Defines a (minimal) mask for discrete approximation of the fourth-order 
+    derivative in the y-direction.
     """
     return np.array([[+1], \
                      [-4], \
                      [+6], \
                      [-4], \
                      [+1]])
 
 
 def computeNjetfcn(
         inpic,
         njetfcn : str,
         sigma : float,
-        normdermethod : Union[str, ScSpNormDerMethod] = 'discgaussLp'
-) -> np.ndarray :
+        normdermethod : Union[str, ScSpNormDerMethod] = 'discgauss',
+        gamma : float = 1.0
+    ) -> np.ndarray :
     """Computes an N-jet function in terms of scale-normalized Gaussian derivatives 
     of the image inpic at scale level sigma in units of the standard deviation of
     the Gaussian kernel, and using the scale normalization method normdermethod.
 
     Implemented N-jet functions:
+
       'L' - smoothed scale-space representation
       'Lx' - 1:st-order partial derivative in x-direction
       'Ly' - 1:st-order partial derivative in y-direction
       'Lxx' - 2:nd-order partial derivative in x-direction
       'Lxy' - mixed 2nd-order partial derivative in x- and y-directions
       'Lyy' - 2:nd-order partial derivative in y-direction
       'Lv' - gradient magnitude
@@ -853,14 +862,15 @@
       'Kappa' - rescaled level curve curvature
       'Lv2Lvv' - 2:nd-order directional derivative in gradient direction * Lv^2
       'Lv3Lvvv' - 3:rd-order directional derivative in gradient direction * Lv^3
       'Lp' - 1:st-order directional derivative in 1:st principal curvature direction
       'Lq' - 1:st-order directional derivative in 2:nd principal curvature direction
       'Lpp' - 2:nd-order directional derivative in 1:st principal curvature direction
       'Lqq' - 2:nd-order directional derivative in 2:nd principal curvature direction
+
     In addition, 3:rd- and 4:th-order partial derivatives are also implemented.
 
     The differential expressions 'Lv', 'Lv2', 'Lv2Lvv' and 'Lv3Lvvv' are used in
     methods for edge detection. The differential expressions 'Laplace', 'detHessian'
     and 'sqrtdetHessian' are used in methods for interest point detection, 
     blob detection and corner detection. The differential expressions 'Lp', 'Lq',
     'Lpp' and 'Lqq' are used in methods for ridge detection.
@@ -878,29 +888,31 @@
     applying the function applyNjetfcn() multiple times for each N-jetfcn.
     """
     if isinstance(normdermethod, str):
         normdermethod = defaultscspnormdermethodobject(normdermethod)
 
     smoothpic = scspconv(inpic, sigma, normdermethod.scspmethod)
 
-    return applyNjetfcn(smoothpic, njetfcn, sigma, normdermethod)
+    return applyNjetfcn(smoothpic, njetfcn, sigma, normdermethod, gamma)
 
 
 def applyNjetfcn(
         smoothpic : np.ndarray,
         njetfcn : str,
         sigma : float = 1.0,
-        normdermethod : Union[str, ScSpNormDerMethod] = 'discgaussLp'
-) -> np.ndarray :
+        normdermethod : Union[str, ScSpNormDerMethod] = 'discgauss',
+        gamma : float = 1.0
+    ) -> np.ndarray :
     """Applies an N-jet function in terms of scale-normalized Gaussian derivatives 
     to an already computed scale-space representation at scale level sigma in units
     of the standard deviation of the Gaussian kernel, and using the scale normalization
     method normdermethod.
 
     Implemented N-jet functions:
+
       'L' - smoothed scale-space representation
       'Lx' - 1:st-order partial derivative in x-direction
       'Ly' - 1:st-order partial derivative in y-direction
       'Lxx' - 2:nd-order partial derivative in x-direction
       'Lxy' - mixed 2nd-order partial derivative in x- and y-directions
       'Lyy' - 2:nd-order partial derivative in y-direction
       'Lv' - gradient magnitude
@@ -912,14 +924,16 @@
       'Lv2Lvv' - 2:nd-order directional derivative in gradient direction * Lv^2
       'Lv3Lvvv' - 3:rd-order directional derivative in gradient direction * Lv^3
       'Lp' - 1:st-order directional derivative in 1:st principal curvature direction
       'Lq' - 1:st-order directional derivative in 2:nd principal curvature direction
       'Lpp' - 2:nd-order directional derivative in 1:st principal curvature direction
       'Lqq' - 2:nd-order directional derivative in 2:nd principal curvature direction
 
+    In addition, 3:rd- and 4:th-order partial derivatives are also implemented.
+
     The differential expressions 'Lv', 'Lv2', 'Lv2Lvv' and 'Lv3Lvvv' are used in
     methods for edge detection. The differential expressions 'Laplace', 'detHessian'
     and 'sqrtdetHessian' are used in methods for interest point detection, 
     blob detection and corner detection. The differential expressions 'Lp', 'Lq',
     'Lpp' and 'Lqq' are used in methods for ridge detection.
 
     The derivatives in the (u, v)-coordinates are based on Equations (6)-(7) in
@@ -940,235 +954,236 @@
               applyNjetfcn(smoothpic[:, :, layer], njetfcn, sigma, normdermethod)
 
     else:
         if njetfcn == 'L':
             outpic = smoothpic
 
         elif njetfcn == 'Lx':
-            outpic = normderfactor(1, 0, sigma, normdermethod) * \
+            outpic = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxmask())
 
         elif njetfcn == 'Ly':
-            outpic = normderfactor(0, 1, sigma, normdermethod) * \
+            outpic = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dymask())
 
         elif njetfcn == 'Lxx':
-            outpic = normderfactor(2, 0, sigma, normdermethod) * \
+            outpic = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxmask())
 
         elif njetfcn == 'Lxy':
-            outpic = normderfactor(1, 1, sigma, normdermethod) * \
+            outpic = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxymask())
 
         elif njetfcn == 'Lyy':
-            outpic = normderfactor(0, 2, sigma, normdermethod) * \
+            outpic = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dyymask())
 
         elif njetfcn == 'Lv':
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
             outpic = np.sqrt(Lx*Lx + Ly*Ly)
 
         elif njetfcn == 'Lv2':
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
             outpic = Lx*Lx + Ly*Ly
 
         elif njetfcn == 'Laplace':
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = Lxx + Lyy
 
         elif njetfcn == 'detHessian':
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = Lxx*Lyy - Lxy*Lxy
 
         elif njetfcn == 'sqrtdetHessian':
             # Signed square root of absolute value of the determinant of the Hessian
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             detHessian = Lxx*Lyy - Lxy*Lxy
             outpic = np.sign(detHessian) * np.sqrt(np.abs(detHessian))
 
         elif njetfcn == 'Kappa':
             # Rescaled level curve curvature
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = Ly*Ly*Lxx + Lx*Lx*Lyy - 2*Lx*Ly*Lxy
 
         elif njetfcn == 'Lv2Lvv':
             # 2nd-order derivative in gradient direction (used for edge detection)
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = Lx*Lx*Lxx + 2*Lx*Ly*Lxy + Ly*Ly*Lyy
 
         elif njetfcn == 'Lv3Lvvv':
             # 3rd-order derivative in gradient direction (used for edge detection)
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
-            Lxxx = normderfactor(3, 0, sigma, normdermethod) * \
+            Lxxx = normderfactor(3, 0, sigma, normdermethod, gamma) * \
                    correlate(smoothpic, dxxxmask())
-            Lxxy = normderfactor(2, 1, sigma, normdermethod) * \
+            Lxxy = normderfactor(2, 1, sigma, normdermethod, gamma) * \
                    correlate(smoothpic, dxxymask())
-            Lxyy = normderfactor(1, 2, sigma, normdermethod) * \
+            Lxyy = normderfactor(1, 2, sigma, normdermethod, gamma) * \
                    correlate(smoothpic, dxyymask())
-            Lyyy = normderfactor(0, 3, sigma, normdermethod) * \
+            Lyyy = normderfactor(0, 3, sigma, normdermethod, gamma) * \
                    correlate(smoothpic, dyyymask())
             outpic = Lx*Lx*Lx*Lxxx + 3*Lx*Lx*Ly*Lxxy + \
                      3*Lx*Ly*Ly*Lxyy + Ly*Ly*Ly*Lyyy
 
         elif njetfcn == 'Lp':
             # 1st-order derivative in first principal curvature direction
             # (used for ridge detection)
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             tmp = (Lxx - Lyy) /(np.finfo(float).eps + \
                                 np.sqrt((Lxx - Lyy)*(Lxx - Lyy) + 4*Lxy*Lxy))
             cosbeta = np.sqrt((1 + tmp)/2)
             sinbeta = np.sign(Lxy) * np.sqrt((1 - tmp)/2)
             outpic = sinbeta * Lx - cosbeta * Ly
 
         elif njetfcn == 'Lq':
             # 1st-order derivative in second principal curvature
             # (used for valley detection)
-            Lx = normderfactor(1, 0, sigma, normdermethod) * \
+            Lx = normderfactor(1, 0, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dxmask())
-            Ly = normderfactor(0, 1, sigma, normdermethod) * \
+            Ly = normderfactor(0, 1, sigma, normdermethod, gamma) * \
                  correlate(smoothpic, dymask())
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             tmp = (Lxx - Lyy) /(np.finfo(float).eps + \
                                 np.sqrt((Lxx - Lyy)*(Lxx - Lyy) + 4*Lxy*Lxy))
             cosbeta = np.sqrt((1 + tmp)/2)
             sinbeta = np.sign(Lxy) * np.sqrt((1 - tmp)/2)
             outpic = cosbeta * Lx + sinbeta * Ly
 
         elif njetfcn == 'Lpp':
             # 2nd-order derivative in first principal curvature direction
             # (used for ridge detection)
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = ((Lxx + Lyy) - \
                       np.sqrt((Lxx - Lyy)*(Lxx - Lyy) + 4*Lxy*Lxy))/2
 
         elif njetfcn == 'Lqq':
             # 2nd-order derivative in second principal curvature direction
             # (used for valley detection)
-            Lxx = normderfactor(2, 0, sigma, normdermethod) * \
+            Lxx = normderfactor(2, 0, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxxmask())
-            Lxy = normderfactor(1, 1, sigma, normdermethod) * \
+            Lxy = normderfactor(1, 1, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dxymask())
-            Lyy = normderfactor(0, 2, sigma, normdermethod) * \
+            Lyy = normderfactor(0, 2, sigma, normdermethod, gamma) * \
                   correlate(smoothpic, dyymask())
             outpic = ((Lxx + Lyy) + \
                       np.sqrt((Lxx - Lyy)*(Lxx - Lyy) + 4*Lxy*Lxy))/2
 
         elif njetfcn == 'Lxxx':
-            outpic = normderfactor(3, 0, sigma, normdermethod) * \
+            outpic = normderfactor(3, 0, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxxmask())
 
         elif njetfcn == 'Lxxy':
-            outpic = normderfactor(2, 1, sigma, normdermethod) * \
+            outpic = normderfactor(2, 1, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxymask())
 
         elif njetfcn == 'Lxyy':
-            outpic = normderfactor(1, 2, sigma, normdermethod) * \
+            outpic = normderfactor(1, 2, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxyymask())
 
         elif njetfcn == 'Lyyy':
-            outpic = normderfactor(0, 3, sigma, normdermethod) * \
+            outpic = normderfactor(0, 3, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dyyymask())
 
         elif njetfcn == 'Lxxxx':
-            outpic = normderfactor(4, 0, sigma, normdermethod) * \
+            outpic = normderfactor(4, 0, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxxxmask())
 
         elif njetfcn == 'Lxxxy':
-            outpic = normderfactor(3, 1, sigma, normdermethod) * \
+            outpic = normderfactor(3, 1, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxxymask())
 
         elif njetfcn == 'Lxxyy':
-            outpic = normderfactor(2, 2, sigma, normdermethod) * \
+            outpic = normderfactor(2, 2, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxxyymask())
 
         elif njetfcn == 'Lxyyy':
-            outpic = normderfactor(1, 3, sigma, normdermethod) * \
+            outpic = normderfactor(1, 3, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dxyyymask())
 
         elif njetfcn == 'Lyyyy':
-            outpic = normderfactor(0, 4, sigma, normdermethod) * \
+            outpic = normderfactor(0, 4, sigma, normdermethod, gamma) * \
                      correlate(smoothpic, dyyyymask())
 
         else:
             raise ValueError(f'NJetFcn {njetfcn} not implemented')
 
     return outpic
 
 
 def normderfactor(
         xorder : int,
         yorder : int,
         sigma : float,
-        normdermethod : Union[str, ScSpNormDerMethod]
-) -> float :
+        normdermethod : Union[str, ScSpNormDerMethod],
+        gamma : float = 1.0
+    ) -> float :
     """Compute the scale normalization factor for the scale-normalied 
     Gaussian derivative of order xorder in the x-direction and of order yorder 
     in the y-direction at scale sigma in units of the standard deviation of 
     the Gaussian kernel and using the scale normalization method normdermethod.
     """
     if isinstance(normdermethod, str):
         normdermethod = defaultscspnormdermethodobject(normdermethod)
@@ -1177,98 +1192,28 @@
         value = 1.0
 
     elif normdermethod.normdermethod == 'varnorm':
         # ==>> Here it could be natural to compensate for the additional variance
         # ==>> for the integrated or linearly integrated Gaussian kernels.
         # ==>> That added variance is, however, scale-dependent, which then
         # ==>> requires a separate calibration for each scale value
-        value = sigma**(xorder + yorder)
-
-    elif normdermethod.normdermethod == 'Lpnorm':
-        if normdermethod.scspmethod.methodname == 'discgauss':
-            if normdermethod.gamma == 1.0:
-                value = \
-                (normgaussder1D_L1norm(xorder, sigma) * \
-                normgaussder1D_L1norm(yorder, sigma)) / \
-                (discgaussder1D_L1norm(xorder, sigma, \
-                                      normdermethod.scspmethod.epsilon) * \
-                discgaussder1D_L1norm(yorder, sigma, \
-                                      normdermethod.scspmethod.epsilon))
-            else:
-                raise ValueError('Lp-normalization so far only implemented \
-for gamma = 1.0')
-
-        elif normdermethod.scspmethod.methodname == 'samplgauss':
-            if normdermethod.gamma == 1.0:
-                value = \
-                (normgaussder1D_L1norm(xorder, sigma) * \
-                normgaussder1D_L1norm(yorder, sigma)) / \
-                (samplgaussder1D_L1norm(xorder, sigma, \
-                                        normdermethod.scspmethod.epsilon) * \
-                samplgaussder1D_L1norm(yorder, sigma, \
-                                       normdermethod.scspmethod.epsilon))
-            else:
-                raise ValueError('Lp-normalization so far only implemented \
-for gamma = 1.0')
-
-        elif normdermethod.scspmethod.methodname == 'normsamplgauss':
-            if normdermethod.gamma == 1.0:
-                value = \
-                (normgaussder1D_L1norm(xorder, sigma) * \
-                normgaussder1D_L1norm(yorder, sigma)) / \
-                (normsamplgaussder1D_L1norm(xorder, sigma, \
-                                            normdermethod.scspmethod.epsilon) * \
-                 normsamplgaussder1D_L1norm(yorder, sigma, \
-                                            normdermethod.scspmethod.epsilon))
-            else:
-                raise ValueError('Lp-normalization so far only implemented \
-for gamma = 1.0')
-
-        elif normdermethod.scspmethod.methodname == 'intgauss':
-            if normdermethod.gamma == 1.0:
-                value = \
-                (normgaussder1D_L1norm(xorder, sigma) * \
-                normgaussder1D_L1norm(yorder, sigma)) / \
-                (intgaussder1D_L1norm(xorder, sigma, \
-                                      normdermethod.scspmethod.epsilon) * \
-                intgaussder1D_L1norm(yorder, sigma, \
-                                     normdermethod.scspmethod.epsilon))
-            else:
-                raise ValueError('Lp-normalization so far only implemented \
-for gamma = 1.0')
-
-        elif normdermethod.scspmethod.methodname == 'linintgauss':
-            if normdermethod.gamma == 1.0:
-                value = \
-                (normgaussder1D_L1norm(xorder, sigma) * \
-                normgaussder1D_L1norm(yorder, sigma)) / \
-                (linintgaussder1D_L1norm(xorder, sigma, \
-                                         normdermethod.scspmethod.epsilon) * \
-                linintgaussder1D_L1norm(yorder, sigma, \
-                                        normdermethod.scspmethod.epsilon))
-            else:
-                raise ValueError('Lp-normalization so far only implemented \
-for gamma = 1.0')
-
-        else:
-            raise ValueError(f'Lp-normalization not implemented for \
-scale-space derivative method {normdermethod.scspmethod.methodname}')
+        value = sigma**(gamma*(xorder + yorder))
 
     else:
         raise ValueError(f'Derivative method {normdermethod.normdermethod} \
 not implemented')
 
     return value
 
 
 def normgaussder1D_L1norm(
         order : int,
         sigma : float,
         gammapar : float = 1.0
-) -> float :
+    ) -> float :
     """Returns the L_1-norm of 1-D gamma-normalized Gaussian derivative 
     of order sigma and at scale sigma in units of the standard deviation of 
     the Gaussian kernel, using the scale normalization parameter gammapar.
 
     Based on Equations (74)-(77) in Lindeberg (1998) "Feature Detection with 
     Automatic Scale Selection", International Journal of Computer Vision,
     30(2): 79-116, combined by gamma-normalization of the scale-normalized
@@ -1282,15 +1227,15 @@
     elif order == 1:
         value = sqrt(2/pi) * s**((gammapar - 1)/2)
 
     elif order == 2:
         value = 2*sqrt(2/(exp(1)*pi)) * s**(gammapar - 1)
 
     elif order == 3:
-        value = (4 + exp(3/2))*sqrt(2/pi)/exp(3/2) * s**(3*(gammapar - 1)/2)
+        value = (4 + exp(3/2)) * sqrt(2/pi) / exp(3/2) * s**(3*(gammapar - 1)/2)
 
     elif order == 4:
         value = \
           2*exp(-3/2 - sqrt(3/2)) * \
           (2*exp(sqrt(6))*sqrt((9 - 3*sqrt(6))/pi) \
                + 3*sqrt((3 - sqrt(6))/pi) \
           + sqrt(6*(3 - sqrt(6))/pi) \
@@ -1298,227 +1243,66 @@
 
     else:
         raise ValueError(f'Not implemented for order {order}')
 
     return value
 
 
-def discgaussder1D_L1norm(
-        order : int,
-        sigma : float,
-        epsilon : float = 0.00000001
-) -> float :
-    """Returns the L_1-norm of the n:th-order difference of the 1-D discrete analogue 
-    of the Gaussian kernel at scale level sigma in units of the standard deviation and 
-    truncated at the tails with a relative approximation error less than epsilon.
-    """
-    smoothkernel = make1Ddiscgaussfilter(sigma, epsilon, 1)
-
-    if order == 0:
-        derkernel = smoothkernel
-
-    elif order == 1:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 0, 1/2]))
-
-    elif order == 2:
-        derkernel = correlate1d(smoothkernel, np.array([1, -2, 1]))
-
-    elif order == 3:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 1, 0, -1, 1/2]))
-
-    elif order == 4:
-        derkernel = correlate1d(smoothkernel, np.array([1, -4, 6, -4, 1]))
-
-    else:
-        raise ValueError(f'Not implemented for order {order}')
-
-    return sum(abs(derkernel))
-
-
-def samplgaussder1D_L1norm(
-        order : int,
-        sigma : float,
-        epsilon : float = 0.00000001
-) -> float :
-    """Returns the L_1-norm of the n:th-order difference of the 1-D sampled 
-    Gaussian kernel at scale level sigma in units of the standard deviation and 
-    truncated at the tails with a relative approximation error less than epsilon.
-    """
-    smoothkernel = make1Dsamplgaussfilter(sigma, epsilon, 1)
-
-    if order == 0:
-        derkernel = smoothkernel
-
-    elif order == 1:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 0, 1/2]))
-
-    elif order == 2:
-        derkernel = correlate1d(smoothkernel, np.array([1, -2, 1]))
-
-    elif order == 3:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 1, 0, -1, 1/2]))
-
-    elif order == 4:
-        derkernel = correlate1d(smoothkernel, np.array([1, -4, 6, -4, 1]))
-
-    else:
-        raise ValueError(f'Not implemented for order {order}')
-
-    return sum(abs(derkernel))
-
-
-def normsamplgaussder1D_L1norm(
-        order : int,
-        sigma : float,
-        epsilon : float = 0.00000001
-) -> float :
-    """Returns the L_1-norm of the n:th-order difference of the 1-D sampled 
-    Gaussian kernel at scale level sigma in units of the standard deviation and 
-    truncated at the tails with a relative approximation error less than epsilon.
-    """
-    smoothkernel = make1Dnormsamplgaussfilter(sigma, epsilon, 1)
-
-    if order == 0:
-        derkernel = smoothkernel
-
-    elif order == 1:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 0, 1/2]))
-
-    elif order == 2:
-        derkernel = correlate1d(smoothkernel, np.array([1, -2, 1]))
-
-    elif order == 3:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 1, 0, -1, 1/2]))
-
-    elif order == 4:
-        derkernel = correlate1d(smoothkernel, np.array([1, -4, 6, -4, 1]))
-
-    else:
-        raise ValueError(f'Not implemented for order {order}')
-
-    return sum(abs(derkernel))
-
-
-def intgaussder1D_L1norm(
-        order : int,
-        sigma : float,
-        epsilon : float = 0.00000001
-) -> float :
-    """Returns the L_1-norm of the n:th-order difference of the 1-D integrated 
-    Gaussian kernel at scale level sigma in units of the standard deviation and 
-    truncated at the tails with a relative approximation error less than epsilon.
-    """
-    smoothkernel = make1Dintgaussfilter(sigma, epsilon, 1)
-
-    if order == 0:
-        derkernel = smoothkernel
-
-    elif order == 1:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 0, 1/2]))
-
-    elif order == 2:
-        derkernel = correlate1d(smoothkernel, np.array([1, -2, 1]))
-
-    elif order == 3:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 1, 0, -1, 1/2]))
-
-    elif order == 4:
-        derkernel = correlate1d(smoothkernel, np.array([1, -4, 6, -4, 1]))
-
-    else:
-        raise ValueError(f'Not implemented for order {order}')
-
-    return sum(abs(derkernel))
-
-
-def linintgaussder1D_L1norm(
-        order : int,
-        sigma : float,
-        epsilon : float = 0.00000001
-) -> float :
-    """Returns the L_1-norm of the n:th-order difference of the 1-D linearly 
-    integrated Gaussian kernel at scale level sigma in units of the standard deviation 
-    and truncated at the tails with a relative approximation error less than epsilon.
-    """
-    smoothkernel = make1Dlinintgaussfilter(sigma, epsilon, 1)
-
-    if order == 0:
-        derkernel = smoothkernel
-
-    elif order == 1:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 0, 1/2]))
-
-    elif order == 2:
-        derkernel = correlate1d(smoothkernel, np.array([1, -2, 1]))
+def Lpnorm(
+        discfilter : np.ndarray,
+        p : float
+    ) -> float :
+    """Computes the lp-norm of a discrete filter"""
 
-    elif order == 3:
-        derkernel = correlate1d(smoothkernel, np.array([-1/2, 1, 0, -1, 1/2]))
+    return (np.sum(np.abs(discfilter))**p)**(1/p)
 
-    elif order == 4:
-        derkernel = correlate1d(smoothkernel, np.array([1, -4, 6, -4, 1]))
 
-    else:
-        raise ValueError(f'Not implemented for order {order}')
+def L1norm(discfilter : np.ndarray) -> float :
+    """Computes the l1-norm of a discrete filter"""
 
-    return sum(abs(derkernel))
+    return np.sum(np.abs(discfilter))
 
 
 def defaultscspnormdermethodobject(
-        scspnormdermethod : str = 'discgaussLp',
-        gamma : float = 1.0
-) -> ScSpNormDerMethod :
+        scspnormdermethod : str = 'discgaussvar'
+    ) -> ScSpNormDerMethod :
     """Converts a user-friendly string for a method for approximating 
     scale-normalized derivatives for discrete data to a class object, including 
     also a specification of the discretization method to use for discrete 
     approximation of the underlying spatial smoothing operation
     """
     if scspnormdermethod == 'discgauss':
-        obj = scspnormdermethodobject('discgauss', 'nonormalization', gamma)
+        obj = scspnormdermethodobject('discgauss', 'nonormalization')
 
     elif scspnormdermethod == 'discgaussvar':
-        obj = scspnormdermethodobject('discgauss', 'varnorm', gamma)
-
-    elif scspnormdermethod == 'discgaussLp':
-        obj = scspnormdermethodobject('discgauss', 'Lpnorm', gamma)
+        obj = scspnormdermethodobject('discgauss', 'varnorm')
 
     elif scspnormdermethod == 'samplgauss':
-        obj = scspnormdermethodobject('samplgauss', 'nonormalization', gamma)
+        obj = scspnormdermethodobject('samplgauss', 'nonormalization')
 
     elif scspnormdermethod == 'samplgaussvar':
-        obj = scspnormdermethodobject('samplgauss', 'varnorm', gamma)
-
-    elif scspnormdermethod == 'samplgaussLp':
-        obj = scspnormdermethodobject('samplgauss', 'Lpnorm', gamma)
+        obj = scspnormdermethodobject('samplgauss', 'varnorm')
 
     elif scspnormdermethod == 'normsamplgauss':
-        obj = scspnormdermethodobject('normsamplgauss', 'nonormalization', gamma)
+        obj = scspnormdermethodobject('normsamplgauss', 'nonormalization')
 
     elif scspnormdermethod == 'normsamplgaussvar':
-        obj = scspnormdermethodobject('normsamplgauss', 'varnorm', gamma)
-
-    elif scspnormdermethod == 'normsamplgaussLp':
-        obj = scspnormdermethodobject('normsamplgauss', 'Lpnorm', gamma)
+        obj = scspnormdermethodobject('normsamplgauss', 'varnorm')
 
     elif scspnormdermethod == 'intgauss':
-        obj = scspnormdermethodobject('intgauss', 'nonormalization', gamma)
+        obj = scspnormdermethodobject('intgauss', 'nonormalization')
 
     elif scspnormdermethod == 'intgaussvar':
-        obj = scspnormdermethodobject('intgauss', 'varnorm', gamma)
-
-    elif scspnormdermethod == 'intgaussLp':
-        obj = scspnormdermethodobject('intgauss', 'Lpnorm', gamma)
+        obj = scspnormdermethodobject('intgauss', 'varnorm')
 
     elif scspnormdermethod == 'linintgauss':
-        obj = scspnormdermethodobject('linintgauss', 'nonormalization', gamma)
+        obj = scspnormdermethodobject('linintgauss', 'nonormalization')
 
     elif scspnormdermethod == 'linintgaussvar':
-        obj = scspnormdermethodobject('linintgauss', 'varnorm', gamma)
-
-    elif scspnormdermethod == 'linintgaussLp':
-        obj = scspnormdermethodobject('linintgauss', 'Lpnorm', gamma)
+        obj = scspnormdermethodobject('linintgauss', 'varnorm')
 
     else:
         raise ValueError(f'Scale-space derivative method {scspnormdermethod} \
 not implemented')
 
     return obj
 
@@ -1540,14 +1324,17 @@
 
     if ysize % 2:
         y = np.linspace(-(ysize-1)/2, (ysize-1)/2, ysize)
     else:
         # Choose convention to fit deltafcn()
         y = np.linspace(-ysize/2, ysize/2-1, ysize)
 
+    # According to our convention, the y-direction goes in the upward direction
+    y = -y
+
     xv, yv = np.meshgrid(x, y, indexing='xy')
 
     x2mom = np.sum(np.sum(xv * xv * spatfilter))/np.sum(np.sum(spatfilter))
     xymom = np.sum(np.sum(xv * yv * spatfilter))/np.sum(np.sum(spatfilter))
     y2mom = np.sum(np.sum(yv * yv * spatfilter))/np.sum(np.sum(spatfilter))
 
     xmean, ymean = filtermean(spatfilter)
@@ -1573,14 +1360,17 @@
 
     if ysize % 2:
         y = np.linspace(-(ysize-1)/2, (ysize-1)/2, ysize)
     else:
         # Choose convention to fit deltafcn()
         y = np.linspace(-ysize/2, ysize/2-1, ysize)
 
+    # According to our convention, the y-direction goes in the upward direction
+    y = -y
+
     xv, yv = np.meshgrid(x, y, indexing='xy')
 
     xmean = np.sum(np.sum(xv * spatfilter))/np.sum(np.sum(spatfilter))
     ymean = np.sum(np.sum(yv * spatfilter))/np.sum(np.sum(spatfilter))
 
     return xmean, ymean
 
@@ -1627,7 +1417,764 @@
 
 def RGB2L(inpic) -> np.ndarray:
     """Converts an RGB colour image to a greylevel image.
     """
     inpic = np.array(inpic).astype('float')
 
     return (inpic[:, :, 0] + inpic[:, :, 1] + inpic[:, :, 2])/3.0
+
+
+def applydirder(
+        smoothpic : np.ndarray,
+        phi : float,
+        phiorder : int,
+        orthorder : int = 0,
+        sigma : float = 1.0,
+        normdermethod : str = 'varnorm'
+    ) -> np.ndarray :
+    """Applies a directional derivative, of order phiorder in the direction phi
+    and of order orthorder in the orthogonal direction, to the input image.
+
+    The directional operator is defined as
+
+    D_phi^phiorder D_orth^orthorder
+
+    for
+
+    D_phi  =  cos phi D_x + sin phi D_y
+    D_orth = -sin phi D_x + cos phi D_y
+
+    where D_x and D_y constitute (discrete approximations of) partial derivative
+    operators along the x- and y-directions, respectively.
+
+    The intention is that if this operation is applied to image data, then
+    it should be preceeded by a call to the spatial smoothing operation,
+    as can be performed by e.g. the function scspconv(). If you want to
+    make use of scale-normalized derivatives, the parameter sigma should
+    then describe the value of the spatial scale parameter used for spatial
+    smoothing in units of the standard deviation of the kernel.
+
+    References:
+
+    Lindeberg (1993) "Scale-Space Theory in Computer Vision", Springer.
+    (See Equation (5.54) on page 139.)
+
+    Lindeberg (2013) "A computational theory of visual receptive fields", 
+    Biological Cybernetics, 107(6): 589-635. (See Equation (69).)
+
+    Lindeberg (2021) "Normative theory of visual receptive fields", 
+    Heliyon 7(1): e05897: 1-20. (See Equation (31) and the explanation
+    to Equation (23).)
+    """
+    # Determine a directional derivative approximation mask
+    mask = dirdermask(phi, phiorder, orthorder)
+
+    # Determine the scale normalization factor
+    if normdermethod == 'varnorm':
+        scalenormfactor = sigma**(phiorder + orthorder)
+    elif normdermethod == 'nonormalization':
+        scalenormfactor = 1.0
+    else:
+        raise ValueError(f'Scale normalization method {normdermethod} not implemented')
+
+    return scalenormfactor * correlate(smoothpic, mask)
+
+
+def dirdermask(
+        phi : float,
+        phiorder : int,
+        orthorder : int = 0,
+    ) -> np.ndarray :
+    """Returns a directional derivative mask of order phiorder in the direction phi
+    and order orthorder in the orthogonal direction.
+
+    The mask will be of size 3 x 3 if the total order of differentiation is either
+    1 or 2, whereas the mask will be of size 5 x 5 if the total order of differentiation
+    is either 3 or 4. If the total order of differentiation is 0, then the mask will 
+    be of size 1 x 1.
+    """
+    if (phiorder == 1) and (orthorder == 0):
+        return dphi_mask(phi)
+    if (phiorder == 2) and (orthorder == 0):
+        return dphiphi_mask(phi)
+    if (phiorder == 0) and (orthorder == 1):
+        return dorth_mask(phi)
+    if (phiorder == 0) and (orthorder == 2):
+        return dorthorth_mask(phi)
+    if (phiorder == 1) and (orthorder == 1):
+        return dphiorth_mask(phi)
+    if (phiorder == 3) and (orthorder == 0):
+        return dphiphiphi_mask(phi)
+    if (phiorder == 2) and (orthorder == 1):
+        return dphiphiorth_mask(phi)
+    if (phiorder == 1) and (orthorder == 2):
+        return dphiorthorth_mask(phi)
+    if (phiorder == 0) and (orthorder == 3):
+        return dorthorthorth_mask(phi)
+    if (phiorder == 4) and (orthorder == 0):
+        return dphiphiphiphi_mask(phi)
+    if (phiorder == 3) and (orthorder == 1):
+        return dphiphiphiorth_mask(phi)
+    if (phiorder == 2) and (orthorder == 2):
+        return dphiphiorthorth_mask(phi)
+    if (phiorder == 1) and (orthorder == 3):
+        return dphiorthorthorth_mask(phi)
+    if (phiorder == 0) and (orthorder == 4):
+        return dorthorthorthorth_mask(phi)
+    if (phiorder == 0) and (orthorder == 0):
+        return np.array([[1]])
+
+    raise ValueError(f"Not implemented directional derivatives of order \
+                     (phiorder {phiorder}) and (orthorder {orthorder})")
+
+
+def dphi_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the first-order directional 
+    derivative in the orientation phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer.
+    """
+    return cos(phi) * dxmask3() + sin(phi) * dymask3()
+
+
+def dphiphi_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the second-order directional 
+    derivative in the orientation phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer.
+    """
+    return cos(phi)**2 * dxxmask3() + \
+           2*cos(phi)*sin(phi) * dxymask3() + \
+           sin(phi)**2 * dyymask3()
+
+
+def dorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the first-order directional 
+    derivative in a perpendicular orientation to phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return -sin(phi) * dxmask3() + cos(phi) * dymask3()
+
+
+def dorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the second-order directional 
+    derivative in a perpendicular orientation to phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return sin(phi)**2 * dxxmask3() \
+           - 2*cos(phi)*sin(phi) * dxymask3() \
+           + cos(phi)**2 * dyymask3()
+
+
+def dphiorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed second-order directional 
+    derivative in the directions of phi and its perpendicular orientation.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return cos(phi)*sin(phi) * (dyymask3() - dxxmask3()) \
+           + (cos(phi)**2 - sin(phi)**2) * dxymask3()
+
+
+def dxmask3() -> np.ndarray :
+    """Defines a mask of size 3 x 3 for discrete approximation of the 
+    first-order derivative in the x-direction.
+    """
+    return np.array([[  0,  0,   0 ], \
+                     [-1/2, 0, +1/2], \
+                     [  0,  0,   0 ]])
+
+
+def dymask3() -> np.ndarray :
+    """Defines a mask of size 3 x 3 for discrete approximation of the 
+    first-order derivative in the y-direction.
+    """
+    return np.array([[0, +1/2, 0], \
+                     [0,   0,  0], \
+                     [0, -1/2, 0]])
+
+
+def dxxmask3() -> np.ndarray :
+    """Defines a mask of size 3 x 3 for discrete approximation of the 
+    second-order derivative in the x-direction.
+    """
+    return np.array([[0,  0,  0], \
+                     [1, -2,  1], \
+                     [0,  0,  0]])
+
+
+def dxymask3() -> np.ndarray :
+    """Defines a mask of size 3 x 3 for discrete approximation of the 
+    mixed second-order derivative in the x- and y-directions.
+    """
+    return np.array([[-1/4, 0, +1/4], \
+                     [   0, 0,    0], \
+                     [+1/4, 0, -1/4]])
+
+
+def dyymask3() -> np.ndarray :
+    """Defines a mask of size 3 x 3 for discrete approximation of the 
+    second-order derivative in the y-direction.
+    """
+    return np.array([[0, +1, 0], \
+                     [0, -2, 0], \
+                     [0, +1, 0]])
+
+
+def dphiphiphi_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the third-order directional 
+    derivative in the orientation phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer.
+    """
+    return cos(phi)**3 * dxxxmask5() + \
+           3*cos(phi)**2 * sin(phi) * dxxymask5() + \
+           3*cos(phi) * sin(phi)**2 * dxyymask5() + \
+           sin(phi)**3 * dyyymask5()
+
+
+def dphiphiorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed third-order directional 
+    derivative, corresponding to a second-order directional derivative in the 
+    orientation phi and a first-order directional derivative in the orthogonal 
+    direction.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return - cos(phi)**2 * sin(phi) * dxxxmask5() \
+           + (cos(phi)**3 - 2 * cos(phi) * sin(phi)**2) * dxxymask5() \
+           - (sin(phi)**3 - 2 * cos(phi)**2 * sin(phi)) * dxyymask5() \
+           + cos(phi) * sin(phi)**2 * dyyymask5()
+
+
+def dphiorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed third-order directional 
+    derivative, corresponding to a first-order directional derivative in the 
+    orientation phi and a second-order directional derivative in the orthogonal 
+    direction.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return cos(phi) * sin(phi)**2 * dxxxmask5() \
+           + (sin(phi)**3 - 2 * cos(phi)**2 * sin(phi)) * dxxymask5() \
+           + (cos(phi)**3 - 2 * cos(phi) * sin(phi)**2) * dxyymask5() \
+           + cos(phi)**2 * sin(phi) * dyyymask5()
+
+
+def dorthorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the third-order directional 
+    derivative in the orientation orthogonal to phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return - sin(phi)**3 * dxxxmask5() \
+           + 3*sin(phi)**2 * cos(phi) * dxxymask5() \
+           - 3*sin(phi) * cos(phi)**2 * dxyymask5() \
+           + cos(phi)**3 * dyyymask5()
+
+
+def dphiphiphiphi_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the fourth-order directional 
+    derivative in the orientation phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer.
+    """
+    return cos(phi)**4 * dxxxxmask5() \
+           + 4 * cos(phi)**3 * sin(phi) * dxxxymask5() \
+           + 6 * cos(phi)**2 * sin(phi)**2 * dxxyymask5() \
+           + 4 * cos(phi) * sin(phi)**3 * dxyyymask5() \
+           + sin(phi)**4 * dyyyymask5()
+
+
+def dphiphiphiorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed fourth-order directional 
+    derivative corresponding to a third-order directional derivative in the orientation 
+    phi and a first-order directional derivative in the orthogonal direction.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return - cos(phi)**3 * sin(phi) * dxxxxmask5() \
+           + (cos(phi)**4 - 3 * cos(phi)**2 * sin(phi)**2) * dxxxymask5() \
+           + 3 * (cos(phi)**3 * sin(phi) - cos(phi) * sin(phi)**3) * dxxyymask5() \
+           + (3 * cos(phi)**2 * sin(phi)**2 - sin(phi)**4) * dxyyymask5() \
+           + cos(phi) * sin(phi)**3 * dyyyymask5()
+
+
+def dphiphiorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed fourth-order directional 
+    derivative corresponding to a second-order directional derivative in the 
+    orientation phi and a second-order directional derivative in the orthogonal 
+    direction.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return cos(phi)**2 * sin(phi)**2 * dxxxxmask5() \
+           + 2 * (cos(phi) * sin(phi)**3 - cos(phi)**3 * sin(phi)) * dxxxymask5() \
+           + (cos(phi)**4 - 4 * cos(phi)**2 * sin(phi)**2 + sin(phi)**4) \
+             * dxxyymask5() \
+           + 2 * (cos(phi)**3 * sin(phi) - cos(phi) * sin(phi)**3) * dxyyymask5() \
+           + cos(phi)**2 * sin(phi)**2 * dyyyymask5()
+
+
+def dphiorthorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the mixed fourth-order directional 
+    derivative corresponding to a first-order directional derivative in the orientation 
+    phi and a third-order directional derivative in the orthogonal direction.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return - cos(phi) * sin(phi)**3 * dxxxxmask5() \
+           + (3 * cos(phi)**2 * sin(phi)**2 - sin(phi)**4) * dxxxymask5() \
+           + 3 * (cos(phi) * sin(phi)**3 - cos(phi)**3 * sin(phi)) * dxxyymask5() \
+           + (cos(phi)**4 - 3 * cos(phi)**2 * sin(phi)**2) * dxyyymask5() \
+           + cos(phi)**3 * sin(phi) * dyyyymask5()
+
+
+def dorthorthorthorth_mask(phi : float) -> np.ndarray :
+    """Defines a mask for discrete approximation of the fourth-order directional 
+    derivative in the orientation orthogonal to phi.
+
+    See Equation (5.54) on page 139 in Lindeberg (1993) 
+    "Scale-Space Theory in Computer Vision", Springer,
+    and note that an orthogonal direction to the unit vector 
+    (cos phi, sin phi) is (-sin phi, cos phi).
+    """
+    return sin(phi)**4 * dxxxxmask5() \
+           - 4 * sin(phi)**3 * cos(phi) * dxxxymask5() \
+           + 6 * sin(phi)**2 * cos(phi)**2 * dxxyymask5() \
+           - 4 * sin(phi) * cos(phi)**3 * dxyyymask5() \
+           + cos(phi)**4 * dyyyymask5()
+
+
+def dxmask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    first-order derivative in the x-direction.
+    """
+    return np.array([[0,   0,  0,   0,  0], \
+                     [0,   0,  0,   0,  0], \
+                     [0, -1/2, 0, +1/2, 0], \
+                     [0,   0,  0,   0,  0], \
+                     [0,   0,  0,   0,  0]])
+
+
+def dymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    first-order derivative in the y-direction.
+    """
+    return np.array([[0, 0,   0,  0, 0], \
+                     [0, 0, +1/2, 0, 0], \
+                     [0, 0,   0,  0, 0], \
+                     [0, 0, -1/2, 0, 0], \
+                     [0, 0,   0,  0, 0]])
+
+
+def dxxmask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    second-order derivative in the x-direction.
+    """
+    return np.array([[0, 0,  0,  0, 0], \
+                     [0, 0,  0,  0, 0], \
+                     [0, 1, -2,  1, 0], \
+                     [0, 0,  0,  0, 0], \
+                     [0, 0,  0,  0, 0]])
+
+
+def dxymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    mixed second-order derivative in the x- and y-directions.
+    """
+    return np.array([[0,    0, 0,    0, 0], \
+                     [0, -1/4, 0, +1/4, 0], \
+                     [0,    0, 0,    0, 0], \
+                     [0, +1/4, 0, -1/4, 0], \
+                     [0,    0, 0,    0, 0]])
+
+
+def dyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    second-order derivative in the y-direction.
+    """
+    return np.array([[0, 0,  0, 0, 0], \
+                     [0, 0, +1, 0, 0], \
+                     [0, 0, -2, 0, 0], \
+                     [0, 0, +1, 0, 0], \
+                     [0, 0,  0, 0, 0]])
+
+
+def dxxxmask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the 
+    third-order derivative in the x-direction.
+    """
+    return np.array([[  0,   0, 0,  0,  0 ], \
+                     [  0,   0, 0,  0,  0 ], \
+                     [-1/2, +1, 0, -1, 1/2], \
+                     [  0,   0, 0,  0,  0 ], \
+                     [  0,   0, 0,  0,  0 ]])
+
+
+def dxxymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the mixed 
+    third-order derivative corresponding to a second-order derivative in the 
+    x-direction and a first-order derivative in the y-direction.
+    """
+    return np.array([[0,   0,   0,   0,  0], \
+                     [0, +1/2, -1, +1/2, 0], \
+                     [0,   0,   0,   0,  0], \
+                     [0, -1/2, +1, -1/2, 0], \
+                     [0,   0,   0,   0,  0]])
+
+
+def dxyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the mixed 
+    third-order derivative corresponding to a first-order derivative in the 
+    x-direction and a second-order derivative in the y-direction.
+    """
+    return np.array([[0,   0,  0,   0,  0], \
+                     [0, -1/2, 0, +1/2, 0], \
+                     [0,   +1, 0,   -1, 0], \
+                     [0, -1/2, 0, +1/2, 0], \
+                     [0,   0,  0,   0,  0]])
+
+
+def dyyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the third-order 
+    derivative in the y-direction.
+    """
+    return np.array([[0, 0, +1/2, 0, 0], \
+                     [0, 0,   -1, 0, 0], \
+                     [0, 0,    0, 0, 0], \
+                     [0, 0,   +1, 0, 0], \
+                     [0, 0, -1/2, 0, 0]])
+
+
+def dxxxxmask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the fourth-order 
+    derivative in the x-direction.
+    """
+    return np.array([[0,  0, 0,  0, 0], \
+                     [0,  0, 0,  0, 0], \
+                     [1, -4, 6, -4, 1], \
+                     [0,  0, 0,  0, 0], \
+                     [0,  0, 0,  0, 0]])
+
+
+def dxxxymask5() -> np.ndarray :
+    """Defines a of size 5 x 5 mask for discrete approximation of the mixed 
+    fourth-order derivative corresponding to a third-order derivative in the 
+    x-direction and a first-order derivative in the y-direction.
+    """
+    return np.array([[   0,    0, 0,    0,    0], \
+                     [-1/4, +1/2, 0, -1/2, +1/4], \
+                     [   0,    0, 0,    0,    0], \
+                     [+1/4, -1/2, 0, +1/2, -1/4], \
+                     [   0,    0, 0,    0,    0]])
+
+
+def dxxyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the mixed 
+    fourth-order derivative corresponding to a second-order derivatives in 
+    the x- and y-directions.
+    """
+    return np.array([[0,  0,  0,  0, 0], \
+                     [0, +1, -2, +1, 0], \
+                     [0, -2, +4, -2, 0], \
+                     [0, +1, -2, +1, 0], \
+                     [0,  0,  0,  0, 0]])
+
+
+def dxyyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the mixed 
+    fourth-order derivative corresponding to a first-order derivative in the 
+    x-direction and a third-order derivative in the y-direction.
+    """
+    return np.array([[0, -1/4, 0, +1/4, 0], \
+                     [0, +1/2, 0, -1/2, 0], \
+                     [0,    0, 0,    0, 0], \
+                     [0, -1/2, 0, +1/2, 0], \
+                     [0, +1/4, 0, -1/4, 0]])
+
+
+def dyyyymask5() -> np.ndarray :
+    """Defines a mask of size 5 x 5 for discrete approximation of the fourth-order 
+    derivative in the y-direction.
+    """
+    return np.array([[0, 0, +1, 0, 0], \
+                     [0, 0, -4, 0, 0], \
+                     [0, 0, +6, 0, 0], \
+                     [0, 0, -4, 0, 0], \
+                     [0, 0, +1, 0, 0]])
+
+
+def make1Dgaussfilter(
+        sigma : float,
+        scspmethod : str = 'discgauss',
+        epsilon : float = 0.00000001
+    ) -> np.array :
+    """Computes a discrete approximation of a Gaussian filter at scale sigma for
+    different types of discrete approximations, given an upper bound epsilon
+    on the truncation error at the tails.
+
+    The following discrete approximation methods have been implemented:
+
+      'discgauss' - the discrete analogue of the Gaussian kernel
+      'samplgauss' - the sampled Gaussian kernel
+      'normsamplgauss' - the normalized sampled Gaussian kernel
+      'intgauss' - the integrated Gaussian kernel
+      'linintgauss' - the linearily interpolated and integrated Gaussian kernel
+
+    The discrete analogue of the Gaussian kernel has the best theoretical properties 
+    of these kernels, in the sense that it obeys both (i) non-enhancement of local 
+    extrema over a 2-D spatial domain and (ii) non-creation of local extrema from 
+    any finer to any coarser level of scale for any 1-D signal. The filter coefficents 
+    are (iii) guaranteed to be in the interval [0, 1] and do (iv) exactly sum to one 
+    for an infinitely sized filter. (v) The spatial standard deviation of the discrete 
+    kernel is also equal to the sigma value.
+
+    The different methods have the possible advantages (+) and disadvantages (-):
+
+    'discgauss' + guarantees non-enhancement of local extrema over a 2-D image domain
+                + guarantees non-creation of new extrema from any finer to any
+                  coarser level of scale over a 1-D signal domain
+                + the kernel values are guaranteed to be in the interval [0, 1]
+                + the kernel values are guaranteed to sum to 1 over an infinite domain
+                + no scale offset at all in the spatial discretization
+
+    'samplgauss' + no added scale offset in the spatial discretization
+                 + for sufficiently large scale values a good approximation of
+                   the underlying continuous model
+                 - the kernel values may become greater than 1 for small values of sigma
+                 - the kernel values do not sum up to one
+                 - for very small values of sigma, the kernels have a too narrow shape
+
+    'normsamplgauss' + no added scale offset in the spatial discretization
+                     + formally the kernel values are guaranteed to be in the 
+                       interval [0, 1]
+                     + formally the kernel values are guaranteed to sum up to 1 
+                     - the complementary normalization of the kernel is ad hoc
+                     - for very small values of sigma, the kernels have a too narrow 
+                       shape
+
+    'intgauss' + the kernel values are guaranteed to be in the interval [0, 1]
+               + the kernel values are guaranteed to sum up to 1 over an infinite domain
+               - the box integration introduces a scale offset of 1/12 at coarser scales
+
+    'linintgauss' + the kernel values are guaranteed to be in the interval [0, 1]
+                  - the triangular window integration introduces a scale offset of 1/6
+                    at coarser scales
+
+    Besides being a string, the argument scspmethod may also be an object
+    having the attributes scspmethod.methodname and scspmethod.epsilon.
+
+    The parameter epsilon specifies an upper bound on the relative truncation error
+    for separable filtering over a D-dimensional domain.
+    """
+    if isinstance(scspmethod, str):
+        scspmethodname = scspmethod
+    else:
+        scspmethodname = scspmethod.methodname
+        epsilon = scspmethod.epsilon
+
+    if scspmethodname == 'discgauss':
+        return make1Ddiscgaussfilter(sigma, epsilon)
+
+    if scspmethodname == 'samplgauss':
+        return make1Dsamplgaussfilter(sigma, epsilon)
+
+    if scspmethodname == 'normsamplgauss':
+        return make1Dnormsamplgaussfilter(sigma, epsilon)
+
+    if scspmethodname == 'intgauss':
+        return make1Dintgaussfilter(sigma, epsilon)
+
+    if scspmethodname == 'linintgauss':
+        return make1Dlinintgaussfilter(sigma, epsilon)
+
+    raise ValueError(f"Gaussian smoothing discretization method \
+{scspmethodname} not implemented")
+
+
+def make1Ddiscgaussderfilter(
+        order : int,
+        sigma : float,
+        N : int
+        ) -> np.ndarray :
+    """Generates a discrete derivative approximation kernel corresponding to the
+    equivalent effect of performing smoothing with the discrete analogue of the
+    Gaussian kernel with standard deviation sigma followed by central differences 
+    to estimate derivative approximations. The filter is truncated at the ends 
+    at -N and -N.
+
+    Note: This kernel is not intended for actual computations of discrete derivative
+    approximations. It is solely intended for analysis of the equivalent effect of
+    smoothing and for graphical visualization.
+    """
+    x = np.linspace(-N, N, 1 + 2*N)
+    T = ive(x, sigma**2)
+
+    if order == 0:
+        return T
+
+    if order == 1:
+        dx = np.array([-1/2, 0, 1/2])
+        return correlate1d(T, dx)
+
+    if order == 2:
+        dxx = np.array([1, -2, 1])
+        return correlate1d(T, dxx)
+
+    if order == 3:
+        dxxx = np.array([-1/2, +1, 0, -1, 1/2])
+        return correlate1d(T, dxxx)
+
+    if order == 4:
+        dxxxx = np.array([1, -4, 6, -4, 1])
+        return correlate1d(T, dxxxx)
+
+    raise ValueError(f"Not implemented for order {order}")
+
+
+def make1Dsamplgaussdifffilter(
+        order : int,
+        sigma : float,
+        N : int
+        ) -> np.ndarray :
+    """Generates a discrete derivative approximation kernel corresponding to the
+    equivalent effect of performing discrete smoothing with the sampled Gaussian 
+    kernel followed by central differences to estimate derivative approximations. 
+
+    Note: This kernel is not intended for actual computations of discrete derivative
+    approximations. It is solely intended for analysis of the equivalent effect of
+    smoothing and for graphical visualization.
+    """
+    x = np.linspace(-N, N, 1 + 2*N)
+    T = gauss(x, sigma)
+
+    if order == 0:
+        return T
+
+    if order == 1:
+        dx = np.array([-1/2, 0, 1/2])
+        return correlate1d(T, dx)
+
+    if order == 2:
+        dxx = np.array([1, -2, 1])
+        return correlate1d(T, dxx)
+
+    if order == 3:
+        dxxx = np.array([-1/2, +1, 0, -1, 1/2])
+        return correlate1d(T, dxxx)
+
+    if order == 4:
+        dxxxx = np.array([1, -4, 6, -4, 1])
+        return correlate1d(T, dxxxx)
+
+    raise ValueError(f"Not implemented for order {order}")
+
+
+def make1Dnormsamplgaussdifffilter(
+        order : int,
+        sigma : float,
+        N : int
+        ) -> np.ndarray :
+    """Generates a discrete derivative approximation kernel corresponding to the
+    equivalent effect of performing discrete smoothing with the normalized 
+    sampled Gaussian kernel followed by central differences to estimate derivative approximations. 
+
+    Note: This kernel is not intended for actual computations of discrete derivative
+    approximations. It is solely intended for analysis of the equivalent effect of
+    smoothing and for graphical visualization.
+    """
+    x = np.linspace(-N, N, 1 + 2*N)
+    T = gauss(x, sigma)
+    T = T/np.sum(T)
+    
+    if order == 0:
+        return T
+
+    if order == 1:
+        dx = np.array([-1/2, 0, 1/2])
+        return correlate1d(T, dx)
+
+    if order == 2:
+        dxx = np.array([1, -2, 1])
+        return correlate1d(T, dxx)
+
+    if order == 3:
+        dxxx = np.array([-1/2, +1, 0, -1, 1/2])
+        return correlate1d(T, dxxx)
+
+    if order == 4:
+        dxxxx = np.array([1, -4, 6, -4, 1])
+        return correlate1d(T, dxxxx)
+
+    raise ValueError(f"Not implemented for order {order}")
+
+
+def make1Dintgaussdifffilter(
+        order : int,
+        sigma : float,
+        N : int
+        ) -> np.ndarray :
+    """Generates a discrete derivative approximation kernel corresponding to the
+    equivalent effect of performing discrete smoothing with the integrated Gaussian 
+    kernel followed by central differences to estimate derivative approximations. 
+
+    Note: This kernel is not intended for actual computations of discrete derivative
+    approximations. It is solely intended for analysis of the equivalent effect of
+    smoothing and for graphical visualization.
+    """
+    x = np.linspace(-N, N, 1 + 2*N)
+    T = scaled_erf(x + 0.5, sigma) - scaled_erf(x - 0.5, sigma)
+
+    if order == 0:
+        return T
+
+    if order == 1:
+        dx = np.array([-1/2, 0, 1/2])
+        return correlate1d(T, dx)
+
+    if order == 2:
+        dxx = np.array([1, -2, 1])
+        return correlate1d(T, dxx)
+
+    if order == 3:
+        dxxx = np.array([-1/2, +1, 0, -1, 1/2])
+        return correlate1d(T, dxxx)
+
+    if order == 4:
+        dxxxx = np.array([1, -4, 6, -4, 1])
+        return correlate1d(T, dxxxx)
+
+    raise ValueError(f"Not implemented for order {order}")
```

