# Comparing `tmp/ANNarchy-4.7.2.6.tar.gz` & `tmp/ANNarchy-4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANNarchy-4.7.2.6.tar", last modified: Thu Aug 17 14:03:17 2023, max compression
+gzip compressed data, was "ANNarchy-4.7.3.tar", last modified: Thu Mar 21 20:45:45 2024, max compression
```

## Comparing `ANNarchy-4.7.2.6.tar` & `ANNarchy-4.7.3.tar`

### file list

```diff
@@ -1,273 +1,275 @@
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.940035 ANNarchy-4.7.2.6/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.897619 ANNarchy-4.7.2.6/ANNarchy/
--rw-r--r--   0 vitay      (501) staff       (20)     1989 2023-08-17 14:03:15.000000 ANNarchy-4.7.2.6/ANNarchy/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.902415 ANNarchy-4.7.2.6/ANNarchy/core/
--rw-r--r--   0 vitay      (501) staff       (20)    28001 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.6/ANNarchy/core/ConnectorMethods.py
--rw-r--r--   0 vitay      (501) staff       (20)    13851 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/core/Dendrite.py
--rw-r--r--   0 vitay      (501) staff       (20)    28338 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/core/Global.py
--rw-r--r--   0 vitay      (501) staff       (20)    20797 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.6/ANNarchy/core/IO.py
--rw-r--r--   0 vitay      (501) staff       (20)    35087 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/core/Monitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    34546 2023-08-17 13:55:58.000000 ANNarchy-4.7.2.6/ANNarchy/core/Network.py
--rw-r--r--   0 vitay      (501) staff       (20)     7309 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/core/NetworkManager.py
--rw-r--r--   0 vitay      (501) staff       (20)     8453 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/core/Neuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    32673 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.6/ANNarchy/core/Population.py
--rw-r--r--   0 vitay      (501) staff       (20)    12829 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/core/PopulationView.py
--rw-r--r--   0 vitay      (501) staff       (20)     6876 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/core/Profiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    65431 2023-08-07 11:45:48.000000 ANNarchy-4.7.2.6/ANNarchy/core/Projection.py
--rw-r--r--   0 vitay      (501) staff       (20)     8383 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.6/ANNarchy/core/Random.py
--rw-r--r--   0 vitay      (501) staff       (20)    10098 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/core/Simulate.py
--rw-r--r--   0 vitay      (501) staff       (20)    95368 2023-06-23 04:21:47.000000 ANNarchy-4.7.2.6/ANNarchy/core/SpecificPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)    15140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/core/SpecificProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     5803 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/ANNarchy/core/Synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     3463 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/core/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/ANNarchy/core/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.903180 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/
--rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Connector.pxd
--rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Connector.pyx
--rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Coordinates.pxd
--rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Coordinates.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Transformations.pyx
--rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/__init__.pxd
--rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.903272 ANNarchy-4.7.2.6/ANNarchy/extensions/
--rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.903769 ANNarchy-4.7.2.6/ANNarchy/extensions/ann_to_snn_conversion/
--rw-r--r--   0 vitay      (501) staff       (20)     9131 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
--rw-r--r--   0 vitay      (501) staff       (20)     3621 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
--rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.905069 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/
--rw-r--r--   0 vitay      (501) staff       (20)    12839 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/AccProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)     2928 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/BoldModel.py
--rw-r--r--   0 vitay      (501) staff       (20)    10439 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/BoldMonitor.py
--rw-r--r--   0 vitay      (501) staff       (20)    15160 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/NormProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)    27888 2022-01-06 14:46:24.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/PredefinedModels.py
--rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/bold/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.906748 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/
--rw-r--r--   0 vitay      (501) staff       (20)    42897 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Convolve.py
--rw-r--r--   0 vitay      (501) staff       (20)     3005 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/ConvolveTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     9368 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Copy.py
--rw-r--r--   0 vitay      (501) staff       (20)     4502 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/CopyTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    24982 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Pooling.py
--rw-r--r--   0 vitay      (501) staff       (20)    14070 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/PoolingTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14093 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Transpose.py
--rw-r--r--   0 vitay      (501) staff       (20)     1583 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.907004 ANNarchy-4.7.2.6/ANNarchy/extensions/diagonal/
--rw-r--r--   0 vitay      (501) staff       (20)    16351 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/diagonal/DiagonalProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/diagonal/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.907393 ANNarchy-4.7.2.6/ANNarchy/extensions/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)    20781 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/hybrid/HybridPopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/hybrid/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.907700 ANNarchy-4.7.2.6/ANNarchy/extensions/image/
--rw-r--r--   0 vitay      (501) staff       (20)     9944 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/image/ImagePopulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/image/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.908000 ANNarchy-4.7.2.6/ANNarchy/extensions/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)    12742 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/tensorboard/Logger.py
--rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/tensorboard/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.908468 ANNarchy-4.7.2.6/ANNarchy/extensions/weightsharing/
--rw-r--r--   0 vitay      (501) staff       (20)    51829 2023-06-23 04:19:41.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/weightsharing/SharedProjection.py
--rw-r--r--   0 vitay      (501) staff       (20)      206 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.6/ANNarchy/extensions/weightsharing/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.910139 ANNarchy-4.7.2.6/ANNarchy/generator/
--rw-r--r--   0 vitay      (501) staff       (20)    42289 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/CodeGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    38174 2023-08-08 09:22:28.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Compiler.py
--rw-r--r--   0 vitay      (501) staff       (20)    10654 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/MonitorGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.911688 ANNarchy-4.7.2.6/ANNarchy/generator/Population/
--rw-r--r--   0 vitay      (501) staff       (20)    59484 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/CUDAGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    26498 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/CUDATemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    41946 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    14427 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/OpenMPTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    20938 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/PopulationGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    37140 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    13356 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/SingleThreadTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Population/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.912731 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/
--rw-r--r--   0 vitay      (501) staff       (20)    14883 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/CPP11Profile.py
--rw-r--r--   0 vitay      (501) staff       (20)     8646 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/CUDAProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     6963 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/PAPIProfile.py
--rw-r--r--   0 vitay      (501) staff       (20)     3947 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/ProfileGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    31714 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/ProfileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Profile/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.914088 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.916392 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/
--rw-r--r--   0 vitay      (501) staff       (20)    14633 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11089 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)    11052 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    36964 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13010 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
--rw-r--r--   0 vitay      (501) staff       (20)    12651 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
--rw-r--r--   0 vitay      (501) staff       (20)    19628 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)    11220 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    15997 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    15664 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8341 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    10511 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    72468 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDAGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.918414 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/
--rw-r--r--   0 vitay      (501) staff       (20)     8715 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    13744 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3654 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37572 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     8436 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     8172 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     6031 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
--rw-r--r--   0 vitay      (501) staff       (20)    19185 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4756 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     5111 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)    51527 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)    22149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/LIL_P.py
--rw-r--r--   0 vitay      (501) staff       (20)     4136 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    60579 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMPGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    49846 2023-08-01 15:26:06.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/ProjectionGenerator.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.920895 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/
--rw-r--r--   0 vitay      (501) staff       (20)     8717 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/BSR.py
--rw-r--r--   0 vitay      (501) staff       (20)    11194 2023-08-08 09:22:41.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
--rw-r--r--   0 vitay      (501) staff       (20)     3413 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/COO.py
--rw-r--r--   0 vitay      (501) staff       (20)    37503 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/CSR.py
--rw-r--r--   0 vitay      (501) staff       (20)     7292 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/CSR_T.py
--rw-r--r--   0 vitay      (501) staff       (20)    17125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense.py
--rw-r--r--   0 vitay      (501) staff       (20)     4489 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
--rw-r--r--   0 vitay      (501) staff       (20)     4792 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     4570 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_T.py
--rw-r--r--   0 vitay      (501) staff       (20)     8588 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/ELL.py
--rw-r--r--   0 vitay      (501) staff       (20)    14808 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/ELLR.py
--rw-r--r--   0 vitay      (501) staff       (20)     4607 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/HYB.py
--rw-r--r--   0 vitay      (501) staff       (20)    45456 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/LIL.py
--rw-r--r--   0 vitay      (501) staff       (20)     4120 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/SELL.py
--rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    57963 2023-05-24 11:13:17.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThreadGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Projection/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    54049 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/PyxGenerator.py
--rw-r--r--   0 vitay      (501) staff       (20)    15018 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Sanity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.923519 ANNarchy-4.7.2.6/ANNarchy/generator/Template/
--rw-r--r--   0 vitay      (501) staff       (20)    29830 2023-08-07 13:55:17.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/BaseTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    16113 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/GlobalOperationTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     2426 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/MakefileTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    19390 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/MonitorTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)    14699 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/PyxTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Template/__init__.py
--rw-r--r--   0 vitay      (501) staff       (20)    15650 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/generator/Utils.py
--rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.2.6/ANNarchy/generator/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.927559 ANNarchy-4.7.2.6/ANNarchy/include/
--rw-r--r--   0 vitay      (501) staff       (20)    26125 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/BSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     6674 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/BSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    17338 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.6/ANNarchy/include/COOMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8165 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/COOMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9119 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8274 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     7660 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixCUDAT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    22237 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixT.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    21843 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8971 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/CSRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30517 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     8778 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrixOffsets.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    32735 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/ELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9264 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/ELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    30967 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/ELLRMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    10305 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/ELLRMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/HYBMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/HYBMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9991 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.6/ANNarchy/include/LILInvMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    37614 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/LILMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    23769 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/PartitionedMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)    25554 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/include/SELLMatrix.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     9628 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/ANNarchy/include/SELLMatrixCUDA.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.6/ANNarchy/include/Specific.hpp
--rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.6/ANNarchy/include/helper_functions.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.928072 ANNarchy-4.7.2.6/ANNarchy/models/
--rw-r--r--   0 vitay      (501) staff       (20)    45126 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.6/ANNarchy/models/Neurons.py
--rw-r--r--   0 vitay      (501) staff       (20)    11837 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.6/ANNarchy/models/Synapses.py
--rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/ANNarchy/models/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.930413 ANNarchy-4.7.2.6/ANNarchy/parser/
--rw-r--r--   0 vitay      (501) staff       (20)    15017 2023-05-24 12:05:12.000000 ANNarchy-4.7.2.6/ANNarchy/parser/AnalyseNeuron.py
--rw-r--r--   0 vitay      (501) staff       (20)    21586 2023-05-24 12:08:11.000000 ANNarchy-4.7.2.6/ANNarchy/parser/AnalyseSynapse.py
--rw-r--r--   0 vitay      (501) staff       (20)    14166 2023-05-24 12:05:32.000000 ANNarchy-4.7.2.6/ANNarchy/parser/CoupledEquations.py
--rw-r--r--   0 vitay      (501) staff       (20)    28868 2023-05-24 12:05:45.000000 ANNarchy-4.7.2.6/ANNarchy/parser/Equation.py
--rw-r--r--   0 vitay      (501) staff       (20)    28842 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/parser/Extraction.py
--rw-r--r--   0 vitay      (501) staff       (20)     4336 2022-12-05 16:13:02.000000 ANNarchy-4.7.2.6/ANNarchy/parser/Function.py
--rw-r--r--   0 vitay      (501) staff       (20)     6049 2022-12-05 16:13:18.000000 ANNarchy-4.7.2.6/ANNarchy/parser/ITE.py
--rw-r--r--   0 vitay      (501) staff       (20)     3032 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/ANNarchy/parser/ParserTemplate.py
--rw-r--r--   0 vitay      (501) staff       (20)     7633 2022-12-05 16:13:32.000000 ANNarchy-4.7.2.6/ANNarchy/parser/StringManipulation.py
--rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/ANNarchy/parser/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.931650 ANNarchy-4.7.2.6/ANNarchy/parser/report/
--rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.2.6/ANNarchy/parser/report/LatexParser.py
--rw-r--r--   0 vitay      (501) staff       (20)    22678 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/ANNarchy/parser/report/LatexReport.py
--rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.2.6/ANNarchy/parser/report/MarkdownReport.py
--rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.6/ANNarchy/parser/report/Report.py
--rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/ANNarchy/parser/report/__init__.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.931748 ANNarchy-4.7.2.6/ANNarchy/thirdparty/
--rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/ANNarchy/thirdparty/randutils.hpp
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.898372 ANNarchy-4.7.2.6/ANNarchy.egg-info/
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-08-17 14:03:17.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     8626 2023-08-17 14:03:17.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/SOURCES.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2023-08-17 14:03:17.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/dependency_links.txt
--rw-r--r--   0 vitay      (501) staff       (20)        1 2021-04-13 07:32:27.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/not-zip-safe
--rw-r--r--   0 vitay      (501) staff       (20)       36 2023-08-17 14:03:17.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/requires.txt
--rw-r--r--   0 vitay      (501) staff       (20)        9 2023-08-17 14:03:17.000000 ANNarchy-4.7.2.6/ANNarchy.egg-info/top_level.txt
--rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.2.6/LICENSE
--rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.2.6/MANIFEST.in
--rw-r--r--   0 vitay      (501) staff       (20)     1429 2023-08-17 14:03:17.940096 ANNarchy-4.7.2.6/PKG-INFO
--rw-r--r--   0 vitay      (501) staff       (20)     1803 2023-08-17 08:10:31.000000 ANNarchy-4.7.2.6/README.md
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.896227 ANNarchy-4.7.2.6/examples/
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.932106 ANNarchy-4.7.2.6/examples/ann_to_snn/
--rw-r--r--   0 vitay      (501) staff       (20)      991 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/examples/ann_to_snn/demo.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.932648 ANNarchy-4.7.2.6/examples/bar_learning/
--rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/examples/bar_learning/BarLearning.py
--rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/examples/bar_learning/BarLearningGPU.py
--rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.6/examples/bar_learning/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.933115 ANNarchy-4.7.2.6/examples/bold_monitor/
--rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.6/examples/bold_monitor/BOLD.py
--rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.2.6/examples/bold_monitor/BOLD_two_inputs.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.933297 ANNarchy-4.7.2.6/examples/gap_junctions/
--rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/examples/gap_junctions/GapJunctions.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.933557 ANNarchy-4.7.2.6/examples/hodgkin_huxley/
--rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-04-12 11:51:52.000000 ANNarchy-4.7.2.6/examples/hodgkin_huxley/HodgkinHuxley.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.934026 ANNarchy-4.7.2.6/examples/homeostatic_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     5062 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/homeostatic_stdp/Ramp.py
--rw-r--r--   0 vitay      (501) staff       (20)     7059 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/homeostatic_stdp/SORF.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.934211 ANNarchy-4.7.2.6/examples/hybrid/
--rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/hybrid/Hybrid.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.934830 ANNarchy-4.7.2.6/examples/image/
--rw-r--r--   0 vitay      (501) staff       (20)     6193 2023-05-24 11:13:07.000000 ANNarchy-4.7.2.6/examples/image/Image.py
--rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/examples/image/Webcam.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/examples/image/Webcam.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.935046 ANNarchy-4.7.2.6/examples/izhikevich/
--rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.6/examples/izhikevich/Izhikevich.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.935233 ANNarchy-4.7.2.6/examples/multinetwork/
--rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.2.6/examples/multinetwork/MultiNetwork.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.935933 ANNarchy-4.7.2.6/examples/neural_field/
--rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.2.6/examples/neural_field/BubbleWorld.pyx
--rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.2.6/examples/neural_field/NeuralField.py
--rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.2.6/examples/neural_field/Viz.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.937019 ANNarchy-4.7.2.6/examples/pyNN/
--rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/AEIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/EIF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/IF_cond_exp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/IF_curr_alpha.py
--rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/non_linear_synapse.py
--rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/pyNN/short_term_plasticity2.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.937161 ANNarchy-4.7.2.6/examples/refractoriness/
--rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/refractoriness/Refractoriness.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.937297 ANNarchy-4.7.2.6/examples/simple_stdp/
--rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/examples/simple_stdp/SimpleSTDPModel.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.937439 ANNarchy-4.7.2.6/examples/structural_plasticity/
--rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/examples/structural_plasticity/StructuralPlasticity.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.938385 ANNarchy-4.7.2.6/examples/tensorboard/
--rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.2.6/examples/tensorboard/BasalGanglia.ipynb
--rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.2.6/examples/tensorboard/BayesianOptimization.ipynb
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.938719 ANNarchy-4.7.2.6/examples/tsodyks_markram/
--rw-r--r--   0 vitay      (501) staff       (20)     3872 2023-04-12 10:39:20.000000 ANNarchy-4.7.2.6/examples/tsodyks_markram/TsodyksMarkram.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.939192 ANNarchy-4.7.2.6/examples/vogels_abbott/
--rw-r--r--   0 vitay      (501) staff       (20)     1940 2020-09-29 13:24:31.000000 ANNarchy-4.7.2.6/examples/vogels_abbott/COBA.py
--rw-r--r--   0 vitay      (501) staff       (20)     1809 2019-07-10 20:15:51.000000 ANNarchy-4.7.2.6/examples/vogels_abbott/CUBA.py
--rw-r--r--   0 vitay      (501) staff       (20)       99 2023-08-04 16:48:38.000000 ANNarchy-4.7.2.6/requirements.txt
--rw-r--r--   0 vitay      (501) staff       (20)      101 2023-08-17 14:03:17.940287 ANNarchy-4.7.2.6/setup.cfg
--rw-r--r--   0 vitay      (501) staff       (20)    10774 2023-08-17 14:03:07.000000 ANNarchy-4.7.2.6/setup.py
-drwxr-xr-x   0 vitay      (501) staff       (20)        0 2023-08-17 14:03:17.939770 ANNarchy-4.7.2.6/tests/
--rw-r--r--   0 vitay      (501) staff       (20)     1122 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/tests/test_CUDA.py
--rw-r--r--   0 vitay      (501) staff       (20)     1062 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/tests/test_openmp.py
--rw-r--r--   0 vitay      (501) staff       (20)     1149 2022-12-14 10:27:19.000000 ANNarchy-4.7.2.6/tests/test_single_thread.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.816075 ANNarchy-4.7.3/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.779308 ANNarchy-4.7.3/ANNarchy/
+-rw-r--r--   0 vitay      (501) staff       (20)     2110 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.783032 ANNarchy-4.7.3/ANNarchy/core/
+-rw-r--r--   0 vitay      (501) staff       (20)    27239 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/ConnectorMethods.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15318 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Dendrite.py
+-rw-r--r--   0 vitay      (501) staff       (20)    29064 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Global.py
+-rw-r--r--   0 vitay      (501) staff       (20)    19962 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/IO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    37599 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Monitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    33705 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Network.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7023 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/NetworkManager.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7515 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Neuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    32486 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Population.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11893 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/PopulationView.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6525 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Profiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)    65839 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Projection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8324 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Random.py
+-rw-r--r--   0 vitay      (501) staff       (20)     9223 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Simulate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    98277 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/SpecificPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14568 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/SpecificProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4871 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3789 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/core/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/ANNarchy/core/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.783840 ANNarchy-4.7.3/ANNarchy/core/cython_ext/
+-rw-r--r--   0 vitay      (501) staff       (20)     1683 2022-05-18 09:30:59.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/Connector.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)    21582 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/Connector.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)      924 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/Coordinates.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)     4941 2022-01-07 10:51:43.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/Coordinates.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     2866 2022-02-02 12:38:23.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/Transformations.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2020-05-31 10:28:52.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/__init__.pxd
+-rw-r--r--   0 vitay      (501) staff       (20)      405 2020-03-10 16:42:34.000000 ANNarchy-4.7.3/ANNarchy/core/cython_ext/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.783956 ANNarchy-4.7.3/ANNarchy/extensions/
+-rw-r--r--   0 vitay      (501) staff       (20)       21 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/extensions/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.784409 ANNarchy-4.7.3/ANNarchy/extensions/ann_to_snn_conversion/
+-rw-r--r--   0 vitay      (501) staff       (20)    23580 2024-03-21 20:38:39.000000 ANNarchy-4.7.3/ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2736 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1719 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py
+-rw-r--r--   0 vitay      (501) staff       (20)       48 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/extensions/ann_to_snn_conversion/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.785326 ANNarchy-4.7.3/ANNarchy/extensions/bold/
+-rw-r--r--   0 vitay      (501) staff       (20)    12317 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/AccProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2012 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/BoldModel.py
+-rw-r--r--   0 vitay      (501) staff       (20)     9517 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/BoldMonitor.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14234 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/NormProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)    26965 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/PredefinedModels.py
+-rw-r--r--   0 vitay      (501) staff       (20)      386 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/ANNarchy/extensions/bold/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.786719 ANNarchy-4.7.3/ANNarchy/extensions/convolution/
+-rw-r--r--   0 vitay      (501) staff       (20)    52492 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/Convolve.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15470 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/ConvolveTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     8523 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/Copy.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3574 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/CopyTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    24843 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/Pooling.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14205 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/PoolingTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13197 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/Transpose.py
+-rw-r--r--   0 vitay      (501) staff       (20)      667 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)      858 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/ANNarchy/extensions/convolution/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.787046 ANNarchy-4.7.3/ANNarchy/extensions/diagonal/
+-rw-r--r--   0 vitay      (501) staff       (20)    15604 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/diagonal/DiagonalProjection.py
+-rw-r--r--   0 vitay      (501) staff       (20)       50 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/extensions/diagonal/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.787316 ANNarchy-4.7.3/ANNarchy/extensions/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)    20879 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/hybrid/HybridPopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       72 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/extensions/hybrid/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.787594 ANNarchy-4.7.3/ANNarchy/extensions/image/
+-rw-r--r--   0 vitay      (501) staff       (20)    10042 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/image/ImagePopulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       62 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/extensions/image/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.787859 ANNarchy-4.7.3/ANNarchy/extensions/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)    11806 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/extensions/tensorboard/Logger.py
+-rw-r--r--   0 vitay      (501) staff       (20)       26 2020-05-31 10:28:52.000000 ANNarchy-4.7.3/ANNarchy/extensions/tensorboard/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.789221 ANNarchy-4.7.3/ANNarchy/generator/
+-rw-r--r--   0 vitay      (501) staff       (20)     4246 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/CmdLineArgParser.py
+-rw-r--r--   0 vitay      (501) staff       (20)    42263 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/CodeGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    35038 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Compiler.py
+-rw-r--r--   0 vitay      (501) staff       (20)     9739 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/MonitorGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.790515 ANNarchy-4.7.3/ANNarchy/generator/Population/
+-rw-r--r--   0 vitay      (501) staff       (20)    61986 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/CUDAGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    26957 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/CUDATemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    41084 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13693 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/OpenMPTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22078 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/PopulationGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    35611 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12637 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/SingleThreadTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)      142 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/ANNarchy/generator/Population/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.791424 ANNarchy-4.7.3/ANNarchy/generator/Profile/
+-rw-r--r--   0 vitay      (501) staff       (20)    13953 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/CPP11Profile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7717 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/CUDAProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6034 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/PAPIProfile.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3013 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/ProfileGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    30855 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/ProfileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)      159 2020-03-10 16:42:34.000000 ANNarchy-4.7.3/ANNarchy/generator/Profile/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.792153 ANNarchy-4.7.3/ANNarchy/generator/Projection/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.794459 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/
+-rw-r--r--   0 vitay      (501) staff       (20)    14586 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10177 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10168 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    39116 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12622 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py
+-rw-r--r--   0 vitay      (501) staff       (20)    12463 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14801 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py
+-rw-r--r--   0 vitay      (501) staff       (20)    23959 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10907 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15625 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    16792 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7469 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10200 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1514 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    77558 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDAGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.796798 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/
+-rw-r--r--   0 vitay      (501) staff       (20)     7967 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11951 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2783 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    36651 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7563 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7248 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5992 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)    18305 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3879 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7888 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     4239 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    50636 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22029 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3989 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1565 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    62306 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMPGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    51285 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/ProjectionGenerator.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.799055 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/
+-rw-r--r--   0 vitay      (501) staff       (20)    18307 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/BSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)    11646 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2542 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/COO.py
+-rw-r--r--   0 vitay      (501) staff       (20)    36733 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/CSR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6419 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)    16946 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3571 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3848 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5288 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7717 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/ELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)    16164 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/ELLR.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3736 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/HYB.py
+-rw-r--r--   0 vitay      (501) staff       (20)    44535 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/LIL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3973 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/SELL.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1671 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    58653 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThreadGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)      233 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/ANNarchy/generator/Projection/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    53905 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/PyxGenerator.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13943 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Sanity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.800018 ANNarchy-4.7.3/ANNarchy/generator/Template/
+-rw-r--r--   0 vitay      (501) staff       (20)    33691 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/BaseTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    17690 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/GlobalOperationTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2525 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/MakefileTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22008 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/MonitorTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)    14191 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/PyxTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/generator/Template/__init__.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15004 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/generator/Utils.py
+-rw-r--r--   0 vitay      (501) staff       (20)       30 2017-07-25 21:21:04.000000 ANNarchy-4.7.3/ANNarchy/generator/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.805531 ANNarchy-4.7.3/ANNarchy/include/
+-rw-r--r--   0 vitay      (501) staff       (20)     8527 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/BSRInvMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    27288 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/BSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     7084 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/BSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    17465 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/COOMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8563 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/COOMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10989 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRCMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8926 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRCMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8600 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRCMatrixCUDAT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    22747 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRCMatrixT.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    22670 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9302 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/CSRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    30581 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/DenseMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     8879 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/DenseMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10925 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/include/DenseMatrixOffsets.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    32799 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/ELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9493 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/ELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    31031 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/ELLRMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10629 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/ELLRMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    19241 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/include/HYBMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     5284 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/include/HYBMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    10267 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/LILInvMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    39297 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/LILMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    24689 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/PartitionedMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)    25701 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/SELLMatrix.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     9540 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/SELLMatrixCUDA.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1092 2022-02-02 12:32:46.000000 ANNarchy-4.7.3/ANNarchy/include/Specific.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     4143 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/include/VecTransformation.hpp
+-rw-r--r--   0 vitay      (501) staff       (20)     1430 2022-02-02 12:32:46.000000 ANNarchy-4.7.3/ANNarchy/include/helper_functions.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.806151 ANNarchy-4.7.3/ANNarchy/models/
+-rw-r--r--   0 vitay      (501) staff       (20)    44201 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/models/Neurons.py
+-rw-r--r--   0 vitay      (501) staff       (20)    10911 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/models/Synapses.py
+-rw-r--r--   0 vitay      (501) staff       (20)      352 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/ANNarchy/models/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.807695 ANNarchy-4.7.3/ANNarchy/parser/
+-rw-r--r--   0 vitay      (501) staff       (20)    14086 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/AnalyseNeuron.py
+-rw-r--r--   0 vitay      (501) staff       (20)    20654 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/AnalyseSynapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)    13232 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/CoupledEquations.py
+-rw-r--r--   0 vitay      (501) staff       (20)    28430 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/Equation.py
+-rw-r--r--   0 vitay      (501) staff       (20)    27914 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/Extraction.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3599 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/Function.py
+-rw-r--r--   0 vitay      (501) staff       (20)     5317 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/ITE.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3130 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/ParserTemplate.py
+-rw-r--r--   0 vitay      (501) staff       (20)     6886 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/ANNarchy/parser/StringManipulation.py
+-rw-r--r--   0 vitay      (501) staff       (20)       86 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/ANNarchy/parser/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.808472 ANNarchy-4.7.3/ANNarchy/parser/report/
+-rw-r--r--   0 vitay      (501) staff       (20)    16861 2023-01-25 15:17:04.000000 ANNarchy-4.7.3/ANNarchy/parser/report/LatexParser.py
+-rw-r--r--   0 vitay      (501) staff       (20)    22711 2024-02-08 08:00:55.000000 ANNarchy-4.7.3/ANNarchy/parser/report/LatexReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)    15846 2021-04-01 06:34:12.000000 ANNarchy-4.7.3/ANNarchy/parser/report/MarkdownReport.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1985 2021-06-05 08:46:21.000000 ANNarchy-4.7.3/ANNarchy/parser/report/Report.py
+-rw-r--r--   0 vitay      (501) staff       (20)        0 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/ANNarchy/parser/report/__init__.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.808567 ANNarchy-4.7.3/ANNarchy/thirdparty/
+-rw-r--r--   0 vitay      (501) staff       (20)    26759 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/ANNarchy/thirdparty/randutils.hpp
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.779940 ANNarchy-4.7.3/ANNarchy.egg-info/
+-rw-r--r--   0 vitay      (501) staff       (20)     2996 2024-03-21 20:45:45.000000 ANNarchy-4.7.3/ANNarchy.egg-info/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     8687 2024-03-21 20:45:45.000000 ANNarchy-4.7.3/ANNarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        1 2024-03-21 20:45:45.000000 ANNarchy-4.7.3/ANNarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 vitay      (501) staff       (20)       47 2024-03-21 20:45:45.000000 ANNarchy-4.7.3/ANNarchy.egg-info/requires.txt
+-rw-r--r--   0 vitay      (501) staff       (20)        9 2024-03-21 20:45:45.000000 ANNarchy-4.7.3/ANNarchy.egg-info/top_level.txt
+-rw-r--r--   0 vitay      (501) staff       (20)      155 2024-03-21 20:38:14.000000 ANNarchy-4.7.3/AUTHORS
+-rw-r--r--   0 vitay      (501) staff       (20)    18092 2017-07-25 21:20:59.000000 ANNarchy-4.7.3/LICENSE
+-rw-r--r--   0 vitay      (501) staff       (20)      274 2021-06-05 08:46:21.000000 ANNarchy-4.7.3/MANIFEST.in
+-rw-r--r--   0 vitay      (501) staff       (20)     2996 2024-03-21 20:45:45.816159 ANNarchy-4.7.3/PKG-INFO
+-rw-r--r--   0 vitay      (501) staff       (20)     1803 2024-02-08 08:00:55.000000 ANNarchy-4.7.3/README.md
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.777596 ANNarchy-4.7.3/examples/
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.808987 ANNarchy-4.7.3/examples/ann_to_snn/
+-rw-r--r--   0 vitay      (501) staff       (20)     3912 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/ann_to_snn/ANNtoSNN.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.809383 ANNarchy-4.7.3/examples/bar_learning/
+-rw-r--r--   0 vitay      (501) staff       (20)     1844 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/examples/bar_learning/BarLearning.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2104 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/examples/bar_learning/BarLearningGPU.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1610 2022-02-01 11:22:20.000000 ANNarchy-4.7.3/examples/bar_learning/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.809650 ANNarchy-4.7.3/examples/bold_monitor/
+-rw-r--r--   0 vitay      (501) staff       (20)     2529 2021-10-04 08:20:34.000000 ANNarchy-4.7.3/examples/bold_monitor/BOLD.py
+-rw-r--r--   0 vitay      (501) staff       (20)     3003 2021-10-04 08:20:34.000000 ANNarchy-4.7.3/examples/bold_monitor/BOLD_two_inputs.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.809774 ANNarchy-4.7.3/examples/gap_junctions/
+-rw-r--r--   0 vitay      (501) staff       (20)      888 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/examples/gap_junctions/GapJunctions.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.809896 ANNarchy-4.7.3/examples/hodgkin_huxley/
+-rw-r--r--   0 vitay      (501) staff       (20)     2496 2023-04-12 11:51:52.000000 ANNarchy-4.7.3/examples/hodgkin_huxley/HodgkinHuxley.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.810195 ANNarchy-4.7.3/examples/homeostatic_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     5055 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/homeostatic_stdp/Ramp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7090 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/homeostatic_stdp/SORF.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.810382 ANNarchy-4.7.3/examples/hybrid/
+-rw-r--r--   0 vitay      (501) staff       (20)     2865 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/hybrid/Hybrid.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.810988 ANNarchy-4.7.3/examples/image/
+-rw-r--r--   0 vitay      (501) staff       (20)     6177 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/image/Image.py
+-rw-r--r--   0 vitay      (501) staff       (20)     7210 2020-05-31 10:28:52.000000 ANNarchy-4.7.3/examples/image/Webcam.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)     2959 2020-05-31 10:28:52.000000 ANNarchy-4.7.3/examples/image/Webcam.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.811108 ANNarchy-4.7.3/examples/izhikevich/
+-rw-r--r--   0 vitay      (501) staff       (20)     1901 2022-02-01 11:22:20.000000 ANNarchy-4.7.3/examples/izhikevich/Izhikevich.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.811241 ANNarchy-4.7.3/examples/multinetwork/
+-rw-r--r--   0 vitay      (501) staff       (20)     1973 2022-02-02 12:32:46.000000 ANNarchy-4.7.3/examples/multinetwork/MultiNetwork.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.811738 ANNarchy-4.7.3/examples/neural_field/
+-rw-r--r--   0 vitay      (501) staff       (20)     1849 2020-05-31 10:28:52.000000 ANNarchy-4.7.3/examples/neural_field/BubbleWorld.pyx
+-rw-r--r--   0 vitay      (501) staff       (20)     1490 2020-03-10 16:42:35.000000 ANNarchy-4.7.3/examples/neural_field/NeuralField.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2281 2022-02-01 11:22:20.000000 ANNarchy-4.7.3/examples/neural_field/Viz.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.812464 ANNarchy-4.7.3/examples/pyNN/
+-rw-r--r--   0 vitay      (501) staff       (20)     1644 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/AEIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2251 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/EIF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1427 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/IF_cond_exp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1361 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/IF_curr_alpha.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1316 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/non_linear_synapse.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2646 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/pyNN/short_term_plasticity2.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.812578 ANNarchy-4.7.3/examples/refractoriness/
+-rw-r--r--   0 vitay      (501) staff       (20)     1070 2019-07-10 20:15:51.000000 ANNarchy-4.7.3/examples/refractoriness/Refractoriness.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.812706 ANNarchy-4.7.3/examples/simple_stdp/
+-rw-r--r--   0 vitay      (501) staff       (20)     2208 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/examples/simple_stdp/SimpleSTDPModel.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.812838 ANNarchy-4.7.3/examples/structural_plasticity/
+-rw-r--r--   0 vitay      (501) staff       (20)     1923 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/examples/structural_plasticity/StructuralPlasticity.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.814623 ANNarchy-4.7.3/examples/tensorboard/
+-rw-r--r--   0 vitay      (501) staff       (20)  1014400 2021-10-01 13:31:48.000000 ANNarchy-4.7.3/examples/tensorboard/BasalGanglia.ipynb
+-rw-r--r--   0 vitay      (501) staff       (20)   208036 2021-07-27 06:26:43.000000 ANNarchy-4.7.3/examples/tensorboard/BayesianOptimization.ipynb
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.815413 ANNarchy-4.7.3/examples/tsodyks_markram/
+-rw-r--r--   0 vitay      (501) staff       (20)     3872 2023-04-12 10:39:20.000000 ANNarchy-4.7.3/examples/tsodyks_markram/TsodyksMarkram.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.815652 ANNarchy-4.7.3/examples/vogels_abbott/
+-rw-r--r--   0 vitay      (501) staff       (20)     2857 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/vogels_abbott/COBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     2724 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/examples/vogels_abbott/CUBA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1355 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/pyproject.toml
+-rw-r--r--   0 vitay      (501) staff       (20)       99 2024-02-08 08:00:55.000000 ANNarchy-4.7.3/requirements.txt
+-rw-r--r--   0 vitay      (501) staff       (20)      101 2024-03-21 20:45:45.816358 ANNarchy-4.7.3/setup.cfg
+-rw-r--r--   0 vitay      (501) staff       (20)     8508 2024-03-21 20:38:15.000000 ANNarchy-4.7.3/setup.py
+drwxr-xr-x   0 vitay      (501) staff       (20)        0 2024-03-21 20:45:45.815974 ANNarchy-4.7.3/tests/
+-rw-r--r--   0 vitay      (501) staff       (20)     1122 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/tests/test_CUDA.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1062 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/tests/test_openmp.py
+-rw-r--r--   0 vitay      (501) staff       (20)     1149 2022-12-14 10:27:19.000000 ANNarchy-4.7.3/tests/test_single_thread.py
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/__init__.py` & `ANNarchy-4.7.3/ANNarchy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Generic imports
-from __future__ import print_function
 import os, sys
 import numpy as np
 
 # ANNarchy core
 from .core.Global import *
 from .core.Simulate import *
 from .core.Neuron import Neuron
 from .core.Synapse import Synapse
 from .core.Population import Population
 from .core.Projection import Projection
 from .core.SpecificPopulation import PoissonPopulation, SpikeSourceArray, TimedArray, HomogeneousCorrelatedSpikeTrains, TimedPoissonPopulation
 from .core.SpecificProjection import DecodingProjection, CurrentInjection
 from .core.Dendrite import Dendrite
-from .core.Random import Uniform, DiscreteUniform, Normal, LogNormal, Gamma, Exponential
+from .core.Random import Uniform, DiscreteUniform, Normal, LogNormal, Gamma, Exponential, Binomial
 from .core.IO import save, load, load_parameter, load_parameters, save_parameters
-from .core.Utils import sparse_random_matrix
-from .core.Monitor import Monitor, raster_plot, histogram, population_rate, smoothed_rate, mean_fr
+from .core.Utils import sparse_random_matrix, sparse_delays_from_weights
+from .core.Monitor import *
 from .core.Network import Network, parallel_run
 from .parser.report.Report import report
 from .models.Neurons import *
 from .models.Synapses import *
 from .extensions import *
 
 # Cython modules
@@ -34,19 +33,24 @@
     print("""
 Warning: Cython modules can not be imported. If you are installing ANNarchy, this is normal, ignore this message. If ANNarchy is already installed, something went wrong with the compilation, try reinstalling.
 """)
 
 # ANNarchy compilation
 from .generator import compile
 
+# several setup() arguments can be set on command-line
+from ANNarchy.generator.CmdLineArgParser import CmdLineArgParser
+_arg_parser = CmdLineArgParser()
+_arg_parser.parse_arguments_for_setup()
+
 # Automatically call ANNarchy.core.Global.clear()
 # if the script terminates
 import atexit
 atexit.register(check_profile_results)
 atexit.register(clear)
 
 # Version
 __version__ = '4.7'
-__release__ = '4.7.2.6'
+__release__ = '4.7.3'
 
 print( 'ANNarchy ' + __version__ + ' (' + __release__ + \
                     ') on ' + sys.platform + ' (' + os.name + ').' )
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/ConnectorMethods.py` & `ANNarchy-4.7.3/ANNarchy/core/ConnectorMethods.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,14 @@
-#===============================================================================
-#
-#     ConnectorMethods.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+Implements the built-in connectivity patterns available in ANNarchy. See the documentaton
+for more details: https://annarchy.readthedocs.io/en/latest/manual/Connector.html
+
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 import numpy as np
 
 from ANNarchy.core import Global
 from ANNarchy.core.Random import RandomDistribution, DiscreteUniform
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.parser.report.LatexParser import _process_random
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Dendrite.py` & `ANNarchy-4.7.3/ANNarchy/core/Dendrite.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,19 @@
-#===============================================================================
-#
-#     Dendrite.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 from ANNarchy.core import Synapse
 from ANNarchy.core.Random import RandomDistribution
 
 import numpy as np
 
-class Dendrite(object):
+class Dendrite :
     """
     A ``Dendrite`` is a sub-group of a ``Projection``, gathering the synapses between the pre-synaptic population and a single post-synaptic neuron.
 
     It can not be created directly, only through a call to ``Projection.dendrite(rank)``:
 
     ```python
     dendrite = proj.dendrite(6)
@@ -278,14 +260,59 @@
                 extra_attributes[var['name']] = init
 
         try:
             self.proj.cyInstance.add_synapse(self.post_rank, rank, w, int(delay/Global.config['dt']), **extra_attributes)
         except Exception as e:
             Global._print(e)
 
+    def create_synapses(self, ranks, weights=None, delays=None):
+        """
+        Creates a synapse for this dendrite with the given pre-synaptic neuron.
+
+        :param ranks: rank of the pre-synaptic neuron
+        :param weights: synaptic weight (defalt: 0.0).
+        :param delays: synaptic delay (default = dt)
+        """
+        if not Global.config['structural_plasticity']:
+            Global._error('"structural_plasticity" has not been set to True in setup(), can not add the synapse.')
+            return
+
+        # No user-side init
+        if weights is None:
+            weights = [0.0] * len(ranks)
+
+        if delays is None:
+            delays = [0] * len(ranks)
+
+        # Collect other attributes than w/delay
+        extra_attribute_names = []
+        for var in self.proj.synapse_type.description['parameters'] + self.proj.synapse_type.description['variables']:
+            if not var['name'] in ['w', 'delay'] and  var['name'] in self.proj.synapse_type.description['local']:
+                extra_attribute_names.append[var['name']]
+
+        # Create the synapses
+        for rank, w, delay in zip(ranks, weights, delays):
+            if self.proj.cyInstance.dendrite_index(self.post_rank, rank) != -1:
+                Global._error('the synapse of rank ' + str(ranks) + ' already exists.')
+                return
+
+            # Set default values for the additional variables
+            extra_attributes = {}
+            for var in extra_attribute_names:
+                if not isinstance(self.proj.init[var], (int, float, bool)):
+                    init = var['init']
+                else:
+                    init = self.proj.init[var]
+                extra_attributes[var] = init
+
+            try:
+                self.proj.cyInstance.add_synapse(self.post_rank, rank, w, int(delay/Global.config['dt']), **extra_attributes)
+            except Exception as e:
+                Global._print(e)
+
     def prune_synapse(self, rank):
         """
         Removes the synapse with the given pre-synaptic neuron from the dendrite.
 
         :param rank: rank of the pre-synaptic neuron
         """
         if not Global.config['structural_plasticity']:
@@ -294,16 +321,28 @@
 
         if not rank in self.pre_ranks:
             Global._error('the synapse with the pre-synaptic neuron of rank ' + str(rank) + ' did not already exist.')
             return
 
         self.proj.cyInstance.remove_synapse(self.post_rank, rank)
 
+    def prune_synapses(self, ranks):
+        """
+        Removes the synapses which belong to the provided pre-synaptic neurons from the dendrite.
+
+        :param ranks: list of ranks of the pre-synaptic neurons
+        """
+        if not Global.config['structural_plasticity']:
+            Global._error('"structural_plasticity" has not been set to True in setup(), can not remove the synapse.')
+            return
+
+        for rank in ranks:
+            self.prune_synapse(rank)
 
-class IndividualSynapse(object):
+class IndividualSynapse :
 
     def __init__(self, dendrite, rank):
         self.dendrite = dendrite
         self.rank = rank
 
     def __getattr__(self, name):
         " Method called when accessing an attribute."
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Global.py` & `ANNarchy-4.7.3/ANNarchy/core/Global.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,20 @@
-#===============================================================================
-#
-#     Global.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+Contains global available functions and state variables,
+e.g., the config dictionary and holds a reference to 
+network instances.
+
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import sys, os
 import inspect
 import traceback
 import numpy as np
-import argparse
 
 from ANNarchy.core.NetworkManager import NetworkManager
 
 # High-level structures
 _objects = {
     'functions': [],
     'neurons': [],
@@ -49,25 +34,26 @@
     'show_time': False,
     'suppress_warnings': False,
     'num_threads': 1,
     'visible_cores': [],
     'paradigm': "openmp",
     'method': "explicit",
     'sparse_matrix_format': "default",
+    'sparse_matrix_storage_order': "post_to_pre",
     'precision': "double",
     'only_int_idx_type': True,
     'seed': -1,
     'structural_plasticity': False,
     'profiling': False,
     'profile_out': None,
     'disable_parallel_rng': True,
     'use_seed_seq': True,
     'use_cpp_connectors': False,
     'disable_split_matrix': True,
-    'disable_SIMD_SpMV': False,
+    'disable_SIMD_SpMV': True,
     'disable_SIMD_Eq': False,
     'disable_shared_library_time_offset': False
    }
 )
 
 # This flags can not be configured through setup()
 _performance_related_config_keys = [
@@ -115,15 +101,18 @@
 def setup(**keyValueArgs):
     """
     The setup function is used to configure ANNarchy simulation environment. It takes various optional arguments:
 
     * dt: simulation step size (default: 1.0 ms).
     * paradigm: parallel framework for code generation. Accepted values: "openmp" or "cuda" (default: "openmp").
     * method: default method to numerize ODEs. Default is the explicit forward Euler method ('explicit').
-    * sparse_matrix_format: the default matrix format for projections in ANNarchy (by default: List-In-List for CPUs and Compressed Sparse Row)
+    * sparse_matrix_format: the default matrix format for projections in ANNarchy (by default: List-In-List for CPUs and Compressed Sparse Row).
+                            Note that affects only the C++ data structures.
+    * sparse_matrix_storage_order: encodes whether the row in a connectivity matrix encodes pre-synaptic neurons (post_to_pre, default) or 
+                                   post-synaptic neurons (pre_to_post). Note that affects only the C++ data structures.
     * precision: default floating precision for variables in ANNarchy. Accepted values: "float" or "double" (default: "double")
     * num_threads: number of treads used by openMP (overrides the environment variable ``OMP_NUM_THREADS`` when set, default = None).
     * visible_cores: allows a fine-grained control which cores are useable for the created threads (default = [] for no limitation).
                      It can be used to limit created openMP threads to a physical socket.
     * structural_plasticity: allows synapses to be dynamically added/removed during the simulation (default: False).
     * seed: the seed (integer) to be used in the random number generators (default = -1 is equivalent to time(NULL)).
 
@@ -210,47 +199,56 @@
         if key not in _performance_related_config_keys:
             _error("The key", key, "does not belong to the performance related keys.")
 
         if key in config.keys():
             config[key] = keyValueArgs[key]
 
             if key == "use_cpp_connectors":
-                _warning("use_cpp_connectors=True is currently disabled, will be enabled soon.")
-                config["use_cpp_connectors"] = False
+                if config[key] == True:
+                    _warning("use_cpp_connectors is an experimental feature, we greatly appreciate bug reports.")
+
+                    if "disable_parallel_rng" in config.keys():
+                        if config["use_cpp_connectors"] and config["disable_parallel_rng"]:
+                            _warning("If 'use_cpp_connectors' is enabled, the 'disable_parallel_rng' flag should be disabled for maximum efficiency.")
 
         else:
             _warning('_optimization_flags(): unknown key:', key)
 
         if key == 'seed': # also seed numpy
             np.random.seed(keyValueArgs[key])
 
         if key == 'sparse_matrix_format':
             # check if this is a supported format
             if keyValueArgs[key] not in ["lil", "csr", "csr_vector", "csr_scalar", "dense", "ell", "ellr", "sell", "coo", "bsr", "hyb", "auto"]:
                 _error("The value", keyValueArgs[key], "provided to sparse_matrix_format is not valid.")
 
 
-def clear():
+def clear(functions=True, neurons=True, synapses=True, constants=True):
     """
     Clears all variables (erasing already defined populations, projections, monitors and constants), as if you had just imported ANNarchy.
 
+    * functions: if True (default), all functions defined with ``add_function`` are erased.
+    * neurons: if True (default), all neurons defined with ``Neuron`` are erased.
+    * synapses: if True (default), all synapses defined with ``Synapse`` are erased.
+    * constants: if True (default), all constants defined with ``Constant`` are erased.
+
     Useful when re-running Jupyter/IPython notebooks multiple times:
 
     ```python
     from ANNarchy import *
     clear()
     ```
     """
     # Reset objects
     global _objects
     _objects = {
-        'functions': [],
-        'neurons': [],
-        'synapses': [],
-        'constants': [],
+        'functions': [] if functions else _objects['functions'],
+        'neurons': [] if neurons else _objects['neurons'],
+        'synapses': [] if synapses else _objects['synapses'],
+        'constants': [] if constants else _objects['constants'],
     }
 
     # Remove the present profiler
     global _profiler
     if _profiler is not None:
         check_profile_results()
 
@@ -269,14 +267,24 @@
     If the user enabled profiling, we here check if we recorded some results.
     """
     if _profiler:
         _profiler.print_profile()
 
         _profiler.store_cpp_time_as_csv()
 
+def get_profiling_instance():
+    """
+    Get profiling instance which requires Global.config["profiling"] == True.
+    """
+    if _profiler:
+        return _profiler
+    else:
+        _warning("To use Profiler instance please activate profiling first.")
+        return None
+
 def reset(populations=True, projections=False, synapses=False, monitors=True, net_id=0):
     """
     Reinitialises the network to its state before the call to compile. The network time will be set to 0ms.
 
     All monitors are emptied.
 
     :param populations: if True (default), the neural parameters and variables will be reset to their initial value.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/IO.py` & `ANNarchy-4.7.3/ANNarchy/core/IO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,14 @@
-#===============================================================================
-#
-#     IO.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+Contains functions for load/save of parameters, connectivtiy and complete networks.
+
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 import os
 import pickle
 import numpy as np
 
 
 def load_parameters(filename, global_only=True, verbose=False, net_id=0):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Monitor.py` & `ANNarchy-4.7.3/ANNarchy/core/Monitor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,30 @@
-#===============================================================================
-#
-#     Monitor.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from . import Global
 from .Population import Population
 from .PopulationView import PopulationView
 from .Projection import Projection
 from .Dendrite import Dendrite
 
 import numpy as np
 import re
 import sys
 from copy import copy, deepcopy
 
-class Monitor(object):
+# objects/functions that should be available by "from ANNarchy import *"
+__all__ = ["Monitor", "raster_plot", "histogram", "population_rate", "smoothed_rate", "mean_fr", "inter_spike_interval", "coefficient_of_variation"]
+
+class Monitor :
     """
     Monitoring class allowing to record easily parameters or variables from Population, PopulationView, Dendrite or Projection objects.
-    
+
     Example:
 
     ```python
     m = Monitor(pop, ['g_exc', 'v', 'spike'], period=10.0)
     ```
 
     It is also possible to record the sum of inputs to each neuron in a rate-coded population:
@@ -181,20 +166,20 @@
         """
         Adds a variable to the list of recorded attributes.
         """
         if not var in self._variables:
             self._variables.append(var)
 
         self._recorded_variables[var] = {
-            'start': [Global.get_current_step(self.net_id)], 
+            'start': [Global.get_current_step(self.net_id)],
             'stop': [None],
         }
 
         self._last_recorded_variables[var] = {
-            'start': [Global.get_current_step(self.net_id)], 
+            'start': [Global.get_current_step(self.net_id)],
             'stop': [None],
         }
 
     def reset(self):
         """
         Reset the monitor to its initial state.
         """
@@ -262,16 +247,16 @@
             self._add_variable(var)
 
         # Start recordings if enabled
         if self._start:
             self.start()
 
     def start(self, variables=None, period=None):
-        """Starts recording the variables. 
-        
+        """Starts recording the variables.
+
         It is called automatically after ``compile()`` if the flag ``start`` was not passed to the constructor.
 
         :param variables: single variable name or list of variable names to start recording (default: the ``variables`` argument passed to the constructor).
         :param period: delay in ms between two recording (default: dt). Not valid for the ``spike`` variable of a Population(View).
         """
         if variables:
             if not isinstance(variables, list):
@@ -326,15 +311,15 @@
                 if isinstance(self.object, (Population, PopulationView)):
                     obj_desc = 'population ' + self.object.name
                 elif isinstance(self.object, Projection):
                     obj_desc = 'projection between ' + self.object.pre.name+' and '+self.object.post.name
                 else:
                     obj_desc = 'dendrite between '+self.object.proj.pre.name+' and '+self.object.proj.post.name
                 Global._warning('Monitor:' + var + ' can not be recorded ('+obj_desc+')')
-            
+
             self._recorded_variables[var]['stop'][-1] = Global.get_current_step(self.net_id)
 
 
     def resume(self):
         "Resumes the recordings."
         # Start recording the variables
         for var in self.variables:
@@ -350,15 +335,15 @@
                 if isinstance(self.object, (Population, PopulationView)):
                     obj_desc = 'population '+self.object.name
                 elif isinstance(self.object, Projection):
                     obj_desc = 'projection between '+self.object.pre.name+' and '+self.object.post.name
                 else:
                     obj_desc = 'dendrite between '+self.object.proj.pre.name+' and '+self.object.proj.post.name
                 Global._warning('Monitor:' + var + ' can not be recorded ('+obj_desc+')')
-            
+
             self._recorded_variables[var]['start'].append(Global.get_current_step(self.net_id))
             self._recorded_variables[var]['stop'].append(None)
 
     def stop(self):
         """
         Stops the recording.
 
@@ -433,15 +418,15 @@
             data[var] = return_variable(self, name, keep)
 
             # Update stopping time
             self._recorded_variables[var]['stop'][-1] = Global.get_current_step(self.net_id)
 
             self._last_recorded_variables[var]['start'] = self._recorded_variables[var]['start']
             self._last_recorded_variables[var]['stop'] = self._recorded_variables[var]['stop']
-            
+
             if not keep:
                 self._recorded_variables[var]['start'] = [Global.get_current_step(self.net_id)]
                 self._recorded_variables[var]['stop'] = [None]
 
         if not force_dict and len(variables)==1:
             return data[variables[0]]
         else:
@@ -463,19 +448,19 @@
     def _get_dendrite(self, proj, name, keep):
         try:
             data = getattr(self.cyInstance, name)
             if not keep:
                 getattr(self.cyInstance, 'clear_' + name)()
         except:
             data = []
-        return np.array(data)
+        return np.array(data, dtype=object)
 
     def times(self, variables=None):
         """
-        Returns the start and stop times (in ms) of the recorded variables. 
+        Returns the start and stop times (in ms) of the recorded variables.
 
         It should only be called after a call to ``get()``, so that it describes when the variables have been recorded.
 
         :param variables: (list of) variables. By default, the times for all variables is returned.
         """
         t = {}
         if variables:
@@ -541,15 +526,15 @@
         for n in data.keys():
             for t in data[n]:
                 times.append(t)
                 ranks.append(n)
 
         return Global.dt()* np.array(times), np.array(ranks)
 
-    def histogram(self, spikes=None, bins=None):
+    def histogram(self, spikes=None, bins=None, per_neuron=False, recording_window=None):
         """
         Returns a histogram for the recorded spikes in the population.
 
         Example:
 
         ```python
         m = Monitor(P[:1000], 'spike')
@@ -566,48 +551,65 @@
         spikes = m.get('spike')
         histo = m.histogram(spikes)
         plt.plot(histo)
         ```
 
         :param spikes: the dictionary of spikes returned by ``get('spike')``. If left empty, ``get('spike')`` will be called. Beware: this erases the data from memory.
         :param bins: the bin size in ms (default: dt).
-
         """
         if not 'spike' in self._variables:
             Global._error('Monitor: spike was not recorded')
 
         # Get data
         if not spikes:
             data = self.get('spike')
         else:
             if 'spike' in spikes.keys():
                 data = spikes['spike']
             else:
                 data = spikes
 
-        if not bins:
-            bins =  Global.config['dt']
+        return histogram(data, bins=bins, per_neuron=per_neuron, recording_window=recording_window)
 
-        # Compute the duration of the recordings
-        t_start = self._last_recorded_variables['spike']['start'][-1]
-        duration = self._last_recorded_variables['spike']['stop'][-1] - self._last_recorded_variables['spike']['start'][-1]
+    def inter_spike_interval(self, spikes=None, ranks=None, per_neuron=False):
+        """
+        Computes the inter-spike interval for the recorded spikes in the population.
 
-        # Number of bins
-        nb_bins = int(duration*Global.config['dt']/bins)
+        :param spikes: the dictionary of spikes returned by ``get('spike')``. If left empty, ``get('spike')`` will be called. Beware: this erases the data from memory.
+        :ranks:        a list of neurons that should be evaluated. By default (None), all neurons are evaluated.
+        :per_neuron:   if set to True, the computed inter-spike intervals are stored per neuron (analog to spikes), otherwise all values are stored in one huge vector (default: False).
+        """
+        # Get data
+        if not spikes:
+            data = self.get('spike')
+        else:
+            if 'spike' in spikes.keys():
+                data = spikes['spike']
+            else:
+                data = spikes
 
-        # Initialize histogram
-        histo = [0 for t in range(nb_bins)]
+        return inter_spike_interval(data, ranks=ranks, per_neuron=per_neuron)
 
-        # Compute histogram
-        neurons = self.object.ranks if isinstance(self.object, PopulationView) else range(self.object.size)
-        for neuron in neurons:
-            for t in data[neuron]:
-                histo[int((t-t_start)/float(bins/Global.config['dt']))] += 1
+    def coefficient_of_variation(self, spikes=None, ranks=None):
+        """
+        Computes the coefficient of variation for the recorded spikes in the population.
 
-        return np.array(histo)
+        :param spikes: the dictionary of spikes returned by ``get('spike')``. If left empty, ``get('spike')`` will be called. Beware: this erases the data from memory.
+        :ranks:        a list of neurons that should be evaluated. By default (None), all neurons are evaluated.
+        """
+        # Get data
+        if not spikes:
+            data = self.get('spike')
+        else:
+            if 'spike' in spikes.keys():
+                data = spikes['spike']
+            else:
+                data = spikes
+
+        return coefficient_of_variation(data, ranks=ranks)
 
     def mean_fr(self, spikes=None):
         """
         Computes the mean firing rate in the population during the recordings.
 
         Example:
 
@@ -759,15 +761,15 @@
         size += sum([get_size(k, seen) for k in obj.keys()])
     elif hasattr(obj, '__dict__'):
         size += get_size(obj.__dict__, seen)
     elif hasattr(obj, '__iter__') and not isinstance(obj, (str, bytes, bytearray)):
         size += sum([get_size(i, seen) for i in obj])
     return size
 
-class MemoryStats(object):
+class MemoryStats :
     """
     Create memory statistics for the main objects in ANNarchy. The current implementation
     focusses on the C++ simulation core. But this module could be further extended to measure
     also the Python objects.
     """
     def __init__(self):
         pass
@@ -832,29 +834,28 @@
         for t in spikes[n]:
             times.append(t)
             ranks.append(n)
 
     return Global.dt()* np.array(times), np.array(ranks)
 
 
-def histogram(spikes, bins=None):
+def histogram(spikes, bins=None, per_neuron=False, recording_window=None):
     """
     Returns a histogram for the recorded spikes in the population.
 
     Example:
 
     ```python
     m = Monitor(P[:1000], 'spike')
     simulate(1000.0)
     spikes = m.get('spike')
     histo = histogram(spikes)
     plt.plot(histo)
     ```
 
-
     :param spikes: the dictionary of spikes returned by ``get('spike')``.
     :param bins: the bin size in ms (default: dt).
     """
     if bins is None:
         bins =  Global.config['dt']
 
     bin_step = int(bins/Global.config['dt'])
@@ -863,32 +864,102 @@
     t_maxes = []
     t_mines = []
     for neuron in spikes.keys():
         if len(spikes[neuron]) == 0 : continue
         t_maxes.append(np.max(spikes[neuron]))
         t_mines.append(np.min(spikes[neuron]))
 
-    t_max = np.max(t_maxes)
-    t_min = np.min(t_mines)
+    if recording_window is None:
+        t_max = np.max(t_maxes)
+        t_min = np.min(t_mines)
+    else:
+        t_min = recording_window[0]
+        t_max = recording_window[1]
     duration = t_max - t_min
 
     # Number of bins
     nb_bins = int(duration/bin_step)
     #print(t_min, t_max, duration, nb_bins)
 
-    # Initialize histogram
-    histo = [0 for t in range(nb_bins+1)]
+    if per_neuron:
+        max_rank = np.amax([x for x in spikes.keys()])+1
+        # Initialize histogram
+        histo = [ [0 for _ in range(nb_bins+1)] for _ in range(max_rank) ]
 
-    # Compute per step histogram
-    for neuron in spikes.keys():
-        for t in spikes[neuron]:
-            histo[int((t-t_min)/float(bin_step))] += 1
+        # Compute per step histogram
+        for neuron in spikes.keys():
+            for t in spikes[neuron]:
+                histo[neuron][int((t-t_min)/float(bin_step))] += 1
+
+    else:
+        # Initialize histogram
+        histo = [0 for t in range(nb_bins+1)]
+
+        # Compute per step histogram
+        for neuron in spikes.keys():
+            for t in spikes[neuron]:
+                histo[int((t-t_min)/float(bin_step))] += 1
 
     return np.array(histo)
 
+def inter_spike_interval(spikes, ranks=None, per_neuron=False):
+    """
+    Computes the inter-spike interval for the record spike events of a population.
+    """
+    isi = {}
+    for neuron_rank, spike_events in spikes.items():
+        # ISI computation requires at least 2 events
+        if len(spike_events) < 2:
+            continue
+
+        # suppress unwanted neurons
+        if ranks is not None:
+            if neuron_rank not in ranks:
+                continue
+
+        # compute time difference between spike events
+        tmp_isi=[]
+        for idx in range(len(spike_events)-1):
+            tmp_isi.append((spike_events[idx+1]-spike_events[idx])*Global.dt())
+
+        isi[neuron_rank] = tmp_isi
+
+    if per_neuron:
+        return isi
+    else:
+        res = []
+        for val in isi.values():
+            res.extend(val)
+        return res
+
+def coefficient_of_variation(spikes, ranks=None, per_neuron=False):
+    """
+    Computes the coefficient of variation of the inter-spike intervals for the recorded spike events of a population.
+    """
+    isi_per_neuron = inter_spike_interval(spikes, ranks=ranks, per_neuron=True)
+    isi_cv = {}
+    for neuron_rank, values in isi_per_neuron.items():
+        if len(values) < 2:
+            continue     # no meaningful mean/std possible
+
+        # suppress unwanted neurons
+        if ranks is not None:
+            if neuron_rank not in ranks:
+                continue
+
+        isi_cv[neuron_rank] = np.std(values) / np.mean(values)
+
+    if per_neuron:
+        return isi_cv
+    else:
+        res = []
+        for val in isi_cv.values():
+            res.append(val)
+        return res
+
 def population_rate(spikes, smooth=0.0):
     """
     Takes the recorded spikes of a population and returns a smoothed firing rate for the population of recorded neurons.
 
     This method is faster than calling ``smoothed_rate`` and then averaging.
 
     The first axis is the neuron index, the second is time.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Network.py` & `ANNarchy-4.7.3/ANNarchy/core/Network.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-#===============================================================================
-#
-#     Network.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from .Population import Population
 from .PopulationView import PopulationView
 from .Projection import Projection
 from .Monitor import Monitor
 from ANNarchy.extensions.bold import BoldMonitor
 
 import ANNarchy.core.Global as Global
 import ANNarchy.core.Simulate as Simulate
 import ANNarchy.core.IO as IO
 import ANNarchy.core.SpecificPopulation as SpecificPopulation
 import ANNarchy.generator.Compiler as Compiler
 import numpy as np
 import os
 
-class Network(object):
+class Network :
     """
     A network gathers already defined populations, projections and monitors in order to run them independently.
 
     This is particularly useful when varying single parameters of a network and comparing the results (see the ``parallel_run()`` method).
 
     Only objects declared before the creation of the network can be used. Global methods such as ``simulate()`` must be used on the network object.
     The objects must be accessed through the ``get()`` method, as the original ones will not be part of the network (a copy is made).
@@ -575,15 +557,25 @@
 
         :param filename: filename, may contain relative or absolute path.
         :param populations: if True, population data will be saved (by default True)
         :param projections: if True, projection data will be saved (by default True)
         """
         IO.save(filename, populations, projections, self.id)
 
-def parallel_run(method, networks=None, number=0, max_processes=-1, measure_time=False, sequential=False, same_seed=False, annarchy_json="", visible_cores=[], **args):
+def parallel_run(
+        method, 
+        networks=None, 
+        number=0, 
+        max_processes=-1, 
+        measure_time=False, 
+        sequential=False, 
+        same_seed=False, 
+        annarchy_json="", 
+        visible_cores=[], 
+        **args):
     """
     Allows to run multiple networks in parallel using multiprocessing.
 
     If the ``networks`` argument is provided as a list of Network objects, the given method will be executed for each of these networks.
 
     If ``number`` is given instead, the same number of networks will be created and the method is applied.
 
@@ -616,18 +608,18 @@
     :param method: a Python method which will be executed for each network. This function must accept an integer as first argument (id of the simulation) and a Network object as second argument.
     :param networks: a list of networks to simulate in parallel.
     :param number: the number of identical networks to run in parallel.
     :param max_processes: maximal number of processes to start concurrently (default: the available number of cores on the machine).
     :param measure_time: if the total simulation time should be printed out.
     :param sequential: if True, runs the simulations sequentially instead of in parallel (default: False).
     :param same_seed: if True, all networks will use the same seed. If not, the seed will be randomly initialized with time(0) for each network (default). It has no influence when the ``networks`` argument is set (the seed has to be set individually for each network using ``net.set_seed()``), only when ``number`` is used.
-    :param annarchy.json: path to a different configuration file if needed (default "").
+    :param annarchy_json: path to a different configuration file if needed (default "").
     :param visible_cores: a list of CPU core ids to simulate on (must have max_processes entries and max_processes must be != -1)
     :param args: other named arguments you want to pass to the simulation method.
-    :return: a list of the values returned by ``method``.
+    :returns: a list of the values returned by ``method``.
 
     """
     # Check inputs
     if not networks and number < 1:
         Global._error('parallel_run(): the networks or number arguments must be set.', exit=True)
 
     if len(visible_cores) > 0 and max_processes == -1:
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/NetworkManager.py` & `ANNarchy-4.7.3/ANNarchy/core/NetworkManager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,18 @@
-#===============================================================================
-#
-#     NetworkManager.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020 Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
+
 import os
+import shutil
 
-class NetworkManager(object):
+class NetworkManager :
     """
     This class implements the management of the data for the different networks. The
     add/remove methods allow the 'random' removal of the network instances and later
     refill of empty spaces.
 
     The class will be placed and instantiated in the ANNarchy.core.Global file.
     """
@@ -188,16 +172,30 @@
             pass
 
         elif self._network[0]['directory'] != None:
             # Removes the library used in last running instance
             if os.path.isfile(self._network[0]['directory']+'/ANNarchyCore' + str(0) + '.so'):
                 os.remove(self._network[0]['directory']+'/ANNarchyCore' + str(0) + '.so')
 
-            if os.path.isdir(self._network[0]['directory']):
-                os.rmdir(self._network[0]['directory'])
+            try:
+                if os.path.isdir(self._network[0]['directory']):
+                    os.rmdir(self._network[0]['directory'])
+
+            except OSError as err:
+                # we notice a not empty directory error
+                if err.errno == 39:
+                    if Global.config["debug"] or Global.config["verbose"]:
+                        Global._warning("Attempted to clear:", self._network[0]['directory'], "using os.rmdir failed ... retry with shutil")
+
+                    # we re-try it with shutil, if it again fails, we ignore it ...
+                    shutil.rmtree(self._network[0]['directory'], ignore_errors=True)
+
+                else:
+                    # Re-throw other errors
+                    raise
 
             self._network[0]['directory'] = None
 
         # This will trigger as last consequence
         # Network.__del__()
         del self._network
         self._create_initial_state()
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Neuron.py` & `ANNarchy-4.7.3/ANNarchy/core/Neuron.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,18 @@
-#===============================================================================
-#
-#     Neuron.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Global import _error, _warning, _objects, config
 from ANNarchy.parser.AnalyseNeuron import analyse_neuron
 from ANNarchy.core.PopulationView import PopulationView
 import numpy as np
 
-class Neuron(object):
+class Neuron :
     """
     Base class to define a neuron.
     """
     # Default name and description for reporting
     _default_names = {'rate': "Rate-coded neuron", 'spike': "Spiking neuron"}
 
     def __init__(self, parameters="", equations="", spike=None, axon_spike=None, reset=None, axon_reset=None, refractory = None, functions=None, name="", description="", extra_values={} ):
@@ -114,15 +96,15 @@
 """ + str(self.axon_spike) + """
 Reset after a spike:
 """ + str(self.reset)
 
         return text
 
 
-class IndividualNeuron(object):
+class IndividualNeuron :
     """
     Neuron object returned by the Population.neuron(rank) method.
 
     This only a wrapper around the Population data. It has the same attributes (parameter and variable) as the original population.
     """
     def __init__(self, population, rank):
         self.population  = population
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Population.py` & `ANNarchy-4.7.3/ANNarchy/core/Population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,23 @@
-#===============================================================================
-#
-#     Population.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 
 from .PopulationView import PopulationView
 from .Random import RandomDistribution
 from .Neuron import IndividualNeuron
 
 import numpy as np
 import copy, inspect
 
 
-class Population(object):
+class Population :
     """
     Container for a population of homogeneous neurons.
     """
 
     def __init__(self, geometry, neuron, name=None, stop_condition=None, storage_order='post_to_pre', copied=False):
         """
         :param geometry: population geometry as tuple. If an integer is given, it is the size of the population.
@@ -183,20 +165,33 @@
         return Population(geometry=self.geometry, neuron=self.neuron_type, name=self.name, stop_condition=self.stop_condition, storage_order=self._storage_order, copied=True)
 
     def _generate(self):
         "Overriden by specific populations to generate the code."
         pass
 
     def _instantiate(self, module):
-        # Create the Cython instance
+        """
+        Instantiates the population after compilation of the C++ simulation core.
+        The function should solely called by Compiler._instantiate().
+
+        :param:     module  cython module (ANNarchyCore instance)
+        """
+        if Global.config["profiling"]:
+            import time
+            t1 = time.time()
+
         try:
             self.cyInstance = getattr(module, self.class_name+'_wrapper')(self.size, self.max_delay)
         except:
             Global._error('unable to instantiate the population', self.name)
 
+        if Global.config["profiling"]:
+            t2 = time.time()
+            Global._profiler.add_entry(t1, t2, "pop"+str(self.id), "instantiate")
+
     def _init_attributes(self):
         """ Method used after compilation to initialize the attributes."""
         # Initialize the population
         self.initialized = True
 
         # Transfer the initial values of all attributes
         for name, value in self.init.items():
@@ -392,22 +387,21 @@
                 ctype = var['ctype']
                 break
 
         return ctype
 
     def __len__(self):
         # Number of neurons in the population.
-        
         return self.size
 
 
     def set(self, values):
         """
         Sets the value of neural variables and parameters.
-        
+
         Example:
 
         ```python
         pop.set({ 'tau' : 20.0, 'r'= np.random.rand((8,8)) } )
         ```
 
         :param values: dictionary of attributes to be updated.
@@ -523,15 +517,15 @@
         This method has an effect on spiking neurons only.
 
         If this method is not called, `r` will always be 0.0. `r` can of course be accessed and recorded as any other variable.
 
         :param window: window in ms over which the spikes will be counted.
         """
         if Global._check_paradigm('cuda'):
-            Global._error('compute_firing_rate() is not supported on CUDA yet.')
+            Global._warning('compute_firing_rate() is currently being evaluated on the host-side, so may be slow ... ')
 
         if self.neuron_type.type == 'rate':
             Global._error('compute_firing_rate(): the neuron is already rate-coded...')
 
         self._compute_mean_fr = float(window)
 
         if self.initialized:
@@ -614,20 +608,30 @@
                 if indices.ndim != 1:
                     Global._error('only one-dimensional lists/arrays are allowed to address a population.')
 
             return PopulationView(self, indices, geometry=(len(indices),))
 
         elif isinstance(indices, slice): # a single slice of ranks
             start, stop, step = indices.start, indices.stop, indices.step
+
+            # no value defined for a position
             if indices.start is None:
                 start = 0
             if indices.stop is None:
                 stop = self.size
             if indices.step is None:
                 step = 1
+
+            # start or end arguments are negative
+            if start < 0:
+                start = self.size + start
+            if stop < 0:
+                stop = self.size + stop
+
+            # generate a new set of indices
             rk_range = np.arange(start, stop, step, dtype="int32")
             return PopulationView(self, rk_range, geometry=(len(rk_range),))
 
         elif isinstance(indices, tuple): # a tuple
             slices = False
             for idx in indices: # check if there are slices in the coordinates
                 if isinstance(idx, slice): # there is at least one
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/PopulationView.py` & `ANNarchy-4.7.3/ANNarchy/core/PopulationView.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-#===============================================================================
-#
-#     PopulationView
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global as Global
 from .Random import RandomDistribution
 import numpy as np
 
-class PopulationView(object):
+class PopulationView :
     """ Container representing a subset of neurons of a Population."""
 
     def __init__(self, population, ranks, geometry=None):
         """
         Create a view of a subset of neurons within the same population.
 
         :param population: population object
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Profiler.py` & `ANNarchy-4.7.3/ANNarchy/core/Profiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,19 @@
-#===============================================================================
-#
-#     Profiler.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018 Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import time
 import csv
 import matplotlib.pylab as plt
 
 import ANNarchy.core.Global as Global
 
-class Profiler(object):
+class Profiler :
     """
     The Profiler module should help to understand the performance of a simulation
     using the ANNarchy neural simulator.
 
     Therefore are functions to investigate memory consumption and timeline
     information provided.
     """
@@ -151,15 +134,34 @@
 
                 # non-defined function
                 if t_start == 0.0:
                     continue
 
                 # CPP functions
                 if group == "cpp core":
-                    csv_writer.writerow( (label, t_start,) )
+                    csv_writer.writerow( (label, t_start, t_end, ) )
+
+    def get_cpp_times(self):
+        """
+        Returns a dicitionary with all measured cpp-timings.
+        """
+        measurement = {}
+        for t_start, t_end, label, group in self._entries:
+            # skip Python functions
+            if group != "cpp core":
+                continue
+
+            # non-defined function
+            if t_start == 0.0:
+                continue
+
+            # CPP functions
+            if group == "cpp core":
+                measurement[label] = t_end
+        return measurement
 
     def show_timeline(self, store_graph=False):
         """
         Visualize the timeline.
         """
         f, ax = plt.subplots()
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Projection.py` & `ANNarchy-4.7.3/ANNarchy/core/Projection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,24 @@
-#===============================================================================
-#
-#     Projection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import numpy as np
 import math, os
 import copy, inspect
 import pickle
 
 from ANNarchy.core import Global
 from ANNarchy.core.Random import RandomDistribution
 from ANNarchy.core.Dendrite import Dendrite
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.core import ConnectorMethods
 
-class Projection(object):
+class Projection :
     """
     Container for all the synapses of the same type between two populations.
     """
 
     def __init__(self, pre, post, target, synapse=None, name=None, disable_omp=True, copied=False):
         """
         By default, the synapse only ensures linear synaptic transmission:
@@ -121,14 +103,15 @@
             self.name = 'proj'+str(self.id)
 
         # Container for control/attribute states
         self.init = {}
 
         # Control-flow variables
         self.init["transmission"] = True
+        self.init["axon_transmission"] = True
         self.init["update"] = True
         self.init["plasticity"] = True
 
         # Get a list of parameters and variables
         self.parameters = []
         for param in self.synapse_type.description['parameters']:
             self.parameters.append(param['name'])
@@ -262,14 +245,18 @@
         copied_proj.connector_name = self.connector_name
 
         # Control flags for code generation (maybe modified by connect_XXX())
         copied_proj._storage_format = self._storage_format
         copied_proj._storage_order = self._storage_order
         copied_proj._no_split_matrix = self._no_split_matrix
 
+        # Specific for OpenMP
+        copied_proj._parallel_pattern = self._parallel_pattern
+        copied_proj._no_split_matrix = self._no_split_matrix
+
         # for some projection types saving is not allowed (e. g. Convolution, Pooling)
         copied_proj._saveable = self._saveable
 
         # optional flags
         if hasattr(self, "_bsr_size"):
             copied_proj._bsr_size = self._bsr_size
 
@@ -336,16 +323,40 @@
             # No default connector -> initialize from LIL
             if self._lil_connectivity:
                 return self.cyInstance.init_from_lil_connectivity(self._lil_connectivity)
             else:
                 return self.cyInstance.init_from_lil_connectivity(self._connection_method(*((self.pre, self.post,) + self._connection_args)))
 
         else:
+            if Global.config["verbose"]:
+                print("Use CPP-side implementation of", self.connector_name,"pattern for ProjStruct"+str(self.id))
+
+            # all-to-all pattern
+            if self.connector_name == "All-to-All":
+                if isinstance(self._connection_args[0], RandomDistribution):
+                    #some kind of distribution
+                    w_dist_arg1, w_dist_arg2 = self._connection_args[0].get_cpp_args()
+                else:
+                    # constant
+                    w_dist_arg1 = self._connection_args[0]
+                    w_dist_arg2 = self._connection_args[0]
+
+                if isinstance(self._connection_args[1], RandomDistribution):
+                    #some kind of distribution
+                    d_dist_arg1, d_dist_arg2 = self._connection_args[1].get_cpp_args()
+                else:
+                    # constant
+                    d_dist_arg1 = self._connection_args[1]
+                    d_dist_arg2 = self._connection_args[1]
+                allow_self_connections = self._connection_args[2]
+
+                return self.cyInstance.all_to_all(self.post.ranks, self.pre.ranks, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections)
+
             # fixed probability pattern
-            if self.connector_name == "Random":
+            elif self.connector_name == "Random":
                 p = self._connection_args[0]
                 allow_self_connections = self._connection_args[3]
                 if isinstance(self._connection_args[1], RandomDistribution):
                     #some kind of distribution
                     w_dist_arg1, w_dist_arg2 = self._connection_args[1].get_cpp_args()
                 else:
                     # constant
@@ -403,14 +414,18 @@
                     storage_format = "csr"
                 else:
                     raise NotImplementedError
 
             else:
                 storage_format = Global.config["sparse_matrix_format"]
 
+        # No storage order specified for this projection by the user, so fall-back to Global setting
+        if storage_order is None:
+            storage_order = Global.config["sparse_matrix_storage_order"]
+
         # Sanity checks
         if self._connection_method != None:
             Global._warning("Projection ", self.name, " was already connected ... data will be overwritten.")
 
         # Store connectivity pattern parameters
         self._connection_method = method
         self._connection_args = args
@@ -496,18 +511,15 @@
             if self.synapse_type.type == "spike":
                 # we need to build up the matrix to analyze
                 self._lil_connectivity = self._connection_method(*((self.pre, self.post,) + self._connection_args))
 
                 # get the decision parameter
                 density = float(self._lil_connectivity.nb_synapses) / float(self.pre.size * self.post.size)
                 if density >= 0.6:
-                    if Global._check_paradigm("cuda"):
-                        storage_format = "csr"  # HD (11th Nov. 2022): there is no Dense_T for spiking and CUDA yet
-                    else:
-                        storage_format = "dense"
+                    storage_format = "dense"
                 else:
                     storage_format = "csr"
 
             else:
                 # we need to build up the matrix to analyze
                 self._lil_connectivity = self._connection_method(*((self.pre, self.post,) + self._connection_args))
 
@@ -534,23 +546,19 @@
         """
         Contrary to the matrix format, the decision for the matrix order is majorly dependent on
         the synapse type.
         """
         if self.synapse_type.type == "rate":
             storage_order = "post_to_pre"
         else:
-            if Global._check_paradigm("cuda"):
-                # HD (11th Nov. 2022): there is no Dense_T / CSRC_T for spiking and CUDA yet
-                storage_order = "post_to_pre"
+            # pre-to-post is not implemented for all formats
+            if self._storage_format in ["dense", "csr"]:
+                storage_order = "pre_to_post"
             else:
-                # pre-to-post is not implemented for all formats
-                if self._storage_format in ["dense", "csr"]:
-                    storage_order = "pre_to_post"
-                else:
-                    storage_order = "post_to_pre"
+                storage_order = "post_to_pre"
 
         Global._info("Automatic matrix order selection for", self.name, ":", storage_order)
         return storage_order
 
     def _has_single_weight(self):
         "If a single weight should be generated instead of a LIL"
         is_cpu = Global.config['paradigm']=="openmp"
@@ -740,15 +748,15 @@
             self.__setattr__(name, val)
 
     def __getattr__(self, name):
         # Method called when accessing an attribute.
         if name == 'initialized' or not hasattr(self, 'initialized'): # Before the end of the constructor
             return object.__getattribute__(self, name)
         elif hasattr(self, 'attributes'):
-            if name in ['plasticity', 'transmission', 'update']:
+            if name in ['plasticity', 'axon_transmission', 'transmission', 'update']:
                 return self._get_flag(name)
             if name in ['delay']:
                 return self._get_delay()
             if name in self.attributes:
                 if not self.initialized:
                     return self.init[name]
                 else:
@@ -760,15 +768,15 @@
         return object.__getattribute__(self, name)
 
     def __setattr__(self, name, value):
         # Method called when setting an attribute.
         if name == 'initialized' or not hasattr(self, 'initialized'): # Before the end of the constructor
             object.__setattr__(self, name, value)
         elif hasattr(self, 'attributes'):
-            if name in ['plasticity', 'transmission', 'update']:
+            if name in ['plasticity', 'axon_transmission', 'transmission', 'update']:
                 self._set_flag(name, bool(value))
                 return
             if name in ['delay']:
                 self._set_delay(value)
                 return
             if name in self.attributes:
                 if not self.initialized:
@@ -822,15 +830,15 @@
 
         # A list is given
         if isinstance(value, list):
             if len(value) == len(self.post_ranks):
                 if attribute in self.synapse_type.description['local']:
                     for idx, n in enumerate(self.post_ranks):
                         if not len(value[idx]) == self.cyInstance.dendrite_size(idx):
-                            Global._error('The postynaptic neuron ' + str(n) + ' receives '+ str(self.cyInstance.dendrite_size(idx))+ ' synapses.')
+                            Global._error('The post-synaptic neuron ' + str(n) + ' of population ' + str(self.post.id) + ' receives '+ str(self.cyInstance.dendrite_size(idx))+ ' synapses and not ' + str(len(value[idx])) + '.')
                         self.cyInstance.set_local_attribute_row(attribute, idx, value[idx], ctype)
                 elif attribute in self.synapse_type.description['semiglobal']:
                     self.cyInstance.set_semiglobal_attribute_all(attribute, value, ctype)
                 else:
                     Global._error('The parameter', attribute, 'is global to the population, cannot assign a list.')
             else:
                 Global._error('The projection has', self.size, 'post-synaptic neurons, the list must have the same size.')
@@ -842,14 +850,15 @@
             elif attribute in self.synapse_type.description['local']:
                 for idx, n in enumerate(self.post_ranks):
                     self.cyInstance.set_local_attribute_row(attribute, idx, value.get_values(self.cyInstance.dendrite_size(idx)), ctype)
             elif attribute in self.synapse_type.description['semiglobal']:
                 self.cyInstance.set_semiglobal_attribute_all(attribute, value.get_values(len(self.post_ranks)), ctype)
             elif attribute in self.synapse_type.description['global']:
                 self.cyInstance.set_global_attribute(attribute, value.get_values(1), ctype)
+
         # A single value is given
         else:
             if attribute == "w" and self._has_single_weight():
                 self.cyInstance.set_global_attribute(attribute, value, ctype)
             elif attribute in self.synapse_type.description['local']:
                 for idx, n in enumerate(self.post_ranks):
                     self.cyInstance.set_local_attribute_row(attribute, idx, value*np.ones(self.cyInstance.dendrite_size(idx)), ctype)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Random.py` & `ANNarchy-4.7.3/ANNarchy/core/Random.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-#===============================================================================
-#
-#     Random.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import numpy as np
 from ANNarchy.core import Global
 
 distributions_arguments = {
     'Uniform' : 2,
     'DiscreteUniform': 2,
     'Normal' : 2,
     'LogNormal': 2,
     'Exponential': 1,
-    'Gamma': 2
+    'Gamma': 2,
+    'Binomial' : 2
 }
 
 distributions_equivalents = {
     'Uniform' : 'std::uniform_real_distribution< %(float_prec)s >',
     'DiscreteUniform': 'std::uniform_int_distribution<int>',
     'Normal' : 'std::normal_distribution< %(float_prec)s >',
     'LogNormal': 'std::lognormal_distribution< %(float_prec)s >',
     'Exponential': 'std::exponential_distribution< %(float_prec)s >',
-    'Gamma': 'std::gamma_distribution< %(float_prec)s >'
+    'Gamma': 'std::gamma_distribution< %(float_prec)s >',
+    'Binomial': 'std::binomial_distribution<int>'
 }
 
 # List of available distributions
 available_distributions = distributions_arguments.keys()
 
-class RandomDistribution(object):
+class RandomDistribution :
     """
     BaseClass for random distributions.
     """
 
     def get_values(self, shape):
         """
         Returns a np.ndarray with the given shape
@@ -260,7 +244,34 @@
             data[data<self.min] = self.min
         if self.max != None:
             data[data>self.max] = self.max
         return data
 
     def latex(self):
         return "$\\Gamma$(" + str(self.alpha) + ', ' + str(self.beta) + ')'
+        
+class Binomial(RandomDistribution):
+    """
+    Random distribution object using the binomial distribution with specified parameters, n trials and p probability of success where n an integer >= 0 and p is in the interval [0,1].
+
+    The returned values are number of successes over the n trials.
+    """
+
+    def __init__(self, n, p):
+        """
+        :param n: trials.
+        :param p: probability of success.
+        """
+        self.n = n
+        self.p = p
+
+    def get_values(self, shape):
+        """
+        Returns a Numpy array with the given shape.
+        """
+        return np.random.binomial(self.n, self.p, size=shape)
+
+    def latex(self):
+        return "$\\mathcal{B}$(" + str(self.n) + ", " + str(self.p) + ")"
+
+    def get_cpp_args(self):
+        return self.n, self.p
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Simulate.py` & `ANNarchy-4.7.3/ANNarchy/core/Simulate.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Simulate.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from .Global import _network
 from .Global import get_current_step, dt
 from .Global import _error, _print
 from math import ceil
 import ANNarchy.core.Global as Global
 import time
 import operator
@@ -58,15 +40,15 @@
     # Compute the number of steps
     nb_steps = ceil(float(duration) / dt())
 
     if measure_time:
         tstart = time.time()
 
     if callbacks and _callbacks_enabled[net_id] and len(_callbacks[net_id]) > 0:
-        _simulate_with_callbacks(duration, net_id)
+        _simulate_with_callbacks(duration, progress_bar, net_id)
     else:
         _network[net_id]['instance'].pyx_run(nb_steps, progress_bar)
 
     if measure_time:
         if net_id > 0:
             _print('Simulating', duration/1000.0, 'seconds of the network', net_id, 'took', time.time() - tstart, 'seconds.')
         else:
@@ -76,43 +58,43 @@
     # measures in ms and Python measures in s
     if Global._profiler:
         t1 = time.time()
         Global._profiler.add_entry( t0, t1, "simulate", "simulate")
 
         # network single step
         overall_avg, _ = Global._profiler._cpp_profiler.get_timing("network", "step")
-        Global._profiler.add_entry(overall_avg/1000.0, 100.0, "overall", "cpp core")
+        Global._profiler.add_entry(overall_avg * nb_steps, 100.0, "overall", "cpp core")
 
         # single operations for populations
         for pop in _network[net_id]['populations']:
             for func in ["step", "rng", "delay", "spike"]:
-                avg_time, std_time = Global._profiler._cpp_profiler.get_timing(pop.name, func)
-                Global._profiler.add_entry( avg_time/1000.0, (avg_time/overall_avg)*100.0, pop.name+"_"+func, "cpp core")
+                avg_time, _ = Global._profiler._cpp_profiler.get_timing(pop.name, func)
+                Global._profiler.add_entry( avg_time * nb_steps, (avg_time/overall_avg)*100.0, pop.name+"_"+func, "cpp core")
 
         # single operations for projections
         for proj in _network[net_id]['projections']:
             for func in ["psp", "step", "post_event"]:
-                avg_time, std_time = Global._profiler._cpp_profiler.get_timing(proj.name, func)
-                Global._profiler.add_entry( avg_time/1000.0, (avg_time/overall_avg)*100.0, proj.name+"_"+func, "cpp core")
+                avg_time, _ = Global._profiler._cpp_profiler.get_timing(proj.name, func)
+                Global._profiler.add_entry( avg_time * nb_steps, (avg_time/overall_avg)*100.0, proj.name+"_"+func, "cpp core")
 
         monitor_avg, _ = Global._profiler._cpp_profiler.get_timing("network", "record")
-        Global._profiler.add_entry( monitor_avg/1000.0, (monitor_avg/overall_avg)*100.0, "record", "cpp core")
+        Global._profiler.add_entry( monitor_avg * nb_steps, (monitor_avg/overall_avg)*100.0, "record", "cpp core")
 
 def simulate_until(max_duration, population, operator='and', measure_time = False, net_id=0):
     """
     Runs the network for the maximal duration in milliseconds. If the ``stop_condition`` defined in the population becomes true during the simulation, it is stopped.
 
     One can specify several populations. If the stop condition is true for any of the populations, the simulation will stop ('or' function).
 
     Example:
 
     ```python
     pop1 = Population( ..., stop_condition = "r > 1.0 : any")
     compile()
-    simulate_until(max_duration=1000.0. population=pop1)
+    simulate_until(max_duration=1000.0, population=pop1)
     ```
 
     :param max_duration: the maximum duration of the simulation in milliseconds.
     :param population: the (list of) population whose ``stop_condition`` should be checked to stop the simulation.
     :param operator: operator to be used ('and' or 'or') when multiple populations are provided (default: 'and').
     :param measure_time: defines whether the simulation time should be printed (default=False).
     :return: the actual duration of the simulation in milliseconds.
@@ -175,15 +157,15 @@
     Clears the list of declared callbacks for the network.
 
     Cannot be undone!
     """
     _callbacks[net_id].clear()
 
 
-class every(object):
+class every :
     """
     Decorator to declare a callback method that will be called periodically during the simulation.
 
     Example of setting increasing inputs to a population every 100 ms, with an offset of 90 ms (or -10 ms relative to the period):
 
     ```python
     @every(period=100., offset=-10.)
@@ -223,15 +205,15 @@
         # once, as part of the decoration process! You can only give
         # it a single argument, which is the function object.
         
         self.func = f
         return f
 
 
-def _simulate_with_callbacks(duration, net_id=0):
+def _simulate_with_callbacks(duration, progress_bar, net_id=0):
     """
     Replaces simulate() when call_backs are defined.
     """
     t_start = get_current_step(net_id)
     length = int(duration/dt())
 
     # Compute the times
@@ -249,14 +231,14 @@
 
     # Sort the times to be sure they are in the right order.
     times = sorted(times, key=operator.itemgetter(0))
 
     for time, callback, n in times:
         # Advance the simulation to the desired time
         if time != get_current_step(net_id):
-            _network[net_id]['instance'].pyx_run(time-get_current_step(net_id))
+            _network[net_id]['instance'].pyx_run(time-get_current_step(net_id), progress_bar)
         # Call the callback
         callback.func(n)
 
     # Go to the end of the duration
     if get_current_step(net_id) < t_start + length:
-        _network[net_id]['instance'].pyx_run(t_start + length - get_current_step(net_id))
+        _network[net_id]['instance'].pyx_run(t_start + length - get_current_step(net_id), progress_bar)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/SpecificPopulation.py` & `ANNarchy-4.7.3/ANNarchy/core/SpecificPopulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     SpecificPopulation.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Population import Population
 from ANNarchy.core.Neuron import Neuron
 import ANNarchy.core.Global as Global
 
 import numpy as np
 
 class SpecificPopulation(Population):
@@ -269,15 +251,15 @@
         """
         pass
 
 class TimedArray(SpecificPopulation):
     """
     Data structure holding sequential inputs for a rate-coded network.
 
-    The input values are stored in the (recordable) attribute `r`, without any further processing. 
+    The input values are stored in the (recordable) attribute `r`, without any further processing.
     You will need to connect this population to another one using the ``connect_one_to_one()`` method.
 
     By default, the firing rate of this population will iterate over the different values step by step:
 
     ```python
     inputs = np.array(
         [
@@ -339,50 +321,90 @@
     ```python
     simulate(100.) # ten inputs are shown with a schedule of 10 ms
     inp.reset()
     simulate(100.) # the same ten inputs are presented again.
     ```
 
     """
-    def __init__(self, rates, schedule=0., period= -1., name=None, copied=False):
+    def __init__(self, rates=None, geometry=None, schedule=0., period= -1., name=None, copied=False):
         """
         :param rates: array of firing rates. The first axis corresponds to time, the others to the desired dimensions of the population.
+        :param geometry: desired dimensions of the population. This argument will be considered if *rates* is None.
         :param schedule: either a single value or a list of time points where inputs should be set. Default: every timestep.
         :param period: time when the timed array will be reset and start again, allowing cycling over the inputs. Default: no cycling (-1.).
         """
         neuron = Neuron(
             parameters="",
             equations=" r = 0.0",
             name="Timed Array",
             description="Timed array source."
         )
+
+        # Sanity check
+        if rates is None and geometry is None:
+            Global._error("TimedArray: either *rates* or *geometry* argument must be set.")
+
         # Geometry of the population
-        geometry = rates.shape[1:]
+        if rates is not None:
+            if geometry is None:
+                geometry = rates.shape[1:]
+            else:
+                if geometry != rates.shape[1:]:
+                    Global._warning("TimedArray: mismatch between *rates* and *geometry* dimensions detected.")
+
+        SpecificPopulation.__init__(self, geometry=geometry, neuron=neuron, name=name, copied=copied)
+
+        self.init['schedule'] = schedule
+        self.init['rates'] = rates
+        self.init['period'] = period
+
+        if rates is not None:
+            self.update(rates=rates, period=period, schedule=schedule)
+
+    @property
+    def r(self):
+        if self.initialized:
+            return self._get_cython_attribute("r")
+        else:
+            Global._error("Read-out of 'r' is only possible after compile.")
+
+    @r.setter
+    def r(self, new_r):
+        Global._error("The value of r is defined through the '*'rates' argument.")
+
+    def update(self, rates, schedule=0., period=-1):
+        """
+        Set a new list of inputs. The first axis corresponds to time, the others to the desired dimensions of the population. Note, the
+        geometry is set during construction phase of the object.
+
+        :param rates: array of firing rates. The first axis corresponds to time, the others to the desired dimensions of the population.
+        :param schedule: either a single value or a list of time points where inputs should be set. Default: every timestep.
+        :param period: time when the timed array will be reset and start again, allowing cycling over the inputs. Default: no cycling (-1.).
+        """
+        self.rates = rates
+        self.period = period
 
         # Check the schedule
         if isinstance(schedule, (int, float)):
             if float(schedule) <= 0.0:
                 schedule = Global.config['dt']
-            schedule = [ float(schedule*i) for i in range(rates.shape[0])]
 
-        if len(schedule) > rates.shape[0]:
+            self.schedule = [ float(schedule*i) for i in range(rates.shape[0])]
+        else:
+            self.schedule = schedule
+
+        if len(self.schedule) > self.rates.shape[0]:
             Global._error('TimedArray: the length of the schedule parameter cannot exceed the first dimension of the rates parameter.')
 
-        if len(schedule) < rates.shape[0]:
+        if len(self.schedule) < self.rates.shape[0]:
             Global._warning('TimedArray: the length of the schedule parameter is smaller than the first dimension of the rates parameter (more data than time points). Make sure it is what you expect.')
 
-        SpecificPopulation.__init__(self, geometry=geometry, neuron=neuron, name=name, copied=copied)
-
-        self.init['schedule'] = schedule
-        self.init['rates'] = rates
-        self.init['period'] = period
-
     def _copy(self):
         "Returns a copy of the population when creating networks."
-        return TimedArray(self.init['rates'] , self.init['schedule'], self.init['period'], self.name, copied=True)
+        return TimedArray(rates=self.rates, geometry=self.geometry, schedule=self.schedule, period=self.period, name=self.name, copied=True)
 
     def _generate_st(self):
         """
         adjust code templates for the specific population for single thread and openMP.
         """
         self._specific_template['declare_additional'] = """
     // Custom local parameters of a TimedArray
@@ -392,15 +414,15 @@
     long int _t; // Internal time
     int _block; // Internal block when inputs are set not at each step
 """ % {'float_prec': Global.config['precision']}
         self._specific_template['access_additional'] = """
     // Custom local parameters of a TimedArray
     void set_schedule(std::vector<int> schedule) { _schedule = schedule; }
     std::vector<int> get_schedule() { return _schedule; }
-    void set_buffer(std::vector< std::vector< %(float_prec)s > > buffer) { _buffer = buffer; r = _buffer[0]; }
+    void set_buffer(std::vector< std::vector< %(float_prec)s > > buffer) { _buffer = buffer; r = _buffer[_block]; }
     std::vector< std::vector< %(float_prec)s > > get_buffer() { return _buffer; }
     void set_period(int period) { _period = period; }
     int get_period() { return _period; }
 """ % {'float_prec': Global.config['precision']}
         self._specific_template['init_additional'] = """
         // Initialize counters
         _t = 0;
@@ -440,16 +462,18 @@
     cpdef set_period( self, period ):
         pop%(id)s.set_period(period)
     cpdef int get_period(self):
         return pop%(id)s.get_period()
 """ % { 'id': self.id }
 
         self._specific_template['update_variables'] = """
-        if(_active){
-            //std::cout << _t << " " << _block<< " " << _schedule[_block] << std::endl;
+        if(_active) {
+        #ifdef _DEBUG
+            std::cout << "TimedArray::update() - " << _t << " " << _block<< " " << _schedule[_block] << std::endl;
+        #endif
 
             // Check if it is time to set the input
             if(_t == _schedule[_block]){
                 // Set the data
                 r = _buffer[_block];
                 // Move to the next block
                 _block++;
@@ -464,17 +488,21 @@
                 // Reset the counters
                 _block=0;
                 _t = -1;
             }
 
             // Always increment the internal time
             _t++;
+
+        #ifdef _DEBUG
+            std::cout << "TimedArray::update(t="<< t <<") - current buffer (min/max) = [" << *std::min_element(r.begin(), r.end()) << "," << *std::max_element(r.begin(), r.end()) <<  "]" << std::endl;
+        #endif
         }
 """
-        
+
         self._specific_template['size_in_bytes'] = """
         // schedule
         size_in_bytes += _schedule.capacity() * sizeof(int);
 
         // buffer
         size_in_bytes += _buffer.capacity() * sizeof(std::vector<%(float_prec)s>);
         for( auto it = _buffer.begin(); it != _buffer.end(); it++ )
@@ -493,15 +521,15 @@
     long int _t; // Internal time
     int _block; // Internal block when inputs are set not at each step
 """ % {'float_prec': Global.config['precision']}
         self._specific_template['access_additional'] = """
     // Custom local parameters of a TimedArray
     void set_schedule(std::vector<int> schedule) { _schedule = schedule; }
     std::vector<int> get_schedule() { return _schedule; }
-    void set_buffer(std::vector< std::vector< %(float_prec)s > > buffer) { _buffer = buffer; r = _buffer[0]; }
+    void set_buffer(std::vector< std::vector< %(float_prec)s > > buffer) { _buffer = buffer; r = _buffer[_block]; }
     std::vector< std::vector< %(float_prec)s > > get_buffer() { return _buffer; }
     void set_period(int period) { _period = period; }
     int get_period() { return _period; }
 """ % {'float_prec': Global.config['precision']}
         self._specific_template['init_additional'] = """
         // Initialize counters
         _t = 0;
@@ -544,14 +572,18 @@
         return pop%(id)s.get_period()
 """ % { 'id': self.id }
 
         self._specific_template['update_variables'] = """
         if(_active){
             #pragma omp single
             {
+            #ifdef _DEBUG
+                std::cout << "TimedArray::update() - " << _t << " " << _block<< " " << _schedule[_block] << std::endl;
+            #endif
+
                 // Check if it is time to set the input
                 if(_t == _schedule[_block]){
                     // Set the data
                     r = _buffer[_block];
                     // Move to the next block
                     _block++;
                     // If was the last block, go back to the first block
@@ -568,15 +600,15 @@
                 }
 
                 // Always increment the internal time
                 _t++;
             }
         }
 """
-        
+
         self._specific_template['size_in_bytes'] = """
         // schedule
         size_in_bytes += _schedule.capacity() * sizeof(int);
 
         // buffer
         size_in_bytes += _buffer.capacity() * sizeof(std::vector<%(float_prec)s>);
         for( auto it = _buffer.begin(); it != _buffer.end(); it++ )
@@ -620,15 +652,15 @@
 
         auto host_it = buffer.begin();
         auto dev_it = gpu_buffer.begin();
         for (; host_it < buffer.end(); host_it++, dev_it++) {
             cudaMemcpy( *dev_it, host_it->data(), host_it->size()*sizeof(%(float_prec)s), cudaMemcpyHostToDevice);
         }
 
-        gpu_r = gpu_buffer[0];
+        gpu_r = gpu_buffer[_block];
     }
     std::vector< std::vector< %(float_prec)s > > get_buffer() {
         std::vector< std::vector< %(float_prec)s > > buffer = std::vector< std::vector< %(float_prec)s > >( gpu_buffer.size(), std::vector<%(float_prec)s>(size,0.0) );
 
         auto host_it = buffer.begin();
         auto dev_it = gpu_buffer.begin();
         for (; host_it < buffer.end(); host_it++, dev_it++) {
@@ -660,32 +692,40 @@
         vector[vector[%(float_prec)s]] get_buffer()
         void set_period(int)
         int get_period()
 """ % {'float_prec': Global.config['precision']}
         self._specific_template['wrapper_access_additional'] = """
     # Custom local parameters timed array
     cpdef set_schedule( self, schedule ):
-        pop%(id)s.set_schedule( schedule )
+        pop%(id)s.set_schedule( np.array(schedule, dtype=int) )
     cpdef np.ndarray get_schedule( self ):
         return np.array(pop%(id)s.get_schedule( ))
 
     cpdef set_rates( self, buffer ):
         pop%(id)s.set_buffer( buffer )
     cpdef np.ndarray get_rates( self ):
         return np.array(pop%(id)s.get_buffer( ))
 
     cpdef set_period( self, period ):
         pop%(id)s.set_period(period)
     cpdef int get_periodic(self):
         return pop%(id)s.get_period()
 """ % { 'id': self.id, 'float_prec': Global.config['precision'] }
 
+        # there is no GPU-side computation
+        self._specific_template['update_variable_body'] = ""
+        self._specific_template['update_variable_invoke'] = ""
+        self._specific_template['update_variable_header'] = ""
+
+        # we switch the GPU buffer which is read out in each time step
         self._specific_template['update_variables'] = """
         if(_active) {
-            // std::cout << _t << " " << _block<< " " << _schedule[_block] << std::endl;
+        #ifdef _DEBUG
+            std::cout << "TimedArray::update() - " << _t << " " << _block<< " " << _schedule[_block] << std::endl;
+        #endif
             // Check if it is time to set the input
             if(_t == _schedule[_block]){
                 // Set the data
                 gpu_r = gpu_buffer[_block];
                 // Move to the next block
                 _block++;
                 // If was the last block, go back to the first block
@@ -701,37 +741,54 @@
                 _t = -1;
             }
 
             // Always increment the internal time
             _t++;
         }
 """
-
-        self._specific_template['update_variable_body'] = ""
-        self._specific_template['update_variable_header'] = ""
+        # call the switch of CPU-buffers (host-side)
         self._specific_template['update_variable_call'] = """
     // host side update of neurons
     pop%(id)s.update();
 """ % {'id': self.id}
 
-        self._specific_template['size_in_bytes'] = "//TODO: "
+        self._specific_template['size_in_bytes'] = """
+        // r
+        size_in_bytes += sizeof(std::vector<%(float_prec)s>);
+        size_in_bytes += r.capacity() * sizeof(%(float_prec)s);
+
+        // schedule
+        size_in_bytes += sizeof(std::vector<int>);
+        size_in_bytes += _schedule.capacity() * sizeof(int);
+
+        // gpu_buffer
+        size_in_bytes += sizeof(std::vector<%(float_prec)s*>);
+        size_in_bytes += gpu_buffer.capacity() * sizeof(%(float_prec)s*);
+""" % {'float_prec': Global.config["precision"]}
 
     def _instantiate(self, module):
         # Create the Cython instance
         self.cyInstance = getattr(module, self.class_name+'_wrapper')(self.size, self.max_delay)
 
     def __setattr__(self, name, value):
         if name == 'schedule':
             if self.initialized:
-                self.cyInstance.set_schedule( np.array(value) / Global.config['dt'] )
+                val_int = np.array((np.atleast_1d(value) / Global.config['dt']), dtype=np.int32)
+                self.cyInstance.set_schedule( val_int )
             else:
                 self.init['schedule'] = value
         elif name == 'rates':
             if self.initialized:
+                if value is None:
+                    return # nothing to do
+
                 if len(value.shape) > 2:
+                    if value.shape[1:] != self.geometry:
+                        Global._error("TimedArray: mismatch between *rates* argument (", value.shape[1:], ") and stored geometry (", self.geometry, ").")
+
                     # we need to flatten the provided data
                     flat_values = value.reshape( (value.shape[0], self.size) )
                     self.cyInstance.set_rates( flat_values )
                 else:
                     self.cyInstance.set_rates( value )
             else:
                 self.init['rates'] = value
@@ -1005,21 +1062,30 @@
 
             // Transfer generated spikes to GPU
             if( spike_count > 0 ) {
                 cudaMemcpy( gpu_spiked, spiked.data(), spike_count * sizeof(int), cudaMemcpyHostToDevice);
             }
         }
         """
+
+        # overwrite default code generation for neural update
         self._specific_template['update_variable_body'] = ""
+        self._specific_template['update_variable_invoke'] = ""
         self._specific_template['update_variable_header'] = ""
         self._specific_template['update_variable_call'] = """
     // host side update of neurons
     pop%(id)s.update();
 """ % {'id': self.id}
 
+        # overwrite default code generation for spike gather
+        self._specific_template['spike_gather_body'] = ""
+        self._specific_template['spike_gather_invoke'] = ""
+        self._specific_template['spike_gather_header'] = ""
+        self._specific_template['spike_gather_call'] = ""
+
     def _instantiate(self, module):
         # Create the Cython instance
         self.cyInstance = getattr(module, self.class_name+'_wrapper')(self.size, self.init['spike_times'], self.max_delay)
 
     def __setattr__(self, name, value):
         if name == 'spike_times':
             if not isinstance(value[0], list): # several neurons
@@ -1595,15 +1661,15 @@
     def _instantiate(self, module):
         # Create the Cython instance
         self.cyInstance = getattr(module, self.class_name+'_wrapper')(self.size, self.max_delay)
 
     def __setattr__(self, name, value):
         if name == 'schedule':
             if self.initialized:
-                self.cyInstance.set_schedule( np.array(value) / Global.config['dt'] )
+                self.cyInstance.set_schedule( value / Global.config['dt'] )
             else:
                 self.init['schedule'] = value
         elif name == 'rates':
             if self.initialized:
                 value = np.array(value)
                 if value.shape[0] != self.schedule.shape[0]:
                     Global._error("TimedPoissonPopulation: the first dimension of rates must match the schedule.")
@@ -2512,8 +2578,8 @@
         return (mur, sigmar)
     x0 = mur / sigmar
     ratio = lambda u, v:u / v
     f = lambda x:ratio(*_rectified_gaussian(x, 1.)) - x0
     y = newton(f, x0 * 1.1) # Secant method
     new_sigma = mur / (np.exp(-0.5 * y ** 2) / ((2. * np.pi) ** .5) + .5 * y * (1. + erf(y * (2 ** (-.5)))))
     new_mu = y * new_sigma
-    return (new_mu, new_sigma)
+    return (new_mu, new_sigma)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/SpecificProjection.py` & `ANNarchy-4.7.3/ANNarchy/core/SpecificProjection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     SpecificProjection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Projection import Projection
 from ANNarchy.core.PopulationView import PopulationView
 
 import ANNarchy.core.Global as Global
 
 class SpecificProjection(Projection):
     """
@@ -165,15 +147,15 @@
             rates_history.push_front(rates);
             rates_history.pop_back();
             for(int i=0; i<post_rank.size(); i++){
                 sum = 0.0;
                 for(int step=0; step<window; step++){
                     sum += rates_history[step][post_rank[i]];
                 }
-                pop%(id_post)s._sum_%(target)s[post_rank[i]] += sum /float(window) * 1000. / dt / float(pre_rank[i].size());
+                pop%(id_post)s._sum_%(target)s[post_rank[i]] += sum / %(float_prec)s(window) * 1000. / dt / %(float_prec)s(pre_rank[i].size());
             }
         } // active
 """ % { 'id_proj': self.id, 'id_pre': self.pre.id, 'id_post': self.post.id, 'target': self.target,
         'post_size': self.post.size, 'float_prec': Global.config['precision'],
         'weight': "w" if self._has_single_weight() else "w[i][j]"}
 
         self._specific_template['psp_prefix'] = """
@@ -218,15 +200,15 @@
                 rates_history.push_front(rates);
                 rates_history.pop_back();
                 for(int i=0; i<post_rank.size(); i++){
                     sum = 0.0;
                     for(int step=0; step<window; step++){
                         sum += rates_history[step][post_rank[i]];
                     }
-                    pop%(id_post)s._sum_%(target)s[post_rank[i]] += sum /float(window) * 1000. / dt / float(pre_rank[i].size());
+                    pop%(id_post)s._sum_%(target)s[post_rank[i]] += sum / %(float_prec)s(window) * 1000. / dt / %(float_prec)s(pre_rank[i].size());
                 }
             } // active
         }
 """ % { 'id_proj': self.id, 'id_pre': self.pre.id, 'id_post': self.post.id, 'target': self.target,
         'post_size': self.post.size, 'float_prec': Global.config['precision'],
         'weight': "w" if self._has_single_weight() else "w[i][j]"}
 
@@ -338,17 +320,24 @@
     while (n < post_size) {
         g_%(target)s[n] += pre_r[n];
 
         n += blockDim.x;
     }
 }
 """ % ids
-        self._specific_template['psp_header'] = """__global__ void cu_proj%(id_proj)s_psp(int post_size, %(float_prec)s *pre_r, %(float_prec)s *g_%(target)s);""" % ids
+        self._specific_template['psp_invoke'] = """
+void proj%(id_proj)s_psp(RunConfig cfg, int post_size, %(float_prec)s *pre_r, %(float_prec)s *g_%(target)s) {
+    cu_proj%(id_proj)s_psp<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(post_size, pre_r, g_%(target)s);
+}
+""" % ids
+        self._specific_template['psp_header'] = """void proj%(id_proj)s_psp(RunConfig cfg, int post_size, %(float_prec)s *pre_r, %(float_prec)s *g_%(target)s);""" % ids
         self._specific_template['psp_call'] = """
-    cu_proj%(id_proj)s_psp<<< 1, 192 >>>(
+    proj%(id_proj)s_psp(
+        RunConfig(1, 192, 0, proj%(id_proj)s.stream),
         pop%(id_post)s.size,
         pop%(id_pre)s.gpu_r,
-        pop%(id_post)s.gpu_g_%(target)s );
+        pop%(id_post)s.gpu_g_%(target)s
+    );
 """ % ids
 
     def connect_current(self):
         return self.connect_one_to_one(weights=1.0)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Synapse.py` & `ANNarchy-4.7.3/ANNarchy/core/Synapse.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-#===============================================================================
-#
-#     Synapse.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 from ANNarchy.parser.AnalyseSynapse import analyse_synapse
 
-class Synapse(object):
+class Synapse :
     """
     Base class to define a synapse.
     """
     # Default name and description for reporting
     _default_names = {'rate': "Rate-coded synapse", 'spike': "Spiking synapse"}
 
     def __init__(self, parameters="", equations="", psp=None, operation='sum', pre_spike=None, post_spike=None, pre_axon_spike=None, functions=None, pruning=None, creating=None, name=None, description=None, extra_values={} ):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/Utils.py` & `ANNarchy-4.7.3/ANNarchy/core/Utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,55 +1,70 @@
-#===============================================================================
-#
-#     Utils.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import numpy as np
 import ANNarchy.core.Global as Global
+from ANNarchy.core.Random import RandomDistribution
 
 ######################
 # Sparse matrices
 ######################
 
-def sparse_random_matrix(pre, post, p, weight, delay=0):
+def sparse_random_matrix(pre, post, p, weight):
     """
-    Returns a sparse (lil) matrix to connect the pre and post populations with the probability p and the value weight.
+    Returns a sparse (lil) matrix to connect the pre and post populations with the
+    probability *p* and the value *weight*, either a constant or an ANNarchy random
+    distribution object.
     """
     try:
         from scipy.sparse import lil_matrix
     except:
         Global._warning("scipy is not installed, sparse matrices won't work")
         return None
     from random import sample
     W=lil_matrix((pre, post))
     for i in range(pre):
         k=np.random.binomial(post,p,1)[0]
-        W.rows[i]=sample(range(post),k)
-        W.data[i]=[weight]*k
+        tmp = sample(range(post),k)
+        W.rows[i]=list(np.sort(tmp))
+        if isinstance(weight, (int, float)):
+            W.data[i]=[weight]*k
+        elif isinstance(weight, RandomDistribution):
+            W.data[i]=weight.get_list_values(k)
+        else:
+            raise ValueError("sparse_random_matrix expects either a float or RandomDistribution object.")
 
     return W
 
+def sparse_delays_from_weights(weight_matrix, delay):
+    """
+    Generates a delay matrix corresponding to the connectivity stored *weight_matrix*.
+    """
+    try:
+        from scipy.sparse import lil_matrix
+    except:
+        Global._warning("scipy is not installed, sparse matrices won't work")
+        return None
+
+    delay_matrix = lil_matrix(weight_matrix.get_shape())
+
+    (rows,cols) = weight_matrix.nonzero()
+
+    for r, c in zip(rows, cols):
+        if isinstance(delay, (int, float)):
+            delay_matrix[r,c] = delay
+        elif isinstance(delay, RandomDistribution):
+            delay_matrix[r,c] = delay.get_value()
+        else:
+            raise ValueError("sparse_random_matrix expects either a float or RandomDistribution object.")
+
+    return delay_matrix
+
 ################################
 ## Performance Measurment
 ################################
 
 def compute_delivered_spikes(proj, spike_events):
     """
     This function counts the number of delivered spikes for a given Projection and
@@ -60,15 +75,15 @@
     * proj:             the Projection
     * spike_events:     the spike events per time step (the result of a spike recording)
     """
     nb_efferent_synapses = proj.nb_efferent_synapses()
     delivered_events = 0
 
     for neur_rank, time_steps in spike_events.items():
-        if neur_rank in proj.pre.ranks:
+        if neur_rank in proj.pre.ranks and neur_rank in nb_efferent_synapses.keys():
             delivered_events += nb_efferent_synapses[neur_rank] * len(time_steps)
 
     return delivered_events
 
 def compute_delivered_spikes_per_second(proj, spike_events, time_in_seconds, scale_factor=(10**6)):
     """
     This function implements a throughput metric for spiking neural networks.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Connector.pxd` & `ANNarchy-4.7.3/ANNarchy/core/cython_ext/Connector.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Connector.pyx` & `ANNarchy-4.7.3/ANNarchy/core/cython_ext/Connector.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Coordinates.pxd` & `ANNarchy-4.7.3/ANNarchy/core/cython_ext/Coordinates.pxd`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Coordinates.pyx` & `ANNarchy-4.7.3/ANNarchy/core/cython_ext/Coordinates.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/core/cython_ext/Transformations.pyx` & `ANNarchy-4.7.3/ANNarchy/core/cython_ext/Transformations.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/bold/AccProjection.py` & `ANNarchy-4.7.3/ANNarchy/extensions/bold/AccProjection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     AccProjection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Oliver Maith <oli_maith@gmx.de>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.core import Global
 
 class AccProjection(SpecificProjection):
     """
     Accumulates the values of a given variable.
     """
@@ -111,15 +93,28 @@
             self._specific_template['init_additional'] = """
         time_for_init_baseline = -1;
         init_baseline_period=1;
         baseline = std::vector<std::vector<%(float_prec)s>>(post_rank.size(), std::vector<%(float_prec)s>() );
         baseline_mean = std::vector<%(float_prec)s>(post_rank.size(), 0);
         baseline_std = std::vector<%(float_prec)s>(post_rank.size(), 1);
 """ % {'float_prec': Global.config['precision']}
+            self._specific_template['clear_additional'] = """
+        for(auto it = baseline.begin(); it != baseline.end(); it++) {
+            it->clear();
+            it->shrink_to_fit();
+        }
+        baseline.clear();
+        baseline.shrink_to_fit();
+
+        baseline_mean.clear();
+        baseline_mean.shrink_to_fit();
 
+        baseline_std.clear();
+        baseline_std.shrink_to_fit();
+"""
             self._specific_template['psp_prefix'] = ""
             self._specific_template['psp_code'] = """
         bool compute_baseline = (t < time_for_init_baseline) ? true : false;
         bool compute_average = (t == time_for_init_baseline) ? true : false;
 
         for(int post_idx = 0; post_idx < post_rank.size(); post_idx++) {
             %(float_prec)s lsum = 0.0;
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/bold/BoldModel.py` & `ANNarchy-4.7.3/ANNarchy/extensions/bold/BoldModel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     BoldModel.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Oliver Maith <oli_maith@gmx.de>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Neuron import Neuron
 
 class BoldModel(Neuron):
     """
     Base class to define a BOLD model to be used in a BOLD monitor.
 
     A BOLD model is quite similar to a regular rate-coded neuron. It gets a weighted sum of inputs with a specific target (e.g. I_CBF) and compute a single output variable (called `BOLD` in the predefined models, but it could be anything).
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/bold/BoldMonitor.py` & `ANNarchy-4.7.3/ANNarchy/extensions/bold/BoldMonitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     BoldMonitor.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2021 Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Oliver Maith <oli_maith@gmx.de>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Population import Population
 from ANNarchy.core.Monitor import Monitor
 from ANNarchy.core import Global
 
 from .PredefinedModels import balloon_RN
 from .AccProjection import AccProjection
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/bold/NormProjection.py` & `ANNarchy-4.7.3/ANNarchy/extensions/bold/NormProjection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     NormProjection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2019  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Oliver Maith <oli_maith@gmx.de>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import numpy as np
 
 from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.core import Global
 
 class NormProjection(SpecificProjection):
     """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/bold/PredefinedModels.py` & `ANNarchy-4.7.3/ANNarchy/extensions/bold/PredefinedModels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     PredefinedModels.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Oliver Maith <oli_maith@gmx.de>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from .BoldModel import BoldModel
 
 #####################################################################
 ### Several balloon model variants following Stephan et al. (2007)
 ###
 ### C = classical coefficient (e. g. no epsilon influence on k_2)
 ### R = revised coefficient (e. g. epsilon influence on k_2)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Convolve.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/Convolve.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,27 @@
-# =============================================================================
-#
-#     Convolution.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2019  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from __future__ import print_function
 import numpy as np
 from copy import deepcopy
 
 from ANNarchy.core import Global
-from ANNarchy.core.Projection import Projection
+from ANNarchy.core.SpecificProjection import SpecificProjection
 
-from ANNarchy.generator.Utils import tabify
+from ANNarchy.generator.Utils import tabify, remove_trailing_spaces
 from .ConvolveTemplate import *
 from .Utils import SharedSynapse
 
 # Indices used for each dimension
 indices = ['i', 'j', 'k', 'l', 'm', 'n']
 
-class Convolution(Projection):
+class Convolution(SpecificProjection):
     """
     Performs a convolution of a weight kernel on the pre-synaptic population.
 
     Despite its name, the operation performed is actually a cross-correlation, as is usual in computer vision and convolutional neural networks:
 
     $$g(x) = \sum_{k=-n}^n h(k) \, f(x + k)$$
 
@@ -94,20 +76,16 @@
         """
         :param pre: pre-synaptic population (either its name or a ``Population`` object).
         :param post: post-synaptic population (either its name or a ``Population`` object).
         :param target: type of the connection
         :param psp: continuous influence of a single synapse on the post-synaptic neuron (default for rate-coded: ``w*pre.r``).
         :param operation: operation (sum, max, min, mean) performed by the kernel (default: sum).
         """
-        # Sanity check
-        #if not pre.neuron_type.type == 'rate':
-        #    Global._error('Convolution: only implemented for rate-coded populations.')
-
         # Create the description, but it will not be used for generation
-        Projection.__init__(
+        SpecificProjection.__init__(
             self,
             pre,
             post,
             target,
             synapse=SharedSynapse(psp=psp, operation=operation, name="Convolution operation", description="Convoluted kernel over the pre-synaptic population."),
             name=name,
             copied=copied
@@ -344,15 +322,15 @@
         Builds up dendrites either from list or dictionary. Called by instantiate().
         """
         if not self._connection_method:
             Global._error('Convolution: The projection between ' + self.pre.name + ' and ' + self.post.name + ' is declared but not connected.')
 
         # Create the Cython instance
         proj = getattr(module, 'proj'+str(self.id)+'_wrapper')
-        self.cyInstance = proj(self.weights, self.pre_coordinates)
+        self.cyInstance = proj(self.pre_coordinates, self.weights)
 
         # Set delays after instantiation
         if self.delays > 0.0:
             self.cyInstance.set_delay(self.delays/Global.config['dt'])
 
         return True
 
@@ -504,24 +482,27 @@
     def _generate(self):
         """
         Overrides default code generation. This function is called during the code generation procedure.
         """
         # Filter definition
         filter_definition, filter_pyx_definition = self._filter_definition()
 
+        # On CPUs we have a pre-load on the inner-most sub-vector
+        use_inner_line = Global._check_paradigm("openmp")
+
         # Convolve_code
         if not self.multiple:
-            convolve_code, sum_code = self._generate_convolve_code()
+            convolve_code, sum_code = self._generate_convolve_code(pre_load_inner_line=use_inner_line)
         else:
-            convolve_code, sum_code = self._generate_bank_code()
+            convolve_code, sum_code = self._generate_bank_code(pre_load_inner_line=use_inner_line)
 
         if Global._check_paradigm("openmp"):
             self._generate_omp(filter_definition, filter_pyx_definition, convolve_code, sum_code)
         elif Global._check_paradigm("cuda"):
-            raise Global.ANNarchyException("Convolution is not available on CUDA devices yet.", True)
+            self._generate_cuda(filter_definition, filter_pyx_definition, convolve_code, sum_code)
         else:
             raise NotImplementedError
 
     def _generate_omp(self, filter_definition, filter_pyx_definition, convolve_code, sum_code, kernel=True):
         """
         OpenMP code generation.
         """
@@ -529,61 +510,43 @@
         base_ids = {
             'id_proj': self.id,
             'size_post': self.post.size,
             'float_prec': Global.config['precision']
         }
 
         # Fill the basic definitions
-        conv_dict = deepcopy(convole_template_omp)
+        conv_dict = deepcopy(convolve_template_omp)
         for key, value in conv_dict.items():
             value = value % base_ids
             conv_dict[key] = value
         self._specific_template.update(conv_dict)
 
         # Kernel-based method: specify w with the correct dimension
         if kernel:
+            # The number of dimension influences the type
+            cpp_type_w = filter_definition.replace(' w;', '')
+            pyx_type_w = filter_pyx_definition.replace(' w', '')
+
+            # Fill the code templates
             self._specific_template['declare_parameters_variables'] = tabify(filter_definition.strip(), 1)
             self._specific_template['export_parameters_variables'] = ""
-            self._specific_template['access_parameters_variables'] = """
-    // Local parameter w
-    %(type_w)s get_w() { return w; }
-    void set_w(%(type_w)s value) { w = value; }
-""" % {'type_w': filter_definition.replace(' w;', '')}
-            self._specific_template['export_connectivity'] += """
-        # Local variable w
-        %(type_w)s get_w()
-        void set_w(%(type_w)s)
-""" % {'type_w': filter_pyx_definition.replace(' w', '')}
-            self._specific_template['wrapper_init_connectivity'] += """
-        proj%(id_proj)s.set_w(weights)
-""" % {'id_proj': self.id}
-
-            self._specific_template['wrapper_access_connectivity'] += """
-    # Local variable w
-    def get_w(self):
-        return proj%(id_proj)s.get_w()
-    def set_w(self, value):
-        proj%(id_proj)s.set_w( value )
-    def get_dendrite_w(self, int rank):
-        return proj%(id_proj)s.get_w()
-    def set_dendrite_w(self, int rank, value):
-        proj%(id_proj)s.set_w(value)
-    def get_synapse_w(self, int rank_post, int rank_pre):
-        return 0.0
-    def set_synapse_w(self, int rank_post, int rank_pre, %(float_prec)s value):
-        pass
-""" % {'id_proj': self.id, 'float_prec': Global.config['precision']}
+            self._specific_template['access_parameters_variables'] = conv_filter_template["openmp"]["access"] % {'type_w': cpp_type_w}
+            self._specific_template['export_connectivity'] += conv_filter_template["pyx_wrapper"]["export"] % {'type_w': pyx_type_w}
+            self._specific_template['wrapper_args'] += conv_filter_template["pyx_wrapper"]["args"]
+            self._specific_template['wrapper_init_connectivity'] += conv_filter_template["pyx_wrapper"]["init"] % {'id_proj': self.id}
+            self._specific_template['wrapper_access_connectivity'] += conv_filter_template["pyx_wrapper"]["access"] % {'id_proj': self.id, 'float_prec': Global.config['precision']}
 
         # Override the monitor to avoid recording the weights
         self._specific_template['monitor_class'] = ""
-
         self._specific_template['monitor_export'] = ""
-
         self._specific_template['monitor_wrapper'] = ""
 
+        # Clean-up
+        self._specific_template['clear_container'] = convolve_template_omp["clear"]
+
         # OMP code
         omp_code = ""
         if Global.config['num_threads'] > 1:
             omp_code = """
         #pragma omp for private(sum, rk_pre, coord) %(psp_schedule)s""" % {'psp_schedule': "" if not 'psp_schedule' in self._omp_config.keys() else self._omp_config['psp_schedule']}
 
         # HD ( 16.10.2015 ):
@@ -617,54 +580,171 @@
 
                 // store result
                 pop%(id_post)s.%(target)s[i] += """ + sum_code + """;
             } // for
         } // if
 """
 
+        # Finalize the processing code
         self._specific_template['psp_code'] = wsum % \
         {   'id_proj': self.id,
             'target': target_code,
             'id_pre': self.pre.id, 'name_pre': self.pre.name, 'size_pre': self.pre.size,
             'id_post': self.post.id, 'name_post': self.post.name, 'size_post': self.post.size,
             'omp_code': omp_code,
             'convolve_code': convolve_code
         }
 
-        self._specific_template['size_in_bytes'] = """
-        // post-ranks
-        size_in_bytes += sizeof(std::vector<int>);
-        size_in_bytes += post_rank.capacity() * sizeof(int);
-
-        // pre-coords
-        size_in_bytes += sizeof(std::vector<std::vector<int>>);
-        size_in_bytes += pre_coords.capacity() * sizeof(std::vector<int>);
-        for (auto it = pre_coords.begin(); it != pre_coords.end(); it++) {
-            size_in_bytes += it->capacity() * sizeof(int);
+    def _generate_cuda(self, filter_definition, filter_pyx_definition, convolve_code, sum_code, kernel=True):
+        """
+        CUDA code generation.
+        """
+        # Basic ids
+        base_ids = {
+            'id_proj': self.id,
+            'size_post': self.post.size,
+            'float_prec': Global.config['precision']
         }
 
-        // filter
-        // TODO:
-"""
-        self._specific_template['clear'] = """
-        // post-ranks
-        post_rank.clear();
-        post_rank.shrink_to_fit();
-
-        // pre-coords
-        for (auto it = pre_coords.begin(); it != pre_coords.end(); it++) {
-            it->clear();
-            it->shrink_to_fit();
+        # Fill the basic definitions
+        conv_dict = deepcopy(convolve_template_cuda)
+        for key, value in conv_dict.items():
+            value = value % base_ids
+            conv_dict[key] = value
+        self._specific_template.update(conv_dict)
+
+        # Kernel-based method: specify w with the correct dimension
+        if kernel:
+            # The number of dimension influences the type
+            cpp_type_w = filter_definition.replace(' w;', '')
+            pyx_type_w = filter_pyx_definition.replace(' w', '')
+
+            # Fill the code templates
+            self._specific_template['declare_parameters_variables'] = conv_filter_template["cuda"]["declare"] % {'cpu_side_filter': filter_definition.strip(), 'float_prec': Global.config["precision"]}
+            self._specific_template['export_parameters_variables'] = ""
+            self._specific_template['access_parameters_variables'] = conv_filter_template["cuda"]["access"] % {'type_w': cpp_type_w, 'id_proj': self.id}
+            self._specific_template['export_connectivity'] += conv_filter_template["pyx_wrapper"]["export"] % {'type_w': pyx_type_w}
+            self._specific_template['wrapper_args'] += conv_filter_template["pyx_wrapper"]["args"]
+            self._specific_template['wrapper_init_connectivity'] += conv_filter_template["pyx_wrapper"]["init"] % {'id_proj': self.id}
+            self._specific_template['wrapper_access_connectivity'] += conv_filter_template["pyx_wrapper"]["access"] % {'id_proj': self.id, 'float_prec': Global.config['precision']}
+
+            # Memory transfer of variables
+            dim_pre = self.dim_pre
+            if self.multiple:
+               dim_pre += 1
+            self._specific_template['host_device_transfer'] += conv_filter_template["cuda"]["host_device_transfer"] % {'ctype': Global.config["precision"], 'id_proj': self.id, 'pre_dim': dim_pre}
+
+            # Other fields
+            self._specific_template['size_in_bytes'] = ""
+
+        # Override the monitor to avoid recording the weights
+        self._specific_template['monitor_class'] = ""
+        self._specific_template['monitor_export'] = ""
+        self._specific_template['monitor_wrapper'] = ""
+
+        # Clean-up
+        self._specific_template['clear_container'] = convolve_template_cuda["clear"]
+
+        # Add pre-synaptic variables to argument list
+        pre_variables_header = ""
+        pre_variables_invoke = ""
+        pre_variables_call = ""
+        for pre_dep in self.synapse_type.description['dependencies']['pre']:
+            # HD (TODO): the type to float precision works for now, but one should
+            #            look up the type in the pre-synaptic neuron type...
+            pre_id_dict = {
+                'id_pre': self.pre.id,
+                'name': pre_dep,
+                'type': Global.config["precision"]
+            }
+            pre_variables_header += ", const %(type)s* __restrict__ pre_%(name)s" % pre_id_dict
+            pre_variables_invoke += ", pre_%(name)s" % pre_id_dict
+            pre_variables_call += ", pop%(id_pre)s.gpu_%(name)s" % pre_id_dict
+
+        # Finalize code templates
+        code_ids = {
+            'id_proj': self.id,
+            'target': self.target,
+            'id_post': self.post.id,
+            'pre_dim': self.dim_pre,
+            'convolve_code': convolve_code,
+            'float_prec': Global.config["precision"],
+            'pre_variables_header': pre_variables_header,
+            'pre_variables_invoke': pre_variables_invoke,
+            'pre_variables_call': pre_variables_call,
+            'pre_variable': "pre_%(name)s" % pre_id_dict,
+            'convolve_code': convolve_code
         }
-        pre_coords.clear();
-        pre_coords.shrink_to_fit();
 
-        // filter
-        // TODO:
-"""
+        # Finalize the processing code
+        if not self.multiple:
+            # Convolution
+            self._specific_template['psp_body'] = cuda_convolution_single_filter["body"] % code_ids
+            self._specific_template['psp_invoke'] = cuda_convolution_single_filter["invoke"] % code_ids
+            self._specific_template['psp_header'] = cuda_convolution_single_filter["header"] % code_ids
+            self._specific_template['psp_call'] = cuda_convolution_single_filter["call"] % code_ids
+
+        else:
+            num_elem_per_filter = 1
+            for i in self.weights.shape[1:]:
+                num_elem_per_filter *= i
+            code_ids.update({
+                'filter_dim': self.dim_kernel,
+                'num_elem_filter': num_elem_per_filter
+            })
+
+            # Bank of filters
+            if len(self.weights.shape)==3 and len(self.pre.geometry)==2:
+                code_ids.update({
+                    'post_size': self.post.size,
+                    'filter_dim_i': self.weights.shape[1],
+                    'filter_dim_j': self.weights.shape[2],
+                    'pre_offset_i': self._center_filter(self.weights.shape[1]),
+                    'pre_offset_j': self._center_filter(self.weights.shape[2]),
+                    'pre_border_i': self.pre.geometry[0]-1,
+                    'pre_border_j': self.pre.geometry[1]-1,
+                    'pre_dim_j': self.pre.geometry[1]
+                })
+                self._specific_template['psp_body'] = cuda_convolution_bank_of_filter_3d["body"] % code_ids
+                self._specific_template['psp_invoke'] = cuda_convolution_bank_of_filter_3d["invoke"] % code_ids
+                self._specific_template['psp_header'] = cuda_convolution_bank_of_filter_3d["header"] % code_ids
+                self._specific_template['psp_call'] = cuda_convolution_bank_of_filter_3d["call"] % code_ids
+
+            elif len(self.weights.shape)==4 and len(self.pre.geometry)==3:
+                code_ids.update({
+                    'post_size': self.post.size,
+                    'filter_dim_i': self.weights.shape[1],
+                    'filter_dim_j': self.weights.shape[2],
+                    'filter_dim_k': self.weights.shape[3],
+                    'pre_offset_i': self._center_filter(self.weights.shape[1]),
+                    'pre_offset_j': self._center_filter(self.weights.shape[2]),
+                    'pre_offset_k': self._center_filter(self.weights.shape[3]),
+                    'pre_border_i': self.pre.geometry[0]-1,
+                    'pre_border_j': self.pre.geometry[1]-1,
+                    'pre_border_k': self.pre.geometry[2]-1,
+                    'pre_dim_j': self.pre.geometry[1],
+                    'pre_dim_k': self.pre.geometry[2]
+                })
+                self._specific_template['psp_body'] = cuda_convolution_bank_of_filter_4d["body"] % code_ids
+                self._specific_template['psp_invoke'] = cuda_convolution_bank_of_filter_4d["invoke"] % code_ids
+                self._specific_template['psp_header'] = cuda_convolution_bank_of_filter_4d["header"] % code_ids
+                self._specific_template['psp_call'] = cuda_convolution_bank_of_filter_4d["call"] % code_ids
+
+            else:
+                self._specific_template['psp_body'] = cuda_convolution_bank_of_filter["body"] % code_ids
+                self._specific_template['psp_invoke'] = cuda_convolution_bank_of_filter["invoke"] % code_ids
+                self._specific_template['psp_header'] = cuda_convolution_bank_of_filter["header"] % code_ids
+                self._specific_template['psp_call'] = cuda_convolution_bank_of_filter["call"] % code_ids
+
+        # Post-neuron is a spike neuron (e.g., part of ANN-to-SNN conversion)
+        if self.post.neuron_type.type == "spike":
+            self._specific_template['psp_call'] = self._specific_template['psp_call'].replace("gpu__sum_"+self.target, "gpu_g_"+self.target)
+
+        # Remove trailing spaces
+        self._specific_template['psp_body'] = remove_trailing_spaces(self._specific_template['psp_body'])
 
     ################################
     ### Utilities
     ################################
     def _center_filter(self, i):
         return int(i/2) if i%2==1 else int(i/2)-1
 
@@ -689,29 +769,50 @@
             if txt == "" : # first coordinate is special
                 txt = indices[0] + "_" + name
             else:
                 txt = str(geometry[d]) + '*(' + txt + ') + ' + indices[d]  + '_' + name
 
         return txt
 
-    def _generate_convolve_code(self):
+    def _filter_coordinates_to_index(self, name, filter_dim):
+        dim = len(filter_dim)
+
+        txt = ""
+
+        for d in range(dim):
+            if txt == "" : # first coordinate is special
+                txt = indices[0] + "_" + name
+            else:
+                txt = str(filter_dim[d]) + '*(' + txt + ') + ' + indices[d]  + '_' + name
+
+        return txt
+
+    def _generate_convolve_code(self, pre_load_inner_line=True):
+        """
+        Generate the loop for the convolution case.
+
+        Parameters:
+
+        * pre_load_inner_line: for CPU-code it's useful to have a local variable for accessing the innermost sub-vector
+        """
 
         # Operation to be performed: sum, max, min, mean
         operation = self.synapse_type.operation
 
         # Main code
         code = tabify("sum = 0.0;\n", 3)
 
         # Generate for loops
         for dim in range(self.dim_kernel):
-            if dim == self.dim_kernel-1:
-                inner_idx = ""
-                for i in range(self.dim_kernel-1):
-                    inner_idx += "["+indices[i]+"_w]"
-                code += "auto inner_line = w"+inner_idx+".data();\n"
+            if pre_load_inner_line:
+                if dim == self.dim_kernel-1:
+                    inner_idx = ""
+                    for i in range(self.dim_kernel-1):
+                        inner_idx += "["+indices[i]+"_w]"
+                    code += "auto inner_line = w"+inner_idx+".data();\n"
 
             code += tabify("""
             for(int %(index)s_w = 0; %(index)s_w < %(size)s;%(index)s_w++) {
             """ % { 'index': indices[dim], 'size': self.weights.shape[dim]}, dim)
 
             # Compute indices
             if dim < self.dim_kernel:
@@ -762,46 +863,71 @@
                 'dim': self.dim_kernel
             }
             code += "int %(index)s_pre = coord[%(dim)s];" % id_dict
 
         # Compute pre-synaptic rank
         code += tabify("""
                 rk_pre = %(value)s;""" % {'value': self._coordinates_to_rank('pre', self.pre.geometry)}, dim)
+        if not pre_load_inner_line:
+            code += tabify("""
+                w_idx = %(value)s;""" % {'value': self._filter_coordinates_to_index('w', self.weights.shape)}, dim)
 
         # Compute the increment
         index = ""
         for dim in range(self.dim_kernel):
             index += '[' + indices[dim] + '_w]'
 
-        increment = self.synapse_type.description['psp']['cpp'] % {
+        # Indices etc. depends on the target platform
+        inc_dict = {
             'id_pre': self.pre.id,
             'id_post': self.post.id,
-            'local_index': index,
-            'global_index': '[i]',
-            'pre_index': '[rk_pre]',
-            'post_index': '[rk_post]',
-            'pre_prefix': 'pop'+str(self.pre.id)+'.',
-            'post_prefix': 'pop'+str(self.post.id)+'.'
         }
+        if Global._check_paradigm("openmp"):
+            inc_dict.update({
+                'global_index': '[i]',
+                'local_index': index,
+                'pre_index': '[rk_pre]',
+                'post_index': '[rk_post]',
+                'pre_prefix': 'pop'+str(self.pre.id)+'.',
+                'post_prefix': 'pop'+str(self.post.id)+'.'
+            })
+        elif Global._check_paradigm("cuda"):
+            inc_dict.update({
+                'global_index': '',
+                'local_index': '[w_idx]',
+                'pre_index': '[rk_pre]',
+                'post_index': '',
+                'pre_prefix': 'pre_',
+                'post_prefix': 'post_'
+            })
+        else:
+            raise NotImplementedError
+
+        # Fill the code template
+        increment = self.synapse_type.description['psp']['cpp'] % inc_dict
 
         # Delays
         if self.delays > Global.config['dt']:
             increment = increment.replace(
                 'pop%(id_pre)s.r[rk_pre]' % {'id_pre': self.pre.id},
                 'delayed_r[rk_pre]'
             )
 
         # Apply the operation
         if operation == "sum":
             if self.dim_kernel == 1:
                 code += tabify("""
                 sum += %(increment)s""" % {'increment': increment}, dim)
             else:
-                code += tabify("""
-                sum += %(increment)s""" % {'increment': increment.replace('w'+inner_idx, 'inner_line')}, dim)
+                if pre_load_inner_line:
+                    code += tabify("""
+                    sum += %(increment)s""" % {'increment': increment.replace('w'+inner_idx, 'inner_line')}, dim)
+                else:
+                    code += tabify("""
+                    sum += %(increment)s""" % {'increment': increment}, dim)
         elif operation == "max":
             code += tabify("""
                 %(float_prec)s _psp = %(increment)s
                 if(_psp > sum) sum = _psp;""" % {'increment': increment, 'float_prec': Global.config['precision']}, dim)
         elif operation == "min":
             code += tabify("""
                 %(float_prec)s _psp = %(increment)s
@@ -832,26 +958,42 @@
         if operation == "mean":
             sum_code = """sum/%(filter_size)s""" % {'filter_size': self.weights.size}
         else:
             sum_code = "sum"
 
         return impl_code, sum_code
 
-    def _generate_bank_code(self):
+    def _generate_bank_code(self, pre_load_inner_line=True):
+        """
+        Generate the loop for the bank of filters case.
+
+        Parameters:
+
+        * pre_load_inner_line: for CPU-code it's useful to have a local variable for accessing the innermost sub-vector
+        """
 
         # Operation to be performed: sum, max, min, mean
         operation = self.synapse_type.operation
 
         # Main code
         code = tabify("sum = 0.0;\n", 3)
 
         # Generate for loops
         for dim in range(self.dim_kernel-1):
+            if pre_load_inner_line:
+                if dim == self.dim_kernel-2:
+                    inner_idx = ""
+                    for i in range(self.dim_kernel-2):
+                        inner_idx += "["+indices[i]+"_w]"
+                    code += tabify("""
+                const %(float_prec)s* w_inner_line = w[coord[%(dim_pre)s]]%(inner_idx)s.data();
+    """ % {'float_prec': Global.config["precision"], 'inner_idx': inner_idx, 'dim_pre': self.dim_pre}, dim)
+
             code += tabify("""
-            for(int %(index)s_w = 0; %(index)s_w < %(size)s;%(index)s_w++) {
+            for (int %(index)s_w = 0; %(index)s_w < %(size)s;%(index)s_w++) {
             """ % { 'index': indices[dim], 'size': self.weights.shape[dim+1]}, dim)
 
             # Compute indices
             if dim < self.dim_kernel:
                 code += tabify(
                     """int %(index)s_pre = coord[%(dim)s] %(operator)s (%(index)s_w - %(center)s);""" %
                     {
@@ -891,29 +1033,57 @@
                 continue;
             }
             """ % { 'index': indices[dim], 'max_size': self.pre.geometry[dim] -1}, 1+dim)
 
         # Compute pre-synaptic rank
         code +=tabify("""
             rk_pre = %(value)s;""" % {'value': self._coordinates_to_rank('pre', self.pre.geometry)}, 1+dim)
+        if not pre_load_inner_line:
+            code += tabify("""
+                w_idx = %(value)s;""" % {'value': self._filter_coordinates_to_index('w', self.weights.shape[1:])}, dim)
 
         # Compute the increment
-        index = "[coord["+str(self.dim_pre)+"]]"
-        for dim in range(self.dim_kernel-1):
-            index += '[' + indices[dim] + '_w]'
+        if pre_load_inner_line:
+            index = "_inner_line["+indices[self.dim_kernel-2]+"_w]"
+        else:
+            index = "[coord["+str(self.dim_pre)+"]]"
+            for dim in range(self.dim_kernel-1):
+                index += '[' + indices[dim] + '_w]'
 
-        increment = self.synapse_type.description['psp']['cpp'] % {
+        # Indices etc. depend on target platform
+        inc_dict = {
             'id_pre': self.pre.id,
             'id_post': self.post.id,
-            'local_index': index,
-            'global_index': '[i]',
-            'pre_index': '[rk_pre]',
-            'post_index': '[rk_post]',
-            'pre_prefix': 'pop'+str(self.pre.id)+'.',
-            'post_prefix': 'pop'+str(self.post.id)+'.'}
+        }
+        if Global._check_paradigm("openmp"):
+            inc_dict.update({
+                'local_index': index,
+                'global_index': '[i]',
+                'pre_index': '[rk_pre]',
+                'post_index': '[rk_post]',
+                'pre_prefix': 'pop'+str(self.pre.id)+'.',
+                'post_prefix': 'pop'+str(self.post.id)+'.'
+            })
+        elif Global._check_paradigm("cuda"):
+            inc_dict.update({
+                'local_index': "[w_idx]",
+                'global_index': '[bIdx]',
+                'pre_index': '[rk_pre]',
+                'post_index': '[bIdx]',
+                'pre_prefix': 'pre_',
+                'post_prefix': 'post_'
+            })
+        else:
+            raise NotImplementedError
+
+        # Pixel-wise applied operation
+        increment = self.synapse_type.description['psp']['cpp']
+        if Global._check_paradigm("cuda"):
+            increment = increment.replace("w%(local_index)s", "w_bank%(local_index)s")
+        increment %= inc_dict
 
         # Delays
         if self.delays > Global.config['dt']:
             increment = increment.replace(
                 'pop%(id_pre)s.r[rk_pre]' % {'id_pre': self.pre.id},
                 'delayed_r[rk_pre]'
             )
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Copy.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/Copy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,23 @@
-# =============================================================================
-#
-#     CopyProjection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2019  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from copy import deepcopy
 
-from ANNarchy.core.Projection import Projection
 from ANNarchy.core import Global
+from ANNarchy.core.SpecificProjection import SpecificProjection
+from ANNarchy.core.Projection import Projection
 from ANNarchy.extensions.convolution import Convolution, Pooling
 
 from .CopyTemplate import copy_proj_template, copy_sum_template
 from .Utils import SharedSynapse
 
-class Copy(Projection):
+class Copy(SpecificProjection):
     """
     Creates a virtual projection reusing the weights and delays of an already-defined projection.
 
     Although the original projection can be learnable, this one can not. Changes in the original weights will be reflected in this projection. The only possible modifications are ``psp`` and ``operation``.
 
     The pre- and post-synaptic populations of both projections must have the same geometry.
 
@@ -55,15 +38,15 @@
         :param post: post-synaptic population (either its name or a ``Population`` object).
         :param target: type of the connection
         :param psp: continuous influence of a single synapse on the post-synaptic neuron (default for rate-coded: ``w*pre.r``).
         :param operation: operation (sum, max, min, mean) performed by the kernel (default: sum).
         """
 
         # Create the description, but it will not be used for generation
-        Projection.__init__(
+        SpecificProjection.__init__(
             self,
             pre=pre,
             post=post,
             target=target,
             synapse = SharedSynapse(psp=psp, operation=operation),
             name=name,
             copied=copied
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Pooling.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/Pooling.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-# =============================================================================
-#
-#     Pooling.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2019  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
-from ANNarchy.core.Projection import Projection
-from ANNarchy.core.Synapse import Synapse
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
+from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.core import Global
 from ANNarchy.generator.Utils import tabify, remove_trailing_spaces
 
 from copy import deepcopy
 
 from .PoolingTemplate import *
 from .Utils import SharedSynapse
 
 # Indices used for each dimension
 indices = ['i', 'j', 'k', 'l', 'm', 'n']
 
-class Pooling(Projection):
+class Pooling(SpecificProjection):
     """
     Performs a pooling operation (e.g. max.pooling) on the pre-synaptic population.
 
     Each post-synaptic neuron covers a specific region (``extent``) of the pre-synaptic
     population, over which the result of the operation on firing rates will be
     assigned to sum(target).
 
@@ -57,26 +38,22 @@
         """
         :param pre: pre-synaptic population (either its name or a ``Population`` object).
         :param post: post-synaptic population (either its name or a ``Population`` object).
         :param target: type of the connection
         :param operation: pooling function to be applied ("max", "min", "mean")
         """
         # Sanity check
-        #if not pre.neuron_type.type == 'rate':
-        #    Global._error('Pooling: only implemented for rate-coded populations.')
-
-        # Sanity check
         if not operation in ["max", "mean", "min"]:
             Global._error("Pooling: the operation must be either 'max', 'mean' or 'min'.")
         self.operation = operation
 
         # Store for _copy
         self.psp = psp
 
-        Projection.__init__(
+        SpecificProjection.__init__(
             self,
             pre,
             post,
             target,
             synapse=SharedSynapse(psp=psp, operation=operation, name="Pooling operation", description=operation+"-pooling operation over the pre-synaptic population."),
             name=name,
             copied=copied
@@ -175,15 +152,15 @@
         """
         if not self._connection_method:
             Global._error(
                 'Pooling: The projection between ' + self.pre.name + ' and ' + self.post.name + ' is declared but not connected.')
 
         # Create the Cython instance
         proj = getattr(module, 'proj' + str(self.id) + '_wrapper')
-        self.cyInstance = proj([], self.pre_coordinates)
+        self.cyInstance = proj(self.pre_coordinates)
 
         return True
 
     def _generate_extent_coordinates(self):
         """
         Generates for each post-neuron the position of the top-left corner, where the pooling should be applied.
 
@@ -237,16 +214,15 @@
         # Convolve_code
         convolve_code, sum_code = self._generate_pooling_code()
 
         # Generate the code
         if Global._check_paradigm("openmp"):
             self._generate_omp(convolve_code, sum_code)
         elif Global._check_paradigm("cuda"):
-            Global._error("Pooling: not available on GPU devices")
-            #self._generate_cuda(convolve_code, sum_code)
+            self._generate_cuda()
         else:
             Global._error("Pooling: not implemented for the configured paradigm")
 
     def _generate_pooling_code(self):
         """
         Generate loop statements for the desired pooling operation.
         """
@@ -418,15 +394,15 @@
         # Compute sum
         wsum = """
         if ( _transmission && pop%(id_pre)s._active ) {
         std::vector<int> coord;
 """ + pre_load_r + """
         %(omp_code)s
         for(int i = 0; i < %(size_post)s; i++){
-            coord = pre_rank[i];
+            coord = pre_coords[i];
 """ + convolve_code + """
             pop%(id_post)s.%(target)s[i] += """ + sum_code + """;
         } // for
         } // if
 """
 
         # Delays
@@ -445,53 +421,53 @@
         }
 
         # Psp code
         self._specific_template['psp_code'] = wsum % psp_dict
         self._specific_template['size_in_bytes'] = """
         // connectivity
         size_in_bytes += sizeof(std::vector<int>);
-        size_in_bytes += pre_rank.capacity() * sizeof(int);
+        size_in_bytes += pre_coords.capacity() * sizeof(int);
 
         size_in_bytes += sizeof(std::vector<std::vector<int>>);
-        size_in_bytes += pre_rank.capacity() * sizeof(std::vector<int>);
-        for (auto it = pre_rank.begin(); it != pre_rank.end(); it++) {
+        size_in_bytes += pre_coords.capacity() * sizeof(std::vector<int>);
+        for (auto it = pre_coords.begin(); it != pre_coords.end(); it++) {
             size_in_bytes += it->capacity() * sizeof(int);
         }
 """
-        self._specific_template['clear'] = """
-        // post-ranks
-        post_rank.clear();
-        post_rank.shrink_to_fit();
-
-        // pre-ranks sub-lists
-        for (auto it = pre_rank.begin(); it != pre_rank.end(); it++) {
-            it->clear();
-            it->shrink_to_fit();
-        }
-        // pre-ranks top-list
-        pre_rank.clear();
-        pre_rank.shrink_to_fit();
-"""
 
-    def _generate_cuda(self, convolve_code, sum_code):
+        # Clean-up
+        self._specific_template['clear_container'] = pooling_template_omp["clear"]
+
+    def _generate_cuda(self):
         """
         Update the ProjectionGenerator._specific_template structure and bypass the standard CUDA code generation.
         """
+        # Extract operation and pre-synaptic variable which should be processed
         pool_operation = self.synapse_type.operation
+        pre_var = self.synapse_type.psp.split(".")[1]
 
         # default value for sum in code depends on operation
         sum_default = "0.0"
         if pool_operation == "min":
             sum_default = "FLT_MAX"
         elif pool_operation == "max":
             sum_default = "FLT_MIN"
 
         # operation to perform
         pool_op_code = cuda_op_code[pool_operation] % {'float_prec': Global.config['precision']}
 
+        # mean operation requires one additional computation
+        if pool_operation == "mean":
+            size = 1
+            for dim in range(self.pre.dimension):
+                size *= self.extent[dim]
+            final_result = "psp[bIdx] += local_res/" + str(size) + ";"
+        else:
+            final_result = "psp[bIdx] += local_res;"
+
         # result dictionary with code for
         # body, call and header
         pool_template = {}
         base_ids = {
             'id_proj': self.id,
             'id_pre': self.pre.id,
             'id_post': self.post.id,
@@ -517,18 +493,20 @@
                 pool_dict.update({
                     'sum_default': sum_default,
                     'row_extent': int(self.extent[0]),
                     'col_extent': int(self.extent[1]),
                     'row_size': int(self.pre.geometry[0]),
                     'col_size': int(self.pre.geometry[1]),
                     'operation': tabify(pool_op_code, 3),
-                    'operation_reduce': pool_op_reduce_code
+                    'operation_reduce': pool_op_reduce_code,
+                    'final_result': final_result
                 })
 
                 pool_template['psp_body'] = cuda_pooling_code_2d_small_extent['psp_body'] % pool_dict
+                pool_template['psp_invoke'] = cuda_pooling_code_2d_small_extent['psp_invoke'] % pool_dict
                 pool_template['psp_header'] = cuda_pooling_code_2d_small_extent['psp_header'] % pool_dict
                 pool_template['psp_call'] = cuda_pooling_code_2d_small_extent['psp_call'] % pool_dict
 
             else:
                 pool_op_reduce_code = cuda_pooling_code_2d['reduce_code'][pool_operation] % {
                     'float_prec': Global.config['precision'],
                     'row_extent': int(self.extent[0]),
@@ -539,42 +517,51 @@
                 pool_dict.update({
                     'sum_default': sum_default,
                     'row_extent': int(self.extent[0]),
                     'col_extent': int(self.extent[1]),
                     'row_size': int(self.pre.geometry[0]),
                     'col_size': int(self.pre.geometry[1]),
                     'operation': tabify(pool_op_code, 3),
-                    'operation_reduce': tabify(pool_op_reduce_code, 2)
+                    'operation_reduce': tabify(pool_op_reduce_code, 2),
+                    'final_result': final_result
                 })
 
                 pool_template['psp_body'] = remove_trailing_spaces(cuda_pooling_code_2d['psp_body'] % pool_dict)
+                pool_template['psp_invoke'] = remove_trailing_spaces(cuda_pooling_code_2d['psp_invoke'] % pool_dict)
                 pool_template['psp_header'] = cuda_pooling_code_2d['psp_header'] % pool_dict
                 pool_template['psp_call'] = cuda_pooling_code_2d['psp_call'] % pool_dict
 
         elif len(self.pre.geometry) == 3:
 
             pool_dict = deepcopy(base_ids)
             pool_dict.update({
                 'sum_default': sum_default,
                 'row_extent': self.extent[0],
                 'col_extent': self.extent[1],
                 'plane_extent': self.extent[2],
                 'row_size': self.pre.geometry[0],
                 'col_size': self.pre.geometry[1],
                 'plane_size': self.pre.geometry[2],
-                'operation': tabify(pool_op_code, 4)
+                'pre_var': pre_var,
+                'operation': tabify(pool_op_code, 4),
+                'final_result': final_result
             })
 
             pool_template['psp_body'] = remove_trailing_spaces(cuda_pooling_code_3d['psp_body'] % pool_dict)
+            pool_template['psp_invoke'] = remove_trailing_spaces(cuda_pooling_code_3d['psp_invoke'] % pool_dict)
             pool_template['psp_header'] = cuda_pooling_code_3d['psp_header'] % pool_dict
-            pool_template['psp_call'] = cuda_pooling_code_3d['psp_header'] % pool_dict
+            pool_template['psp_call'] = cuda_pooling_code_3d['psp_call'] % pool_dict
 
         else:
             raise NotImplementedError
 
+        # Post-neuron is a spike neuron (e.g., part of ANN-to-SNN conversion)
+        if self.post.neuron_type.type == "spike":
+            pool_template['psp_call'] = pool_template['psp_call'].replace("gpu__sum_"+self.target, "gpu_g_"+self.target)
+
         # Update psp fields
         self._specific_template.update(pool_template)
 
         # Specific template for generation (wrapper, etc)
         pool_dict = deepcopy(pooling_template_cuda)
         for key, value in pool_dict.items():
             value = value % base_ids
@@ -582,14 +569,17 @@
         self._specific_template.update(pool_dict)
 
         self._specific_template['wrapper_connector_call'] = ""
         self._specific_template['access_parameters_variables'] = ""
 
         self._specific_template['size_in_bytes'] = "//TODO:\n"
 
+        # Clean-up
+        self._specific_template['clear_container'] = pooling_template_cuda["clear"]
+
     @staticmethod
     def _coordinates_to_rank(name, geometry):
         """
         Generate the code for array access, for instance used
         for pre-synaptic ranks.
         """
         dim = len(geometry)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/PoolingTemplate.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/PoolingTemplate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,62 @@
-# =============================================================================
-#
-#     PoolingTemplate.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 pooling_template_omp = {
     'include_additional': '#include <limits>',
 
     # Declare the connectivity matrix
     'declare_connectivity_matrix': """
     // connectivity data
-    std::vector<int> post_rank;
-    std::vector< std::vector<int> > pre_rank;
+    std::vector< std::vector<int> > pre_coords;
     """,
 
     # Accessors for the connectivity matrix
     'access_connectivity_matrix': """
     // Accessor to connectivity data
-    std::vector<int> get_post_rank() { return post_rank; }
-    void set_post_rank(std::vector<int> ranks) { post_rank = ranks; }
-    std::vector< std::vector<int> > get_pre_rank() { return pre_rank; }
-    void set_pre_rank(std::vector< std::vector<int> > ranks) { pre_rank = ranks; }
-    int nb_synapses() { 
-        int size = 0;
-        for(auto it = pre_rank.cbegin(); it != pre_rank.cend(); it++)
-            size += it->size(); 
-        return size;
-    }
-    int dendrite_size(int n) { return pre_rank[n].size(); }
-    int nb_dendrites() { return post_rank.size(); }
+    std::vector< std::vector<int> > get_pre_coords() { return pre_coords; }
+    void set_pre_coords(std::vector< std::vector<int> > coords) { pre_coords = coords; }
 """,
 
     # Export the connectivity matrix
     'export_connectivity': """
-        vector[int] get_post_rank()
-        vector[vector[int]] get_pre_rank()
-        void set_post_rank(vector[int])
-        void set_pre_rank(vector[vector[int]])
-        int nb_synapses()
-        int dendrite_size(int n)
-        int nb_dendrites()
+        vector[vector[int]] get_pre_coords()
+        void set_pre_coords(vector[vector[int]])
 """,
 
     # No additional variables
     'declare_parameters_variables': "",
     'access_parameters_variables': "",
     'export_parameters_variables': "",
 
     # Arguments to the wrapper constructor
-    'wrapper_args': "weights, coords",
+    'wrapper_args': "coords",
 
     # Initialize the wrapper connectivity matrix
     'wrapper_init_connectivity': """
-        proj%(id_proj)s.set_post_rank(list(range(%(size_post)s)))
-        proj%(id_proj)s.set_pre_rank(coords)
+        proj%(id_proj)s.set_pre_coords(coords)
 """,
     # Something like init_from_lil?
     'wrapper_connector_call': "",
 
     # Wrapper access to connectivity matrix
     'wrapper_access_connectivity': """
-    # Connectivity
+    property size:
+        def __get__(self):
+            return %(size_post)s
     def post_rank(self):
-        return proj%(id_proj)s.get_post_rank()
-    def pre_rank(self, int n):
-        return proj%(id_proj)s.get_pre_rank()
+        return list(np.arange(0, %(size_post)s))
+    def pre_coords(self):
+        return proj%(id_proj)s.get_pre_coords()
     def nb_synapses(self):
-        return proj%(id_proj)s.nb_synapses()
+        return 0
     def dendrite_size(self, lil_idx):
-        return proj%(id_proj)s.dendrite_size(lil_idx)
+        return 0
 """,
 
     # Wrapper access to variables
     'wrapper_access_parameters_variables': "",
 
     # Variables for the psp code
     'psp_prefix': """
@@ -97,112 +64,132 @@
         %(float_prec)s sum=%(sum_default)s;
     """,
 
     # Delays
     'wrapper_init_delay': "",
     
     # Override the monitor to avoid recording the weights
-    'monitor_class':"""
-""",
-    'monitor_export': """
-""",
-     'monitor_wrapper': """
+    'monitor_class':"",
+    'monitor_export': "",
+    'monitor_wrapper': "",
+
+    # Clear connectivity
+    'clear': """
+        // pre-coords sub-lists
+        for (auto it = pre_coords.begin(); it != pre_coords.end(); it++) {
+            it->clear();
+            it->shrink_to_fit();
+        }
+        // pre-coords top-list
+        pre_coords.clear();
+        pre_coords.shrink_to_fit();
 """
 }
 
 pooling_template_cuda = {
     'include_additional': '#include <cfloat>',
 
     # Declare the connectivity matrix
     'declare_connectivity_matrix': """
-    std::vector< std::vector<int> > coords;
-    int *gpu_coords;
+    std::vector< std::vector<int> > pre_coords;
+    int *gpu_pre_coords;
     """,
 
     # Accessors for the connectivity matrix
     'access_connectivity_matrix': """
     // Accessor to pre-synaptic coordinates (upper left corner)
-    std::vector< std::vector<int> > get_coords() { return this->coords; }
-    void set_coords(std::vector< std::vector<int> > coords) {
-        this->coords = coords;
+    std::vector< std::vector<int> > get_pre_coords() { return pre_coords; }
+    void set_pre_coords(std::vector< std::vector<int> > coords) {
+        // host side
+        pre_coords = coords;
 
         // Flattening coords
         auto num_coords = coords.size();
         auto coord_width = coords[0].size();
         auto flat_coords = std::vector<int>(num_coords*coord_width, 0);
         for (auto i = 0; i < num_coords; i++) {
             for( auto j = 0; j < coord_width; j++ ) {
                 flat_coords[i*coord_width+j] = coords[i][j];
             }
         }
 
-        cudaMalloc((void**)&gpu_coords, flat_coords.size()*sizeof(int));
-        cudaMemcpy( gpu_coords, flat_coords.data(), flat_coords.size()*sizeof(int), cudaMemcpyHostToDevice);
+        cudaMalloc((void**)&gpu_pre_coords, flat_coords.size()*sizeof(int));
+        cudaMemcpy( gpu_pre_coords, flat_coords.data(), flat_coords.size()*sizeof(int), cudaMemcpyHostToDevice);
         auto err = cudaGetLastError();
         if (err != cudaSuccess) {
             std::cerr << "Pooling: " << cudaGetErrorString(err) << std::endl;
         }
     }
-    int dendrite_size(int n) { return 0; }
-    int nb_synapses() { return 0; }
 """,
 
     # Export the connectivity matrix
     'export_connectivity': """
         # Connectivity
-        vector[vector[int]] get_coords()
-        void set_coords(vector[vector[int]])
+        vector[vector[int]] get_pre_coords()
+        void set_pre_coords(vector[vector[int]])
 """,
 
     # Arguments to the wrapper constructor
-    'wrapper_args': "weights, coords",
+    'wrapper_args': "coords",
 
     # Initialize the wrapper connectivity matrix
     'wrapper_init_connectivity': """
-        proj%(id_proj)s.set_coords(coords)
+        proj%(id_proj)s.set_pre_coords(coords)
 """,
     # Wrapper access to connectivity matrix
     'wrapper_access_connectivity': """
-    # Connectivity
     def post_rank(self):
-        return np.arange(0, %(size_post)s)
-    def pre_rank(self, int n):
-        return proj%(id_proj)s.get_coords()
+        return []
     def nb_synapses(self):
-        return proj%(id_proj)s.nb_synapses()
+        return 0
     def dendrite_size(self, n):
-        return proj%(id_proj)s.dendrite_size(n)
+        return 0
 """,
 
     # Wrapper access to variables
     'wrapper_access_parameters_variables': "",
 
     'init_connectivity_matrix': "",
 
     # Memory transfer of variables
     'host_device_transfer': "",
     'device_host_transfer': "",
 
     # Override the monitor to avoid recording the weights
     'monitor_class':"",
     'monitor_export': "",
-    'monitor_wrapper': ""
+    'monitor_wrapper': "",
+
+    # Memory management
+    'clear': """
+    // pre-coords sub-lists (host-side)
+    for (auto it = pre_coords.begin(); it != pre_coords.end(); it++) {
+        it->clear();
+        it->shrink_to_fit();
+    }
+    // pre-coords top-list (host-side)
+    pre_coords.clear();
+    pre_coords.shrink_to_fit();
+
+    // device side
+    cudaFree(gpu_pre_coords);
+"""
 }
 
 cuda_op_code = {
     'min': """if ( local_r < local_res ) local_res = local_r;""",
     'max': """if ( local_r > local_res ) local_res = local_r;""",
     'mean': "local_res += local_r;"
 }
 
 #
 # For really small kernels it turns out to be beneficial
 # to perform the operation with a single thread per block.
 cuda_pooling_code_2d_small_extent = {
-    'psp_body': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int num_centers, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r) {
+    'psp_body': """__global__ void cu_pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int num_centers, const int* __restrict__ centers, const %(float_prec)s* __restrict__ %(pre_var)s) {
     int bIdx = blockIdx.x;
     int tid = threadIdx.x;
 
     // shared storage need to be initialized
     extern %(float_prec)s __shared__ sdata[];
     sdata[tid] = %(sum_default)s;
     __syncthreads();
@@ -222,36 +209,43 @@
                 continue;
 
             for( int y = 0; y < %(col_extent)s; y++ ) {
                 idx_y = y_coords + y;
                 if ( idx_y >= %(col_size)s )
                     continue;
 
-                local_r = r [ idx_x * %(col_size)s + idx_y ];
+                local_%(pre_var)s = %(pre_var)s[ idx_x * %(col_size)s + idx_y ];
 %(operation)s
             }
         }
 
         // store intermediate result
         sdata[tid] = local_res;
         __syncthreads();
 
         // Reduction in shared memory
 %(operation_reduce)s
     }
 };
 """,
-    'psp_header': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int num_centers, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r);
+    'psp_invoke': """
+void pooling_proj%(id_proj)s (RunConfig cfg, %(float_prec)s* psp, const int num_centers, const int* centers, const %(float_prec)s* %(pre_var)s) {
+    cu_pooling_proj%(id_proj)s<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        psp, num_centers, centers, %(pre_var_invoke)s
+    );
+}
+""",
+    'psp_header': """void pooling_proj%(id_proj)s (RunConfig cfg, %(float_prec)s* psp, const int num_centers, const int* centers, const %(float_prec)s* %(pre_var)s);
 """,
     'psp_call': """
     int coords_per_block = floor(32.0 / static_cast<%(float_prec)s>(%(col_extent)s));
     int num_blocks = ceil(static_cast<%(float_prec)s>(%(size_post)s) / static_cast<%(float_prec)s>(coords_per_block));
     int thread_per_block = %(col_extent)s * coords_per_block;
     int shared_mem_size = thread_per_block * sizeof(%(float_prec)s);
-    pooling_proj%(id_proj)s<<< num_blocks, thread_per_block, thread_per_block >>>( pop%(id_post)s.gpu__sum_%(target)s, %(size_post)s, proj%(id_proj)s.gpu_coords, pop%(id_pre)s.gpu_r );
+    pooling_proj%(id_proj)s(RunConfig(num_blocks, thread_per_block, shared_mem_size, proj%(id_proj)s.stream), pop%(id_post)s.gpu__sum_%(target)s, %(size_post)s, proj%(id_proj)s.gpu_pre_coords, pop%(id_pre)s.gpu_%(pre_var)s );
 """,
     # The reduction stage is responsible to fuse the several local results within
     # the warp to the final result. ATTENTION: there are several results in this warp
     'reduce_code': {
         'max': """
     if ( tid %% %(col_extent)s == 0 ) {
         for(int y = 1; y < %(col_extent)s; y++)
@@ -263,15 +257,15 @@
     }
 }
 
 #
 # Pooling implementation where a warp handles a row
 # at once.
 cuda_pooling_code_2d = {
-    'psp_body': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int shared_size, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r) {
+    'psp_body': """__global__ void cu_pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int shared_size, const int* __restrict__ centers, const %(float_prec)s* __restrict__ %(pre_var)s) {
     int bIdx = blockIdx.x;
     int tid = threadIdx.x;
 
     // get pre-synaptic coordinates
     int x_coords = centers[2*bIdx];
     int y_coords = centers[2*bIdx+1];
 
@@ -295,37 +289,44 @@
                 continue;
 
             for( int y = tid; y < %(col_extent)s; y += blockDim.x ) {
                 idx_y = y_coords + y;
                 if ( idx_y >= %(col_size)s )
                     continue;
 
-                local_r = r [ idx_x * %(col_size)s + idx_y ];
+                local_%(pre_var)s = %(pre_var)s[ idx_x * %(col_size)s + idx_y ];
 %(operation)s
             }
         }
 
         // store intermediate result
         sdata[tid] = local_res;
         __syncthreads();
 
         // Reduction in shared memory
 %(operation_reduce)s
     }
 }
 """,
-    'psp_header': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int shared_size, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r);
+    'psp_invoke': """
+void pooling_proj%(id_proj)s(RunConfig cfg, %(float_prec)s* psp, const int shared_size, const int* centers, const %(float_prec)s* %(pre_var)s) {
+    cu_pooling_proj%(id_proj)s<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        psp, shared_size, centers, r
+    );
+}
+""",
+    'psp_header': """void pooling_proj%(id_proj)s(RunConfig cfg, %(float_prec)s* psp, const int shared_size, const int* centers, const %(float_prec)s* %(pre_var)s);
 """,
     # Technically, we could use more than warp-size threads.
     # But as we often have small extents it is not required (HD: 27. Nov. 2020)
     'psp_call': """
     auto tpb = 32;
     auto shared_size = min(32, tpb);
     auto smem_size = 2 * shared_size * sizeof(%(float_prec)s);
-    pooling_proj%(id_proj)s<<< %(size_post)s, tpb, smem_size >>>( pop%(id_post)s.gpu__sum_%(target)s, 2*shared_size, proj%(id_proj)s.gpu_coords, pop%(id_pre)s.gpu_r );
+    pooling_proj%(id_proj)s(RunConfig(%(size_post)s, tpb, smem_size, proj%(id_projs).stream), pop%(id_post)s.gpu__sum_%(target)s, 2*shared_size, proj%(id_proj)s.gpu_pre_coords, pop%(id_pre)s.gpu_%(pre_var)s );
 """,
     # The reduction stage is responsible to fuse the
     # several local results within the warp to the final result
     'reduce_code': {
         'min': """if (tid < 16)
 {
     volatile %(float_prec)s* smem = sdata;
@@ -380,48 +381,61 @@
     psp[bIdx] = sdata[0] / static_cast<%(float_prec)s>(%(row_extent)s * %(col_extent)s);
 }
 """
     }
 }
 
 cuda_pooling_code_3d = {
-    'psp_body': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int shared_size, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r) {
+    'psp_body': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int* __restrict__ centers, const %(float_prec)s* __restrict__ %(pre_var)s) {
     int bIdx = blockIdx.x;
-    int tid = threadIdx.x;
 
     int x_coords = centers[3*bIdx];
     int y_coords = centers[3*bIdx+1];
     int z_coords = centers[3*bIdx+2];
 
     int idx_x, idx_y, idx_z;
     %(float_prec)s local_r = 0.0;
     %(float_prec)s local_res = %(sum_default)s;
 
-    for( int x = 0; x < %(row_extent)s; x++ ) {
+    for (int x = 0; x < %(row_extent)s; x++ ) {
         idx_x = x_coords + x;
         if ( idx_x >= %(row_size)s )
             continue;
 
-        for( int y = 0; y < %(col_extent)s; y++ ) {
+        for (int y = 0; y < %(col_extent)s; y++ ) {
             idx_y = y_coords + y;
             if ( idx_y >= %(col_size)s )
                 continue;
 
-            for(int z = 0; z < %(plane_extent)s; z++) {
+            for (int z = 0; z < %(plane_extent)s; z++) {
                 idx_z = z_coords + z;
                 if ( idx_z >= %(plane_size)s )
                     continue;
 
-                local_r = r [ %(plane_size)s * (%(col_size)s * idx_x + idx_y) + idx_z ];
+                local_r = %(pre_var)s[ %(plane_size)s * (%(col_size)s * idx_x + idx_y) + idx_z ];
 %(operation)s
             }
         }
     }
 
-    psp[bIdx] = local_res;
+    %(final_result)s
+}
+""",
+    'psp_invoke': """void pooling_proj%(id_proj)s(RunConfig cfg, %(float_prec)s* psp, const int* centers, const %(float_prec)s* %(pre_var)s) {
+    pooling_proj%(id_proj)s<<< %(size_post)s, 1 >>>(psp, centers, %(pre_var)s);
+}
 """,
-    'psp_header': """__global__ void pooling_proj%(id_proj)s ( %(float_prec)s* __restrict__ psp, const int* __restrict__ centers, const %(float_prec)s* __restrict__ r);
+    'psp_header': """void pooling_proj%(id_proj)s(RunConfig cfg, %(float_prec)s* psp, const int* centers, const %(float_prec)s* %(pre_var)s);
 """,
     'psp_call': """
-    pooling_proj%(id_proj)s<<< %(size_post)s, 1 >>>( pop%(id_post)s.gpu__sum_%(target)s, proj%(id_proj)s.gpu_coords, pop%(id_pre)s.gpu_r );
+    if (proj%(id_proj)s._transmission && pop%(id_post)s._active ) {
+        pooling_proj%(id_proj)s(RunConfig(%(size_post)s, 1, 0, proj%(id_proj)s.stream), pop%(id_post)s.gpu__sum_%(target)s, proj%(id_proj)s.gpu_pre_coords, pop%(id_pre)s.gpu_%(pre_var)s );
+
+    #ifdef _DEBUG
+        auto proj%(id_proj)s_pool_err = cudaDeviceSynchronize();
+        if ( proj%(id_proj)s_pool_err != cudaSuccess) {
+            std::cout << "Pooling projection %(id_proj)s - psp: " << cudaGetErrorString( proj%(id_proj)s_pool_err ) << std::endl;
+        }
+    #endif
+    }
 """
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Transpose.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/Transpose.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-# =============================================================================
-#
-#     CopyProjection.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>,
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
-from ANNarchy.core.Projection import Projection
+from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.models.Synapses import DefaultRateCodedSynapse, DefaultSpikingSynapse
 
-class Transpose(Projection):
+class Transpose(SpecificProjection):
     """
     Creates a transposed projection reusing the weights of an already-defined rate-coded projection. Even though the
     original projection can be learnable, this one can not. The computed post-synaptic potential is the default case
     for rate-coded projections: w * pre.r
 
     The proposed *target* can differ from the target of the forward projection.
 
@@ -44,23 +26,23 @@
     def __init__(self, proj, target):
         """
         :param proj: original projection
         :param target: type of the connection (can differ from the original one)
         """
         # Transpose is not intended for hybrid projections
         if proj.pre.neuron_type.type == "rate" and proj.post.neuron_type.type == "rate":
-            Projection.__init__(
+            SpecificProjection.__init__(
                 self,
                 pre = proj.post,
                 post = proj.pre,
                 target = target,
                 synapse = DefaultRateCodedSynapse
             )
         elif proj.pre.neuron_type.type == "spike" and proj.post.neuron_type.type == "spike":
-            Projection.__init__(
+            SpecificProjection.__init__(
                 self,
                 pre = proj.post,
                 post = proj.pre,
                 target = target,
                 synapse = DefaultSpikingSynapse
             )
         else:
@@ -192,15 +174,15 @@
     def nb_dendrites(self):
         return proj%(id_proj)s.nb_dendrites()
     def dendrite_size(self, lil_idx):
         return proj%(id_proj)s.dendrite_size(lil_idx)
 """ % { 'id_proj': self.id }
 
         # memory management
-        self._specific_template['determine_size_in_bytes'] = ""
+        self._specific_template['size_in_bytes'] = ""
         self._specific_template['clear_container'] = ""
 
         #
         # suppress monitor
         self._specific_template['monitor_export'] = ""
         self._specific_template['monitor_wrapper'] = ""
         self._specific_template['monitor_class'] = ""
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/Utils.py` & `ANNarchy-4.7.3/tests/test_single_thread.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,35 @@
-# =============================================================================
-#
-#     Utils.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2019  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-# =============================================================================
-from ANNarchy.core.Synapse import Synapse
-
-class SharedSynapse(Synapse):
-    """
-    Shared synapse for report()
-    """
-    # For reporting
-    _instantiated = []
-
-    def __init__(self, psp, operation, name="Shared synapse", description="Weight shared over all synapses of the projection."):
-        """
-        """
-        # Shared synapses are non-plastic.
-        Synapse.__init__(self, 
-            psp=psp, operation=operation,
-            name=name, 
-            description=description
-        )
+"""
 
-        # For reporting
-        self._instantiated.append(True)
+    test_single_thread.py
+
+    This file is part of ANNarchy.
+
+    Copyright (C) 2013-2016 Joseph Gussev <joseph.gussev@s2012.tu-chemnitz.de>,
+    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
+    Julien Vitay <julien.vitay@informatik.tu-chemnitz.de>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    ANNarchy is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+"""
+import unittest
+
+from Common import *
+from Interface import *
+from Neuron import *
+from Synapse import *
+# without further arguments ANNarchy generates single threaded code
+
+
+if __name__ == '__main__':
+    unittest.main(verbosity=2)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/convolution/__init__.py` & `ANNarchy-4.7.3/ANNarchy/extensions/convolution/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/diagonal/DiagonalProjection.py` & `ANNarchy-4.7.3/ANNarchy/extensions/diagonal/DiagonalProjection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 """
-
-    DiagonalProjection.py
-
-    This file is part of ANNarchy.
-
-    Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    ANNarchy is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
 """
+
 from ANNarchy.core.Projection import Projection
 import ANNarchy.core.Global as Global
 
 import numpy as np
 
 
 class DiagonalProjection(Projection):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/hybrid/HybridPopulation.py` & `ANNarchy-4.7.3/ANNarchy/extensions/hybrid/HybridPopulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Population import Population
 from ANNarchy.core.Neuron import Neuron
 import ANNarchy.core.Global as Global
 
 class Spike2RatePopulation(Population):
     """
     Converts a population of spiking neurons into a population of rate-coded neurons.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/image/ImagePopulation.py` & `ANNarchy-4.7.3/ANNarchy/extensions/image/ImagePopulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Population import Population
 from ANNarchy.core.Neuron import Neuron
 import ANNarchy.core.Global as Global
 from ANNarchy.generator.Compiler import extra_libs 
 
 try:
     from PIL import Image
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/extensions/tensorboard/Logger.py` & `ANNarchy-4.7.3/ANNarchy/extensions/tensorboard/Logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     tensorboard/Logger.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 try:
     from tensorboardX import SummaryWriter
 except Exception as e:
     print(e)
     Global._error("tensorboard extension: please install tensorboardX (pip install tensorboardX).")
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/CodeGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/CodeGenerator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#==============================================================================
-#
-#     CodeGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2019  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#==============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import time
 import ANNarchy.core.Global as Global
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.parser.Extraction import extract_functions
 
 from ANNarchy.generator.PyxGenerator import PyxGenerator
 from ANNarchy.generator.MonitorGenerator import MonitorGenerator
@@ -154,30 +136,41 @@
         for proj in self._projections:
             self._proj_desc.append(self._projgen.header_struct(proj, self._annarchy_dir))
 
         # where all source files should take place
         source_dest = self._annarchy_dir+'/generate/net'+str(self._net_id)+'/'
 
         # Generate header code for the analysed pops and projs
-        with open(source_dest+'ANNarchy.h', 'w') as ofile:
-            ofile.write(self._generate_header())
+        if Global.config['paradigm'] == "openmp":
+            with open(source_dest+'ANNarchy.h', 'w') as ofile:
+                ofile.write(self._generate_header())
+
+        elif Global.config['paradigm'] == "cuda":
+            invoke_header, host_header = self._generate_header()
+            with open(source_dest+'ANNarchyKernel.cuh', 'w') as ofile:
+                ofile.write(invoke_header)
+            with open(source_dest+'ANNarchy.h', 'w') as ofile:
+                ofile.write(host_header)
+
+        else:
+            raise NotImplementedError
 
         # Generate monitor code for the analysed pops and projs
         self._recordgen.generate()
 
         # Generate cpp code for the analysed pops and projs
         if Global.config['paradigm'] == "openmp":
             with open(source_dest+'ANNarchy.cpp', 'w') as ofile:
                 ofile.write(self._generate_body())
 
         elif Global.config['paradigm'] == "cuda":
             device_code, host_code = self._generate_body()
-            with open(source_dest+'ANNarchyHost.cu', 'w') as ofile:
+            with open(source_dest+'ANNarchy.cpp', 'w') as ofile:
                 ofile.write(host_code)
-            with open(source_dest+'ANNarchyDevice.cu', 'w') as ofile:
+            with open(source_dest+'ANNarchyKernel.cu', 'w') as ofile:
                 ofile.write(device_code)
 
         else:
             raise NotImplementedError
 
         # Generate cython code for the analysed pops and projs
         with open(source_dest+'ANNarchyCore'+str(self._net_id)+'.pyx', 'w') as ofile:
@@ -264,15 +257,15 @@
                     if isinstance(proj.pre, PopulationView):
                         proj.pre.population.delayed_variables.append(var)
                     else:
                         proj.pre.delayed_variables.append(var)
 
         # Make sure the operations are declared only once
         for pop in self._populations:
-            pop.global_operations = [dict(y) for y in set(tuple(x.items()) for x in pop.global_operations)]
+            pop.global_operations = [dict(y) for y in sorted(set(tuple(x.items())) for x in pop.global_operations)]
             pop.delayed_variables = sorted(list(set(pop.delayed_variables)))
 
     def _generate_header(self):
         """
         Generate the ANNarchy.h code. This header represents the interface to
         the Python extension and therefore includes all network objects.
         """
@@ -306,30 +299,50 @@
                 'proj_struct': proj_struct,
                 'pop_ptr': pop_ptr,
                 'proj_ptr': proj_ptr,
                 'custom_func': custom_func,
                 'custom_constant': custom_constant,
                 'built_in': BaseTemplate.built_in_functions + BaseTemplate.integer_power_cpu % {'float_prec': Global.config['precision']},
             }
+            return header_code
+
         elif Global.config['paradigm'] == "cuda":
-            header_code = BaseTemplate.cuda_header_template % {
+            # kernel declaration
+            invoke_kernel_def = ""
+            for pop in self._pop_desc:
+                invoke_kernel_def += pop['update_header']
+
+            for proj in self._proj_desc:
+                invoke_kernel_def += proj['psp_kernel_decl']
+                invoke_kernel_def += proj['update_synapse_header']
+                invoke_kernel_def += proj['postevent_header']
+
+            glob_ops_header, _, _ = self._body_def_glops()
+            invoke_kernel_def += glob_ops_header
+
+            device_invoke_header = BaseTemplate.cuda_device_invoke_header % {
+                'float_prec': Global.config['precision'],
+                'invoke_kernel_def': invoke_kernel_def
+            }
+
+            host_header_code = BaseTemplate.cuda_header_template % {
                 'float_prec': Global.config['precision'],
                 'pop_struct': pop_struct,
                 'proj_struct': proj_struct,
                 'pop_ptr': pop_ptr,
                 'proj_ptr': proj_ptr,
                 'custom_func': custom_func,
                 'built_in': BaseTemplate.built_in_functions,
                 'custom_constant': custom_constant
             }
+            return device_invoke_header, host_header_code
+        
         else:
             raise NotImplementedError
 
-        return header_code
-
     def _header_custom_functions(self):
         """
         Generate code for custom functions defined globally and are usable
         witihn neuron or synapse descriptions. These functions can only rely on
         provided arguments.
         """
         if len(Global._objects['functions']) == 0:
@@ -375,17 +388,16 @@
         Returns (openMP):
 
         * decl_code: declarations in header file
         * init_code: initialization code
 
         Returns (CUDA):
 
-        * host_decl_code: declarations in header file (host side)
-        * host_init_code: initialization code (host side)
         * device_decl_code: declarations in header file (device side)
+        * host_init_code: initialization code (host side)
 
         """
         if Global._check_paradigm("openmp"):
             if len(Global._objects['constants']) == 0:
                 return "", ""
 
             decl_code = ""
@@ -399,42 +411,43 @@
                 decl_code += """
 %(float_prec)s %(name)s;
 void set_%(name)s(%(float_prec)s value){%(name)s = value;};""" % obj_str
                 init_code += """
         %(name)s = 0.0;""" % obj_str
 
             return decl_code, init_code
+
         elif Global._check_paradigm("cuda"):
             if len(Global._objects['constants']) == 0:
-                return "", "", ""
+                return "", ""
 
-            host_decl_code = ""
             host_init_code = ""
             device_decl_code = ""
             for obj in Global._objects['constants']:
                 obj_str = {
                     'name': obj.name,
                     'value': obj.value,
                     'float_prec': Global.config['precision']
                 }
-                host_decl_code += """
-__device__ __constant__ %(float_prec)s %(name)s;
-void set_%(name)s(%(float_prec)s value){
+                device_decl_code += """__device__ __constant__ %(float_prec)s %(name)s;
+void set_%(name)s(%(float_prec)s value) {
     cudaError_t err = cudaMemcpyToSymbol(%(name)s, &value, sizeof(%(float_prec)s), 0, cudaMemcpyHostToDevice);
 #ifdef _DEBUG
-    std::cout << "set %(name)s " << value << std::endl;
+    std::cout << "set global constant %(name)s = " << value << std::endl;
     if ( err != cudaSuccess )
         std::cerr << cudaGetErrorString(err) << std::endl;
 #endif
 }""" % obj_str
-                device_decl_code += "__device__ __constant__ %(float_prec)s %(name)s;\n" % obj_str
+
+                # TODO: is this really needed, it's overwritten anyways ?
                 host_init_code += """
-        %(name)s = 0.0;""" % obj_str
+        set_%(name)s(0.0);""" % obj_str
+
+            return device_decl_code, host_init_code
 
-            return host_decl_code, host_init_code, device_decl_code
         else:
             raise NotImplementedError
 
     def _generate_body(self):
         """
         Generate the codes 'main' library file. The generated code
         will be used in different files, dependent on the chosen
@@ -568,117 +581,107 @@
             # return the codes via the descriptor dictionary.
             #
             # This ensures a consistent interface in the generators and also in the generated
             # codes, but sometimes require additional overhead. Hopefully NVidia will improve
             # their linker in the next releases, so one could remove this overhead.
             psp_call = ""
             for proj in self._proj_desc:
-                psp_call += proj['psp_call']
+                psp_call += proj['psp_host_call']
 
             # custom constants
-            host_custom_constant, _, device_custom_constant = self._body_custom_constants()
+            device_custom_constant, _ = self._body_custom_constants()
 
             # custom functions
             custom_func = ""
             for pop in self._pop_desc:
                 custom_func += pop['custom_func']
             for proj in self._proj_desc:
                 custom_func += proj['custom_func']
             for _, func in Global._objects['functions']:
                 custom_func += extract_functions(func, local_global=True)[0]['cpp'].replace("inline", "__device__") + '\n'
 
             # pre-defined/common available kernel
             common_kernel = self._cuda_common_kernel(self._projections)
 
             pop_kernel = ""
+            pop_invoke_kernel = ""
             for pop in self._pop_desc:
                 pop_kernel += pop['update_body']
+                pop_invoke_kernel += pop['update_invoke']
 
             pop_update_fr = ""
             for pop in self._pop_desc:
                 pop_update_fr += pop['update_FR']
 
-            psp_kernel = ""
-            for proj in self._proj_desc:
-                psp_kernel += proj['psp_body']
-
-            kernel_def = ""
-            for pop in self._pop_desc:
-                kernel_def += pop['update_header']
-
+            psp_device_kernel = ""
+            psp_invoke_kernel = ""
             for proj in self._proj_desc:
-                kernel_def += proj['psp_header']
-                kernel_def += proj['update_synapse_header']
-                kernel_def += proj['postevent_header']
+                psp_device_kernel += proj['psp_device_kernel']
+                psp_invoke_kernel += proj['psp_invoke_kernel']
 
             delay_code = ""
             for pop in self._pop_desc:
                 if 'update_delay' in pop.keys():
                     delay_code += pop['update_delay']
 
             syn_kernel = ""
+            syn_invoke_kernel = ""
             for proj in self._proj_desc:
                 syn_kernel += proj['update_synapse_body']
+                syn_invoke_kernel += proj['update_synapse_invoke']
 
             syn_call = ""
             for proj in self._proj_desc:
                 syn_call += proj['update_synapse_call']
 
-            postevent_kernel = ""
+            postevent_device_kernel = ""
+            postevent_invoke_kernel = ""
             for proj in self._proj_desc:
-                postevent_kernel += proj['postevent_body']
+                postevent_device_kernel += proj['postevent_body']
+                postevent_invoke_kernel += proj['postevent_invoke']
 
             postevent_call = ""
             for proj in self._proj_desc:
                 postevent_call += proj['postevent_call']
 
             clear_sums = self._body_resetcomputesum_pop()
 
             # global operations
-            glob_ops_header, glob_ops_body = self._body_def_glops()
-            kernel_def += glob_ops_header
+            _, glob_ops_invoke, glob_ops_body = self._body_def_glops()
 
             # determine number of threads per kernel
             threads_per_kernel = self._cuda_kernel_config()
 
-            #  concurrent kernel execution
+            # concurrent kernel execution
             stream_setup = self._cuda_stream_config()
 
             # memory transfers
             host_device_transfer, device_host_transfer = "", ""
             for pop in self._pop_desc + self._proj_desc:
                 host_device_transfer += pop['host_to_device']
                 device_host_transfer += pop['device_to_host']
 
-            #Profiling
+            # Profiling
             if self._profgen:
                 prof_dict = self._profgen.generate_body_dict()
             else:
                 prof_dict = Profile.ProfileGenerator(self._annarchy_dir, self._net_id).generate_body_dict()
 
-            #
-            # HD ( 31.07.2016 ):
-            #
-            # I'm not really sure, what exactly causes the problem with this
-            # atomicAdd function. If we move it into ANNarchyDevice.cu, the
-            # macro seems to be evaluated wrongly and the atomicAdd() function
-            # appears doubled or appears not.
-            #
-            # So as "solution", the atomicAdd definition block resides in
-            # ANNarchyHost and only the computation kernels are placed in
-            # ANNarchyDevice. If we decide to use SDK8 as lowest requirement,
-            # one can move this kernel too.
-            device_code = BaseTemplate.cuda_device_kernel_template % {
-                #device stuff
+            device_code = BaseTemplate.cuda_device_kernel % {      # Target: ANNarchyKernel.cu
                 'common_kernel': common_kernel,
                 'pop_kernel': pop_kernel,
-                'psp_kernel': psp_kernel,
+                'pop_invoke_kernel': pop_invoke_kernel,
+                'psp_kernel': psp_device_kernel,
+                'psp_invoke_kernel': psp_invoke_kernel,
                 'syn_kernel': syn_kernel,
+                'syn_invoke_kernel': syn_invoke_kernel,
                 'glob_ops_kernel': glob_ops_body,
-                'postevent_kernel': postevent_kernel,
+                'glob_ops_invoke_kernel': glob_ops_invoke,
+                'postevent_kernel': postevent_device_kernel,
+                'postevent_invoke_kernel': postevent_invoke_kernel,
                 'custom_func': custom_func,
                 'custom_constant': device_custom_constant,
                 'built_in': BaseTemplate.built_in_functions + BaseTemplate.integer_power_cuda % {'float_prec': Global.config['precision']},
                 'float_prec': Global.config['precision']
             }
 
             base_dict = {
@@ -698,21 +701,19 @@
                 'initialize' : self._body_initialize(),
                 'structural_plasticity': structural_plasticity,
 
                 # cuda host specific
                 'stream_setup': stream_setup,
                 'host_device_transfer': host_device_transfer,
                 'device_host_transfer': device_host_transfer,
-                'kernel_def': kernel_def,
-                'kernel_config': threads_per_kernel,
-                'custom_constant': host_custom_constant
+                'kernel_config': threads_per_kernel
             }
             base_dict.update(prof_dict)
+            host_code = BaseTemplate.cuda_host_body_template % base_dict    # Target: ANNarchy.cpp
 
-            host_code = BaseTemplate.cuda_host_body_template % base_dict
             return device_code, host_code
         else:
             raise NotImplementedError
 
     def _body_initialize(self):
         """
         Define codes for the method initialize(), comprising of population and projection
@@ -734,15 +735,15 @@
         if Global.config['paradigm'] == "openmp":
             # Custom  constants
             _, custom_constant = self._body_custom_constants()
 
             init_tpl = BaseTemplate.omp_initialize_template
         elif Global.config['paradigm'] == "cuda":
             # Custom  constants
-            _, custom_constant, _ = self._body_custom_constants()
+            _, custom_constant = self._body_custom_constants()
 
             init_tpl = BaseTemplate.cuda_initialize_template
         else:
             raise NotImplementedError
 
         return init_tpl % {
             'prof_init': profiling_init,
@@ -795,15 +796,15 @@
                 ops.append(op['function'])
 
         # no global operations
         if ops == []:
             if Global._check_paradigm("openmp"):
                 return ""
             elif Global._check_paradigm("cuda"):
-                return "", ""
+                return "", "", ""
             else:
                 raise NotImplementedError("CodeGenerator._body_def_glops(): no implementation for "+Global.config["paradigm"])
 
         type_def = {
             'type': Global.config['precision']
         }
 
@@ -818,21 +819,23 @@
             for op in sorted(list(set(ops))):
                 code += global_op_template[op] % type_def
 
             return code
 
         elif Global._check_paradigm("cuda"):
             header = ""
+            invoke = ""
             body = ""
 
             for op in sorted(list(set(ops))):
                 header += global_operation_templates_cuda[op]['header'] % type_def
+                invoke += global_operation_templates_cuda[op]['invoke'] % type_def
                 body += global_operation_templates_cuda[op]['body'] % type_def
 
-            return header, body
+            return header, invoke, body
         else:
             raise NotImplementedError("CodeGenerator._body_def_glops(): no implementation for "+Global.config["paradigm"])
 
     def _body_run_until(self):
         """
         Generate the code for conditioned stop of simulation
         """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Compiler.py` & `ANNarchy-4.7.3/ANNarchy/generator/Compiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,30 @@
-#===============================================================================
-#
-#     Compiler.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import os, sys, importlib
 import subprocess
 import shutil
 import multiprocessing
 import time
 import json
-import argparse
 import numpy as np
 
 # ANNarchy core informations
 import ANNarchy
 import ANNarchy.core.Global as Global
 
 from ANNarchy.extensions.bold.NormProjection import _update_num_aff_connections
 from ANNarchy.generator.Template.MakefileTemplate import *
 from ANNarchy.generator.CodeGenerator import CodeGenerator
 from ANNarchy.generator.Sanity import check_structure, check_experimental_features
 from ANNarchy.generator.Utils import check_cuda_version
+from ANNarchy.parser.report.Report import report
 
 # String containing the extra libs which can be added by extensions
 # e.g. extra_libs = ['-lopencv_core', '-lopencv_video']
 extra_libs = []
 
 def _folder_management(annarchy_dir, profile_enabled, clean, net_id):
     """
@@ -60,15 +42,15 @@
         Global._print("Create subdirectory.")
 
     if clean or profile_enabled:
         shutil.rmtree(annarchy_dir, True)
 
     # Create the subdirectory
     if not os.path.exists(annarchy_dir):
-        os.mkdir(annarchy_dir)
+        os.makedirs(annarchy_dir)
         os.mkdir(annarchy_dir+'/build')
         os.mkdir(annarchy_dir+'/generate')
 
     # Subdirectory for building networks
     if not os.path.exists(annarchy_dir+'/build/net'+str(net_id)):
         os.mkdir(annarchy_dir+'/build/net'+str(net_id))
 
@@ -78,42 +60,14 @@
 
     # Save current ANNarchy version and paradigm
     with open(annarchy_dir+'/release', 'w') as wfile:
         wfile.write(Global.config['paradigm']+', '+ANNarchy.__release__)
 
     sys.path.append(annarchy_dir)
 
-def setup_parser():
-    """
-    ANNarchy scripts can be run by several command line arguments. These are
-    checked with the ArgumentParser provided by Python.
-    """
-    # override the error behavior of OptionParser,
-    # normally an unknwon arg would raise an exception
-    parser = argparse.ArgumentParser(description='ANNarchy: Artificial Neural Networks architect.')
-
-    group = parser.add_argument_group('General')
-    group.add_argument("-c", "--clean", help="Forces recompilation.", action="store_true", default=False, dest="clean")
-    group.add_argument("-d", "--debug", help="Compilation with debug symbols and additional checks.", action="store_true", default=False, dest="debug")
-    group.add_argument("-v", "--verbose", help="Shows all messages.", action="store_true", default=None, dest="verbose")
-    group.add_argument("--prec", help="Set the floating precision used.", action="store", type=str, default=None, dest="precision")
-
-    group = parser.add_argument_group('OpenMP')
-    group.add_argument("-j", "--num_threads", help="Number of threads to use.", type=int, action="store", default=None, dest="num_threads")
-    group.add_argument("--visible_cores", help="Cores where the threads should be placed.", type=str, action="store", default=None, dest="visible_cores")
-
-    group = parser.add_argument_group('CUDA')
-    group.add_argument("--gpu", help="Enables CUDA and optionally specifies the GPU id (default: 0).", type=int, action="store", nargs='?', default=-1, const=0, dest="gpu_device")
-
-    group = parser.add_argument_group('Internal')
-    group.add_argument("--profile", help="Enables profiling.", action="store_true", default=None, dest="profile")
-    group.add_argument("--profile_out", help="Target file for profiling data.", action="store", type=str, default=None, dest="profile_out")
-
-    return parser
-
 def compile(
         directory='annarchy',
         clean=False,
         populations=None,
         projections=None,
         compiler="default",
         compiler_flags="default",
@@ -148,47 +102,29 @@
     """
     # Check if the network has already been compiled
     if Global._network[net_id]['compiled']:
         Global._print("""compile(): the network has already been compiled, doing nothing.
     If you are re-running a Jupyter notebook, you should call `clear()` right after importing ANNarchy in order to reset everything.""")
         return
 
-    # Get the command-line arguments
-    parser = setup_parser()
-    options, unknown = parser.parse_known_args()
+    # Get command-line arguments. Note that setup() related flags has been partially parsed!
+    options, unknown = ANNarchy._arg_parser.parser.parse_known_args()
+
+    # Check for unknown flags
     if len(unknown) > 0 and Global.config['verbose']:
         Global._warning('unrecognized command-line arguments:', unknown)
 
-    # if the parameters set on command-line they overwrite Global.config
-    if options.num_threads is not None:
-        Global.config['num_threads'] = options.num_threads
-    if options.visible_cores is not None:
-        try:
-            core_list = [int(x) for x in options.visible_cores.split(",")]
-            Global.config['visible_cores'] = core_list
-        except:
-            Global._error("As argument for 'visible_cores' a comma-seperated list of integers is expected.")
-
     # Get CUDA configuration
     if options.gpu_device >= 0:
-        Global.config['paradigm'] = "cuda"
         cuda_config['device'] = int(options.gpu_device)
 
     # Check that a single backend is chosen
     if (options.num_threads != None) and (options.gpu_device >= 0):
         Global._error('CUDA and openMP can not be active at the same time, please check your command line arguments.')
 
-    # Verbose
-    if options.verbose is not None:
-        Global.config['verbose'] = options.verbose
-
-    # Precision
-    if options.precision is not None:
-        Global.config['precision'] = options.precision
-
     # check if profiling was enabled by --profile
     if options.profile != None:
         profile_enabled = options.profile
         Global.config['profiling'] = options.profile
         Global.config['profile_out'] = options.profile_out
     # check if profiling enabled due compile()
     if profile_enabled != False and options.profile == None:
@@ -294,14 +230,18 @@
 
     # NormProjections require an update of afferent projections
     _update_num_aff_connections(compiler.net_id)
 
     if Global.config['verbose']:
         Global._print('OK')
 
+    # Create a report if requested
+    if options.report is not None:
+        report(options.report)
+
 def python_environment():
     """
     Python environment configuration, required by Compiler.generate_makefile. Contains among others the python version, library path and cython version.
 
     Warning: changes to this method should be copied to setup.py.
     """
     # Python version
@@ -622,30 +562,31 @@
         #
         # hdin (22.03.2016): we should verify in the future, if compute_35 remains as best
         # configuration for Keplar and upwards.
         cuda_gen = ""
         gpu_flags = ""
         gpu_compiler = "nvcc"
         gpu_ldpath = ""
+        xcompiler_flags = ""
         if sys.platform.startswith('linux') and Global.config['paradigm'] == "cuda":
             cuda_gen = "" # TODO: -arch sm_%(ver)s
 
             if self.debug_build:
                 gpu_flags = "-g -G -D_DEBUG"
 
             # read the config file for the cuda lib path
             if 'cuda' in self.user_config.keys():
                 gpu_compiler = self.user_config['cuda']['compiler']
                 gpu_ldpath = '-L' + self.user_config['cuda']['path'] + '/lib'
                 gpu_flags += self.user_config['cuda']['flags']
 
             # -Xcompiler expects the arguments seperated by ','
             if len(cpu_flags.strip()) > 0:
-                cpu_flags = cpu_flags.replace(" ",",")
-                cpu_flags += ","
+                xcompiler_flags = cpu_flags.replace(" ",",")
+                xcompiler_flags += ","
 
         # Extra libs from extensions such as opencv
         libs = self.extra_libs
         for lib in extra_libs:
             libs += str(lib) + ' '
 
         # Python environment
@@ -687,14 +628,15 @@
         makefile_flags = {
             'compiler': self.compiler,
             'add_sources': self.add_sources,
             'cpu_flags': cpu_flags,
             'cuda_gen': cuda_gen,
             'gpu_compiler': gpu_compiler,
             'gpu_flags': gpu_flags,
+            'xcompiler_flags': xcompiler_flags,
             'gpu_ldpath': gpu_ldpath,
             'openmp': omp_flag,
             'extra_libs': libs,
             'py_version': py_version,
             'py_major': py_major,
             'cython': cython,
             'python_include': python_include,
@@ -833,14 +775,17 @@
         try:
             dev_id = int(user_config['cuda']['device'])
         except KeyError:
             dev_id = 0
 
         cython_module.set_device(dev_id)
 
+    # Instantiate CPP objects
+    cython_module.pyx_create()
+
     # Configure seeds for random number generators
     # Required for state updates and also (in future) construction of connectivity
     if Global.config['seed'] == -1:
         seed = time.time()
     else:
         seed = Global.config['seed']
 
@@ -872,15 +817,15 @@
         # Create the projection
         proj._instantiate(cython_module)
 
         if Global.config['show_time']:
             Global._print('Creating the projection took', (time.time()-t0)*1000, 'milliseconds')
 
     # Finish to initialize the network
-    cython_module.pyx_create(Global.config['dt'])
+    cython_module.pyx_initialize(Global.config['dt'])
 
     # Set the user-defined constants
     for obj in Global._objects['constants']:
         getattr(cython_module, '_set_'+obj.name)(obj.value)
 
     # Transfer initial values
     for pop in Global._network[net_id]['populations']:
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/CUDAGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/CUDAGenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CUDAGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import re
 from math import ceil
 from copy import deepcopy
 
 import ANNarchy
 
 from ANNarchy.core import Global
@@ -102,31 +84,36 @@
         update_rng = self._update_random_distributions(pop)
 
         # Update global operations
         update_global_ops = self._update_globalops(pop)
 
         # Update the neural variables
         if pop.neuron_type.type == "rate":
-            body, header, update_call = self._update_rate_neuron(pop)
+            body, invoke, header, call = self._update_rate_neuron(pop)
         else:
-            body, header, update_call = self._update_spiking_neuron(pop)
+            update_body, update_invoke, update_header, update_call = self._update_spiking_neuron(pop)
+            spike_body, spike_invoke, spike_header, spike_call = self._spike_gather(pop)
+            body = update_body + spike_body
+            invoke = update_invoke + spike_invoke
+            header = update_header + spike_header
+            call = update_call + spike_call
         update_variables = ""
 
         # Memory transfers
         host_to_device, device_to_host = self._memory_transfers(pop)
 
         # Stop condition
         stop_condition = self._stop_condition(pop)
 
         # Local functions
         host_local_func, device_local_func = self._local_functions(pop)
         declaration_parameters_variables += host_local_func
 
         # Memory management
-        determine_size_in_bytes = self._determine_size_in_bytes(pop)
+        size_in_bytes = self._size_in_bytes(pop)
         clear_container = self._clear_container(pop)
 
         # Profiling
         if self._prof_gen:
             include_profile = """#include "Profiling.h"\n"""
             declare_profile, init_profile = self._prof_gen.generate_init_population(pop)
         else:
@@ -220,15 +207,15 @@
             'update_rng': update_rng,
             'update_delay': update_delay,
             'update_max_delay': update_max_delay,
             'update_global_ops': update_global_ops,
             'stop_condition': stop_condition,
             'host_to_device': host_to_device,
             'device_to_host': device_to_host,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container
         }
 
         # Store the complete header definition in a single file
         with open(annarchy_dir+'/generate/net'+str(self._net_id)+'/pop'+str(pop.id)+'.hpp', 'w') as ofile:
             ofile.write(code)
 
@@ -237,15 +224,16 @@
             'include': """#include "pop%(id)s.hpp"\n""" % {'id': pop.id},
             'extern': """extern PopStruct%(id)s pop%(id)s;\n"""% {'id': pop.id},
             'instance': """PopStruct%(id)s pop%(id)s;\n"""% {'id': pop.id},
             'init': """    pop%(id)s.init_population();\n""" % {'id': pop.id}
         }
 
         pop_desc['custom_func'] = device_local_func
-        pop_desc['update'] = update_call
+        pop_desc['update'] = call
+        pop_desc['update_invoke'] = invoke
         pop_desc['update_body'] = body
         pop_desc['update_header'] = header
         pop_desc['update_delay'] = """    pop%(id)s.update_delay();\n""" % {'id': pop.id} if pop.max_delay > 1 else ""
         pop_desc['update_FR'] = """    pop%(id)s.update_FR();\n""" % {'id': pop.id} if pop.neuron_type.type == "spike" else ""
 
         if len(pop.global_operations) > 0:
             pop_desc['gops_update'] = self._update_globalops(pop) % {'id': pop.id}
@@ -260,42 +248,18 @@
         Clear allocated data structures.
 
         The function overrrides the default behavior as we need a de-allocation
         on host and device side.
         """
         from ANNarchy.generator.Utils import tabify
 
-        code = ""
+        # Variables (host-side), which contains also Mean-FR code
+        code = PopulationGenerator._clear_container(self, pop)
 
-        # Variables (host-side)
-        code += "// Variables\n"
-        for attr in pop.neuron_type.description['variables']:
-            # HD: we need to clear only local variables, the others are no vectors
-            if attr['locality'] == "local":
-                # HD: clear alone does not deallocate, it only resets size.
-                #     So we need to call shrink_to_fit afterwards.
-                ids = {'ctype': attr['ctype'], 'name': attr['name']}
-                code += "%(name)s.clear();\n" % ids
-                code += "%(name)s.shrink_to_fit();\n" % ids
-
-        code += "\n/* Free device variables */\n"
-
-        # Mean-FR (implemented only on host-side)
-        if pop.neuron_type.description['type'] == 'spike':
-            code += """
-// Mean Firing Rate
-for (auto it = _spike_history.begin(); it != _spike_history.end(); it++) {
-    while(!it->empty())
-        it->pop();
-}
-_spike_history.clear();
-_spike_history.shrink_to_fit();
-"""
-
-        # Variables device side
+        # Variables (device side)
         code += "// parameters\n"
         for attr in pop.neuron_type.description['parameters']:
             if attr['locality'] == "local":
                 code += """cudaFree(gpu_%(name)s); \n""" % {'name': attr['name']}
 
         code += "\n// variables\n"
         for attr in pop.neuron_type.description['variables']:
@@ -306,23 +270,14 @@
             delay_tpl = self._templates['attribute_delayed']
             for var in pop.delayed_variables:
                 if var in pop.neuron_type.description['local']:
                     code += delay_tpl['local']['clear'] % {'name': var}
                 else:
                     continue
 
-        # Random variables
-        code += "\n// RNGs\n"
-        for dist in pop.neuron_type.description['random_distributions']:
-            rng_ids = {
-                'id': pop.id,
-                'rd_name': dist['name'],
-            }
-            code += self._templates['rng'][dist['locality']]['clear'] % rng_ids
-
         # clear PSP targets ( for rate-coded neurons, for spiking they are part of population variables )
         code += "\n// targets\n"
         if pop.neuron_type.type == 'rate':
             for target in sorted(list(set(pop.neuron_type.description['targets'] + pop.targets))):
                 code += """cudaFree(gpu__sum_%(target)s); \n""" % {'target': target}
 
         # just code layout
@@ -348,17 +303,17 @@
         if pop.neuron_type.type != 'rate':
             return ""
 
         code = ""
         for target in sorted(list(set(pop.neuron_type.description['targets'] + pop.targets))):
             code += """
     #if defined (__pop%(id)s_nb__)
-        clear_sum <<< __pop%(id)s_nb__, __pop%(id)s_tpb__ >>> ( pop%(id)s.size, pop%(id)s.gpu__sum_%(target)s );
+        call_clear_sum( RunConfig(__pop%(id)s_nb__, __pop%(id)s_tpb__, 0, pop%(id)s.stream), pop%(id)s.size, pop%(id)s.gpu__sum_%(target)s );
     #else
-        clear_sum <<< pop%(id)s._nb_blocks, pop%(id)s._threads_per_block >>> ( pop%(id)s.size, pop%(id)s.gpu__sum_%(target)s );
+        call_clear_sum( RunConfig(pop%(id)s._nb_blocks, pop%(id)s._threads_per_block, 0, pop%(id)s.stream), pop%(id)s.size, pop%(id)s.gpu__sum_%(target)s );
     #endif
 """ % {'id': pop.id, 'target': target}
 
         if code != "":
             code = """
     if ( pop%(id)s._active ) {
 %(reset_code)s
@@ -555,14 +510,15 @@
     def _gen_kernel_args(self, pop, locality):
         """
         Generate the argument and call statemen for neural variables
         used in equations as well as there dependencies.
         """
         # Gather all variable names
         add_args_header = "const long int t, const %(type)s dt" % {'type':Global.config['precision']}
+        add_args_invoke = "t, dt"
         add_args_call = "t, dt"
 
         deps = []
 
         # Variables
         for var in pop.neuron_type.description['variables']:
             if var['locality'] == locality:
@@ -571,44 +527,51 @@
                     deps += var['dependencies']
 
         # Random distributions
         for rd in pop.neuron_type.description['random_distributions']:
             for dep in rd['dependencies']:
                 deps.append(dep)
 
+        # Remove doublons / sort the attribute names to
+        # prevent unnecessary recompiles
+        deps = sorted(list(set(deps)))
+
         # Generate the header and call lines
-        deps = list(set(deps))
         for dep in deps:
             attr_type, attr_dict = self._get_attr_and_type(pop, dep)
             if attr_type == None:
                 continue
 
             ids = {
                 'id': pop.id,
                 'name': attr_dict['name'],
                 'type': attr_dict['ctype']
             }
 
             if attr_type == 'par':
                 if dep in pop.neuron_type.description['global']:
                     add_args_header += ", const %(type)s %(name)s" % ids
+                    add_args_invoke += ", %(name)s" % ids
                     add_args_call += ", pop%(id)s.%(name)s" % ids
                 else:
                     add_args_header += ", %(type)s* __restrict__ %(name)s" % ids
+                    add_args_invoke += ", %(name)s" % ids
                     add_args_call += ", pop%(id)s.gpu_%(name)s" % ids
             elif attr_type == 'var':
                 add_args_header += ", %(type)s* __restrict__ %(name)s" % ids
+                add_args_invoke += ", %(name)s" % ids
                 add_args_call += ", pop%(id)s.gpu_%(name)s" % ids
             elif attr_type == 'rand':
                 add_args_header += ", curandState* state_%(name)s" % ids
+                add_args_invoke += ", state_%(name)s" % ids
                 add_args_call += ", pop%(id)s.gpu_%(name)s" % ids
             else:
                 raise NotImplementedError
 
-        return add_args_header, add_args_call
+        return add_args_header, add_args_invoke, add_args_call
 
     def _local_functions(self, pop):
         """
         Definition of user-defined local functions attached to
         a neuron. These functions will take place in the
         ANNarchyDevice.cu file.
 
@@ -721,14 +684,33 @@
         dependent on a population related condition. The code for
         this is generated here and added to the ANNarchy.cpp/.cu
         file.
         """
         if not pop.stop_condition: # no stop condition has been defined
             return ""
 
+        # Special case for early return based on emitted events
+        if pop.stop_condition.replace(" ", "") == "spiked:any":
+            # HD (3rd May 2023): do not use spiked.empty as for single-thread/openMP
+            #                    as this container is pre-allocated to speedup monitor readout.
+            stop_code = """
+    // Stop condition (any)
+    bool stop_condition() {
+        return (spike_count>0);
+    } """
+            return stop_code
+
+        elif pop.stop_condition.replace(" ", "") == "spiked:all":
+            stop_code = """
+    // Stop condition (all)
+    bool stop_condition() {
+        return spike_count == size;
+    } """
+            return stop_code
+
         # Process the stop condition
         pop.neuron_type.description['stop_condition'] = {'eq': pop.stop_condition}
         from ANNarchy.parser.Extraction import extract_stop_condition
         extract_stop_condition(pop.neuron_type.description)
 
         mem_transfer = ""
         for dep in pop.neuron_type.description['stop_condition']['dependencies']:
@@ -843,39 +825,31 @@
         Generate the execution code for updating neural variables, more precise local and global ones.
 
         The resulting code comprise of several parts: creating of local and global update code, generating
         function prototype and finally calling statement.
 
         Returns:
 
-            a tuple of three strings, comprising of:
-
-                * body:    kernel implementation
-                * header:  kernel prototypes
-                * call:    kernel call
+            * tuple of four code snippets (device_kernel, device_invoke, kernel_decl, host_call)
 
         """
-        # HD ( 18. Nov. 2016 )
-        #
-        # In some user-defined cases the host and device side need something to do to
-        # in order to realize specific functionality. Yet I simply add a update()
-        # call, if update_variables was set.
+        # Use pre-defined code template
         if 'update_variables' in pop._specific_template.keys():
-            call = """
-        // host side update of neurons
-        pop%(id)s.update();
-""" % {'id': pop.id}
-            return "", "", call
+            try:
+                return pop._specific_template['update_variable_body'], pop._specific_template['update_variable_invoke'], pop._specific_template['update_variable_header'], pop._specific_template['update_variable_call']
+            except KeyError:
+                Global._error("\nCode generation error: if one attempts to override the population update on CUDA devices, one need to define all of the following fields of _specific_template dictionary:\n\tupdate_variables, update_variable_call, update_variable_header, update_variable_invoke, update_variable_body")
 
         # Is there any variable?
         if len(pop.neuron_type.description['variables']) == 0:
-            return "", "", ""
+            return "", "", "", ""
 
-        header = ""
-        body = ""
+        device_kernel = ""
+        kernel_invoke = ""
+        kernel_decl = ""
         local_call = ""
         global_call = ""
 
         # some defaults
         ids = {
             'id': pop.id,
             'local_index': "[i]",
@@ -937,119 +911,131 @@
 
         # replace local function calls
         if len(pop.neuron_type.description['functions']) > 0:
             glob_eqs, loc_eqs = self._replace_local_funcs(pop, glob_eqs, loc_eqs)
 
         # Global operations
         if glob_eqs.strip() != '':
-            add_args_header, add_args_call = self._gen_kernel_args(pop, 'global')
+            add_args_header, add_args_invoke, add_args_call = self._gen_kernel_args(pop, 'global')
 
             for op in pop.global_operations:
                 ids = {
                     'id': pop.id,
                     'type': Global.config['precision'],
                     'op': op['function'],
                     'var': op['variable']
                 }
                 add_args_header += """, %(type)s _%(op)s_%(var)s """ % ids
                 add_args_call += """, pop%(id)s._%(op)s_%(var)s""" % ids
 
             # finalize code templates
-            body += CUDATemplates.population_update_kernel['global']['body'] % {
+            device_kernel += CUDATemplates.population_update_kernel['global']['device_kernel'] % {
                 'id': pop.id,
                 'add_args': add_args_header,
                 'global_eqs':glob_eqs,
                 'pre_loop': tabify(pre_loop, 1)
             }
-            header += CUDATemplates.population_update_kernel['global']['header'] % {
+            kernel_invoke += CUDATemplates.population_update_kernel['global']['invoke_kernel'] % {
+                'id': pop.id,
+                'add_args': add_args_header,
+                'add_args_call': add_args_invoke,
+            }
+            kernel_decl += CUDATemplates.population_update_kernel['global']['kernel_decl'] % {
                 'id': pop.id, 'add_args': add_args_header
             }
-            global_call = CUDATemplates.population_update_kernel['global']['call'] % {
+            global_call = CUDATemplates.population_update_kernel['global']['host_call'] % {
                 'id': pop.id, 'add_args': add_args_call
             }
 
         # Local variables
         if loc_eqs.strip() != '':
-            add_args_header, add_args_call = self._gen_kernel_args(pop, 'local')
+            add_args_header, add_args_invoke, add_args_call = self._gen_kernel_args(pop, 'local')
 
             # targets
             for target in sorted(list(set(pop.neuron_type.description['targets'] + pop.targets))):
                 add_args_header += """, %(type)s* _sum_%(target)s""" % {'type': Global.config['precision'], 'target' : target}
+                add_args_invoke += """, _sum_%(target)s""" % {'target' : target}
                 add_args_call += """, pop%(id)s.gpu__sum_%(target)s""" % {'id': pop.id, 'target' : target}
 
             # global operations
             for op in pop.global_operations:
                 ids = {
                     'id': pop.id,
                     'type': Global.config['precision'],
                     'op': op['function'],
                     'var': op['variable']
                 }
                 add_args_header += """, %(type)s _%(op)s_%(var)s """ % ids
+                add_args_invoke += """, _%(op)s_%(var)s """ % ids
                 add_args_call += """, pop%(id)s._%(op)s_%(var)s""" % ids
 
             # finalize code templates
-            body += CUDATemplates.population_update_kernel['local']['body'] % {
+            device_kernel += CUDATemplates.population_update_kernel['local']['device_kernel'] % {
                 'id': pop.id,
                 'add_args': add_args_header,
                 'pop_size': pop.size,
                 'local_eqs': loc_eqs,
                 'pre_loop': tabify(pre_loop, 1)
             }
-            header += CUDATemplates.population_update_kernel['local']['header'] % {
+            kernel_invoke += CUDATemplates.population_update_kernel['local']['invoke_kernel'] % {
+                'id': pop.id,
+                'add_args': add_args_header,
+                'add_args_call': add_args_invoke,
+            }
+            kernel_decl += CUDATemplates.population_update_kernel['local']['kernel_decl'] % {
                 'id': pop.id,
                 'add_args': add_args_header
             }
-            local_call = CUDATemplates.population_update_kernel['local']['call'] % {
+            local_call = CUDATemplates.population_update_kernel['local']['host_call'] % {
                 'id': pop.id,
                 'add_args': add_args_call
             }
 
         # Call statement consists of two parts
-        call = """
+        host_call = """
     // Updating the local and global variables of population %(id)s
     if ( pop%(id)s._active ) {
         %(global_call)s
 
         %(local_call)s
     }
 """ % {'id':pop.id, 'global_call': global_call, 'local_call': local_call}
 
         if self._prof_gen:
-            call = self._prof_gen.annotate_update_neuron(pop, call)
+            host_call = self._prof_gen.annotate_update_neuron(pop, host_call)
 
-        return body, header, call
+        return device_kernel, kernel_invoke, kernel_decl, host_call
 
     def _update_spiking_neuron(self, pop):
         """
         Generate the neural update code for GPU devices. We split up the
         calculation into three parts:
 
             * evolvement of global differential equations
             * evolvement of local differential equations
             * spike gathering
 
         Return:
 
-            * tuple of three code snippets (body, header, call)
+            * tuple of four code snippets (device_kernel, device_invoke, kernel_decl, host_call)
         """
-        # Is there any variable?
-        if len(pop.neuron_type.description['variables']) == 0:
-            return "", "", ""
-
-        # The purpose of this lines is explained in _update_rate_neuron
-        # HD: 19. May 2017
+        # Use pre-defined code template
         if 'update_variables' in pop._specific_template.keys():
             try:
-                return pop._specific_template['update_variable_body'], pop._specific_template['update_variable_header'], pop._specific_template['update_variable_call']
+                return pop._specific_template['update_variable_body'], pop._specific_template['update_variable_invoke'], pop._specific_template['update_variable_header'], pop._specific_template['update_variable_call']
             except KeyError:
-                Global._error("\nCode generation error: if one attempts to override the population update on CUDA devices, one need to define all of the following fields of _specific_template dictionary:\n\tupdate_variables, update_variable_call, update_variable_header, update_variable_body")
+                Global._error("\nCode generation error: if one attempts to override the population update on CUDA devices, one need to define all of the following fields of _specific_template dictionary:\n\tupdate_variables, update_variable_call, update_variable_header, update_variable_invoke, update_variable_body")
 
-        header = ""
-        body = ""
+        # Is there any variable?
+        if len(pop.neuron_type.description['variables']) == 0:
+            return "", "", "", ""
+
+        kernel_decl = ""
+        device_kernel = ""
+        device_invoke = ""
         local_call = ""
         global_call = ""
 
         # some defaults
         ids = {
             'id': pop.id,
             'local_index': "[i]",
@@ -1110,25 +1096,26 @@
 
         # replace local function calls
         if len(pop.neuron_type.description['functions']) > 0:
             glob_eqs, loc_eqs = self._replace_local_funcs(pop, glob_eqs, loc_eqs)
 
         # Global variables
         if glob_eqs.strip() != '':
-            add_args_header, add_args_call = self._gen_kernel_args(pop, 'global')
+            add_args_header, add_args_invoke, add_args_call = self._gen_kernel_args(pop, 'global')
 
             # global operations
             for op in pop.global_operations:
                 ids = {
                     'id': pop.id,
                     'type': Global.config['precision'],
                     'op': op['function'],
                     'var': op['variable']
                 }
                 add_args_header += """, %(type)s _%(op)s_%(var)s """ % ids
+                add_args_invoke += """, _%(op)s_%(var)s """ % ids
                 add_args_call += """, pop%(id)s._%(op)s_%(var)s""" % ids
 
             # finalize code templates
             body += CUDATemplates.population_update_kernel['global']['body'] % {
                 'id': pop.id,
                 'add_args': add_args_header,
                 'pre_loop': pre_code,
@@ -1139,25 +1126,26 @@
             }
             global_call = CUDATemplates.population_update_kernel['global']['call'] % {
                 'id': pop.id, 'add_args': add_args_call, 'stream_id': pop.id
             }
 
         # Local variables
         if loc_eqs.strip() != '':
-            add_args_header, add_args_call = self._gen_kernel_args(pop, 'local')
+            add_args_header, add_args_invoke, add_args_call = self._gen_kernel_args(pop, 'local')
 
             # global operations
             for op in pop.global_operations:
                 ids = {
                     'id': pop.id,
                     'type': Global.config['precision'],
                     'op': op['function'],
                     'var': op['variable']
                 }
                 add_args_header += """, %(type)s _%(op)s_%(var)s """ % ids
+                add_args_invoke += """, _%(op)s_%(var)s """ % ids
                 add_args_call += """, pop%(id)s._%(op)s_%(var)s""" % ids
 
             # Is there a refractory period?
             if pop.neuron_type.refractory or pop.refractory:
                 # 'old' loc_eqs is now only executed ouside refractory period
                 loc_eqs = """
         // Refractory period
@@ -1167,76 +1155,108 @@
             refractory_remaining[i]--;
         } else{
 %(loc_eqs)s
         }
 """ %  {'refr_eqs': refr_eqs, 'loc_eqs': loc_eqs}
 
                 add_args_header += ", int* refractory_remaining"
+                add_args_invoke += ", refractory_remaining"
                 add_args_call += """, pop%(id)s.gpu_refractory_remaining""" %{'id':pop.id}
 
             # finalize code templates
-            body += CUDATemplates.population_update_kernel['local']['body'] % {
+            device_kernel += CUDATemplates.population_update_kernel['local']['device_kernel'] % {
                 'id': pop.id, 'add_args': add_args_header, 'pop_size': pop.size, 'pre_loop': pre_code, 'local_eqs': loc_eqs
             }
-            header += CUDATemplates.population_update_kernel['local']['header'] % {
+            device_invoke += CUDATemplates.population_update_kernel['local']['invoke_kernel'] % {
+                'id': pop.id, 'add_args': add_args_header, 'add_args_call': add_args_invoke
+            }
+            kernel_decl += CUDATemplates.population_update_kernel['local']['kernel_decl'] % {
                 'id': pop.id, 'add_args': add_args_header
             }
-            local_call = CUDATemplates.population_update_kernel['local']['call'] % {
+            local_call = CUDATemplates.population_update_kernel['local']['host_call'] % {
                 'id': pop.id, 'add_args': add_args_call, 'stream_id': pop.id
             }
 
         # Call statement consists of two parts
-        call = """
+        host_call = """
     // Updating the local and global variables of population %(id)s
     if ( pop%(id)s._active ) {
         %(global_call)s
 
         %(local_call)s
     }
 """ % {'id':pop.id, 'global_call': global_call, 'local_call': local_call}
 
         if self._prof_gen:
-            call = self._prof_gen.annotate_update_neuron(pop, call)
+            host_call = self._prof_gen.annotate_update_neuron(pop, host_call)
+
+        return device_kernel, device_invoke, kernel_decl, host_call
+
+    def _spike_gather(self, pop):
+        """
+        Process the spike condition and generate the corresponding kernel including call code.
+
+        Returns: four separate strings containg:
+
+        *device_kernel*:    device code
+        *invoke_kernel*:    defice function invocation
+        *kernel_decl*:      header definition for invoke_kernel
+        *host_call*:        device function call
+        """
+        # some defaults
+        ids = {
+            'id': pop.id,
+            'local_index': "[i]",
+            'global_index': "[0]"
+        }
+
+        if 'spike_gather_body' in pop._specific_template.keys():
+            try:
+                return pop._specific_template['spike_gather_body'], pop._specific_template['spike_gather_invoke'], pop._specific_template['spike_gather_header'], pop._specific_template['spike_gather_call']
+            except KeyError:
+                Global._error("\nCode generation error: if one attempts to override the spike gathering on CUDA devices, one need to define all of the following fields of _specific_template dictionary: spike_gather_call, spike_gather_header, spike_gather_body")
 
-        #
-        # Process the spike condition and generate 2nd set of kernels
-        #
         cond = pop.neuron_type.description['spike']['spike_cond']
         reset = ""
         for eq in pop.neuron_type.description['spike']['spike_reset']:
             reset += """
             %(reset)s
 """ % {'reset': eq['cpp']}
 
         # arguments
         header_args = ""
+        header_invoke = ""
         call_args = ""
 
         # gather all attributes required by this kernel
         kernel_deps = []
         for var in pop.neuron_type.description['spike']['spike_cond_dependencies']:
             kernel_deps.append(var)
         for reset_eq in pop.neuron_type.description['spike']['spike_reset']:
             kernel_deps.append(reset_eq['name'])
             for var in reset_eq['dependencies']:
                 kernel_deps.append(var)
-        kernel_deps = list(set(kernel_deps)) # remove doubled entries
+
+        # remove doubled entries and sort to prevent unnecessary recompiles
+        kernel_deps = sorted(list(set(kernel_deps)))
 
         # generate header, call and body args
         for var in kernel_deps:
             attr_type, attr_dict = self._get_attr_and_type(pop, var)
 
             if attr_type == 'par' and attr_dict['locality'] == "global":
                 header_args += ", const " + attr_dict['ctype'] + " " + var
+                header_invoke += ", " + var
                 call_args += ", pop"+str(pop.id)+"."+var
 
                 cond = cond.replace(var+"%(global_index)s", var)
                 reset = reset.replace(var+"%(global_index)s", var)
             else:
-                header_args += ", "+attr_dict['ctype']+"* " + var
+                header_args += ", " + attr_dict['ctype'] + "* " + var
+                header_invoke += ", " + var
                 call_args += ", pop"+str(pop.id)+".gpu_"+var
 
         # Fill the templates with the correct ids
         cond = cond % ids
         reset = reset % ids
 
         # Is there a refractory period?
@@ -1255,66 +1275,74 @@
                         found = True
                         break
                 if not found:
                     Global._error("refractory = "+ pop.neuron_type.refractory + ": parameter or variable does not exist.")
 
                 refrac_inc = "refractory_remaining[i] = %(refrac_var)s;" % {'refrac_var': refrac_var}
                 header_args += ", %(type)s *%(name)s, int* refractory_remaining" % {'type': param['ctype'], 'name': param['name']}
+                header_invoke += ", %(name)s, refractory_remaining" % {'name': param['name']}
                 call_args += ", pop%(id)s.gpu_%(name)s, pop%(id)s.gpu_refractory_remaining" %{'id':pop.id, 'name': param['name']}
 
             else: # default case
                 refrac_inc = "refractory_remaining[i] = %(refrac_var)s;" % {'refrac_var': refrac_var}
                 header_args += ", int *refractory, int* refractory_remaining"
+                header_invoke += ", refractory, refractory_remaining"
                 call_args += """, pop%(id)s.gpu_refractory, pop%(id)s.gpu_refractory_remaining""" %{'id':pop.id}
         else:
             refrac_inc = ""
 
         # With ANNarchy 4.7.2 we introduced two different kernel:
         # a) single block (standard version prior to ANNarchy 4.7.2)
         # b) multiple blocks (new in ANNarchy 4.7.2)
         if pop.size < 32:
             launch_config = """int tpb = 32;\nint nb_blocks = 1;\n"""
         else:
             launch_config = """int tpb = 32;\nint nb_blocks = %(nb)s;\n""" % {'nb': int(min(65535, float(pop.size)/32.0))}
         launch_config = tabify(launch_config, 2)
 
-        body += CUDATemplates.spike_gather_kernel['body'] % {
+        device_kernel = CUDATemplates.spike_gather_kernel['device_kernel'] % {
             'id': pop.id,
             'pop_size': str(pop.size),
-            'default': 'const long int t, const %(float_prec)s dt, int* spiked, long int* last_spike' % {'float_prec': Global.config['precision']},
+            'float_prec': Global.config['precision'],
             'args': header_args,
             'cond': cond,
             'reset': reset,
             'refrac_inc': refrac_inc
         }
 
-        header += CUDATemplates.spike_gather_kernel['header'] % {
+        invoke_kernel = CUDATemplates.spike_gather_kernel['invoke_kernel'] % {
+            'id': pop.id,
+            'float_prec': Global.config['precision'],
+            'args': header_args,
+            'args_call': header_invoke
+        }
+
+        kernel_decl = CUDATemplates.spike_gather_kernel['kernel_decl'] % {
             'id': pop.id,
             'default': 'const long int t, const %(float_prec)s dt, int* spiked, long int* last_spike' % {'float_prec': Global.config['precision']},
             'args': header_args
         }
 
         if pop.max_delay > 1:
             default_args = 't, dt, pop%(id)s.gpu_delayed_spiked.front(), pop%(id)s.gpu_last_spike' % {'id': pop.id}
         else: # no_delay
             default_args = 't, dt, pop%(id)s.gpu_spiked, pop%(id)s.gpu_last_spike' % {'id': pop.id}
 
-        spike_gather = CUDATemplates.spike_gather_kernel['call'] % {
+        host_call = CUDATemplates.spike_gather_kernel['host_call'] % {
             'id': pop.id,
             'default': default_args,
             'args': call_args % {'id': pop.id},
             'stream_id': pop.id,
             'launch_config': launch_config
         }
 
         if self._prof_gen:
-            spike_gather = self._prof_gen.annotate_spike_gather(pop, spike_gather)
-        call += spike_gather
+            host_call = self._prof_gen.annotate_spike_gather(pop, host_call)
 
-        return body, header, call
+        return device_kernel, invoke_kernel, kernel_decl, host_call
 
     def _memory_transfers(self, pop):
         """
         Before evaluation neuron/synaptic equations we need to update the data
         on the GPU. To synchronize the states of variables after simulation of
         several steps, we need to transfer variables back to the host.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/CUDATemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/CUDATemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CUDATemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 population_header = """/*
  *  ANNarchy-version: %(annarchy_version)s
  */
  #pragma once
 #include "ANNarchy.h"
 
 // host defines
@@ -143,15 +125,15 @@
     void device_to_host() {
 %(device_to_host)s
     }
 
     // Memory Management: track memory consumption
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     // Memory Management: clear container
     void clear() {
 %(clear_container)s
     }
@@ -572,14 +554,26 @@
         cudaMemcpy(gpu_spike_count, &spike_count, sizeof(unsigned int), cudaMemcpyHostToDevice);
 """,
         'reset': """
         spiked = std::vector<int>(size, 0);
         last_spike.clear();
         last_spike = std::vector<long int>(size, -10000L);
         spike_count = 0;
+""",
+        'clear': """
+// Spike events (host-side)
+spiked.clear();
+spiked.shrink_to_fit();
+
+last_spike.clear();
+last_spike.shrink_to_fit();
+
+// Spike events (device-side)
+cudaFree(gpu_spiked);
+cudaFree(gpu_last_spike);
 """
     },
     'refractory': {
         'declare': """
     // Refractory period
     std::vector<int> refractory;
     int *gpu_refractory;
@@ -625,74 +619,90 @@
         last_spike = std::vector<long int>(size, -10000L);
 """
 }
 
 # Contains all codes related to the population update
 #
 # 1st level distinguish 'local' and 'global' update
-# 2nd level distinguish 'body', 'header' and 'call' template
+# 2nd level distinguish 'device_kernel', 'invoke_kernel', 'header' and 'host_call' template
 population_update_kernel = {
     'global': {
-        'body': """// Updating global variables of population %(id)s
+        'device_kernel': """// Updating global variables of population %(id)s
 __global__ void cuPop%(id)s_global_step( %(add_args)s )
 {
 %(pre_loop)s
 
 %(global_eqs)s
 }
 """,
-        'header': "__global__ void cuPop%(id)s_global_step( %(add_args)s );\n",
-        'call': """
-        cuPop%(id)s_global_step<<< 1, 1, 0, pop%(id)s.stream >>>( %(add_args)s );
+        'invoke_kernel': """void pop%(id)s_global_step(RunConfig cfg, %(add_args)s ) {
+    cuPop%(id)s_global_step<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        // arguments
+        %(add_args_call)s
+    );
+}""",
+        'kernel_decl': """void pop%(id)s_global_step(RunConfig cfg, %(add_args)s );
+""",
+        'host_call': """
+        pop%(id)s_global_step(RunConfig(1, 1, 0, pop%(id)s.stream), %(add_args)s );
     #ifdef _DEBUG
         cudaError_t err_pop%(id)s_global_step = cudaGetLastError();
         if( err_pop%(id)s_global_step != cudaSuccess) {
             std::cout << "pop%(id)s_step: " << cudaGetErrorString(err_pop%(id)s_global_step) << std::endl;
             exit(0);
         }
     #endif
 """
     },
     'local': {
-        'body': """// Updating local variables of population %(id)s
+        'device_kernel': """// Updating local variables of population %(id)s
 __global__ void cuPop%(id)s_local_step( %(add_args)s )
 {
     int i = threadIdx.x + blockDim.x * blockIdx.x;
 %(pre_loop)s
 
     while ( i < %(pop_size)s )
     {
 %(local_eqs)s
 
         i += blockDim.x * gridDim.x;
     }
 }
 """,
-        'header': "__global__ void cuPop%(id)s_local_step( %(add_args)s );\n",
-        'call': """
+        'invoke_kernel': """
+void pop%(id)s_local_step(RunConfig cfg, %(add_args)s ) {
+    cuPop%(id)s_local_step<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        // arguments
+        %(add_args_call)s
+    );
+}
+""",
+        'kernel_decl': "void pop%(id)s_local_step(RunConfig cfg, %(add_args)s );\n",
+        'host_call': """
     #if defined (__pop%(id)s_nb__)
-        cuPop%(id)s_local_step<<< __pop%(id)s_nb__, __pop%(id)s_tpb__, 0, pop%(id)s.stream >>>( %(add_args)s );
+        pop%(id)s_local_step(RunConfig(__pop%(id)s_nb__, __pop%(id)s_tpb__, 0, pop%(id)s.stream), %(add_args)s );
     #else
-        cuPop%(id)s_local_step<<< pop%(id)s._nb_blocks, pop%(id)s._threads_per_block, 0, pop%(id)s.stream >>>( %(add_args)s );
+        pop%(id)s_local_step(RunConfig(pop%(id)s._nb_blocks, pop%(id)s._threads_per_block, 0, pop%(id)s.stream), %(add_args)s );
     #endif
+
     #ifdef _DEBUG
         cudaError_t err_pop%(id)s_local_step = cudaGetLastError();
         if( err_pop%(id)s_local_step != cudaSuccess) {
             std::cout << "pop%(id)s_step: " << cudaGetErrorString(err_pop%(id)s_local_step) << std::endl;
             exit(0);
         }
     #endif
 """
     }
 }
 
 spike_gather_kernel = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for population %(id)s
-__global__ void cuPop%(id)s_spike_gather( unsigned int* num_events, %(default)s%(args)s )
+__global__ void cu_pop%(id)s_spike_gather( unsigned int* num_events, const long int t, const %(float_prec)s dt, int* spiked, long int* last_spike%(args)s )
 {
     int i = blockIdx.x * blockDim.x + threadIdx.x;
     __shared__ int local_spiked[32];
     __shared__ int num_local_events[1];
     num_local_events[0] = 0;
     __syncthreads();
 
@@ -719,35 +729,50 @@
             num_local_events[0] = 0;
         }
         __syncthreads();
         i += gridDim.x * blockDim.x;
     }
 }
 """,
-    'header': """
-__global__ void cuPop%(id)s_spike_gather( unsigned int* num_events, %(default)s%(args)s );
+    'invoke_kernel': """
+void pop%(id)s_spike_gather(RunConfig cfg, unsigned int* num_events, const long int t, const %(float_prec)s dt, int* spiked, long int* last_spike%(args)s ) {
+    // Compute current events
+    cu_pop%(id)s_spike_gather<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        /* default arguments */
+        num_events, t, dt, spiked, last_spike
+        /* other variables */
+        %(args_call)s
+    );
+}
+""",
+    'kernel_decl': """
+void pop%(id)s_spike_gather(RunConfig cfg, unsigned int* num_events, %(default)s%(args)s );
 """,
     # As we use atomicAdd operations, multiple blocks are not
     # working correctly, consequently spawn only one block.
-    'call': """
+    'host_call': """
     // Check if neurons emit a spike in population %(id)s
     if ( pop%(id)s._active ) {
         // Reset old events
-        clear_num_events<<< 1, 1, 0, pop%(id)s.stream >>>(pop%(id)s.gpu_spike_count);
+        call_clear_num_events(RunConfig(1, 1, 0, pop%(id)s.stream), pop%(id)s.gpu_spike_count);
 
         // launch configuration
 %(launch_config)s
 
         // Compute current events
-        cuPop%(id)s_spike_gather<<< nb_blocks, tpb, 0, pop%(id)s.stream >>>(
-              pop%(id)s.gpu_spike_count,
-              /* default arguments */
-              %(default)s
-              /* other variables */
-              %(args)s );
+        pop%(id)s_spike_gather(
+            /* kernel config */
+            RunConfig(nb_blocks, tpb, 0, pop%(id)s.stream),
+            /* number of emeitted events (return value) */
+            pop%(id)s.gpu_spike_count,
+            /* default arguments */
+            %(default)s
+            /* other variables */
+            %(args)s
+        );
 
     #ifdef _DEBUG
         cudaError_t err_pop_spike_gather_%(id)s = cudaGetLastError();
         if(err_pop_spike_gather_%(id)s != cudaSuccess)
             std::cout << "pop%(id)s_spike_gather: " << cudaGetErrorString(err_pop_spike_gather_%(id)s) << std::endl;
     #endif
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/OpenMPGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/OpenMPGenerator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,12 @@
-#===============================================================================
-#
-#     OpenMPGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
-import datetime
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from copy import deepcopy
 
 import ANNarchy
 
 from ANNarchy.generator.Template.GlobalOperationTemplate import global_operation_templates_omp_extern as global_op_extern_dict
 from ANNarchy.generator.Utils import generate_equation_code, tabify, remove_trailing_spaces
 from ANNarchy.core import Global
@@ -126,15 +107,15 @@
             update_variables = self._update_spiking_neuron(pop)
             test_spike_cond = self._spike_gather(pop)
 
         # Stop condition
         stop_condition = self._stop_condition(pop)
 
         # Memory management
-        determine_size_in_bytes = self._determine_size_in_bytes(pop)
+        size_in_bytes = self._size_in_bytes(pop)
         clear_container = self._clear_container(pop)
 
         # Profiling
         if self._prof_gen:
             include_profile = """#include "Profiling.h"\n"""
             declare_profile, init_profile = self._prof_gen.generate_init_population(pop)
         else:
@@ -190,15 +171,14 @@
         if 'update_global_ops' in pop._specific_template.keys():
             update_global_ops = pop._specific_template['update_global_ops']
 
         # Fill the template
         code = self._templates['population_header'] % {
             # version tag
             'annarchy_version': ANNarchy.__release__,
-            #'time_stamp': '{:%Y-%b-%d %H:%M:%S}'.format(datetime.datetime.now()),
             # fill code templates
             'float_prec': Global.config['precision'],
             'id': pop.id,
             'name': pop.name,
             'size': pop.size,
             'include_additional': include_additional,
             'include_profile': include_profile,
@@ -224,15 +204,15 @@
             'update_variables': update_variables,
             'test_spike_cond': test_spike_cond,
             'update_rng': update_rng,
             'update_delay': update_delay,
             'update_max_delay': update_max_delay,
             'update_global_ops': update_global_ops,
             'stop_condition': stop_condition,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container
         }
 
         # remove right-trailing spaces
         code = remove_trailing_spaces(code)
 
         # Store the complete header definition in a single file
@@ -266,50 +246,14 @@
             pop_desc['delay_update'] = tabify("""pop%(id)s.update_delay();\n""" % {'id': pop.id}, 1)
 
         if len(pop.global_operations) > 0:
             pop_desc['gops_update'] = """\tpop%(id)s.update_global_ops(tid, nt);\n""" % {'id': pop.id}
 
         return pop_desc
 
-    def _clear_container(self, pop):
-        """
-        Generate code template to destroy allocated container of the C++ object *pop*.
-
-        User defined elements, parallelization support data structures or similar are not considered. Consequently
-        implementing generators should extent the resulting code template.
-        """
-        from ANNarchy.generator.Utils import tabify
-        code = ""
-
-        # Variables
-        code += "// Variables\n"
-        for attr in pop.neuron_type.description['variables']:
-            # HD: we need to clear only local variables, the others are no vectors
-            if attr['locality'] == "local":
-                # HD: clear alone does not deallocate, it only resets size.
-                #     So we need to call shrink_to_fit afterwards.
-                ids = {'ctype': attr['ctype'], 'name': attr['name']}
-                code += "%(name)s.clear();\n" % ids
-                code += "%(name)s.shrink_to_fit();\n" % ids
-
-        # Mean-FR
-        if pop.neuron_type.description['type'] == 'spike':
-            code += """
-// Mean Firing Rate
-for (auto it = _spike_history.begin(); it != _spike_history.end(); it++) {
-    while(!it->empty())
-        it->pop();
-}
-_spike_history.clear();
-_spike_history.shrink_to_fit();
-"""
-
-        code = tabify(code, 2)
-        return code
-
     ##################################################
     # Reset compute sums
     ##################################################
     def reset_computesum(self, pop):
         """
         For rate-coded neurons each step the weighted sum of inputs is computed. The implementation
         codes of the computes_rate kernel expect zeroed arrays. The same applies for the AccProjections
@@ -465,14 +409,31 @@
         dependent on a population related condition. The code for
         this is generated here and added to the ANNarchy.cpp/.cu
         file.
         """
         if not pop.stop_condition: # no stop condition has been defined
             return ""
 
+        # Special case for early return based on emitted events
+        if pop.stop_condition.replace(" ", "") == "spiked:any":
+            stop_code = """
+    // Stop condition (any)
+    bool stop_condition() {
+        return !spiked.empty();
+    } """
+            return stop_code
+
+        elif pop.stop_condition.replace(" ", "") == "spiked:all":
+            stop_code = """
+    // Stop condition (all)
+    bool stop_condition() {
+        return spiked.size() == size;
+    } """
+            return stop_code
+
         # Process the stop condition
         pop.neuron_type.description['stop_condition'] = {'eq': pop.stop_condition}
         from ANNarchy.parser.Extraction import extract_stop_condition
         extract_stop_condition(pop.neuron_type.description)
 
         # Retrieve the code
         condition = pop.neuron_type.description['stop_condition']['cpp']% {
@@ -754,19 +715,22 @@
         # Local variables, evaluated in parallel
         eqs = generate_equation_code(
             pop.id, pop.neuron_type.description, 'local', padding=4)
         eqs = eqs % id_dict
         if eqs.strip() != "":
             code += """
             // Updating the local variables
-            #pragma omp for simd
+            %(omp_code)s
             for (int i = 0; i < size; i++) {
 %(eqs)s
             }
-""" % {'eqs': eqs}
+""" % {
+    'omp_code': "#pragma omp for simd" if not Global.config["disable_SIMD_Eq"] else "#pragma omp for",
+    'eqs': eqs
+}
 
         # finish code
         final_code = """
         if( _active ) {
 %(code)s
         } // active
 """ % {'code': code}
@@ -853,21 +817,22 @@
         final_eq = """
         if( _active ) {
 %(comp_inref)s
 
 %(global_code)s
 
             // Updating local variables
-            #pragma omp for simd
+            %(omp_code)s
             for (int i = 0; i < size; i++) {
 %(local_code)s
             }
 
         } // active
 """ % {
+    'omp_code': "#pragma omp for simd" if not Global.config["disable_SIMD_Eq"] else "#pragma omp for",
     'comp_inref': comp_inref,
     'local_code': local_code,
     'global_code': global_code,
     }
 
         # if profiling enabled, annotate with profiling code
         if self._prof_gen:
@@ -978,22 +943,16 @@
         # If a population is too small, the overhead of local arrays and
         # fusion afterwards would be to high.
         if pop.size > Global.OMP_MIN_NB_NEURONS:
             mean_FR_update = tabify(mean_FR_update,1)
 
             gather_code = """
         if ( _active ) {
-            #pragma omp master
-            {
-                spiked.clear();
-            }
             auto local_spikes = std::vector<int>();
 
-            #pragma omp barrier
-
             #pragma omp for nowait
             for (int i = 0; i < size; i++) {
 %(refrac_check)s
 
                 // Spike emission
                 if( %(condition)s ) { // Condition is met
                     // Reset variables
@@ -1014,21 +973,44 @@
         %(mean_FR_update)s
 
             local_spiked_sizes[tid+1] = local_spikes.size();
             #pragma omp barrier
 
             #pragma omp single
             {
+            #ifdef _DEBUG_SPIKE_GATHER
+                std::cout << "time step - " << t << ": ";
+                for (auto it = local_spiked_sizes.begin(); it != local_spiked_sizes.end(); it++) {
+                    std::cout << *it << ", ";
+                }
+                std::cout << " --> ";
+            #endif
+
+                // compute storage offsets
                 for (int i = 1; i < (global_num_threads+1); i++) {
                     local_spiked_sizes[i] += local_spiked_sizes[i-1];
                 }
-                spiked.resize(spiked.size()+local_spiked_sizes[global_num_threads]);
-            }
 
-            std::copy(local_spikes.begin(), local_spikes.end(), spiked.begin() + local_spiked_sizes[tid]);
+            #ifdef _DEBUG_SPIKE_GATHER
+                for (auto it = local_spiked_sizes.begin(); it != local_spiked_sizes.end(); it++) {
+                    std::cout << *it << ", ";
+                }
+            #endif
+
+                // set the result container to the correct size
+                spiked.resize(local_spiked_sizes[global_num_threads]);
+
+            #ifdef _DEBUG_SPIKE_GATHER
+                std::cout << "(" << std::to_string(static_cast<long long>(spiked.size())) << " events)" << std::endl;
+            #endif
+            } // implicit barrier
+
+            // each thread computes it local data to the shared container
+            if (!local_spikes.empty())
+                std::copy(local_spikes.begin(), local_spikes.end(), spiked.begin() + local_spiked_sizes[tid]);
         } // active
 """
         else:
             gather_code = """
         if ( _active ) {
         #pragma omp single
         {
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/OpenMPTemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/OpenMPTemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-#===============================================================================
-#
-#     OpenMPTemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
-
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Definition of a population as a c-like struct, divided
 # into two groups: rate or spike
 #
 # Parameters:
 #
 #    id: id of the population
@@ -143,15 +123,15 @@
     }
 
     %(stop_condition)s
 
     // Memory management: track the memory consumption
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     // Memory management: track the memory consumption
     void clear() {
 %(clear_container)s
     }
@@ -364,39 +344,41 @@
 #    rd_name:
 #    rd_update:
 cpp_11_rng = {
     'dist_decl': "auto dist_%(rd_name)s = %(rd_init)s;",
     'local': {
         'decl': "std::vector<%(type)s> %(rd_name)s ;",
         'init': "%(rd_name)s = std::vector<%(type)s>(size, 0.0);",
-        'update': "%(rd_name)s[i] = dist_%(rd_name)s(rng[%(index)s]);"
+        'update': "%(rd_name)s[i] = dist_%(rd_name)s(rng[%(index)s]);",
+        'clear': "%(rd_name)s.clear();\n%(rd_name)s.shrink_to_fit();"
     },
     'global': {
         'decl': "%(type)s %(rd_name)s;",
         'init': "%(rd_name)s = 0.0;",
-        'update': "%(rd_name)s = dist_%(rd_name)s(rng[0]);"
+        'update': "%(rd_name)s = dist_%(rd_name)s(rng[0]);",
+        'clear': ""
     },
     'omp_code_seq': """
         if (_active){
 
             #pragma omp single
             {
 %(rng_dist)s
 %(update_rng_global)s
 %(update_rng_local)s
             }
         }
     """,
     'omp_code_par': """
         if (_active){
-%(rng_dist)s            
+%(rng_dist)s
 %(update_rng_global)s
 %(update_rng_local)s
         }
-    """     
+    """
 }
 
 rate_psp = {
     'decl': """
     std::vector<%(float_prec)s> _sum_%(target)s;""",
     'init': """
         // Post-synaptic potential
@@ -427,14 +409,22 @@
 """,
         'reset': """
         spiked.clear();
         spiked.shrink_to_fit();
         local_spiked_sizes = std::vector<int>(global_num_threads+1, 0);
         last_spike.clear();
         last_spike = std::vector<long int>(size, -10000L);
+""",
+        'clear': """
+// Spike events
+spiked.clear();
+spiked.shrink_to_fit();
+
+last_spike.clear();
+last_spike.shrink_to_fit();
 """
     },
     'axon_spike': {
         'declare': """
     // Structures for managing axonal spikes
     std::vector<int> axonal;
 """,
@@ -445,15 +435,15 @@
         'reset': """
         axonal.clear();
         axonal.shrink_to_fit();
 """,
         'pyx_wrapper': """
     # Axonal spike events
 """
-    },    
+    },
     'refractory': {
 
         'declare': """
     // Refractory period
     std::vector<int> refractory;
     std::vector<int> refractory_remaining;
     std::vector<short int> in_ref;
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/PopulationGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/PopulationGenerator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     PopulationGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 from ANNarchy.generator.Utils import tabify
 
 class PopulationGenerator(object):
     """
     Base class for population generators in ANNarchy. Inherited by
 
@@ -346,17 +328,72 @@
         """
         Generate code template to destroy allocated container of the C++ object *pop*. Should be implemented by child
         class.
 
         User defined elements, parallelization support data structures or similar are not considered. Consequently
         implementing generators should extent the resulting code template.
         """
-        raise NotImplementedError
+        from ANNarchy.generator.Utils import tabify
+        code = """
+    #ifdef _DEBUG
+        std::cout << "PopStruct%(id)s::clear()" << std::endl;
+    #endif
+""" % {'id': pop.id}
+
+       # Variables
+        code += "// Parameters\n"
+        for attr in pop.neuron_type.description['parameters']:
+            # HD: we need to clear only local parameters, the others are no vectors
+            if attr['locality'] == "local":
+                # HD: clear alone does not deallocate, it only resets size.
+                #     So we need to call shrink_to_fit afterwards.
+                ids = {'ctype': attr['ctype'], 'name': attr['name']}
+                code += "%(name)s.clear();\n" % ids
+                code += "%(name)s.shrink_to_fit();\n" % ids
+        code+="\n"
+
+        # Variables
+        code += "// Variables\n"
+        for attr in pop.neuron_type.description['variables']:
+            # HD: we need to clear only local variables, the others are no vectors
+            if attr['locality'] == "local":
+                # HD: clear alone does not deallocate, it only resets size.
+                #     So we need to call shrink_to_fit afterwards.
+                ids = {'ctype': attr['ctype'], 'name': attr['name']}
+                code += "%(name)s.clear();\n" % ids
+                code += "%(name)s.shrink_to_fit();\n" % ids
+
+        # Spike-specific code
+        if pop.neuron_type.description['type'] == 'spike':
+            code += self._templates['spike_specific']['spike']['clear']
+
+            # Mean - FR
+            code += """
+// Mean Firing Rate
+for (auto it = _spike_history.begin(); it != _spike_history.end(); it++) {
+    while(!it->empty())
+        it->pop();
+}
+_spike_history.clear();
+_spike_history.shrink_to_fit();
+"""
+
+        # Random variables
+        code += "\n// RNGs\n"
+        for dist in pop.neuron_type.description['random_distributions']:
+            rng_ids = {
+                'id': pop.id,
+                'rd_name': dist['name'],
+            }
+            code += self._templates['rng'][dist['locality']]['clear'] % rng_ids
+
+        code = tabify(code, 2)
+        return code
 
-    def _determine_size_in_bytes(self, pop):
+    def _size_in_bytes(self, pop):
         """
         Generate code template to determine size in bytes for the C++ object *pop*. Please note, that this contain only
         default elements (parameters, variables). User defined elements, parallelization support data structures or
         similar are not considered.
 
         Consequently implementing generators should extent the resulting code template. This is done by filling the
         'size_in_bytes' field in the _specific_template.
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/SingleThreadGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/SingleThreadGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,12 @@
-#===============================================================================
-#
-#     SingleThreadGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
-import datetime
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from copy import deepcopy
 
 import ANNarchy
 
 from ANNarchy.generator.Template.GlobalOperationTemplate import global_operation_templates_st_extern as global_op_extern_dict
 from ANNarchy.generator.Utils import generate_equation_code, tabify, remove_trailing_spaces
 from ANNarchy.core import Global
@@ -126,15 +107,15 @@
             update_variables = self._update_spiking_neuron(pop)
             test_spike_cond = self._spike_gather(pop)
 
         # Stop condition
         stop_condition = self._stop_condition(pop)
 
         # Memory management
-        determine_size_in_bytes = self._determine_size_in_bytes(pop)
+        size_in_bytes = self._size_in_bytes(pop)
         clear_container = self._clear_container(pop)
 
         # Profiling
         if self._prof_gen:
             include_profile = """#include "Profiling.h"\n"""
             declare_profile, init_profile = self._prof_gen.generate_init_population(pop)
         else:
@@ -223,15 +204,15 @@
             'update_variables': update_variables,
             'test_spike_cond': test_spike_cond,
             'update_rng': update_rng,
             'update_delay': update_delay,
             'update_max_delay': update_max_delay,
             'update_global_ops': update_global_ops,
             'stop_condition': stop_condition,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container
         }
 
         # remove right-trailing spaces
         code = remove_trailing_spaces(code)
 
         # Store the complete header definition in a single file
@@ -264,47 +245,14 @@
             pop_desc['delay_update'] = """\tpop%(id)s.update_delay();\n""" % {'id': pop.id}
 
         if len(pop.global_operations) > 0:
             pop_desc['gops_update'] = """\tpop%(id)s.update_global_ops();\n""" % {'id': pop.id}
 
         return pop_desc
 
-    def _clear_container(self, pop):
-        """
-        Generate code template to destroy allocated container of the C++ object *pop*.
-        """
-        from ANNarchy.generator.Utils import tabify
-        code = ""
-
-        # Variables
-        code += "// Variables\n"
-        for attr in pop.neuron_type.description['variables']:
-            # HD: we need to clear only local variables, the others are no vectors
-            if attr['locality'] == "local":
-                # HD: clear alone does not deallocate, it only resets size.
-                #     So we need to call shrink_to_fit afterwards.
-                ids = {'ctype': attr['ctype'], 'name': attr['name']}
-                code += "%(name)s.clear();\n" % ids
-                code += "%(name)s.shrink_to_fit();\n" % ids
-
-        # Mean-FR
-        if pop.neuron_type.description['type'] == 'spike':
-            code += """
-// Mean Firing Rate
-for (auto it = _spike_history.begin(); it != _spike_history.end(); it++) {
-    while(!it->empty())
-        it->pop();
-}
-_spike_history.clear();
-_spike_history.shrink_to_fit();
-"""
-
-        code = tabify(code, 2)
-        return code
-
     ##################################################
     # Reset compute sums
     ##################################################
     def reset_computesum(self, pop):
         """
         For rate-coded neurons each step the weighted sum of inputs is computed. The implementation
         codes of the computes_rate kernel expect zeroed arrays. The same applies for the AccProjections
@@ -453,14 +401,31 @@
         dependent on a population related condition. The code for
         this is generated here and added to the ANNarchy.cpp/.cu
         file.
         """
         if not pop.stop_condition: # no stop condition has been defined
             return ""
 
+        # Special case for early return based on emitted events
+        if pop.stop_condition.replace(" ", "") == "spiked:any":
+            stop_code = """
+    // Stop condition (any)
+    bool stop_condition() {
+        return !spiked.empty();
+    } """
+            return stop_code
+
+        elif pop.stop_condition.replace(" ", "") == "spiked:all":
+            stop_code = """
+    // Stop condition (all)
+    bool stop_condition() {
+        return spiked.size() == size;
+    } """
+            return stop_code
+
         # Process the stop condition
         pop.neuron_type.description['stop_condition'] = {'eq': pop.stop_condition}
         from ANNarchy.parser.Extraction import extract_stop_condition
         extract_stop_condition(pop.neuron_type.description)
 
         # Retrieve the code
         condition = pop.neuron_type.description['stop_condition']['cpp']% {
@@ -781,20 +746,21 @@
         # finish code
         final_eq = """
         if( _active ) {
 %(comp_inref)s
 
 %(global_code)s
             // Updating local variables
-            #pragma omp simd
+            %(omp_simd)s
             for(int i = 0; i < size; i++){
 %(local_code)s
             }
         } // active
 """ % {
+    'omp_simd': "#pragma omp simd" if not Global.config["disable_SIMD_Eq"] else "",
     'comp_inref': comp_inref,
     'local_code': local_code,
     'global_code': global_code
     }
 
         # if profiling enabled, annotate with profiling code
         if self._prof_gen:
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Population/SingleThreadTemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Population/SingleThreadTemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,11 @@
-#===============================================================================
-#
-#     SingleThreadTemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
-
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Definition of a population as a c-like struct, divided
 # into two groups: rate or spike
 #
 # Parameters:
 #
 #    id: id of the population
@@ -129,15 +109,15 @@
     }
 
     %(stop_condition)s
 
     // Memory management: track the memory consumption
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     // Memory management: destroy all the C++ data
     void clear() {
 #ifdef _DEBUG
     std::cout << "PopStruct%(id)s::clear() - this = " << this << std::endl;
@@ -345,30 +325,32 @@
 #    rd_name:
 #    rd_update:
 cpp_11_rng = {
     'dist_decl': "auto dist_%(rd_name)s = %(rd_init)s;",
     'local': {
         'decl': "std::vector<%(type)s> %(rd_name)s ;",
         'init': "%(rd_name)s = std::vector<%(type)s>(size, 0.0);",
-        'update': "%(rd_name)s[i] = dist_%(rd_name)s(rng[%(index)s]);"
+        'update': "%(rd_name)s[i] = dist_%(rd_name)s(rng[%(index)s]);",
+        'clear': "%(rd_name)s.clear();\n%(rd_name)s.shrink_to_fit();"
     },
     'global': {
         'decl': "%(type)s %(rd_name)s;",
         'init': "%(rd_name)s = 0.0;",
-        'update': "%(rd_name)s = dist_%(rd_name)s(rng[0]);"
+        'update': "%(rd_name)s = dist_%(rd_name)s(rng[0]);",
+        'clear': ""
     },
     'update': """
         if (_active) {
 %(rng_dist)s
 %(update_rng_global)s
             for(int i = 0; i < size; i++) {
 %(update_rng_local)s
             }
         }
-    """     
+    """
 }
 
 rate_psp = {
     'decl': """
     std::vector<%(float_prec)s> _sum_%(target)s;""",
     'init': """
         // Post-synaptic potential
@@ -393,14 +375,22 @@
         last_spike = std::vector<long int>(size, -10000L);
 """,
         'reset': """
         // Spiking variables
         spiked.clear();
         spiked.shrink_to_fit();
         std::fill(last_spike.begin(), last_spike.end(), -10000L);
+""",
+        'clear': """
+// Spike events
+spiked.clear();
+spiked.shrink_to_fit();
+
+last_spike.clear();
+last_spike.shrink_to_fit();
 """
     },
     'axon_spike': {
         'declare': """
     // Structures for managing axonal spikes
     std::vector<int> axonal;
 """,
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Profile/CPP11Profile.py` & `ANNarchy-4.7.3/ANNarchy/generator/Profile/CPP11Profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CPP11Profile.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 from ANNarchy.generator.Utils import tabify
 
 from .ProfileGenerator import ProfileGenerator
 from .ProfileTemplate import profile_base_template, cpp11_profile_template, cpp11_omp_profile_template, cpp11_profile_header
 
 class CPP11Profile(ProfileGenerator):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Profile/CUDAProfile.py` & `ANNarchy-4.7.3/ANNarchy/generator/Profile/CUDAProfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CUDAProfile.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 
 from .ProfileGenerator import ProfileGenerator
 from .ProfileTemplate import profile_base_template, cuda_profile_template, cuda_profile_header
 
 class CUDAProfile(ProfileGenerator):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Profile/PAPIProfile.py` & `ANNarchy-4.7.3/ANNarchy/generator/Profile/PAPIProfile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     PAPIProfile.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 
 from .ProfileGenerator import ProfileGenerator
 from .ProfileTemplate import profile_base_template, papi_profile_template, papi_profile_header
 
 class PAPIProfile(ProfileGenerator):
     """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Profile/ProfileTemplate.py` & `ANNarchy-4.7.3/ANNarchy/generator/Profile/ProfileTemplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     ProfileTemplate.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================papi_profile_header=\
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 profile_base_template = """#pragma once
 
 #include <memory>
 #include <iostream>
 #include <string>
 #include <vector>
 #include <map>
@@ -419,16 +401,17 @@
 
     inline void start_wall_time() {
         _start = std::chrono::steady_clock::now();
     }
 
     inline void stop_wall_time() {
         _stop = std::chrono::steady_clock::now();
-        std::chrono::duration<float> dur = _stop - _start;
-        _raw_data.push_back( dur.count() * 1000 * 1000); // duration is in sec
+        std::chrono::duration<double, std::milli> dur = _stop - _start;
+        // The measured times are stored in seconds
+        _raw_data.push_back(std::chrono::duration<double>(dur).count());
     }
 
     void reset() {
         debug_cout("Reset Measurement object");
         _raw_data.clear();
         _mean = 0.0;
         _std = 0.0;
@@ -783,15 +766,16 @@
     inline void stop_wall_time() {
         cudaEventRecord(_stop);
 
         cudaEventSynchronize(_stop);
         float milliseconds = 0;
         cudaEventElapsedTime(&milliseconds, _start, _stop);
 
-        _raw_data.push_back(double(milliseconds*1000.0)); // storage in us
+         // The measured times are stored in seconds
+        _raw_data.push_back(double(milliseconds/1000.0));
     }
 
     void reset() {
         debug_cout("Reset Measurement object");
         _raw_data.clear();
         _mean = 0.0;
         _std = 0.0;
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/BSR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/BSR.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-#===============================================================================
-#
-#     BSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020-21  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
 additional_global_functions = ""
 
 launch_config = {
     'init': """
@@ -231,21 +213,22 @@
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
             %(name)s_device_to_host = t;
         }
 """
 }
 
-#   BSR implementation following Eberhardt & Hoemmen (2016) - row-per-thread
+# BSR implementation following Eberhardt & Hoemmen (2016) - row-per-thread
+#
+# In this variant, each thread computes one row in a dense block and is intended for larger block sizes.
+# We ensure, that the number of threads in a CUDA block is equal to the tile-size. Further we assume
+# squared dense blocks. Last but not least, each CUDA block computes at least one blocked row in the BSR.
 #
-#   In this variant, each thread computes one row in a dense block and is intended for larger block sizes.
-#   We ensure, that the number of threads in a CUDA block is equal to the tile-size. Further we assume
-#   squared dense blocks. Last but not least, each CUDA block computes at least one blocked row in the BSR.
 rate_psp_kernel_rpt = {
-    'body': {
+    'device_kernel': {
         'sum': """
 __global__ void cu_proj%(id_proj)s_psp_bsr(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     const %(idx_type)s idx = threadIdx.x;
     const %(idx_type)s block_row = blockIdx.x;
     const %(size_type)s tile_size2 = tile_size * tile_size;
     extern %(float_prec)s __shared__ loc_pre_r[];
 
@@ -266,17 +249,17 @@
         }
 
         %(target_arg)s[row * tile_size + idx] += lsum;
     }
 }
 """
     },
-    'header': """__global__ void cu_proj%(id)s_psp_bsr(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'device_header': """__global__ void cu_proj%(id)s_psp_bsr(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
-    'call': """
+    'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
         unsigned int nb_blocks = std::min<unsigned int>(proj%(id_proj)s.block_row_size(), 65535);
         size_t smem_size = proj%(id_proj)s.get_tile_size() * sizeof(%(float_prec)s);
         cu_proj%(id_proj)s_psp_bsr<<<nb_blocks, proj%(id_proj)s.get_tile_size(), smem_size>>>(
             %(conn_args)s
             /* other variables */
@@ -288,15 +271,14 @@
     #ifdef _DEBUG
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
-
 """,
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
@@ -306,21 +288,29 @@
             'min': "DBL_MAX",
             'max': "DBL_MIN",
             'mean': "0.0"
         }
     }
 }
 
-#   BSR implementation following Eberhardt & Hoemmen (2016) - column-by-column
+# BSR implementation following Eberhardt & Hoemmen (2016) - column-by-column
+#
+# This variant is intended for small block sizes.
+#
+# Keys - structure:
 #
-#   This variant is intended for small block sizes.
+# * device_kernel
+#    * sum
+# * kernel_decl
+# * host_call
+# * thread_init
 rate_psp_kernel_cbc = {
-    'body': {
+    'device_kernel': {
         'sum': """
-__global__ void cu_proj%(id_proj)s_psp_bsr(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {        
+__global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     unsigned int tIdx = threadIdx.x;
     unsigned int bIdx = blockIdx.x;
     extern %(float_prec)s __shared__ sdata[];
     %(idx_type)s tile_size2 = tile_size *  tile_size;
 
     int blocks_per_warp = floorf(blockDim.x / tile_size2);
     int block_offset = int(float(tIdx) / float(tile_size2));
@@ -356,41 +346,59 @@
         for (int i = tIdx; i < tile_size2; i+= tile_size) {
             %(target_arg)s[bIdx * tile_size+tIdx] += sdata[i];
         }
     }
 }
 """,
 },
-    'header': """__global__ void cu_proj%(id)s_psp_bsr(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void call_proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
+    // kernel launch
+    cu_proj%(id_proj)s_psp<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        %(conn_args_call)s
+        /* other variables */
+        %(add_args_call)s
+        /* result */
+        %(target_arg_call)s
+    );
+}
+""",
+    'kernel_decl': """void call_proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
     'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        // one local variable per thread
-        size_t smem_size = proj%(id_proj)s._threads_per_block * sizeof(%(float_prec)s);
-
-        // kernel launch
-        cu_proj%(id_proj)s_psp_bsr<<<proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, smem_size>>>(
+        // kernel configuration
+        RunConfig proj%(id_proj)s_psp_cfg;
+        proj%(id_proj)s_psp_cfg.nb = proj%(id_proj)s._nb_blocks;
+        proj%(id_proj)s_psp_cfg.tpb = proj%(id_proj)s._threads_per_block;
+        proj%(id_proj)s_psp_cfg.smem_size = proj%(id_proj)s._threads_per_block * sizeof(%(float_prec)s);    // one local variable per thread
+        proj%(id_proj)s_psp_cfg.stream = proj%(id_proj)s.stream;
+
+        // invoke kernel
+        call_proj%(id_proj)s_psp (
+            /* kernel config */
+            proj%(id_proj)s_psp_cfg,
+            /* ranks and offsets */
             %(conn_args)s
-            /* other variables */
+            /* computation data */
             %(add_args)s
             /* result */
             %(target_arg)s
         );
 
     #ifdef _DEBUG
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
 
 """,
-    'kernel_call': "",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
@@ -403,15 +411,15 @@
     }
 }
 
 conn_templates = {
     # connectivity representation
     'conn_header': "const %(idx_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ col_ids, const %(idx_type)s n_block_rows, const %(idx_type)s tile_size",
     'conn_call': "proj%(id_proj)s.gpu_block_row_pointer(), proj%(id_proj)s.gpu_block_column_index(), proj%(id_proj)s.block_row_size(), proj%(id_proj)s.get_tile_size()",
-    'conn_kernel': "",
+    'conn_kernel': "row_ptr, col_ids, n_block_rows, tile_size",
 
     # launch config
     'launch_config': launch_config,
 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/BaseTemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/BaseTemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CUDATemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 projection_header = """/*
  *  ANNarchy-version: %(annarchy_version)s
  */
 #pragma once
 
 #include "ANNarchy.h"
 %(sparse_matrix_include)s
@@ -51,15 +33,15 @@
 
 %(connector_call)s
 
 %(declare_connectivity_matrix)s
 %(access_connectivity_matrix)s
 
     // Transmission and plasticity flags
-    bool _transmission, _plasticity, _update;
+    bool _transmission, _axon_transmission, _plasticity, _update;
     int _update_period;
     long int _update_offset;
 
 %(declare_delay)s
 %(declare_event_driven)s
 %(declare_rng)s
 %(declare_parameters_variables)s
@@ -109,15 +91,15 @@
     // Additional access methods
 %(access_parameters_variables)s
 %(access_additional)s
 
     // Memory management
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     void clear() {
     #ifdef _DEBUG
         std::cout << "PopStruct%(id_proj)s::clear()" << std::endl;
     #endif
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/COO.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_T.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,36 @@
-#===============================================================================
-#
-#     COO.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020-21  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
 additional_global_functions = ""
 
 launch_config = {
     'init': """
-        _threads_per_block = 192;
-        unsigned int tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_synapses())/static_cast<double>(_threads_per_block)));
-        _nb_blocks = std::min<unsigned int>(65535, tmp_blocks);
-
+        _threads_per_block = 64;
+        _nb_blocks = std::min<unsigned int>(nb_dendrites(), 65535);
+    
     #ifdef _DEBUG
-        std::cout << "Initial kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
+        std::cout << "Kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """,
     'update': """
         if (nb_blocks != -1) {
             _nb_blocks = static_cast<unsigned int>(nb_blocks);
             _threads_per_block = threads_per_block;
         }else{
             _threads_per_block = threads_per_block;
-            unsigned int tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_synapses())/static_cast<double>(_threads_per_block)));
-            _nb_blocks = std::min<unsigned int>(65535, tmp_blocks);
+            _nb_blocks = std::min<unsigned int>(nb_dendrites(), 65535);
         }
 
     #ifdef _DEBUG
-        std::cout << "Updated kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
+        std::cout << "Updated configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """
 }
 
 attribute_decl = {
     'local': """
     // Local %(attr_type)s %(name)s
@@ -62,43 +42,57 @@
     'semiglobal': """
     // Semiglobal %(attr_type)s %(name)s
     std::vector< %(type)s >  %(name)s ;
     %(type)s* gpu_%(name)s;
     long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
 """,
-    'global': """
+    'global': {
+        'parameter': """
+    // Global %(attr_type)s %(name)s
+    %(type)s %(name)s;
+""",
+        'variable': """
     // Global %(attr_type)s %(name)s
     %(type)s %(name)s;
     %(type)s* gpu_%(name)s;
     long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
 """
+    }
 }
 
 attribute_cpp_init = {
     'local': """
         // Local %(attr_type)s %(name)s
         %(name)s = init_matrix_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_matrix_variable_gpu<%(type)s>(%(name)s);
         %(name)s_host_to_device = true;
         %(name)s_device_to_host = t;
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_vector_variable_gpu<%(type)s>(%(name)s);
-        %(name)s_dirty = true;
+        %(name)s_host_to_device = true;
+        %(name)s_device_to_host = t;
 """,
-    'global': """
+    'global': {
+        'parameter': """
+        // Global %(attr_type)s %(name)s
+        %(name)s = 0.0;
+    """,
+        'variable': """
         // Global %(attr_type)s %(name)s
         %(name)s = static_cast<%(type)s>(%(init)s);
         cudaMalloc((void**)&gpu_%(name)s, sizeof(%(type)s));
-        %(name)s_dirty = true;
+        %(name)s_host_to_device = true;
+        %(name)s_device_to_host = t;
 """
+    }
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
         size_in_bytes += sizeof(bool);
         size_in_bytes += sizeof(%(ctype)s*);
@@ -118,33 +112,41 @@
         size_in_bytes += sizeof(%(ctype)s*);
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
-        // %(name)s
+        // %(name)s - host
+        %(name)s.clear();
+        %(name)s.shrink_to_fit();
+
+        // %(name)s - device
         cudaFree(gpu_%(name)s);
 """,
     'semiglobal': """
-        // %(name)s
+        // %(name)s - host
+        %(name)s.clear();
+        %(name)s.shrink_to_fit();
+
+        // %(name)s - device
         cudaFree(gpu_%(name)s);
 """,
     'global': ""
 }
 
 attribute_host_to_device = {
     'local': """
         // %(name)s: local
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), this->nb_synapses() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), num_non_zeros_ * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -152,15 +154,15 @@
     'semiglobal': """
         // %(name)s: semiglobal
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), this->nb_dendrites() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), post_ranks_.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -186,144 +188,204 @@
 attribute_device_to_host = {
     'local': """
         // %(name)s: local
         if ( %(name)s_device_to_host < t ) {
         #ifdef _DEBUG
             std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( %(name)s.data(), gpu_%(name)s, this->nb_synapses() * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
+            cudaMemcpy( %(name)s.data(), gpu_%(name)s, num_non_zeros_ * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
         #ifdef _DEBUG
             cudaError_t err_%(name)s = cudaGetLastError();
             if ( err_%(name)s != cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
             %(name)s_device_to_host = t;
         }
 """,
     'semiglobal': """
-        // %(name)s: semiglobal
-        if ( %(name)s_device_to_host < t ) {
+            // %(name)s: semiglobal
         #ifdef _DEBUG
             std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( %(name)s.data(), gpu_%(name)s, this->nb_dendrites() * sizeof(%(type)s), cudaMemcpyDeviceToHost);
+            cudaMemcpy( %(name)s.data(), gpu_%(name)s, post_ranks_.size() * sizeof(%(type)s), cudaMemcpyDeviceToHost);
         #ifdef _DEBUG
             cudaError_t err_%(name)s = cudaGetLastError();
             if ( err_%(name)s != cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
-            %(name)s_device_to_host = t;
-        }
 """,
     'global': """
-        // %(name)s: global
-        if ( %(name)s_device_to_host < t ) {
+            // %(name)s: global
         #ifdef _DEBUG
             std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
         #endif
             cudaMemcpy( &%(name)s, gpu_%(name)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
         #ifdef _DEBUG
             cudaError_t err_%(name)s = cudaGetLastError();
             if ( err_%(name)s != cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
-            %(name)s_device_to_host = t;
-        }
 """
 }
 
-rate_psp_kernel = {
-    'body': {
-        'sum': """
-__global__ void cu_proj%(id_proj)s_psp_coo(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
-    %(size_type)s j = segments[blockIdx.x] + threadIdx.x;
-    %(size_type)s C = segments[blockIdx.x+1];
-    %(size_type)s block_off = segment_size * blockIdx.x;
-
-    extern %(float_prec)s __shared__ sdata[];
-
-    if (threadIdx.x < segment_size)
-        sdata[threadIdx.x] = 0.0;
-    __syncthreads();
-
-    for( ; j < C; j += blockDim.x ) {
-
-        %(float_prec)s sum = %(psp)s
-        %(idx_type)s loc_idx = row_indices[j]-block_off;
-        atomicAdd(&(sdata[loc_idx]), sum);
-    }
-
-    __syncthreads();
-    if (threadIdx.x < segment_size)
-        %(target_arg)s[block_off + threadIdx.x] += sdata[threadIdx.x];
-}
+delay = {
+    'uniform': {
+        'declare': """
+    // Uniform delay
+    int delay ;""",
+        'pyx_struct': """
+        # Non-uniform delay
+        int delay""",
+        'init': "delay = delays[0][0];",
+        'pyx_wrapper_init': """
+        proj%(id_proj)s.delay = syn.uniform_delay""",
+        'pyx_wrapper_accessor': """
+    # Access to non-uniform delay
+    def get_delay(self):
+        return proj%(id_proj)s.delay
+    def get_dendrite_delay(self, idx):
+        return proj%(id_proj)s.delay
+    def set_delay(self, value):
+        print("set delay", value)
+        proj%(id_proj)s.delay = value
 """
     },
-    'header': """__global__ void cu_proj%(id)s_psp_coo(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'nonuniform_rate_coded': {
+        'declare': """
+    // Non-uniform delay
+    std::vector< std::vector< int > > delay ;""",
+        'pyx_struct': """
+        # Non-uniform delay
+        vector[vector[int]] delay""",
+    
+        'init': "",
+
+        'pyx_wrapper_init': """
+        proj%(id_proj)s.delay = syn.delay""",
+    
+        'pyx_wrapper_accessor': """
+    # Access to non-uniform delay
+    def get_delay(self):
+        return proj%(id_proj)s.delay
+    def get_dendrite_delay(self, idx):
+        return proj%(id_proj)s.delay[idx]
+    def set_delay(self, value):
+        proj%(id_proj)s.delay = value
+"""
+    },
+    'nonuniform_spiking': None
+}
+
+event_driven = {
+    'declare': """
+    std::vector< long > _last_event;
+    long* _gpu_last_event;
+""",
+    'cpp_init': """
+    _last_event = init_matrix_variable<long>(-10000);
+    _gpu_last_event = init_matrix_variable_gpu<long>(_last_event);    
 """,
-    'host_call': """
-    // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
-    if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        int sharedMemSize = proj%(id_proj)s.segment_size() * sizeof(%(float_prec)s);
-        cu_proj%(id_proj)s_psp_coo<<< proj%(id_proj)s.number_of_segments(), proj%(id_proj)s._threads_per_block, sharedMemSize >>>(
-            %(conn_args)s
-            /* other variables */
-            %(add_args)s
-            /* result */
-            %(target_arg)s
-        );
+    'pyx_struct': """
+        vector[long] _last_event
+""",
+    'pyx_wrapper_init':
+"""
+        proj%(id_proj)s._last_event = vector[long]( syn._matrix.num_elements(), -10000)
+"""
+}
 
-    #ifdef _DEBUG
-        auto err = cudaGetLastError();
-        if ( err != cudaSuccess ) {
-            std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
+spike_event_transmission = {
+    'device_kernel': """// gpu device kernel for projection %(id_proj)s
+__global__ void cu_proj%(id_proj)s_psp( %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* spike_count, %(conn_args_header)s %(kernel_args_header)s ) {
+    int b_idx = blockIdx.x;
+    int pre_rank = spiked[b_idx];
+
+    while (b_idx < *spike_count) {
+        int syn_idx = threadIdx.x + row_ptr[pre_rank];
+        while (syn_idx < row_ptr[pre_rank+1]){
+%(psp)s
+            syn_idx += blockDim.x;
         }
-    #endif
+        b_idx += gridDim.x;
     }
+
+}
+""",
+    'invoke_kernel': """
+void proj%(id_proj)s_psp(RunConfig cfg, %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* spike_count,  %(conn_args_header)s %(kernel_args_header)s) {
+    cu_proj%(id_proj)s_psp<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* default events */
+        dt, plasticity,
+        /* pre-synaptic events */
+        spiked, spike_count,
+        /* connectivity */
+        %(conn_args_invoke)s
+        /* other arguments */
+        %(kernel_args_invoke)s
+    );
+}
 """,
-    'kernel_call': "",
-    'thread_init': {
-        'float': {
-            'sum': "0.0f",
-            'min': "FLT_MAX",
-            'max': "FLT_MIN",
-            'mean': "0.0f"
-        },
-        'double': {
-            'sum': "0.0",
-            'min': "DBL_MAX",
-            'max': "DBL_MIN",
-            'mean': "0.0"
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* spike_count,  %(conn_args_header)s %(kernel_args_header)s);
+""",
+    'host_call': """
+        if ( pop%(id_pre)s._active && (pop%(id_pre)s.spike_count > 0) && proj%(id_proj)s._transmission) {
+            int tpb = 1024;//__pop%(id_pre)s_pop%(id_post)s_%(target)s_tpb__;
+            int nbBlocks = pop%(id_pre)s.spike_count;
+            
+            proj%(id_proj)s_psp(
+                RunConfig(nbBlocks, tpb, 0, proj%(id_proj)s.stream),
+                /* default events */
+                dt, proj%(id_proj)s._plasticity,
+                /* pre-synaptic events */
+                pop%(id_pre)s.gpu_spiked, pop%(id_pre)s.gpu_spike_count,
+                %(conn_args)s
+                /* other arguments */
+                %(kernel_args)s
+            );
+
+        #ifdef _DEBUG
+            cudaDeviceSynchronize();
+            cudaError_t err_psp_proj%(id_proj)s = cudaGetLastError();
+            if( err_psp_proj%(id_proj)s != cudaSuccess) {
+                std::cout << "proj%(id_proj)s_psp (" << t << "): " << std::endl;
+                std::cout << "   " << cudaGetErrorString(err_psp_proj%(id_proj)s) << std::endl;
+            }
+        #endif
         }
-    }
+"""
 }
 
 conn_templates = {
     # connectivity representation
-    'conn_header': "const %(idx_type)s segment_size, const %(size_type)s *segments, const %(idx_type)s* __restrict__ row_indices, const %(idx_type)s* __restrict__ column_indices",
-    'conn_call': "proj%(id_proj)s.segment_size(), proj%(id_proj)s.gpu_segments(), proj%(id_proj)s.gpu_row_indices(), proj%(id_proj)s.gpu_column_indices()",
+    'conn_header' : "const %(idx_type)s post_size, const %(idx_type)s* __restrict__  rank_post, const %(size_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ rank_pre",
+    'conn_call' : "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank, proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank",
     'conn_kernel': "",
 
     # launch config
     'launch_config': launch_config,
 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
-    'attribute_cpp_delete': attribute_cpp_delete,
+    'attribute_cpp_delete':attribute_cpp_delete,
     'host_to_device': attribute_host_to_device,
     'device_to_host': attribute_device_to_host,
+    'delay': delay,
+    'event_driven': event_driven,
 
     # operations
-    'rate_psp': rate_psp_kernel,
+    'spike_transmission': {
+        'event_driven': spike_event_transmission
+    }
 }
 
 conn_ids = {
     'local_index': "[j]",
     'semiglobal_index': '[i]',
     'global_index': '[0]',
-    'pre_index': '[column_indices[j]]',
-    'post_index': '[row_indices[j]]',
+    'pre_index': '[rank_pre[j]]',
+    'post_index': '[col_idx[syn_idx]]',
     'pre_prefix': 'pre_',
     'post_prefix': 'post_',
+    'delay_nu' : '[delay[j]-1]', # non-uniform delay
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-#===============================================================================
-#
-#     CSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
 additional_global_functions = """
 // warp reduce as in Dinkelbach et al. 2012 / Harris (CUDA Webinar 2)
 template<typename DATA_TYPE>
 __device__ void half_warp_reduce_sum(volatile DATA_TYPE* data, unsigned int tid) {
@@ -318,24 +299,20 @@
 """,
     'pyx_wrapper_init':
 """
         proj%(id_proj)s._last_event = vector[long]( syn._matrix.num_elements(), -10000)
 """
 }
 
-#
-# Implement the continuous transmission for rate-coded synapses.
+# Implement the continuous signal transmission for rate-coded synapses. The *sum* operation
+# is comparable to the SpMV operation. Next to that, we implement also comparison operators
+# and average of the rows.
 #
 rate_psp_kernel = {
-    # Comment to if (tid < 32) block:
-    #
-    # now that we are using warp-synchronous programming (below)
-    # we need to declare our shared memory volatile so that the compiler
-    # doesn't reorder stores to it and induce incorrect behavior.
-    'body': {
+    'device_kernel': {
         'sum':"""
 template<int BLOCKSIZE>
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     unsigned int tid = threadIdx.x;
     unsigned int bid = blockIdx.x;
     extern %(float_prec)s __shared__ sdata[];
 
@@ -362,15 +339,15 @@
         // write result for this block to global mem
         if (tid == 0) { %(target_arg)s[rk_post] += sdata[0]; }
 
         bid += gridDim.x;
     }
 }
 """,
-    'min':"""
+        'min':"""
 template<int BLOCKSIZE>
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     unsigned int tid = threadIdx.x;
     unsigned int bid = blockIdx.x;
     extern %(float_prec)s __shared__ sdata[];
 
     while( bid < post_size ) {
@@ -419,15 +396,15 @@
             %(target_arg)s[rk_post] += sdata[0];
         }
 
         bid += gridDim.x;
     }
 }
 """,
-    'max':"""
+        'max':"""
 template<int BLOCKSIZE>
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     unsigned int tid = threadIdx.x;
     unsigned int bid = blockIdx.x;
     extern %(float_prec)s __shared__ sdata[];
 
     while( bid < post_size ) {
@@ -475,16 +452,16 @@
             %(target_arg)s[rk_post] += sdata[0];
         }
 
         bid += gridDim.x;
     }
 }
 """,
-    # Technically a sum operation, but the result is normalized with the number of connection entries
-    'mean': """
+        # Technically a sum operation, but the result is normalized with the number of connection entries
+        'mean': """
 template<int BLOCKSIZE>
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     unsigned int tid = threadIdx.x;
     unsigned int bid = blockIdx.x;
     extern %(float_prec)s __shared__ sdata[];
 
     while( bid < post_size ) {
@@ -513,33 +490,15 @@
         if (tid == 0) { %(target_arg)s[rk_post] += sdata[0] / (%(float_prec)s(row_ptr[bid+1]-row_ptr[bid])); }
 
         bid += gridDim.x;
     }
 }
 """
     },
-    'header': """void call_proj%(id)s_psp(const int nb_blocks, const int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
-""",
-    'host_call': """
-    // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
-    if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        call_proj%(id_proj)s_psp(
-            /* kernel config */
-            proj%(id_proj)s._nb_blocks,
-            proj%(id_proj)s._threads_per_block,
-            /* ranks and offsets */
-            %(conn_args)s
-            /* computation data */
-            %(add_args)s
-            /* result */
-            %(target_arg)s
-        );
-    }
-""",
-    'kernel_call': """
+    'invoke_kernel': """
 void call_proj%(id_proj)s_psp(const int nb_blocks, const int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     int sharedMemSize = threads_per_block * sizeof(%(float_prec)s);
 
     switch(threads_per_block) {
         case 32:
             {
                 cu_proj%(id_proj)s_psp<32><<< nb_blocks, threads_per_block, sharedMemSize>>>(
@@ -582,26 +541,44 @@
                     %(add_args_call)s
                     /* result */
                     %(target_arg_call)s
                 );
             }break;
         default:
         {
-            std::cerr << "The kernel configuration tpb = " << threads_per_block << " is not supported" << std::endl;
+            printf("The kernel configuration tpb = %%i is not supported.\\n", threads_per_block);
         }
     }
 
 #ifdef _DEBUG
     auto err = cudaGetLastError();
     if ( err != cudaSuccess ) {
-        std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
+        printf("cu_proj%(id_proj)s_psp: %%s.\\n", cudaGetErrorString(err));
     }
 #endif
 }
 """,
+    'kernel_decl': """void call_proj%(id_proj)s_psp(const int nb_blocks, const int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+""",
+    'host_call': """
+    // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
+    if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
+        call_proj%(id_proj)s_psp(
+            /* kernel config */
+            proj%(id_proj)s._nb_blocks,
+            proj%(id_proj)s._threads_per_block,
+            /* ranks and offsets */
+            %(conn_args)s
+            /* computation data */
+            %(add_args)s
+            /* result */
+            %(target_arg)s
+        );
+    }
+""",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
@@ -610,17 +587,19 @@
             'min': "DBL_MAX",
             'max': "DBL_MIN",
             'mean': "0.0"
         }
     }
 }
 
+# Implements the event-driven signal transmission between spiking neurons.
+#
 spike_event_transmission = {
-    'body': """// gpu device kernel for projection %(id)s
-__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int num_events, %(conn_arg)s %(kernel_args)s ) {
+    'device_kernel': """// gpu device kernel for projection %(id_proj)s
+__global__ void cu_proj%(id_proj)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int num_events, %(conn_args_header)s %(kernel_args_header)s ) {
     int bid = blockIdx.x;
     int tid = threadIdx.x;
 
     while ( bid < num_events ) {
         int pre_index = spiked[bid];
 
         int j = col_ptr[pre_index] + tid;
@@ -641,28 +620,47 @@
             j += blockDim.x;
         }
 
         bid += gridDim.x;
     }
 }
 """,
-    'header': """__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int num_events, %(conn_header)s %(kernel_args)s);
+    'invoke_kernel': """void proj%(id_proj)s_psp(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int num_events, %(conn_args_header)s %(kernel_args_header)s) {
+        cu_proj%(id_proj)s_psp<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+            /* default params */
+            t, dt, plasticity,
+            /* pre-synaptic spike events */
+            spiked, num_events,
+            /* connectivity */
+            %(conn_args_invoke)s
+            /* function arguments */
+            %(kernel_args_invoke)s
+        );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int num_events, %(conn_args_header)s %(kernel_args_header)s);
 """,
-    'call': """
+    'host_call': """
     if ( pop%(id_pre)s._active && (%(pre_spike_count)s > 0) && proj%(id_proj)s._transmission ) {
+        RunConfig proj%(id_proj)s_psp_cfg;
+        proj%(id_proj)s_psp_cfg.nb = static_cast<unsigned int>(%(pre_spike_count)s);
     #if defined (__proj%(id_proj)s_%(target)s_nb__)
-        unsigned int tpb = __proj%(id_proj)s_%(target)s_tpb__;
+        proj%(id_proj)s_psp_cfg.tpb = __proj%(id_proj)s_%(target)s_tpb__;
     #else
-        unsigned int tpb = proj%(id_proj)s._threads_per_block;
+        proj%(id_proj)s_psp_cfg.tpb = proj%(id_proj)s._threads_per_block;
     #endif
-        unsigned int nb = static_cast<unsigned int>(%(pre_spike_count)s);
+        proj%(id_proj)s_psp_cfg.smem_size = 0;
+        proj%(id_proj)s_psp_cfg.stream = proj%(id_proj)s.stream;
 
         // compute psp using backward view ...
-        cu_proj%(id_proj)s_psp<<< nb, tpb, 0, proj%(id_proj)s.stream >>>( 
-            t, dt, proj%(id_proj)s._plasticity, 
+        proj%(id_proj)s_psp(
+            /* kernel config */
+            proj%(id_proj)s_psp_cfg
+            /* default params */
+            , t, dt, proj%(id_proj)s._plasticity,
             /* pre-synaptic spike events */
             %(pre_spike_events)s, %(pre_spike_count)s,
             /* connectivity */
             %(conn_args)s
             /* kernel config */
             %(kernel_args)s
         );
@@ -675,31 +673,31 @@
             std::cout << "   " << cudaGetErrorString(err_psp_proj%(id_proj)s) << std::endl;
         }
     #endif
     }
 """
 }
 
-spike_continous_transmission = {
+spike_continuous_transmission = {
     #
     # This kernel computes the post-synaptic potential for continous
     # transmission using the forward view of connectivty data.
     #
     # ATTENTION: post_idx and post_rank diverge in case of non-existant
     #            dendrites
     #
     # TODO: it might be more effective to split this kernel into two functions ...
-    'body': """// gpu device kernel for projection %(id_proj)s
-__global__ void cu_proj%(id_proj)s_cont_psp( %(float_prec)s dt, bool plasticity, int post_size, int* post_ranks, 
+    'device_kernel': """// gpu device kernel for projection %(id_proj)s
+__global__ void cu_proj%(id_proj)s_cont_psp( %(float_prec)s dt, bool plasticity, int post_size, int* post_ranks,
                                             /* connectivity */
                                             int* row_ptr, int* col_idx, %(float_prec)s *w
                                             /* additional arguments */
                                             %(kernel_args)s
                                             /* target */
-                                            , %(float_prec)s* %(target_arg)s ) 
+                                            , %(float_prec)s* %(target_arg)s )
 {
     int post_idx = blockIdx.x;
     int tid = threadIdx.x;
     extern %(float_prec)s __shared__ sdata[];
     while ( post_idx < post_size ) {
         // which dendrite we are working on
         int post_rank = post_ranks[post_idx];
@@ -731,27 +729,42 @@
             %(target_arg)s[post_rank] += sdata[0];
         }
         __syncthreads();
         post_idx += gridDim.x;
     }
 }
 """,
-    'header': """__global__ void cu_proj%(id)s_event_psp( %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, int* col_ptr, int* row_idx, int* inv_idx, %(float_prec)s *w %(kernel_args)s);
-__global__ void cu_proj%(id)s_cont_psp( %(float_prec)s dt, bool plasticity, int post_size, int* post_ranks, int* row_ptr, int* col_idx, %(float_prec)s *w %(kernel_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void proj%(id_proj)s_cont_psp(RunConfig cfg, %(float_prec)s dt, bool plasticity, int post_size, int* post_ranks, int* row_ptr, int* col_idx, %(float_prec)s *w %(kernel_args)s %(target_arg)s ) {
+    cu_proj%(id_proj)s_cont_psp<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        dt, plasticity, post_size, post_ranks,
+        /* connectivity */
+        row_ptr, col_idx, w
+        /* additional arguments */
+        %(kernel_args_invoke)s
+        /* target */
+        %(target_arg_invoke)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_cont_psp(RunConfig cfg, %(float_prec)s dt, bool plasticity, int post_size, int* post_ranks, int* row_ptr, int* col_idx, %(float_prec)s *w %(kernel_args)s %(target_arg)s );
 """,
-        'call': """
+        'host_call': """
     if ( pop%(id_pre)s._active && proj%(id_proj)s._transmission ) {
     #if defined (__proj%(id_proj)s_%(target)s_nb__)
         unsigned int tpb = __proj%(id_proj)s_%(target)s_tpb__;
     #else
         unsigned int tpb = proj%(id_proj)s._threads_per_block;
     #endif
 
         // compute continous transmission using forward view ...
-        cu_proj%(id_proj)s_cont_psp<<< proj%(id_proj)s.nb_dendrites(), tpb, tpb*sizeof(%(float_prec)s), proj%(id_proj)s.stream >>>( 
+        proj%(id_proj)s_cont_psp(
+            /* kernel configuration */
+            RunConfig(proj%(id_proj)s.nb_dendrites(), tpb, tpb*sizeof(%(float_prec)s), proj%(id_proj)s.stream),
+            /* default arguments */
             dt, proj%(id_proj)s._plasticity, proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank, 
             /* connectivity */
             proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank, proj%(id_proj)s.gpu_w
             /* additional arguments */ 
             %(kernel_args)s
             /* target */
             %(target_arg)s
@@ -768,33 +781,46 @@
     }
 """
 }
 
 # Update of global synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 global_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_global_step(
     /* default params */
     const long int t, const %(float_prec)s dt
     /* additional params */
     %(kernel_args)s,
     /* plasticity enabled */
     bool plasticity )
 {
 %(pre_loop)s
 %(global_eqs)s
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_global_step(const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+    'invoke_kernel': """
+void proj%(id_proj)s_global_step(RunConfig cfg, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_global_step<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        /* default args*/
+        t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_global_step(RunConfig cfg, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-    'call': """
+    'host_call': """
         // global update
-        cuProj%(id_proj)s_global_step<<< 1, 1, 0, proj%(id_proj)s.stream>>>(
+        proj%(id_proj)s_global_step(
+            RunConfig(1, 1, 0, proj%(id_proj)s.stream),
             /* default args*/
             t, _dt
             /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
@@ -808,15 +834,15 @@
     #endif
 """
 }
 
 # Update of semiglobal synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 semiglobal_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_semiglobal_step(
     const %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post,
     /* default params */
     const long int t, const %(float_prec)s dt
     /* additional params */
     %(kernel_args)s,
@@ -829,55 +855,62 @@
     while ( i < post_size ) {
 %(semiglobal_eqs)s
 
         i += gridDim.x * blockDim.x;
     }
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_semiglobal_step(%(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+    'invoke_kernel': """
+void proj%(id_proj)s_semiglobal_step(RunConfig cfg, %(idx_type)s post_size, const %(idx_type)s* rank_post, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_semiglobal_step<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        post_size, rank_post,
+        /* default args*/
+        t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_semiglobal_step(RunConfig cfg, %(idx_type)s post_size, const %(idx_type)s* rank_post, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-    'call': """
+    'host_call': """
         // semiglobal update
     #if defined (__proj%(id_proj)s_%(target)s_tpb__)
-        cuProj%(id_proj)s_semiglobal_step<<< __proj%(id_proj)s_%(target)s_nb__, __proj%(id_proj)s_%(target)s_tpb__, 0, proj%(id_proj)s.stream >>>(
-            proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank,
-            /* default args*/
-            t, _dt
-            /* kernel args */
-            %(kernel_args_call)s
-            /* synaptic plasticity */
-            , proj%(id_proj)s._plasticity
-        );
+        RunConfig proj%(id_proj)s_semiglobal_step_cfg = RunConfig(__proj%(id_proj)s_%(target)s_nb__, __proj%(id_proj)s_%(target)s_tpb__, 0, proj%(id_proj)s.stream);
     #else
         nb_blocks = ceil( %(float_prec)s(proj%(id_proj)s.nb_dendrites()) / %(float_prec)s(proj%(id_proj)s._threads_per_block));
-        cuProj%(id_proj)s_semiglobal_step<<< nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream >>>(
+        RunConfig proj%(id_proj)s_semiglobal_step_cfg = RunConfig(nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream);
+    #endif
+        proj%(id_proj)s_semiglobal_step(
+            proj%(id_proj)s_semiglobal_step_cfg,
             proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank,
             /* default args*/
             t, _dt
             /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
-    #endif
 
     #ifdef _DEBUG
         cudaDeviceSynchronize();
         err = cudaGetLastError();
         if ( err != cudaSuccess) {
             std::cout << "proj%(id_proj)s_semiglobal_step: " << cudaGetErrorString( err ) << std::endl;
         }
     #endif
 """
 }
 
 # Update of local synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 local_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_local_step(
     /* connectivity */
     %(conn_args)s,
     /* default params */
     const long int t, const %(float_prec)s dt
     /* additional params */
@@ -896,42 +929,48 @@
     {
 %(local_eqs)s
 
         j += blockDim.x;
     }
 }
 """,
-        'header': """__global__ void cuProj%(id_proj)s_local_step(%(conn_args)s, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity);
+        'invoke_kernel': """
+void proj%(id_proj)s_local_step(RunConfig cfg, %(conn_args)s, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_local_step<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* connectivity */
+        %(conn_args_call)s
+        /* default args*/
+        , t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+}
+""",
+        'kernel_decl': """void proj%(id_proj)s_local_step(RunConfig cfg, %(conn_args)s, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-        'call': """
+        'host_call': """
         // local update
     #if defined (__proj%(id_proj)s_%(target)s_tpb__)
-        cuProj%(id_proj)s_local_step<<< __proj%(id_proj)s_nb__, __proj%(id_proj)s_%(target)s_tpb__, 0, proj%(id_proj)s.stream >>>(
-            pop%(id_post)s.size,
-            /* connectivity */
-            %(conn_args_call)s
-            /* default args*/
-            , t, _dt
-            /* kernel args */
-            %(kernel_args_call)s
-            /* synaptic plasticity */
-            , proj%(id_proj)s._plasticity
-        );
+        RunConfig proj%(id_proj)s_local_step_cfg = RunConfig(__proj%(id_proj)s_nb__, __proj%(id_proj)s_%(target)s_tpb__, 0, proj%(id_proj)s.stream);
     #else
-        cuProj%(id_proj)s_local_step<<< proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream >>>(
+        RunConfig proj%(id_proj)s_local_step_cfg = RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream);
+    #endif
+        proj%(id_proj)s_local_step(
+            proj%(id_proj)s_local_step_cfg,
             /* connectivity */
             %(conn_args_call)s
             /* default args*/
             , t, _dt
             /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
-    #endif
 
     #ifdef _DEBUG
         cudaDeviceSynchronize();
         err = cudaGetLastError();
         if ( err != cudaSuccess) {
             std::cout << "proj%(id_proj)s_step: " << cudaGetErrorString( err ) << std::endl;
         }
@@ -958,45 +997,61 @@
 # Evaluation of post-event equations
 #
 spike_postevent = {
     #
     # Called if storage_order is 'post_to_pre'. The vector pop%(id).gpu_spiked must be interpreted
     # as a boolean array. The parallelization happens across pop%(id).spike_count blocks.
     #
-    'body': """// Projection %(id_proj)s: post-synaptic events
-__global__ void cuProj%(id_proj)s_postevent( const long int t, const %(float_prec)s dt, bool plasticity, int *post_rank, int* spiked, long int* pre_last_spike, %(conn_args)s %(float_prec)s* w %(add_args)s ) {
+    'device_kernel': """// Projection %(id_proj)s: post-synaptic events
+__global__ void cuProj%(id_proj)s_postevent( const long int t, const %(float_prec)s dt, bool plasticity, int *post_rank, int* spiked, long int* pre_last_spike, %(conn_args)s, %(float_prec)s* w %(add_args)s ) {
     int i = spiked[blockIdx.x]; // post-synaptic
     int j = row_ptr[i]+threadIdx.x;        // pre-synaptic
 
     while ( j < row_ptr[i+1] ) {
         int rk_post = post_rank[i];
 
     // event-driven
 %(event_driven)s
     // post-event
 %(post_code)s
         j+= blockDim.x;
     }
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_postevent( const long int t, const %(float_prec)s dt, bool plasticity, int *post_rank, int* spiked, long int* pre_last_spike, %(conn_args)s %(float_prec)s* w %(add_args)s );
+    'invoke_kernel': """
+void proj%(id_proj)s_postevent(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *post_rank, int* spiked, long int* pre_last_spike, %(conn_args)s, %(float_prec)s* w %(add_args)s ){
+    cuProj%(id_proj)s_postevent<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        t, dt, plasticity, post_rank,
+        /* post-spike and pre-spike time points */
+        spiked, pre_last_spike,
+        /* connectivity */
+        %(conn_args_invoke)s
+        /* weights */
+        , w
+        /* other variables */
+        %(add_args_invoke)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_postevent(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *post_rank, int* spiked, long int* pre_last_spike, %(conn_args)s, %(float_prec)s* w %(add_args)s );
 """,
     # Each cuda block compute one of the spiking post-synaptic neurons
-    'call': """
+    'host_call': """
     if ( proj%(id_proj)s._transmission && pop%(id_post)s._active && (pop%(id_post)s.spike_count > 0) ) {
     #if defined (__proj%(id_proj)s_%(target)s_nb__)
         int tpb = __proj%(id_proj)s_%(target)s_tpb__;
     #else
         int tpb = proj%(id_proj)s._threads_per_block;
     #endif
 
-        cuProj%(id_proj)s_postevent<<< pop%(id_post)s.spike_count, tpb >>>(
+        proj%(id_proj)s_postevent(
+            RunConfig(pop%(id_post)s.spike_count, tpb, 0, proj%(id_proj)s.stream),
             t, dt, proj%(id_proj)s._plasticity, proj%(id_proj)s.gpu_post_rank,
             /* post-spike and pre-spike time points */
-            pop%(id_post)s.gpu_spiked, pop%(id_pre)s.gpu_last_spike
+            pop%(id_post)s.gpu_spiked, pop%(id_pre)s.gpu_last_spike,
             /* connectivity */
             %(conn_args)s
             /* weights */
             , proj%(id_proj)s.gpu_w
             /* other variables */
             %(add_args)s
         );
@@ -1030,15 +1085,15 @@
     'delay': delay,
     'event_driven': event_driven,
 
     # operations
     'rate_psp': rate_psp_kernel,
     'spike_transmission': {
         'event_driven': spike_event_transmission,
-        'continous': spike_continous_transmission,
+        'continuous': spike_continuous_transmission,
     },
     'synapse_update': {
         'global': global_synapse_update,
         'semiglobal': semiglobal_synapse_update,
         'local': local_synapse_update,
         'call': synapse_update_call
     },
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_Scalar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-#===============================================================================
-#
-#     CSR_Scalar.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
 additional_global_functions = ""
 
 launch_config = {
     'init': """
@@ -309,15 +291,15 @@
 """
         proj%(id_proj)s._last_event = vector[long]( syn._matrix.num_elements(), -10000)
 """
 }
 
 rate_psp_kernel = {
     # As discussed in Bell and Garland (2009) this kernel variant computes one row per thread
-    'body': {
+    'device_kernel': {
         'sum':"""
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
     %(idx_type)s row_idx = blockIdx.x * blockDim.x + threadIdx.x;
 
     while( row_idx < post_size ) {
         %(float_prec)s sum = 0.0;
 
@@ -327,21 +309,34 @@
         %(target_arg)s[rank_post[row_idx]] = sum;
 
         row_idx += blockDim.x * gridDim.x;
     }
 }
 """
     },
-    'header': """__global__ void cu_proj%(id)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
+    cu_proj%(id_proj)s_psp<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* ranks and offsets */
+        %(conn_args_call)s
+        /* computation data */
+        %(add_args_call)s
+        /* result */
+        %(target_arg_call)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
     'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-
-        cu_proj%(id_proj)s_psp<<< proj%(id_proj)s._nb_blocks,  proj%(id_proj)s._threads_per_block >>>(
+        proj%(id_proj)s_psp(
+            /* kernel config */
+            RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block,0, proj%(id_proj)s.stream),
             /* ranks and offsets */
             %(conn_args)s
             /* computation data */
             %(add_args)s
             /* result */
             %(target_arg)s
         );
@@ -350,15 +345,14 @@
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
 """,
-    'kernel_call': "",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
@@ -371,15 +365,15 @@
     }
 }
 
 conn_templates = {
     # connectivity representation
     'conn_header' : "const %(idx_type)s post_size, const %(idx_type)s* __restrict__  rank_post, const %(size_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ rank_pre",
     'conn_call' : "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank, proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank",
-    'conn_kernel': "",
+    'conn_kernel': "post_size, rank_post, row_ptr, rank_pre",
 
     # launch config
     'launch_config': launch_config,
 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
@@ -390,15 +384,15 @@
     'delay': delay,
     'event_driven': event_driven,
 
     # operations
     'rate_psp': rate_psp_kernel,
     'spike_transmission': {
         'event_driven': None,
-        'continous': None,
+        'continuous': None,
     },
     'synapse_update': {
         'global': None,
         'semiglobal': None,
         'local': None,
         'call': None
     },
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/CSR_Vector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,40 @@
-#===============================================================================
-#
-#     CSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
-additional_global_functions = ""
+additional_global_functions = """
+// Alternative implementation for Keplar and upwards
+// https://developer.nvidia.com/blog/faster-parallel-reductions-kepler/
+#define FULL_WARP_MASK 0xFFFFFFFF
+template<class ValueType, unsigned int WARP_SIZE>
+__device__ ValueType warp_reduce (ValueType val)
+{
+    for(int offset = WARP_SIZE/2; offset > 0; offset /= 2)
+        val += __shfl_down_sync(FULL_WARP_MASK, val, offset, 32);
+
+    return val;
+}
+"""
 
 launch_config = {
     'init': """
         _threads_per_block = 64;
-        _nb_blocks = std::min<unsigned int>(nb_dendrites(), 65535);
+        _nb_blocks = std::min<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)), 65535);
     
     #ifdef _DEBUG
         std::cout << "Kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """,
     'update': """
-        if (nb_blocks != -1) {
-            _nb_blocks = static_cast<unsigned int>(nb_blocks);
-            _threads_per_block = threads_per_block;
-        }else{
-            _threads_per_block = threads_per_block;
-            _nb_blocks = std::min<unsigned int>(nb_dendrites(), 65535);
-        }
-
     #ifdef _DEBUG
-        std::cout << "Updated configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
+        std::cout << "The CSR vector implementation is fixed to a specific thread configuration." << std::endl;
     #endif
 """
 }
 
 attribute_decl = {
     'local': """
     // Local %(attr_type)s %(name)s
@@ -308,57 +293,128 @@
 """,
     'pyx_wrapper_init':
 """
         proj%(id_proj)s._last_event = vector[long]( syn._matrix.num_elements(), -10000)
 """
 }
 
-spike_event_transmission = {
-    'body': """// gpu device kernel for projection %(id)s
-    __global__ void cu_proj%(id)s_psp( %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* spike_count, %(conn_arg)s %(kernel_args)s ) {
-        int b_idx = blockIdx.x;
-        int pre_rank = spiked[b_idx];
-       
-        while (b_idx < *spike_count) {
-            int syn_idx = threadIdx.x + row_ptr[pre_rank];
-            while (syn_idx < row_ptr[pre_rank+1]){
-%(psp)s
-                syn_idx += blockDim.x;
-		    }
-            b_idx += gridDim.x;
-        }
+rate_psp_kernel = {
+    # Adapted from Bell and Garland 2008, taken from https://code.google.com/archive/p/cusp-library/downloads (26. mar. 2018)
+    #
+    #   HD (2019): I needed to add a volatile variable, otherwise the results were wrong ...
+    #   HD (2020): I replaced the local reduction by a warp primitive introduced with CUDA 9.0
+    'device_kernel': {
+        'sum':"""
+template<unsigned int BLOCK_SIZE, unsigned int WARP_SIZE>
+__global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
+    __shared__ %(size_type)s ptrs[BLOCK_SIZE/WARP_SIZE][2];
+
+    const %(idx_type)s thread_id   = BLOCK_SIZE * blockIdx.x + threadIdx.x;  // global thread index
+    const %(idx_type)s thread_lane = threadIdx.x & (WARP_SIZE-1);            // thread index within the warp
+    const %(idx_type)s warp_id     = thread_id   / WARP_SIZE;                // global warp index
+    const %(idx_type)s warp_lane   = threadIdx.x / WARP_SIZE;                // warp index within the CTA
+    const %(idx_type)s num_warps   = (BLOCK_SIZE / WARP_SIZE) * gridDim.x;   // total number of active warps
+
+    for(%(idx_type)s row = warp_id; row < post_size; row += num_warps){
+
+        // use two threads to fetch Ap[row] and Ap[row+1]
+        // this is considerably faster than the straightforward version
+        if(thread_lane < 2)
+            ptrs[warp_lane][thread_lane] = row_ptr[row + thread_lane];
+        const %(size_type)s row_start = ptrs[warp_lane][0];                   //same as: row_start = Ap[row];
+        const %(size_type)s row_end   = ptrs[warp_lane][1];                   //same as: row_end   = Ap[row+1];
+
+        // compute local sum
+        %(float_prec)s sum = 0;
+        for(%(size_type)s j = row_start + thread_lane; j < row_end; j += WARP_SIZE)
+            sum += %(psp)s
+
+        // reduce local sums to row sum (ASSUME: warpsize 32)
+        sum = warp_reduce<%(float_prec)s, WARP_SIZE>(sum);
+
+        // first thread writes warp result
+        if (thread_lane == 0)
+            %(target_arg)s[rank_post[row]] = sum;
+    }
+}
+"""
+    },
+    'invoke_kernel': """
+void launch_proj%(id_proj)s_psp(const unsigned int nb_blocks, const unsigned int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
 
+    switch (threads_per_block)
+    {
+        case 64:
+        {
+            cu_proj%(id_proj)s_psp<64,32><<< nb_blocks, threads_per_block>>>(
+                /* ranks and offsets */
+                %(conn_args_call)s
+                /* computation data */
+                %(add_args_call)s
+                /* result */
+                %(target_arg_call)s
+            );
+        }break;
+
+        default:
+        {
+            std::cerr << "The kernel configuration tpb = " << threads_per_block << " is not supported" << std::endl;
+        }
     }
-    """,
-    'header': """__global__ void cu_proj%(id)s_psp( %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* spike_count,  %(conn_header)s %(kernel_args)s);
-    """,
-    'call': """
-        if ( pop%(id_pre)s._active && (pop%(id_pre)s.spike_count > 0) && proj%(id_proj)s._transmission) {
-            int tpb = 1024;//__pop%(id_pre)s_pop%(id_post)s_%(target)s_tpb__;
-            int nbBlocks = pop%(id_pre)s.spike_count;
-            
-            cu_proj%(id_proj)s_psp<<< nbBlocks, tpb, 0, proj%(id_proj)s.stream >>>( dt, proj%(id_proj)s._plasticity, pop%(id_pre)s.gpu_spiked, pop%(id_pre)s.gpu_spike_count, %(conn_args)s %(kernel_args)s);
+}
+""",    
+    'kernel_decl': """void launch_proj%(id_proj)s_psp(const unsigned int nb_blocks, const unsigned int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+""",
+    'host_call': """
+    // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
+    if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
+        const unsigned int BLOCK_SIZE = proj%(id_proj)s._threads_per_block;
+        const unsigned int WARPS_PER_BLOCK = BLOCK_SIZE / 32;
+        const unsigned int MAX_BLOCKS = MAX_THREADS / BLOCK_SIZE;
+        const unsigned int NUM_BLOCKS = std::min(MAX_BLOCKS, DIVIDE_INTO( proj%(id_proj)s.nb_dendrites(), WARPS_PER_BLOCK));
+
+        launch_proj%(id_proj)s_psp(
+            NUM_BLOCKS, BLOCK_SIZE,
+            /* ranks and offsets */
+            %(conn_args)s
+            /* computation data */
+            %(add_args)s
+            /* result */
+            %(target_arg)s
+        );
 
-        #ifdef _DEBUG
-            cudaDeviceSynchronize();
-            cudaError_t err_psp_proj%(id_proj)s = cudaGetLastError();
-            if( err_psp_proj%(id_proj)s != cudaSuccess) {
-                std::cout << "proj%(id_proj)s_psp (" << t << "): " << std::endl;
-                std::cout << "   " << cudaGetErrorString(err_psp_proj%(id_proj)s) << std::endl;
-            }
-        #endif
+    #ifdef _DEBUG
+        auto err = cudaGetLastError();
+        if ( err != cudaSuccess ) {
+            std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
-    """
+    #endif
+    }
+""",
+    'thread_init': {
+        'float': {
+            'sum': "0.0f",
+            'min': "FLT_MAX",
+            'max': "FLT_MIN",
+            'mean': "0.0f"
+        },
+        'double': {
+            'sum': "0.0",
+            'min': "DBL_MAX",
+            'max': "DBL_MIN",
+            'mean': "0.0"
+        }
+    }
 }
 
 conn_templates = {
     # connectivity representation
     'conn_header' : "const %(idx_type)s post_size, const %(idx_type)s* __restrict__  rank_post, const %(size_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ rank_pre",
     'conn_call' : "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank, proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank",
-    'conn_kernel': "",
+    'conn_kernel': "post_size, rank_post, row_ptr, rank_pre",
 
     # launch config
     'launch_config': launch_config,
 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
@@ -366,17 +422,26 @@
     'attribute_cpp_delete':attribute_cpp_delete,
     'host_to_device': attribute_host_to_device,
     'device_to_host': attribute_device_to_host,
     'delay': delay,
     'event_driven': event_driven,
 
     # operations
+    'rate_psp': rate_psp_kernel,
     'spike_transmission': {
-        'event_driven': spike_event_transmission
-    }
+        'event_driven': None,
+        'continuous': None,
+    },
+    'synapse_update': {
+        'global': None,
+        'semiglobal': None,
+        'local': None,
+        'call': None
+    },
+    'post_event': None
 }
 
 conn_ids = {
     'local_index': "[j]",
     'semiglobal_index': '[i]',
     'global_index': '[0]',
     'pre_index': '[rank_pre[j]]',
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/CSR_Vector.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/ELL.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,95 @@
-#===============================================================================
-#
-#     CSR_Vector.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
-# (directly imported by CodeGenerator if needed)
-additional_global_functions = """
-// Alternative implementation for Keplar and upwards
-// https://developer.nvidia.com/blog/faster-parallel-reductions-kepler/
-#define FULL_WARP_MASK 0xFFFFFFFF
-template<class ValueType, unsigned int WARP_SIZE>
-__device__ ValueType warp_reduce (ValueType val)
-{
-    for(int offset = WARP_SIZE/2; offset > 0; offset /= 2)
-        val += __shfl_down_sync(FULL_WARP_MASK, val, offset, 32);
-
-    return val;
-}
-"""
+additional_global_functions = ""
 
 launch_config = {
     'init': """
-        _threads_per_block = 64;
-        _nb_blocks = std::min<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)), 65535);
-    
+        _threads_per_block = 32;
+        auto tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)));
+        _nb_blocks = std::min<unsigned int>(tmp_blocks, 65535);
+
     #ifdef _DEBUG
-        std::cout << "Kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
+        std::cout << "Initial kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """,
     'update': """
+        if (nb_blocks != -1) {
+            _nb_blocks = static_cast<unsigned int>(nb_blocks);
+            _threads_per_block = threads_per_block;
+        }else{
+            _threads_per_block = threads_per_block;
+            auto tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)));
+            _nb_blocks = std::min<unsigned int>(tmp_blocks, 65535);
+        }
+
     #ifdef _DEBUG
-        std::cout << "The CSR vector implementation is fixed to a specific thread configuration." << std::endl;
+        std::cout << "Updated kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """
 }
 
+
 attribute_decl = {
     'local': """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """,
     'semiglobal': """
     // Semiglobal %(attr_type)s %(name)s
     std::vector< %(type)s >  %(name)s ;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """,
     'global': {
-        'parameter': """
-    // Global %(attr_type)s %(name)s
+        'parameter':
+    """
+    // Global parameter %(name)s
     %(type)s %(name)s;
 """,
         'variable': """
-    // Global %(attr_type)s %(name)s
+    // Global variable %(name)s
     %(type)s %(name)s;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """
     }
 }
 
 attribute_cpp_init = {
     'local': """
         // Local %(attr_type)s %(name)s
         %(name)s = init_matrix_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_matrix_variable_gpu<%(type)s>(%(name)s);
-        %(name)s_host_to_device = true;
+        %(name)s_host_to_device = false;
         %(name)s_device_to_host = t;
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_vector_variable_gpu<%(type)s>(%(name)s);
-        %(name)s_host_to_device = true;
+        %(name)s_host_to_device = false;
         %(name)s_device_to_host = t;
 """,
-    'global': {
+    'global': { 
         'parameter': """
-        // Global %(attr_type)s %(name)s
+        // Global parameter %(name)s
         %(name)s = 0.0;
-    """,
+""",
         'variable': """
-        // Global %(attr_type)s %(name)s
+        // Global variable %(name)s
         %(name)s = static_cast<%(type)s>(%(init)s);
         cudaMalloc((void**)&gpu_%(name)s, sizeof(%(type)s));
         %(name)s_host_to_device = true;
         %(name)s_device_to_host = t;
 """
     }
 }
@@ -160,15 +141,15 @@
     'local': """
         // %(name)s: local
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), num_non_zeros_ * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), %(name)s.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -176,15 +157,15 @@
     'semiglobal': """
         // %(name)s: semiglobal
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), post_ranks_.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), %(name)s.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -210,49 +191,30 @@
 attribute_device_to_host = {
     'local': """
         // %(name)s: local
         if ( %(name)s_device_to_host < t ) {
         #ifdef _DEBUG
             std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( %(name)s.data(), gpu_%(name)s, num_non_zeros_ * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
+            cudaMemcpy( %(name)s.data(), gpu_%(name)s, %(name)s.size() * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
         #ifdef _DEBUG
             cudaError_t err_%(name)s = cudaGetLastError();
             if ( err_%(name)s != cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
             %(name)s_device_to_host = t;
         }
 """,
-    'semiglobal': """
-            // %(name)s: semiglobal
-        #ifdef _DEBUG
-            std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
-        #endif
-            cudaMemcpy( %(name)s.data(), gpu_%(name)s, post_ranks_.size() * sizeof(%(type)s), cudaMemcpyDeviceToHost);
-        #ifdef _DEBUG
-            cudaError_t err_%(name)s = cudaGetLastError();
-            if ( err_%(name)s != cudaSuccess )
-                std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
-        #endif
-""",
-    'global': """
-            // %(name)s: global
-        #ifdef _DEBUG
-            std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
-        #endif
-            cudaMemcpy( &%(name)s, gpu_%(name)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
-        #ifdef _DEBUG
-            cudaError_t err_%(name)s = cudaGetLastError();
-            if ( err_%(name)s != cudaSuccess )
-                std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
-        #endif
-"""
+    'semiglobal': "",
+    'global': ""
 }
 
+#
+#   Synaptic delays
+#
 delay = {
     'uniform': {
         'declare': """
     // Uniform delay
     int delay ;""",
         'pyx_struct': """
         # Non-uniform delay
@@ -263,115 +225,68 @@
         'pyx_wrapper_accessor': """
     # Access to non-uniform delay
     def get_delay(self):
         return proj%(id_proj)s.delay
     def get_dendrite_delay(self, idx):
         return proj%(id_proj)s.delay
     def set_delay(self, value):
-        print("set delay", value)
-        proj%(id_proj)s.delay = value
-"""
-    },
-    'nonuniform_rate_coded': {
-        'declare': """
-    // Non-uniform delay
-    std::vector< std::vector< int > > delay ;""",
-        'pyx_struct': """
-        # Non-uniform delay
-        vector[vector[int]] delay""",
-    
-        'init': "",
-
-        'pyx_wrapper_init': """
-        proj%(id_proj)s.delay = syn.delay""",
-    
-        'pyx_wrapper_accessor': """
-    # Access to non-uniform delay
-    def get_delay(self):
-        return proj%(id_proj)s.delay
-    def get_dendrite_delay(self, idx):
-        return proj%(id_proj)s.delay[idx]
-    def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
-    },
-    'nonuniform_spiking': None
-}
-
-event_driven = {
-    'declare': """
-    std::vector< long > _last_event;
-    long* _gpu_last_event;
-""",
-    'cpp_init': """
-    _last_event = init_matrix_variable<long>(-10000);
-    _gpu_last_event = init_matrix_variable_gpu<long>(_last_event);    
-""",
-    'pyx_struct': """
-        vector[long] _last_event
-""",
-    'pyx_wrapper_init':
-"""
-        proj%(id_proj)s._last_event = vector[long]( syn._matrix.num_elements(), -10000)
-"""
+    }
 }
 
+#
+# Implement the continuous transmission for rate-code synapses.
+#
 rate_psp_kernel = {
-    # Adapted from Bell and Garland 2008, taken from https://code.google.com/archive/p/cusp-library/downloads (26. mar. 2018)
-    #
-    #   HD (2019): I needed to add a volatile variable, otherwise the results were wrong ...
-    #   HD (2020): I replaced the local reduction by a warp primitive introduced with CUDA 9.0
-    'body': {
+    'device_kernel': {
         'sum':"""
-template<unsigned int BLOCK_SIZE, unsigned int WARP_SIZE>
-__global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
-    __shared__ %(size_type)s ptrs[BLOCK_SIZE/WARP_SIZE][2];
-
-    const %(idx_type)s thread_id   = BLOCK_SIZE * blockIdx.x + threadIdx.x;  // global thread index
-    const %(idx_type)s thread_lane = threadIdx.x & (WARP_SIZE-1);            // thread index within the warp
-    const %(idx_type)s warp_id     = thread_id   / WARP_SIZE;                // global warp index
-    const %(idx_type)s warp_lane   = threadIdx.x / WARP_SIZE;                // warp index within the CTA
-    const %(idx_type)s num_warps   = (BLOCK_SIZE / WARP_SIZE) * gridDim.x;   // total number of active warps
-
-    for(%(idx_type)s row = warp_id; row < post_size; row += num_warps){
-
-        // use two threads to fetch Ap[row] and Ap[row+1]
-        // this is considerably faster than the straightforward version
-        if(thread_lane < 2)
-            ptrs[warp_lane][thread_lane] = row_ptr[row + thread_lane];
-        const %(size_type)s row_start = ptrs[warp_lane][0];                   //same as: row_start = Ap[row];
-        const %(size_type)s row_end   = ptrs[warp_lane][1];                   //same as: row_end   = Ap[row+1];
-
-        // compute local sum
-        %(float_prec)s sum = 0;
-        for(%(size_type)s j = row_start + thread_lane; j < row_end; j += WARP_SIZE)
-            sum += %(psp)s
-
-        // reduce local sums to row sum (ASSUME: warpsize 32)
-        sum = warp_reduce<%(float_prec)s, WARP_SIZE>(sum);
-
-        // first thread writes warp result
-        if (thread_lane == 0)
-            %(target_arg)s[rank_post[row]] = sum;
+__global__ void cu_proj%(id_proj)s_psp_ell(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
+    int i = blockIdx.x * blockDim.x + threadIdx.x;
+
+    while ( i < post_size ) {
+        %(idx_type)s rk_post = rank_post[i];
+        %(float_prec)s localSum = %(thread_init)s;
+
+        for (%(size_type)s j =0; j < maxnzr; j++) {
+            %(idx_type)s rk_pre = rank_pre[j*post_size+i];
+            if (rk_pre == zero_marker)
+                break;
+
+            localSum += %(psp)s
+        }
+
+        %(target_arg)s%(post_index)s += localSum;
+
+        i += gridDim.x * blockDim.x;
     }
 }
-"""
+"""        
     },
-    'header': """void launch_proj%(id)s_psp(const unsigned int nb_blocks, const unsigned int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s) {
+    cu_proj%(id_proj)s_psp_ell<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* ranks and offsets */
+        %(conn_args_call)s
+        /* computation data */
+        %(add_args_call)s
+        /* result */
+        %(target_arg_call)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
     'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        const unsigned int BLOCK_SIZE = proj%(id_proj)s._threads_per_block;
-        const unsigned int WARPS_PER_BLOCK = BLOCK_SIZE / 32;
-        const unsigned int MAX_BLOCKS = MAX_THREADS / BLOCK_SIZE;
-        const unsigned int NUM_BLOCKS = std::min(MAX_BLOCKS, DIVIDE_INTO( proj%(id_proj)s.nb_dendrites(), WARPS_PER_BLOCK));
 
-        launch_proj%(id_proj)s_psp(
-            NUM_BLOCKS, BLOCK_SIZE,
+        proj%(id_proj)s_psp(
+            /* kernel config */
+            RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block,0, proj%(id_proj)s.stream),
             /* ranks and offsets */
             %(conn_args)s
             /* computation data */
             %(add_args)s
             /* result */
             %(target_arg)s
         );
@@ -380,91 +295,219 @@
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
 """,
-    'kernel_call': """
-void launch_proj%(id_proj)s_psp(const unsigned int nb_blocks, const unsigned int threads_per_block, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
-
-    switch (threads_per_block)
-    {
-        case 64:
-        {
-            cu_proj%(id_proj)s_psp<64,32><<< nb_blocks, threads_per_block>>>(
-                /* ranks and offsets */
-                %(conn_args_call)s
-                /* computation data */
-                %(add_args_call)s
-                /* result */
-                %(target_arg_call)s
-            );
-        }break;
-
-        default:
-        {
-            std::cerr << "The kernel configuration tpb = " << threads_per_block << " is not supported" << std::endl;
-        }
-    }
-}
-""",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
         'double': {
             'sum': "0.0",
             'min': "DBL_MAX",
             'max': "DBL_MIN",
             'mean': "0.0"
         }
+    }    
+}
+
+# Update of global synaptic equations, consist of body (annarchyDevice.cu),
+# header and call semantic (take place in ANNarchyHost.cu)
+global_synapse_update = {
+    'body': """
+// gpu device kernel for projection %(id_proj)s
+__global__ void cuProj%(id_proj)s_global_step(
+    /* default params */
+    const long int t, %(float_prec)s dt
+    /* additional params */
+    %(kernel_args)s,
+    /* plasticity enabled */
+    bool plasticity 
+) {
+%(pre_loop)s
+%(global_eqs)s
+}
+""",
+    'header': """__global__ void cuProj%(id_proj)s_global_step(const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+""",
+    'call': """
+        // global update
+        cuProj%(id_proj)s_global_step<<< 1, 1, 0, proj%(id_proj)s.stream>>>(
+            /* default args*/
+            t, _dt
+            /* kernel args */
+            %(kernel_args_call)s
+            /* synaptic plasticity */
+            , proj%(id_proj)s._plasticity
+        );
+
+    #ifdef _DEBUG
+        cudaDeviceSynchronize();
+        err = cudaGetLastError();
+        if ( global_step != cudaSuccess) {
+            std::cout << "proj%(id_proj)s_step: " << cudaGetErrorString( err ) << std::endl;
+        }
+    #endif
+"""
+}
+
+# Update of semiglobal synaptic equations, consist of body (annarchyDevice.cu),
+# header and call semantic (take place in ANNarchyHost.cu)
+semiglobal_synapse_update = {
+    'body': """
+// gpu device kernel for projection %(id_proj)s
+__global__ void cuProj%(id_proj)s_semiglobal_step(
+    /* default params */
+    %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt
+    /* additional params */
+    %(kernel_args)s,
+    /* plasticity enabled */
+    bool plasticity
+) {
+    int i = threadIdx.x + blockIdx.x*blockDim.x;
+
+%(pre_loop)s
+    while ( i < post_size ) {
+%(semiglobal_eqs)s
+
+        i += gridDim.x * blockDim.x;
+    }
+}
+""",
+    'header': """__global__ void cuProj%(id_proj)s_semiglobal_step(%(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+""",
+    'call': """
+        // semiglobal update
+        cuProj%(id_proj)s_semiglobal_step<<< proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream >>>(
+            proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_ranks_,
+            /* default args*/
+            t, _dt
+            /* kernel args */
+            %(kernel_args_call)s
+            /* synaptic plasticity */
+            , proj%(id_proj)s._plasticity
+        );
+
+    #ifdef _DEBUG
+        cudaDeviceSynchronize();
+        err = cudaGetLastError();
+        if ( err != cudaSuccess) {
+            std::cout << "proj%(id_proj)s_semiglobal_step: " << cudaGetErrorString( err ) << std::endl;
+        }
+    #endif
+"""
+}
+
+# Update of local synaptic equations, consist of body (annarchyDevice.cu),
+# header and call semantic (take place in ANNarchyHost.cu)
+local_synapse_update = {
+    'body': """
+// gpu device kernel for projection %(id_proj)s
+__global__ void cuProj%(id_proj)s_local_step(
+    /* connectivity */
+    %(conn_args)s,
+    /* default params */
+    const long int t, %(float_prec)s dt
+    /* additional params */
+    %(kernel_args)s,
+    /* plasticity enabled */
+    bool plasticity 
+) {
+    int i = blockIdx.x * blockDim.x + threadIdx.x;
+%(pre_loop)s
+
+    // Updating local variables of projection %(id_proj)s
+    while ( i < post_size )
+    {
+        for ( int j = 0; j < maxnzr; j++ ) {
+            if (rank_pre[j*post_size+i] == zero_marker)
+                break;
+
+%(local_eqs)s
+        }
+
+        i += blockDim.x * gridDim.x;
     }
 }
+""",
+        'header': """__global__ void cuProj%(id_proj)s_local_step(%(conn_args)s, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+""",
+        'call': """
+        // local update
+        cuProj%(id_proj)s_local_step<<< 1, 32, 0, proj%(id_proj)s.stream >>>(
+            /* default args*/
+            %(conn_args_call)s
+            /* default args*/
+            , t, _dt
+            /* kernel args */
+            %(kernel_args_call)s
+            /* synaptic plasticity */
+            , proj%(id_proj)s._plasticity
+        );
+
+    #ifdef _DEBUG
+        cudaDeviceSynchronize();
+        err = cudaGetLastError();
+        if ( err != cudaSuccess) {
+            std::cout << "proj%(id_proj)s_step: " << cudaGetErrorString( err ) << std::endl;
+        }
+    #endif
+""",
+}
+
+# call semantic for global, semiglobal and local kernel
+synapse_update_call = """
+    // proj%(id_proj)s: pop%(pre)s -> pop%(post)s
+    if ( proj%(id_proj)s._transmission && proj%(id_proj)s._update && proj%(id_proj)s._plasticity && ( (t - proj%(id_proj)s._update_offset)%%proj%(id_proj)s._update_period == 0L)) {
+        %(float_prec)s _dt = dt * proj%(id_proj)s._update_period;
+#ifdef _DEBUG
+    cudaError_t err;
+#endif
+%(global_call)s
+int nb_blocks;
+%(semiglobal_call)s
+%(local_call)s
+    }
+"""
 
 conn_templates = {
     # connectivity representation
-    'conn_header' : "const %(idx_type)s post_size, const %(idx_type)s* __restrict__  rank_post, const %(size_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ rank_pre",
-    'conn_call' : "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank, proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank",
-    'conn_kernel': "post_size, rank_post, row_ptr, rank_pre",
+    'conn_header': "const %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const %(idx_type)s* __restrict__ rank_pre, const %(idx_type)s maxnzr, const %(idx_type)s zero_marker",
+    'conn_call': "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_ranks_, proj%(id_proj)s.gpu_col_idx_, proj%(id_proj)s.get_maxnzr(), std::numeric_limits<%(idx_type)s>::max()",
+    'conn_kernel': "post_size, rank_post, rank_pre, maxnzr, zero_marker",
 
     # launch config
     'launch_config': launch_config,
-
+ 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
-    'attribute_cpp_delete':attribute_cpp_delete,
+    'attribute_cpp_delete': attribute_cpp_delete,
     'host_to_device': attribute_host_to_device,
     'device_to_host': attribute_device_to_host,
     'delay': delay,
-    'event_driven': event_driven,
 
     # operations
     'rate_psp': rate_psp_kernel,
-    'spike_transmission': {
-        'event_driven': None,
-        'continous': None,
-    },
     'synapse_update': {
-        'global': None,
-        'semiglobal': None,
-        'local': None,
-        'call': None
-    },
-    'post_event': None
+        'global': global_synapse_update,
+        'semiglobal': semiglobal_synapse_update,
+        'local': local_synapse_update,
+        'call': synapse_update_call
+    }
 }
 
 conn_ids = {
-    'local_index': "[j]",
+    'local_index': "[j*post_size+i]",
     'semiglobal_index': '[i]',
     'global_index': '[0]',
-    'pre_index': '[rank_pre[j]]',
-    'post_index': '[rank_post[i]]',
+    'pre_index': '[rk_pre]',
+    'post_index': '[rk_post]',
     'pre_prefix': 'pre_',
-    'post_prefix': 'post_',
-    'delay_nu' : '[delay[j]-1]', # non-uniform delay
+    'post_prefix': 'post_'
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/Dense.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/ELLR.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,131 +1,121 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
-# (directly imported by CodeGenerator if needed)
 additional_global_functions = ""
 
 launch_config = {
     'init': """
-        _threads_per_block = 0;
-        _nb_blocks = 0;
+        _threads_per_block = 32;
+        auto tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)));
+        _nb_blocks = std::min<unsigned int>(tmp_blocks, 65535);
 
     #ifdef _DEBUG
-        std::cout << "Kernel configuration is a fixed 2D kernel" << std::endl;
+        std::cout << "Initial kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """,
     'update': """
-        // Generate the kernel launch configuration
-        _threads_per_block = 0;
-        _nb_blocks = 0;
+        if (nb_blocks != -1) {
+            _nb_blocks = static_cast<unsigned int>(nb_blocks);
+            _threads_per_block = threads_per_block;
+        }else{
+            _threads_per_block = threads_per_block;
+            auto tmp_blocks = static_cast<unsigned int>(ceil(static_cast<double>(nb_dendrites())/static_cast<double>(_threads_per_block)));
+            _nb_blocks = std::min<unsigned int>(tmp_blocks, 65535);
+        }
 
     #ifdef _DEBUG
-        std::cout << "Kernel configuration is a fixed 2D kernel" << std::endl;
+        std::cout << "Updated kernel configuration: " << _nb_blocks << ", " << _threads_per_block << std::endl;
     #endif
 """
 }
 
 attribute_decl = {
     'local': """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """,
     'semiglobal': """
     // Semiglobal %(attr_type)s %(name)s
     std::vector< %(type)s >  %(name)s ;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """,
     'global': {
-        'parameter': """
-    // Global %(attr_type)s %(name)s
+        'parameter':
+    """
+    // Global parameter %(name)s
     %(type)s %(name)s;
 """,
         'variable': """
-    // Global %(attr_type)s %(name)s
+    // Global variable %(name)s
     %(type)s %(name)s;
     %(type)s* gpu_%(name)s;
-    long int %(name)s_device_to_host;
     bool %(name)s_host_to_device;
+    long int %(name)s_device_to_host;
 """
     }
 }
 
-
 attribute_cpp_init = {
-    'local':
-"""
+    'local': """
         // Local %(attr_type)s %(name)s
-        %(name)s = init_matrix_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
+        %(name)s = init_matrix_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_matrix_variable_gpu<%(type)s>(%(name)s);
-        %(name)s_host_to_device = true;
+        %(name)s_host_to_device = false;
         %(name)s_device_to_host = t;
 """,
-    'semiglobal':
-"""
+    'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
-        %(name)s = init_vector_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
+        %(name)s = init_vector_variable<%(type)s>(%(init)s);
         gpu_%(name)s = init_vector_variable_gpu<%(type)s>(%(name)s);
-        %(name)s_host_to_device = true;
+        %(name)s_host_to_device = false;
         %(name)s_device_to_host = t;
 """,
-    'global': {
+    'global': { 
         'parameter': """
-        // Global %(attr_type)s %(name)s
+        // Global parameter %(name)s
         %(name)s = 0.0;
-    """,
+""",
         'variable': """
-        // Global %(attr_type)s %(name)s
+        // Global variable %(name)s
         %(name)s = static_cast<%(type)s>(%(init)s);
         cudaMalloc((void**)&gpu_%(name)s, sizeof(%(type)s));
         %(name)s_host_to_device = true;
         %(name)s_device_to_host = t;
 """
     }
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
+        size_in_bytes += sizeof(bool);
+        size_in_bytes += sizeof(%(ctype)s*);
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
+        size_in_bytes += sizeof(bool);
+        size_in_bytes += sizeof(%(ctype)s*);
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
-        // Global %(attr_type)s %(name)s
+        // Global
+        size_in_bytes += sizeof(bool);
+        size_in_bytes += sizeof(%(ctype)s*);
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
         // %(name)s - host
@@ -150,15 +140,15 @@
     'local': """
         // %(name)s: local
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), this->num_rows_ * this->num_columns_ * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), %(name)s.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -166,15 +156,15 @@
     'semiglobal': """
         // %(name)s: semiglobal
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( gpu_%(name)s, %(name)s.data(), this->num_rows_ * sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, %(name)s.data(), %(name)s.size() * sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -182,15 +172,15 @@
     'global': """
         // %(name)s: global
         if ( %(name)s_host_to_device )
         {
         #ifdef _DEBUG
             std::cout << "HtoD: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            //cudaMemcpy( gpu_%(name)s, &%(name)s, sizeof( %(type)s ), cudaMemcpyHostToDevice);
+            cudaMemcpy( gpu_%(name)s, &%(name)s, sizeof( %(type)s ), cudaMemcpyHostToDevice);
             %(name)s_host_to_device = false;
         #ifdef _DEBUG
             cudaError_t err = cudaGetLastError();
             if ( err!= cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err) << std::endl;
         #endif
         }
@@ -200,132 +190,96 @@
 attribute_device_to_host = {
     'local': """
         // %(name)s: local
         if ( %(name)s_device_to_host < t ) {
         #ifdef _DEBUG
             std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
         #endif
-            cudaMemcpy( %(name)s.data(), gpu_%(name)s, num_rows_ * num_columns_ * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
+            cudaMemcpy( %(name)s.data(), gpu_%(name)s, %(name)s.size() * sizeof( %(type)s ), cudaMemcpyDeviceToHost);
         #ifdef _DEBUG
             cudaError_t err_%(name)s = cudaGetLastError();
             if ( err_%(name)s != cudaSuccess )
                 std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
         #endif
             %(name)s_device_to_host = t;
         }
 """,
-    'semiglobal': """
-            // %(name)s: semiglobal
-        #ifdef _DEBUG
-            std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
-        #endif
-            //cudaMemcpy( %(name)s.data(), gpu_%(name)s, post_ranks_.size() * sizeof(%(type)s), cudaMemcpyDeviceToHost);
-        #ifdef _DEBUG
-            cudaError_t err_%(name)s = cudaGetLastError();
-            if ( err_%(name)s != cudaSuccess )
-                std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
-        #endif
-""",
-    'global': """
-            // %(name)s: global
-        #ifdef _DEBUG
-            std::cout << "DtoH: %(name)s ( proj%(id)s )" << std::endl;
-        #endif
-            //cudaMemcpy( &%(name)s, gpu_%(name)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
-        #ifdef _DEBUG
-            cudaError_t err_%(name)s = cudaGetLastError();
-            if ( err_%(name)s != cudaSuccess )
-                std::cout << "  error: " << cudaGetErrorString(err_%(name)s) << std::endl;
-        #endif
-"""
+    'semiglobal': "",
+    'global': ""
 }
 
+#
+#   Synaptic delays
+#
 delay = {
     'uniform': {
         'declare': """
     // Uniform delay
     int delay ;""",
-
-        'pyx_struct':
-"""
-        # Uniform delay
+        'pyx_struct': """
+        # Non-uniform delay
         int delay""",
-        'init': """
-    delay = delays[0][0];
-""",
-        'pyx_wrapper_init':
-"""
+        'init': "delay = delays[0][0];",
+        'pyx_wrapper_init': """
         proj%(id_proj)s.delay = syn.uniform_delay""",
-        'pyx_wrapper_accessor':
-"""
+        'pyx_wrapper_accessor': """
     # Access to non-uniform delay
     def get_delay(self):
         return proj%(id_proj)s.delay
     def get_dendrite_delay(self, idx):
         return proj%(id_proj)s.delay
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
     }
 }
 
 #
-# Implement the continuous transmission for rate-coded synapses.
+# Implement the continuous transmission for rate-code synapses.
 #
 rate_psp_kernel = {
-    # Comment to if (tid < 32) block:
-    #
-    # now that we are using warp-synchronous programming (below)
-    # we need to declare our shared memory volatile so that the compiler
-    # doesn't reorder stores to it and induce incorrect behavior.
-    'body': {
+    'device_kernel': {
         'sum':"""
 __global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s ) {
-    %(idx_type)s rk_post = blockIdx.y*blockDim.y+threadIdx.y;
-    %(float_prec)s __shared__ sdata[16][32];
-    unsigned int tid = threadIdx.x;
+    int i = blockIdx.x * blockDim.x + threadIdx.x;
 
-    while( rk_post < post_size ) {
-        sdata[threadIdx.y][threadIdx.x] = 0.0;
-        %(size_type)s j = rk_post * pre_size + threadIdx.x;
+    while( i < post_size ) {
+        
+        %(float_prec)s localSum = %(thread_init)s;
 
-        for (%(idx_type)s rk_pre = threadIdx.x; rk_pre < pre_size; rk_pre+=blockDim.x, j+= blockDim.x) {
-            sdata[threadIdx.y][threadIdx.x] += %(psp)s
-        }
+        for(int j =0; j < rl[i]; j++)
+            localSum += %(psp)s
 
-        __syncthreads();
+        %(target_arg)s%(post_index)s += localSum;
 
-        // do reduction in shared mem within one warp
-        if (threadIdx.x < 16) {
-            volatile %(float_prec)s* data = sdata[threadIdx.y];
-            data[tid] += data[tid + 16];
-            data[tid] += data[tid +  8];
-            data[tid] += data[tid +  4];
-            data[tid] += data[tid +  2];
-            data[tid] += data[tid +  1];
-        }
-
-        if (threadIdx.x == 0) %(target_arg)s%(post_index)s += sdata[threadIdx.y][0];
-        __syncthreads();
-        rk_post += gridDim.y*blockDim.y;
+        i += gridDim.x * blockDim.x;
     }
 }
 """
     },
-    'header': """__global__ void cu_proj%(id)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s) {
+    cu_proj%(id_proj)s_psp<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        /* ranks and offsets */
+        %(conn_args_call)s
+        /* computation data */
+        %(add_args_call)s
+        /* result */
+        %(target_arg_call)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
     'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        // 2D-Kernel: y number rows, x number columns
-        auto num_block_rows = static_cast<%(idx_type)s>(ceil(double(proj%(id_proj)s.num_rows())/16.0));
-        auto thread_dim = dim3(32, 16, 1);
-        auto block_dim = dim3(1, num_block_rows, 1);
 
-        cu_proj%(id_proj)s_psp<<< block_dim, thread_dim>>>(
+        proj%(id_proj)s_psp(
+            RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block,0, proj%(id_proj)s.stream),
             /* ranks and offsets */
             %(conn_args)s
             /* computation data */
             %(add_args)s
             /* result */
             %(target_arg)s
         );
@@ -334,103 +288,68 @@
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
 """,
-    'kernel_call': "",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
         'double': {
             'sum': "0.0",
             'min': "DBL_MAX",
             'max': "DBL_MIN",
             'mean': "0.0"
         }
-    }
+    }    
 }
 
-spike_event_transmission = {
-    'body': """// gpu device kernel for projection %(id)s
-__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_arg)s %(kernel_args)s ) {
-    int tid = threadIdx.x;
-    int row_idx = blockIdx.x ;
-
-    while( row_idx < row_size ) {
-        int row_begin = row_idx * column_size;
-
-        for (int i = tid; i < num_events[0]; i+=blockDim.x) {
-            atomicAdd(&g_%(target)s[row_idx], w[row_begin + spiked[i]]);
-        }
-
-        row_idx += gridDim.x;
-    }
-}
-""",
-    'header': """__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_header)s %(kernel_args)s);
-""",
-    'call': """
-    if ( pop%(id_pre)s._active && (pop%(id_pre)s.spike_count > 0) && proj%(id_proj)s._transmission ) {
-        int tpb = 32;
-        int nb = proj%(id_proj)s.num_rows();
-
-        // compute psp
-        cu_proj%(id_proj)s_psp<<< nb, tpb, 0, proj%(id_proj)s.stream >>>(
-            t, dt, proj%(id_proj)s._plasticity,
-            /* pre-synaptic events */
-            pop%(id_pre)s.gpu_spiked, pop%(id_pre)s.gpu_spike_count,
-            /* connectivity */
-            %(conn_args)s
-            /* kernel config */
-            %(kernel_args)s
-        );
-    #ifdef _DEBUG
-        cudaDeviceSynchronize();
-        cudaError_t err_psp_proj%(id_proj)s = cudaGetLastError();
-        if( err_psp_proj%(id_proj)s != cudaSuccess) {
-            std::cout << "proj%(id_proj)s_psp (" << t << "): " << std::endl;
-            std::cout << "   " << cudaGetErrorString(err_psp_proj%(id_proj)s) << std::endl;
-        }
-    #endif
-    }
-"""
-}
 
 # Update of global synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 global_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_global_step(
     /* default params */
-    const long int, const %(float_prec)s dt
+    const long int t, %(float_prec)s dt
     /* additional params */
     %(kernel_args)s,
     /* plasticity enabled */
-    bool plasticity )
-{
+    bool plasticity
+) {
 %(pre_loop)s
 %(global_eqs)s
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_global_step( %(float_prec)s dt %(kernel_args)s, bool plasticity);
+    'invoke_kernel': """void proj%(id_proj)s_global_step(RunConfig cfg, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_global_step<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        /* default args*/
+        t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_global_step(RunConfig cfg, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-    'call': """
+    'host_call': """
         // global update
-        cuProj%(id_proj)s_global_step<<< 1, 1, 0, proj%(id_proj)s.stream>>>(
-            proj%(id_proj)s.nb_dendrites(),
+        proj%(id_proj)s_global_step(
+            /* kernel configuration */
+            RunConfig(1, 1, 0, proj%(id_proj)s.stream),
             /* default args*/
             t, _dt
-            /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
 
     #ifdef _DEBUG
         cudaDeviceSynchronize();
@@ -441,43 +360,61 @@
     #endif
 """
 }
 
 # Update of semiglobal synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 semiglobal_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_semiglobal_step(
+    %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post,
     /* default params */
-    const %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, const %(float_prec)s dt
+    const long int t, %(float_prec)s dt
     /* additional params */
     %(kernel_args)s,
     /* plasticity enabled */
-    bool plasticity
+    bool plasticity 
 ) {
     int i = threadIdx.x + blockIdx.x*blockDim.x;
+    
 
 %(pre_loop)s
     while ( i < post_size ) {
 %(semiglobal_eqs)s
 
         i += gridDim.x * blockDim.x;
     }
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_semiglobal_step(const %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
+    'invoke_kernel': """
+void proj%(id_proj)s_semiglobal_step(RunConfig cfg, %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_semiglobal_step<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* connectivity */
+        post_size, rank_post,
+        /* default args*/
+        t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_semiglobal_step(RunConfig cfg, %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-    'call': """
+    'host_call': """
         // semiglobal update
-        nb_blocks = ceil( %(float_prec)s(proj%(id_proj)s.nb_dendrites()) / 32.0);
-        cuProj%(id_proj)s_semiglobal_step<<< nb_blocks, 32, 0, proj%(id_proj)s.stream >>>(
-            proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_rank_,
+        proj%(id_proj)s_semiglobal_step(
+            RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream),
+            /* connectivity */
+            proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_ranks_,
             /* default args*/
-            proj%(id_proj)s.gpu_post_rank, proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank, t, _dt
+            t, dt
             /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
 
     #ifdef _DEBUG
@@ -489,75 +426,79 @@
     #endif
 """
 }
 
 # Update of local synaptic equations, consist of body (annarchyDevice.cu),
 # header and call semantic (take place in ANNarchyHost.cu)
 local_synapse_update = {
-    'body': """
+    'device_kernel': """
 // gpu device kernel for projection %(id_proj)s
 __global__ void cuProj%(id_proj)s_local_step(
     /* connectivity */
-    %(idx_type)s post_size, %(idx_type)s pre_size, char* mask,
+    %(conn_args)s,
     /* default params */
-    const long int t, const %(float_prec)s dt
+    const long int t, %(float_prec)s dt
     /* additional params */
     %(kernel_args)s,
     /* plasticity enabled */
     bool plasticity
 ) {
-    %(idx_type)s rk_post = blockIdx.x;
-    %(idx_type)s rk_pre = threadIdx.x;
-    %(size_type)s j = rk_post*pre_size+rk_pre;
-
+    int i = blockIdx.x * blockDim.x + threadIdx.x;
 %(pre_loop)s
+
     // Updating local variables of projection %(id_proj)s
-    while ( rk_pre < pre_size )
+    while ( i < post_size )
     {
-        if (mask[j]) {
+        for ( int j = 0; j < rl[i]; j++ ) {
 %(local_eqs)s
         }
 
-        j += blockDim.x;
-        rk_pre += blockDim.x;
+        i += blockDim.x * gridDim.x;
     }
 }
 """,
-    'header': """__global__ void cuProj%(id_proj)s_local_step(%(idx_type)s post_size, %(idx_type)s pre_size, char* mask, const long int t, const %(float_prec)s dt %(kernel_args)s, bool plasticity);
+    'invoke_kernel': """
+void proj%(id_proj)s_local_step(RunConfig cfg, %(conn_args)s, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity) {
+    cuProj%(id_proj)s_local_step<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        /* connectivity */
+        %(conn_args_call)s
+        /* default args*/
+        , t, dt
+        /* kernel args */
+        %(kernel_args_call)s
+        /* synaptic plasticity */
+        , plasticity
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_local_step(RunConfig cfg, %(conn_args)s, const long int t, %(float_prec)s dt %(kernel_args)s, bool plasticity);
 """,
-    'call': """
+    'host_call': """
         // local update
-    #if defined (__proj%(id_proj)s_%(target)s_tpb__)
-        cuProj%(id_proj)s_local_step<<< __proj%(id_proj)s_nb__, __proj%(id_proj)s_%(target)s_tpb__, 0, proj%(id_proj)s.stream >>>(
-            /* default args*/
-            pop%(id_post)s.size, pop%(id_pre)s.size, proj%(id_proj)s.device_mask(), t, _dt
-            /* kernel args */
-            %(kernel_args_call)s
-            /* synaptic plasticity */
-            , proj%(id_proj)s._plasticity
-        );
-    #else
-        cuProj%(id_proj)s_local_step<<< proj%(id_proj)s.nb_dendrites(), 32, 0, proj%(id_proj)s.stream >>>(
+        proj%(id_proj)s_local_step(
+            /* kernel configuration */
+            RunConfig(1, 32, 0, proj%(id_proj)s.stream),
+            /* connectivity */
+            %(conn_args_call)s
             /* default args*/
-            pop%(id_post)s.size, pop%(id_pre)s.size, proj%(id_proj)s.device_mask(), t, _dt
+            , t, _dt
             /* kernel args */
             %(kernel_args_call)s
             /* synaptic plasticity */
             , proj%(id_proj)s._plasticity
         );
-    #endif
 
     #ifdef _DEBUG
         cudaDeviceSynchronize();
         err = cudaGetLastError();
         if ( err != cudaSuccess) {
             std::cout << "proj%(id_proj)s_step: " << cudaGetErrorString( err ) << std::endl;
         }
     #endif
-""",
+"""
 }
 
 # call semantic for global, semiglobal and local kernel
 synapse_update_call = """
     // proj%(id_proj)s: pop%(pre)s -> pop%(post)s
     if ( proj%(id_proj)s._transmission && proj%(id_proj)s._update && proj%(id_proj)s._plasticity && ( (t - proj%(id_proj)s._update_offset)%%proj%(id_proj)s._update_period == 0L)) {
         %(float_prec)s _dt = dt * proj%(id_proj)s._update_period;
@@ -569,45 +510,42 @@
 %(semiglobal_call)s
 %(local_call)s
     }
 """
 
 conn_templates = {
     # connectivity representation
-    'conn_header': "const %(idx_type)s post_size, const %(idx_type)s pre_size",
-    'conn_call': "pop%(id_post)s.size, pop%(id_pre)s.size",
-    'conn_kernel': "",
+    'conn_header': "const %(idx_type)s post_size, const %(idx_type)s* __restrict__ rank_post, const %(idx_type)s* __restrict__ rank_pre, const %(idx_type)s* __restrict__ rl",
+    'conn_call': "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.gpu_post_ranks_, proj%(id_proj)s.gpu_col_idx_, proj%(id_proj)s.gpu_rl_",
+    'conn_kernel': "post_size, rank_post, rank_pre, rl",
 
     # launch config
     'launch_config': launch_config,
-
+ 
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'host_to_device': attribute_host_to_device,
     'device_to_host': attribute_device_to_host,
     'delay': delay,
 
-    #operations
+    # operations
     'rate_psp': rate_psp_kernel,
-    'spike_transmission': {
-        'event_driven': spike_event_transmission
-    },
     'synapse_update': {
         'global': global_synapse_update,
         'semiglobal': semiglobal_synapse_update,
         'local': local_synapse_update,
         'call': synapse_update_call
     }
 }
 
 conn_ids = {
-    'local_index': "[j]",
-    'semiglobal_index': '[rk_post]',
+    'local_index': "[j*post_size+i]",
+    'semiglobal_index': '[i]',
     'global_index': '[0]',
     'pre_index': '[rk_pre]',
     'post_index': '[rk_post]',
     'pre_prefix': 'pre_',
     'post_prefix': 'post_'
-}
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/Dense_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/Dense_T.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-#===============================================================================
-#
-#     Dense_T.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 # (directly imported by CodeGenerator if needed)
 additional_global_functions = ""
 
 launch_config = {
     'init': """
@@ -265,16 +246,16 @@
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
     }
 }
 
 spike_event_transmission = {
-    'body': """// gpu device kernel for projection %(id)s
-__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_arg)s %(kernel_args)s ) {
+    'device_kernel': """// gpu device kernel for projection %(id_proj)s
+__global__ void cu_proj%(id_proj)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_args_header)s %(kernel_args_header)s ) {
     int tid = threadIdx.x;
     int col_idx = blockIdx.x * blockDim.x + tid;
 
     __shared__ %(float_prec)s shared_psp[32];
     while( col_idx < row_size ) {
         shared_psp[tid] = 0.0;
 
@@ -285,23 +266,37 @@
         }
 
         g_%(target)s[col_idx] += shared_psp[tid];
         col_idx += gridDim.x * blockDim.x;
     }
 }
 """,
-    'header': """__global__ void cu_proj%(id)s_psp( const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_header)s %(kernel_args)s);
+    'invoke_kernel': """
+void proj%(id_proj)s_psp(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_args_header)s %(kernel_args_header)s) {
+    cu_proj%(id_proj)s_psp<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(
+        t, dt, plasticity,
+        /* pre-synaptic events */
+        spiked, num_events,
+        /* connectivity */
+        %(conn_args_invoke)s
+        /* kernel config */
+        %(kernel_args_invoke)s
+    );
+}
+""",
+    'kernel_decl': """void proj%(id_proj)s_psp(RunConfig cfg, const long int t, const %(float_prec)s dt, bool plasticity, int *spiked, unsigned int* num_events, %(conn_args_header)s %(kernel_args_header)s);
 """,
-    'call': """
+    'host_call': """
     if ( pop%(id_pre)s._active && (pop%(id_pre)s.spike_count > 0) && proj%(id_proj)s._transmission ) {
         int tpb = 32;
         int nb = int(ceil(double(proj%(id_proj)s.num_rows()) / double(tpb)));
 
         // compute psp
-        cu_proj%(id_proj)s_psp<<< nb, tpb, 0, proj%(id_proj)s.stream >>>(
+        proj%(id_proj)s_psp(
+            RunConfig(nb, tpb, 0, proj%(id_proj)s.stream),
             t, dt, proj%(id_proj)s._plasticity,
             /* pre-synaptic events */
             pop%(id_pre)s.gpu_spiked, pop%(id_pre)s.gpu_spike_count,
             /* connectivity */
             %(conn_args)s
             /* kernel config */
             %(kernel_args)s
@@ -335,15 +330,16 @@
     'host_to_device': attribute_host_to_device,
     'device_to_host': attribute_device_to_host,
     'delay': delay,
 
     #operations
     'rate_psp': None,
     'spike_transmission': {
-        'event_driven': spike_event_transmission
+        'event_driven': spike_event_transmission,
+        'continuous': None
     },
     'synapse_update': {
         'global': None,
         'semiglobal': None,
         'local': None,
         'call': None
     }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/HYB.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/HYB.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-#===============================================================================
-#
-#     HYB.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 additional_global_functions = ""
 
 #TODO: maybe it would make more sense to split up the nb_blocks and tpb for ELL and COO
 launch_config = {
     'init': """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/SELL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/SELL.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,11 @@
-#===============================================================================
-#
-#     SELLR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 # Code which should be added prior to kernels
 additional_global_functions = ""
 
 init_launch_config = {
     'init': """
         // Generate the kernel launch configuration
@@ -240,17 +222,17 @@
     }
 }
 
 #
 # Implement the continuous transmission for rate-code synapses.
 #
 rate_psp_kernel = {
-    'body': {
+    'device_kernel': {
         'sum':"""
-__global__ void cu_proj%(id_proj)s_psp_sell(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s) {
+__global__ void cu_proj%(id_proj)s_psp(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s) {
     //global row
     unsigned int row = blockIdx.x * blockDim.x + threadIdx.x;   
 
     if ( row < post_size ) {
         %(float_prec)s tmp = 0.0;
         unsigned int offset = row_ptr[blockIdx.x];
         unsigned int local_max_length = (row_ptr[blockIdx.x + 1] - offset)/block_size;
@@ -261,20 +243,35 @@
             tmp += %(psp)s
         }
         %(target_arg)s%(post_index)s += tmp;
     }
 }
 """
     },
-    'header': """__global__ void cu_proj%(id)s_psp_sell(%(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
+    'invoke_kernel': """
+void call_proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s) {
+    cu_proj%(id_proj)s_psp<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(
+        /* ranks and offsets */
+        %(conn_args_call)s
+        /* computation data */
+        %(add_args_call)s
+        /* result */
+        %(target_arg_call)s
+    );
+}
+""",
+    'kernel_decl': """void call_proj%(id_proj)s_psp(RunConfig cfg, %(conn_args)s%(add_args)s, %(float_prec)s* %(target_arg)s );
 """,
     'host_call': """
     // proj%(id_proj)s: pop%(id_pre)s -> pop%(id_post)s
     if ( pop%(id_post)s._active && proj%(id_proj)s._transmission ) {
-        cu_proj%(id_proj)s_psp_sell<<< proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block >>>(
+        RunConfig proj%(id_proj)s_psp_cfg = RunConfig(proj%(id_proj)s._nb_blocks, proj%(id_proj)s._threads_per_block, 0, proj%(id_proj)s.stream);
+        call_proj%(id_proj)s_psp (
+            /* kernel config */
+            proj%(id_proj)s_psp_cfg,
             /* ranks and offsets */
             %(conn_args)s
             /* computation data */
             %(add_args)s
             /* result */
             %(target_arg)s
         );
@@ -283,15 +280,14 @@
         auto err = cudaGetLastError();
         if ( err != cudaSuccess ) {
             std::cout << "cu_proj%(id_proj)s_psp: " << cudaGetErrorString(err) << std::endl;
         }
     #endif
     }
 """,
-    'kernel_call': "",
     'thread_init': {
         'float': {
             'sum': "0.0f",
             'min': "FLT_MAX",
             'max': "FLT_MIN",
             'mean': "0.0f"
         },
@@ -304,15 +300,15 @@
     }    
 }
 
 conn_templates = {
     # connectivity representation
     'conn_header': "const %(idx_type)s post_size, const %(idx_type)s block_size, const %(size_type)s* __restrict__ row_ptr, const %(idx_type)s* __restrict__ rank_pre",
     'conn_call': "proj%(id_proj)s.nb_dendrites(), proj%(id_proj)s.get_block_size(), proj%(id_proj)s.d_row_ptr, proj%(id_proj)s.d_col_idx",
-    'conn_kernel': "",
+    'conn_kernel': "post_size, block_size, row_ptr, rank_pre",
 
     # launch config
     'launch_config': init_launch_config,
  
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDA/__init__.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDA/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/CUDAGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/CUDAGenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,24 @@
-#===============================================================================
-#
-#     CUDAGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
 """
 The CUDAGenerator is responsible for the complete code generation process
 in ANNarchy to support CUDA devices. Generate the header for a Population
 object to run either on a Nvidia GPU using Nvidia SDK > 5.0 and CC > 2.0
+
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
 """
 import re
 import ANNarchy
 
 from copy import deepcopy
 
 from ANNarchy.core import Global
 from ANNarchy.core.Population import Population
 from ANNarchy.core.PopulationView import PopulationView
+from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.generator.Utils import generate_equation_code, tabify, check_and_apply_pow_fix, determine_idx_type_for_projection
 
 from ANNarchy.generator.Population.PopulationGenerator import PopulationGenerator
 
 from ANNarchy.generator.Projection.ProjectionGenerator import ProjectionGenerator, get_bounds
 from ANNarchy.generator.Projection.CUDA import *
 
@@ -75,24 +56,25 @@
 
         # concurrent streams
         decl['cuda_stream'] = BaseTemplates.cuda_stream
 
         # Initiliaze the projection
         init_weights, init_delays, init_parameters_variables = self._init_parameters_variables(proj, single_matrix)
 
-        variables_body, variables_header, variables_call = self._update_synapse(proj)
+        variables_body, variables_invoke, variables_header, variables_call = self._update_synapse(proj)
 
         # Update the random distributions
         init_rng = self._init_random_distributions(proj)
 
         # Post event
-        post_event_body, post_event_header, post_event_call = self._post_event(proj)
+        post_event_body, post_event_invoke, post_event_header, post_event_call = self._post_event(proj)
 
         # Compute sum is the trickiest part
-        psp_header, psp_body, psp_call = self._computesum_rate(proj) if proj.synapse_type.type == 'rate' else self._computesum_spiking(proj)
+        psp_device_kernel, psp_invoke_kernel, psp_kernel_decl, psp_host_call =\
+            self._computesum_rate(proj) if proj.synapse_type.type == 'rate' else self._computesum_spiking(proj)
 
         # Detect event-driven variables
         has_event_driven = False
         for var in proj.synapse_type.description['variables']:
             if var['method'] == 'event-driven':
                 has_event_driven = True
 
@@ -121,15 +103,15 @@
             declare_connectivity_matrix = proj._specific_template['declare_connectivity_matrix']
             access_connectivity_matrix = proj._specific_template['access_connectivity_matrix']
 
         # Memory transfers
         host_device_transfer, device_host_transfer = self._memory_transfers(proj)
 
         # Memory management
-        determine_size_in_bytes = self._determine_size_in_bytes(proj)
+        size_in_bytes = self._size_in_bytes(proj)
         clear_container = self._clear_container(proj)
 
         # Local functions
         host_local_func, device_local_func = self._local_functions(proj)
         decl['parameters_variables'] += host_local_func
 
         # Profiling
@@ -191,15 +173,15 @@
             'init_parameters_variables': init_parameters_variables,
             'init_additional': init_additional,
             'init_profile': init_profile,
             'access_parameters_variables': accessor,
             'access_additional': access_additional,
             'host_to_device': host_device_transfer,
             'device_to_host': device_host_transfer,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container
         }
 
         # Store the file in generate ( will be compared with files contained
         # in build/ later on )
         with open(annarchy_dir+'/generate/net'+str(self._net_id)+'/proj'+str(proj.id)+'.hpp', 'w') as ofile:
             ofile.write(final_code)
@@ -208,27 +190,32 @@
         proj_desc = {
             'include': """#include "proj%(id)s.hpp"\n""" % {'id': proj.id},
             'extern': """extern ProjStruct%(id)s proj%(id)s;\n"""% {'id': proj.id},
             'instance': """ProjStruct%(id)s proj%(id)s;\n"""% {'id': proj.id},
             'init': """    proj%(id)s.init_projection();\n""" % {'id' : proj.id}
         }
 
-        proj_desc['psp_header'] = psp_header
-        proj_desc['psp_body'] = psp_body
-        proj_desc['psp_call'] = psp_call
-        proj_desc['custom_func'] = device_local_func
+        # synaptic transmission: continuous / pre-event
+        proj_desc['psp_device_kernel'] = psp_device_kernel
+        proj_desc['psp_invoke_kernel'] = psp_invoke_kernel
+        proj_desc['psp_kernel_decl'] = psp_kernel_decl
+        proj_desc['psp_host_call'] = psp_host_call
 
         proj_desc['update_synapse_header'] = variables_header
         proj_desc['update_synapse_body'] = variables_body
+        proj_desc['update_synapse_invoke'] = variables_invoke
         proj_desc['update_synapse_call'] = variables_call
 
         proj_desc['postevent_header'] = post_event_header
         proj_desc['postevent_body'] = post_event_body
+        proj_desc['postevent_invoke'] = post_event_invoke
         proj_desc['postevent_call'] = post_event_call
 
+        proj_desc['custom_func'] = device_local_func
+
         proj_desc['host_to_device'] = tabify("proj%(id)s.host_to_device();" % {'id':proj.id}, 1)+"\n"
         proj_desc['device_to_host'] = tabify("proj%(id)s.device_to_host();" % {'id':proj.id}, 1)+"\n"
 
         return proj_desc
 
     def _configure_template_ids(self, proj):
         """
@@ -246,14 +233,16 @@
             'id_post': proj.post.id,
             'id_pre': proj.pre.id,
             'idx_type': idx_type,
             'size_type': size_type,
             'float_prec': Global.config["precision"],
             'pre_prefix': 'pre_',
             'post_prefix': 'post_',
+            'host_pre_prefix': 'pop'+ str(proj.pre.id) + '.',
+            'host_post_prefix': 'pop'+ str(proj.post.id) + '.'
         })
 
         # Indices to access data depend on the storage format/storage order
         # Please note, that the indices stored in the template files are related
         # to rate-coded models/codes.
         if proj._storage_format == "csr":
             if proj._storage_order == "post_to_pre":
@@ -329,35 +318,53 @@
         else:
             raise Global.InvalidConfiguration("   The storage_format="+str(proj._storage_format)+" is not available on CUDA devices")
 
     def _generate_launch_config(self, proj):
         """
         TODO: multiple targets???
         """
+        if isinstance(proj, SpecificProjection):
+            # HD (24th Feb. 2023): user-defined codes has their own kernel-call statements,
+            #                      therefore this adjustment is not needed
+            return "", ""
+
         init_code = self._templates['launch_config']['init'] % {
             'id_proj': proj.id
         }
         update_code = self._templates['launch_config']['update'] % {
             'id_proj': proj.id
         }
         return init_code, update_code
 
     def _computesum_rate(self, proj):
         """
-        returns all data needed for compute postsynaptic sum kernels:
+        Returns the code templates needed to compute post-synaptic sum kernels:
 
-        header:  kernel prototypes
-        body:    kernel implementation
-        call:    kernel call
+        device_kernel:     device kernel
+        invoke_kernel:     kernel invocation
+        kernel_decl:   kernel export
+        host_call:              call invoke function 
         """
         # Specific projection
-        if 'psp_header' in proj._specific_template.keys() and \
-            'psp_body' in proj._specific_template.keys() and \
+        if 'psp_header' in proj._specific_template.keys() or \
+            'psp_body' in proj._specific_template.keys() or \
             'psp_call' in proj._specific_template.keys():
-            return proj._specific_template['psp_header'], proj._specific_template['psp_body'], proj._specific_template['psp_call']
+
+            try:
+                device_kernel_header = proj._specific_template['psp_header']
+                kernel_invoke = proj._specific_template['psp_invoke']
+                device_kernel = proj._specific_template['psp_body']
+                host_call = proj._specific_template['psp_call']
+            except KeyError:
+                Global._error('At least one of the following fields is missing for psp: header, invoke, body or call')
+
+            if self._prof_gen:
+                host_call = self._prof_gen.annotate_computesum_rate(proj, host_call)
+
+            return device_kernel, kernel_invoke, device_kernel_header, host_call
 
         # Dictionary of keywords to transform the parsed equations
         ids = deepcopy(self._template_ids)
 
         # Some adjustments to spare single used local variables
         if proj._storage_format == "ellr":
             ids['post_index'] = "[rank_post[i]]"
@@ -371,16 +378,15 @@
 
         #
         # Retrieve the PSP
         add_args_header = ""
         add_args_call = ""
         add_args_kernel = ""
         if not 'psp' in  proj.synapse_type.description.keys(): # default
-            psp = """%(preprefix)s.r%(pre_index)s * w%(local_index)s;"""
-
+            psp = """%(preprefix)sr%(pre_index)s * w%(local_index)s;"""
             add_args_header += "const %(float_prec)s* __restrict__ pre_r, const %(float_prec)s* __restrict__ w" % {'float_prec': Global.config['precision']}
             add_args_call = "pop%(id_pre)s.gpu_r, proj%(id_proj)s.gpu_w " % {'id_proj': proj.id, 'id_pre': proj.pre.id}
             add_args_kernel = "pre_r, w"
 
         else: # custom psp
             psp = (proj.synapse_type.description['psp']['cpp'])
 
@@ -397,19 +403,20 @@
                 add_args_kernel += ", %(name)s" % attr_ids
 
             for dep in list(set(proj.synapse_type.description['dependencies']['pre'])):
                 _, attr = PopulationGenerator._get_attr_and_type(proj.pre, dep)
                 attr_ids = {
                     'id_pre': proj.pre.id,
                     'type': attr['ctype'],
-                    'name': attr['name']
+                    'name': attr['name'],
+                    'host_pre_prefix': self._template_ids['host_pre_prefix']
                 }
 
                 add_args_header += ", const %(type)s* __restrict__ pre_%(name)s" % attr_ids
-                add_args_call += ", pop%(id_pre)s.gpu_%(name)s" % attr_ids
+                add_args_call += ", %(host_pre_prefix)sgpu_%(name)s" % attr_ids
                 add_args_kernel += ", pre_%(name)s" % attr_ids
 
         # Special case where w is a single value
         if proj._has_single_weight():
             psp = re.sub(
                 r'([^\w]+)w%\(local_index\)s',
                 r'\1w',
@@ -426,69 +433,55 @@
         conn_call = ""
 
         #
         # finish the kernel etc.
         operation = proj.synapse_type.operation
 
         if proj._storage_format != "hyb":
-            idx_type, _, size_type, _ = determine_idx_type_for_projection(proj)
-
-            id_dict = {
-                'id_proj': proj.id,
-                'id_pre': proj.pre.id,
-                'id_post': proj.post.id,
-                'idx_type': idx_type,
-                'size_type': size_type
-            }
             # connectivity
-            conn_header = self._templates['conn_header'] % id_dict
-            conn_call = self._templates['conn_call'] % id_dict
+            conn_header = self._templates['conn_header'] % ids
+            conn_call = self._templates['conn_call'] % ids
             conn_kernel = self._templates['conn_kernel']
 
-            body_code = self._templates['rate_psp']['body'][operation] % {
-                'float_prec': Global.config['precision'],
-                'idx_type': idx_type,
-                'size_type': size_type,
-                'id_proj': proj.id,
+            body_dict = deepcopy(ids)
+            body_dict.update({
+                # device function
                 'conn_args': conn_header,
                 'target_arg': "sum_"+proj.target,
                 'add_args': add_args_header,
                 'psp': psp  % ids,
                 'thread_init': self._templates['rate_psp']['thread_init'][Global.config['precision']][operation],
-                'post_index': ids['post_index']
-            }
-            body_code += self._templates['rate_psp']['kernel_call'] % {
-                'float_prec': Global.config['precision'],
-                'id_proj': proj.id,
-                'conn_args': conn_header,
-                'target_arg': "sum_"+proj.target,
-                'add_args': add_args_header,
+                # call function
                 'conn_args_call': conn_kernel,
                 'target_arg_call': ", sum_%(target)s" % {'id_post': proj.post.id, 'target': proj.target},
                 'add_args_call': add_args_kernel,
-            }
+            })
+            device_kernel = self._templates['rate_psp']['device_kernel'][operation] % body_dict
 
-            header_code = self._templates['rate_psp']['header'] % {
-                'float_prec': Global.config['precision'],
-                'id': proj.id,
-                'conn_args': conn_header,
-                'target_arg': "sum_"+proj.target,
-                'add_args': add_args_header
-            }
-            call_code = self._templates['rate_psp']['host_call'] % {
-                'id_proj': proj.id,
-                'id_pre': proj.pre.id,
-                'id_post': proj.post.id,
+            if 'invoke_kernel' in self._templates['rate_psp'].keys():
+                invoke_kernel = self._templates['rate_psp']['invoke_kernel'] % body_dict
+                kernel_decl = self._templates['rate_psp']['kernel_decl'] % body_dict
+            else:
+                invoke_kernel = ""
+                kernel_decl = self._templates['rate_psp']['kernel_decl'] % {
+                    'float_prec': Global.config['precision'],
+                    'id': proj.id,
+                    'conn_args': conn_header,
+                    'target_arg': "sum_"+proj.target,
+                    'add_args': add_args_header
+                }
+
+            host_call_dict = deepcopy(ids)
+            host_call_dict.update({
                 'conn_args': conn_call,
-                'target': proj.target,
-                'target_arg': ", pop%(id_post)s.gpu__sum_%(target)s" % {'id_post': proj.post.id, 'target': proj.target},
-                'add_args': add_args_call,
-                'float_prec': Global.config['precision'],
-                'idx_type': idx_type
-            }
+                'target_arg': ", pop%(id_post)s.gpu__sum_%(target)s" % host_call_dict,
+                'add_args': add_args_call
+            })
+            host_call = self._templates['rate_psp']['host_call'] % host_call_dict
+
         else:
             # Should be equal to ProjectionGenerator._configure_template_ids()
             idx_type, _, size_type, _ = determine_idx_type_for_projection(proj)
             id_dict = {
                 'id_proj': proj.id,
                 'id_pre': proj.pre.id,
                 'id_post': proj.post.id,
@@ -588,48 +581,54 @@
             if isinstance(proj.pre, PopulationView):
                 delayed_variables = proj.pre.population.delayed_variables
             else:
                 delayed_variables = proj.pre.delayed_variables
 
             id_pre = str(proj.pre.id)
             for var in sorted(list(set(delayed_variables))):
-                call_code = call_code.replace("pop"+id_pre+".gpu_"+var, "pop"+id_pre+".gpu_delayed_"+var+"[proj"+str(proj.id)+".delay-1]")
+                host_call = host_call.replace("pop"+id_pre+".gpu_"+var, "pop"+id_pre+".gpu_delayed_"+var+"[proj"+str(proj.id)+".delay-1]")
 
         # Profiling
         if self._prof_gen:
-            call_code = self._prof_gen.annotate_computesum_rate(proj, call_code)
+            host_call = self._prof_gen.annotate_computesum_rate(proj, host_call)
 
-        return header_code, body_code, call_code
+        return device_kernel, invoke_kernel, kernel_decl, host_call
 
     def _computesum_spiking(self, proj):
         """
         Generate code for the spike propagation. As ANNarchy supports a set of
         different data structures, this method split in up into several sub
         functions.
 
         In contrast to _computesum_rate() the spike propagation kernel need
         to implement the signal transmission (event- as well as continous)
         and also the equations filled in the 'pre-spike' field of synapse
         desctiption.
         """
-        # Specific template ?
-        if 'header' in proj._specific_template.keys() and \
-           'body' in proj._specific_template.keys() and \
-           'call' in proj._specific_template.keys():
+        if 'psp_header' in proj._specific_template.keys() or \
+            'psp_body' in proj._specific_template.keys() or \
+            'psp_call' in proj._specific_template.keys():
+
             try:
-                header = proj._specific_template['header']
-                body = proj._specific_template['body']
-                call = proj._specific_template['call']
+                device_kernel_header = proj._specific_template['psp_header']
+                kernel_invoke = proj._specific_template['psp_invoke']
+                device_kernel = proj._specific_template['psp_body']
+                host_call = proj._specific_template['psp_call']
             except KeyError:
-                Global._error('header,spike_count body and call should be overwritten')
-            return header, body, call
+                Global._error('At least one of the following fields is missing for psp: header, invoke, body or call')
+
+            if self._prof_gen:
+                host_call = self._prof_gen.annotate_computesum_rate(proj, host_call)
+
+            return device_kernel, kernel_invoke, device_kernel_header, host_call
 
         # some variables needed for the final templates
         psp_code = ""
-        kernel_args = ""
+        kernel_args_header = ""
+        kernel_args_invoke = ""
         kernel_args_call = ""
 
         pre_spike_code = ""
         kernel_deps = []
 
         if proj.max_delay > 1 and proj.uniform_delay == -1:
             Global._error("Non-uniform delays are not supported yet on GPUs.")
@@ -650,15 +649,17 @@
                     'semiglobal_index': '[post_rank]',
                     'global_index': '[0]',
                     'float_prec': Global.config['precision'],
                     'pre_index': '[row_idx[syn_idx]]',
                     'post_index': '[post_rank]',
                 })
             else:
-                raise NotImplementedError
+                ids.update({
+                    'local_index': "[syn_idx]"
+                })
 
         elif proj._storage_format == "dense":
             # HD (27th Feb. 2023): the dense matrix has no explicit indices, as the position is
             #                      computed inside the kernel.
             if proj._storage_order == "post_to_pre":
                 pass
             else:
@@ -774,129 +775,151 @@
         if has_exact:
             event_driven_code += """
     // Update the last event for the synapse
     _last_event%(local_index)s = t;
 """
 
             # event-driven requires access to last event variable
-            kernel_args += ", long* _last_event"
+            kernel_args_header += ", long* _last_event"
+            kernel_args_invoke += ", _last_event"
             kernel_args_call += ", proj%(id_proj)s._gpu_last_event"  % ids
 
         # Add pre- and post-synaptic population dependencies
         pre_post_deps = list(set(proj.synapse_type.description['dependencies']['pre'] + proj.synapse_type.description['dependencies']['post']))
         pre_post_args = self._gen_kernel_args(proj, pre_post_deps, pre_post_deps)
-        kernel_args += pre_post_args[0]
-        kernel_args_call += pre_post_args[1]
+        kernel_args_header += pre_post_args[0]
+        kernel_args_invoke += pre_post_args[1]
+        kernel_args_call += pre_post_args[2]
+
+        # sort out doublings
+        kernel_deps = sorted(list(set(kernel_deps)))
 
         # Add synaptic variables to kernel arguments
-        kernel_deps = list(set(kernel_deps)) # sort out doublings
         for dep in kernel_deps:
             if dep == "w" or dep == "g_target":
                 # already contained
                 continue
 
             attr_type, attr_dict = self._get_attr_and_type(proj, dep)
             attr_ids = {
                 'id_proj': proj.id,
                 'name': attr_dict['name'],
                 'type': attr_dict['ctype']
             }
 
             if attr_type == 'par' and attr_dict['locality'] == "global":
-                kernel_args += ", const %(type)s %(name)s" % attr_ids
+                kernel_args_header += ", const %(type)s %(name)s" % attr_ids
+                kernel_args_invoke += ", %(name)s" % attr_ids
                 kernel_args_call += ", proj%(id_proj)s.%(name)s" % attr_ids
 
                 # replace any occurences of this parameter
                 if event_driven_code.strip() != '':
                     event_driven_code = event_driven_code.replace(attr_dict['name']+'%(global_index)s', attr_dict['name'])
                 if pre_spike_code.strip() != '':
                     pre_spike_code = pre_spike_code.replace(attr_dict['name']+'%(global_index)s', attr_dict['name'])
             else:
-                kernel_args += ", %(type)s* %(name)s" % attr_ids
+                kernel_args_header += ", %(type)s* %(name)s" % attr_ids
+                kernel_args_invoke += ", %(name)s" % attr_ids
                 kernel_args_call += ", proj%(id_proj)s.gpu_%(name)s" % attr_ids
 
-        #
-        # Finally, fill the templates,
-        # we start with the event-driven component.
+        # PSP targets
+        targets_call = ""
+        targets_invoke = ""
+        targets_header = ""
+        target_list = proj.target if isinstance(proj.target, list) else [proj.target]
+        for target in target_list:
+            targets_call += ", pop%(id_post)s.gpu_g_"+target
+            targets_invoke += ", g_"+target
+            targets_header += (", %(float_prec)s* g_"+target) % {'float_prec': Global.config['precision']}
+
+        # Construct code for event-driven transmission
         #
         if len(pre_spike_code) == 0 and len(psp_code) == 0:
-            header = ""
-            body = ""
-            call = ""
+            # no event-driven component detected
+            device_kernel = ""
+            invoke_kernel = ""
+            kernel_decl = ""
+            host_call= ""
+
         else:
             # select the correct template
             template = self._templates['spike_transmission']['event_driven']
 
             # Connectivity description, we need to read-out the view
             # which represents the pre-synaptic entries which means
             # columns in post-to-pre and rows for pre-to-post orientation.
             if proj._storage_format == "csr":
                 if proj._storage_order == "post_to_pre":
-                    conn_header = "%(size_type)s* col_ptr, %(idx_type)s* row_idx, %(idx_type)s* inv_idx, %(float_prec)s *w" % ids
+                    conn_args_header = "%(size_type)s* col_ptr, %(idx_type)s* row_idx, %(idx_type)s* inv_idx, %(float_prec)s *w" % ids
+                    conn_args_invoke = "col_ptr, row_idx, inv_idx, w"
                     conn_call = "proj%(id_proj)s.gpu_col_ptr, proj%(id_proj)s.gpu_row_idx, proj%(id_proj)s.gpu_inv_idx, proj%(id_proj)s.gpu_w" % ids
                 else:
-                    conn_header = "%(size_type)s* row_ptr, %(idx_type)s* col_idx, %(float_prec)s *w" % ids
+                    conn_args_header = "%(size_type)s* row_ptr, %(idx_type)s* col_idx, %(float_prec)s *w" % ids
+                    conn_args_invoke = "row_ptr, col_idx, w"
                     conn_call = "proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_col_idx, proj%(id_proj)s.gpu_w" % ids
             elif proj._storage_format == "dense":
-                conn_header = "const %(idx_type)s row_size, const %(idx_type)s column_size, const %(float_prec)s *w" % ids
+                conn_args_header = "const %(idx_type)s row_size, const %(idx_type)s column_size, %(float_prec)s *w" % ids
+                conn_args_invoke = "row_size, column_size, w"
                 conn_call = "proj%(id_proj)s.num_rows(), proj%(id_proj)s.num_columns(), proj%(id_proj)s.gpu_w" % ids
             else:
                 raise NotImplementedError
 
             # Population sizes
             pre_size = proj.pre.size if isinstance(proj.pre, Population) else proj.pre.population.size
             post_size = proj.post.size if isinstance(proj.post, Population) else proj.post.population.size
 
-            # PSP targets
-            targets_call = ""
-            targets_header = ""
-            target_list = proj.target if isinstance(proj.target, list) else [proj.target]
-            for target in target_list:
-                targets_call += ", pop%(id_post)s.gpu_g_"+target
-                targets_header += (", %(float_prec)s* g_"+target) % {'float_prec': Global.config['precision']}
-
             # Delays
             if proj.max_delay > 1:
                 if proj.uniform_delay == -1: # Non-uniform delays
                     raise NotImplementedError
                 else:
                     pre_spike_events = "pop%(id_pre)s.gpu_delayed_spiked[proj%(id_proj)s.delay-1]" % {'id_pre': proj.pre.id, 'id_proj': proj.id}
                     pre_spike_count = "pop%(id_pre)s.host_delayed_num_events[proj%(id_proj)s.delay-1]" % {'id_pre': proj.pre.id, 'id_proj': proj.id}
             else:
                 pre_spike_events = "pop%(id_pre)s.gpu_spiked" % {'id_pre': proj.pre.id}
                 pre_spike_count = "pop%(id_pre)s.spike_count" % {'id_pre': proj.pre.id}
 
-            # finalize call, body and header
-            call = template['call'] % {
+            # Finalize event-driven part
+            device_kernel = template['device_kernel'] % {
                 'id_proj': proj.id,
-                'id_pre': proj.pre.id,
-                'id_post': proj.post.id,
-                'target': target_list[0],
-                'pre_spike_events': pre_spike_events,
-                'pre_spike_count': pre_spike_count,
-                'kernel_args': kernel_args_call  % {'id_post': proj.post.id, 'target': target},
-                'conn_args': conn_call + targets_call % {'id_post': proj.post.id}
-            }
-            body = template['body'] % {
-                'id': proj.id,
                 'float_prec': Global.config['precision'],
-                'conn_arg': conn_header + targets_header,
-                'kernel_args': kernel_args,
+                'conn_args_header': conn_args_header + targets_header,
+                'kernel_args_header': kernel_args_header,
                 'event_driven': tabify(event_driven_code % ids, 2),
                 'psp': tabify(psp_code, 3),
                 'pre_event': tabify(pre_spike_code % ids, 3),
                 'pre_size': pre_size,
                 'post_size': post_size,
                 'target': target_list[0]  # only for dense!
             }
-            header = template['header'] % {
-                'id': proj.id,
+            invoke_kernel = template['invoke_kernel'] % {
+                'id_proj': proj.id,
+                'float_prec': Global.config['precision'],
+                'conn_args_header': conn_args_header + targets_header,
+                'conn_args_invoke': conn_args_invoke + targets_invoke,
+                'kernel_args_header': kernel_args_header,
+                'kernel_args_invoke': kernel_args_invoke,
+                'pre_spike_events': pre_spike_events.replace("pop"+str(proj.pre.id)+".gpu_", ""),
+                'pre_spike_count': pre_spike_count.replace("pop"+str(proj.pre.id)+".", ""),
+            }
+            kernel_decl = template['kernel_decl'] % {
+                'id_proj': proj.id,
                 'float_prec': Global.config['precision'],
-                'conn_header': conn_header + targets_header,
-                'kernel_args': kernel_args
+                'conn_args_header': conn_args_header + targets_header,
+                'kernel_args_header': kernel_args_header
+            }
+            host_call = template['host_call'] % {
+                'id_proj': proj.id,
+                'id_pre': proj.pre.id,
+                'id_post': proj.post.id,
+                'target': target_list[0],
+                'pre_spike_events': pre_spike_events,
+                'pre_spike_count': pre_spike_count,
+                'kernel_args': kernel_args_call  % {'id_post': proj.post.id, 'target': target},
+                'conn_args': conn_call + targets_call % {'id_post': proj.post.id}
             }
 
         # If the synaptic transmission is not event-based,
         # we need to add a rate-coded-like kernel.
         if 'psp' in  proj.synapse_type.description.keys():
             # transfrom psp equation
             psp_code = proj.synapse_type.description['psp']['cpp']
@@ -919,51 +942,61 @@
 
                 _, attr = self._get_attr_and_type(proj, dep)
                 attr_ids = {
                     'id_proj': proj.id,
                     'type': attr['ctype'],
                     'name': attr['name']
                 }
-                kernel_args += ", %(type)s* %(name)s" % attr_ids
+                kernel_args_header += ", %(type)s* %(name)s" % attr_ids
+                kernel_args_invoke += ", %(name)s" % attr_ids
                 kernel_args_call += ", proj%(id_proj)s.gpu_%(name)s" % attr_ids
 
             psp_code = proj.synapse_type.description['psp']['cpp'] % ids
 
             # select the correct template
-            template = self._templates['spike_transmission']['continous']
+            template = self._templates['spike_transmission']['continuous']
 
-            call += template['call'] % {
+            host_call += template['host_call'] % {
                 'id_proj': proj.id,
                 'id_pre': proj.pre.id,
                 'id_post': proj.post.id,
-                'target_arg': ', pop%(id_post)s.gpu_g_%(target)s' % {'id_post': proj.post.id, 'target': proj.target},
+                'target_arg': targets_call % {'id_post': proj.post.id},
                 'target': proj.target,
                 'kernel_args': kernel_args_call,
                 'float_prec': Global.config['precision']
             }
-            body += template['body'] % {
+            device_kernel += template['device_kernel'] % {
                 'id_proj': proj.id,
-                'target_arg': proj.target,
-                'kernel_args':  kernel_args,
+                'target_arg': target_list[0],
+                'kernel_args': kernel_args_header,
                 'psp': psp_code,
                 'pre_code': tabify(pre_spike_code % ids, 3),
                 'float_prec': Global.config['precision']
             }
-            header += template['header'] % {
-                'id': proj.id,
-                'kernel_args': kernel_args,
-                'target_arg': 'g_'+proj.target,
+            invoke_kernel += template['invoke_kernel'] % {
+                'id_proj': proj.id,
+                'target_arg': proj.target,
+                'kernel_args': kernel_args_header,
+                'kernel_args_invoke': kernel_args_invoke,
+                'target_arg': targets_header,
+                'target_arg_invoke': targets_invoke,
+                'float_prec': Global.config['precision']
+            }
+            kernel_decl += template['kernel_decl'] % {
+                'id_proj': proj.id,
+                'kernel_args': kernel_args_header,
+                'target_arg': targets_header,
                 'float_prec': Global.config['precision']
             }
 
         # Annotate code
         if self._prof_gen:
-            call = self._prof_gen.annotate_computesum_spiking(proj, call)
+            host_call = self._prof_gen.annotate_computesum_spiking(proj, host_call)
 
-        return header, body, call
+        return device_kernel, invoke_kernel, kernel_decl, host_call
 
 
     def _declaration_accessors(self, proj, single_matrix):
         """
         Extend basic declaration statements by CUDA streams.
         """
         declaration, accessor = ProjectionGenerator._declaration_accessors(self, proj, single_matrix)
@@ -1018,113 +1051,124 @@
         to be extended with the additional variables.
 
         Parameters:
 
         * proj: currently processed projection object
         * pop_deps: list of of variable names which are either from pre- or post-synaptic populations
         * deps: list of all attribute names which are dependencies
+
+        Returns (3 strings): kernel_args_decl, kernel_args_invoke, kernel_args_call
         """
-        kernel_args = ""
+        kernel_args_decl = ""
+        kernel_args_invoke = ""
         kernel_args_call = ""
 
         for dep in deps:
             # The variable dep is part of pre-/post population
             if dep in pop_deps:
 
                 if dep in proj.synapse_type.description['dependencies']['pre']:
                     attr_type, attr_dict = PopulationGenerator._get_attr_and_type(proj.pre, dep)
                     ids = {
                         'type': attr_dict['ctype'],
                         'name': attr_dict['name'],
                         'id': proj.pre.id
                     }
-                    kernel_args += ", %(type)s* pre_%(name)s" % ids
+                    kernel_args_decl += ", %(type)s* pre_%(name)s" % ids
+                    kernel_args_invoke += ", pre_%(name)s" % ids
                     kernel_args_call += ", pop%(id)s.gpu_%(name)s" % ids
 
                 if dep in proj.synapse_type.description['dependencies']['post']:
                     attr_type, attr_dict = PopulationGenerator._get_attr_and_type(proj.post, dep)
                     ids = {
                         'type': attr_dict['ctype'],
                         'name': attr_dict['name'],
                         'id': proj.post.id
                     }
-                    kernel_args += ", %(type)s* post_%(name)s" % ids
+                    kernel_args_decl += ", %(type)s* post_%(name)s" % ids
+                    kernel_args_invoke += ", post_%(name)s" % ids
                     kernel_args_call += ", pop%(id)s.gpu_%(name)s" % ids
 
             # The variable dep is part of the projection
             else:
                 attr_type, attr_dict = ProjectionGenerator._get_attr_and_type(proj, dep)
 
                 if attr_type == "par":
                     ids = {
                         'id_proj': proj.id,
                         'type': attr_dict['ctype'],
                         'name': attr_dict['name']
                     }
 
                     if dep in proj.synapse_type.description['global']:
-                        kernel_args += ", const %(type)s %(name)s" % ids
+                        kernel_args_decl += ", const %(type)s %(name)s" % ids
+                        kernel_args_invoke += ", %(name)s" % ids
                         kernel_args_call += ", proj%(id_proj)s.%(name)s" % ids
                     else:
-                        kernel_args += ", %(type)s* %(name)s" % ids
+                        kernel_args_decl += ", %(type)s* %(name)s" % ids
+                        kernel_args_invoke += ", %(name)s" % ids
                         kernel_args_call += ", proj%(id_proj)s.gpu_%(name)s" % ids
 
-
                 elif attr_type == "var":
                     ids = {
                         'id_proj': proj.id,
                         'type': attr_dict['ctype'],
                         'name': attr_dict['name']
                     }
-                    kernel_args += ", %(type)s* %(name)s" % ids
+                    kernel_args_decl += ", %(type)s* %(name)s" % ids
+                    kernel_args_invoke += ", %(name)s" % ids
                     kernel_args_call += ", proj%(id_proj)s.gpu_%(name)s" % ids
 
                 elif attr_type == "rand":
                     ids = {
                         'id_proj': proj.id,
                         'type': 'curandState',
                         'name': attr_dict['name']
                     }
-                    kernel_args += ", %(type)s* state_%(name)s" % ids
+                    kernel_args_decl += ", %(type)s* state_%(name)s" % ids
+                    kernel_args_invoke += ", state_%(name)s" % ids
                     kernel_args_call += ", proj%(id_proj)s.gpu_%(name)s" % ids
                 else:
                     raise ValueError("attr_type for variable " + dep +" is invalid")
 
         #
         # global operations related to pre- and post-synaptic operations
         for glop in proj.synapse_type.description['pre_global_operations']:
             attr = PopulationGenerator._get_attr(proj.pre, glop['variable'])
             ids = {
                 'id': proj.pre.id,
                 'name': glop['variable'],
                 'type': attr['ctype'],
                 'func': glop['function']
             }
-            kernel_args += ", %(type)s pre__%(func)s_%(name)s" % ids
+            kernel_args_decl += ", %(type)s pre__%(func)s_%(name)s" % ids
+            kernel_args_invoke += ", pre__%(func)s_%(name)s" % ids
             kernel_args_call += ", pop%(id)s._%(func)s_%(name)s" % ids
 
         for glop in proj.synapse_type.description['post_global_operations']:
             attr = PopulationGenerator._get_attr(proj.post, glop['variable'])
             ids = {
                 'id': proj.post.id,
                 'name': glop['variable'],
                 'type': attr['ctype'],
                 'func': glop['function']
             }
-            kernel_args += ", %(type)s post__%(func)s_%(name)s" % ids
+            kernel_args_decl += ", %(type)s post__%(func)s_%(name)s" % ids
+            kernel_args_invoke += ", post__%(func)s_%(name)s" % ids
             kernel_args_call += ", pop%(id)s._%(func)s_%(name)s" % ids
 
         #
         # event-driven spike synapses require the access to last_spike member
         # of pre- and post-synaptic populations.
         if proj.synapse_type.type == "spike":
-            kernel_args = ", long int* pre_last_spike, long int* post_last_spike" + kernel_args
+            kernel_args_decl = ", long int* pre_last_spike, long int* post_last_spike" + kernel_args_decl
+            kernel_args_invoke = ", pre_last_spike, post_last_spike" + kernel_args_invoke
             kernel_args_call = ", pop%(id_pre)s.gpu_last_spike, pop%(id_post)s.gpu_last_spike" % {'id_pre': proj.pre.id, 'id_post': proj.post.id} + kernel_args_call
 
-        return kernel_args, kernel_args_call
+        return kernel_args_decl, kernel_args_invoke, kernel_args_call
 
     def _header_structural_plasticity(self, proj):
         Global._error("Structural Plasticity is not supported on GPUs yet.")
 
     def _local_functions(self, proj):
         """
         Definition of user-defined local functions attached to
@@ -1262,49 +1306,39 @@
         return loc_eqs, glob_eqs
 
     def _post_event(self, proj):
         """
         Post-synaptic event kernel for CUDA devices
         """
         if proj.synapse_type.type == "rate":
-            return "", "", ""
+            return "", "", "", ""
 
         if proj.synapse_type.description['post_spike'] == []:
-            return "", "", ""
+            return "", "", "", ""
 
         # Get basic template ids
         ids = deepcopy(self._template_ids)
 
-        # Adjust the ids if necessary
-        if proj._storage_format == "csr":
-            ids.update({
-                'local_index': "[j]",
-                'semiglobal_index': '[i]',
-                'global_index': '[0]',
-                'pre_index': '[col_idx[j]]',
-                'post_index': '[post_rank[i]]',
-            })
-        else:
-            raise NotImplementedError
-
         add_args_header = ""
+        add_args_invoke = ""
         add_args_call = ""
 
         # Event-driven integration
         has_event_driven = False
         for var in proj.synapse_type.description['variables']:
             if var['method'] == 'event-driven':
                 has_event_driven = True
 
         # Generate event-driven code
         event_driven_code = ""
         event_deps = []
         if has_event_driven:
             # event-driven rely on last pre-synaptic event
             add_args_header += ", long* _last_event"
+            add_args_invoke += ", _last_event"
             add_args_call += ", proj%(id_proj)s._gpu_last_event" % {'id_proj': proj.id}
 
             for var in proj.synapse_type.description['variables']:
                 if var['method'] == 'event-driven':
                     event_driven_code += '// ' + var['eq'] + '\n'
                     event_driven_code += var['cpp'] + '\n'
 
@@ -1324,96 +1358,109 @@
                 post_code += "if(plasticity)\n"
             post_code += post_eq['cpp'] + '\n'
             post_code += get_bounds(post_eq) + '\n'
 
             # add dependencies, only right side!
             for deps in post_eq['dependencies']:
                 post_deps.append(deps)
+
             # left side of equations is not part of dependencies
             post_deps.append(post_eq['name'])
 
         # Create add_args for event-driven eqs and post_event
-        kernel_deps = list(set(post_deps+event_deps)) # variables can occur in several eqs
+        kernel_deps = sorted(list(set(post_deps+event_deps))) # variables can occur in several eqs
         for dep in kernel_deps:
             if dep == "w":
                 continue
 
             attr_type, attr_dict = self._get_attr_and_type(proj, dep)
             attr_ids = {
                 'id': proj.id, 'type': attr_dict['ctype'], 'name': attr_dict['name']
             }
             if attr_type == 'par' and attr_dict['locality'] == "global":
                 add_args_header += ', const %(type)s %(name)s' % attr_ids
+                add_args_invoke += ', %(name)s' % attr_ids
                 add_args_call += ', proj%(id)s.%(name)s' % attr_ids
 
                 if post_code.strip != '':
                     post_code = post_code.replace(attr_dict['name']+"%(global_index)s", attr_dict['name'])
                 if event_driven_code.strip() != '':
                     event_driven_code = event_driven_code.replace(attr_dict['name']+"%(global_index)s", attr_dict['name'])
             else:
                 add_args_header += ', %(type)s* %(name)s' % attr_ids
+                add_args_invoke += ', %(name)s' % attr_ids
                 add_args_call += ', proj%(id)s.gpu_%(name)s' % attr_ids
 
         # Check for equations which consider post-synaptic neural state variables
         for post_eq in proj.synapse_type.description['post_spike']:
+            for dep in post_eq['prepost_dependencies']['pre']:
+                attr_type, attr_dict = PopulationGenerator._get_attr_and_type(proj.pre, dep)
+                attr_ids = {
+                    'id': proj.pre.id, 'type': attr_dict['ctype'], 'name': attr_dict['name']
+                }
+                add_args_header += ', %(type)s* pre_%(name)s' % attr_ids
+                add_args_invoke += ', pre_%(name)s' % attr_ids
+                add_args_call += ', pop%(id)s.gpu_%(name)s' % attr_ids
+
             for dep in post_eq['prepost_dependencies']['post']:
                 attr_type, attr_dict = PopulationGenerator._get_attr_and_type(proj.post, dep)
                 attr_ids = {
                     'id': proj.post.id, 'type': attr_dict['ctype'], 'name': attr_dict['name']
                 }
                 add_args_header += ', %(type)s* post_%(name)s' % attr_ids
+                add_args_invoke += ', post_%(name)s' % attr_ids
                 add_args_call += ', pop%(id)s.gpu_%(name)s' % attr_ids
 
-        # Connectivity arguments
-        if proj._storage_format == "csr":
-            idx_type, _, size_type, _ = determine_idx_type_for_projection(proj)
-            conn_ids = {'idx_type': idx_type, 'size_type': size_type}
-
-            if proj._storage_order == "post_to_pre":
-                conn_header = "%(size_type)s* row_ptr, %(idx_type)s* col_idx, " % conn_ids
-                conn_call = ", proj%(id_proj)s.gpu_row_ptr, proj%(id_proj)s.gpu_pre_rank"
-            else:
-                conn_header = "%(size_type)s* col_ptr, %(idx_type)s* row_idx, " % conn_ids
-                conn_call = ", proj%(id_proj)s.gpu_col_ptr, proj%(id_proj)s.gpu_row_idx"
-
+        # select code template
+        try:
             templates = self._templates['post_event']
 
-        else:
-            raise NotImplementedError
+        except KeyError:
+            raise Global._error("No CUDA code template for post_event ( format =", proj._storage_format, " and order =", proj._storage_order,")")
+
+        # Fill code templates
+        postevent_body = templates['device_kernel'] % {
+            'id_proj': proj.id,
+            'conn_args': self._templates['conn_header'] % ids,
+            'add_args': add_args_header,
+            'event_driven': tabify(event_driven_code % ids, 2),
+            'post_code': tabify(post_code % ids, 2),
+            'float_prec': Global.config['precision'],
+        }
 
-        postevent_header = templates['header'] % {
+        postevent_invoke = templates['invoke_kernel'] % {
             'id_proj': proj.id,
-            'conn_args': conn_header,
+            'conn_args': self._templates['conn_header'] % ids,
+            'conn_args_invoke': self._templates['conn_kernel'],
             'add_args': add_args_header,
+            'add_args_invoke': add_args_invoke,
             'float_prec': Global.config['precision']
         }
 
-        postevent_body = templates['body'] % {
+        postevent_header = templates['kernel_decl'] % {
             'id_proj': proj.id,
-            'conn_args': conn_header,
+            'conn_args': self._templates['conn_header']% ids,
             'add_args': add_args_header,
-            'event_driven': tabify(event_driven_code % ids, 2),
-            'post_code': tabify(post_code % ids, 2),
             'float_prec': Global.config['precision']
         }
 
-        postevent_call = templates['call'] % {
+        postevent_call = templates['host_call'] % {
             'id_proj': proj.id,
             'id_pre': proj.pre.id,
             'id_post': proj.post.id,
             'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
-            'conn_args': conn_call % ids,
+            'conn_args': self._templates['conn_call'] % ids,
             'add_args': add_args_call
         }
 
         # Annotate code
         if self._prof_gen:
             postevent_call = self._prof_gen.annotate_post_event(proj, postevent_call)
 
-        return postevent_body, postevent_header, postevent_call
+        return postevent_body, postevent_invoke, postevent_header, postevent_call
 
     def _init_random_distributions(self, proj):
         # Random numbers
         code = ""
         if len(proj.synapse_type.description['random_distributions']) > 0:
             code += """
         // Random numbers"""
@@ -1476,20 +1523,27 @@
         .. Note:
 
         This function is a helper function and should be called by
         _update_synapse() only.
         """
         # Process equations and determine dependencies
         syn_deps, neur_deps = self._select_deps(proj, locality)
-        kernel_args, kernel_args_call = self._gen_kernel_args(proj, neur_deps, syn_deps)
+        kernel_args, kernel_args_invoke, kernel_args_call = self._gen_kernel_args(proj, neur_deps, syn_deps)
 
         # Add pre_rank/post_rank identifier if needed
         rk_assign = ""
         if locality == "semiglobal":
-            rk_assign += "%(idx_type)s rk_post = rank_post%(semiglobal_index)s;\n"
+            if proj._storage_format in ["csr"] :
+                rk_assign += "%(idx_type)s rk_post = rank_post%(semiglobal_index)s;\n"
+            elif proj._storage_format in ["ellr"]:
+                rk_assign += ""
+            elif proj._storage_format in ["dense"]:
+                rk_assign += "%(idx_type)s rk_post = i;\n"
+            else:
+                raise NotImplementedError
 
         elif locality=="local":
             # rk_pre/rk_pre depend on the matrix format
             if proj._storage_format in ["csr"] :
                 rk_assign += "%(idx_type)s rk_pre = rank_pre%(local_index)s;\n"
             elif proj._storage_format in ["dense"]:
                 pass
@@ -1520,40 +1574,40 @@
                     pre_loop = pre_loop.replace(attr_dict["name"]+"%(global_index)s", attr_dict["name"])
 
         # Finalize equations, add pre-loop and/or rank assignment
         equations = (rk_assign + equations) % ids
         if pre_loop.strip() != '':
             pre_loop = """\n// Updating the step sizes\n""" + pre_loop % ids
 
-        return equations, pre_loop, kernel_args, kernel_args_call
+        return equations, pre_loop, kernel_args, kernel_args_invoke, kernel_args_call
 
     def _update_synapse(self, proj):
         """
         Generate the device codes for synaptic equations. As the parallel
         evaluation of local and global equations within one kernel would require
         a __syncthread() call, we split up the implementation into two seperate
         parts.
 
         Return:
 
-        * a tuple contain three strings ( body, call, header )
+        * a tuple contain three strings ( device_kernel, call, header )
         """
         # Global variables
         global_eq = generate_equation_code(proj.id, proj.synapse_type.description, 'global', 'proj', padding=1, wrap_w="plasticity")
 
         # Semiglobal variables
         semiglobal_eq = generate_equation_code(proj.id, proj.synapse_type.description, 'semiglobal', 'proj', padding=2, wrap_w="plasticity")
 
         # Local variables
         pad = 2 if proj._storage_format == "csr" else 3
         local_eq = generate_equation_code(proj.id, proj.synapse_type.description, 'local', 'proj', padding=pad, wrap_w="plasticity")
 
         # Something to do?
         if global_eq.strip() == '' and semiglobal_eq.strip() == '' and local_eq.strip() == '':
-            return "", "", ""
+            return "", "", "", ""
 
         # Modify the default dictionary for specific formats
         ids = deepcopy(self._template_ids)
         if proj._storage_format == "ell":
             ids['pre_index'] = '[rk_pre]'
             ids['post_index'] = '[rk_post]'
         elif proj._storage_format == "csr":
@@ -1570,114 +1624,142 @@
             'id_post': proj.post.id,
             'float_prec': Global.config['precision'],
             'idx_type': idx_type,
             'size_type': size_type
         })
 
         # generate the code
-        body = ""
-        header = ""
+        device_kernel = ""
+        invoke_kernel = ""
+        kernel_header = ""
         local_call = ""
         global_call = ""
         semiglobal_call = ""
 
         #
         # Fill code templates for global, semiglobal and local equations
         #
         if global_eq.strip() != '':
-            global_eq, global_pre_code, kernel_args_global, kernel_args_call_global = self._process_equations( proj, global_eq, ids, 'global' )
+            global_eq, global_pre_code, kernel_args_global, kernel_args_invoke_global, kernel_args_call_global =\
+                self._process_equations( proj, global_eq, ids, 'global' )
 
         if semiglobal_eq.strip() != '':
-            semiglobal_eq, semiglobal_pre_code, kernel_args_semiglobal, kernel_args_call_semiglobal =  self._process_equations( proj, semiglobal_eq, ids, 'semiglobal' )
+            semiglobal_eq, semiglobal_pre_code, kernel_args_semiglobal, kernel_args_invoke_semiglobal, kernel_args_call_semiglobal =\
+                self._process_equations( proj, semiglobal_eq, ids, 'semiglobal' )
 
         if local_eq.strip() != '':
-            local_eq, local_pre_code, kernel_args_local, kernel_args_call_local =  self._process_equations( proj, local_eq, ids, 'local' )
+            local_eq, local_pre_code, kernel_args_local, kernel_args_invoke_local, kernel_args_call_local =\
+                self._process_equations( proj, local_eq, ids, 'local' )
 
         # replace the random distributions
         local_eq, global_eq = self._replace_random(local_eq, ids['local_index'], global_eq, proj.synapse_type.description['random_distributions'])
 
         #
         # replace local function calls
         if len(proj.synapse_type.description['functions']) > 0:
             global_eq, semiglobal_eq, local_eq = self._replace_local_funcs(proj, global_eq, semiglobal_eq, local_eq)
 
         # connectivity
         conn_header = self._templates['conn_header'] % ids
+        conn_invoke = self._templates['conn_kernel'] % ids
         conn_call = self._templates['conn_call'] % ids
 
         # we seperated the execution of global/semiglobal/local into three kernels
         # as the threads would have two different loads.
         if global_eq.strip() != '':
             body_dict = {
                 'kernel_args': kernel_args_global,
                 'global_eqs': global_eq,
                 'pre_loop':  global_pre_code,
             }
             body_dict.update(ids)
-            body += self._templates['synapse_update']['global']['body'] % body_dict
+            device_kernel += self._templates['synapse_update']['global']['device_kernel'] % body_dict
+
+            invoke_dict = {
+                'kernel_args': kernel_args_semiglobal,
+                'kernel_args_call': kernel_args_invoke_semiglobal
+            }
+            invoke_dict.update(ids)
+            invoke_kernel += self._templates['synapse_update']['global']['invoke_kernel'] % invoke_dict
 
             header_dict = {
                 'kernel_args': kernel_args_global,
             }
             header_dict.update(ids)
-            header += self._templates['synapse_update']['global']['header'] % header_dict
+            kernel_header += self._templates['synapse_update']['global']['kernel_decl'] % header_dict
 
             call_dict = deepcopy(ids)
             call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'kernel_args_call': kernel_args_call_global,
             })
-            global_call = self._templates['synapse_update']['global']['call'] % call_dict
+            global_call = self._templates['synapse_update']['global']['host_call'] % call_dict
 
         if semiglobal_eq.strip() != '':
             body_dict = {
                 'kernel_args': kernel_args_semiglobal,
                 'semiglobal_eqs': semiglobal_eq,
                 'pre_loop': semiglobal_pre_code,
             }
             body_dict.update(ids)
-            body += self._templates['synapse_update']['semiglobal']['body'] % body_dict
+            device_kernel += self._templates['synapse_update']['semiglobal']['device_kernel'] % body_dict
+
+            invoke_dict = {
+                'kernel_args': kernel_args_semiglobal,
+                'kernel_args_call': kernel_args_invoke_semiglobal
+            }
+            invoke_dict.update(ids)
+            invoke_kernel += self._templates['synapse_update']['semiglobal']['invoke_kernel'] % invoke_dict
 
             header_dict = {
                 'kernel_args': kernel_args_semiglobal,
             }
             header_dict.update(ids)
-            header += self._templates['synapse_update']['semiglobal']['header'] % header_dict
+            kernel_header += self._templates['synapse_update']['semiglobal']['kernel_decl'] % header_dict
 
             call_dict = deepcopy(ids)
             call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'kernel_args_call': kernel_args_call_semiglobal,
             })
-            semiglobal_call = self._templates['synapse_update']['semiglobal']['call'] % call_dict
+            semiglobal_call = self._templates['synapse_update']['semiglobal']['host_call'] % call_dict
 
         if local_eq.strip() != '':
             body_dict = {
                 'conn_args': conn_header,
                 'kernel_args': kernel_args_local,
                 'local_eqs': local_eq,
                 'pre_loop': tabify(local_pre_code,1)
             }
             body_dict.update(ids)
-            body += self._templates['synapse_update']['local']['body'] % body_dict
+            device_kernel += self._templates['synapse_update']['local']['device_kernel'] % body_dict
+
+            invoke_dict = {
+                'conn_args': conn_header,
+                'conn_args_call': conn_invoke,
+                'kernel_args': kernel_args_local,
+                'kernel_args_call': kernel_args_invoke_local
+            }
+            invoke_dict.update(ids)
+            invoke_kernel += self._templates['synapse_update']['local']['invoke_kernel'] % invoke_dict
 
             header_dict = {
                 'conn_args': conn_header,
                 'kernel_args': kernel_args_local
             }
             header_dict.update(ids)
-            header += self._templates['synapse_update']['local']['header'] % header_dict
+            kernel_header += self._templates['synapse_update']['local']['kernel_decl'] % header_dict
 
             call_dict = deepcopy(ids)
             call_dict.update({
                 'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
                 'conn_args_call': conn_call,
                 'kernel_args_call': kernel_args_call_local
             })
-            local_call = self._templates['synapse_update']['local']['call'] % call_dict
+            local_call = self._templates['synapse_update']['local']['host_call'] % call_dict
 
         call = self._templates['synapse_update']['call'] % {
             'id_proj': proj.id,
             'post': proj.post.id,
             'pre': proj.pre.id,
             'target': proj.target[0] if isinstance(proj.target, list) else proj.target,
             'global_call': global_call,
@@ -1686,8 +1768,8 @@
             'float_prec': Global.config['precision']
         }
 
         # Profiling
         if self._prof_gen:
             call = self._prof_gen.annotate_update_synapse(proj, call)
 
-        return body, header, call
+        return device_kernel, invoke_kernel, kernel_header, call
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/BSR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/BSR.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     BSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector<%(type)s> %(name)s;
 """,
     'semiglobal':
@@ -51,14 +34,16 @@
         // Global %(attr_type)s %(name)s
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
+        size_in_bytes += sizeof(std::vector<%(ctype)s>);
+        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
 """,
     'global': """
         // Global %(attr_type)s %(name)s
 """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/BaseTemplates.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     OpenMPTemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 projection_header = """/*
  *  ANNarchy-version: %(annarchy_version)s
  */
 #pragma once
 
 #include "ANNarchy.h"
 %(sparse_matrix_include)s
@@ -48,15 +30,15 @@
 
 %(connector_call)s
 
 %(declare_connectivity_matrix)s
 %(access_connectivity_matrix)s
 
     // Transmission and plasticity flags
-    bool _transmission, _plasticity, _update;
+    bool _transmission, _axon_transmission, _plasticity, _update;
     int _update_period;
     long int _update_offset;
 
 %(declare_delays)s
 %(declare_event_driven)s
 %(declare_rng)s
 %(declare_parameters_variables)s
@@ -74,14 +56,15 @@
     // Method called to initialize the projection
     void init_projection() {
     #ifdef _DEBUG
         std::cout << "ProjStruct%(id_proj)s::init_projection()" << std::endl;
     #endif
 
         _transmission = true;
+        _axon_transmission = true;
         _update = true;
         _plasticity = true;
         _update_period = 1;
         _update_offset = 0L;
 
         init_attributes();
 
@@ -141,15 +124,15 @@
 
     // Access additional
 %(access_additional)s
 
     // Memory management
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     // Structural plasticity
 %(creating)s
 %(pruning)s
 
@@ -184,32 +167,51 @@
         // should not happen
         std::cerr << "ProjStruct%(id_proj)s::get_local_attribute_row_%(ctype_name)s: " << name << " not found" << std::endl;
         return std::vector<%(ctype)s>();
     }
 
     %(ctype)s get_local_attribute_%(ctype_name)s(std::string name, int rk_post, int rk_pre) {
     #ifdef _DEBUG
-        std::cout << "ProjStruct%(id_proj)s::get_local_attribute_row_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<")" << std::endl;
+        std::cout << "ProjStruct%(id_proj)s::get_local_attribute_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<")" << std::endl;
     #endif
 %(local_get3)s
 
         // should not happen
-        std::cerr << "ProjStruct%(id_proj)s::get_local_attribute: " << name << " not found" << std::endl;
+        std::cerr << "ProjStruct%(id_proj)s::get_local_attribute_%(ctype_name)s: " << name << " not found" << std::endl;
         return 0.0;
     }
 
     void set_local_attribute_all_%(ctype_name)s(std::string name, std::vector<std::vector<%(ctype)s>> value) {
+    #ifdef _DEBUG
+        auto min_value = std::numeric_limits<%(ctype)s>::max();
+        auto max_value = std::numeric_limits<%(ctype)s>::min();
+        for (auto it = value.cbegin(); it != value.cend(); it++ ){
+            auto loc_min = *std::min_element(it->cbegin(), it->cend());
+            if (loc_min < min_value)
+                min_value = loc_min;
+            auto loc_max = *std::max_element(it->begin(), it->end());
+            if (loc_max > max_value)
+                max_value = loc_max;
+        }
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_all_%(ctype_name)s(name = " << name << ", min(" << name << ")=" <<std::to_string(min_value) << ", max("<<name<<")="<<std::to_string(max_value)<< ")" << std::endl;
+    #endif
 %(local_set1)s
     }
 
     void set_local_attribute_row_%(ctype_name)s(std::string name, int rk_post, std::vector<%(ctype)s> value) {
+    #ifdef _DEBUG
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_row_%(ctype_name)s(name = "<<name<<", rk_post = " << rk_post << ", min("<<name<<")="<<std::to_string(*std::min_element(value.begin(), value.end())) << ", max("<<name<<")="<<std::to_string(*std::max_element(value.begin(), value.end()))<< ")" << std::endl;
+    #endif
 %(local_set2)s
     }
 
     void set_local_attribute_%(ctype_name)s(std::string name, int rk_post, int rk_pre, %(ctype)s value) {
+    #ifdef _DEBUG
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<", value = " << std::to_string(value) << ")" << std::endl;
+    #endif
 %(local_set3)s
     }
 """,
     "semiglobal": """
     std::vector<%(ctype)s> get_semiglobal_attribute_all_%(ctype_name)s(std::string name) {
 %(semiglobal_get1)s
 
@@ -381,110 +383,13 @@
     """,
         'update': """
             %(rd_name)s = dist_%(rd_name)s(rng);
     """
     }
 }
 
-######################################
-### Dense Matrix templates
-######################################
-dense_summation_operation = {
-    'sum' : """
-%(pre_copy)s
-%(omp_code)s
-for(int i = 0; i < pop%(id_post)s.size; i++) {
-    sum = 0.0;
-    for(int j = 0; j < pop%(id_pre)s.size; j++) {
-        sum += %(psp)s ;
-    }
-    pop%(id_post)s._sum_%(target)s[i] += sum;
-}
-""",
-    'max': """
-%(pre_copy)s
-%(omp_code)s
-for(int i = 0; i < pop%(id_post)s.size; i++){
-    int j = 0;
-    sum = %(psp)s ;
-    for(int j = 1; j < pop%(id_pre)s.size; j++){
-        if(%(psp)s > sum){
-            sum = %(psp)s ;
-        }
-    }
-    pop%(id_post)s._sum_%(target)s[i] += sum;
-}
-""",
-    'min': """
-%(pre_copy)s
-%(omp_code)s
-for(int i = 0; i < pop%(id_post)s.size; i++){
-    int j= 0;
-    sum = %(psp)s ;
-    for(int j = 1; j < pop%(id_pre)s.size; j++){
-        if(%(psp)s < sum){
-            sum = %(psp)s ;
-        }
-    }
-    pop%(id_post)s._sum_%(target)s[i] += sum;
-}
-""",
-    'mean': """
-%(pre_copy)s
-%(omp_code)s
-for(int i = 0; i < pop%(id_post)s.size; i++){
-    sum = 0.0 ;
-    for(int j = 0; j < pop%(id_pre)s.size; j++){
-        sum += %(psp)s ;
-    }
-    pop%(id_post)s._sum_%(target)s[i] += sum / (double)(pop%(id_pre)s.size);
-}
-"""
-}
-
-spiking_summation_fixed_delay_dense_matrix = """
-// Event-based summation
-if (_transmission && pop%(id_post)s._active){
-    // TODO?
-} // active
-"""
-
-dense_update_variables = {
-    'local': """
-// Check periodicity
-if(_transmission && _update && pop%(id_post)s._active && ( (t - _update_offset)%%_update_period == 0L)){
-    // Global variables
-    %(global)s
-    // Local variables
-    %(omp_code)s
-    for(int i = 0; i < pop%(id_post)s.size; i++){
-        rk_post = i; // dense: ranks are indices
-        // Semi-global variables
-    %(semiglobal)s
-        for(int j = 0; j < pop%(id_pre)s.size; j++){
-            rk_pre = j; // dense: ranks are indices
-    %(local)s
-        }
-    }
-}
-""",
-    'global': """
-// Check periodicity
-if(_transmission && _update && pop%(id_post)s._active && ( (t - _update_offset)%%_update_period == 0L)){
-    // Global variables
-    %(global)s
-    // Semi-global variables
-    %(omp_code)s
-    for(int i = 0; i < pop%(id_post)s.size; i++){
-        rk_post = i;
-    %(semiglobal)s
-    }
-}
-"""
-}
-
 openmp_templates = {
     'projection_header': projection_header,
     'attr_acc': attribute_acc,
     'accessor_template': attribute_template,
     'rng': cpp_11_rng
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/COO.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_PV.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     COO.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -39,14 +22,16 @@
 }
 
 attribute_cpp_init = {
     'local':
 """
         // Local %(attr_type)s %(name)s
         %(name)s = init_matrix_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
+        if(%(name)s.empty())
+            return false;
 """,
     'semiglobal':
 """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
 """,
     'global':
@@ -56,23 +41,23 @@
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
-        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();       
+        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
-        // Global
+        // Global %(attr_type)s %(name)s
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
         // %(name)s
@@ -83,53 +68,82 @@
         // %(name)s
         %(name)s.clear();
         %(name)s.shrink_to_fit();
 """,
     'global': ""
 }
 
-###############################################################
-# Rate-coded continuous transmission
-###############################################################
-coo_summation_operation = {
-    'sum' : """
-%(pre_copy)s
-
-auto row_it = row_indices_.begin();
-auto col_it = column_indices_.begin();
-%(size_type)s nnz = nb_synapses();
-%(float_prec)s* __restrict__ target_ptr = %(post_prefix)s_sum_%(target)s.data();
-
-#pragma omp for
-for(int j = 0; j < nnz; j++) {
-    #pragma omp atomic
-    target_ptr%(post_index)s += %(psp)s;
-}
-""",
-    'max': "",
-    'min': "",
-    'mean': "",
-}
-
-###############################################################
-# Rate-coded synaptic plasticity
-###############################################################
-update_variables = {
-    'local': ""
-}
+delay = {
+    'uniform': {
+        'declare': """
+    // Uniform delay
+    int delay ;""",
+        
+        'pyx_struct':
+"""
+        # Uniform delay
+        int delay""",
+        'init': """
+    delay = delays[0][0];
+""",
+        'pyx_wrapper_init':
+"""
+        proj%(id_proj)s.delay = syn.uniform_delay""",
+        'pyx_wrapper_accessor':
+"""
+    # Access to non-uniform delay
+    def get_delay(self):
+        return proj%(id_proj)s.delay
+    def get_dendrite_delay(self, idx):
+        return proj%(id_proj)s.delay
+    def set_delay(self, value):
+        proj%(id_proj)s.delay = value
+"""
+    }
+}
+
+spiking_summation_fixed_delay = """// Event-based summation
+if (_transmission && %(post_prefix)s_active){
+
+    for (%(idx_type)s rk_post = 0; rk_post < num_rows(); rk_post++) {
+        // Iterate over all spiking neurons
+        for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
+            %(idx_type)s rk_pre = (*it);
+            if ((rk_pre < this->low_column_rank_) || (rk_pre >= this->high_column_rank_))
+                continue;
+
+            %(size_type)s j = rk_post*this->num_columns_ + *it;
+
+            %(g_target)s
+
+            if (mask_[j]) {
+                %(event_driven)s
+                %(pre_event)s
+            }
+        }
+    }
+} // active
+"""
 
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
-    
-    'rate_coded_sum': coo_summation_operation,
-    'update_variables': update_variables
+    'delay': delay,
+
+    #operations
+    'rate_coded_sum': None,
+    'vectorized_default_psp': None,
+    'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
+    'update_variables': None,
 }
 
 conn_ids = {
     'local_index': '[j]',
-    'pre_index': '[*(col_it+j)]',
-    'post_index': '[*(row_it+j)]',
-}
+    'semiglobal_index': '[rk_post]',
+    'global_index': '',
+    'post_index': '[rk_post]',
+    'pre_index': '[rk_pre]',
+    'delay_u' : '[delay-1]' # uniform delay
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_P.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_P.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     CSR_P.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< std::vector<%(type)s> > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_T.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-#===============================================================================
-#
-#     CSR_T.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/CSR_T.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,35 @@
-#===============================================================================
-#
-#     CSR_T_P.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
-    std::vector< std::vector<%(type)s> > %(name)s;
+    std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
 """
     // Semiglobal %(attr_type)s %(name)s
-    std::vector< %(type)s > %(name)s ;
+    std::vector< %(type)s >  %(name)s ;
 """,
     'global':
 """
     // Global %(attr_type)s %(name)s
     %(type)s  %(name)s ;
 """
 }
 
 attribute_cpp_init = {
     'local':
 """
         // Local %(attr_type)s %(name)s
-        %(name)s = init_matrix_variable< %(type)s, std::vector<%(type)s> >(%(init)s);
+        %(name)s = init_matrix_variable< %(type)s >(%(init)s);
 """,
     'semiglobal':
 """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable< %(type)s >(%(init)s);
 """,
     'global':
@@ -57,37 +38,31 @@
         %(name)s = %(init)s;
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
-        size_in_bytes += sizeof(std::vector<std::vector<%(ctype)s>>);
-        size_in_bytes += sizeof(std::vector<%(ctype)s>) * %(name)s.capacity();
-        for(auto it = %(name)s.cbegin(); it != %(name)s.cend(); it++)
-            size_in_bytes += (it->capacity()) * sizeof(%(ctype)s);
+        size_in_bytes += sizeof(std::vector<%(ctype)s>);
+        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();       
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
-        // Global %(attr_type)s %(name)s
+        // Global
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
         // %(name)s
-        for (auto it = %(name)s.begin(); it != %(name)s.end(); it++) {
-            it->clear();
-            it->shrink_to_fit();
-        };
         %(name)s.clear();
         %(name)s.shrink_to_fit();
 """,
     'semiglobal': """
         // %(name)s
         %(name)s.clear();
         %(name)s.shrink_to_fit();
@@ -100,16 +75,16 @@
         'declare': """
     std::vector<int> delay;
     int max_delay;
     int idx_delay;
     std::vector< std::vector< std::vector< int > > > _delayed_spikes;
 """,
         'init': """
-    delay = init_matrix_variable<int>(1);
-    update_matrix_variable_all<int>(delay, delays);
+    delay = init_variable<int>(1);
+    update_variable_all<int>(delay, delays);
 
     idx_delay = 0;
     max_delay = %(pre_prefix)smax_delay;
 """,
         'reset': """
         while(!_delayed_spikes.empty()) {
             auto elem = _delayed_spikes.back();
@@ -149,64 +124,136 @@
         proj%(id_proj)s.reset_ring_buffer()
 """
     }    
 }
 
 event_driven = {
     'declare': """
-    std::vector<std::vector<long>> _last_event;
+    std::vector<long> _last_event;
 """,
     'cpp_init': """
         // Event-driven
-        _last_event = init_matrix_variable<long, std::vector<long>>(-10000);
+        _last_event = init_matrix_variable<long>(-10000);
 """,
     'pyx_struct': """
         vector[vector[long]] _last_event
 """,
 }
 
+csr_summation_operation = {
+    'sum' : """
+%(pre_copy)s
+
+for(int i = 0; i < row_ptr_.size()-1; i++) {
+    sum = 0.0;
+    for(int j = row_ptr_[i]; j < row_ptr_[i+1]; j++) {
+        sum += %(psp)s ;
+    }
+    %(post_prefix)s_sum_%(target)s%(post_index)s += sum;
+}
+"""
+}
+
+update_variables = {
+    'local': """
+if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L) ){
+    %(global)s
+
+    int nb_post = static_cast<int>(post_ranks_.size());
+    for (int i = 0; i < nb_post; i++) {
+        rk_post = post_ranks_[i];
+
+        // semiglobal variables
+    %(semiglobal)s
+
+        // local variables
+        for (int j = col_ptr_[rk_post]; j < col_ptr_[rk_post+1]; j++) {
+            rk_pre = row_idx_[j];
+    %(local)s
+        }
+    }
+}
+""",
+    'global': """
+if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L)){
+    %(global)s
+
+    // semiglobal variables
+    for(int i = 0; i < post_ranks.size(); i++){
+        rk_post = post_ranks[i];
+    %(semiglobal)s
+    }
+}
+"""
+}
+
 spiking_summation_fixed_delay = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
-    auto row_ptr_ = sub_matrices_[tid]->row_ptr();
-    auto col_idx_ = sub_matrices_[tid]->col_idx();
 
     // Iterate over all spiking neurons
     for( int _idx = 0; _idx < %(pre_array)s.size(); _idx++) {
         // Rank of the presynaptic neuron
         int _pre = %(pre_array)s[_idx];
 
+        // slice in CSRC
+        int beg = row_ptr_[_pre];
+        int end = row_ptr_[_pre+1];
+
         // Iterate over connected post neurons
-        for(int syn = row_ptr_[_pre]; syn < row_ptr_[_pre + 1]; syn++) {
+        for (int syn = beg; syn < end; syn++) {
 
             // Event-driven integration
             %(event_driven)s
             // Update conductance
             %(g_target)s
             // Synaptic plasticity: pre-events
             %(pre_event)s
         }
     }
 } // active
 """
 
+spiking_post_event =  """
+if(_transmission && %(post_prefix)s_active){
+    int rk_post, beg, end;
+
+    for (int _idx_i = 0; _idx_i < %(post_prefix)sspiked.size(); _idx_i++) {
+        // Rank of the postsynaptic neuron which fired
+        rk_post = post_ranks_[%(post_prefix)sspiked[_idx_i]];
+
+        // slice in CSRC
+        beg = col_ptr_[rk_post];
+        end = col_ptr_[rk_post+1];
+
+        // Iterate over all synapse to this neuron
+        for (int j = beg; j < end; j++) {
+%(event_driven)s
+%(post_event)s
+        }
+    }
+}
+"""
+
 conn_templates = {
     # accessors
     'delay': delay,
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'event_driven': event_driven,
 
     #operations
-    'spiking_sum_fixed_delay': {
-        'outer_loop': spiking_summation_fixed_delay,
-    }
+    'update_variables': update_variables,
+    'rate_coded_sum': csr_summation_operation,
+    'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
+    'spiking_sum_variable_delay': None,
+    'post_event': spiking_post_event
 }
 
 conn_ids = {
-    'local_index': '[j]',
+    'local_index': '[inv_idx_[j]]',
     'semiglobal_index': '[i]',
     'global_index': '',
-    'post_index': '[i]',
     'pre_index': '[row_idx_[j]]',
-}
+    'post_index': '[i]',
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/Dense.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/Dense.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -520,16 +502,17 @@
 # as it would lead to 100% cache misses and an enormously high number of memory stalls.
 spiking_summation_fixed_delay_outer_loop = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
 
     // Iterate over all spiking neurons
     #pragma omp for
     for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
+        %(idx_type)s rk_pre = *it;
         for (%(idx_type)s rk_post = 0; rk_post < num_rows(); rk_post++) {
-            %(size_type)s j = rk_post*this->num_columns_ + *it;
+            %(size_type)s j = rk_post*this->num_columns_ + rk_pre;
 
             if (mask_[j]) {
                 // post-synaptic popential
                 #pragma omp atomic%(g_target)s
 
                 // 'on-pre' events
                 #pragma omp critical
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/Dense_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/Dense_T.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -126,16 +108,17 @@
     {
         std::cout << "thread " << tid << ": " << mat_slice_beg_ << " - " << mat_slice_end_ << std::endl;
     }
 #endif
 
     // Iterate over all spiking neurons
     for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
-        %(size_type)s beg = (*it) * this->num_rows_;
-        %(size_type)s end = (*it+1) * this->num_rows_;
+        %(idx_type)s rk_pre = (*it);
+        %(size_type)s beg = rk_pre * this->num_rows_;
+        %(size_type)s end = (rk_pre+1) * this->num_rows_;
 
         // Iterate over columns
         for (%(idx_type)s rk_post = mat_slice_beg_; rk_post < mat_slice_end_; rk_post++) {
             %(size_type)s j = beg + rk_post;
             
             %(g_target)s
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/ELL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/ELL.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     ELL.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/ELLR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/ELLR.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     ELLR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/LIL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/LIL.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     LIL.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< std::vector< %(type)s > > %(name)s;
 """,
     'semiglobal':
@@ -1060,15 +1042,17 @@
         }
     }
 } // active
 """
 
 spiking_summation_fixed_delay_inner_loop = """
 // Event-based summation
-if (_transmission && %(post_prefix)s_active){
+if (_transmission && %(post_prefix)s_active) {
+
+    %(spiked_array_fusion)s
 
     // Iterate over all incoming spikes (possibly delayed constantly)
     for (int _idx_j = 0; _idx_j < %(pre_array)s.size(); _idx_j++ ) {
         // Rank of the presynaptic neuron
         int rk_j = %(pre_array)s[_idx_j];
 
         // Find the presynaptic neuron in the inverse connectivity matrix
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/LIL_P.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/LIL_P.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     LIL_P.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< std::vector< std::vector<%(type)s > > > %(name)s;
 """,
     'semiglobal':
@@ -141,42 +123,58 @@
     def get_dendrite_delay(self, idx):
         return proj%(id_proj)s.delay
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """},
     'nonuniform_rate_coded': {
         'declare': """
-    std::vector<std::vector<int>> delay;
+    std::vector<std::vector<std::vector<int>>> delay;
     int max_delay;
+
+    std::vector<int> get_dendrite_delay(int row) {
+        return get_matrix_variable_row<int, std::vector<std::vector<int>>>(delay, row);
+    }
+    std::vector<std::vector<int>> get_delay() {
+        return get_matrix_variable_all<int, std::vector<std::vector<int>>>(delay);
+    }
+    void set_dendrite_delay(int row, std::vector<int> value) {
+        update_matrix_variable_row<int, std::vector<std::vector<int>>>(delay, row, value);
+    }
+    void set_delay(std::vector<std::vector<int>> value) {
+        update_matrix_variable_all<int, std::vector<std::vector<int>>>(delay, value);
+    }
 """,
         'init': """
-    delay = init_matrix_variable<int>(1);
+    delay = init_matrix_variable<int, std::vector<std::vector<int>>>(1);
     update_matrix_variable_all<int>(delay, delays);
 
     max_delay = %(pre_prefix)smax_delay;
 """,
         'reset': "",
         'pyx_struct':
 """
         # Non-uniform delay
-        vector[vector[int]] delay
+        vector[vector[int]] get_delay()
+        vector[int] get_dendrite_delay(int)
+        void set_delay(vector[vector[int]])
+        void set_dendrite_delay(int, vector[int])
         int max_delay
         void update_max_delay(int)
         void reset_ring_buffer()
 """,
         'pyx_wrapper_init': "",
         'pyx_wrapper_accessor':
 """
     # Access to non-uniform delay
     def get_delay(self):
-        return proj%(id_proj)s.delay
+        return proj%(id_proj)s.get_delay()
     def get_dendrite_delay(self, idx):
-        return proj%(id_proj)s.delay[idx]
+        return proj%(id_proj)s.get_dendrite_delay(idx)
     def set_delay(self, value):
-        proj%(id_proj)s.delay = value
+        proj%(id_proj)s.set_delay(value)
     def get_max_delay(self):
         return proj%(id_proj)s.max_delay
     def set_max_delay(self, value):
         proj%(id_proj)s.max_delay = value
     def update_max_delay(self, value):
         proj%(id_proj)s.update_max_delay(value)
     def reset_ring_buffer(self):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/SELL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/SELL.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     SELLR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#                         Qi Tang <kevin2014tq@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -84,21 +66,56 @@
         // %(name)s
         %(name)s.clear();
         %(name)s.shrink_to_fit();
 """,
     'global': ""
 }
 
+#############################################
+##  Synaptic delay
+#############################################
+delay = {
+    'uniform': {
+        'declare': """
+    // Uniform delay
+    int delay ;""",
+
+        'pyx_struct':
+"""
+        # Uniform delay
+        int delay""",
+        'init': """
+    delay = delays[0][0];
+""",
+        'pyx_wrapper_init':
+"""
+        proj%(id_proj)s.delay = syn.uniform_delay""",
+        'pyx_wrapper_accessor':
+"""
+    # Access to non-uniform delay
+    def get_delay(self):
+        return proj%(id_proj)s.delay
+    def get_dendrite_delay(self, idx):
+        return proj%(id_proj)s.delay
+    def set_delay(self, value):
+        proj%(id_proj)s.delay = value
+"""
+    },
+    'nonuniform_rate_coded': None,
+    'nonuniform_spiking': None
+}
+
 ###############################################################
 # Rate-coded continuous transmission
 ###############################################################
 continuous_transmission = {
     'sum' : """
+%(pre_copy)s
+
 // iterate across all blocks
-#pragma omp for
 for (%(idx_type)s i = 0; i < num_blocks_; i++) {
     
     //compute maxlength (maxnzr) in each block
     %(size_type)s maxlength = (row_ptr_[i + 1] - row_ptr_[i]) / block_size_;
 
     // iterate over all values within the block
     for (%(idx_type)s j = 0; j < block_size_; j++) {
@@ -126,15 +143,15 @@
 
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
-    'delay': None,
+    'delay': delay,
     
     # operations
     'rate_coded_sum': continuous_transmission,
     'vectorized_default_psp': {},
     'update_variables': None
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMP/__init__.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/OpenMPGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMPGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,22 @@
-#===============================================================================
-#
-#     OpenMPGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 import ANNarchy
 
 # ANNarchy objects
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.models.Synapses import DefaultRateCodedSynapse
 
 # Code templates
 from ANNarchy.generator.Projection.ProjectionGenerator import ProjectionGenerator, get_bounds
 from ANNarchy.generator.Projection.OpenMP import *
-from ANNarchy.generator.Projection.SingleThread import LIL_SingleThread
 
 # Useful functions
 from ANNarchy.generator.Utils import generate_equation_code, tabify, remove_trailing_spaces, check_avx_instructions, determine_idx_type_for_projection
 
 import re
 from copy import deepcopy
 
@@ -147,25 +127,17 @@
             connector_call = ""
             declare_connectivity_matrix = proj._specific_template['declare_connectivity_matrix']
             access_connectivity_matrix = proj._specific_template['access_connectivity_matrix']
 
         # local functions
         decl['parameters_variables'] += self._local_functions(proj)
 
-        # Size of a projection object
-        if 'determine_size_in_bytes' in proj._specific_template.keys():
-            determine_size_in_bytes = proj._specific_template['determine_size_in_bytes']
-        else:
-            determine_size_in_bytes = self._determine_size_in_bytes(proj)
-
-        # Clear variables
-        if 'clear_container' in proj._specific_template.keys():
-            clear_container = proj._specific_template['clear_container']
-        else:
-            clear_container = self._clear_container(proj)
+        # Memory management
+        size_in_bytes = self._size_in_bytes(proj)
+        clear_container = self._clear_container(proj)
 
         # Structural plasiticity
         creating = self.creating(proj)
         pruning = self.pruning(proj)
 
         # Profiling
         if self._prof_gen:
@@ -239,15 +211,15 @@
             'update_variables': update_variables,
             'update_max_delay': update_max_delay,
             'reset_ring_buffer': reset_ring_buffer,
             'post_event_prefix': post_event_prefix,
             'post_event': post_event,
             'access_parameters_variables': accessor,
             'access_additional': access_additional,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container,
             'sparse_format': sparse_matrix_format,
             'sparse_format_args': sparse_matrix_args,
             'float_prec': Global.config['precision'],
             'creating': creating,
             'pruning': pruning
         }
@@ -585,14 +557,62 @@
 
                 except KeyError:
                     # No fitting code found, so we fall back to normal code generation
                     # TODO: add internal error log, which key was missing?
                     Global._debug("No SIMD implementation found, fallback to non-SIMD code")
                     template = ""
 
+            else:
+                # Other optimizations like loop unroll etc?
+                if proj._storage_format == "bsr":
+                    try:
+                        # not yet implemented
+                        if proj._has_single_weight():
+                            raise KeyError
+
+                        from ANNarchy.generator.Projection.ProjectionGenerator import determine_bsr_blocksize
+                        if hasattr(proj, "_bsr_size"):
+                            blockDim = proj._bsr_size
+                        else:
+                            blockDim = determine_bsr_blocksize(proj.pre.population.size if isinstance(proj.pre, PopulationView) else proj.pre.size, proj.post.population.size if isinstance(proj.post, PopulationView) else proj.post.size)
+
+                        # Loop unroll depends on the block-size
+                        unrolled_template = template = self._templates["unrolled_default_psp"][blockDim]
+
+                        # Check if we implemented a SIMD version
+                        if simd_type in unrolled_template.keys():
+                            template = unrolled_template[simd_type]['multi_w']['sum'][Global.config["precision"]]
+                        else:
+                            template = unrolled_template['none']['multi_w']["sum"]
+
+                        # the access to pre-synaptic firing depends on the delay
+                        if proj.max_delay <= 1:
+                            # no synaptic delay
+                            ids.update({
+                                'get_r': ids['pre_prefix']+"r.data()",
+                            })
+
+                            psp_code = template % ids
+
+                            if self._prof_gen:
+                                psp_code = self._prof_gen.annotate_computesum_rate(proj, psp_code)
+
+                            return "", psp_code
+                        else:
+                            # HD (23th Nov 2021): the unrolled code templates for specific kernels is a highly
+                            #                     experimental feature. I will implement the delay case if we
+                            #                     are sure that we really use this.
+                            pass
+
+                    except KeyError:
+                        # No fitting code found, so we fall back to normal code generation
+                        # TODO: add internal error log, which key was missing?
+                        Global._debug("No SIMD implementation found, fallback to non-SIMD code")
+                        template = ""
+
         # Choose the relevant summation template
         try:
             template = self._templates['rate_coded_sum']
         except:
             Global._error("OpenMPGenerator: no template for storage_format = "+proj._storage_format+" configuration available")
 
         # Dictionary of keywords to transform the parsed equations
@@ -723,14 +743,18 @@
         Specific templates:
 
             * psp_prefix and psp_code
         """
         if 'psp_prefix' in proj._specific_template.keys() and 'psp_code' in proj._specific_template.keys():
             psp_prefix = proj._specific_template['psp_prefix']
             psp_code = proj._specific_template['psp_code']
+
+            if len(psp_code) > 0 and self._prof_gen:
+                psp_code = self._prof_gen.annotate_computesum_spiking(proj, psp_code)
+
             return psp_prefix, psp_code
 
         # If the connectivity is stored as post_to_pre, we need to use the
         # inversed matrix view to acces the psp/weight vectors. As we
         # parallelize over pre-neurons, there is a chance of concurrent accesses
         # towards psp.
         #
@@ -1003,23 +1027,26 @@
             else: # Uniform delays
                 template = self._templates['spiking_sum_fixed_delay'][proj._parallel_pattern]
                 pre_array = "%(pre_prefix)s_delayed_spike[delay-1]" % ids
         else:
             pre_array = "%(pre_prefix)sspiked" % ids
             template = self._templates['spiking_sum_fixed_delay'][proj._parallel_pattern]
 
+        # sanity check
         if template == None:
-            Global._error("Code generation error: no template available")
+            Global._error("Code generation error for proj%(id)s: no template available " % {'id': proj.id})
 
         # Axonal spike events
         spiked_array_fusion_code = ""
         if proj.synapse_type.pre_axon_spike:
             spiked_array_fusion_code = """
     std::vector<int> tmp_spiked = %(pre_array)s;
-    tmp_spiked.insert( tmp_spiked.end(), %(pre_prefix)saxonal.begin(), %(pre_prefix)saxonal.end() );
+    if (_axon_transmission) {
+        tmp_spiked.insert( tmp_spiked.end(), %(pre_prefix)saxonal.begin(), %(pre_prefix)saxonal.end() );
+    }
 """ % {'pre_prefix': ids['pre_prefix'], 'pre_array': pre_array}
 
             pre_array = "tmp_spiked"
 
         # Generate the whole code block
         code = ""
         if g_target_code != "" or pre_code != "":
@@ -1170,14 +1197,15 @@
 
         # Get basic template ids and update if necessary.
         ids = deepcopy(self._template_ids)
         if proj._storage_format == "lil":
             ids.update({
                 'post_index': '[rk_post]',
             })
+
         elif proj._storage_format == "csr":
             if proj._storage_order == "post_to_pre":
                 if single_matrix:
                     ids.update({
                         'semiglobal_index': '[*it]',
                         'pre_index': '[_col_idx[j]]',
                         'post_index': '[rk_post]',
@@ -1196,20 +1224,26 @@
                         'local_index': "[inv_idx_[j]]",
                         'semiglobal_index': '[*it]',
                         'global_index': '',
                         'pre_index': '[row_idx_[j]]',
                         'post_index': '[]',
                     })
                 else:
-                    raise NotImplementedError
+                    ids.update({
+                        'local_index': "[tid][inv_idx_[j]]",
+                        'semiglobal_index': "[tid][*it]",
+                        'global_index': "",
+                        'pre_index': "[row_idx_[j]]",
+                        'post_index': "",
+                    })
 
         else:
             raise NotImplementedError
 
-        # TODO: purpose?
+        # Definition of format-specific local variables.
         if proj._storage_format == "lil":
             post_event_prefix = ""
         elif proj._storage_format == "csr":
             post_event_prefix = """
         int rk_post;
         std::vector<int>::iterator it;
         """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/ProjectionGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/ProjectionGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     ProjectionGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2018  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.core import Random as ANNRandom
 from ANNarchy.extensions.convolution import Transpose
 
 # Useful functions
 from ANNarchy.generator.Utils import tabify, determine_idx_type_for_projection, cpp_connector_available
@@ -307,14 +289,27 @@
                             single_matrix = False
 
                     else:
                         sparse_matrix_format = "CSRCMatrixCUDAT<"+idx_type+", "+size_type+">"
                         sparse_matrix_include = "#include \"CSRCMatrixCUDAT.hpp\"\n"
                         single_matrix = True
 
+            elif proj._storage_format == "bsr":
+                if proj._storage_order == "post_to_pre":
+                    if Global._check_paradigm("openmp"):
+                        sparse_matrix_format = "BSRInvMatrix<"+idx_type+", "+size_type+", false>"
+                        sparse_matrix_include = "#include \"BSRInvMatrix.hpp\"\n"
+                        single_matrix = True
+
+                    else:
+                        raise NotImplementedError
+
+                else:
+                    raise NotImplementedError
+
             elif proj._storage_format == "dense":
                 if proj._storage_order == "post_to_pre":
                     if Global._check_paradigm("openmp"):
                         if proj._has_pop_view and Global.config["num_threads"] == 1:
                             sparse_matrix_format = "DenseMatrixOffsets<"+idx_type+", "+size_type+", char, false>"
                             sparse_matrix_include = "#include \"DenseMatrixOffsets.hpp\"\n"
                             single_matrix = True
@@ -404,15 +399,27 @@
         Each of the pre-defined pattern requires probably different initialization values.
         If no C++ implementation for a pattern is available a default construction from
         LIL is set.
         """
         #
         # Define the correct projection init code. Not all patterns have specialized
         # implementations.
-        if proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
+        if proj.connector_name == "All-to-All" and cpp_connector_available("All-to-All", proj._storage_format, proj._storage_order):
+            connector_call = """
+    bool all_to_all_pattern(std::vector<%(idx_type)s> post_ranks, std::vector<%(idx_type)s> pre_ranks, %(float_prec)s w_dist_arg1, %(float_prec)s w_dist_arg2, %(float_prec)s d_dist_arg1, %(float_prec)s d_dist_arg2, bool allow_self_connections) {
+        static_cast<%(sparse_format)s*>(this)->all_to_all_pattern(post_ranks, pre_ranks, allow_self_connections);
+
+%(init_weights)s
+%(init_delays)s
+
+        return true;
+    }
+"""
+
+        elif proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
             connector_call = """
     bool fixed_probability_pattern(std::vector<%(idx_type)s> post_ranks, std::vector<%(idx_type)s> pre_ranks, %(float_prec)s p, %(float_prec)s w_dist_arg1, %(float_prec)s w_dist_arg2, %(float_prec)s d_dist_arg1, %(float_prec)s d_dist_arg2, bool allow_self_connections) {
         static_cast<%(sparse_format)s*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng%(rng_idx)s%(num_threads)s);
 
 %(init_weights)s
 %(init_delays)s
 
@@ -481,16 +488,22 @@
                     Global.CodeGeneratorException("Non-uniform delays on rate-coded or spiking synapses are not available for CUDA devices.")
 
                 if proj.synapse_type.type == "rate":
                     key_delay = "nonuniform_rate_coded"
                 else:
                     key_delay = "nonuniform_spiking"
 
-            declare_delay = self._templates['delay'][key_delay]['declare']
-            init_delay = self._templates['delay'][key_delay]['init']
+            try:
+                declare_delay = self._templates['delay'][key_delay]['declare']
+                init_delay = self._templates['delay'][key_delay]['init']
+            except:
+                if key_delay == "uniform":
+                    raise NotImplementedError("uniform delays are not support by the", proj._storage_format, "format.")
+                else:
+                    raise NotImplementedError("non-uniform delays are not support by the", proj._storage_format, "format.")
         else:
             declare_delay = ""
             init_delay = ""
 
         # Code for declarations and accessors
         declare_parameters_variables, accessor = self._generate_default_get_set(proj, single_matrix)
 
@@ -779,15 +792,20 @@
                                 'name': var['name']
                             }
 
                         elif isinstance(proj.connector_weight_dist, ANNRandom.Uniform):
                             if single_spmv_matrix:
                                 init_code = "w = init_matrix_variable_uniform<%(float_prec)s>(w_dist_arg1, w_dist_arg2, rng[0]);"
                             else:
-                                init_code = "w = init_matrix_variable_uniform<%(float_prec)s>(w_dist_arg1, w_dist_arg2, rng);"
+                                if proj._storage_format == "lil":
+                                    init_code = "w = init_matrix_variable_uniform<%(float_prec)s, std::vector< std::vector<%(float_prec)s> > >(w_dist_arg1, w_dist_arg2, rng);"
+                                elif proj._storage_format == "csr":
+                                    init_code = "w = init_matrix_variable_uniform<%(float_prec)s, std::vector<%(float_prec)s> >(w_dist_arg1, w_dist_arg2, rng);"
+                                else:
+                                    raise NotImplementedError
 
                         elif isinstance(proj.connector_weight_dist, ANNRandom.Normal):
                             if single_spmv_matrix:
                                 init_code = "w = init_matrix_variable_normal<%(float_prec)s>(w_dist_arg1, w_dist_arg2, rng[0]);"
                             else:
                                 init_code = "w = init_matrix_variable_normal<%(float_prec)s>(w_dist_arg1, w_dist_arg2, rng);"
 
@@ -939,27 +957,27 @@
         "Implemented by child class"
         raise NotImplementedError
 
     def _update_synapse(self, proj):
         "Implemented by child class"
         raise NotImplementedError
 
-    def _determine_size_in_bytes(self, proj):
+    def _size_in_bytes(self, proj):
         """
         Generate code template to determine size in bytes for the C++ object *proj*. Please note, that this contain only
         default elementes (parameters, variables). User defined elements, parallelization support data structures or similar
         are not considered.
 
         Consequently implementing generators should extent the resulting code template. This is done by the 'size_in_bytes'
         field in the _specific_template dictionary.
         """
         if 'size_in_bytes' in proj._specific_template.keys():
+            # Specific operations will not be part of throughput analysis (HD: 18th Nov. 2023)
             return proj._specific_template['size_in_bytes']
 
-        from ANNarchy.generator.Utils import tabify
         code = ""
 
         # Connectivity
         _, sparse_matrix_format, _, single_matrix = self._select_sparse_matrix_format(proj)
         code += """
         // connectivity
         size_in_bytes += static_cast<%(spm)s*>(this)->size_in_bytes();
@@ -984,21 +1002,20 @@
     def _clear_container(self, proj):
         """
         Generate code template to destroy allocated container of the C++ object *proj*.
 
         User defined elements, parallelization support data structures or similar are not considered.
         Consequently implementing generators should extent the resulting code template.
         """
-        _, spm_format, _, _ = self._select_sparse_matrix_format(proj)
-
-        # SpecificProjection should define this field
-        if 'clear' in proj._specific_template.keys():
-            return proj._specific_template["clear"]
+        # SpecificProjection: the complete code has been overwritten
+        if 'clear_container' in proj._specific_template.keys():
+            return proj._specific_template['clear_container']
 
-        # Connectivity
+        # Connectivity, either default format or overwritten by SpecificProjection
+        _, spm_format, _, _ = self._select_sparse_matrix_format(proj)
         if 'declare_connectivity_matrix' not in proj._specific_template.keys():
             code = """
         // Connectivity
         static_cast<%(spm)s*>(this)->clear();
 """  % {'spm': spm_format}
         else:
             code = ""
@@ -1008,14 +1025,18 @@
             ids = {'ctype': attr['ctype'], 'name': attr['name']}
 
             if attr['name'] == "w" and proj._has_single_weight():
                 code += self._templates['attribute_cpp_delete']['global'] % ids    
             else:
                 code += self._templates['attribute_cpp_delete'][attr['locality']] % ids
 
+        # SpecificProjection added some additional code
+        if 'clear_additional' in proj._specific_template.keys():
+            code += proj._specific_template["clear_additional"]
+
         return code
 
 
 ######################################
 ### Code generation
 ######################################
 def get_bounds(param):
@@ -1035,27 +1056,30 @@
         'index': "%(local_index)s",
         'var' : param['name'],
         'val' : val,
         'operator': '<' if bound == 'min' else '>'
       }
     return code
 
+#   TODO (HD): 
+#       we should think about to allow any block size, even though it would lead to padding zeros
 def determine_bsr_blocksize(pre_size, post_size):
     """
     The size of dense blocks within blocked sparse row (BSR) format should fit into
     the matrix dimensions.
 
     To ensure this, we determines the smallest common divisor for two population sizes.
     """
     def determine_scd(val1, val2):
         from numpy import amin
-        min_num = amin([pre_size, post_size])
+        min_num = amin([val1, val2])
 
         i = 2
         while i < min_num:
-            if (pre_size%i==0) and (post_size%i==0):
+            if (val1%i==0) and (val2%i==0):
                 return i
             i+= 1
         
         return 1
 
+    # determine smallest common divisor
     return determine_scd(pre_size, post_size)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/BaseTemplates.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     BaseTemplates.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 projection_header = """/*
  *  ANNarchy-version: %(annarchy_version)s
  */
 #pragma once
 
 #include "ANNarchy.h"
 %(sparse_matrix_include)s
@@ -47,15 +29,15 @@
 
 %(connector_call)s
 
 %(declare_connectivity_matrix)s
 %(access_connectivity_matrix)s
 
     // Transmission and plasticity flags
-    bool _transmission, _plasticity, _update;
+    bool _transmission, _axon_transmission, _plasticity, _update;
     int _update_period;
     long int _update_offset;
 
 %(declare_delays)s
 %(declare_event_driven)s
 %(declare_rng)s
 %(declare_parameters_variables)s
@@ -74,14 +56,15 @@
     // Method called to initialize the projection
     void init_projection() {
     #ifdef _DEBUG
         std::cout << "ProjStruct%(id_proj)s::init_projection() - this = " << this << std::endl;
     #endif
 
         _transmission = true;
+        _axon_transmission = true;
         _update = true;
         _plasticity = true;
         _update_period = 1;
         _update_offset = 0L;
 
         init_attributes();
 
@@ -132,15 +115,15 @@
 
     // Access additional
 %(access_additional)s
 
     // Memory management
     long int size_in_bytes() {
         long int size_in_bytes = 0;
-%(determine_size)s
+%(size_in_bytes)s
         return size_in_bytes;
     }
 
     // Structural plasticity
 %(creating)s
 %(pruning)s
 
@@ -175,32 +158,51 @@
         // should not happen
         std::cerr << "ProjStruct%(id_proj)s::get_local_attribute_row_%(ctype_name)s: " << name << " not found" << std::endl;
         return std::vector<%(ctype)s>();
     }
 
     %(ctype)s get_local_attribute_%(ctype_name)s(std::string name, int rk_post, int rk_pre) {
     #ifdef _DEBUG
-        std::cout << "ProjStruct%(id_proj)s::get_local_attribute_row_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<")" << std::endl;
+        std::cout << "ProjStruct%(id_proj)s::get_local_attribute_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<")" << std::endl;
     #endif
 %(local_get3)s
 
         // should not happen
         std::cerr << "ProjStruct%(id_proj)s::get_local_attribute: " << name << " not found" << std::endl;
         return 0.0;
     }
 
     void set_local_attribute_all_%(ctype_name)s(std::string name, std::vector<std::vector<%(ctype)s>> value) {
+    #ifdef _DEBUG
+        auto min_value = std::numeric_limits<%(ctype)s>::max();
+        auto max_value = std::numeric_limits<%(ctype)s>::min();
+        for (auto it = value.cbegin(); it != value.cend(); it++ ){
+            auto loc_min = *std::min_element(it->cbegin(), it->cend());
+            if (loc_min < min_value)
+                min_value = loc_min;
+            auto loc_max = *std::max_element(it->begin(), it->end());
+            if (loc_max > max_value)
+                max_value = loc_max;
+        }
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_all_%(ctype_name)s(name = " << name << ", min(" << name << ")=" <<std::to_string(min_value) << ", max("<<name<<")="<<std::to_string(max_value)<< ")" << std::endl;
+    #endif
 %(local_set1)s
     }
 
     void set_local_attribute_row_%(ctype_name)s(std::string name, int rk_post, std::vector<%(ctype)s> value) {
+    #ifdef _DEBUG
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_row_%(ctype_name)s(name = "<<name<<", rk_post = " << rk_post << ", min("<<name<<")="<<std::to_string(*std::min_element(value.begin(), value.end())) << ", max("<<name<<")="<<std::to_string(*std::max_element(value.begin(), value.end()))<< ")" << std::endl;
+    #endif
 %(local_set2)s
     }
 
     void set_local_attribute_%(ctype_name)s(std::string name, int rk_post, int rk_pre, %(ctype)s value) {
+    #ifdef _DEBUG
+        std::cout << "ProjStruct%(id_proj)s::set_local_attribute_%(ctype_name)s(name = "<<name<<", rk_post = "<<rk_post<<", rk_pre = "<<rk_pre<<", value = " << std::to_string(value) << ")" << std::endl;
+    #endif
 %(local_set3)s
     }
 """,
     "semiglobal": """
     std::vector<%(ctype)s> get_semiglobal_attribute_all_%(ctype_name)s(std::string name) {
 %(semiglobal_get1)s
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/CSR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/CSR.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-#===============================================================================
-#
-#     CSR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2018-2020  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
@@ -935,16 +916,19 @@
 
     %(semiglobal)s
     }
 }
 """
 }
 
+###############################################################
+# Event-driven updates
+###############################################################
 spiking_summation_fixed_delay_csr = """// Event-based summation
-if (_transmission && %(post_prefix)s_active){
+if (_transmission && %(post_prefix)s_active) {
     // w as CSR
     const int * __restrict__ col_ptr = _col_ptr.data();
 
     // Iterate over all spiking neurons
     for (int _idx = 0; _idx < %(pre_array)s.size(); _idx++) {
         int _pre = %(pre_array)s[_idx];
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/CSR_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/CSR_T_P.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,35 @@
-#===============================================================================
-#
-#     CSR_T.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
-    std::vector< %(type)s > %(name)s;
+    std::vector< std::vector<%(type)s> > %(name)s;
 """,
     'semiglobal':
 """
     // Semiglobal %(attr_type)s %(name)s
-    std::vector< %(type)s >  %(name)s ;
+    std::vector< %(type)s > %(name)s ;
 """,
     'global':
 """
     // Global %(attr_type)s %(name)s
     %(type)s  %(name)s ;
 """
 }
 
 attribute_cpp_init = {
     'local':
 """
         // Local %(attr_type)s %(name)s
-        %(name)s = init_matrix_variable< %(type)s >(%(init)s);
+        %(name)s = init_matrix_variable< %(type)s, std::vector<%(type)s> >(%(init)s);
 """,
     'semiglobal':
 """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable< %(type)s >(%(init)s);
 """,
     'global':
@@ -55,31 +38,37 @@
         %(name)s = %(init)s;
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
-        size_in_bytes += sizeof(std::vector<%(ctype)s>);
-        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();       
+        size_in_bytes += sizeof(std::vector<std::vector<%(ctype)s>>);
+        size_in_bytes += sizeof(std::vector<%(ctype)s>) * %(name)s.capacity();
+        for(auto it = %(name)s.cbegin(); it != %(name)s.cend(); it++)
+            size_in_bytes += (it->capacity()) * sizeof(%(ctype)s);
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
-        // Global
+        // Global %(attr_type)s %(name)s
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
         // %(name)s
+        for (auto it = %(name)s.begin(); it != %(name)s.end(); it++) {
+            it->clear();
+            it->shrink_to_fit();
+        };
         %(name)s.clear();
         %(name)s.shrink_to_fit();
 """,
     'semiglobal': """
         // %(name)s
         %(name)s.clear();
         %(name)s.shrink_to_fit();
@@ -92,16 +81,16 @@
         'declare': """
     std::vector<int> delay;
     int max_delay;
     int idx_delay;
     std::vector< std::vector< std::vector< int > > > _delayed_spikes;
 """,
         'init': """
-    delay = init_variable<int>(1);
-    update_variable_all<int>(delay, delays);
+    delay = init_matrix_variable<int>(1);
+    update_matrix_variable_all<int>(delay, delays);
 
     idx_delay = 0;
     max_delay = %(pre_prefix)smax_delay;
 """,
         'reset': """
         while(!_delayed_spikes.empty()) {
             auto elem = _delayed_spikes.back();
@@ -141,112 +130,70 @@
         proj%(id_proj)s.reset_ring_buffer()
 """
     }    
 }
 
 event_driven = {
     'declare': """
-    std::vector<long> _last_event;
+    std::vector<std::vector<long>> _last_event;
 """,
     'cpp_init': """
         // Event-driven
-        _last_event = init_matrix_variable<long>(-10000);
+        _last_event = init_matrix_variable<long, std::vector<long>>(-10000);
 """,
     'pyx_struct': """
         vector[vector[long]] _last_event
 """,
 }
 
-csr_summation_operation = {
-    'sum' : """
-%(pre_copy)s
-
-for(int i = 0; i < row_ptr_.size()-1; i++) {
-    sum = 0.0;
-    for(int j = row_ptr_[i]; j < row_ptr_[i+1]; j++) {
-        sum += %(psp)s ;
-    }
-    %(post_prefix)s_sum_%(target)s%(post_index)s += sum;
-}
-"""
-}
-
-update_variables = {
-    'local': """
-if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L) ){
-    %(global)s
-
-    int nb_post = static_cast<int>(post_ranks_.size());
-    for (int i = 0; i < nb_post; i++) {
-        rk_post = post_ranks_[i];
-
-        // semiglobal variables
-    %(semiglobal)s
-
-        // local variables
-        for (int j = col_ptr_[rk_post]; j < col_ptr_[rk_post+1]; j++) {
-            rk_pre = row_idx_[j];
-    %(local)s
-        }
-    }
-}
-""",
-    'global': """
-if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L)){
-    %(global)s
-
-    // semiglobal variables
-    for(int i = 0; i < post_ranks.size(); i++){
-        rk_post = post_ranks[i];
-    %(semiglobal)s
-    }
-}
-"""
-}
-
 spiking_summation_fixed_delay = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
+    auto row_ptr_ = sub_matrices_[tid]->row_ptr();
+    auto col_idx_ = sub_matrices_[tid]->col_idx();
 
     // Iterate over all spiking neurons
     for( int _idx = 0; _idx < %(pre_array)s.size(); _idx++) {
         // Rank of the presynaptic neuron
         int _pre = %(pre_array)s[_idx];
 
-        // slice in CSRC
-        int beg = row_ptr_[_pre];
-        int end = row_ptr_[_pre+1];
-
         // Iterate over connected post neurons
-        for (int syn = beg; syn < end; syn++) {
+        for(int syn = row_ptr_[_pre]; syn < row_ptr_[_pre + 1]; syn++) {
 
             // Event-driven integration
             %(event_driven)s
             // Update conductance
             %(g_target)s
             // Synaptic plasticity: pre-events
             %(pre_event)s
         }
     }
 } // active
 """
 
 spiking_post_event =  """
-if(_transmission && %(post_prefix)s_active){
-    int rk_post, beg, end;
+if (_transmission && %(post_prefix)s_active) {
+    auto col_ptr_ = sub_matrices_[tid]->col_ptr();
+    auto row_idx_ = sub_matrices_[tid]->row_idx();
+    auto inv_idx_ = sub_matrices_[tid]->inverse_indices();
+    int part_beg = tid *  chunk_size_;
+    int part_end = (tid+1) *  chunk_size_;
 
-    for (int _idx_i = 0; _idx_i < %(post_prefix)sspiked.size(); _idx_i++) {
+    #pragma omp for
+    for(int _idx_i = 0; _idx_i < %(post_prefix)sspiked.size(); _idx_i++) {
         // Rank of the postsynaptic neuron which fired
-        rk_post = post_ranks_[%(post_prefix)sspiked[_idx_i]];
+        rk_post = %(post_prefix)sspiked[_idx_i];
 
-        // slice in CSRC
-        beg = col_ptr_[rk_post];
-        end = col_ptr_[rk_post+1];
+        // not in the partition of the thread
+        if (rk_post < part_beg)
+            continue;
+        if (rk_post >= part_end)
+            continue;
 
         // Iterate over all synapse to this neuron
-        for (int j = beg; j < end; j++) {
+        for(int j = col_ptr_[rk_post]; j < col_ptr_[rk_post+1]; j++){
 %(event_driven)s
 %(post_event)s
         }
     }
 }
 """
 
@@ -256,21 +203,20 @@
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'event_driven': event_driven,
 
     #operations
-    'update_variables': update_variables,
-    'rate_coded_sum': csr_summation_operation,
-    'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
-    'spiking_sum_variable_delay': None,
+    'spiking_sum_fixed_delay': {
+        'outer_loop': spiking_summation_fixed_delay,
+    },
     'post_event': spiking_post_event
 }
 
 conn_ids = {
-    'local_index': '[inv_idx_[j]]',
+    'local_index': '[j]',
     'semiglobal_index': '[i]',
     'global_index': '',
-    'pre_index': '[row_idx_[j]]',
     'post_index': '[i]',
-}
+    'pre_index': '[row_idx_[j]]',
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -91,15 +73,14 @@
 }
 
 delay = {
     'uniform': {
         'declare': """
     // Uniform delay
     int delay ;""",
-        
         'pyx_struct':
 """
         # Uniform delay
         int delay""",
         'init': """
     delay = delays[0][0];
 """,
@@ -115,14 +96,26 @@
         return proj%(id_proj)s.delay
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
     }
 }
 
+event_driven = {
+    'declare': """
+    std::vector<long> _last_event;
+""",
+    'cpp_init': """
+    _last_event = init_matrix_variable<long>(-10000);
+""",
+    'pyx_struct': """
+        vector[vector[long]] _last_event
+"""
+}
+
 ######################################
 ### Dense Matrix templates
 ######################################
 dense_summation_operation = {
     'sum' : """
 %(pre_copy)s
 
@@ -472,20 +465,20 @@
 # as it would lead to 100% cache misses and an enormously high number of memory stalls.
 spiking_summation_fixed_delay = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
 
     for (%(idx_type)s rk_post = 0; rk_post < num_rows(); rk_post++) {
         // Iterate over all spiking neurons
         for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
-            %(size_type)s j = rk_post*this->num_columns_ + *it;
-
-            %(g_target)s
+            %(idx_type)s rk_pre = *it;
+            %(size_type)s j = rk_post*this->num_columns_ + rk_pre;
 
             if (mask_[j]) {
                 %(event_driven)s
+                %(g_target)s
                 %(pre_event)s
             }
         }
     }
 } // active
 """
 
@@ -499,15 +492,14 @@
     // Local variables
     for(%(idx_type)s i = 0; i < %(post_prefix)ssize; i++){
         rk_post = i; // dense: ranks are indices
 
         // Semi-global variables
     %(semiglobal)s
 
-       
         // Local variables are updated to boolean flag
         %(size_type)s j = i*%(pre_prefix)ssize;
         for(rk_pre = 0; rk_pre < %(pre_prefix)ssize; rk_pre++, j++) {
             if(mask_[j]) {
 %(local)s
             }
         }
@@ -525,14 +517,30 @@
         rk_post = i;
     %(semiglobal)s
     }
 }
 """
 }
 
+spiking_post_event = """
+if (_transmission && %(post_prefix)s_active) {
+
+    %(idx_type)s columns = pop%(id_pre)s.size;
+
+    for (%(idx_type)s _idx_i = 0; _idx_i < %(post_prefix)sspiked.size(); _idx_i++) {
+        %(idx_type)s post_rank = %(post_prefix)sspiked[_idx_i];
+
+        for (%(size_type)s j = post_rank * columns; j < (post_rank+1) * columns; j++) {
+%(event_driven)s
+%(post_event)s
+        }
+    }
+}
+"""
+
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'delay': delay,
@@ -548,17 +556,19 @@
         },
         'avx512': {
             'multi_w': continuous_transmission_avx512
         }
     },
     'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
     'update_variables': dense_update_variables,
+    'post_event': spiking_post_event,
+    'event_driven': event_driven
 }
 
 conn_ids = {
     'local_index': '[j]',
     'semiglobal_index': '[rk_post]',
     'global_index': '',
     'post_index': '[rk_post]',
     'pre_index': '[rk_pre]',
     'delay_u' : '[delay-1]' # uniform delay
-}
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_PV.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#     Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -118,25 +100,32 @@
 """
     }
 }
 
 spiking_summation_fixed_delay = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
 
-    for (%(idx_type)s rk_post = 0; rk_post < num_rows(); rk_post++) {
-        // Iterate over all spiking neurons
-        for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
-            %(idx_type)s rk_pre = (*it);
-            if ((rk_pre < this->low_column_rank_) || (rk_pre >= this->high_column_rank_))
-                continue;
-
-            %(size_type)s j = rk_post*this->num_columns_ + *it;
-
+    // Iterate over all spiking neurons
+    for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
+        %(idx_type)s rk_pre = (*it);
+        if ((rk_pre < this->low_column_rank_) || (rk_pre >= this->high_column_rank_))
+            continue;
+
+        %(size_type)s beg = (rk_pre - this->low_column_rank_) * this->num_rows_;
+        %(size_type)s end = ((rk_pre+1) - this->low_column_rank_) * this->num_rows_;
+
+        // Post-synaptic potential
+        %(idx_type)s rk_post = this->low_row_rank_;
+        for (%(size_type)s j = beg; j < end; j++, rk_post++) {
             %(g_target)s
+        }
 
+        // 'on-pre' events
+        rk_post = 0;
+        for (%(size_type)s j = beg; j < end; j++, rk_post++) {
             if (mask_[j]) {
                 %(event_driven)s
                 %(pre_event)s
             }
         }
     }
 } // active
@@ -147,18 +136,18 @@
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'delay': delay,
 
     #operations
-    'rate_coded_sum': None,
-    'vectorized_default_psp': None,
+    'rate_coded_sum': "",
+    'vectorized_default_psp': {},
     'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
-    'update_variables': None,
+    'update_variables': "",
 }
 
 conn_ids = {
     'local_index': '[j]',
     'semiglobal_index': '[rk_post]',
     'global_index': '',
     'post_index': '[rk_post]',
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_PV_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/Dense_T.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021-22  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#                            Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -91,15 +73,14 @@
 }
 
 delay = {
     'uniform': {
         'declare': """
     // Uniform delay
     int delay ;""",
-        
         'pyx_struct':
 """
         # Uniform delay
         int delay""",
         'init': """
     delay = delays[0][0];
 """,
@@ -115,60 +96,122 @@
         return proj%(id_proj)s.delay
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
     }
 }
 
+event_driven = {
+    'declare': """
+    std::vector<long> _last_event;
+""",
+    'cpp_init': """
+    _last_event = init_matrix_variable<long>(-10000);
+""",
+    'pyx_struct': """
+        vector[vector[long]] _last_event
+"""
+}
+
 spiking_summation_fixed_delay = """// Event-based summation
 if (_transmission && %(post_prefix)s_active){
 
     // Iterate over all spiking neurons
     for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
-        %(idx_type)s rk_pre = (*it);
-        if ((rk_pre < this->low_column_rank_) || (rk_pre >= this->high_column_rank_))
-            continue;
-
-        %(size_type)s beg = (rk_pre - this->low_column_rank_) * this->num_rows_;
-        %(size_type)s end = ((rk_pre+1) - this->low_column_rank_) * this->num_rows_;
-
-        // Post-synaptic potential
-        %(idx_type)s rk_post = this->low_row_rank_;
-        for (%(size_type)s j = beg; j < end; j++, rk_post++) {
-            %(g_target)s
-        }
+        %(idx_type)s rk_pre = *it;
+        %(size_type)s beg = rk_pre * this->num_rows_;
+        %(size_type)s end = (rk_pre+1) * this->num_rows_;
 
         // 'on-pre' events
-        rk_post = 0;
+        %(idx_type)s rk_post = 0;
         for (%(size_type)s j = beg; j < end; j++, rk_post++) {
             if (mask_[j]) {
                 %(event_driven)s
+                %(g_target)s
                 %(pre_event)s
             }
         }
     }
 } // active
 """
 
+dense_update_variables = {
+    'local': """
+// Check periodicity
+if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L)){
+    // Global variables
+    %(global)s
+
+    // Local variables
+    for(%(idx_type)s i = 0; i < %(post_prefix)ssize; i++){
+        rk_post = i; // dense: ranks are indices
+
+        // Semi-global variables
+    %(semiglobal)s
+
+        // Local variables are updated to boolean flag
+        %(size_type)s j = i*%(pre_prefix)ssize;
+        for(rk_pre = 0; rk_pre < %(pre_prefix)ssize; rk_pre++, j++) {
+            if(mask_[j]) {
+%(local)s
+            }
+        }
+    }
+}
+""",
+    'global': """
+// Check periodicity
+if(_transmission && _update && %(post_prefix)s_active && ( (t - _update_offset)%%_update_period == 0L)){
+    // Global variables
+    %(global)s
+
+    // Semi-global variables
+    for(int i = 0; i < %(post_prefix)ssize; i++){
+        rk_post = i;
+    %(semiglobal)s
+    }
+}
+"""
+}
+
+spiking_post_event = """
+if (_transmission && %(post_prefix)s_active) {
+
+    %(idx_type)s rows = pop%(id_pre)s.size;
+    %(idx_type)s columns = pop%(id_post)s.size;
+
+    for (%(idx_type)s _idx_i = 0; _idx_i < %(post_prefix)sspiked.size(); _idx_i++) {
+        %(idx_type)s post_rank = %(post_prefix)sspiked[_idx_i];
+
+        for (%(size_type)s j = post_rank; j < this->num_rows_ * this->num_columns_; j += this->num_rows_) {
+%(event_driven)s
+%(post_event)s
+        }
+    }
+}
+"""
+
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'delay': delay,
 
     #operations
-    'rate_coded_sum': "",
+    'rate_coded_sum': None,
     'vectorized_default_psp': {},
     'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
-    'update_variables': "",
+    'update_variables': dense_update_variables,
+    'post_event': spiking_post_event,
+    'event_driven': event_driven
 }
 
 conn_ids = {
     'local_index': '[j]',
     'semiglobal_index': '[rk_post]',
     'global_index': '',
     'post_index': '[rk_post]',
     'pre_index': '[rk_pre]',
     'delay_u' : '[delay-1]' # uniform delay
-}
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/Dense_T.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/OpenMP/SELL.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Dense.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021-22  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#                            Julien Vitay <julien.vitay@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -40,16 +22,14 @@
 }
 
 attribute_cpp_init = {
     'local':
 """
         // Local %(attr_type)s %(name)s
         %(name)s = init_matrix_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
-        if(%(name)s.empty())
-            return false;
 """,
     'semiglobal':
 """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
 """,
     'global':
@@ -59,23 +39,23 @@
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
-        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
+        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();       
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         size_in_bytes += sizeof(std::vector<%(ctype)s>);
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
-        // Global %(attr_type)s %(name)s
+        // Global
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
     'local': """
         // %(name)s
@@ -86,20 +66,23 @@
         // %(name)s
         %(name)s.clear();
         %(name)s.shrink_to_fit();
 """,
     'global': ""
 }
 
+#############################################
+##  Synaptic delay
+#############################################
 delay = {
     'uniform': {
         'declare': """
     // Uniform delay
     int delay ;""",
-        
+
         'pyx_struct':
 """
         # Uniform delay
         int delay""",
         'init': """
     delay = delays[0][0];
 """,
@@ -112,59 +95,72 @@
     def get_delay(self):
         return proj%(id_proj)s.delay
     def get_dendrite_delay(self, idx):
         return proj%(id_proj)s.delay
     def set_delay(self, value):
         proj%(id_proj)s.delay = value
 """
-    }
-}
+    },
+    'nonuniform_rate_coded': None,
+    'nonuniform_spiking': None
+}
+
+###############################################################
+# Rate-coded continuous transmission
+###############################################################
+continuous_transmission = {
+    'sum' : """
+%(pre_copy)s
+
+// iterate across all blocks
+#pragma omp for
+for (%(idx_type)s i = 0; i < num_blocks_; i++) {
+    
+    //compute maxlength (maxnzr) in each block
+    %(size_type)s maxlength = (row_ptr_[i + 1] - row_ptr_[i]) / block_size_;
+
+    // iterate over all values within the block
+    for (%(idx_type)s j = 0; j < block_size_; j++) {
+        %(size_type)s pos = row_ptr_[i] + j * maxlength;
+        //row_now: compute global row idx
+        %(size_type)s row_now = i * block_size_ + j;
+
+        if (row_now < num_rows_) {
+            %(float_prec)s sum = 0.0;
+            for (int k = 0; k < maxlength; k++) {
+                %(idx_type)s rk_pre = col_idx_[pos+k];
 
-spiking_summation_fixed_delay = """// Event-based summation
-if (_transmission && %(post_prefix)s_active){
-
-    // Iterate over all spiking neurons
-    for (auto it = %(pre_prefix)sspiked.cbegin(); it != %(pre_prefix)sspiked.cend(); it++) {
-        %(size_type)s beg = (*it) * this->num_rows_;
-        %(size_type)s end = (*it+1) * this->num_rows_;
-
-        // Post-synaptic potential
-        %(idx_type)s rk_post = 0;
-        for (%(size_type)s j = beg; j < end; j++, rk_post++) {
-            %(g_target)s
-        }
-
-        // 'on-pre' events
-        rk_post = 0;
-        for (%(size_type)s j = beg; j < end; j++, rk_post++) {
-            if (mask_[j]) {
-                %(event_driven)s
-                %(pre_event)s
+                sum += %(psp)s;
             }
+            pop%(id_post)s._sum_%(target)s[row_now] += sum;
         }
+        
     }
-} // active
-"""
+}
+""",
+    'max': "",
+    'min': "",
+    'mean': "",
+}
 
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
     'delay': delay,
-
-    #operations
-    'rate_coded_sum': "",
+    
+    # operations
+    'rate_coded_sum': continuous_transmission,
     'vectorized_default_psp': {},
-    'spiking_sum_fixed_delay': spiking_summation_fixed_delay,
-    'update_variables': "",
+    'update_variables': None
 }
 
 conn_ids = {
-    'local_index': '[j]',
-    'semiglobal_index': '[rk_post]',
+    'local_index': '[pos+k]',
+    'semiglobal_index': '[i]',
     'global_index': '',
     'post_index': '[rk_post]',
     'pre_index': '[rk_pre]',
     'delay_u' : '[delay-1]' # uniform delay
 }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/ELL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/ELL.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     ELL.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/ELLR.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/ELLR.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,12 @@
-#===============================================================================
-#
-#     ELLR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2020  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< %(type)s > %(name)s;
 """,
     'semiglobal':
@@ -334,14 +317,65 @@
                     lsum += _tmp_sum[k];
 
                 // remainder loop
                 for (; _s < _stop; _s++)
                     lsum += _pre_r[_idx[_s]] * _w[_s];
 
                 %(post_prefix)s_sum_%(target)s%(post_index)s += lsum;
+            }
+        } // active
+    #else
+        std::cerr << "The code was not compiled with AVX support. Please check your compiler flags ..." << std::endl;
+    #endif
+""",
+        'float': """
+    #ifdef __AVX__
+        if (_transmission && %(post_prefix)s_active) {
+            %(size_type)s _s, _stop;
+            float _tmp_sum[8];
+            float* __restrict__ _pre_r = %(get_r)s;
+
+            %(idx_type)s nb_post = static_cast<%(idx_type)s>(post_ranks_.size());
+            for (%(idx_type)s i = 0; i < nb_post; i++) {
+                %(idx_type)s rk_post = post_ranks_[i];
+                %(idx_type)s* __restrict__ _idx = col_idx_.data();
+                float* __restrict__ _w = w.data();
+
+                _s = i*maxnzr_;
+                _stop = i*maxnzr_+rl_[i];
+                __m256 _tmp_reg_sum = _mm256_setzero_ps();
+
+                for (; _s+16 < _stop; _s+=16) {
+                    __m256 _tmp_r = _mm256_set_ps(
+                        _pre_r[_idx[_s+7]], _pre_r[_idx[_s+6]], _pre_r[_idx[_s+5]], _pre_r[_idx[_s+4]],
+                        _pre_r[_idx[_s+3]], _pre_r[_idx[_s+2]], _pre_r[_idx[_s+1]], _pre_r[_idx[_s]]
+                    );
+                    __m256 _tmp_r2 = _mm256_set_ps(
+                        _pre_r[_idx[_s+15]], _pre_r[_idx[_s+14]], _pre_r[_idx[_s+13]], _pre_r[_idx[_s+12]],
+                        _pre_r[_idx[_s+11]], _pre_r[_idx[_s+10]], _pre_r[_idx[_s+9]], _pre_r[_idx[_s+8]]
+                    );
+
+                    __m256 _tmp_w = _mm256_loadu_ps(&_w[_s]);
+                    __m256 _tmp_w2 = _mm256_loadu_ps(&_w[_s+8]);
+
+                    _tmp_reg_sum = _mm256_add_ps(_tmp_reg_sum, _mm256_mul_ps(_tmp_r, _tmp_w));
+                    _tmp_reg_sum = _mm256_add_ps(_tmp_reg_sum, _mm256_mul_ps(_tmp_r2, _tmp_w2));
+                }
+
+                _mm256_storeu_ps(_tmp_sum, _tmp_reg_sum);
+                float lsum = static_cast<double>(0.0);
+                // partial sums
+                for (int k = 0; k < 8; k++)
+                    lsum += _tmp_sum[k];
+
+                // remainder loop
+                for (; _s < _stop; _s++)
+                    lsum += _pre_r[_idx[_s]] * _w[_s];
+
+                %(post_prefix)s_sum_%(target)s%(post_index)s += lsum;
             }
         } // active
     #else
         std::cerr << "The code was not compiled with AVX support. Please check your compiler flags ..." << std::endl;
     #endif
 """
     }
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/LIL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/LIL.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     LIL.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2022  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 attribute_decl = {
     'local':
 """
     // Local %(attr_type)s %(name)s
     std::vector< std::vector<%(type)s > > %(name)s;
 """,
     'semiglobal':
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/SELL.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/HYB.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,146 @@
-#===============================================================================
-#
-#     SELLR.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2022  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
-#                         Qi Tang <kevin2014tq@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
-attribute_decl = {
-    'local':
 """
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
+attribute_decl = {
+    'local': """
     // Local %(attr_type)s %(name)s
-    std::vector< %(type)s > %(name)s;
+    hyb_local<%(type)s>* %(name)s;
 """,
-    'semiglobal':
-"""
+    'semiglobal': """
     // Semiglobal %(attr_type)s %(name)s
-    std::vector< %(type)s >  %(name)s ;
+    std::vector<%(type)s> %(name)s;
 """,
-    'global':
-"""
+    'global': """
     // Global %(attr_type)s %(name)s
-    %(type)s  %(name)s ;
+    %(type)s %(name)s;
 """
 }
 
 attribute_cpp_init = {
-    'local':
-"""
+    'local': """
         // Local %(attr_type)s %(name)s
         %(name)s = init_matrix_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
 """,
-    'semiglobal':
-"""
+    'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
         %(name)s = init_vector_variable<%(type)s>(static_cast<%(type)s>(%(init)s));
 """,
-    'global':
-"""
+    'global': """
         // Global %(attr_type)s %(name)s
         %(name)s = %(init)s;
 """
 }
 
 attribute_cpp_size = {
     'local': """
         // Local %(attr_type)s %(name)s
-        size_in_bytes += sizeof(std::vector<%(ctype)s>);
-        size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();       
+        size_in_bytes += sizeof(hyb_local<%(ctype)s>);
+        size_in_bytes += (%(name)s->ell.capacity()) * sizeof(%(ctype)s);
+        size_in_bytes += (%(name)s->coo.capacity()) * sizeof(%(ctype)s);
 """,
     'semiglobal': """
         // Semiglobal %(attr_type)s %(name)s
-        size_in_bytes += sizeof(std::vector<%(ctype)s>);
+        size_in_bytes += sizeof(std::vector<%(ctype)s>());
         size_in_bytes += sizeof(%(ctype)s) * %(name)s.capacity();
 """,
     'global': """
         // Global
         size_in_bytes += sizeof(%(ctype)s);
 """
 }
 
 attribute_cpp_delete = {
-    'local': """
+    'local':  """
         // %(name)s
-        %(name)s.clear();
-        %(name)s.shrink_to_fit();
+        %(name)s->clear();
 """,
-    'semiglobal': """
-        // %(name)s
-        %(name)s.clear();
-        %(name)s.shrink_to_fit();
+    'semiglobal': "",
+    'global': "",
+}
+
+delay = {
+    'uniform': {
+        'declare': """
+    // Uniform delay
+    int delay ;""",
+
+        'pyx_struct':
+"""
+        # Uniform delay
+        int delay""",
+        'init': """
+    delay = delays[0][0];
 """,
-    'global': ""
+        'pyx_wrapper_init':
+"""
+        proj%(id_proj)s.delay = syn.uniform_delay""",
+        'pyx_wrapper_accessor':
+"""
+    # Access to non-uniform delay
+    def get_delay(self):
+        return proj%(id_proj)s.delay
+    def get_dendrite_delay(self, idx):
+        return proj%(id_proj)s.delay
+    def set_delay(self, value):
+        proj%(id_proj)s.delay = value
+"""
+    }
 }
 
 ###############################################################
 # Rate-coded continuous transmission
 ###############################################################
-continuous_transmission = {
+hyb_summation_operation = {
     'sum' : """
-// iterate across all blocks
-for (%(idx_type)s i = 0; i < num_blocks_; i++) {
-    
-    //compute maxlength (maxnzr) in each block
-    %(size_type)s maxlength = (row_ptr_[i + 1] - row_ptr_[i]) / block_size_;
+%(pre_copy)s
+
+// ELLPACK partition
+auto post_ranks = get_post_rank();
+auto maxnzr_ = ell_matrix_->get_maxnzr();
+auto col_idx_ = ell_matrix_->get_column_indices();
+const %(idx_type)s nonvalue_idx = std::numeric_limits<%(idx_type)s>::max();
+
+%(idx_type)s nb_post = static_cast<%(idx_type)s>(post_ranks.size());
+for (%(idx_type)s i = 0; i < nb_post; i++) {
+    %(idx_type)s rk_post = post_ranks[i]; // Get postsynaptic rank
+
+    sum = 0.0;
+    %(size_type)s beg = i*maxnzr_;
+    %(size_type)s end = (i+1)*maxnzr_;
+    for (%(size_type)s j = beg; j < end; j++) {
+        %(idx_type)s rk_pre = col_idx_[j];
+        if (rk_pre == nonvalue_idx)
+            break;
 
-    // iterate over all values within the block
-    for (%(idx_type)s j = 0; j < block_size_; j++) {
-        %(size_type)s pos = row_ptr_[i] + j * maxlength;
-        //row_now: compute global row idx
-        %(size_type)s row_now = i * block_size_ + j;
-
-        if (row_now < num_rows_) {
-            %(float_prec)s sum = 0.0;
-            for (int k = 0; k < maxlength; k++) {
-                %(idx_type)s rk_pre = col_idx_[pos+k];
-
-                sum += %(psp)s;
-            }
-            pop%(id_post)s._sum_%(target)s[row_now] += sum;
-        }
-        
+        sum += %(ell_psp)s ;
     }
+    %(post_prefix)s_sum_%(target)s%(ell_post_index)s += sum;
+}
+
+// Coordinate partition
+auto nnz = coo_matrix_->nb_synapses();
+auto row_it = coo_matrix_->get_row_indices();
+auto col_it = coo_matrix_->get_column_indices();
+
+for(int j = 0; j < nnz; j++, row_it++, col_it++) {
+    %(post_prefix)s_sum_%(target)s%(coo_post_index)s += %(coo_psp)s;
 }
 """,
     'max': "",
     'min': "",
     'mean': "",
 }
 
 conn_templates = {
     # accessors
     'attribute_decl': attribute_decl,
     'attribute_cpp_init': attribute_cpp_init,
     'attribute_cpp_size': attribute_cpp_size,
     'attribute_cpp_delete': attribute_cpp_delete,
-    'delay': None,
+    'delay': delay,
     
-    # operations
-    'rate_coded_sum': continuous_transmission,
-    'vectorized_default_psp': {},
-    'update_variables': None
+    'rate_coded_sum': hyb_summation_operation,
+    'update_variables': ""
 }
-
-conn_ids = {
-    'local_index': '[pos+k]',
-    'semiglobal_index': '[i]',
-    'global_index': '',
-    'post_index': '[rk_post]',
-    'pre_index': '[rk_pre]',
-    'delay_u' : '[delay-1]' # uniform delay
-}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThread/__init__.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThread/__init__.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Projection/SingleThreadGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/Projection/SingleThreadGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,11 @@
-#===============================================================================
-#
-#     SingleThreadGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2016-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
 
 import ANNarchy
 
 # ANNarchy objects
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.models.Synapses import DefaultRateCodedSynapse
@@ -142,25 +123,17 @@
             connector_call = ""
             declare_connectivity_matrix = proj._specific_template['declare_connectivity_matrix']
             access_connectivity_matrix = proj._specific_template['access_connectivity_matrix']
 
         # Local functions
         decl['parameters_variables'] += self._local_functions(proj)
 
-        # Size of a projection object
-        if 'determine_size_in_bytes' in proj._specific_template.keys():
-            determine_size_in_bytes = proj._specific_template['determine_size_in_bytes']
-        else:
-            determine_size_in_bytes = self._determine_size_in_bytes(proj)
-
-        # Clear variables
-        if 'clear_container' in proj._specific_template.keys():
-            clear_container = proj._specific_template['clear_container']
-        else:
-            clear_container = self._clear_container(proj)
+        # Memory management
+        size_in_bytes = self._size_in_bytes(proj)
+        clear_container = self._clear_container(proj)
 
         # Structural plasiticity
         creating = self.creating(proj)
         pruning = self.pruning(proj)
 
         # Profiling
         if self._prof_gen:
@@ -222,15 +195,15 @@
             'update_prefix': update_prefix,
             'update_variables': update_variables,
             'update_max_delay': update_max_delay,
             'reset_ring_buffer': reset_ring_buffer,
             'post_event': post_event,
             'access_parameters_variables': accessor,
             'access_additional': access_additional,
-            'determine_size': determine_size_in_bytes,
+            'size_in_bytes': size_in_bytes,
             'clear_container': clear_container,
             'float_prec': Global.config['precision'],
             'creating': creating,
             'pruning': pruning
         }
 
         # Generate the final code
@@ -551,15 +524,15 @@
                         from ANNarchy.generator.Projection.ProjectionGenerator import determine_bsr_blocksize
                         if hasattr(proj, "_bsr_size"):
                             blockDim = proj._bsr_size
                         else:
                             blockDim = determine_bsr_blocksize(proj.pre.population.size if isinstance(proj.pre, PopulationView) else proj.pre.size, proj.post.population.size if isinstance(proj.post, PopulationView) else proj.post.size)
 
                         # Loop unroll depends on the block-size
-                        unrolled_template = template = self._templates["unrolled_default_psp"][blockDim]
+                        unrolled_template = self._templates["unrolled_default_psp"][blockDim]
 
                         # Check if we implemented a SIMD version
                         if simd_type in unrolled_template.keys():
                             template = unrolled_template[simd_type]['multi_w']['sum'][Global.config["precision"]]
                         else:
                             template = unrolled_template['none']['multi_w']["sum"]
 
@@ -576,15 +549,15 @@
                                 psp_code = self._prof_gen.annotate_computesum_rate(proj, psp_code)
 
                             return "", psp_code
                         else:
                             # HD (23th Nov 2021): the unrolled code templates for specific kernels is a highly
                             #                     experimental feature. I will implement the delay case if we
                             #                     are sure that we really use this.
-                            pass
+                            raise KeyError
 
                     except KeyError:
                         # No fitting code found, so we fall back to normal code generation
                         # TODO: add internal error log, which key was missing?
                         Global._debug("No SIMD implementation found, fallback to non-SIMD code")
                         template = ""
 
@@ -735,14 +708,67 @@
         """ % {'post_prefix': ids['post_prefix'], 'code': tabify(sum_code, 3)}
 
         if self._prof_gen:
             final_code = self._prof_gen.annotate_computesum_rate(proj, final_code)
 
         return psp_prefix, final_code
 
+    def _process_g_target_code(self, proj, eq, ids):
+        """
+        TODO: docs!
+        """
+        # PSP form
+        g_target = eq['cpp'].split('=')[1]
+        # Operation (g_target is replaced by sum in 'cpp')
+        operation = re.search(r'sum (.*?)=', eq['cpp']).group(1).strip() + "="
+        # Check targets
+        if isinstance(proj.target, str):
+            targets = [proj.target]
+        else:
+            targets = proj.target
+
+        g_target_code = ""
+        for target in targets:
+            # Special case where w is a single value
+            if proj._has_single_weight():
+                g_target = re.sub(
+                    r'([^\w]+)w%\(local_index\)s',
+                    r'\1w',
+                    g_target
+                )
+
+            # update post-synaptic potential code
+            target_dict = {
+                'post_prefix': ids['post_prefix'],
+                'target': target,
+                'g_target': g_target % ids,
+                'eq': eq['eq'],
+                'post_index': ids['post_index'],
+                'operation': operation
+            }
+            g_target_code += """
+    %(post_prefix)sg_%(target)s%(post_index)s %(operation)s %(g_target)s
+"""% target_dict
+
+            # Determine bounds
+            for key, val in eq['bounds'].items():
+                if not key in ['min', 'max']:
+                    continue
+                try:
+                    value = str(float(val))
+                except: # TODO: more complex operations
+                    value = val % ids
+
+                g_target_code += """
+    if (%(post_prefix)sg_%(target)s%(post_index)s %(op)s %(val)s)
+        %(post_prefix)sg_%(target)s%(post_index)s = %(val)s;
+""" % {'post_prefix': ids['post_prefix'], 'target': target, 'post_index': ids['post_index'], 'op': "<" if key == 'min' else '>', 'val': value}
+
+        return g_target_code
+
     def _computesum_spiking(self, proj):
         """
         Generate codes for spike propagation and pre-spike part of event-driven equations.
 
         Returns:
 
             * psp_prefix: set of variables needed in the kernel, positioned at the begin of
@@ -752,14 +778,18 @@
         Specific templates:
 
             * psp_prefix and psp_code
         """
         if 'psp_prefix' in proj._specific_template.keys() and 'psp_code' in proj._specific_template.keys():
             psp_prefix = proj._specific_template['psp_prefix']
             psp_code = proj._specific_template['psp_code']
+
+            if len(psp_code) > 0 and self._prof_gen:
+                psp_code = self._prof_gen.annotate_computesum_spiking(proj, psp_code)
+
             return psp_prefix, psp_code
 
         psp_prefix = """int nb_post; double sum;"""
 
         # Basic tags, dependent on storage format are assuming a feedforward
         # transmission.
         ids = deepcopy(self._template_ids)
@@ -784,15 +814,15 @@
                 ids.update({
                     'local_index': "[syn]",
                     'semiglobal_index': '[col_idx_[syn]]',
                     'pre_index': '[rk_j]',
                     'post_index': '[col_idx_[syn]]',
                 })
 
-        elif proj._storage_format == "dense":
+        elif proj._storage_format in ["bsr","dense"]:
             # nothing to do here, as the indices can simply switched
             pass
 
         else:
             # HD (19th May 2022):
             # many formats will need to adapt here. By raising this
             # error, I remember us that we need to check this carefully
@@ -804,68 +834,22 @@
             continous_transmission = True
 
         ####################################################
         # Event-driven summation of g_target
         ####################################################
         # Strings
         updated_variables_list = []
-        g_target = ""
         g_target_code = ""
 
         # Analyse all elements of pre_spike
         for eq in proj.synapse_type.description['pre_spike']:
             # g_target is treated differently
             # Must be at the end of the equations
             if eq['name'] == 'g_target':
-                # PSP form
-                g_target = eq['cpp'].split('=')[1]
-                # Operation (g_target is replaced by sum in 'cpp')
-                operation = re.search(r'sum (.*?)=', eq['cpp']).group(1).strip() + "="
-                # Check targets
-                if isinstance(proj.target, str):
-                    targets = [proj.target]
-                else:
-                    targets = proj.target
-
-                g_target_code = ""
-                for target in targets:
-                    # Special case where w is a single value
-                    if proj._has_single_weight():
-                        g_target = re.sub(
-                            r'([^\w]+)w%\(local_index\)s',
-                            r'\1w',
-                            g_target
-                        )
-
-                    # update post-synaptic potential code
-                    target_dict = {
-                        'post_prefix': ids['post_prefix'],
-                        'target': target,
-                        'g_target': g_target % ids,
-                        'eq': eq['eq'],
-                        'post_index': ids['post_index'],
-                        'operation': operation
-                    }
-                    g_target_code += """
-            %(post_prefix)sg_%(target)s%(post_index)s %(operation)s %(g_target)s
-"""% target_dict
-
-                    # Determine bounds
-                    for key, val in eq['bounds'].items():
-                        if not key in ['min', 'max']:
-                            continue
-                        try:
-                            value = str(float(val))
-                        except: # TODO: more complex operations
-                            value = val % ids
-
-                        g_target_code += """
-            if (%(post_prefix)sg_%(target)s%(post_index)s %(op)s %(val)s)
-                %(post_prefix)sg_%(target)s%(post_index)s = %(val)s;
-""" % {'post_prefix': ids['post_prefix'], 'target': target, 'post_index': ids['post_index'], 'op': "<" if key == 'min' else '>', 'val': value}
+                g_target_code += self._process_g_target_code(proj, eq, ids)
 
             else:
                 # process equations in pre_spike which
                 # are not 'g_target'
 
                 condition = ""
                 # Check conditions to update the variable
@@ -898,42 +882,57 @@
 """ % eq_dict
                 else: # Normal synaptic variable
                     updated_variables_list += """
 // %(eq)s
 %(cpp)s
 %(bounds)s""" % eq_dict
 
-
-        # Generate the default post-conductance increase
-        # default g_target += w
-        if not continous_transmission and g_target == "":
-            # Check targets
-            if isinstance(proj.target, str):
-                targets = [proj.target]
-            else:
-                targets = proj.target
-
-            g_target_code = ""
-            for target in targets:
-                g_target_code += """
-            // Increase the post-synaptic conductance g_target += w
-            %(post_prefix)sg_%(target)s%(post_index)s += w%(local_index)s;
-"""
-
         # Special case where w is a single value
         if proj._has_single_weight():
             g_target_code = re.sub(
                 r'([^\w]+)w%\(local_index\)s',
                 r'\1w',
                 g_target_code
             )
 
         # finalize g_target_code
         g_target_code = g_target_code % ids
 
+        # Generate the default post-conductance increase
+        # if no g_target statement is present and no continuous transmission (e.g. gap-junction)
+        if not continous_transmission and len(g_target_code) == 0:
+            # default g_target += w
+            default_code = """
+            // Increase the post-synaptic conductance g_target += w
+            %(post_prefix)sg_%(target)s%(post_index)s += w%(local_index)s;
+"""
+
+            # Special case where w is a single value
+            if proj._has_single_weight():
+                default_code = re.sub(
+                    r'([^\w]+)w%\(local_index\)s',
+                    r'\1w',
+                    default_code
+                )
+
+            # Check targets
+            if isinstance(proj.target, str):
+                targets = [proj.target]
+            else:
+                targets = proj.target
+
+            # Iterate over all targets
+            for target in targets:
+                g_target_code += default_code % {
+                    'post_prefix': ids['post_prefix'],
+                    'post_index': ids['post_index'],
+                    'local_index': ids['local_index'],
+                    'target': target
+                }
+
         # Event-driven integration of synaptic variables
         has_exact = False
         event_driven_code = ''
         for var in proj.synapse_type.description['variables']:
             if var['method'] == 'event-driven':
                 has_exact = True
                 event_driven_code += """
@@ -974,39 +973,63 @@
         else:
             pre_array = "%(pre_prefix)sspiked" % ids
             template = self._templates['spiking_sum_fixed_delay']
 
         if template == None:
             Global._error("Code generation error: no template available")
 
+        complete_code = ""
+
         # Axonal spike events
         spiked_array_fusion_code = ""
         if proj.synapse_type.pre_axon_spike:
-            spiked_array_fusion_code = """
-    std::vector<int> tmp_spiked = %(pre_array)s;
-    tmp_spiked.insert( tmp_spiked.end(), %(pre_prefix)saxonal.begin(), %(pre_prefix)saxonal.end() );
-""" % {'pre_prefix': ids['pre_prefix'], 'pre_array': pre_array}
+            if proj.synapse_type.description['raw_pre_spike'] == proj.synapse_type.description['raw_axon_spike']:
+                # default and axonal spike share the same mechanism,
+                # therefore we can join the two spike event list
+                spiked_array_fusion_code = """
+        std::vector<int> tmp_spiked = %(pre_array)s;
+        if (_axon_transmission) {
+            tmp_spiked.insert( tmp_spiked.end(), %(pre_prefix)saxonal.begin(), %(pre_prefix)saxonal.end() );
+        }
+    """ % {'pre_prefix': ids['pre_prefix'], 'pre_array': pre_array}
 
-            pre_array = "tmp_spiked"
+                pre_array = "tmp_spiked"
+
+            else:
+                # axon_spike uses a different equation
+                # HD (20. Oct. 2023): together with Oliver Maith we decided that the equations are limited
+                #                     to g_target += ...
+                ids.update({
+                    'pre_array': "pop%(id_pre)s.axonal" % {'id_pre': proj.pre.id},
+                    'pre_event': "",
+                    'g_target': self._process_g_target_code(proj, proj.synapse_type.description['pre_axon_spike'][0], ids),
+                    'target': proj.target, # for omp reduce
+                    'event_driven': "",
+                    'spiked_array_fusion': ""
+                })
+                complete_code += template % ids
+                complete_code = complete_code.replace("(_transmission", "(_axon_transmission")  # TODO: quite hacky ...
+
+                # for the default code generation path
+                pre_array = "pop%(id_pre)s.spiked" % {'id_pre': proj.pre.id}
 
         # Generate the whole code block
-        code = ""
         if g_target_code != "" or pre_code != "":
             ids.update({
                 'pre_array': pre_array,
                 'pre_event': pre_code,
                 'g_target': g_target_code,
                 'target': proj.target, # for omp reduce
                 'event_driven': event_driven_code,
                 'spiked_array_fusion': spiked_array_fusion_code
             })
-            code = template % ids
+            complete_code += template % ids
 
         # Add tabs
-        code = tabify(code, 2)
+        complete_code = tabify(complete_code, 2)
 
         ####################################################
         # Not even-driven summation of psp: like rate-coded
         ####################################################
         if 'psp' in  proj.synapse_type.description.keys(): # not event-based
             # Compute it as if it were rate-coded
             _, psp_code = self._computesum_rate(proj)
@@ -1016,23 +1039,23 @@
             # Change _sum_target into g_target (TODO: handling of PopulationViews???)
             psp_code = psp_code.replace(
                 '%(post_prefix)s_sum_%(target)s' % ids,
                 '%(post_prefix)sg_%(target)s' % ids
             )
 
             # Add it to the main code
-            code += """
+            complete_code += """
         // PSP-based summation"""
-            code += psp_code
+            complete_code += psp_code
 
         # Annotate code
         if self._prof_gen:
-            code = self._prof_gen.annotate_computesum_spiking(proj, code)
+            complete_code = self._prof_gen.annotate_computesum_spiking(proj, complete_code)
 
-        return psp_prefix, code
+        return psp_prefix, complete_code
 
     def _header_structural_plasticity(self, proj):
         """
         Generate extension code for C header_struct: variable declaration, add and remove synapses.
 
         Templates:
 
@@ -1154,14 +1177,15 @@
         # Generate event-driven code
         event_driven_code = ""
         if has_event_driven:
             for var in proj.synapse_type.description['variables']:
                 if var['method'] == 'event-driven':
                     event_driven_code += '// ' + var['eq'] + '\n'
                     event_driven_code += var['cpp'] % ids + '\n'
+
             event_driven_code += """
 // Update the last event for the synapse
 _last_event%(local_index)s = t;
 """ % ids
 
             event_driven_code = tabify(event_driven_code, 3)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/PyxGenerator.py` & `ANNarchy-4.7.3/ANNarchy/generator/PyxGenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,25 @@
-#===============================================================================
-#
-#     PyxGenerator.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
 from ANNarchy.core.Population import Population
 from ANNarchy.core.Projection import Projection
+from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.extensions.bold import BoldMonitor
 from ANNarchy.extensions.convolution import Transpose
 
 from ANNarchy.generator.Template import PyxTemplate
 
 from ANNarchy.generator.Population import OpenMPTemplates as omp_templates
 from ANNarchy.generator.Population import CUDATemplates as cuda_templates
 
-from ANNarchy.generator.Projection.OpenMP import BaseTemplates as proj_omp_templates
-
 from ANNarchy.generator.Projection.SingleThread import *
 from ANNarchy.generator.Projection.OpenMP import *
 from ANNarchy.generator.Projection.CUDA import *
 from ANNarchy.generator.Utils import tabify, determine_idx_type_for_projection, cpp_connector_available
 
 class PyxGenerator(object):
     """
@@ -688,18 +669,20 @@
                 if not var['name'] in ['w', 'delay'] and  var['name'] in proj.synapse_type.description['local']:
                     extra_args += ', ' + var['ctype'] + ' ' +  var['name']
             # Generate the code
             structural_plasticity += sp_tpl['func'] % {'extra_args': extra_args}
 
         # Check if either a custom definition or a CPP side init
         # is available otherwise fall back to init from LIL
-        if proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
-            export_connector = tabify("void fixed_probability_pattern(vector[%(idx_type)s], vector[%(idx_type)s], %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, bool)", 2)
+        if proj.connector_name == "All-to-All" and cpp_connector_available("All-to-All", proj._storage_format, proj._storage_order):
+            export_connector = tabify("bool all_to_all_pattern(vector[%(idx_type)s], vector[%(idx_type)s], %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, bool)", 2)
+        elif proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
+            export_connector = tabify("bool fixed_probability_pattern(vector[%(idx_type)s], vector[%(idx_type)s], %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, bool)", 2)
         elif proj.connector_name == "Random Convergent" and cpp_connector_available("Random Convergent", proj._storage_format, proj._storage_order):
-            export_connector = tabify("void fixed_number_pre_pattern(vector[%(idx_type)s], vector[%(idx_type)s], %(idx_type)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s)", 2)
+            export_connector = tabify("bool fixed_number_pre_pattern(vector[%(idx_type)s], vector[%(idx_type)s], %(idx_type)s, %(float_prec)s, %(float_prec)s, %(float_prec)s, %(float_prec)s)", 2)
         else:
             export_connector = tabify("bool init_from_lil(vector[%(idx_type)s], vector[vector[%(idx_type)s]], vector[vector[%(float_prec)s]], vector[vector[int]])", 2)
 
         # Data types, only of interest if Global.config["only_int_idx_type"] is false
         idx_types = determine_idx_type_for_projection(proj)
         idx_type_dict = {
             'float_prec': Global.config["precision"],
@@ -833,23 +816,28 @@
                     extra_values += ', ' +  var['name']
 
             # Generate the code
             structural_plasticity += sp_tpl['func'] % {'id' : proj.id, 'extra_args': extra_args, 'extra_values': extra_values}
 
         # Check if either a custom definition or a CPP side init
         # is available otherwise fall back to init from LIL
-        if proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
+        if proj.connector_name == "All-to-All" and cpp_connector_available("All-to-All", proj._storage_format, proj._storage_order):
+            wrapper_connector_call = """
+    def all_to_all(self, post_ranks, pre_ranks, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections):
+        return proj%(id_proj)s.all_to_all_pattern(post_ranks, pre_ranks, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections)
+""" % {'id_proj': proj.id}
+        elif proj.connector_name == "Random" and cpp_connector_available("Random", proj._storage_format, proj._storage_order):
             wrapper_connector_call = """
     def fixed_probability(self, post_ranks, pre_ranks, p, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections):
-        proj%(id_proj)s.fixed_probability_pattern(post_ranks, pre_ranks, p, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections)
+        return proj%(id_proj)s.fixed_probability_pattern(post_ranks, pre_ranks, p, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2, allow_self_connections)
 """ % {'id_proj': proj.id}
         elif proj.connector_name == "Random Convergent" and cpp_connector_available("Random Convergent", proj._storage_format, proj._storage_order):
             wrapper_connector_call = """
     def fixed_number_pre(self, post_ranks, pre_ranks, number_synapses_per_row, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2):
-        proj%(id_proj)s.fixed_number_pre_pattern(post_ranks, pre_ranks, number_synapses_per_row, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2)
+        return proj%(id_proj)s.fixed_number_pre_pattern(post_ranks, pre_ranks, number_synapses_per_row, w_dist_arg1, w_dist_arg2, d_dist_arg1, d_dist_arg2)
 """ % {'id_proj': proj.id}
         else:
             wrapper_connector_call = """
     def init_from_lil_connectivity(self, synapses):
         " synapses is an instance of LILConnectivity "
         return proj%(id_proj)s.init_from_lil(synapses.post_rank, synapses.pre_rank, synapses.w, synapses.delay)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Sanity.py` & `ANNarchy-4.7.3/ANNarchy/generator/Sanity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,17 @@
-#===============================================================================
-#
-#     Sanity.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import re
 
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
+from ANNarchy.core.SpecificProjection import SpecificProjection
 from ANNarchy.models.Synapses import DefaultSpikingSynapse, DefaultRateCodedSynapse
 
 # No variable can have these names
 reserved_variables = [
     't',
     'dt',
     't_pre',
@@ -184,22 +167,19 @@
     """
     ANNarchy 4.7 introduced a set of sparse matrix formats. Some of them are not implemented for
     all paradigms or might not support specific optimizations.
     """
     for proj in projections:
         # Most of the sparse matrix formats are not trivially invertable and therefore we can not implement
         # spiking models with them
-        if proj.synapse_type.type == "spike" and proj._storage_format in ["csr_vector", "csr_scalar", "ell", "ellr", "coo", "hyb", "bsr"]:
+        if proj.synapse_type.type == "spike" and proj._storage_format in ["csr_vector", "csr_scalar", "ell", "ellr", "coo", "hyb"]:
             raise Global.ANNarchyException("Using 'storage_format="+ proj._storage_format + "' is not allowed for spiking synapses.", True)
 
         # For some of the sparse matrix formats we don't implemented plasticity yet.
         if proj.synapse_type.type == "spike":
-            if proj._storage_format in ["dense"] and not isinstance(proj.synapse_type, DefaultSpikingSynapse):
-                raise Global.ANNarchyException("Using 'storage_format="+ proj._storage_format + "' is only allowed for default spiking synapses yet.", True)
-
             if Global._check_paradigm("cuda") and proj._storage_format in ["csr"] and proj._storage_order=="pre_to_post" and not isinstance(proj.synapse_type, DefaultSpikingSynapse):
                 raise Global.ANNarchyException("Using 'storage_format="+ proj._storage_format + "' and 'storage_order="+ proj._storage_order + "' is on GPUs only allowed for default spiking synapses yet.", True)
 
             # Continous transmission, e.g. gap junctions, should not be combined with pre-to-post
             if 'psp' in  proj.synapse_type.description.keys() and proj._storage_order=="pre_to_post":
                 raise Global.ANNarchyException("Using continuous transmission within a spiking synapse prevents the application of pre-to-post matrix ordering", True)
 
@@ -226,15 +206,16 @@
                     raise Global.ANNarchyException("Using 'storage_format="+ proj._storage_format + "' is and non-uniform delays is not implemented.", True)
 
         if not Global._check_paradigm("cuda") and (proj._storage_format in ["csr_scalar", "csr_vector"]):
             Global._error("The CSR variants csr_scalar/csr_vector are only intended for GPUs.")
 
         if Global._check_paradigm("cuda") and proj._storage_format == "lil":
             proj._storage_format = "csr"
-            Global._info("LIL-type projections are not available for GPU devices ... default to CSR")
+            if not isinstance(proj, SpecificProjection):
+                Global._info("LIL-type projections are not available for GPU devices ... default to CSR")
 
         if Global._check_paradigm("cuda") and proj._storage_format == "ell":
             Global._info("We would recommend to use ELLPACK-R (format=ellr) on GPUs.")
 
 def _check_prepost(populations, projections):
     """
     Checks that when a synapse uses pre.x r post.x, the variable x exists in the corresponding neuron
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Template/BaseTemplate.py` & `ANNarchy-4.7.3/ANNarchy/generator/Template/BaseTemplate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 omp_header_template = """#pragma once
 
 #include <string>
 #include <vector>
 #include <algorithm>
 #include <map>
 #include <deque>
@@ -87,26 +92,32 @@
 
 /*
  *  Initialization
  */
 void initialize(const %(float_prec)s dt_) ;
 
 /*
+ *  Life-time management
+ */
+void create_cpp_instances();
+void destroy_cpp_instances();
+
+/*
  * Time export
  *
-*/
+ */
 long int getTime();
 void setTime(const long int t_);
 %(float_prec)s getDt();
 void setDt(const %(float_prec)s dt_);
 
 /*
  * Number of threads
  *
-*/
+ */
 void setNumberThreads(int threads, std::vector<int> core_list);
 
 /*
  * Seed for the RNG
  *
 */
 void setSeed(long int seed, int num_sources, bool use_seed_seq);
@@ -165,15 +176,18 @@
     if (id < recorders.size())
         return recorders[id];
     else
         return nullptr;
 }
 void removeRecorder(Monitor* recorder){
     for (unsigned int i=0; i<recorders.size(); i++){
-        if(recorders[i] == recorder){
+        if (recorders[i] == recorder) {
+            // delete the present instance
+            delete recorders[i];
+            // mark the slot as free
             recorders[i] = nullptr;
             break;
         }
     }
 }
 
 /*
@@ -329,14 +343,29 @@
 
     rng.push_back(std::mt19937(seed));
 
     rng.shrink_to_fit();
 }
 
 /*
+ *  Life-time management
+ */
+void create_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Instantiate C++ objects ..." << std::endl;
+#endif
+}
+
+void destroy_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Destroy C++ objects ..." << std::endl;
+#endif
+}
+
+/*
  * Access to time and dt
  */
 long int getTime() {return t;}
 void setTime(const long int t_) { t=t_;}
 %(float_prec)s getDt() { return dt;}
 void setDt(const %(float_prec)s dt_) { dt=dt_;}
 
@@ -433,15 +462,16 @@
     if (id < recorders.size())
         return recorders[id];
     else
         return nullptr;
 }
 void removeRecorder(Monitor* recorder){
     for (unsigned int i=0; i<recorders.size(); i++){
-        if(recorders[i] == recorder){
+        if (recorders[i] == recorder) {
+            delete recorders[i];
             recorders[i] = nullptr;
             break;
         }
     }
 }
 
 /*
@@ -682,27 +712,51 @@
         }
     }
 
     rng.shrink_to_fit();
 }
 
 /*
+ *  Life-time management
+ */
+void create_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Instantiate C++ objects ..." << std::endl;
+#endif
+}
+
+void destroy_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Destroy C++ objects ..." << std::endl;
+#endif
+}
+
+/*
  * Access to time and dt
  */
 long int getTime() {return t;}
 void setTime(const long int t_) { t=t_;}
 %(float_prec)s getDt() { return dt;}
 void setDt(const %(float_prec)s dt_) { dt=dt_;}
 
 /*
  * Number of threads
  *
  */
 void setNumberThreads(const int threads, const std::vector<int> core_list)
 {
+#ifdef _DEBUG
+    std::cout << "Set new number of threads:" << threads << std::endl;
+    if (!core_list.empty()) {
+        std::cout << "Use thread placement: [";
+        for (auto it = core_list.begin(); it != core_list.end(); it++) std::cout << *it << " ";
+        std::cout << "]";
+    }
+#endif
+
     // set worker set size
     global_num_threads = threads;
 
 #ifdef __linux__
     // set a cpu mask to prevent moving of threads
     cpu_set_t mask;
 
@@ -865,14 +919,20 @@
 #endif
     cudaError_t err = cudaSetDevice(device_id);
     if ( err != cudaSuccess )
         std::cerr << "Set device " << device_id << ": " << cudaGetErrorString(err) << std::endl;
 }
 
 /*
+ *  Life-time management
+ */
+void create_cpp_instances();
+void destroy_cpp_instances();
+
+/*
  * Time export
  */
 long int getTime();
 void setTime(const long int t_);
 %(float_prec)s getDt();
 void setDt(const %(float_prec)s dt_);
 
@@ -880,19 +940,19 @@
  * Seed for the RNG (host-side!)
  */
 void setSeed(const long int seed, const int num_sources, const bool use_seed_seq);
 
 #endif
 """
 
-cuda_device_kernel_template = """#include <cuda_runtime_api.h>
-#include <curand_kernel.h>
-#include <float.h>
-#include <stdio.h>
-#include <iostream>
+cuda_device_kernel = """#include "ANNarchyKernel.cuh"
+
+/********************************************************************/
+/*  Device kernel definitions                                       */
+/********************************************************************/
 
 /****************************************
  * atomicAdd for non-Pascal             *
  ****************************************/
 #if !defined(__CUDA_ARCH__) || __CUDA_ARCH__ >= 600
 #else
     __device__ double atomicAdd(double* address, double val)
@@ -925,17 +985,17 @@
     while( i < N )
     {
         curand_init( seed, i+sequence_offset, 0, &states[ i ] );
         i += blockDim.x * gridDim.x;
     }
 }
 
-/******************************************
- * clear psp-related state variables      *
- ******************************************/
+/****************************************
+ * clear psp-related state variables    *
+ ****************************************/
 __global__ void clear_num_events(unsigned int* num_events) {
     *num_events = 0;
 }
 
 __global__ void clear_sum(int num_elem, %(float_prec)s *sum) {
     int j = threadIdx.x + blockIdx.x * blockDim.x;
 
@@ -985,46 +1045,19 @@
  ****************************************/
 %(glob_ops_kernel)s
 
 /****************************************
  * postevent kernel                     *
  ****************************************/
 %(postevent_kernel)s
-"""
-
-cuda_host_body_template =\
-"""#include "ANNarchy.h"
-%(prof_include)s
-#include <math.h>
-
-// cuda specific header
-#include <cuda_runtime_api.h>
-#include <curand.h>
-#include <float.h>
-
-// Directly set the number of blocks/number of threads
-%(kernel_config)s
-
-// Required by Bell & Garland Kernel
-#define MAX_THREADS (30 * 1024)
-#define DIVIDE_INTO(x,y) ((x + y - 1)/y)
 
-// Kernel definitions
-__global__ void update_t(int t_host);
-__global__ void clear_sum(int num_elem, %(float_prec)s *sum);
-__global__ void clear_num_events(unsigned int* num_events);
-%(kernel_def)s
 
-// Custom Constant
-%(custom_constant)s
-
-//
-// Handling GPU and CPU rng
-//
-__global__ void rng_setup_kernel( int N, long long int offset, curandState* states, unsigned long long seed );
+/********************************************************************/
+/*  Device kernel invocations                                       */
+/********************************************************************/
 
 // We need to generate different state sequences per kernel call
 static long long int sequence_offset=0;
 
 void init_curand_states( int N, curandState* states, unsigned long long seed ) {
     int numThreads = 64;
     int numBlocks = ceil (float(N) / float(numThreads));
@@ -1035,14 +1068,109 @@
 #ifdef _DEBUG
     cudaError_t err = cudaGetLastError();
     if ( err != cudaSuccess )
         std::cout << "init_curand_state: " << cudaGetErrorString(err) << std::endl;
 #endif
 }
 
+void call_clear_sum(RunConfig cfg, int num_elem, %(float_prec)s *sum) {
+    clear_sum<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(num_elem, sum);
+}
+
+void call_clear_num_events(RunConfig cfg, unsigned int* num_events) {
+    clear_num_events<<<cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream>>>(num_events);
+}
+
+/****************************************
+ * updating neural variables            *
+ ****************************************/
+ %(pop_invoke_kernel)s
+
+/****************************************
+ * weighted sum kernels                 *
+ ****************************************/
+%(psp_invoke_kernel)s
+
+/****************************************
+ * update synapses kernel               *
+ ****************************************/
+%(syn_invoke_kernel)s
+
+/****************************************
+ * global operations kernel             *
+ ****************************************/
+%(glob_ops_invoke_kernel)s
+
+/****************************************
+ * postevent kernel                     *
+ ****************************************/
+%(postevent_invoke_kernel)s
+"""
+
+cuda_device_invoke_header ="""#pragma once
+#include <cuda_runtime_api.h>
+#include <curand_kernel.h>
+#include <float.h>
+#include <stdio.h>
+#include <iostream>
+
+// Encapsulates the four parameters required for a kernel invocation.
+struct RunConfig{
+    dim3 nb;
+    dim3 tpb;
+    int smem_size;
+    cudaStream_t stream;
+
+    RunConfig() = default;
+
+    RunConfig(int nb, int tpb, int smem_size, cudaStream_t stream) {
+        this->nb = dim3(nb,1,1);
+        this->tpb = dim3(tpb,1,1);
+        this->smem_size = smem_size;
+        this->stream = stream;
+    }
+
+    RunConfig(dim3 nb, dim3 tpb, int smem_size, cudaStream_t stream) {
+        this->nb = nb;
+        this->tpb = tpb;
+        this->smem_size = smem_size;
+        this->stream = stream;
+    }
+};
+
+// Pre-defined kernel definitions
+void init_curand_states( int N, curandState* states, unsigned long long seed );
+
+void call_clear_sum(RunConfig cfg, int num_elem, %(float_prec)s *sum);
+void call_clear_num_events(RunConfig cfg, unsigned int* num_events);
+
+// Model-related kernel definitions
+%(invoke_kernel_def)s
+
+"""
+
+cuda_host_body_template =\
+"""// ANNarchy-related header
+#include "ANNarchy.h"
+#include "ANNarchyKernel.cuh"
+
+%(prof_include)s
+#include <math.h>
+
+// Directly set the number of blocks/number of threads
+%(kernel_config)s
+
+// Required by Bell & Garland Kernel
+#define MAX_THREADS (30 * 1024)
+#define DIVIDE_INTO(x,y) ((x + y - 1)/y)
+
+//
+// Handling GPU and CPU rng
+//
+
 std::vector<std::mt19937> rng;
 unsigned long long global_seed;
 
 void setSeed(const long int seed, const int num_sources, const bool use_seed_seq){
     rng.clear();
 
     if (num_sources == 1) {
@@ -1069,15 +1197,48 @@
 
 /*
  * Internal data
  */
 %(float_prec)s dt;
 long int t;
 
-// Recorders
+// Populations
+%(pop_ptr)s
+
+// Projections
+%(proj_ptr)s
+
+// Stream configuration (available for CC > 3.x devices)
+// NOTE: if the CC is lower then 3.x modification of stream
+//       parameter (4th arg) is automatically ignored by CUDA
+%(stream_setup)s
+
+// Initialize the internal data
+void initialize(%(float_prec)s _dt) {
+%(initialize)s
+}
+
+/*
+ *  Life-time management
+ */
+void create_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Instantiate C++ objects ..." << std::endl;
+#endif
+}
+
+void destroy_cpp_instances() {
+#ifdef _DEBUG
+    std::cout << "Destroy C++ objects ..." << std::endl;
+#endif
+}
+
+/*
+ * Recorders
+ */
 std::vector<Monitor*> recorders;
 int addRecorder(Monitor* recorder){
     int found = -1;
 
     for (unsigned int i=0; i<recorders.size(); i++) {
         if (recorders[i] == nullptr) {
             found = i;
@@ -1098,37 +1259,22 @@
     if (id < recorders.size())
         return recorders[id];
     else
         return nullptr;
 }
 void removeRecorder(Monitor* recorder){
     for (unsigned int i=0; i<recorders.size(); i++){
-        if(recorders[i] == recorder){
+        if (recorders[i] == recorder) {
+            delete recorders[i];
             recorders[i] = nullptr;
             break;
         }
     }
 }
 
-// Populations
-%(pop_ptr)s
-
-// Projections
-%(proj_ptr)s
-
-// Stream configuration (available for CC > 3.x devices)
-// NOTE: if the CC is lower then 3.x modification of stream
-//       parameter (4th arg) is automatically ignored by CUDA
-%(stream_setup)s
-
-// Initialize the internal data
-void initialize(%(float_prec)s _dt) {
-%(initialize)s
-}
-
 /**
  *  Implementation remark (27.02.2015, HD) to: run(int), step() and single_step()
  *
  *  we have two functions in ANNarchy to run simulation code: run(int) and step(). The latter one to
  *  run several steps at once, the other one just a single step. On CUDA I face the problem, that I
  *  propably need to update variables before step() and definitly changed variables after step().
  *  run(int) calls step() normally, if I add transfer codes in step(), run(N) would end up in N
@@ -1195,15 +1341,15 @@
     // Postsynaptic events
     ////////////////////////////////
 %(post_event)s
 
     ////////////////////////////////
     // Recording neural/synaptic variables
     ////////////////////////////////
-%(prof_record_pre)s    
+%(prof_record_pre)s
     for (unsigned int i=0; i < recorders.size(); i++){
         if (recorders[i])
             recorders[i]->record();
     }
 %(prof_record_post)s
 
     ////////////////////////////////
@@ -1249,14 +1395,19 @@
 
 void step() {
 %(host_device_transfer)s
 %(prof_run_pre)s
     single_step();
 %(prof_run_post)s
 
+    auto err = cudaGetLastError();
+    if (err != cudaSuccess) {
+        std::cerr << "An error occured within simulation loop: " << cudaGetErrorString(err) << std::endl;
+    }
+
     cudaDeviceSynchronize();
 }
 
 /*
  * Access to time and dt
  *
  */
@@ -1303,14 +1454,17 @@
 
 %(prof_init)s
 
 %(pop_init)s
 
 %(proj_init)s
 
+    // global constants
+%(custom_constant)s
+
     // create streams
     stream_setup();
 """
 
 built_in_functions = """
 #define positive(x) (x>0.0? x : 0.0)
 #define negative(x) (x<0.0? x : 0.0)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Template/GlobalOperationTemplate.py` & `ANNarchy-4.7.3/ANNarchy/generator/Template/GlobalOperationTemplate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 global_operation_templates_st = {
     'max' : """
 // Computes the maximum value of an array
 %(type)s max_value(const %(type)s* array, int n)
 {
     %(type)s max = array[0];
     for(int i=1; i<n; i++)
@@ -258,15 +263,14 @@
 }
 
 #
 # determine correct kernel sizes
 #
 global_operation_templates_cuda = {
    'max' : {
-        'header' : """__global__ void cuMaxValue(%(type)s* result, %(type)s *gpu_array, int N);""",
         'body' : """// Computes the maximum value of an array
 __global__ void cuMaxValue(%(type)s* result, %(type)s *gpu_array, int N)
 {
     unsigned int tid = threadIdx.x;
     unsigned int i = tid;
 
     extern %(type)s __shared__ sdata[];
@@ -301,24 +305,34 @@
     // write result for this block to global mem
     if (tid == 0)
     {
         *result = sdata[0];
     }
 }
 """,
+        'invoke': """void cuda_max_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N) {
+    cuMaxValue <<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>> ( result, gpu_array, N );
+}
+""",
+        'header': """void cuda_max_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N);""",
+
         'call' : """
     if ( pop%(id)s._active ) {
-        cuMaxValue <<< 1, 32, 64 * 8 >>> ( pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
+        cuda_max_value(RunConfig(1, 32, 64 * sizeof(%(type)s), pop%(id)s.stream), pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
         cudaMemcpy(&pop%(id)s._max_%(var)s, pop%(id)s._gpu_%(op)s_%(var)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
+    #ifdef _DEBUG
+        auto glob_%(op)s_pop%(id)s_err = cudaGetLastError();
+        if (glob_%(op)s_pop%(id)s_err != cudaSuccess)
+            std::cerr << "Global operation '%(op)s' (PopStruct%(id)s): " <<  << std::endl;
+    #endif
     }
 """
     },
 
     'min' : {
-        'header' : """__global__ void cuMinValue(%(type)s* result, %(type)s *gpu_array, int N);""",
         'body' : """// Computes the minimum value of an array
 __global__ void cuMinValue(%(type)s* result, %(type)s *gpu_array, int N)
 {
     unsigned int tid = threadIdx.x;
     unsigned int i = tid;
 
     extern %(type)s __shared__ sdata[];
@@ -353,24 +367,29 @@
     // write result for this block to global mem
     if (tid == 0)
     {
         *result = sdata[0];
     }
 }
 """,
+        'invoke' : """
+void cuda_min_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N) {
+    cuMinValue <<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>> ( result, gpu_array, N );
+}
+""",
+        'header' : """void cuda_min_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N);""",
         'call' : """
     if ( pop%(id)s._active ) {
-        cuMinValue <<< 1, 32, 64 * 8 >>> ( pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
+        cuda_min_value(RunConfig(1, 32, 64 * sizeof(%(type)s), pop%(id)s.stream), pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
         cudaMemcpy(&pop%(id)s._min_%(var)s, pop%(id)s._gpu_%(op)s_%(var)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
     }
 """
     },
 
     'mean' : {
-        'header' : """__global__ void cuMeanValue(%(type)s* result, %(type)s *gpu_array, int N);""",
         'body' : """// Computes the mean value of an array
 __global__ void cuMeanValue(%(type)s* result, %(type)s *gpu_array, int N)
 {
     unsigned int tid = threadIdx.x;
     unsigned int i = tid;
 
     extern %(type)s __shared__ sdata[];
@@ -405,25 +424,29 @@
     // write result for this block to global mem
     if (tid == 0)
     {
         *result = sdata[0] / (%(type)s)N;
     }
 }
 """,
-    'call' : """
+        'invoke' : """void cuda_mean_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N) {
+    cuMeanValue <<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>> ( result, gpu_array, N );
+}
+""",
+        'header' : """void cuda_mean_value(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N);""",
+        'call' : """
     if ( pop%(id)s._active ) {
-        cuMeanValue <<< 1, 32, 64 * 8 >>> ( pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
+        cuda_mean_value(RunConfig(1, 32, 64 * sizeof(%(type)s), pop%(id)s.stream), pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
         cudaMemcpy(&pop%(id)s._%(op)s_%(var)s, pop%(id)s._gpu_%(op)s_%(var)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
     }
 """
     },
 
     # Computes the L1-norm of an array
     'norm1' : {
-        'header' : """__global__ void cuNorm1(%(type)s* result, %(type)s *gpu_array, int N);""",
         'body' : """// Computes the L1-norm value of an array
 __global__ void cuNorm1(%(type)s* result, %(type)s *gpu_array, int N)
 {
     unsigned int tid = threadIdx.x;
     unsigned int i = tid;
 
     extern %(type)s __shared__ sdata[];
@@ -458,25 +481,30 @@
     // write back result
     if (tid == 0)
     {
         *result = sdata[0];
     }
 }
 """,
-    'call' : """
+        'invoke': """
+void cuda_norm1(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N) {
+    cuNorm1<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(result, gpu_array, N);
+}
+""",
+        'header' : """void cuda_norm1(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N);""",
+        'call' : """
     if ( pop%(id)s._active ) {
-        cuNorm1 <<< 1, 32, 64 * 8 >>> ( pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
+        cuda_norm1(RunConfig(1, 32, 64 * sizeof(%(type)s), pop%(id)s.stream), pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
         cudaMemcpy(&pop%(id)s._%(op)s_%(var)s, pop%(id)s._gpu_%(op)s_%(var)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
     }
 """
     },
 
     # Computes the L2-norm (Euclidian) of an array
     'norm2' : {
-        'header' : """__global__ void cuNorm2(%(type)s* result, %(type)s *gpu_array, int N);""",
         'body' : """// Computes the L2-norm value of an array
 __global__ void cuNorm2(%(type)s* result, %(type)s *gpu_array, int N)
 {
     unsigned int tid = threadIdx.x;
     unsigned int i = tid;
 
     extern %(type)s __shared__ sdata[];
@@ -511,15 +539,21 @@
     // write back result
     if (tid == 0)
     {
         *result = sqrt(sdata[0]);
     }
 }
 """,
-    'call' : """
+        'invoke': """
+void cuda_norm2(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N) {
+    cuNorm2<<< cfg.nb, cfg.tpb, cfg.smem_size, cfg.stream >>>(result, gpu_array, N);
+}
+""",
+        'header' : """void cuda_norm2(RunConfig cfg, %(type)s* result, %(type)s *gpu_array, int N);""",
+        'call' : """
     if ( pop%(id)s._active ) {
-        cuNorm2 <<< 1, 32, 64 * 8 >>> ( pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
+        cuda_norm2(RunConfig(1, 32, 64 * sizeof(%(type)s), pop%(id)s.stream), pop%(id)s._gpu_%(op)s_%(var)s, pop%(id)s.gpu_%(var)s, pop%(id)s.size );
         cudaMemcpy(&pop%(id)s._%(op)s_%(var)s, pop%(id)s._gpu_%(op)s_%(var)s, sizeof(%(type)s), cudaMemcpyDeviceToHost);
     }
 """
     }
-}
+}
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Template/MakefileTemplate.py` & `ANNarchy-4.7.3/ANNarchy/generator/Template/MakefileTemplate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+"""
+MAKEFILE templates.
+
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 # Linux, Seq or OMP
 linux_omp_template = """# Makefile generated by ANNarchy
 all:
 \t%(cython)s -%(py_major)s --cplus %(cython_ext)s -D ANNarchyCore%(net_id)s.pyx
 \t%(compiler)s %(cpu_flags)s -std=c++14 -fPIC -shared %(openmp)s \\
         *.cpp  %(add_sources)s -o ANNarchyCore%(net_id)s.so \\
         %(python_include)s -I%(numpy_include)s -I%(annarchy_include)s -I%(thirdparty_include)s \\
@@ -15,22 +22,22 @@
 \trm -rf *.so
 """
 
 # Linux, CUDA
 linux_cuda_template = """# Makefile generated by ANNarchy
 all:
 \t%(cython)s -%(py_major)s --cplus %(cython_ext)s -D ANNarchyCore%(net_id)s.pyx
-\t%(gpu_compiler)s %(gpu_flags)s -std=c++14 -c -Xcompiler -std=c++14,-fPIC, ANNarchyDevice.cu -o ANNarchyDevice.o
-\t%(gpu_compiler)s %(cuda_gen)s %(gpu_flags)s -Xcompiler %(cpu_flags)s-std=c++14,-fPIC,-shared \\
-        ANNarchyHost.cu *.cpp ANNarchyDevice.o -o ANNarchyCore%(net_id)s.so \\
+\t%(gpu_compiler)s %(gpu_flags)s -std=c++14 -c -Xcompiler %(xcompiler_flags)s-std=c++14,-fPIC, ANNarchyKernel.cu -o ANNarchyKernel.o
+\t%(compiler)s %(cpu_flags)s -std=c++14 -fPIC -shared \\
+        *.cpp ANNarchyKernel.o -o ANNarchyCore%(net_id)s.so \\
         %(python_include)s -I%(numpy_include)s -I%(annarchy_include)s \\
         %(cython_ext)s \\
         %(python_lib)s \\
         %(gpu_ldpath)s \\
-        %(python_libpath)s %(extra_libs)s
+        %(python_libpath)s -lcurand -lcudart %(extra_libs)s
 \tmv ANNarchyCore%(net_id)s.so ../..
 
 clean:
 \trm -rf *.o
 \trm -rf *.so
 """
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Template/PyxTemplate.py` & `ANNarchy-4.7.3/ANNarchy/generator/Template/PyxTemplate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     PyxTemplate.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2021  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 pyx_template = '''# cython: embedsignature=True
 from cpython.exc cimport PyErr_CheckSignals
 from libcpp.vector cimport vector
 from libcpp.map cimport map, pair
 from libcpp cimport bool
 from libcpp.string cimport string
 from math import ceil
@@ -65,15 +47,17 @@
 %(monitor_struct)s
 
     # Instances
 %(pop_ptr)s
 %(proj_ptr)s
 
     # Methods
+    void create_cpp_instances()
     void initialize(%(float_prec)s)
+    void destroy_cpp_instances()
     void setSeed(long, int, bool)
     void run(int nbSteps) nogil
     int run_until(int steps, vector[int] populations, bool or_and)
     void step()
 
     # Time
     long getTime()
@@ -99,17 +83,21 @@
 
 # User-defined functions
 %(functions_wrapper)s
 
 # User-defined constants
 %(constants_wrapper)s
 
-# Initialize the network
-def pyx_create(%(float_prec)s dt):
+# Initialize/Destroy the network
+def pyx_create():
+    create_cpp_instances()
+def pyx_initialize(%(float_prec)s dt):
     initialize(dt)
+def pyx_destroy():
+    destroy_cpp_instances()
 
 # Simple progressbar on the command line
 def progress(count, total, status=''):
     """
     Prints a progress bar on the command line.
 
     adapted from: https://gist.github.com/vladignatyev/06860ec2040cb497f0f3
@@ -315,14 +303,15 @@
 
 # Export for projections
 proj_pyx_struct = """
     # Export Projection %(id_proj)s
     cdef struct ProjStruct%(id_proj)s :
         # Flags
         bool _transmission
+        bool _axon_transmission
         bool _plasticity
         bool _update
         int _update_period
         long _update_offset
 
         # Connectivity
 %(export_connectivity)s
@@ -349,24 +338,26 @@
 cdef class proj%(id_proj)s_wrapper :
 
     def __init__(self, %(wrapper_args)s):
         %(wrapper_init)s
 
 %(wrapper_connector_call)s
 
-    property size:
-        def __get__(self):
-            return proj%(id_proj)s.nb_dendrites()
-
     # Transmission flag
     def _get_transmission(self):
         return proj%(id_proj)s._transmission
     def _set_transmission(self, bool l):
         proj%(id_proj)s._transmission = l
 
+    # Transmission flag (axon spikes)
+    def _get_axon_transmission(self):
+        return proj%(id_proj)s._axon_transmission
+    def _set_axon_transmission(self, bool l):
+        proj%(id_proj)s._axon_transmission = l
+
     # Update flag
     def _get_update(self):
         return proj%(id_proj)s._update
     def _set_update(self, bool l):
         proj%(id_proj)s._update = l
 
     # Plasticity flag
@@ -414,14 +405,18 @@
         vector[%(idx_type)s] get_dendrite_pre_rank(%(idx_type)s)
         %(size_type)s nb_synapses()
         %(idx_type)s nb_dendrites()
         %(idx_type)s dendrite_size(%(idx_type)s)
 """
 
 pyx_default_conn_wrapper = """
+    property size:
+        def __get__(self):
+            return proj%(id_proj)s.nb_dendrites()
+
     def post_rank(self):
         return proj%(id_proj)s.get_post_rank()
     def pre_rank_all(self):
         return proj%(id_proj)s.get_pre_ranks()
     def pre_rank(self, int n):
         return proj%(id_proj)s.get_dendrite_pre_rank(n)
     def nb_dendrites(self):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/generator/Utils.py` & `ANNarchy-4.7.3/ANNarchy/generator/Utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Utils.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core import Global
 from ANNarchy.core.PopulationView import PopulationView
 
 import re
 import subprocess
 import sys
 
@@ -308,30 +290,35 @@
     # The user disabled this feature
     if not Global.config["use_cpp_connectors"]:
         return False
 
     cpp_patterns = {
         'st': {
             'post_to_pre': {
-                "lil": ["Random", "Random Convergent"],
+                "lil": ["Random", "Random Convergent", "All-to-All"],
                 "csr": ["Random", "Random Convergent"],
                 "coo": [],
                 "hyb": [],
                 "ell": [],
                 "dense": ["Random"]
             },
             'pre_to_post': {
                 "csr": ["Random", "Random Convergent"]
             }
         },
         'omp': {
-            "lil": [],
-            "csr": [],
-            "coo": [],
-            "ell": []
+            'post_to_pre': {
+                "lil": ["Random"],
+                "csr": [],
+                "coo": [],
+                "ell": []
+            },
+            'pre_to_post': {
+                "csr": ["Random"]
+            }
         },
         'cuda': {
             'post_to_pre': {
                 "csr": ["Random", "Random Convergent"],
                 "coo": [],
                 "ellr": ["Random", "Random Convergent"],
                 "dense": ["Random"]
@@ -385,15 +372,18 @@
     """
     Some features like atomic add for double values and power function are dependent on the CUDA version.
     """
     version_str = str(subprocess.check_output([nvcc_executable, "--version"]))
     try:
         version = float(version_str.split("\\")[-2].split(",")[1].split(" ")[2])
     except:
-        Global._error("Could not detect CUDA version: please check the CUDA installation or the configuration in annarchy.json")
+        try:
+            version = float(version_str.split("\\")[-3].split(",")[1].split(" ")[2])
+        except:
+            Global._error("Could not detect CUDA version: please check the CUDA installation or the configuration in annarchy.json")
 
     return version
 
 def check_and_apply_pow_fix(eqs):
     """
     CUDA SDKs before 7.5 had an error if std=c++11 is enabled related
     to pow(double, int). Only pow(double, double) was detected as
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/BSRMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/BSRMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     /**
      *  @brief      check if the matrix fits into RAM
      *  @details    Unlike CUDA it appears that the standard C++ API does not
      *              provide a function to get the available RAM at a present time.
      *              Many sources recommended to use the /proc/meminfo file
      */
     bool check_free_memory(size_t required) {
+    #ifdef __linux__
         FILE *meminfo = fopen("/proc/meminfo", "r");
         
         // TODO:    I'm not completely sure, what we want to do
         //          in this case. Currently, we would hope for the best ...
         if(meminfo == nullptr) {
             std::cerr << "Could not read '/proc/meminfo'. ANNarchy can not catch to large allocations ..." << std::endl;
             return true;
@@ -77,14 +78,18 @@
 
         fclose(meminfo);
         size_t available = static_cast<size_t>(ram) * 1024;
     #ifdef _DEBUG
         std::cout << "BSRMatrix: allocate " << required << " from " << available << " bytes " << std::endl;
     #endif
         return required < available;
+
+    #else
+        return true;
+    #endif
     }
 
     // Attention: this function returns the LIL indices, this easier for the following processing
     std::vector<std::vector<IT>> split_row_indices(std::vector<IT>& row_indices, IT nb_block_rows) {
     #ifdef _DEBUG
         std::cout << "BSRMatrix::split_row_indices()" << std::endl;
     #endif
@@ -288,14 +293,18 @@
         // last row
         this->block_row_pointer_[nb_block_rows] = this->block_column_index_.size();
 
         // sanity check (did we allocate enough dense blocks?)
         std::cout << total_blocks << " times " << tile_size_ << "x" << tile_size_ << "-> " << total_blocks * tile_size_ * tile_size_ << " elements." << std::endl;
         assert( this->tile_data_.size() == (total_blocks * tile_size_ * tile_size_) );
 
+        // remove unneccessary allocated space
+        this->block_column_index_.shrink_to_fit();
+        this->tile_data_.shrink_to_fit();
+
         return true;
     }
 
     //
     //  Accessors for the Python ANNarchy interface
     //
 
@@ -612,8 +621,25 @@
         size += block_row_pointer_.capacity() * sizeof(IT);
         size += block_column_index_.capacity() * sizeof(IT);
         size += tile_data_.capacity() * sizeof(char);
         size += post_ranks_.capacity() * sizeof(IT);
 
         return size;
     }
+
+    void print_data_representation(bool print_memory_footprint=true) {
+        std::cout << "BSR tile size:        " << this->tile_size_ << std::endl;
+        std::cout << "Number of block rows: " << this->block_row_pointer_.size()-1 << std::endl;
+        std::cout << "block column indices = [ ";
+        for (IT block_row_idx = 0; block_row_idx < this->block_row_pointer_.size()-1; block_row_idx++ ) {
+            std::cout << "[ ";
+            for (IT blk_col_idx = block_row_pointer_[block_row_idx]; blk_col_idx < block_row_pointer_[block_row_idx+1]; blk_col_idx++) {
+                std::cout << block_column_index_[blk_col_idx] << " ";
+            }
+            std::cout << "] ";
+        }
+        std::cout << "]" << std::endl;
+
+        if (print_memory_footprint)
+            std::cout << "Requires " << (this->size_in_bytes() / 1024.0 / 1024) << "MB (~" << this->size_in_bytes() / this->nb_synapses() << " bytes per non-zero)" << std::endl;
+    }
 };
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/BSRMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/BSRMatrixCUDA.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -44,17 +44,26 @@
     #ifdef _DEBUG
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
         return required < free;
     }
 
     void free_device_memory() {
-        cudaFree(gpu_block_row_pointer_);
-        cudaFree(gpu_block_column_index_);
-        cudaFree(gpu_tile_data_);
+        if (gpu_block_row_pointer_) {
+            cudaFree(gpu_block_row_pointer_);
+            gpu_block_row_pointer_ = nullptr;
+        }
+        if (gpu_block_column_index_) {
+            cudaFree(gpu_block_column_index_);
+            gpu_block_column_index_ = nullptr;
+        }
+        if (gpu_tile_data_) {
+            cudaFree(gpu_tile_data_);
+            gpu_tile_data_ = nullptr;
+        }
     }
 
     bool transfer_to_device() {
         // Allocate 
         cudaMalloc((void**)&gpu_block_row_pointer_, this->block_row_pointer_.size() * sizeof(IT));
         cudaMalloc((void**)&gpu_block_column_index_, this->block_column_index_.size() * sizeof(IT));
         cudaMalloc((void**)&gpu_tile_data_, this->tile_data_.size()*sizeof(char));
@@ -78,15 +87,17 @@
 
 public:
     BSRMatrixCUDA(const unsigned int num_rows, const unsigned int num_columns, const unsigned int block_size) :
         BSRMatrix<IT, ST, false>(num_rows, num_columns, block_size) {
     #ifdef _DEBUG
         std::cout << "BSRMatrixCUDA::BSRMatrixCUDA()" << std::endl;
     #endif
-
+            gpu_block_row_pointer_ = nullptr;
+            gpu_block_column_index_ = nullptr;
+            gpu_tile_data_ = nullptr;
         }
 
     /**
      *  @brief      Destructor
      *  @details    Please note, the clear() method should be called in advance.
      */
     ~BSRMatrixCUDA() {
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/COOMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/COOMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,18 @@
         for( ; post_it != post_ranks.end(); post_it++, pre_it++) {
             // #elements in this row we need the post index
             auto tmp = std::vector<IT>(pre_it->size(), *post_it);
 
             row_indices_.insert(row_indices_.end(), tmp.begin(), tmp.end());
             column_indices_.insert(column_indices_.end(), pre_it->begin(), pre_it->end());
         }
+
+        // remove unneccessary allocated space
+        row_indices_.shrink_to_fit();
+        column_indices_.shrink_to_fit();
     
     #ifdef _DEBUG
         std::cout << row_indices_.size() << " coordinate pairs created." << std::endl;
 
     #ifdef _DEBUG_CONN
         auto row_it = row_indices_.begin();
         auto col_it = column_indices_.begin();
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/COOMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/COOMatrixCUDA.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,26 @@
     #ifdef _DEBUG
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
         return required < free;
     }
 
     void free_device_memory() {
-        cudaFree(gpu_row_indices_);
-        cudaFree(gpu_column_indices_);
+        if (gpu_row_indices_) {
+            cudaFree(gpu_row_indices_);
+            gpu_row_indices_ = nullptr;
+        }
+        if (gpu_column_indices_) {
+            cudaFree(gpu_column_indices_);
+            gpu_column_indices_ = nullptr;
+        }
+        if (gpu_segments_) {
+            cudaFree(gpu_segments_);
+            gpu_segments_ = nullptr;
+        }
 
         auto err = cudaGetLastError();
         if (err != cudaSuccess)
             std::cerr << "COOMatrixCUDA::free_device_memory(): " << cudaGetErrorString(err) << std::endl;
     }
 
     bool host_to_device_transfer() {
@@ -108,15 +118,17 @@
         }
         */
     #endif
     }
 
   public:
     explicit COOMatrixCUDA<IT, ST, SEGMENT_SIZE>(const IT num_rows, const IT num_columns) : COOMatrix<IT, ST>(num_rows, num_columns) {
-
+        gpu_row_indices_ = nullptr;
+        gpu_column_indices_ = nullptr;
+        gpu_segments_ = nullptr;
     }
 
     COOMatrixCUDA<IT, ST, SEGMENT_SIZE>( COOMatrix<IT, ST>* other ) : COOMatrix<IT, ST>( other ) {
     #ifdef _DEBUG
         std::cout << "COOMatrixCUDA::copy constructor"<< std::endl;
     #endif
         compute_segments();
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/CSRCMatrix.hpp`

 * *Files 16% similar despite different names*

```diff
@@ -200,22 +200,28 @@
                 _inv_idx.insert(_inv_idx.end(), inv_idx[i].begin(), inv_idx[i].end());
 
                 curr_off += inv_post_rank[i].size();
             }
         }
         _col_ptr.push_back(curr_off);
 
-        if ( this->num_non_zeros_ != curr_off )
+        // remove unneccessary allocated space
+        _row_idx.shrink_to_fit();
+        _inv_idx.shrink_to_fit();
+
+        // sanity check
+        if ( this->num_non_zeros_ != curr_off ) {
             std::cerr << "Something went wrong: (nb_synapes = " << this->num_non_zeros_ << ") != (curr_off = " << curr_off << ")" << std::endl;
-    #ifdef _DEBUG_CONN
-        std::cout << "Pre to Post:" << std::endl;
-        for ( int i = 0; i < this->num_columns_; i++ ) {
-            std::cout << i << ": " << col_ptr[i] << " -> " << col_ptr[i+1] << std::endl;
+        } else {
+        #if defined(_DEBUG_CONN)
+            print_data_representation(2, true);
+        #elif defined(_DEBUG)
+            print_data_representation(2, false);
+        #endif
         }
-    #endif
     }
 
     /**
      *  @brief      get a list of pre-synaptic neuron ranks and their efferent connections.
      *  @details    while the LILMatrix::nb_synapses and LILMatrix::nb_synapses_per_dendrite are row-centered this
      *              function contains the number of row entries for all columns with at least one row entry.
      *  @returns    a std::map with the pre-synaptic ranks as index and the number of nonzeros per column.
@@ -249,8 +255,46 @@
         size += sizeof(std::vector<IT>);
         size += _row_idx.capacity() * sizeof(IT);
         size += sizeof(std::vector<IT>);
         size += _inv_idx.capacity() * sizeof(ST);
 
         return size;
     }
+
+    void print_data_representation(int indent_spaces=0, bool print_container=true) {
+        int empty_columns = 0;
+        for (IT r = 0; r < _col_ptr.size()-1; r++ ) {
+            if (_col_ptr[r+1]-_col_ptr[r] == 0)
+                empty_columns++;
+        }
+
+        if (print_container) {
+            std::cout << std::string(indent_spaces, ' ') << "Forward view:" << std::endl;
+            static_cast<CSRMatrix<IT, ST>*>(this)->print_data_representation(indent_spaces+2, print_container);
+
+            std::cout << std::string(indent_spaces, ' ') << "Backward view:" << std::endl;
+            std::cout << std::string(indent_spaces+2, ' ') << "#empty columns: " << empty_columns << std::endl;
+            std::cout << std::string(indent_spaces+2, ' ') << "CSRCMatrix instance at " << this << std::endl;
+
+            std::cout << std::string(indent_spaces+4, ' ') << "col_begin = [ ";
+            for (IT c = 0; c < _col_ptr.size(); c++ ) {
+                std::cout << static_cast<unsigned long>(_col_ptr[c]) << " ";
+            }
+            std::cout << "]" << std::endl;
+
+            std::cout << std::string(indent_spaces+4, ' ') << "row_idx = [ ";
+            for (auto i = 0; i < _row_idx.size(); i++ ) {
+                std::cout << static_cast<unsigned long>(_row_idx[i]) << " ";
+            }
+            std::cout << "]" << std::endl;
+
+            std::cout << std::string(indent_spaces+4, ' ') << "inv_idx = [ ";
+            for (auto i = 0; i < _inv_idx.size(); i++ ) {
+                std::cout << static_cast<unsigned long>(_row_idx[i]) << " ";
+            }
+            std::cout << "]" << std::endl;
+        }else {
+            std::cout << std::string(indent_spaces, ' ') << "#empty columns: " << empty_columns << std::endl;
+        }
+
+    }
 };
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/CSRCMatrixCUDA.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,40 @@
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
         return (required < free);
     }
 
     void free_device_memory() {
         // CSR forward view
-        cudaFree(gpu_post_rank);
-        cudaFree(gpu_row_ptr);
-        cudaFree(gpu_pre_rank);
+        if (gpu_post_rank) {
+            cudaFree(gpu_post_rank);
+            gpu_post_rank = nullptr;
+        }
+        if (gpu_row_ptr) {
+            cudaFree(gpu_row_ptr);
+            gpu_row_ptr = nullptr;
+        }
+        if (gpu_pre_rank) {
+            cudaFree(gpu_pre_rank);
+            gpu_pre_rank = nullptr;
+        }
 
         // backward view
-        cudaFree(gpu_col_ptr);
-        cudaFree(gpu_row_idx);
-        cudaFree(gpu_inv_idx);
+        if (gpu_col_ptr) {
+            cudaFree(gpu_col_ptr);
+            gpu_col_ptr = nullptr;
+        }
+        if (gpu_row_idx) {
+            cudaFree(gpu_row_idx);
+            gpu_row_idx = nullptr;
+        }
+        if (gpu_inv_idx) {
+            cudaFree(gpu_inv_idx);
+            gpu_inv_idx = nullptr;
+        }
 
         // check for errors
         auto free_err = cudaGetLastError();
         if (free_err != cudaSuccess) {
             std::cerr << "CSRCMatrixCUDA::free_device_memory: " << cudaGetErrorString(free_err) << std::endl;
         }
     }
@@ -108,14 +126,21 @@
 
     // backward view
     ST* gpu_col_ptr;
     IT* gpu_row_idx;
     IT* gpu_inv_idx;
 
     explicit CSRCMatrixCUDA<IT, ST>(const IT num_rows, const IT num_columns) : CSRCMatrix<IT, ST>(num_rows, num_columns) {
+        gpu_post_rank = nullptr;
+        gpu_row_ptr = nullptr;
+        gpu_pre_rank = nullptr;
+
+        gpu_col_ptr = nullptr;
+        gpu_row_idx = nullptr;
+        gpu_inv_idx = nullptr;
     }
 
     /**
      *  @brief      Destructor
      */
     ~CSRCMatrixCUDA() {
     #ifdef _DEBUG
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixCUDAT.hpp` & `ANNarchy-4.7.3/ANNarchy/include/DenseMatrixCUDA.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 /*
- *    CSRCMatrixCUDAT.hpp
+ *    DenseMatrixCUDA.hpp
  *
  *    This file is part of ANNarchy.
  *
- *    Copyright (C) 2022    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
+ *    Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
+ *                        Julien Vitay <julien.vitay@gmail.com>
  *
  *    This program is free software: you can redistribute it and/or modify
  *    it under the terms of the GNU General Public License as published by
  *    the Free Software Foundation, either version 3 of the License, or
  *    (at your option) any later version.
  *
  *    ANNarchy is distributed in the hope that it will be useful,
@@ -16,187 +17,210 @@
  *    GNU General Public License for more details.
  *
  *    You should have received a copy of the GNU General Public License
  *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 #pragma once
 
-#include "CSRCMatrixT.hpp"
+#include "DenseMatrix.hpp"
 
-/**
- *  @brief      Implementation of the *compressed sparse row and column* format in transposed form on CUDA devices.
- *  @details    For more details on the format please refer to CSRCMatrixT.
+/*
+ *  @brief              Connectivity representation using a full matrix.
+ *  @details            Contrary to all other classes in this template library this matrix format is not a sparse matrix.
+ *  @tparam     IT      data type to represent the ranks within the matrix. Generally unsigned data types should be chosen.
+ *                      The data type determines the maximum size for the number of elements in a column respectively the number
+ *                      of rows encoded in the matrix:
+ * 
+ *                      - unsigned char (1 byte):        [0 .. 255]
+ *                      - unsigned short int (2 byte):   [0 .. 65.535]
+ *                      - unsigned int (4 byte):         [0 .. 4.294.967.295]
+ *
+ *                      The chosen data type should be able to represent the maximum values (LILMatrix::num_rows_ and ::num_columns_)
+ * 
+ *              ST      the second type should be used if the index type IT could overflow. For instance, the nb_synapses method should return ST as
+ *                      the maximum value in case a full dense matrix would be IT times IT entries.
+ *              MT      We need to store if a matrix value is set in a bitmask. The size of each entry is determined by MT (we recommend char as its only 1 byte).
  */
-template<typename IT = unsigned int, typename ST = unsigned long int>
-class CSRCMatrixCUDAT: public CSRCMatrixT<IT, ST> {
+template<typename IT = unsigned int, typename ST = unsigned long int, typename MT = char, bool row_major = false>
+class DenseMatrixCUDA : public DenseMatrix<IT, ST, MT, row_major> {
 protected:
-    bool check_free_device_memory(size_t required) {
+    MT* gpu_mask_;
+
+    bool check_free_memory(size_t required) {
         size_t free, total;
         cudaMemGetInfo( &free, &total );
     #ifdef _DEBUG
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
-        return (required < free);
+        return required < free;
     }
 
     void free_device_memory() {
     #ifdef _DEBUG
-        std::cout << "CSRCMatrixCUDAT::host_to_device()" << std::endl;
-    #endif        
-
-
-        // check for errors
+        std::cout << "DenseMatrixCUDA::free_device_memory()" << std::endl;
+    #endif
+        if (gpu_mask_) {
+            cudaFree(gpu_mask_);
+            gpu_mask_ = nullptr;
+        }
         auto free_err = cudaGetLastError();
         if (free_err != cudaSuccess) {
-            std::cerr << "CSRCMatrixCUDAT::free_device_memory: " << cudaGetErrorString(free_err) << std::endl;
+            std::cerr << "DenseMatrixCUDA::free_device_memory: " << cudaGetErrorString(free_err) << std::endl;
         }
     }
 
-    bool host_to_device_transfer() {
+    bool host_to_device() {
     #ifdef _DEBUG
-        std::cout << "CSRCMatrixCUDAT::host_to_device()" << std::endl;
+        std::cout << "DenseMatrixCUDA::host_to_device()" << std::endl;
     #endif
         //
-        //  Free (maybe) existing allocations
-        free_device_memory();
-
-        // Sanity check: can we allocate the data?
-        size_t req_size = sizeof(IT)*this->post_ranks_.size() + sizeof(ST)*this->row_ptr_.size() + sizeof(IT)*this->col_idx_.size() + this->col_ptr_.size()*sizeof(ST) + this->row_idx_.size()*sizeof(IT) + this->inv_idx_.size()*sizeof(IT);
-        if (!check_free_device_memory(req_size))
-            return false;
-
-        //
         //  Allocate device memory
-        cudaMalloc((void**)&gpu_post_rank, this->post_ranks_.size()*sizeof(IT));
-        cudaMalloc((void**)&gpu_row_ptr, this->row_ptr_.size()*sizeof(ST));
-        cudaMalloc((void**)&gpu_col_idx, this->col_idx_.size()*sizeof(IT));
-        cudaMalloc((void**)&gpu_col_ptr, this->col_ptr_.size()*sizeof(ST));
-        cudaMalloc((void**)&gpu_row_idx, this->row_idx_.size()*sizeof(IT));
-        cudaMalloc((void**)&gpu_inv_idx, this->inv_idx_.size()*sizeof(IT));
+        cudaMalloc((void**)&gpu_mask_, this->mask_.size()*sizeof(MT));
         auto malloc_err = cudaGetLastError();
         if (malloc_err != cudaSuccess) {
-            std::cerr << "CSRCMatrixCUDA::init_matrix_from_lil - cudaMalloc: " << cudaGetErrorString(malloc_err) << std::endl;
+            std::cerr << "CSRMatrixCUDA::init_matrix_from_lil - cudaMalloc: " << cudaGetErrorString(malloc_err) << std::endl;
             return false;
         }
 
         //
-        // Copy data
-        cudaMemcpy(gpu_post_rank, this->post_ranks_.data(), this->post_ranks_.size()*sizeof(IT), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_row_ptr, this->row_ptr_.data(), this->row_ptr_.size()*sizeof(ST), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_col_idx, this->col_idx_.data(), this->col_idx_.size()*sizeof(IT), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_col_ptr, this->col_ptr_.data(), this->col_ptr_.size()*sizeof(ST), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_row_idx, this->row_idx_.data(), this->row_idx_.size()*sizeof(IT), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_inv_idx, this->inv_idx_.data(), this->inv_idx_.size()*sizeof(IT), cudaMemcpyHostToDevice);
+        //  Copy data
+        cudaMemcpy(gpu_mask_, this->mask_.data(), this->mask_.size()*sizeof(MT), cudaMemcpyHostToDevice);
         auto copy_err = cudaGetLastError();
         if (copy_err != cudaSuccess) {
-            std::cerr << "CSRCMatrixCUDA::init_matrix_from_lil - cudaMemcpy: " << cudaGetErrorString(copy_err) << std::endl;
+            std::cerr << "CSRMatrixCUDA::init_matrix_from_lil - cudaMemcpy: " << cudaGetErrorString(copy_err) << std::endl;
             return false;
         }
 
         return true;
     }
 
 public:
-    // CSR forward view
-    IT* gpu_post_rank;
-    ST* gpu_row_ptr;
-    IT* gpu_col_idx;
-
-    // backward view
-    ST* gpu_col_ptr;
-    IT* gpu_row_idx;
-    IT* gpu_inv_idx;
 
-    /**
-     *  @brief      Constructor
-     */
-    explicit CSRCMatrixCUDAT<IT, ST>(const IT num_rows, const IT num_columns) : CSRCMatrixT<IT, ST>(num_rows, num_columns) {
+    explicit DenseMatrixCUDA(const IT num_rows, const IT num_columns): DenseMatrix<IT, ST, MT, row_major>(num_rows, num_columns) {
+    #ifdef _DEBUG
+        std::cout << "DenseMatrixCUDA::DenseMatrixCUDA()" << std::endl;
+    #endif
+        gpu_mask_ = nullptr;
     }
 
     /**
      *  @brief      Destructor
+     *  @details    calls the DenseMatrix::clear method. Is not declared as virtual as inheriting classes in our
+     *              framework should never be destroyed by the base pointer.
      */
-    ~CSRCMatrixCUDAT() {
+    ~DenseMatrixCUDA() {
     #ifdef _DEBUG
-        std::cout << "CSRCMatrixCUDA::~CSRCMatrixCUDA()" << std::endl;
+        std::cout << "DenseMatrixCUDA::~DenseMatrixCUDA()" << std::endl;
     #endif
+        clear();
+    }
+
+    inline MT* device_mask() {
+        return this->gpu_mask_;
     }
 
     /**
-     *  @brief      clear the matrix
-     *  @details    should be called before destructor.
+     *  @brief      Clear the dense matrix.
+     *  @details    Clears the connectivity data stored in the *post_rank* and *pre_rank* STL containers and free 
+     *              the allocated memory. **Important**: allocated variables are not effected by this!
      */
     void clear() {
     #ifdef _DEBUG
-        std::cout << "CSRCMatrixCUDA::clear()" << std::endl;
+        std::cout << "DenseMatrixCUDA::clear()" << std::endl;
     #endif
-        // clear host
-        static_cast<CSRCMatrixT<IT, ST>*>(this)->clear();
-
-        // clear device
-        free_device_memory();
     }
 
     bool init_matrix_from_lil(std::vector<IT> &row_indices, std::vector< std::vector<IT> > &column_indices) {
     #ifdef _DEBUG
-        std::cout << "CSRCMatrixCUDAT::init_matrix_from_lil() " << std::endl;
+        std::cout << "DenseMatrixCUDA::init_matrix_from_lil() " << std::endl;
     #endif
-        // host side
-        bool success = static_cast<CSRCMatrixT<IT, ST>*>(this)->init_matrix_from_lil(row_indices, column_indices);
+        // Initialization on host side
+        bool success = static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->init_matrix_from_lil(row_indices, column_indices);
         if (!success)
             return false;
 
-        // copy to gpu
-        return host_to_device_transfer();
+        // transfer to GPU
+        return host_to_device();
+    }
+
+    void fixed_probability_pattern(std::vector<int> post_ranks, std::vector<int> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
+    #ifdef _DEBUG
+        std::cout << "CSRMatrixCUDA::fixed_probability_pattern() " << std::endl;
+    #endif
+        // Initialization on host side
+        static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng);
+
+        // transfer to GPU
+        host_to_device();
     }
 
     //
     //  Variables
     //
     template <typename VT>
     VT* init_matrix_variable_gpu(const std::vector<VT> &host_variable) {
-        size_t size_in_bytes = this->num_non_zeros_*sizeof(VT);
-        if (!check_free_device_memory(size_in_bytes)) {
-            std::cerr << "Failed to allocate the GPU variable. Please check the available memory ..." << std::endl;
-            return nullptr;
-        }
+    #ifdef _DEBUG
+        std::cout << "DenseMatrixCUDA::init_matrix_variable_gpu()" << std::endl;
+    #endif
+        size_t num_dense_elem = this->num_rows_ * this->num_columns_;
+        assert( (num_dense_elem == host_variable.size()) );
 
         VT* gpu_variable;
-        cudaMalloc((void**)&gpu_variable, size_in_bytes);
-        cudaMemcpy(gpu_variable, host_variable.data(), size_in_bytes, cudaMemcpyHostToDevice);
+        cudaMalloc((void**)&gpu_variable, num_dense_elem*sizeof(VT));
+        cudaMemcpy(gpu_variable, host_variable.data(), num_dense_elem*sizeof(VT), cudaMemcpyHostToDevice);
+
+        auto err = cudaGetLastError();
+        if (err != cudaSuccess) {
+            std::cerr << "DenseMatrixCUDA::init_matrix_variable_gpu: " << cudaGetErrorString(err) << std::endl;
+        }
 
         return gpu_variable;
     }
 
     template <typename VT>
     VT* init_vector_variable_gpu(const std::vector<VT> &host_variable) {
-        size_t size_in_bytes = this->post_ranks_.size() * sizeof(VT);
-        if (!check_free_device_memory(size_in_bytes)) {
-            std::cerr << "Failed to allocate the GPU variable. Please check the available memory ..." << std::endl;
-            return nullptr;
-        }
+    #ifdef _DEBUG
+        std::cout << "DenseMatrixCUDA::init_vector_variable_gpu()" << std::endl;
+    #endif
+        assert( (this->num_rows_ == host_variable.size()) );
+        size_t size_in_bytes = this->num_rows_ * sizeof(VT);
+        check_free_memory(size_in_bytes);
 
         VT* gpu_variable;
         cudaMalloc((void**)&gpu_variable, size_in_bytes);
         cudaMemcpy(gpu_variable, host_variable.data(), size_in_bytes, cudaMemcpyHostToDevice);
 
+        auto err = cudaGetLastError();
+        if (err != cudaSuccess) {
+            std::cerr << "DenseMatrixCUDA::init_vector_variable_gpu: " << cudaGetErrorString(err) << std::endl;
+        }
+
         return gpu_variable;
     }
 
     //
     // Read-out variables from GPU and return as LIL
     //
     template <typename VT>
     std::vector<std::vector<VT>> get_device_matrix_variable_as_lil(VT* gpu_variable) {
         auto host_tmp = std::vector<std::vector<VT>>();
-        if (gpu_variable == nullptr)
-            return host_tmp;
 
-        auto flat_data = std::vector<VT>(this->num_non_zeros_, 0.0);
-        cudaMemcpy(flat_data.data(), gpu_variable, this->num_non_zeros_*sizeof(VT), cudaMemcpyDeviceToHost);
+        auto flat_data = std::vector<VT>(this->num_rows_*this->num_columns_, 0.0);
+        cudaMemcpy(flat_data.data(), gpu_variable, this->num_rows_*this->num_columns_*sizeof(VT), cudaMemcpyDeviceToHost);
 
-        for (auto post_rk = this->post_ranks_.cbegin(); post_rk != this->post_ranks_.cend(); post_rk++) {
-            host_tmp.push_back(std::vector<VT>(flat_data.begin()+this->row_begin_[*post_rk], flat_data.begin()+this->row_begin_[*post_rk+1]));
-        }
-        return host_tmp;
+        return this->get_matrix_variable_all(flat_data);
+    }
+
+    /**
+     *  @brief      computes the size in bytes
+     *  @details    contains also the required size of LILMatrix partition but not account allocated variables.
+     *  @returns    size in bytes for stored connectivity
+     *  @see        LILMatrix::size_in_bytes()
+     */
+    size_t size_in_bytes() {
+        size_t size = 2 * sizeof(IT);               // scalar values
+
+        size += static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->size_in_bytes();
+
+        return size;
     }
-};
+};
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRCMatrixT.hpp` & `ANNarchy-4.7.3/ANNarchy/include/CSRCMatrixT.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     // intended as pre-synaptic view
     std::vector<ST> row_ptr_;       ///< i-th element marks the begin of the i-th row
     std::vector<IT> col_idx_;       ///< contains the column indices in row major order order. To access row i, get indices from row_begin_.
 
     // intended as post-synaptic view
     std::vector<ST> col_ptr_;       ///<
     std::vector<IT> row_idx_;
-    std::vector<IT> inv_idx_;
+    std::vector<ST> inv_idx_;
 
     IT num_rows_;
     IT num_columns_;
     ST num_non_zeros_;
 
     /**
      *
@@ -99,14 +99,17 @@
         for (auto i = 0; i < col_ptr_.size() - 1; i++) {
             ST row_len = col_ptr_[i+1] - col_ptr_[i];
             if (row_len > 0)
                 post_ranks.push_back(i);
         }
 
         post_ranks_ = std::move(post_ranks);
+
+        // remove unneccessary allocated space
+        col_idx_.shrink_to_fit();
     }
 
  public:
     explicit CSRCMatrixT(const IT num_rows, const IT num_columns):
         num_rows_(num_rows), num_columns_(num_columns) {
     #ifdef _DEBUG
         std::cout << "CSRCMatrixT::CSRCMatrixT() with dense dimensions " << this->num_rows_ << " times " << this->num_columns_ << std::endl;
@@ -127,14 +130,26 @@
         return row_ptr_.data();
     }
 
     inline IT* col_idx() {
         return col_idx_.data();
     }
 
+    inline ST* col_ptr() {
+        return col_ptr_.data();
+    }
+
+    inline IT* row_idx() {
+        return row_idx_.data();
+    }
+
+    inline IT* inverse_indices() {
+        return inv_idx_.data();
+    }
+
     /*
      *  Create CSRC_T from LIL while ensuring an ascending index in rows. This function is called from Python.
      */
     bool init_matrix_from_lil(std::vector<IT> post_ranks, std::vector< std::vector<IT> > pre_ranks) {
     #ifdef _DEBUG
         std::cout << "CSRCMatrixT::init_matrix_from_lil()" << std::endl;
     #endif
@@ -288,14 +303,17 @@
             col_idx_.insert(col_idx_.end(), tmp_transposed_lil[r].begin(), tmp_transposed_lil[r].end());
             num_non_zeros_ += tmp_transposed_lil[r].size();
         }
         row_ptr_[num_columns_] = num_non_zeros_;
 
         // Create backward view (post-synaptic rank as rows)
         inverse_connectivity_matrix();
+
+        // remove unneccessary allocated space
+        col_idx_.shrink_to_fit();
     }
 
     void fixed_probability_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
         clear();
 
         // Generate post_to_pre LIL
         auto lil_mat = new LILMatrix<IT, ST>(num_rows_, num_columns_);
@@ -354,14 +372,19 @@
                 inv_idx_.insert(inv_idx_.end(), inv_idx[i].begin(), inv_idx[i].end());
 
                 curr_off += static_cast<ST>(inv_post_rank[i].size());
             }
         }
         col_ptr_[this->num_rows_] = curr_off;
 
+        // remove unneccessary allocated space
+        row_idx_.shrink_to_fit();
+        inv_idx_.shrink_to_fit();
+
+        // sanity check
         if ( num_non_zeros_ != curr_off ) {
             std::cerr << "Something went wrong:" << std::endl;
             std::cerr << " - fwd dimensions: " << row_ptr_.size() << std::endl;
             std::cerr << " - bwd dimensions: " << col_ptr_.size() << std::endl;
             std::cerr << " - nb_synapes = " << num_non_zeros_ << " ( differs from curr_off = " << curr_off << ")" << std::endl;
         }
     #ifdef _DEBUG_CONN
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/CSRMatrix.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -171,18 +171,21 @@
 
         // sanity check after transformation
         if (lil_row_idx != row_indices.size())
             std::cerr << "something went wrong ..." << std::endl;
         if (num_non_zeros_ != col_idx_.size())
             std::cerr << "something went wrong ... " << num_non_zeros_ << std::endl;
 
-    #ifdef _DEBUG
-        std::cout << "init completed" << std::endl;
-        std::cout << "  #nnz: " << num_non_zeros_ << std::endl;
-        std::cout << "  #empty rows: " << num_rows_ - post_ranks_.size() << std::endl;
+        // remove unneccessary allocated space
+        col_idx_.shrink_to_fit();
+
+    #if defined(_DEBUG_CONN)
+        print_data_representation(2, true);
+    #elif defined(_DEBUG)
+        print_data_representation(2, false);
     #endif
         return true;
     }
 
     /**
      *  @brief      reads in a .csv file which contains the matrix stored as COO.
      *  @see        LILMatrix::init_matrix_from_lil()
@@ -251,14 +254,18 @@
                 post_ranks_.push_back(row);
                 lil_values.push_back(std::move(tmp_values[row]));
             }
         }
         row_begin_[row_begin_.size()-1]=col_idx_.size();
         num_non_zeros_ = col_idx_.size();
 
+        // remove unneccessary allocated space
+        col_idx_.shrink_to_fit();
+        post_ranks_.shrink_to_fit();
+
         // Sanity check
         assert( (num_non_zeros_ == coo_pairs) );
 
     #ifdef _DEBUG
         std::cout << "Extracted " << coo_pairs << " from " << filename << std::endl;
     #endif
 
@@ -293,14 +300,17 @@
             std::sort(tmp_col_indices.begin(), tmp_col_indices.end());
 
             // store in CSR
             col_idx_.insert(col_idx_.end(), tmp_col_indices.begin(), tmp_col_indices.end());
             num_non_zeros_ += nnz_per_row;
         }
         row_begin_[num_rows_] = num_non_zeros_;
+
+        // remove unneccessary allocated space
+        col_idx_.shrink_to_fit();
     }
 
     void fixed_probability_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
     #ifdef _DEBUG
         std::cout << "CSRMatrix::fixed_probability_pattern()" << std::endl;
         std::cout << " rows: " << post_ranks.size() << std::endl;
         std::cout << " p: " << p << std::endl;
@@ -532,32 +542,39 @@
     }
 
     /**
      *  @brief      print the matrix representation to console.
      *  @details    All important fields are printed. Please note, that type casts are
      *              required to print-out the numbers encoded in unsigned char as numbers. 
      */
-    virtual void print_data_representation() {
-        std::cout << "CSRMatrix instance at " << this << std::endl;
-        std::cout << "  #rows: " << static_cast<unsigned long>(num_rows_) << std::endl;
-        std::cout << "  #columns: " << static_cast<unsigned long>(num_columns_) << std::endl;
-        std::cout << "  #nnz: " << num_non_zeros_ << std::endl;
-
-        std::cout << "  post_ranks = [ " << std::endl;
-        for (IT r = 0; r < post_ranks_.size(); r++ ) {
-            std::cout << static_cast<unsigned long>(post_ranks_[r]) << " ";
+    void print_data_representation(int indent_spaces=0, bool print_container=true) {
+        std::cout << std::string(indent_spaces, ' ') << "#rows: " << static_cast<unsigned long>(num_rows_) << std::endl;
+        std::cout << std::string(indent_spaces, ' ') << "#columns: " << static_cast<unsigned long>(num_columns_) << std::endl;
+        std::cout << std::string(indent_spaces, ' ') << "#nnz: " << num_non_zeros_ << std::endl;
+        int empty_rows = 0;
+        for (IT r = 0; r < post_ranks_.size()-1; r++ ) {
+            if (post_ranks_[r+1]-post_ranks_[r] == 0)
+                empty_rows++;
         }
-        std::cout << "]" << std::endl;
+        std::cout << std::string(indent_spaces, ' ') << "#empty rows: " << empty_rows << std::endl;
+        if (print_container) {
+            std::cout << std::string(indent_spaces, ' ') << "CSRMatrix instance at " << this << std::endl;
+            std::cout << std::string(indent_spaces+2, ' ') << "post_ranks = [ ";
+            for (IT r = 0; r < post_ranks_.size(); r++ ) {
+                std::cout << static_cast<unsigned long>(post_ranks_[r]) << " ";
+            }
+            std::cout << "]" << std::endl;
 
-        std::cout << "  row_begin_ = [ " << std::endl;
-        for (auto i = 0; i < row_begin_.size(); i++ ) {
-            std::cout << row_begin_[i] << " ";
-        }
-        std::cout << "]" << std::endl;
+            std::cout << std::string(indent_spaces+2, ' ') << "row_begin_ = [ ";
+            for (auto i = 0; i < row_begin_.size(); i++ ) {
+                std::cout << row_begin_[i] << " ";
+            }
+            std::cout << "]" << std::endl;
 
-        std::cout << "  col_idx_ = [ " << std::endl;
-        for (auto i = 0; i < col_idx_.size(); i++ ) {
-            std::cout << static_cast<unsigned long>(col_idx_[i]) << " ";
+            std::cout << std::string(indent_spaces+2, ' ') << "col_idx_ = [ ";
+            for (auto i = 0; i < col_idx_.size(); i++ ) {
+                std::cout << static_cast<unsigned long>(col_idx_[i]) << " ";
+            }
+            std::cout << "]" << std::endl;
         }
-        std::cout << "]" << std::endl;
     }
 };
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/CSRMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/CSRMatrixCUDA.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -37,17 +37,27 @@
         return required < free;
     }
 
     void free_device_memory() {
     #ifdef _DEBUG
         std::cout << "CSRMatrixCUDA::free_device_memory()" << std::endl;
     #endif
-        cudaFree(gpu_post_rank);
-        cudaFree(gpu_row_ptr);
-        cudaFree(gpu_pre_rank);
+        if (gpu_post_rank) {
+            cudaFree(gpu_post_rank);
+            gpu_post_rank = nullptr;
+        }
+        if (gpu_row_ptr) {
+            cudaFree(gpu_row_ptr);
+            gpu_row_ptr = nullptr;
+        }
+        if (gpu_pre_rank) {
+            cudaFree(gpu_pre_rank);
+            gpu_pre_rank = nullptr;
+        }
+
         auto free_err = cudaGetLastError();
         if (free_err != cudaSuccess) {
             std::cerr << "CSRMatrixCUDA::free_device_memory: " << cudaGetErrorString(free_err) << std::endl;
         }
     }
 
     bool host_to_device() {
@@ -92,14 +102,17 @@
     IT* gpu_post_rank;
     IT* gpu_pre_rank;
 
     CSRMatrixCUDA<IT, ST>(const IT num_rows, const IT num_columns) : CSRMatrix<IT, ST>(num_rows, num_columns) {
     #ifdef _DEBUG
         std::cout << "CSRMatrixCUDA::CSRMatrixCUDA()" << std::endl;
     #endif
+        gpu_row_ptr = nullptr;
+        gpu_post_rank = nullptr;
+        gpu_pre_rank = nullptr;
     }
 
     /**
      *  @brief      Destructor
      *  @details    responsible to delete the allocated GPU memory.
      */
     ~CSRMatrixCUDA() {
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/DenseMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     /**
      *  @brief      check if the matrix fits into RAM
      *  @details    Unlike CUDA it appears that the standard C++ API does not
      *              provide a function to get the available RAM at a present time.
      *              Many sources recommended to use the /proc/meminfo file
      */
     bool check_free_memory(size_t required) {
+    #ifdef __linux__
         FILE *meminfo = fopen("/proc/meminfo", "r");
 
         // TODO:    I'm not completely sure, what we want to do
         //          in this case. Currently, we would hope for the best ...
         if(meminfo == nullptr) {
             std::cerr << "Could not read '/proc/meminfo'. ANNarchy can not catch to large allocations ..." << std::endl;
             return true;
@@ -73,14 +74,18 @@
 
         fclose(meminfo);
         size_t available = static_cast<size_t>(ram) * 1024;
     #ifdef _DEBUG
         std::cout << "DenseMatrix: allocate " << required << " from " << available << " bytes " << std::endl;
     #endif
         return required < available;
+
+    #else
+        return true;
+    #endif
     }
 
     /*
      *  @brief      Decode the column indices for nonzeros in the matrix.
      */
     virtual std::vector<IT> decode_column_indices(IT row_idx) {
     #ifdef _DEBUG
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/ELLMatrixCUDA.hpp`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 /*
- *    DenseMatrixCUDA.hpp
+ *    ELLMatrixCUDA.hpp
  *
  *    This file is part of ANNarchy.
  *
- *    Copyright (C) 2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
- *                        Julien Vitay <julien.vitay@gmail.com>
+ *    Copyright (C) 2020-2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
  *
  *    This program is free software: you can redistribute it and/or modify
  *    it under the terms of the GNU General Public License as published by
  *    the Free Software Foundation, either version 3 of the License, or
  *    (at your option) any later version.
  *
  *    ANNarchy is distributed in the hope that it will be useful,
@@ -17,206 +16,260 @@
  *    GNU General Public License for more details.
  *
  *    You should have received a copy of the GNU General Public License
  *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 #pragma once
 
-#include "DenseMatrix.hpp"
+#include "ELLMatrix.hpp"
 
-/*
- *  @brief              Connectivity representation using a full matrix.
- *  @details            Contrary to all other classes in this template library this matrix format is not a sparse matrix.
- *  @tparam     IT      data type to represent the ranks within the matrix. Generally unsigned data types should be chosen.
- *                      The data type determines the maximum size for the number of elements in a column respectively the number
- *                      of rows encoded in the matrix:
- * 
- *                      - unsigned char (1 byte):        [0 .. 255]
- *                      - unsigned short int (2 byte):   [0 .. 65.535]
- *                      - unsigned int (4 byte):         [0 .. 4.294.967.295]
- *
- *                      The chosen data type should be able to represent the maximum values (LILMatrix::num_rows_ and ::num_columns_)
- * 
- *              ST      the second type should be used if the index type IT could overflow. For instance, the nb_synapses method should return ST as
- *                      the maximum value in case a full dense matrix would be IT times IT entries.
- *              MT      We need to store if a matrix value is set in a bitmask. The size of each entry is determined by MT (we recommend char as its only 1 byte).
+/**
+ *  @brief      An implementation of the ELLPACK format intended for the usage on GPUs.
+ *  @details    This implementation is intended as part of the hybrid ELLPACK/Coordinate
+ *              format. For single use, we intended the usage of the modified
+ *              ELLPACK-R format.
  */
-template<typename IT = unsigned int, typename ST = unsigned long int, typename MT = char, bool row_major = false>
-class DenseMatrixCUDA : public DenseMatrix<IT, ST, MT, row_major> {
+template<typename IT = unsigned int, typename ST = unsigned long int>
+class ELLMatrixCUDA: public ELLMatrix<IT, ST, false> {
 protected:
-    MT* gpu_mask_;
-
     bool check_free_memory(size_t required) {
         size_t free, total;
         cudaMemGetInfo( &free, &total );
     #ifdef _DEBUG
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
         return required < free;
     }
 
     void free_device_memory() {
-    #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::free_device_memory()" << std::endl;
-    #endif
-        cudaFree(gpu_mask_);
-        auto free_err = cudaGetLastError();
-        if (free_err != cudaSuccess) {
-            std::cerr << "DenseMatrixCUDA::free_device_memory: " << cudaGetErrorString(free_err) << std::endl;
+        if (gpu_post_ranks_) {
+            cudaFree(gpu_post_ranks_);
+            gpu_post_ranks_ = nullptr;
+        }
+        if (gpu_col_idx_) {
+            cudaFree(gpu_col_idx_);
+            gpu_col_idx_ = nullptr;
         }
+
+        auto err = cudaGetLastError();
+        if (err != cudaSuccess)
+            std::cerr << "ELLMatrixCUDA::free_device_memory(): " << cudaGetErrorString(err) << std::endl;
     }
 
-    bool host_to_device() {
-    #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::host_to_device()" << std::endl;
-    #endif
-        //
-        //  Allocate device memory
-        cudaMalloc((void**)&gpu_mask_, this->mask_.size()*sizeof(MT));
-        auto malloc_err = cudaGetLastError();
-        if (malloc_err != cudaSuccess) {
-            std::cerr << "CSRMatrixCUDA::init_matrix_from_lil - cudaMalloc: " << cudaGetErrorString(malloc_err) << std::endl;
+    bool host_to_device_transfer() {
+        // Sanity check: can we allocate the data?
+        if (!check_free_memory(sizeof(IT)*this->post_ranks_.size() + sizeof(IT)*this->col_idx_.size()))
             return false;
-        }
 
-        //
-        //  Copy data
-        cudaMemcpy(gpu_mask_, this->mask_.data(), this->mask_.size()*sizeof(MT), cudaMemcpyHostToDevice);
-        auto copy_err = cudaGetLastError();
-        if (copy_err != cudaSuccess) {
-            std::cerr << "CSRMatrixCUDA::init_matrix_from_lil - cudaMemcpy: " << cudaGetErrorString(copy_err) << std::endl;
+        // Allocate the data arrays
+        cudaMalloc((void**)& gpu_post_ranks_, sizeof(IT)*this->post_ranks_.size());
+        cudaMalloc((void**)& gpu_col_idx_, sizeof(IT)*this->col_idx_.size());
+
+        // Copy the data arrays
+        cudaMemcpy(gpu_post_ranks_, this->post_ranks_.data(), sizeof(IT)*this->post_ranks_.size(), cudaMemcpyHostToDevice);
+        cudaMemcpy(gpu_col_idx_, this->col_idx_.data(), sizeof(IT)*this->col_idx_.size(), cudaMemcpyHostToDevice);
+
+        auto err = cudaGetLastError();
+        if (err != cudaSuccess) {
+            std::cerr << "ELLMatrixCUDA::host_to_device_transfer(): " << cudaGetErrorString(err) << std::endl;
             return false;
+        }else{
+            return true;
         }
-
-        return true;
     }
 
 public:
+    IT* gpu_post_ranks_;
+    IT* gpu_col_idx_;
 
-    explicit DenseMatrixCUDA(const IT num_rows, const IT num_columns): DenseMatrix<IT, ST, MT, row_major>(num_rows, num_columns) {
+    /**
+     *  Default constructor
+     */
+    explicit ELLMatrixCUDA<IT, ST>(const IT num_rows, const IT num_columns) : ELLMatrix<IT, ST, false>(num_rows, num_columns) {
     #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::DenseMatrixCUDA()" << std::endl;
+        std::cout << "ELLMatrixCUDA::ELLMatrixCUDA()" << std::endl;
     #endif
+        gpu_post_ranks_ = nullptr;
+        gpu_col_idx_ = nullptr;
     }
 
     /**
-     *  @brief      Destructor
-     *  @details    calls the DenseMatrix::clear method. Is not declared as virtual as inheriting classes in our
-     *              framework should never be destroyed by the base pointer.
+     *  Initialize host side with other ELLPACK-R instance (host side)
      */
-    ~DenseMatrixCUDA() {
+    ELLMatrixCUDA<IT, ST>( ELLMatrix<IT, ST, false>* other ) : ELLMatrix<IT, ST, false>( other ) {
     #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::~DenseMatrixCUDA()" << std::endl;
+        std::cout << "ELLMatrixCUDA::copy constructor"<< std::endl;    
     #endif
-        clear();
+        host_to_device_transfer();
     }
 
-    inline MT* device_mask() {
-        return this->gpu_mask_;
+    /**
+     *  @brief      Destructor
+     */
+    ~ELLMatrixCUDA() {
+    #ifdef _DEBUG
+        std::cout << "ELLMatrixCUDA::~ELLMatrixCUDA()" << std::endl;
+    #endif
     }
 
     /**
-     *  @brief      Clear the dense matrix.
-     *  @details    Clears the connectivity data stored in the *post_rank* and *pre_rank* STL containers and free 
-     *              the allocated memory. **Important**: allocated variables are not effected by this!
+     *  @brief      clear the matrix
+     *  @details    should be called before destructor.
      */
     void clear() {
     #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::clear()" << std::endl;
+        std::cout << "ELLMatrixCUDA::clear()" << std::endl;
     #endif
+        // clear host
+        static_cast<ELLMatrix<IT, ST, false>*>(this)->clear();
+
+        // clear device
+        free_device_memory();
     }
 
-    bool init_matrix_from_lil(std::vector<IT> &row_indices, std::vector< std::vector<IT> > &column_indices) {
+    bool init_matrix_from_lil(std::vector<IT> &post_ranks, std::vector< std::vector<IT> > &pre_ranks) {
+        assert( (post_ranks.size() == pre_ranks.size()) );
+        assert( (post_ranks.size() > 0) );
+
     #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::init_matrix_from_lil() " << std::endl;
+        std::cout << "ELLMatrixCUDA::init_matrix_from_lil()" << std::endl;
     #endif
-        // Initialization on host side
-        bool success = static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->init_matrix_from_lil(row_indices, column_indices);
-        if (!success)
+        // Initialize on host
+        bool success = static_cast<ELLMatrix<IT, ST, false>*>(this)->init_matrix_from_lil(post_ranks, pre_ranks);
+        if(!success)
             return false;
 
+        // Initialize on device and transfer data
+        return host_to_device_transfer();
+    }
+
+    void fixed_number_pre_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, IT nnz_per_row, std::mt19937& rng) {
+    #ifdef _DEBUG
+        std::cout << "ELLMatrixCUDA::fixed_number_pre_pattern()" << std::endl;
+    #endif
+        // Initialization on host side
+        static_cast<ELLMatrix<IT, ST, false>*>(this)->fixed_number_pre_pattern(post_ranks, pre_ranks, nnz_per_row, rng);
+
         // transfer to GPU
-        return host_to_device();
+        host_to_device_transfer();
     }
 
     void fixed_probability_pattern(std::vector<int> post_ranks, std::vector<int> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
     #ifdef _DEBUG
-        std::cout << "CSRMatrixCUDA::fixed_probability_pattern() " << std::endl;
+        std::cout << "ELLMatrixCUDA::fixed_probability_pattern() " << std::endl;
     #endif
         // Initialization on host side
-        static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng);
+        static_cast<ELLMatrix<IT, ST, false>*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng);
 
         // transfer to GPU
-        host_to_device();
+        host_to_device_transfer();
     }
 
     //
-    //  Variables
+    //  Init variables
     //
-    template <typename VT>
+    template<typename VT>
     VT* init_matrix_variable_gpu(const std::vector<VT> &host_variable) {
     #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::init_matrix_variable_gpu()" << std::endl;
+        std::cerr << "ELLMatrixCUDA::init_matrix_variable_gpu()" << std::endl;
     #endif
-        size_t num_dense_elem = this->num_rows_ * this->num_columns_;
-        assert( (num_dense_elem == host_variable.size()) );
+        size_t size_in_bytes = host_variable.size() * sizeof(VT);
+        // sanity check
+        check_free_memory(size_in_bytes);
 
-        VT* gpu_variable;
-        cudaMalloc((void**)&gpu_variable, num_dense_elem*sizeof(VT));
-        cudaMemcpy(gpu_variable, host_variable.data(), num_dense_elem*sizeof(VT), cudaMemcpyHostToDevice);
+        // Allocate
+        VT* new_variable;
+        cudaMalloc((void**)& new_variable, size_in_bytes);
 
+        // Copy
+        cudaMemcpy(new_variable, host_variable.data(), size_in_bytes, cudaMemcpyHostToDevice);
+    #ifdef _DEBUG
         auto err = cudaGetLastError();
-        if (err != cudaSuccess) {
-            std::cerr << "DenseMatrixCUDA::init_matrix_variable_gpu: " << cudaGetErrorString(err) << std::endl;
-        }
-
-        return gpu_variable;
+        if (err != cudaSuccess)
+            std::cerr << "ELLMatrixCUDA::init_matrix_variable_gpu<>(): " << cudaGetErrorString(err) << std::endl;
+    #endif
+        return new_variable;
     }
 
-    template <typename VT>
+    template<typename VT>
     VT* init_vector_variable_gpu(const std::vector<VT> &host_variable) {
-    #ifdef _DEBUG
-        std::cout << "DenseMatrixCUDA::init_vector_variable_gpu()" << std::endl;
-    #endif
-        assert( (this->num_rows_ == host_variable.size()) );
-        size_t size_in_bytes = this->num_rows_ * sizeof(VT);
+        size_t size_in_bytes = host_variable.size() * sizeof(VT);
+        // sanity check
         check_free_memory(size_in_bytes);
 
-        VT* gpu_variable;
-        cudaMalloc((void**)&gpu_variable, size_in_bytes);
-        cudaMemcpy(gpu_variable, host_variable.data(), size_in_bytes, cudaMemcpyHostToDevice);
-
-        auto err = cudaGetLastError();
-        if (err != cudaSuccess) {
-            std::cerr << "DenseMatrixCUDA::init_vector_variable_gpu: " << cudaGetErrorString(err) << std::endl;
-        }
-
-        return gpu_variable;
+        // Allocate
+        VT* new_variable;
+        cudaMalloc((void**)& new_variable, host_variable.size() * sizeof(VT));
+
+        // Copy
+        cudaMemcpy(new_variable, host_variable.data(), host_variable.size() * sizeof(VT), cudaMemcpyHostToDevice);
+        return new_variable;
     }
 
     //
     // Read-out variables from GPU and return as LIL
     //
     template <typename VT>
     std::vector<std::vector<VT>> get_device_matrix_variable_as_lil(VT* gpu_variable) {
-        auto host_tmp = std::vector<std::vector<VT>>();
-
-        auto flat_data = std::vector<VT>(this->num_rows_*this->num_columns_, 0.0);
-        cudaMemcpy(flat_data.data(), gpu_variable, this->num_rows_*this->num_columns_*sizeof(VT), cudaMemcpyDeviceToHost);
-
-        return this->get_matrix_variable_all(flat_data);
+        auto tmp = std::vector<std::vector<VT>>();
+        return tmp;
+    }
+    
+    IT* get_device_col_idx() {
+        return gpu_col_idx_;
     }
 
     /**
      *  @brief      computes the size in bytes
      *  @details    contains also the required size of LILMatrix partition but not account allocated variables.
      *  @returns    size in bytes for stored connectivity
      *  @see        LILMatrix::size_in_bytes()
      */
     size_t size_in_bytes() {
-        size_t size = 2 * sizeof(IT);               // scalar values
+        // standard ELLPACK size
+        size_t size = static_cast<ELLMatrix<IT, ST, false>*>(this)->size_in_bytes();
 
-        size += static_cast<DenseMatrix<IT, ST, MT, row_major>*>(this)->size_in_bytes();
+        // GPU pointer
+        size += 2 * sizeof(IT*);
 
         return size;
     }
-};
+
+    /**
+     *  \brief      overloaded std::ostream operator<<
+     *  \details    for the object itself
+     *  \param[IN]  os      ostream instance
+     *  \param[IN]  matrix  object instance
+     *  \return     manipulated ostream instance
+     */
+     friend std::ostream& operator<< (std::ostream& os, const ELLMatrixCUDA<IT>& matrix) {
+        os << "num_rows_: " << matrix.num_rows_ << std::endl;
+        os << "maxnzr_: " << matrix.maxnzr_ << std::endl;
+        
+        os << "col_idx_:" << std::endl;
+        os << "[ ";
+        for(int s = 0; s < matrix.col_idx_.size(); s++) {
+            os << matrix.col_idx_[s] << " ";
+        }
+        os << "]" << std::endl;
+        os << "values_:" << std::endl;
+        for(int r = 0; r < matrix.num_rows_; r++) {
+            os << "[ ";
+            for(int s = 0; s < matrix.maxnzr_; s++) {
+                os << matrix.values_[s * matrix.num_rows_ + r] << " ";
+            }
+            os << "]" << std::endl;
+        }
+        return os;
+    }
+
+    /**
+     *  \brief      overloaded std::ostream operator<<
+     *  \details    for the reference to an object
+     *  \param[IN]  os      ostream instance
+     *  \param[IN]  matrix  object reference
+     *  \return     manipulated ostream instance
+     */
+    friend std::ostream& operator<< (std::ostream& os, ELLMatrixCUDA<IT>* matrix) {
+        return os << *matrix;
+    }
+};
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/DenseMatrixOffsets.hpp` & `ANNarchy-4.7.3/ANNarchy/include/DenseMatrixOffsets.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/ELLMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/ELLMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     /**
      *  @brief      check if the matrix fits into RAM
      *  @details    Unlike CUDA it appears that the standard C++ API does not
      *              provide a function to get the available RAM at a present time.
      *              Many sources recommended to use the /proc/meminfo file
      */
     bool check_free_memory(size_t required) {
+    #ifdef __linux__
         FILE *meminfo = fopen("/proc/meminfo", "r");
         
         // TODO:    I'm not completely sure, what we want to do
         //          in this case. Currently, we would hope for the best ...
         if(meminfo == nullptr) {
             std::cerr << "Could not read '/proc/meminfo'. ANNarchy can not catch to large allocations ..." << std::endl;
             return true;
@@ -110,14 +111,18 @@
 
         fclose(meminfo);
         size_t available = static_cast<size_t>(ram) * 1024;
     #ifdef _DEBUG
         std::cout << "ELLMatrix: allocate " << required << " from " << available << " bytes " << std::endl;
     #endif
         return required < available;
+
+    #else
+        return true;
+    #endif
     }
 
   public:
     /**
      *  @brief      Constructor
      *  @details    Does not initialize any data.
      *  @param[in]  num_rows        number of rows of the original matrix (this value is only provided to have an unified interface)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/ELLMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/SELLMatrixCUDA.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 /*
- *    ELLMatrixCUDA.hpp
+ *    SELLMatrixCUDA.hpp
  *
  *    This file is part of ANNarchy.
  *
- *    Copyright (C) 2020-2021  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
+ *	  Copyright (C) 2021-22  Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>,
+ *                  2021-22  Qi Tang <kevin2014tq@gmail.com>
  *
  *    This program is free software: you can redistribute it and/or modify
  *    it under the terms of the GNU General Public License as published by
  *    the Free Software Foundation, either version 3 of the License, or
  *    (at your option) any later version.
  *
  *    ANNarchy is distributed in the hope that it will be useful,
@@ -15,253 +16,271 @@
  *    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  *    GNU General Public License for more details.
  *
  *    You should have received a copy of the GNU General Public License
  *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 #pragma once
+#include "SELLMatrix.hpp"
 
-#include "ELLMatrix.hpp"
-
-/**
- *  @brief      An implementation of the ELLPACK format intended for the usage on GPUs.
- *  @details    This implementation is intended as part of the hybrid ELLPACK/Coordinate
- *              format. For single use, we intended the usage of the modified
- *              ELLPACK-R format.
- */
 template<typename IT = unsigned int, typename ST = unsigned long int>
-class ELLMatrixCUDA: public ELLMatrix<IT, ST, false> {
-protected:
+class SELLMatrixCUDA : public SELLMatrix<IT, ST, false> {
+  protected:
     bool check_free_memory(size_t required) {
-        size_t free, total;
-        cudaMemGetInfo( &free, &total );
+          size_t free, total;
+          cudaMemGetInfo(&free, &total);
+
     #ifdef _DEBUG
-        std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
+          std::cout << "Allocate " << required << " and have " << free << "( " << (double(required) / double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
-        return required < free;
+        return (required < free);
     }
 
     void free_device_memory() {
-        cudaFree(gpu_post_ranks_);
-        cudaFree(gpu_col_idx_);
+        if(d_row_ptr) {
+            cudaFree(d_row_ptr);
+            d_row_ptr = nullptr;
+        }
+        if (d_col_idx) {
+            cudaFree(d_col_idx);
+            d_col_idx = nullptr;
+        }
 
         auto err = cudaGetLastError();
         if (err != cudaSuccess)
-            std::cerr << "ELLMatrixCUDA::free_device_memory(): " << cudaGetErrorString(err) << std::endl;
+            std::cerr << "SELLMatrixCUDA::free_device_memory(): " << cudaGetErrorString(err) << std::endl;
     }
 
-    bool host_to_device_transfer() {
+    void host_to_device_transfer() {
+        //compute memory require
+        size_t row_ptr_size = this->row_ptr_.size() * sizeof(ST);
+        size_t col_idx_size = this->col_idx_.size() * sizeof(IT);
+
         // Sanity check: can we allocate the data?
-        if (!check_free_memory(sizeof(IT)*this->post_ranks_.size() + sizeof(IT)*this->col_idx_.size()))
-            return false;
+        check_free_memory(row_ptr_size + col_idx_size);
 
         // Allocate the data arrays
-        cudaMalloc((void**)& gpu_post_ranks_, sizeof(IT)*this->post_ranks_.size());
-        cudaMalloc((void**)& gpu_col_idx_, sizeof(IT)*this->col_idx_.size());
+        cudaMalloc((void**)&d_row_ptr, row_ptr_size);
+        cudaMalloc((void**)&d_col_idx, col_idx_size);
 
         // Copy the data arrays
-        cudaMemcpy(gpu_post_ranks_, this->post_ranks_.data(), sizeof(IT)*this->post_ranks_.size(), cudaMemcpyHostToDevice);
-        cudaMemcpy(gpu_col_idx_, this->col_idx_.data(), sizeof(IT)*this->col_idx_.size(), cudaMemcpyHostToDevice);
+        cudaMemcpy(d_row_ptr, this->row_ptr_.data(), row_ptr_size, cudaMemcpyHostToDevice);
+        cudaMemcpy(d_col_idx, this->col_idx_.data(), col_idx_size, cudaMemcpyHostToDevice);
 
         auto err = cudaGetLastError();
-        if (err != cudaSuccess) {
+        if (err != cudaSuccess)
             std::cerr << "ELLMatrixCUDA::host_to_device_transfer(): " << cudaGetErrorString(err) << std::endl;
-            return false;
-        }else{
-            return true;
-        }
     }
 
-public:
-    IT* gpu_post_ranks_;
-    IT* gpu_col_idx_;
+  public:
+    ST* d_row_ptr;
+    IT* d_col_idx;
+
 
     /**
      *  Default constructor
      */
-    explicit ELLMatrixCUDA<IT, ST>(const IT num_rows, const IT num_columns) : ELLMatrix<IT, ST, false>(num_rows, num_columns) {
+    explicit SELLMatrixCUDA<IT,ST>(const IT num_rows, const IT num_columns, const IT block_size) : SELLMatrix<IT,ST, false>(num_rows, num_columns, block_size) {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::ELLMatrixCUDA()" << std::endl;
+        std::cout << "SELLMatrixCUDA::SELLMatrixCUDA()" << std::endl;
     #endif
+        d_row_ptr = nullptr;
+        d_col_idx = nullptr;
     }
 
     /**
-     *  Initialize host side with other ELLPACK-R instance (host side)
+     *  Initialize host side with other sliced ELLPACK instance (host side)
      */
-    ELLMatrixCUDA<IT, ST>( ELLMatrix<IT, ST, false>* other ) : ELLMatrix<IT, ST, false>( other ) {
+    /*SELLMatrixCUDA<IT,ST>(SELLMatrix<IT, ST, false>* other) : SELLMatrix<IT,ST, false>(other) {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::copy constructor"<< std::endl;    
+            std::cout << "SELLMatrixCUDA::copy constructor" << std::endl;
     #endif
         host_to_device_transfer();
-    }
+    }*/
 
     /**
      *  @brief      Destructor
      */
-    ~ELLMatrixCUDA() {
+    ~SELLMatrixCUDA() {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::~ELLMatrixCUDA()" << std::endl;
+        std::cout << "SELLMatrixCUDA::~SELLMatrixCUDA()" << std::endl;
     #endif
     }
 
     /**
      *  @brief      clear the matrix
      *  @details    should be called before destructor.
      */
     void clear() {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::clear()" << std::endl;
+            std::cout << "SELLMatrixCUDA::clear()" << std::endl;
     #endif
         // clear host
-        static_cast<ELLMatrix<IT, ST, false>*>(this)->clear();
+        static_cast<SELLMatrix<IT, ST, false>*>(this)->clear();
 
         // clear device
         free_device_memory();
     }
 
-    bool init_matrix_from_lil(std::vector<IT> &post_ranks, std::vector< std::vector<IT> > &pre_ranks) {
-        assert( (post_ranks.size() == pre_ranks.size()) );
-        assert( (post_ranks.size() > 0) );
+
+    /*
+    *   init matrix from lil format  
+    */
+    bool init_matrix_from_lil(std::vector<IT>& post_ranks, std::vector< std::vector<IT> >& pre_ranks) {
+        assert((post_ranks.size() == pre_ranks.size()));
+        assert((post_ranks.size() > 0));
 
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::init_matrix_from_lil()" << std::endl;
+            std::cout << "SELLMatrixCUDA::init_matrix_from_lil()" << std::endl;
     #endif
-        // Initialize on host
-        bool success = static_cast<ELLMatrix<IT, ST, false>*>(this)->init_matrix_from_lil(post_ranks, pre_ranks);
-        if(!success)
-            return false;
+        static_cast<SELLMatrix<IT, ST, false>*>(this)->init_matrix_from_lil(post_ranks, pre_ranks);
 
-        // Initialize on device and transfer data
-        return host_to_device_transfer();
+        host_to_device_transfer();
+
+        return true;
     }
 
-    void fixed_number_pre_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, IT nnz_per_row, std::mt19937& rng) {
+    bool fixed_number_pre_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, IT nnz_per_row, std::mt19937& rng) {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::fixed_number_pre_pattern()" << std::endl;
+            std::cout << "SELLMatrixCUDA::fixed_number_pre_pattern()" << std::endl;
     #endif
         // Initialization on host side
-        static_cast<ELLMatrix<IT, ST, false>*>(this)->fixed_number_pre_pattern(post_ranks, pre_ranks, nnz_per_row, rng);
+        static_cast<SELLMatrix<IT, ST, false>*>(this)->fixed_number_pre_pattern(post_ranks, pre_ranks, nnz_per_row, rng);
 
         // transfer to GPU
         host_to_device_transfer();
+
+        return true;
     }
 
+    /*
     void fixed_probability_pattern(std::vector<int> post_ranks, std::vector<int> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
     #ifdef _DEBUG
-        std::cout << "ELLMatrixCUDA::fixed_probability_pattern() " << std::endl;
+            std::cout << "SELLMatrixCUDA::fixed_probability_pattern() " << std::endl;
     #endif
         // Initialization on host side
-        static_cast<ELLMatrix<IT, ST, false>*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng);
+        static_cast<SELLMatrix<IT, false>*>(this)->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng);
 
         // transfer to GPU
         host_to_device_transfer();
-    }
+    }  */
+
 
     //
     //  Init variables
     //
     template<typename VT>
-    VT* init_matrix_variable_gpu(const std::vector<VT> &host_variable) {
+    VT* init_matrix_variable_gpu(const std::vector<VT>& host_variable) {
     #ifdef _DEBUG
-        std::cerr << "ELLMatrixCUDA::init_matrix_variable_gpu()" << std::endl;
+            std::cerr << "SELLMatrixCUDA::init_matrix_variable_gpu()" << std::endl;
     #endif
         size_t size_in_bytes = host_variable.size() * sizeof(VT);
         // sanity check
-        check_free_memory(size_in_bytes);
+        if (!check_free_memory(size_in_bytes))
+            return nullptr;
 
         // Allocate
         VT* new_variable;
-        cudaMalloc((void**)& new_variable, size_in_bytes);
+        cudaMalloc((void**)&new_variable, size_in_bytes);
+    #ifdef _DEBUG
+        auto malloc_err = cudaGetLastError();
+        if (malloc_err != cudaSuccess)
+            std::cerr << "SELLMatrixCUDA::init_matrix_variable_gpu<>() - allocate: " << cudaGetErrorString(malloc_err) << std::endl;
+    #endif
 
         // Copy
         cudaMemcpy(new_variable, host_variable.data(), size_in_bytes, cudaMemcpyHostToDevice);
+
     #ifdef _DEBUG
-        auto err = cudaGetLastError();
-        if (err != cudaSuccess)
-            std::cerr << "ELLMatrixCUDA::init_matrix_variable_gpu<>(): " << cudaGetErrorString(err) << std::endl;
+        auto memcpy_err = cudaGetLastError();
+        if (memcpy_err != cudaSuccess)
+            std::cerr << "SELLMatrixCUDA::init_matrix_variable_gpu<>() - memcpy: " << cudaGetErrorString(memcpy_err) << std::endl;
     #endif
         return new_variable;
     }
 
+    // Init vector variable
     template<typename VT>
-    VT* init_vector_variable_gpu(const std::vector<VT> &host_variable) {
+    VT* init_vector_variable_gpu(const std::vector<VT>& host_variable) {
         size_t size_in_bytes = host_variable.size() * sizeof(VT);
         // sanity check
         check_free_memory(size_in_bytes);
 
         // Allocate
         VT* new_variable;
-        cudaMalloc((void**)& new_variable, host_variable.size() * sizeof(VT));
+        cudaMalloc((void**)&new_variable, host_variable.size() * sizeof(VT));
 
         // Copy
         cudaMemcpy(new_variable, host_variable.data(), host_variable.size() * sizeof(VT), cudaMemcpyHostToDevice);
         return new_variable;
     }
 
     //
     // Read-out variables from GPU and return as LIL
     //
-    template <typename VT>
+    /*template <typename VT>
     std::vector<std::vector<VT>> get_device_matrix_variable_as_lil(VT* gpu_variable) {
         auto tmp = std::vector<std::vector<VT>>();
         return tmp;
-    }
-    
-    IT* get_device_col_idx() {
-        return gpu_col_idx_;
-    }
+    }*/
 
-    /**
-     *  @brief      computes the size in bytes
-     *  @details    contains also the required size of LILMatrix partition but not account allocated variables.
-     *  @returns    size in bytes for stored connectivity
-     *  @see        LILMatrix::size_in_bytes()
-     */
-    size_t size_in_bytes() {
-        // standard ELLPACK size
-        size_t size = static_cast<ELLMatrix<IT, ST, false>*>(this)->size_in_bytes();
+    template<typename VT>
+    void get_vector_variable_from_gpu(std::vector<VT>& host_variable, VT* d_variable) {
+        size_t size_in_bytes = host_variable.size() * sizeof(VT);
 
-        // GPU pointer
-        size += 2 * sizeof(IT*);
+        // Copy
+        cudaMemcpy(host_variable.data(), d_variable, size_in_bytes, cudaMemcpyDeviceToHost);
+    }
 
-        return size;
+    IT* get_device_col_idx() {
+        return d_col_idx;
     }
 
     /**
      *  \brief      overloaded std::ostream operator<<
      *  \details    for the object itself
      *  \param[IN]  os      ostream instance
      *  \param[IN]  matrix  object instance
      *  \return     manipulated ostream instance
      */
-     friend std::ostream& operator<< (std::ostream& os, const ELLMatrixCUDA<IT>& matrix) {
+    friend std::ostream& operator<< (std::ostream& os, const SELLMatrixCUDA<IT>& matrix) {
         os << "num_rows_: " << matrix.num_rows_ << std::endl;
-        os << "maxnzr_: " << matrix.maxnzr_ << std::endl;
-        
+        os << "blocksize_: " << matrix.blocksize_ << std::endl;
+        os << "num_blocks_: " << matrix.num_blocks_ << std::endl;
+        os << "num_non_zeros_: " << matrix.num_non_zeros_ << std::endl;
+
         os << "col_idx_:" << std::endl;
         os << "[ ";
-        for(int s = 0; s < matrix.col_idx_.size(); s++) {
+        for (int s = 0; s < matrix.col_idx_.size(); s++) {
             os << matrix.col_idx_[s] << " ";
         }
         os << "]" << std::endl;
-        os << "values_:" << std::endl;
-        for(int r = 0; r < matrix.num_rows_; r++) {
-            os << "[ ";
-            for(int s = 0; s < matrix.maxnzr_; s++) {
-                os << matrix.values_[s * matrix.num_rows_ + r] << " ";
-            }
-            os << "]" << std::endl;
+
+        os << "post_ranks_:" << std::endl;
+        os << "[ ";
+        for (int s = 0; s < matrix.post_ranks_.size(); s++) {
+            os << matrix.post_ranks_[s] << " ";
+        }
+        os << "]" << std::endl;
+
+        os << "rowptr_:" << std::endl;
+        os << "[ ";
+        for (int s = 0; s < matrix.rowptr_.size(); s++) {
+            os << matrix.rowptr_[s] << " ";
         }
+        os << "]" << std::endl;
+
         return os;
     }
 
     /**
      *  \brief      overloaded std::ostream operator<<
      *  \details    for the reference to an object
      *  \param[IN]  os      ostream instance
      *  \param[IN]  matrix  object reference
      *  \return     manipulated ostream instance
      */
-    friend std::ostream& operator<< (std::ostream& os, ELLMatrixCUDA<IT>* matrix) {
+    friend std::ostream& operator<< (std::ostream& os, SELLMatrixCUDA<IT>* matrix) {
         return os << *matrix;
     }
-};
+
+};
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/ELLRMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/ELLRMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     /**
      *  @brief      check if the matrix fits into RAM
      *  @details    Unlike CUDA it appears that the standard C++ API does not
      *              provide a function to get the available RAM at a present time.
      *              Many sources recommended to use the /proc/meminfo file
      */
     bool check_free_memory(size_t required) {
+    #ifdef __linux__
         FILE *meminfo = fopen("/proc/meminfo", "r");
         
         // TODO:    I'm not completely sure, what we want to do
         //          in this case. Currently, we would hope for the best ...
         if(meminfo == nullptr) {
             std::cerr << "Could not read '/proc/meminfo'. ANNarchy can not catch to large allocations ..." << std::endl;
             return true;
@@ -107,14 +108,18 @@
 
         fclose(meminfo);
         size_t available = static_cast<size_t>(ram) * 1024;
     #ifdef _DEBUG
         std::cout << "ELLRMatrix: allocate " << required << " from " << available << " bytes " << std::endl;
     #endif
         return required < available;
+
+    #else
+        return true;
+    #endif
     }
 
 public:
     /**
      *  \brief      Constructor
      *  \details    Does not initialize any data.
      *  \param[in]  num_rows        number of rows of the original matrix (this value is only provided to have an unified interface)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/ELLRMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/ELLRMatrixCUDA.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,26 @@
     #ifdef _DEBUG
         std::cout << "Allocate " << required << " and have " << free << "( " << (double(required)/double(total)) * 100.0 << " percent of total memory)" << std::endl;
     #endif
         return required < free;
     }
 
     void free_device_memory() {
-        cudaFree(gpu_post_ranks_);
-        cudaFree(gpu_col_idx_);
-        cudaFree(gpu_rl_);
+        if (gpu_post_ranks_) {
+            cudaFree(gpu_post_ranks_);
+            gpu_post_ranks_ = nullptr;
+        }
+        if (gpu_col_idx_) {
+            cudaFree(gpu_col_idx_);
+            gpu_col_idx_ = nullptr;
+        }
+        if (gpu_rl_) {
+            cudaFree(gpu_rl_);
+            gpu_rl_ = nullptr;
+        }
 
         auto err = cudaGetLastError();
         if (err != cudaSuccess)
             std::cerr << "ELLRMatrixCUDA::free_device_memory(): " << cudaGetErrorString(err) << std::endl;
     }
 
     bool host_to_device_transfer() {
@@ -91,14 +100,17 @@
     /**
      *  Default constructor
      */
     explicit ELLRMatrixCUDA<IT, ST>(const IT num_rows, const IT num_columns) : ELLRMatrix<IT, ST, false>(num_rows, num_columns) {
     #ifdef _DEBUG
         std::cout << "ELLRMatrixCUDA::ELLRMatrixCUDA()" << std::endl;
     #endif
+        gpu_post_ranks_ = nullptr;
+        gpu_col_idx_ = nullptr;
+        gpu_rl_ = nullptr;
     }
 
     /**
      *  Initialize host side with other ELLPACK-R instance (host side)
      */
     ELLRMatrixCUDA<IT, ST>( ELLRMatrix<IT, ST, false>* other ) : ELLRMatrix<IT, ST, false>( other ) {
     #ifdef _DEBUG
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/HYBMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/HYBMatrix.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/HYBMatrixCUDA.hpp` & `ANNarchy-4.7.3/ANNarchy/include/HYBMatrixCUDA.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/LILInvMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/LILInvMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -29,39 +29,39 @@
  *              indexing from the column side. The backward view allows a column-based indexing of the connectivity matrix.
  *              But be aware, that there is a higher spreading of memory access. As the LILMatrix is inherited and ANNarchy
  *              user-interface is row-oriented, this class does not contain any get/set or initialize methods for the variables.
  *              The connector methods should call the LILMatrix counter parts and LILInvMatrix::inverse_connectivity_matrix()
  *              afterwards.
  *
  *              Let's consider the following example matrix
- * 
+ *
  *                      | 0 1 0 |
  *                  A = | 2 0 3 |
  *                      | 0 0 0 |
  *                      | 0 0 4 |
- * 
+ *
  *              has the LIL representation
- * 
+ *
  *                  post_rank = [ 0 1 3 ]
  *
  *                  pre_rank = [ [ 1 ], [ 0, 2  ], [ 2 ] ]
- * 
+ *
  *              The backward view would consists of std::map<> with the keys 0, 1, 2 as all columns contain at least one value. The attached vectors
  *              will contain the row indices:
- * 
+ *
  *                  inv_pre_rank = [
  *                      0: [1],
  *                      1: [0],
  *                      2: [1, 3]
  *                  ]
- * 
+ *
  *              The inv_post_rank will then contain the dense column indices additionally:
- * 
+ *
  *                  inv_post_rank = [0, 1, 2]
- * 
+ *
  *  @tparam     IT      data type to represent the ranks within the matrix. Please refer to LILMatrix for more details.
  *              ST      the second type should be used if the index type IT could overflow. Please refer to LILMatrix for more details.
  *
  */
 template<typename IT = unsigned int, typename ST = unsigned long int>
 class LILInvMatrix: public LILMatrix<IT, ST> {
 public:
@@ -87,28 +87,35 @@
         }
 
         // store the dense column indices, please note that std::map has sorted indices
         inv_post_rank = std::vector< IT >();
         for (auto it = inv_pre_rank.begin(); it != inv_pre_rank.end(); it++) {
             inv_post_rank.push_back(it->first);
         }
+
+        // remove unneccessary allocated bytes (caused by push_back)
+        for (auto it = inv_pre_rank.begin(); it != inv_pre_rank.end(); it++) {
+            // idx pairs are stored in avector
+            it->second.shrink_to_fit();
+        }
+        inv_post_rank.shrink_to_fit();
     }
 
 public:
     /**
-     *  @brief      Constructor 
+     *  @brief      Constructor
      */
     explicit LILInvMatrix(const IT num_rows, const IT num_columns)  : LILMatrix<IT, ST>(num_rows, num_columns) {
     #ifdef _DEBUG
         std::cout << "Created LIL-type matrix with backward view " << this << " using dense dimension " << static_cast<long>(this->num_rows_) << "x" << static_cast<long>(this->num_columns_) << std::endl;
     #endif
     }
 
     /**
-     *  @brief      Destructor 
+     *  @brief      Destructor
      */
     ~LILInvMatrix() {
     #ifdef _DEBUG
         std::cout << "LILInvMatrix::~LILInvMatrix()" << std::endl;
     #endif
     }
 
@@ -246,8 +253,8 @@
         for ( auto it = inv_pre_rank.begin(); it != inv_pre_rank.end(); it++ ) {
             size += sizeof(IT); // key
             size += (it->second).capacity() * sizeof(IT); // value
         }
 
         return size;
     }
-};
+};
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/LILMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/LILMatrix.hpp`

 * *Files 4% similar despite different names*

```diff
@@ -22,85 +22,85 @@
  *
  */
 #pragma once
 
 /**
  *  @brief      Implementation of the *list-in-list* (LIL) sparse matrix format.
  *  @details    The LIL format comprises of a nested vector *pre_rank*, where the top-level indicates a row and the sub-level vector
- *              the column indices. To consider the existance of empty-rows, we have an additional array *post_rank* who assigns the 
+ *              the column indices. To consider the existance of empty-rows, we have an additional array *post_rank* who assigns the
  *              row index to the entry in the *pre_rank* structure.
- * 
+ *
  *              Let's consider the following example matrix
- * 
+ *
  *                      | 0 1 0 |
  *                  A = | 2 0 3 |
  *                      | 0 0 0 |
  *                      | 0 0 4 |
- * 
+ *
  *              As all rows, except the second, contain at least one entry the *post_rank* array would be:
- * 
+ *
  *                  post_rank = [ 0 1 3 ]
  *
  *              The *pre_rank* array contains in each sub vector the column indices:
  *
  *                  pre_rank = [ [ 1 ], [ 0, 2  ], [ 2 ] ]
- * 
+ *
  *              Please note, that contrary to some SpMV implementations in all ANNarchy versions the values of the matrix are stored in
  *              a seperate LIL structure which follows the same scheme:
- * 
+ *
  *                  w = [ [ 1 ], [ 2, 3 ], [ 4 ] ]
- * 
+ *
  *              The background is simply the fact that we have often multiple variables and one want to store only one time pre- and post-synaptic ranks.
  *              Such a variable is initialized with the init_matrix_variable<> methods. A second special case is that some operations require only a row
- *              vector of size (*num_rows_*) these variables are initialized with a seperate init_row_variable<> methods. 
+ *              vector of size (*num_rows_*) these variables are initialized with a seperate init_row_variable<> methods.
  *
  *              The Python interface of ANNarchy can access the connectivity data through the following functions:
- * 
+ *
  *              - LILMatrix<IT>::get_post_rank()
  *              - LILMatrix<IT>::get_pre_ranks()
  *              - LILMatrix<IT>::get_dendrite_pre_rank()
  *              - LILMatrix<IT>::nb_synapses()
  *              - LILMatrix<IT>::nb_dendrites()
- * 
- *              The template class is also responsible for the init/get/update of variables marked as *semiglobal* and *local*. A *local* variable can be 
+ *
+ *              The template class is also responsible for the init/get/update of variables marked as *semiglobal* and *local*. A *local* variable can be
  *              filled with either constant or randomly drawn values, please note the specialized functions for more details:
- * 
+ *
  *              - LILMatrix<IT>::init_matrix_variable() for a (at maximum) num_rows_ by num_column_ matrix with a constant value
  *              - LILMatrix<IT>::init_matrix_variable_uniform() for a (at maximum) num_rows_ by num_column_ matrix with a constant value
  *              - LILMatrix<IT>::init_matrix_variable_normal() for a (at maximum) num_rows_ by num_column_ matrix with a constant value
  *
  *              The *local* variables can be updated by single values, a row or the complete variable. Please note, that a *lil_idx* is required for two of
  *              these functions which could be obtained by usage of the LILMatrix::post_rank array.
  *
  *              - LILMatrix<IT>::update_matrix_variable()
  *              - LILMatrix<IT>::update_matrix_variable_row()
  *              - LILMatrix<IT>::update_matrix_variable_all()
- * 
+ *
  *              The same applies for the read-out of the allocated variable containers:
- * 
+ *
  *              - LILMatrix<IT>::get_matrix_variable()
  *              - LILMatrix<IT>::get_matrix_variable_row()
  *              - LILMatrix<IT>::get_matrix_variable_all()
- * 
+ *
  *              All these methods are also available as vector_variable methods which are responsible for the *semiglobal* variables. Contrary to local variables
  *              those are stored in 1D-vectors of the same size as LILMatrix::post_rank.
- * 
+ *
  *              **Implementation notice**: this functions might appear as obsolete, as they only return the provided containers back, but they are part of a common
  *              interface for single-thread and multi-thread interface (this again eases the code generation).
- * 
+ *
  *  @tparam     IT      data type to represent the ranks within the matrix. Generally unsigned data types should be chosen.
  *                      The data type determines the maximum size for the number of elements in a column respectively the number
  *                      of rows encoded in the matrix:
- * 
+ *
  *                      - unsigned char (1 byte):        [0 .. 255]
  *                      - unsigned short int (2 byte):   [0 .. 65.535]
  *                      - unsigned int (4 byte):         [0 .. 4.294.967.295]
  *
  *                      The chosen data type should be able to represent the maximum values (LILMatrix::num_rows_ and ::num_columns_)
- * 
+ *
  *              ST      the second type should be used if the index type IT could overflow. For instance, the nb_synapses method should return ST as
  *                      the maximum value in case a full dense matrix would be IT times IT entries.
  */
 template<typename IT = unsigned int, typename ST = unsigned long int>
 class LILMatrix {
 public:
     const IT num_rows_;                     ///< maximum number of rows which equals the maximum length of post_rank as well as maximum size of top-level of pre_rank.
@@ -134,15 +134,15 @@
     #ifdef _DEBUG
         std::cout << "LILMatrix::~LILMatrix()" << std::endl;
     #endif
     }
 
     /**
      *  @brief      Clear the sparse matrix representation.
-     *  @details    Clears the connectivity data stored in the *post_rank* and *pre_rank* STL containers and free 
+     *  @details    Clears the connectivity data stored in the *post_rank* and *pre_rank* STL containers and free
      *              the allocated memory. **Important**: allocated variables are not effected by this!
      */
     void clear() {
     #ifdef _DEBUG
         std::cout << "LILMatrix::clear()" << std::endl;
     #endif
         post_rank.clear();
@@ -215,19 +215,19 @@
     bool init_matrix_from_lil(std::vector<IT> &post_ranks, std::vector< std::vector<IT> > &pre_ranks) {
     #ifdef _DEBUG
         std::cout << "LILMatrix::init_matrix_from_lil()" << std::endl;
     #endif
         // Sanity checks
         assert ( (post_ranks.size() == pre_ranks.size()) );
         assert ( (post_ranks.size() <= num_rows_) );
-        
+
         // store the data
         this->post_rank = post_ranks;
         this->pre_rank = pre_ranks;
-    
+
     #ifdef _DEBUG
         print_matrix_statistics();
     #endif
         return true;
     }
 
     /**
@@ -286,15 +286,15 @@
         }
 
         // create a LIL from the read data
         auto lil_ranks = std::vector<IT>();
         auto lil_col_idx = std::vector<std::vector<IT>>();
         auto lil_values = std::vector<std::vector<VT>>();
         for(auto row = 0; row < num_rows_; row++) {
-            
+
             if (tmp_col_idx[row].size() > 0) {
                 lil_ranks.push_back(row);
                 lil_col_idx.push_back(std::move(tmp_col_idx[row]));
                 lil_values.push_back(std::move(tmp_values[row]));
             }
         }
 
@@ -305,15 +305,49 @@
         auto value = init_matrix_variable<VT>(0.0);
         update_matrix_variable_all<VT>(value, lil_values);
 
         return value;
     }
 
     /**
-     *  @brief      initialize connectivity using a fixed_number_pre pattern 
+     *  @brief      initialize connectivity using an all-to-all pattern.
+     *  @details    For more details on this pattern see the ANNarchy Documentation.
+     *  @param[in]  post_ranks              list of row indices of all rows which contain at least on elements to be accounted.
+     *  @param[in]  pre_ranks               list of list, where the i-th sub-vector should contain a list of potential
+     *                                      connection candidates for the i-th post-synaptic neuron.
+     *  @param[in]  allow_self_connections  whether neurons with the same rank should be connected or not.
+     */
+    bool all_to_all_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, bool allow_self_connections) {
+    #ifdef _DEBUG
+        std::cout << "LILMatrix::all_to_all_pattern()" << std::endl;
+        std::cout << " #rows: " << post_ranks.size() << std::endl;
+        std::cout << " #columns: " << pre_ranks.size() << std::endl;
+        std::cout << " self-connections: " << allow_self_connections << std::endl;
+    #endif
+        post_rank = post_ranks;
+
+        if (allow_self_connections) {
+            // copy N times the pre-rank vector
+            pre_rank = std::vector< std::vector<IT> >(post_rank.size(), pre_ranks);
+
+        } else {
+            pre_rank = std::vector< std::vector<IT> >(post_rank.size(), std::vector<IT>());
+
+            // need to remove the i-th column index for row i
+            for (IT i = 0; i < post_ranks.size(); i++) {
+                pre_rank[i].insert(pre_rank[i].begin(), pre_ranks.begin(), pre_ranks.begin()+i);
+                pre_rank[i].insert(pre_rank[i].begin()+i, pre_ranks.begin()+i+1, pre_ranks.end());
+            }
+        }
+
+        return true;
+    }
+
+    /**
+     *  @brief      initialize connectivity using a fixed_number_pre pattern
      *  @details    For more details on this pattern see the ANNarchy Documentation.
      *  @param[in]  post_ranks  list of row indices of all rows which contain at least on elements to be accounted.
      *  @param[in]  pre_ranks   list of list, where the i-th sub-vector should contain a list of potential connection candidates for the i-th post-synaptic neuron.
      *  @param[in]  nnz_per_row number of pre-synaptic neurons which should be randomly selected from the list.
      *  @param[in]  rng         a merseanne twister generator (need to be seeded in prior if necessary)
      */
     bool fixed_number_pre_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, IT nnz_per_row, std::mt19937& rng) {
@@ -328,25 +362,25 @@
         // for each row we select a subset of the provided pre ranks
         for(auto lil_idx = 0; lil_idx < post_ranks.size(); lil_idx++) {
             // shuffle indices (source vector is modified!)
             std::shuffle(pre_ranks.begin(), pre_ranks.end(), rng);
 
             // select nnz_per_row elements
             auto tmp_col_indices = std::vector<IT>(pre_ranks.begin(), pre_ranks.begin()+nnz_per_row);
-            
+
             // sort the indices before storage
             std::sort(tmp_col_indices.begin(), tmp_col_indices.end());
             pre_rank[lil_idx] = std::move(tmp_col_indices);
         }
 
         return true;
     }
 
     /**
-     *  @brief      initialize connectivity using a fixed_probability pattern 
+     *  @brief      initialize connectivity using a fixed_probability pattern
      *  @details    For more details on this pattern see the ANNarchy Documentation.
      *  @param[in]  post_ranks  list of row indices of all rows which contain at least on elements to be accounted.
      *  @param[in]  pre_ranks   list of list, where the i-th sub-vector should contain a list of potential connection candidates for the i-th post-synaptic neuron.
      *  @param[in]  p           probability for a connection being set between two neurons.
      *  @param[in]  rng         a merseanne twister generator (need to be seeded in prior if necessary)
      */
     bool fixed_probability_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, double p, bool allow_self_connections, std::mt19937& rng) {
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/PartitionedMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/PartitionedMatrix.hpp`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
  *
  *    You should have received a copy of the GNU General Public License
  *    along with this program.  If not, see <http://www.gnu.org/licenses/>.
  */
 #pragma once
 
 /**
- *  @brief      Wrapper class for handling multiple instances of LIL.
+ *  @brief      Wrapper class for handling multiple instances of SPARSE_MATRIX_TYPE.
  *  @details    In order to support the parallel evaluation of expecially spiking networks
  *              we divide the whole matrix into as many as threads parts.
  *  @tparam     SPARSE_MATRIX_TYPE  sparse matrix class, most likely a LILMatrix, LILInvMatrix or CSRCMatrix
  *  @tparam     IT                  index type which should be the same as used in the SPARSE_MATRIX_TYPE declaration
  *  @tparam     ST                  size type which should be the same as used in the SPARSE_MATRIX_TYPE declaration
  */
 template<typename SPARSE_MATRIX_TYPE, typename IT = unsigned int, typename ST = unsigned long int>
 class PartitionedMatrix {
 protected:
-    const IT num_rows_;
-    const IT num_columns_;
-    IT num_partitions_;            ///< stores the number of threads used for allocation. Should not change during runtime, or the data structure needs to be reinited.
-    IT chunk_size_;             ///< number of rows computed by each thread
+    const IT num_rows_;     ///< number of rows in the original matrix
+    const IT num_columns_;  ///< number of columns in the original matrix
+    IT num_partitions_;     ///< stores the number of threads used for allocation. Should not change during runtime, or the data structure needs to be reinited.
+    IT chunk_size_;         ///< number of rows computed by each thread
 
     /**
      *  @brief      Divide the matrix across rows in equally large partitions.
      *  @details    Sets the chunk_size_ as well as the slices_ attribute.
      */
     void divide_post_ranks(std::vector<IT> &row_indices, int num_partitions) {
         clear();
@@ -52,15 +52,15 @@
             int end = std::min(static_cast<int>((i+1) * chunk_size_), static_cast<int>(num_rows_));
 
             sub_matrices_.push_back(new SPARSE_MATRIX_TYPE(num_rows_, num_columns_));
         }
 
         // ATTENTION: this assumes that row_indices are sorted ascending
         int lower_bound = 0;
-        for(int part_idx = 0; part_idx < num_partitions_; part_idx++) {
+        for (int part_idx = 0; part_idx < num_partitions_; part_idx++) {
             int part_border = (part_idx+1) * chunk_size_;
 
             auto it = std::partition(row_indices.begin(), row_indices.end(), [&part_border](int i){return i < part_border;});
             int size = std::distance(row_indices.begin(), it);
 
             slices_.push_back(std::pair<int,int>(lower_bound, size));
             lower_bound = size;
@@ -74,38 +74,42 @@
     explicit PartitionedMatrix(const unsigned int num_rows, const unsigned int num_columns) :
         num_rows_(num_rows), num_columns_(num_columns) {
     }
 
     ~PartitionedMatrix() {
     }
 
+    int chunk_size() {
+        return this->chunk_size_;
+    }
+
     void clear() {
         // delete old stuff
         for(auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++)
             delete *it;
         sub_matrices_.clear();
         slices_.clear();
     }
 
     //
     //  Connectivity accessors ( for Cython )
     //
-    std::vector<IT> get_post_rank() { 
+    std::vector<IT> get_post_rank() {
         auto complete_post_ranks = std::vector<IT>();
 
         for (auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++) {
             auto post_rank_slice = (*it)->get_post_rank();
             complete_post_ranks.insert(complete_post_ranks.end(), post_rank_slice.begin(), post_rank_slice.end());
         }
 
         return complete_post_ranks;
     }
 
-    std::vector<std::vector<IT>> get_pre_ranks() { 
-        auto complete_pre_ranks = std::vector<std::vector<IT>>(); 
+    std::vector<std::vector<IT>> get_pre_ranks() {
+        auto complete_pre_ranks = std::vector<std::vector<IT>>();
 
         for (auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++) {
             auto tmp = (*it)->get_pre_ranks();
 
             complete_pre_ranks.insert(complete_pre_ranks.end(), tmp.begin(), tmp.end());
         }
 
@@ -163,41 +167,42 @@
         }
         return efferents;
     }
 
     bool init_matrix_from_lil(std::vector<IT> &post_ranks, std::vector< std::vector<IT> > &pre_ranks, const IT num_partitions) {
         assert ( (post_ranks.size() == pre_ranks.size()) );
     #ifdef _DEBUG
-        std::cout << "ParallelLIL::init_matrix_from_lil():" << std::endl;
+        std::cout << "PartitionedMatrix::init_matrix_from_lil():" << std::endl;
     #endif
         // determine partitions
         divide_post_ranks(post_ranks, num_partitions);
 
-    #ifdef _DEBUG
-        std::cout << "partitions per thread:" << std::endl;
-        for (int t = 0; t < num_partitions; t++) {
-            std::cout << "tid = " << t << ": " << std::distance(post_ranks.begin(), post_ranks.begin()+slices_[t].first) <<
-            " to " << std::distance(post_ranks.begin(), post_ranks.begin()+slices_[t].second) << 
-            " ( " << slices_[t].second - slices_[t].first << " items )" << std::endl;
-        }
-    #endif
         auto slice_it = slices_.begin();
         int part_idx = 0;
         for(; slice_it != slices_.end(); slice_it++, part_idx++) {
             // create sub matrix with the previously determined slices
             auto post_rank_slice = std::vector<IT>(post_ranks.begin()+slice_it->first, post_ranks.begin()+slice_it->second);
             auto pre_rank_slice = std::vector< std::vector<IT> >(pre_ranks.begin()+slice_it->first, pre_ranks.begin()+slice_it->second);
 
             bool success = sub_matrices_[part_idx]->init_matrix_from_lil(post_rank_slice, pre_rank_slice);
             if (!success) {
                 std::cerr << "Failed to initialize partition " << part_idx << std::endl;
                 return false;
             }
         }
 
+    #ifdef _DEBUG
+        std::cout << "PartitionedMatrix: created " << num_partitions << " partitions with partition borders:" << std::endl;
+        for (int t = 0; t < num_partitions; t++) {
+            std::cout << "  partition " << t << ": " << std::distance(post_ranks.begin(), post_ranks.begin()+slices_[t].first) <<
+            " to " << std::distance(post_ranks.begin(), post_ranks.begin()+slices_[t].second) << 
+            " ( " << slices_[t].second - slices_[t].first << " rows, "<< sub_matrices_[t]->nb_synapses() <<" nnz )" << std::endl;
+        }
+    #endif
+
         return true;
     }
 
     /**
      *  @brief      reads in a .csv file which contains the matrix stored as COO.
      *  @details    this function creates also the variable array, which is usually performed afterwards.
      *  @tparam     VT          value type of the nonzero
@@ -252,15 +257,15 @@
         }
 
         // create a LIL from the read data
         auto lil_ranks = std::vector<IT>();
         auto lil_col_idx = std::vector<std::vector<IT>>();
         auto lil_values = std::vector<std::vector<VT>>();
         for(auto row = 0; row < num_rows_; row++) {
-            
+
             if (tmp_col_idx[row].size() > 0) {
                 lil_ranks.push_back(row);
                 lil_col_idx.push_back(std::move(tmp_col_idx[row]));
                 lil_values.push_back(std::move(tmp_values[row]));
             }
         }
 
@@ -296,48 +301,61 @@
         // Create the matrix as in single thread
         auto lil_mat = new SPARSE_MATRIX_TYPE(num_rows_, num_columns_);
         lil_mat->fixed_number_pre_pattern(post_ranks, pre_ranks, nnz_per_row, rng[0]);
 
         // distribute towards threads
         auto slice_it = slices_.begin();
         int part_idx = 0;
-        for(; slice_it != slices_.end(); slice_it++, part_idx++) {        
+        for(; slice_it != slices_.end(); slice_it++, part_idx++) {
             auto sliced_lil = lil_mat->slice_across_rows(slice_it->first, slice_it->second);
             sub_matrices_[part_idx]->init_matrix_from_lil(sliced_lil->post_rank, sliced_lil->pre_rank);
         }
     #endif
     }
 
     void fixed_probability_pattern(std::vector<IT> post_ranks, std::vector<IT> pre_ranks, double p, bool allow_self_connections, std::vector<std::mt19937>& rng, const unsigned int num_partitions) {
     #ifdef _DEBUG
         std::cout << "ParallelLIL::fixed_probability_pattern():" << std::endl;
     #endif
         // determine partitions
         divide_post_ranks(post_ranks, num_partitions);
 
-        auto it = slices_.begin();
-        int part_idx = 0;
-        for(; it != slices_.end(); it++, part_idx++) {
-            // create sub matrix with the previously determined slices
-            auto post_rank_slice = std::vector<IT>(post_ranks.begin()+it->first, post_ranks.begin()+it->second);
+    #if !defined(_DISABLE_PARALLEL_RNG) and defined(_OPENMP)
+        #pragma omp parallel num_threads(num_partitions)
+        {
+            int tid = omp_get_thread_num();
+            auto slice = slices_[tid];
+            auto post_rank_slice = std::vector<IT>(post_ranks.begin()+slice.first, post_ranks.begin()+slice.second);
+            sub_matrices_[tid]->fixed_probability_pattern(post_rank_slice , pre_ranks, p, allow_self_connections, rng[tid]);
+        }
+    #else
+        // Create the matrix as in single thread
+        auto single_matrix = new SPARSE_MATRIX_TYPE(num_rows_, num_columns_);
+        single_matrix->fixed_probability_pattern(post_ranks, pre_ranks, p, allow_self_connections, rng[0]);
 
-            sub_matrices_[part_idx]->fixed_probability_pattern(post_rank_slice , pre_ranks, p, allow_self_connections, rng[0]);
+        // distribute towards threads
+        auto slice_it = slices_.begin();
+        int part_idx = 0;
+        for (; slice_it != slices_.end(); slice_it++, part_idx++) {
+            auto sliced_lil = single_matrix->slice_across_rows(slice_it->first, slice_it->second);
+            sub_matrices_[part_idx]->init_matrix_from_lil(sliced_lil->post_rank, sliced_lil->pre_rank);
         }
+    #endif
     }
 
     //
     //  Initialize matrix variables ( post-size times pre-size divided into num_partitions chunks)
     //
     /**
      *  @brief      Initialize a matrix variable
      *  @tparam     PART_TYPE   as the slice type depends on the format, e. g. LIL vector<vector<VT>> and CSRC vector<VT>
      *                          but I wanted to have an unified interface, the PART_TYPE provides the necessary information.
      */
     template <typename VT, typename PART_TYPE>
-    std::vector< PART_TYPE > init_matrix_variable(VT default_value) {    
+    std::vector< PART_TYPE > init_matrix_variable(VT default_value) {
         auto new_variable = std::vector< PART_TYPE >();
         for(auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++) {
             new_variable.push_back((*it)->init_matrix_variable(default_value));
         }
 
         return new_variable;
     }
@@ -358,15 +376,15 @@
         return new_variable;
     #else
         auto new_variable = std::vector< PART_TYPE >();
         for(auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++) {
             new_variable.push_back(std::move((*it)->init_matrix_variable_uniform(a, b, rng[0])));
         }
         return new_variable;
-    #endif        
+    #endif
     }
 
     template <typename VT, typename PART_TYPE>
     std::vector< PART_TYPE > init_matrix_variable_normal(VT mean, VT sigma, std::vector<std::mt19937>& rng) {
     #ifdef _DEBUG
         std::cout << "Initialize variable with Normal(" << mean << ", " << sigma << ")" << std::endl;
     #endif
@@ -381,15 +399,15 @@
         return new_variable;
     #else
         auto new_variable = std::vector< PART_TYPE >();
         for(auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++) {
             new_variable.push_back(std::move((*it)->init_matrix_variable_normal(mean, sigma, rng[0])));
         }
         return new_variable;
-    #endif        
+    #endif
     }
 
     //
     //  Update matrix variables
     //
     template <typename VT, typename PART_TYPE>
     inline void update_matrix_variable(std::vector< PART_TYPE > &variable, const IT lil_idx, const IT col_idx, const VT value)
@@ -563,22 +581,23 @@
         for (auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++)
             (*it)->print_data_representation();
   
     }
 
     // Returns size in bytes for connectivity
     size_t size_in_bytes() {
-        size_t size = 4 * sizeof(unsigned int);
+        // constants
+        size_t size = 4 * sizeof(IT);
 
         // partitions
         size += sizeof(std::vector<SPARSE_MATRIX_TYPE*>);
         size += sub_matrices_.capacity() * sizeof(SPARSE_MATRIX_TYPE*);
         for (auto it = sub_matrices_.begin(); it != sub_matrices_.end(); it++)
             size += static_cast<SPARSE_MATRIX_TYPE*>(*it)->size_in_bytes();
 
         // ranges
         size += sizeof(std::vector<std::pair<IT, IT>>);
         size += slices_.capacity() * sizeof(std::pair<IT, IT>);
 
         return size;
     };
-};
+};
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/SELLMatrix.hpp` & `ANNarchy-4.7.3/ANNarchy/include/SELLMatrix.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,19 @@
             mask_.insert(mask_.end(), temp_block_mask.begin(), temp_block_mask.end());
             temp_block_col.clear();
             temp_block_mask.clear();
         }
 
         row_ptr_.push_back(col_idx_.size());
 
+        // remove unneccessary allocated space
+        row_ptr_.shrink_to_fit();
+        col_idx_.shrink_to_fit();
+        mask_.shrink_to_fit();
+
         // sanity check
         if (lil_row_idx != row_indices.size()) {
             std::cerr << "SELLMatrix::init_matrix_from_lil() something went wrong ..." << std::endl;
             return false;
         }
 
         // sanity check (did we allocate enough dense blocks?)
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/Specific.hpp` & `ANNarchy-4.7.3/ANNarchy/include/Specific.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/include/helper_functions.hpp` & `ANNarchy-4.7.3/ANNarchy/include/helper_functions.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/models/Neurons.py` & `ANNarchy-4.7.3/ANNarchy/models/Neurons.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Neurons.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Neuron import Neuron
 
 def list_standard_neurons():
     "Returns a list of standard neuron models available."
     return [
         LeakyIntegrator, 
         Izhikevich,
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/models/Synapses.py` & `ANNarchy-4.7.3/ANNarchy/models/Synapses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Synapses.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Synapse import Synapse
 from ANNarchy.core.Global import _error
 
 
 def list_standard_synapses():
     "Returns a list of standard neuron models available."
     return [STP, STDP, Hebb, Oja, IBCM]
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/AnalyseNeuron.py` & `ANNarchy-4.7.3/ANNarchy/parser/AnalyseNeuron.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     AnalyseNeuron.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Global import _error, _warning, config
 from ANNarchy.core.Random import available_distributions, distributions_arguments, distributions_equivalents
 from ANNarchy.parser.Equation import Equation
 from ANNarchy.parser.StringManipulation import *
 from ANNarchy.parser.ITE import *
 from ANNarchy.parser.Extraction import *
 from ANNarchy.parser.CoupledEquations import CoupledEquations
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/AnalyseSynapse.py` & `ANNarchy-4.7.3/ANNarchy/parser/AnalyseSynapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     AnalyseSynapse.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from ANNarchy.core.Global import _error, _warning, config
 from ANNarchy.core.Random import available_distributions, distributions_arguments, distributions_equivalents
 from ANNarchy.parser.Equation import Equation
 from ANNarchy.parser.StringManipulation import *
 from ANNarchy.parser.ITE import *
 from ANNarchy.parser.Extraction import *
 from ANNarchy.parser.CoupledEquations import CoupledEquations
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/CoupledEquations.py` & `ANNarchy-4.7.3/ANNarchy/parser/CoupledEquations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     CoupledEquations.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 from .Equation import Equation
 from .ParserTemplate import create_local_dict, user_functions
 
 from sympy import *
 
 import re
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/Equation.py` & `ANNarchy-4.7.3/ANNarchy/parser/Equation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Equation.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 from .ParserTemplate import create_local_dict, user_functions
 
 import sympy as sp
 import re
 from copy import deepcopy
 
@@ -174,20 +156,30 @@
             user_functions=self.user_functions
         )
 
         if Global.config["precision"]=="float":
             #
             # Add the f-suffix to floating value constants
             matches = re.findall(r"[-]?[0-9]+\.[0-9]+", c_code)
-            matches = list(set(matches))    # remove doublons, e. g. 0.5*dt
+            matches = sorted(list(set(matches)))    # remove doublons, e. g. 0.5*dt
+
             for m in matches:
                 fval = float(m)
                 fval = round(fval, 8)       # shorten the val to a reasonable length
                 c_code = c_code.replace(m, str(fval)+"f")
 
+            # If found constants have an overlap, e.g., 5.0 and 15.0, we create
+            # multiple suffixes, e.g., 15.0ff. Therefore, we need to remove them
+            # afterwards ...
+            matches = re.findall(r"[-]?[0-9]+\.[0-9]+f[f]+", c_code)
+            for m in matches:
+                fval = float(m.split("f")[0])
+                fval = round(fval, 8)       # shorten the val to a reasonable length
+                c_code = c_code.replace(m, str(fval)+"f")
+
             # Replace the math functions with their single precision
             # to circumenvent problems induced by implicit type conversion
             # e. g. pow(double, double) by powf(float, float)
             for func in ["fabs", "pow", "exp", "sin", "cos", "tan"]:
                 c_code = c_code.replace(func+"(", func+"f(")
 
         return c_code
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/Extraction.py` & `ANNarchy-4.7.3/ANNarchy/parser/Extraction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,12 @@
-#===============================================================================
-#
-#     Extraction.py
-#
-#     This file is part of ANNarchy.
-#
-#     Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-#     Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-#
-#     This program is free software: you can redistribute it and/or modify
-#     it under the terms of the GNU General Public License as published by
-#     the Free Software Foundation, either version 3 of the License, or
-#     (at your option) any later version.
-#
-#     ANNarchy is distributed in the hope that it will be useful,
-#     but WITHOUT ANY WARRANTY; without even the implied warranty of
-#     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-#     GNU General Public License for more details.
-#
-#     You should have received a copy of the GNU General Public License
-#     along with this program.  If not, see <http://www.gnu.org/licenses/>.
-#
-#===============================================================================
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 import ANNarchy.core.Global as Global
 from ANNarchy.core.Random import available_distributions, distributions_arguments, distributions_equivalents
 from ANNarchy.parser.Equation import Equation
 from ANNarchy.parser.Function import FunctionParser
 from ANNarchy.parser.StringManipulation import *
 from ANNarchy.parser.ITE import *
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/Function.py` & `ANNarchy-4.7.3/ANNarchy/parser/Function.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 """
-
-    Function.py
-
-    This file is part of ANNarchy.
-
-    Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    ANNarchy is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
 """
+
 import ANNarchy.core.Global as Global
 from ANNarchy.parser.Equation import transform_condition
 from .ParserTemplate import parser_dict, functions_dict, user_functions
 
 import sympy as sp
 from sympy.parsing.sympy_parser import parse_expr, standard_transformations, convert_xor, auto_number
 import re
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/ITE.py` & `ANNarchy-4.7.3/ANNarchy/parser/ITE.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 """
-
-    ITE.py
-
-    This file is part of ANNarchy.
-
-    Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    ANNarchy is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
 """
+
 from ANNarchy.core.Global import _error, _print
 from ANNarchy.parser.Equation import Equation
 from ANNarchy.parser.Function import FunctionParser
 from ANNarchy.parser.StringManipulation import *
 
 
 def translate_ITE(name, eq, condition, description, untouched, function=False):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/ParserTemplate.py` & `ANNarchy-4.7.3/ANNarchy/parser/ParserTemplate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+"""
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
+"""
+
 from sympy import Symbol, Function
 import ANNarchy.core.Global as Global
 
 # Dictionary of default elements for the C++ generation
 parser_dict = {
     'dt' : Symbol('dt'),
     't' : Symbol('(double(t)*dt)'),
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/StringManipulation.py` & `ANNarchy-4.7.3/ANNarchy/parser/StringManipulation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,12 @@
 """
-
-    StringManipulation.py
-
-    This file is part of ANNarchy.
-
-    Copyright (C) 2013-2016  Julien Vitay <julien.vitay@gmail.com>,
-    Helge Uelo Dinkelbach <helge.dinkelbach@gmail.com>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    ANNarchy is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
+:copyright: Copyright 2013 - now, see AUTHORS.
+:license: GPLv2, see LICENSE for details.
 """
+
 ####################################
 # Functions for string manipulation
 ####################################
 import re
 from ANNarchy.core.Global import _error, _warning, _print, authorized_keywords
 
 def split_equation(definition):
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/report/LatexParser.py` & `ANNarchy-4.7.3/ANNarchy/parser/report/LatexParser.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/report/LatexReport.py` & `ANNarchy-4.7.3/ANNarchy/parser/report/LatexReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,16 @@
         parameters = ""
         for idx, param in enumerate(pop.parameters):
             val = pop.init[param]
             if isinstance(val, (list, np.ndarray)):
                 val = "$[" + str(np.array(val).min()) + ", " + str(np.array(val).max()) + "]$"
             parameters += pop_tpl % {'name': LatexParser.pop_name(pop.name) if idx==0 else "", 'param': LatexParser._latexify_name(param, []), 'value': val}
 
-        txt += popparameters_template % {'parameters': parameters, 'firstpopulation': "\hdr{3}{H}{Population parameters}\\\\ \\hline" if rk==0 else ""}
+        if parameters != "":
+            txt += popparameters_template % {'parameters': parameters, 'firstpopulation': "\hdr{3}{H}{Population parameters}\\\\ \\hline" if rk==0 else ""}
 
     return txt
 
 def _generate_projections(net_id, gather_subprojections):
     txt = ""
     proj_tpl = """
     %(pre)s & %(post)s & %(target)s & %(synapse)s &
```

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/report/MarkdownReport.py` & `ANNarchy-4.7.3/ANNarchy/parser/report/MarkdownReport.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/parser/report/Report.py` & `ANNarchy-4.7.3/ANNarchy/parser/report/Report.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy/thirdparty/randutils.hpp` & `ANNarchy-4.7.3/ANNarchy/thirdparty/randutils.hpp`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/ANNarchy.egg-info/SOURCES.txt` & `ANNarchy-4.7.3/ANNarchy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+AUTHORS
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 ANNarchy/__init__.py
 ANNarchy.egg-info/PKG-INFO
 ANNarchy.egg-info/SOURCES.txt
 ANNarchy.egg-info/dependency_links.txt
-ANNarchy.egg-info/not-zip-safe
 ANNarchy.egg-info/requires.txt
 ANNarchy.egg-info/top_level.txt
 ANNarchy/core/ConnectorMethods.py
 ANNarchy/core/Dendrite.py
 ANNarchy/core/Global.py
 ANNarchy/core/IO.py
 ANNarchy/core/Monitor.py
@@ -36,14 +37,15 @@
 ANNarchy/core/cython_ext/Coordinates.pyx
 ANNarchy/core/cython_ext/Transformations.pyx
 ANNarchy/core/cython_ext/__init__.pxd
 ANNarchy/core/cython_ext/__init__.py
 ANNarchy/extensions/__init__.py
 ANNarchy/extensions/ann_to_snn_conversion/ANNtoSNNConverter.py
 ANNarchy/extensions/ann_to_snn_conversion/InputEncoding.py
+ANNarchy/extensions/ann_to_snn_conversion/ReadOut.py
 ANNarchy/extensions/ann_to_snn_conversion/__init__.py
 ANNarchy/extensions/bold/AccProjection.py
 ANNarchy/extensions/bold/BoldModel.py
 ANNarchy/extensions/bold/BoldMonitor.py
 ANNarchy/extensions/bold/NormProjection.py
 ANNarchy/extensions/bold/PredefinedModels.py
 ANNarchy/extensions/bold/__init__.py
@@ -60,16 +62,15 @@
 ANNarchy/extensions/diagonal/__init__.py
 ANNarchy/extensions/hybrid/HybridPopulation.py
 ANNarchy/extensions/hybrid/__init__.py
 ANNarchy/extensions/image/ImagePopulation.py
 ANNarchy/extensions/image/__init__.py
 ANNarchy/extensions/tensorboard/Logger.py
 ANNarchy/extensions/tensorboard/__init__.py
-ANNarchy/extensions/weightsharing/SharedProjection.py
-ANNarchy/extensions/weightsharing/__init__.py
+ANNarchy/generator/CmdLineArgParser.py
 ANNarchy/generator/CodeGenerator.py
 ANNarchy/generator/Compiler.py
 ANNarchy/generator/MonitorGenerator.py
 ANNarchy/generator/PyxGenerator.py
 ANNarchy/generator/Sanity.py
 ANNarchy/generator/Utils.py
 ANNarchy/generator/__init__.py
@@ -138,14 +139,15 @@
 ANNarchy/generator/Projection/SingleThread/__init__.py
 ANNarchy/generator/Template/BaseTemplate.py
 ANNarchy/generator/Template/GlobalOperationTemplate.py
 ANNarchy/generator/Template/MakefileTemplate.py
 ANNarchy/generator/Template/MonitorTemplate.py
 ANNarchy/generator/Template/PyxTemplate.py
 ANNarchy/generator/Template/__init__.py
+ANNarchy/include/BSRInvMatrix.hpp
 ANNarchy/include/BSRMatrix.hpp
 ANNarchy/include/BSRMatrixCUDA.hpp
 ANNarchy/include/COOMatrix.hpp
 ANNarchy/include/COOMatrixCUDA.hpp
 ANNarchy/include/CSRCMatrix.hpp
 ANNarchy/include/CSRCMatrixCUDA.hpp
 ANNarchy/include/CSRCMatrixCUDAT.hpp
@@ -163,14 +165,15 @@
 ANNarchy/include/HYBMatrixCUDA.hpp
 ANNarchy/include/LILInvMatrix.hpp
 ANNarchy/include/LILMatrix.hpp
 ANNarchy/include/PartitionedMatrix.hpp
 ANNarchy/include/SELLMatrix.hpp
 ANNarchy/include/SELLMatrixCUDA.hpp
 ANNarchy/include/Specific.hpp
+ANNarchy/include/VecTransformation.hpp
 ANNarchy/include/helper_functions.hpp
 ANNarchy/models/Neurons.py
 ANNarchy/models/Synapses.py
 ANNarchy/models/__init__.py
 ANNarchy/parser/AnalyseNeuron.py
 ANNarchy/parser/AnalyseSynapse.py
 ANNarchy/parser/CoupledEquations.py
@@ -183,15 +186,15 @@
 ANNarchy/parser/__init__.py
 ANNarchy/parser/report/LatexParser.py
 ANNarchy/parser/report/LatexReport.py
 ANNarchy/parser/report/MarkdownReport.py
 ANNarchy/parser/report/Report.py
 ANNarchy/parser/report/__init__.py
 ANNarchy/thirdparty/randutils.hpp
-examples/ann_to_snn/demo.py
+examples/ann_to_snn/ANNtoSNN.py
 examples/bar_learning/BarLearning.py
 examples/bar_learning/BarLearningGPU.py
 examples/bar_learning/Viz.py
 examples/bold_monitor/BOLD.py
 examples/bold_monitor/BOLD_two_inputs.py
 examples/gap_junctions/GapJunctions.py
 examples/hodgkin_huxley/HodgkinHuxley.py
```

### Comparing `ANNarchy-4.7.2.6/LICENSE` & `ANNarchy-4.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/README.md` & `ANNarchy-4.7.3/README.md`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/bar_learning/BarLearning.py` & `ANNarchy-4.7.3/examples/bar_learning/BarLearning.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/bar_learning/BarLearningGPU.py` & `ANNarchy-4.7.3/examples/bar_learning/BarLearningGPU.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/bar_learning/Viz.py` & `ANNarchy-4.7.3/examples/bar_learning/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/bold_monitor/BOLD.py` & `ANNarchy-4.7.3/examples/bold_monitor/BOLD.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/bold_monitor/BOLD_two_inputs.py` & `ANNarchy-4.7.3/examples/bold_monitor/BOLD_two_inputs.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/gap_junctions/GapJunctions.py` & `ANNarchy-4.7.3/examples/gap_junctions/GapJunctions.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/hodgkin_huxley/HodgkinHuxley.py` & `ANNarchy-4.7.3/examples/hodgkin_huxley/HodgkinHuxley.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/homeostatic_stdp/Ramp.py` & `ANNarchy-4.7.3/examples/homeostatic_stdp/Ramp.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,29 +22,29 @@
         d = 8. : population
         tau_ampa = 5. : population
         tau_nmda = 150. : population
         vrev = 0.0 : population
     """ ,
     equations="""
         # Inputs
-        I = g_ampa * (vrev - v) + g_nmda * nmda(v, -80.0, 60.0) * (vrev -v)  
-        # Midpoint scheme      
+        I = g_ampa * (vrev - v) + g_nmda * nmda(v, -80.0, 60.0) * (vrev -v)
+        # Midpoint scheme
         dv/dt = (0.04 * v + 5.0) * v + 140.0 - u + I : init=-65., midpoint
         du/dt = a * (b*v - u) : init=-13., midpoint
         # Izhikevich scheme
         # new_v = v + 0.5*(0.04 * v^2 + 5.0 * v + 140.0 - u + I) : init=-65.
         # v = new_v + 0.5*(0.04 * new_v^2 + 5.0 * new_v + 140.0 - u + I) : init=-65.
         # u += a * (b*v - u) : init=-13.
         # Conductances
         tau_ampa * dg_ampa/dt = -g_ampa : exponential
         tau_nmda * dg_nmda/dt = -g_nmda : exponential
-    """ , 
+    """ ,
     spike = """
         v >= 30.
-    """, 
+    """,
     reset = """
         v = c
         u += d
     """,
     functions = """
         nmda(v, t, s) = ((v-t)/(s))^2 / (1.0 + ((v-t)/(s))^2)
     """
@@ -76,17 +76,17 @@
         tau_minus * dltd/dt = -ltd : exponential
         # Nearest-neighbour
         w += if t_post >= t_pre: ltp else: - ltd : min=0.0, max=w_max
     """,
     pre_spike="""
         g_target += w
         ltp = A_plus
-    """,         
+    """,
     post_spike="""
-        ltd = A_minus 
+        ltd = A_minus
     """
 )
 
 # STDP with homeostatic regulation
 homeo_stdp = Synapse(
     parameters="""
         # STDP
@@ -114,18 +114,18 @@
         # Nearest-neighbour
         stdp = if t_post >= t_pre: ltp else: - ltd 
         w += (alpha * w * (1- R/Rtarget) + beta * stdp ) * K : min=w_min, max=w_max
     """,
     pre_spike="""
         g_target += w
         ltp = A_plus
-    """,         
+    """,
     post_spike="""
-        ltd = A_minus 
-    """ 
+        ltd = A_minus
+    """
 )
 
 # Projection without homeostatic mechanism
 proj1 = Projection(inp, pop1, ['ampa', 'nmda'], synapse=nearest_neighbour_stdp)
 proj1.connect_all_to_all(Uniform(0.01, 0.03))
 
 # Projection with homeostatic mechanism
@@ -163,12 +163,11 @@
 plt.plot(data3[-1, :], 'r-')
 plt.plot(data4[-1, :], 'bx')
 axes = plt.gca()
 axes.set_ylim([0., 0.035])
 plt.xlabel('# neuron')
 plt.ylabel('Weights after 1000s')
 plt.subplot(313)
-plt.imshow(data4.T, aspect='auto', cmap='hot')
+plt.imshow(np.array(data4, dtype='float').T, aspect='auto', cmap='hot')
 plt.xlabel('Time (s)')
 plt.ylabel('# neuron')
 plt.show()
-
```

### Comparing `ANNarchy-4.7.2.6/examples/homeostatic_stdp/SORF.py` & `ANNarchy-4.7.3/examples/homeostatic_stdp/SORF.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # Parameters
 nb_neuron = 4 # Number of exc and inh neurons
 size = (32, 32) # input size
 freq = 1.2 # nb_cycles/half-image
 nb_stim = 40 # Number of grating per epoch
 nb_epochs = 20 # Number of epochs
-max_freq = 28. # Max frequency of the poisson neurons 
+max_freq = 28. # Max frequency of the poisson neurons
 T = 10000. # Period for averaging the firing rate
 
 # Izhikevich Coba neuron with AMPA, NMDA and GABA receptors
 RSNeuron = Neuron(
     parameters = """
         a = 0.02 : population
         b = 0.2 : population
@@ -35,26 +35,26 @@
         vrev_nmda = 0.0 : population
         vrev_gabaa = -70.0 : population
         vrev_gabab = -90.0 : population
     """ ,
     equations="""
         # Inputs
         I = g_ampa * (vrev_ampa - v) + g_nmda * nmda(v, -80.0, 60.0) * (vrev_nmda -v) + g_gabaa * (vrev_gabaa - v) + g_gabab * (vrev_gabab -v)
-        # Midpoint scheme      
+        # Midpoint scheme
         dv/dt = (0.04 * v + 5.0) * v + 140.0 - u + I : init=-65., min=-90., midpoint
         du/dt = a * (b*v - u) : init=-13., midpoint
         # Conductances
         tau_ampa * dg_ampa/dt = -g_ampa : exponential
         tau_nmda * dg_nmda/dt = -g_nmda : exponential
         tau_gabaa * dg_gabaa/dt = -g_gabaa : exponential
         tau_gabab * dg_gabab/dt = -g_gabab : exponential
-    """ , 
+    """ ,
     spike = """
         v >= 30.
-    """, 
+    """,
     reset = """
         v = c
         u += d
         g_ampa = 0.0
         g_nmda = 0.0
         g_gabaa = 0.0
         g_gabab = 0.0
@@ -91,18 +91,18 @@
         # Traces
         tau_plus  * dltp/dt = -ltp : exponential
         tau_minus * dltd/dt = -ltd : exponential
     """,
     pre_spike="""
         g_target += w
         ltp = A_plus
-    """,         
+    """,
     post_spike="""
-        ltd = A_minus 
-    """ 
+        ltd = A_minus
+    """
 )
 
 # Input population
 OnPoiss = PoissonPopulation(size, rates=1.0)
 OffPoiss = PoissonPopulation(size, rates=1.0)
 
 # RS neuron for the input buffers
@@ -213,15 +213,15 @@
 plt.plot(datae[:, 0], label='Exc')
 plt.plot(datai[:, 0], label='Inh')
 plt.title('Mean FR of the Exc and Inh neurons')
 plt.legend()
 
 plt.figure()
 plt.subplot(121)
-plt.imshow(dataw.T, aspect='auto', cmap='hot')
+plt.imshow(np.array(dataw, dtype='float').T, aspect='auto', cmap='hot')
 plt.title('Timecourse of feedforward weights')
 plt.colorbar()
 plt.subplot(122)
-plt.imshow(datal.T, aspect='auto', cmap='hot')
+plt.imshow(np.array(datal, dtype='float').T, aspect='auto', cmap='hot')
 plt.title('Timecourse of inhibitory weights')
 plt.colorbar()
-plt.show()
+plt.show()
```

### Comparing `ANNarchy-4.7.2.6/examples/hybrid/Hybrid.py` & `ANNarchy-4.7.3/examples/hybrid/Hybrid.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/image/Image.py` & `ANNarchy-4.7.3/examples/image/Image.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,89 +1,89 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 # # Image Processing
 
 # This simple example in `examples/image` demonstrates how to load images directly into the firing rates of a population and apply basic linear filters on it.
-# 
+#
 # It relies on the ANNarchy extensions `image` and `convolution` which must be explicitly imported:
 
 from ANNarchy import *
 from ANNarchy.extensions.image import *
 from ANNarchy.extensions.convolution import Convolution, Pooling
 clear()
 
 
 # `ANNarchy.extensions.image` depends on the Python bindings of OpenCV, they must be installed before running the script.
-# 
+#
 # We first create an `ImagePopulation` that will load images:
 
 image = ImagePopulation(geometry=(480, 640, 3))
 
 
 # Its geometry specifies the size of the images that can be loaded, here 640x480 RGB images. Note the geometry must be of the form (height, width, channels), where channels is 1 for grayscale images and 3 for color images.
-# 
-# The next step is to reduce the size of the image, what can be done by using the `Pooling` class of the `convolution` extension. 
-# 
+#
+# The next step is to reduce the size of the image, what can be done by using the `Pooling` class of the `convolution` extension.
+#
 # We define a dummy artificial neuron, whose firing rate `r` will simply be the sum of excitatory connections /ensured to be positive, but this should always be the case). We then create a smaller population `pooled` with this neuron type, and connect it to the `ImagePopulation` using mean-pooling:
 
 # Simple ANN
 LinearNeuron = Neuron(equations="r=sum(exc): min=0.0")
 
 # Subsampling population
 pooled = Population(geometry=(48, 64, 3), neuron = LinearNeuron)
 
 # Mean-pooling projection
 pool_proj = Pooling(pre=image, post=pooled, target='exc', operation='mean')
 pool_proj.connect_pooling()
 
 
 # The `pooled` population reduces the size of the image by a factor ten (defined by the size of the population) by averaging the pixels values over 10x10 regions (`operation` is set to `'mean'`, but one could use `'max'` or `'min'`). The `connect_pooling()` connector creates the "fake" connection pattern (as no weights are involved).
-# 
+#
 # Let's apply now a 3x3 box filter on each channel of the pooled population:
 
 # Smoothing population
 smoothed = Population(geometry=(48, 64, 3), neuron = LinearNeuron)
 
 # Box filter projection
 box_filter = np.ones((3, 3, 1))/9.
 smooth_proj = Convolution(pre=pooled, post=smoothed, target='exc')
 smooth_proj.connect_filter(weights=box_filter)
 
 
 # To perform a convolution operation on the population (or more precisely a cross-correlation), we call the `connect_filter()` connector method of the `Convolution` projection. It requires to define a kernel (`weights`) that will be convolved over the input population. Here we use a simple box filter, but any filter can be used.
-# 
+#
 # As the `pooled` population has three dimensions and we want to smooth the activities per color channel, we need to define a (3, 3, 1) kernel. If we wanted to smooth also over the color channels, we could have used a (3, 3) filter: the resulting population would have the shape (48, 64).
-# 
+#
 # We now apply a bank of three filters, each selective to a particular color (red/green/blue). This filters do not have a spatial extent (1x1 convolution), but sum over the third dimension (the color channels):
 
-# Convolution population    
+# Convolution population
 filtered = Population(geometry=(48, 64, 3), neuron = LinearNeuron)
 
 # Red/Green/Blue filter bank
-filter_bank = np.array([ 
-    [[ [2.0, -1.0, -1.0] ]] , # Red filter 
+filter_bank = np.array([
+    [[ [2.0, -1.0, -1.0] ]] , # Red filter
     [[ [-1.0, 2.0, -1.0] ]] , # Blue filter
     [[ [-1.0, -1.0, 2.0] ]]   # Green filter
 ])
 filter_proj = Convolution(pre=smoothed, post=filtered, target='exc')
 filter_proj.connect_filters(weights=filter_bank)
 
 # Each of the three filter has the shape (1, 1, 3). The result of each convolution would then be (48, 64), but as there are three filters, the output population is (48, 64, 3). The last dimension does not correspond to the number of color channels, but to the number of filters in the bank: if you add a filter, the population will have to be (48, 64, 4).
-# 
+#
 # Banks of filters require to use `connect_filters()` instead of `connect_filter()`.
 
 compile()
 
 # After compilation, we can load an image into the input population:
 
 image.set_image('test.jpg')
 
 # To see the result, we need to simulate for four time steps (4 milliseconds, as `dt=1.0`).
-# 
+#
 # 1. Step 1: The `image` population loads the image.
 # 2. Step 2: The `pooled` population subsamples the image.
 # 3. Step 3: The `smoothed` population filters the pooled image.
 # 4. Step 4: The bank of filters are applied by `filtered`.
 
 simulate(4.0)
```

### Comparing `ANNarchy-4.7.2.6/examples/image/Webcam.ipynb` & `ANNarchy-4.7.3/examples/image/Webcam.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/image/Webcam.py` & `ANNarchy-4.7.3/examples/image/Webcam.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/izhikevich/Izhikevich.py` & `ANNarchy-4.7.3/examples/izhikevich/Izhikevich.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/multinetwork/MultiNetwork.py` & `ANNarchy-4.7.3/examples/multinetwork/MultiNetwork.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/neural_field/BubbleWorld.pyx` & `ANNarchy-4.7.3/examples/neural_field/BubbleWorld.pyx`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/neural_field/NeuralField.py` & `ANNarchy-4.7.3/examples/neural_field/NeuralField.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/neural_field/Viz.py` & `ANNarchy-4.7.3/examples/neural_field/Viz.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/AEIF_cond_exp.py` & `ANNarchy-4.7.3/examples/pyNN/AEIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/EIF_cond_exp.py` & `ANNarchy-4.7.3/examples/pyNN/EIF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/IF_cond_exp.py` & `ANNarchy-4.7.3/examples/pyNN/IF_cond_exp.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/IF_curr_alpha.py` & `ANNarchy-4.7.3/examples/pyNN/IF_curr_alpha.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/non_linear_synapse.py` & `ANNarchy-4.7.3/examples/pyNN/non_linear_synapse.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/pyNN/short_term_plasticity2.py` & `ANNarchy-4.7.3/examples/pyNN/short_term_plasticity2.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/refractoriness/Refractoriness.py` & `ANNarchy-4.7.3/examples/refractoriness/Refractoriness.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/simple_stdp/SimpleSTDPModel.py` & `ANNarchy-4.7.3/examples/simple_stdp/SimpleSTDPModel.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/structural_plasticity/StructuralPlasticity.py` & `ANNarchy-4.7.3/examples/structural_plasticity/StructuralPlasticity.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/tensorboard/BasalGanglia.ipynb` & `ANNarchy-4.7.3/examples/tensorboard/BasalGanglia.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/tensorboard/BayesianOptimization.ipynb` & `ANNarchy-4.7.3/examples/tensorboard/BayesianOptimization.ipynb`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/examples/tsodyks_markram/TsodyksMarkram.py` & `ANNarchy-4.7.3/examples/tsodyks_markram/TsodyksMarkram.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/tests/test_CUDA.py` & `ANNarchy-4.7.3/tests/test_CUDA.py`

 * *Files identical despite different names*

### Comparing `ANNarchy-4.7.2.6/tests/test_openmp.py` & `ANNarchy-4.7.3/tests/test_openmp.py`

 * *Files identical despite different names*

