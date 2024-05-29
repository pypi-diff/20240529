# Comparing `tmp/scs-3.2.4.post1.tar.gz` & `tmp/scs-3.2.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-3.2.4.post1.tar", last modified: Wed Nov 22 11:59:41 2023, max compression
+gzip compressed data, was "scs-3.2.4.post2.tar", last modified: Wed May 29 18:41:03 2024, max compression
```

## Comparing `scs-3.2.4.post1.tar` & `scs-3.2.4.post2.tar`

### file list

```diff
@@ -1,210 +1,211 @@
--rw-r--r--   0        0        0      115 2023-11-22 11:07:49.000000 scs-3.2.4.post1/.bumpversion.cfg
--rw-r--r--   0        0        0     1572 2023-11-22 11:07:49.000000 scs-3.2.4.post1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     6864 2023-11-22 11:07:49.000000 scs-3.2.4.post1/.github/workflows/build.yml
--rw-r--r--   0        0        0      463 2023-11-22 11:07:49.000000 scs-3.2.4.post1/.gitignore
--rw-r--r--   0        0        0       78 2023-11-22 11:07:49.000000 scs-3.2.4.post1/.gitmodules
--rw-r--r--   0        0        0     1075 2023-11-22 11:07:49.000000 scs-3.2.4.post1/LICENSE
--rw-r--r--   0        0        0      355 2023-11-22 11:07:49.000000 scs-3.2.4.post1/MANIFEST.in
--rw-r--r--   0        0        0      567 2023-11-22 11:07:49.000000 scs-3.2.4.post1/README.md
--rwxr-xr-x   0        0        0      144 2023-11-22 11:07:49.000000 scs-3.2.4.post1/distribute.sh
--rw-r--r--   0        0        0    10691 2023-11-22 11:07:49.000000 scs-3.2.4.post1/legacy_setup.py
--rw-r--r--   0        0        0     5296 2023-11-22 11:07:49.000000 scs-3.2.4.post1/meson.build
--rw-r--r--   0        0        0      258 2023-11-22 11:07:49.000000 scs-3.2.4.post1/meson.options
--rw-r--r--   0        0        0   357429 2023-11-22 11:07:49.000000 scs-3.2.4.post1/notebooks/analyze_csv_logs.ipynb
--rw-r--r--   0        0        0   276982 2023-11-22 11:07:49.000000 scs-3.2.4.post1/notebooks/scs_benchmarks.ipynb
--rw-r--r--   0        0        0   217308 2023-11-22 11:07:49.000000 scs-3.2.4.post1/notebooks/scs_qp.ipynb
--rw-r--r--   0        0        0      380 2023-11-22 11:07:49.000000 scs-3.2.4.post1/pyproject.toml
--rw-r--r--   0        0        0     6136 2023-11-22 11:07:49.000000 scs-3.2.4.post1/scs/__init__.py
--rw-r--r--   0        0        0     2598 2023-11-22 11:07:49.000000 scs-3.2.4.post1/scs/scsmodule.h
--rw-r--r--   0        0        0    26835 2023-11-22 11:07:49.000000 scs-3.2.4.post1/scs/scsobject.h
--rw-r--r--   0        0        0     1237 2023-11-22 11:07:49.000000 scs-3.2.4.post1/scs/scspy.c
--rw-r--r--   0        0        0      295 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.bumpversion.cfg
--rw-r--r--   0        0        0      855 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0     1247 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/build.yml
--rw-r--r--   0        0        0     1048 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/build_mkl.yml
--rw-r--r--   0        0        0      453 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/build_openmp.yml
--rw-r--r--   0        0        0      962 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/buildpp.yml
--rw-r--r--   0        0        0     1278 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/cmake.yml
--rw-r--r--   0        0        0     1332 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/cmake_mkl.yml
--rw-r--r--   0        0        0      688 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/cmake_openmp.yml
--rw-r--r--   0        0        0      971 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      773 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/docs.yml
--rw-r--r--   0        0        0      353 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/gpu.yml
--rw-r--r--   0        0        0      568 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.github/workflows/valgrind.yml
--rw-r--r--   0        0        0      488 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/.gitignore
--rw-r--r--   0        0        0     1009 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/CITATION.cff
--rw-r--r--   0        0        0    15786 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/CMakeLists.txt
--rw-r--r--   0        0        0     1110 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/LICENSE.txt
--rw-r--r--   0        0        0     8572 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/Makefile
--rw-r--r--   0        0        0      922 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/README.md
--rw-r--r--   0        0        0     8748 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/cmake/AddInstallRPATHSupport.cmake
--rw-r--r--   0        0        0     2499 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/cmake/AddUninstallTarget.cmake
--rw-r--r--   0        0        0    28861 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/cmake/InstallBasicPackageFiles.cmake
--rw-r--r--   0        0        0      435 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/cmake/scs_types.h.in
--rw-r--r--   0        0        0   114472 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/Doxyfile
--rw-r--r--   0        0        0      736 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/Makefile
--rw-r--r--   0        0        0     1916 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/_static/css/scs_theme.css
--rw-r--r--   0        0        0     1150 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/_static/favicon.ico
--rw-r--r--   0        0        0   180020 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/_static/scs_logo.png
--rw-r--r--   0        0        0   154780 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/_static/scs_logo_transparent.png
--rw-r--r--   0        0        0     9294 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/acceleration.rst
--rw-r--r--   0        0        0     4324 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/equilibration.rst
--rw-r--r--   0        0        0     5932 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/index.rst
--rw-r--r--   0        0        0     1037 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/relaxation.rst
--rw-r--r--   0        0        0     7510 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/scale.rst
--rw-r--r--   0        0        0     1680 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/algorithm/warm_start.rst
--rw-r--r--   0        0        0     3230 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/c.rst
--rw-r--r--   0        0        0     2396 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/compile_flags.rst
--rw-r--r--   0        0        0     7064 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/cones.rst
--rw-r--r--   0        0        0     1326 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/exit_flags.rst
--rw-r--r--   0        0        0     1150 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/index.rst
--rw-r--r--   0        0        0     2868 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/info.rst
--rw-r--r--   0        0        0      302 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/julia.rst
--rw-r--r--   0        0        0     1372 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/matlab.rst
--rw-r--r--   0        0        0      868 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/matrices.rst
--rw-r--r--   0        0        0     3054 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/python.rst
--rw-r--r--   0        0        0     1365 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/r.rst
--rw-r--r--   0        0        0       97 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/ruby.rst
--rw-r--r--   0        0        0     3082 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/api/settings.rst
--rw-r--r--   0        0        0     1636 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/blas_lapack/index.rst
--rw-r--r--   0        0        0     2554 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/citing/index.rst
--rw-r--r--   0        0        0     3051 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/conf.py
--rw-r--r--   0        0        0     1127 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/contributing/index.rst
--rw-r--r--   0        0        0        7 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/.gitignore
--rw-r--r--   0        0        0      526 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/c.rst
--rw-r--r--   0        0        0      405 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/index.rst
--rw-r--r--   0        0        0      967 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/julia.rst
--rw-r--r--   0        0        0      451 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/matlab.rst
--rw-r--r--   0        0        0      342 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/basic_qp.rst
--rw-r--r--   0        0        0     1605 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.py
--rw-r--r--   0        0        0     1444 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.py.out
--rw-r--r--   0        0        0     1342 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.rst
--rw-r--r--   0        0        0     1894 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.py
--rw-r--r--   0        0        0    11938 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.py.out
--rw-r--r--   0        0        0     1767 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.rst
--rw-r--r--   0        0        0     2935 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.py
--rw-r--r--   0        0        0    13637 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.py.out
--rw-r--r--   0        0        0     3211 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.rst
--rw-r--r--   0        0        0     3521 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.py
--rw-r--r--   0        0        0     8375 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.py.out
--rw-r--r--   0        0        0     2082 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.rst
--rw-r--r--   0        0        0      608 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/qp.py
--rw-r--r--   0        0        0     1403 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python/qp.py.out
--rw-r--r--   0        0        0      381 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/python.rst
--rw-r--r--   0        0        0     2620 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/qp.c
--rw-r--r--   0        0        0     1545 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/qp.c.out
--rw-r--r--   0        0        0      540 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/qp.m
--rw-r--r--   0        0        0     1940 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/qp.m.out
--rw-r--r--   0        0        0     1100 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/qp.prob
--rw-r--r--   0        0        0     3275 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/r.rst
--rw-r--r--   0        0        0       90 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/examples/ruby.rst
--rw-r--r--   0        0        0    21926 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/files/windows1.png
--rw-r--r--   0        0        0    81416 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/files/windows2.png
--rw-r--r--   0        0        0    17775 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/files/windows3.png
--rw-r--r--   0        0        0      885 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/help/index.rst
--rw-r--r--   0        0        0     3888 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/index.rst
--rw-r--r--   0        0        0     4439 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/c.rst
--rw-r--r--   0        0        0      382 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/index.rst
--rw-r--r--   0        0        0      502 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/julia.rst
--rw-r--r--   0        0        0      452 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/matlab.rst
--rw-r--r--   0        0        0     1168 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/python.rst
--rw-r--r--   0        0        0      184 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/r.rst
--rw-r--r--   0        0        0       94 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/install/ruby.rst
--rw-r--r--   0        0        0     4593 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/linear_solver/index.rst
--rw-r--r--   0        0        0      795 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/make.bat
--rw-r--r--   0        0        0       42 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/docs/src/requirements.txt
--rw-r--r--   0        0        0     3035 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/aa.h
--rw-r--r--   0        0        0     1611 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/cones.h
--rw-r--r--   0        0        0      581 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/ctrlc.h
--rw-r--r--   0        0        0     5584 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/glbopts.h
--rw-r--r--   0        0        0      804 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/linalg.h
--rw-r--r--   0        0        0     2187 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/linsys.h
--rw-r--r--   0        0        0      493 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/normalize.h
--rw-r--r--   0        0        0      571 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/rw.h
--rw-r--r--   0        0        0    10182 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/scs.h
--rw-r--r--   0        0        0     1010 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/scs_blas.h
--rw-r--r--   0        0        0      586 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/scs_types.h
--rw-r--r--   0        0        0     2817 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/scs_work.h
--rw-r--r--   0        0        0     1218 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/include/util.h
--rw-r--r--   0        0        0     8307 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/cpu/direct/private.c
--rw-r--r--   0        0        0      786 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/cpu/direct/private.h
--rw-r--r--   0        0        0     8893 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/cpu/indirect/private.c
--rw-r--r--   0        0        0      737 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/cpu/indirect/private.h
--rw-r--r--   0        0        0     6482 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/csparse.c
--rw-r--r--   0        0        0      831 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/csparse.h
--rw-r--r--   0        0        0     2068 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/LICENSE.txt
--rw-r--r--   0        0        0    14798 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/SuiteSparse_config.c
--rw-r--r--   0        0        0     9151 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/SuiteSparse_config.h
--rw-r--r--   0        0        0    17956 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd.h
--rw-r--r--   0        0        0     5716 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_1.c
--rw-r--r--   0        0        0    64847 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_2.c
--rw-r--r--   0        0        0     4868 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_aat.c
--rw-r--r--   0        0        0     1876 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_control.c
--rw-r--r--   0        0        0     1259 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_defaults.c
--rw-r--r--   0        0        0     5012 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_dump.c
--rw-r--r--   0        0        0      941 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_global.c
--rw-r--r--   0        0        0     4299 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_info.c
--rw-r--r--   0        0        0     7706 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_internal.h
--rw-r--r--   0        0        0     6084 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_order.c
--rw-r--r--   0        0        0     3703 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_post_tree.c
--rw-r--r--   0        0        0     5509 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_postorder.c
--rw-r--r--   0        0        0     3808 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_preprocess.c
--rw-r--r--   0        0        0     2980 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/amd_valid.c
--rw-r--r--   0        0        0      528 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/amd/changes
--rw-r--r--   0        0        0    11357 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/LICENSE
--rw-r--r--   0        0        0     4865 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/README.md
--rw-r--r--   0        0        0      210 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/changes
--rw-r--r--   0        0        0     7683 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl.c
--rw-r--r--   0        0        0     6397 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl.h
--rw-r--r--   0        0        0      533 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl_types.h
--rw-r--r--   0        0        0     2581 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/gpu/gpu.c
--rw-r--r--   0        0        0     3952 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/gpu/gpu.h
--rw-r--r--   0        0        0    16766 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/gpu/indirect/private.c
--rw-r--r--   0        0        0     1419 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/gpu/indirect/private.h
--rw-r--r--   0        0        0     6311 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/mkl/direct/private.c
--rw-r--r--   0        0        0     1227 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/mkl/direct/private.h
--rw-r--r--   0        0        0    12150 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/scs_matrix.c
--rw-r--r--   0        0        0     1839 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/linsys/scs_matrix.h
--rw-r--r--   0        0        0     5112 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/scs.mk
--rw-r--r--   0        0        0    14893 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/aa.c
--rw-r--r--   0        0        0    22699 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/cones.c
--rw-r--r--   0        0        0     1770 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/ctrlc.c
--rw-r--r--   0        0        0    10370 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/exp_cone.c
--rw-r--r--   0        0        0     3996 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/linalg.c
--rw-r--r--   0        0        0     2598 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/normalize.c
--rw-r--r--   0        0        0    15587 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/rw.c
--rw-r--r--   0        0        0    40471 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/scs.c
--rw-r--r--   0        0        0      147 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/scs_version.c
--rw-r--r--   0        0        0     3900 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/src/util.c
--rw-r--r--   0        0        0     1651 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/minunit.h
--rw-r--r--   0        0        0     7970 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problem_utils.h
--rw-r--r--   0        0        0     3065 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/degenerate.h
--rw-r--r--   0        0        0     3051 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/hs21_tiny_qp.h
--rw-r--r--   0        0        0     2917 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/hs21_tiny_qp_rw.h
--rw-r--r--   0        0        0     3260 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/infeasible_tiny_qp.h
--rw-r--r--   0        0        0  1128241 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/max_ent
--rw-r--r--   0        0        0      238 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/max_ent.h
--rw-r--r--   0        0        0     7530 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/qafiro_tiny_qp.h
--rw-r--r--   0        0        0     8481 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/random_prob
--rw-r--r--   0        0        0      229 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/random_prob.h
--rw-r--r--   0        0        0     7271 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/rob_gauss_cov_est.h
--rw-r--r--   0        0        0     1656 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/small_lp.h
--rw-r--r--   0        0        0    22554 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/small_qp.h
--rw-r--r--   0        0        0     2523 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/test_exp_cone.h
--rw-r--r--   0        0        0     1311 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/test_prob_from_data_file.h
--rw-r--r--   0        0        0     1250 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/test_validation.h
--rw-r--r--   0        0        0     2517 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/problems/unbounded_tiny_qp.h
--rw-r--r--   0        0        0     5047 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/random_socp_prob.c
--rw-r--r--   0        0        0     3911 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/rng.h
--rw-r--r--   0        0        0     2666 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/run_from_file.c
--rw-r--r--   0        0        0     2137 2023-11-08 11:20:07.000000 scs-3.2.4.post1/scs_source/test/run_tests.c
--rw-r--r--   0        0        0     7016 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/gen_random_cone_prob.py
--rw-r--r--   0        0        0     2193 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/solve_random_cone_prob.py
--rw-r--r--   0        0        0     2482 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_scs_basic.py
--rw-r--r--   0        0        0     2400 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_scs_object.py
--rw-r--r--   0        0        0      472 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_scs_quad.py
--rw-r--r--   0        0        0     2446 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_scs_rand.py
--rw-r--r--   0        0        0     2452 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_scs_sdp.py
--rw-r--r--   0        0        0     2781 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_solve_random_cone_prob.py
--rw-r--r--   0        0        0     2545 2023-11-22 11:07:49.000000 scs-3.2.4.post1/test/test_solve_random_cone_prob_mkl.py
--rw-r--r--   0        0        0     2060 2023-11-22 11:59:42.000476 scs-3.2.4.post1/PKG-INFO
+-rw-r--r--   0        0        0      115 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.bumpversion.cfg
+-rw-r--r--   0        0        0     1572 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      536 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.github/dependabot.yml
+-rw-r--r--   0        0        0     7687 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      463 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.gitignore
+-rw-r--r--   0        0        0       78 2024-05-29 18:22:00.000000 scs-3.2.4.post2/.gitmodules
+-rw-r--r--   0        0        0     1075 2024-05-29 18:22:00.000000 scs-3.2.4.post2/LICENSE
+-rw-r--r--   0        0        0      355 2024-05-29 18:22:00.000000 scs-3.2.4.post2/MANIFEST.in
+-rw-r--r--   0        0        0      567 2024-05-29 18:22:00.000000 scs-3.2.4.post2/README.md
+-rwxr-xr-x   0        0        0      144 2024-05-29 18:22:00.000000 scs-3.2.4.post2/distribute.sh
+-rw-r--r--   0        0        0    10691 2024-05-29 18:22:00.000000 scs-3.2.4.post2/legacy_setup.py
+-rw-r--r--   0        0        0     6143 2024-05-29 18:22:00.000000 scs-3.2.4.post2/meson.build
+-rw-r--r--   0        0        0      354 2024-05-29 18:22:00.000000 scs-3.2.4.post2/meson.options
+-rw-r--r--   0        0        0   357429 2024-05-29 18:22:00.000000 scs-3.2.4.post2/notebooks/analyze_csv_logs.ipynb
+-rw-r--r--   0        0        0   276982 2024-05-29 18:22:00.000000 scs-3.2.4.post2/notebooks/scs_benchmarks.ipynb
+-rw-r--r--   0        0        0   217308 2024-05-29 18:22:00.000000 scs-3.2.4.post2/notebooks/scs_qp.ipynb
+-rw-r--r--   0        0        0      380 2024-05-29 18:22:00.000000 scs-3.2.4.post2/pyproject.toml
+-rw-r--r--   0        0        0     6136 2024-05-29 18:22:00.000000 scs-3.2.4.post2/scs/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-29 18:22:00.000000 scs-3.2.4.post2/scs/scsmodule.h
+-rw-r--r--   0        0        0    26835 2024-05-29 18:22:00.000000 scs-3.2.4.post2/scs/scsobject.h
+-rw-r--r--   0        0        0     1237 2024-05-29 18:22:00.000000 scs-3.2.4.post2/scs/scspy.c
+-rw-r--r--   0        0        0      295 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.bumpversion.cfg
+-rw-r--r--   0        0        0      855 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0     1247 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1048 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/build_mkl.yml
+-rw-r--r--   0        0        0      453 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/build_openmp.yml
+-rw-r--r--   0        0        0      962 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/buildpp.yml
+-rw-r--r--   0        0        0     1278 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/cmake.yml
+-rw-r--r--   0        0        0     1332 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/cmake_mkl.yml
+-rw-r--r--   0        0        0      688 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/cmake_openmp.yml
+-rw-r--r--   0        0        0      971 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      773 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      353 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/gpu.yml
+-rw-r--r--   0        0        0      568 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.github/workflows/valgrind.yml
+-rw-r--r--   0        0        0      488 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/.gitignore
+-rw-r--r--   0        0        0     1009 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/CITATION.cff
+-rw-r--r--   0        0        0    15929 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/CMakeLists.txt
+-rw-r--r--   0        0        0     1110 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/LICENSE.txt
+-rw-r--r--   0        0        0     8572 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/Makefile
+-rw-r--r--   0        0        0      922 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/README.md
+-rw-r--r--   0        0        0     8748 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/cmake/AddInstallRPATHSupport.cmake
+-rw-r--r--   0        0        0     2499 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/cmake/AddUninstallTarget.cmake
+-rw-r--r--   0        0        0    28861 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/cmake/InstallBasicPackageFiles.cmake
+-rw-r--r--   0        0        0      435 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/cmake/scs_types.h.in
+-rw-r--r--   0        0        0   114472 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/Doxyfile
+-rw-r--r--   0        0        0      736 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/Makefile
+-rw-r--r--   0        0        0     1916 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/_static/css/scs_theme.css
+-rw-r--r--   0        0        0     1150 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/_static/favicon.ico
+-rw-r--r--   0        0        0   180020 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/_static/scs_logo.png
+-rw-r--r--   0        0        0   154780 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/_static/scs_logo_transparent.png
+-rw-r--r--   0        0        0     9294 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/acceleration.rst
+-rw-r--r--   0        0        0     4324 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/equilibration.rst
+-rw-r--r--   0        0        0     5932 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/index.rst
+-rw-r--r--   0        0        0     1037 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/relaxation.rst
+-rw-r--r--   0        0        0     7510 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/scale.rst
+-rw-r--r--   0        0        0     1680 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/algorithm/warm_start.rst
+-rw-r--r--   0        0        0     3230 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/c.rst
+-rw-r--r--   0        0        0     2396 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/compile_flags.rst
+-rw-r--r--   0        0        0     7064 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/cones.rst
+-rw-r--r--   0        0        0     1326 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/exit_flags.rst
+-rw-r--r--   0        0        0     1150 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/index.rst
+-rw-r--r--   0        0        0     2868 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/info.rst
+-rw-r--r--   0        0        0      302 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/julia.rst
+-rw-r--r--   0        0        0     1372 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/matlab.rst
+-rw-r--r--   0        0        0      868 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/matrices.rst
+-rw-r--r--   0        0        0     3054 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/python.rst
+-rw-r--r--   0        0        0     1365 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/r.rst
+-rw-r--r--   0        0        0       97 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/ruby.rst
+-rw-r--r--   0        0        0     3082 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/api/settings.rst
+-rw-r--r--   0        0        0     1636 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/blas_lapack/index.rst
+-rw-r--r--   0        0        0     2554 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/citing/index.rst
+-rw-r--r--   0        0        0     3051 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/conf.py
+-rw-r--r--   0        0        0     1127 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/contributing/index.rst
+-rw-r--r--   0        0        0        7 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/.gitignore
+-rw-r--r--   0        0        0      526 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/c.rst
+-rw-r--r--   0        0        0      405 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/index.rst
+-rw-r--r--   0        0        0      967 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/julia.rst
+-rw-r--r--   0        0        0      451 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/matlab.rst
+-rw-r--r--   0        0        0      342 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/basic_qp.rst
+-rw-r--r--   0        0        0     1605 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.py
+-rw-r--r--   0        0        0     1444 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.py.out
+-rw-r--r--   0        0        0     1342 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.rst
+-rw-r--r--   0        0        0     1894 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.py
+-rw-r--r--   0        0        0    11938 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.py.out
+-rw-r--r--   0        0        0     1767 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.rst
+-rw-r--r--   0        0        0     2935 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.py
+-rw-r--r--   0        0        0    13637 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.py.out
+-rw-r--r--   0        0        0     3211 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.rst
+-rw-r--r--   0        0        0     3521 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.py
+-rw-r--r--   0        0        0     8375 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.py.out
+-rw-r--r--   0        0        0     2082 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.rst
+-rw-r--r--   0        0        0      608 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/qp.py
+-rw-r--r--   0        0        0     1403 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python/qp.py.out
+-rw-r--r--   0        0        0      381 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/python.rst
+-rw-r--r--   0        0        0     2620 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/qp.c
+-rw-r--r--   0        0        0     1545 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/qp.c.out
+-rw-r--r--   0        0        0      540 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/qp.m
+-rw-r--r--   0        0        0     1940 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/qp.m.out
+-rw-r--r--   0        0        0     1100 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/qp.prob
+-rw-r--r--   0        0        0     3275 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/r.rst
+-rw-r--r--   0        0        0       90 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/examples/ruby.rst
+-rw-r--r--   0        0        0    21926 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/files/windows1.png
+-rw-r--r--   0        0        0    81416 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/files/windows2.png
+-rw-r--r--   0        0        0    17775 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/files/windows3.png
+-rw-r--r--   0        0        0      885 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/help/index.rst
+-rw-r--r--   0        0        0     3888 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/index.rst
+-rw-r--r--   0        0        0     4439 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/c.rst
+-rw-r--r--   0        0        0      382 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/index.rst
+-rw-r--r--   0        0        0      502 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/julia.rst
+-rw-r--r--   0        0        0      452 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/matlab.rst
+-rw-r--r--   0        0        0     1168 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/python.rst
+-rw-r--r--   0        0        0      184 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/r.rst
+-rw-r--r--   0        0        0       94 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/install/ruby.rst
+-rw-r--r--   0        0        0     4593 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/linear_solver/index.rst
+-rw-r--r--   0        0        0      795 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/make.bat
+-rw-r--r--   0        0        0       42 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/docs/src/requirements.txt
+-rw-r--r--   0        0        0     3035 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/aa.h
+-rw-r--r--   0        0        0     1611 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/cones.h
+-rw-r--r--   0        0        0      581 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/ctrlc.h
+-rw-r--r--   0        0        0     5584 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/glbopts.h
+-rw-r--r--   0        0        0      804 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/linalg.h
+-rw-r--r--   0        0        0     2187 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/linsys.h
+-rw-r--r--   0        0        0      493 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/normalize.h
+-rw-r--r--   0        0        0      571 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/rw.h
+-rw-r--r--   0        0        0    10182 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/scs.h
+-rw-r--r--   0        0        0     1010 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/scs_blas.h
+-rw-r--r--   0        0        0      586 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/scs_types.h
+-rw-r--r--   0        0        0     2817 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/scs_work.h
+-rw-r--r--   0        0        0     1218 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/include/util.h
+-rw-r--r--   0        0        0     8307 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/cpu/direct/private.c
+-rw-r--r--   0        0        0      786 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/cpu/direct/private.h
+-rw-r--r--   0        0        0     8893 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/cpu/indirect/private.c
+-rw-r--r--   0        0        0      737 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/cpu/indirect/private.h
+-rw-r--r--   0        0        0     6482 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/csparse.c
+-rw-r--r--   0        0        0      831 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/csparse.h
+-rw-r--r--   0        0        0     2068 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/LICENSE.txt
+-rw-r--r--   0        0        0    14798 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/SuiteSparse_config.c
+-rw-r--r--   0        0        0     9151 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/SuiteSparse_config.h
+-rw-r--r--   0        0        0    17956 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd.h
+-rw-r--r--   0        0        0     5716 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_1.c
+-rw-r--r--   0        0        0    64847 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_2.c
+-rw-r--r--   0        0        0     4868 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_aat.c
+-rw-r--r--   0        0        0     1876 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_control.c
+-rw-r--r--   0        0        0     1259 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_defaults.c
+-rw-r--r--   0        0        0     5012 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_dump.c
+-rw-r--r--   0        0        0      941 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_global.c
+-rw-r--r--   0        0        0     4299 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_info.c
+-rw-r--r--   0        0        0     7706 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_internal.h
+-rw-r--r--   0        0        0     6084 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_order.c
+-rw-r--r--   0        0        0     3703 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_post_tree.c
+-rw-r--r--   0        0        0     5509 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_postorder.c
+-rw-r--r--   0        0        0     3808 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_preprocess.c
+-rw-r--r--   0        0        0     2980 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/amd_valid.c
+-rw-r--r--   0        0        0      528 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/amd/changes
+-rw-r--r--   0        0        0    11357 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/LICENSE
+-rw-r--r--   0        0        0     4865 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/README.md
+-rw-r--r--   0        0        0      210 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/changes
+-rw-r--r--   0        0        0     7683 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl.c
+-rw-r--r--   0        0        0     6397 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl.h
+-rw-r--r--   0        0        0      533 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl_types.h
+-rw-r--r--   0        0        0     2581 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/gpu/gpu.c
+-rw-r--r--   0        0        0     3952 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/gpu/gpu.h
+-rw-r--r--   0        0        0    16766 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/gpu/indirect/private.c
+-rw-r--r--   0        0        0     1419 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/gpu/indirect/private.h
+-rw-r--r--   0        0        0     6311 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/mkl/direct/private.c
+-rw-r--r--   0        0        0     1227 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/mkl/direct/private.h
+-rw-r--r--   0        0        0    12150 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/scs_matrix.c
+-rw-r--r--   0        0        0     1839 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/linsys/scs_matrix.h
+-rw-r--r--   0        0        0     5112 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/scs.mk
+-rw-r--r--   0        0        0    14893 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/aa.c
+-rw-r--r--   0        0        0    22715 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/cones.c
+-rw-r--r--   0        0        0     1770 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/ctrlc.c
+-rw-r--r--   0        0        0    10370 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/exp_cone.c
+-rw-r--r--   0        0        0     3996 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/linalg.c
+-rw-r--r--   0        0        0     2598 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/normalize.c
+-rw-r--r--   0        0        0    15587 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/rw.c
+-rw-r--r--   0        0        0    40471 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/scs.c
+-rw-r--r--   0        0        0      147 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/scs_version.c
+-rw-r--r--   0        0        0     3900 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/src/util.c
+-rw-r--r--   0        0        0     1651 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/minunit.h
+-rw-r--r--   0        0        0     7970 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problem_utils.h
+-rw-r--r--   0        0        0     3065 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/degenerate.h
+-rw-r--r--   0        0        0     3051 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/hs21_tiny_qp.h
+-rw-r--r--   0        0        0     2917 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/hs21_tiny_qp_rw.h
+-rw-r--r--   0        0        0     3260 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/infeasible_tiny_qp.h
+-rw-r--r--   0        0        0  1128241 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/max_ent
+-rw-r--r--   0        0        0      238 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/max_ent.h
+-rw-r--r--   0        0        0     7530 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/qafiro_tiny_qp.h
+-rw-r--r--   0        0        0     8481 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/random_prob
+-rw-r--r--   0        0        0      229 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/random_prob.h
+-rw-r--r--   0        0        0     7271 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/rob_gauss_cov_est.h
+-rw-r--r--   0        0        0     1656 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/small_lp.h
+-rw-r--r--   0        0        0    22554 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/small_qp.h
+-rw-r--r--   0        0        0     2523 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/test_exp_cone.h
+-rw-r--r--   0        0        0     1311 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/test_prob_from_data_file.h
+-rw-r--r--   0        0        0     1250 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/test_validation.h
+-rw-r--r--   0        0        0     2517 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/problems/unbounded_tiny_qp.h
+-rw-r--r--   0        0        0     5047 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/random_socp_prob.c
+-rw-r--r--   0        0        0     3911 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/rng.h
+-rw-r--r--   0        0        0     2666 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/run_from_file.c
+-rw-r--r--   0        0        0     2137 2024-05-02 10:40:53.000000 scs-3.2.4.post2/scs_source/test/run_tests.c
+-rw-r--r--   0        0        0     7016 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/gen_random_cone_prob.py
+-rw-r--r--   0        0        0     2193 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/solve_random_cone_prob.py
+-rw-r--r--   0        0        0     2482 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_scs_basic.py
+-rw-r--r--   0        0        0     2400 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_scs_object.py
+-rw-r--r--   0        0        0      472 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_scs_quad.py
+-rw-r--r--   0        0        0     2446 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_scs_rand.py
+-rw-r--r--   0        0        0     2452 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_scs_sdp.py
+-rw-r--r--   0        0        0     2781 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_solve_random_cone_prob.py
+-rw-r--r--   0        0        0     2545 2024-05-29 18:22:00.000000 scs-3.2.4.post2/test/test_solve_random_cone_prob_mkl.py
+-rw-r--r--   0        0        0     2060 2024-05-29 18:41:04.117384 scs-3.2.4.post2/PKG-INFO
```

### Comparing `scs-3.2.4.post1/.github/ISSUE_TEMPLATE.md` & `scs-3.2.4.post2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/.github/workflows/build.yml` & `scs-3.2.4.post2/.github/workflows/build.yml`

 * *Files 13% similar despite different names*

```diff
@@ -22,27 +22,28 @@
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: [ ubuntu-latest ]
-        python-version: [ 3.7, 3.8, 3.9, "3.10", "3.11" ]
+        python-version: [ 3.8, 3.9, "3.10", "3.11" ]
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: recursive
-      - uses: conda-incubator/setup-miniconda@v2
+      - uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
+          miniforge-version: latest
           channels: conda-forge,anaconda
       - name: Install dependencies
         run: |
           conda install scipy numpy pytest
       - name: Test
         run: |
           python legacy_setup.py install --scs --openmp
@@ -53,94 +54,114 @@
     runs-on: ${{ matrix.os }}
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest, windows-latest ]
-        python-version: [ 3.7, 3.8, 3.9, "3.10", "3.11", "3.12"]
+        # macos-13 runners have intel chips. macos-14 and above
+        # runners have Apple silicon chips.
+        os: [ ubuntu-latest, macos-13, windows-latest ]
+        python-version: [ 3.8, 3.9, "3.10", "3.11", "3.12"]
+        link_mkl: [true, false]
 
     env:
       PYTHON_VERSION: ${{ matrix.python-version }}
+      LINK_MKL: ${{ matrix.link_mkl }}
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: recursive
+
       - name: Set Additional Envs
         shell: bash
         run: |
           echo "DEPLOY=$( [[ $GITHUB_EVENT_NAME == 'push' && $GITHUB_REF == 'refs/tags'* ]] && echo 'True' || echo 'False' )" >> $GITHUB_ENV
-      - uses: conda-incubator/setup-miniconda@v2
+          echo "PYTHON_SUBVERSION=$(echo $PYTHON_VERSION | cut -c 3-)" >> $GITHUB_ENV
+      - uses: conda-incubator/setup-miniconda@v3
         with:
           auto-update-conda: true
           python-version: ${{ matrix.python-version }}
+          miniforge-version: latest
           channels: conda-forge,anaconda
       - name: Install dependencies
         run: |
-          if [[ "$PYTHON_VERSION" == "3.7" ]] || [[ "$PYTHON_VERSION" == "3.8" ]] || [[ "$PYTHON_VERSION" == "3.9" ]]; then
-            conda install scipy=1.5 numpy=1.19 pytest mkl openblas lapack
+          if [[ "$LINK_MKL" == "true" ]]; then
+            BLAS_PKGS="blas-devel=*=*mkl"
+          else
+            BLAS_PKGS="blas-devel=*=*openblas"
+          fi
+          if [[ "$PYTHON_VERSION" == "3.8" ]] || [[ "$PYTHON_VERSION" == "3.9" ]]; then
+            conda install scipy=1.5 numpy=1.19 pytest $BLAS_PKGS pkg-config
           elif [[ "$PYTHON_VERSION" == "3.10" ]]; then
-            conda install scipy=1.7 numpy=1.21 pytest mkl openblas lapack
+            conda install scipy=1.7 numpy=1.21 pytest $BLAS_PKGS pkg-config
           elif [[ "$PYTHON_VERSION" == "3.11" ]]; then
-            conda install scipy=1.9.3 numpy=1.23.4 pytest mkl openblas lapack
+            conda install scipy=1.9.3 numpy=1.23.4 pytest $BLAS_PKGS pkg-config
           elif [[ "$PYTHON_VERSION" == "3.12" ]]; then
-            conda install scipy numpy pytest mkl openblas lapack
+            conda install scipy numpy pytest $BLAS_PKGS pkg-config
           fi
       - name: Build
         run: |
-          if [[ "$PYTHON_VERSION" == "3.7" ]] || [[ "$PYTHON_VERSION" == "3.8" ]]; then
-            python legacy_setup.py install
-          elif [[ "$PYTHON_VERSION" != "3.7" ]] && [[ "$PYTHON_VERSION" != "3.8" ]]; then
+          if [[ "$PYTHON_VERSION" == "3.8" ]]; then
+            if [[ "$LINK_MKL" == "true" ]]; then
+              python legacy_setup.py install --scs --mkl
+            else
+              python legacy_setup.py install
+            fi
+          elif [[ "$PYTHON_VERSION" != "3.8" ]]; then
             python -c "import numpy as np; print('NUMPY BLAS INFOS'); print(np.show_config())"
-            python -m pip install --verbose .
+            if [[ "$LINK_MKL" == "true" ]]; then
+              python -m pip install --verbose -Csetup-args=-Dlink_mkl=true .
+            else
+              python -m pip install --verbose .
+            fi
           fi
       - name: Test
         run: |
           pytest
           rm -rf build/
       - name: Build and test windows wheels
-        if: ${{startsWith(matrix.os, 'windows')}}
+        if: ${{startsWith(matrix.os, 'windows') && !matrix.link_mkl}}
         run: |
           python -m pip install build
           python -m build -Csetup-args="-Dlink_blas_statically=True"
           python -m pip install delvewheel
           delvewheel repair dist/*whl
           conda remove openblas # to check static linkage
           pip install wheelhouse/*whl --force-reinstall
           pytest
       - name: Upload artifacts to github
-        if: ${{env.DEPLOY == 'True' && startsWith(matrix.os, 'windows')}}
-        uses: actions/upload-artifact@v1
+        if: ${{ startsWith(matrix.os, 'windows') }}
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-${{ matrix.os }}-3-${{ env.PYTHON_SUBVERSION }}
           path: ./wheelhouse
 
 
   build_wheels:
     needs: build
 
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        os: [ ubuntu-latest, macos-latest ]
-        python-version: [ 3.7, 3.8, 3.9, "3.10", "3.11", "3.12"]
+        os: [ ubuntu-latest, macos-13, macos-latest ]
+        python-version: [ 3.8, 3.9, "3.10", "3.11", "3.12"]
 
     env:
       RUNNER_OS: ${{ matrix.os }}
       PYTHON_VERSION: ${{ matrix.python-version }}
 
     steps:
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           submodules: recursive
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
       - name: Set Additional Envs
         shell: bash
         run: |
           echo "PYTHON_SUBVERSION=$(echo $PYTHON_VERSION | cut -c 3-)" >> $GITHUB_ENV
           echo "SINGLE_ACTION_CONFIG=$( [[ $PYTHON_VERSION == 3.8 && $RUNNER_OS == 'macOS' ]] && echo 'True' || echo 'False' )" >> $GITHUB_ENV
@@ -148,56 +169,63 @@
 
       - name: Build wheels
         env:
           CIBW_MANYLINUX_X86_64_IMAGE: manylinux2014
           CIBW_BUILD: "cp3${{env.PYTHON_SUBVERSION}}-*"
           CIBW_SKIP: "*-win32 *-manylinux_i686 *-musllinux*"
           CIBW_BEFORE_ALL_LINUX: yum install -y openblas-devel
-          CIBW_BEFORE_ALL_MACOS: >
-            brew install openblas &&
-            cp -r /usr/local/opt/openblas/lib/* /usr/local/lib &&
-            cp /usr/local/opt/openblas/include/* /usr/local/include
           CIBW_ENVIRONMENT_MACOS: CFLAGS='-Wno-error=implicit-function-declaration'
           CIBW_BUILD_VERBOSITY: 3
           CIBW_TEST_REQUIRES: pytest
           CIBW_TEST_COMMAND: pytest {package}
-        uses: joerick/cibuildwheel@v2.16.2
+        uses: joerick/cibuildwheel@v2.18.1
 
       - name: Build source
         if: ${{env.SINGLE_ACTION_CONFIG == 'True'}}
         run: |
           python -m pip install build
           python -m build -Csetup-args="-Dlink_blas_statically=True" --outdir=wheelhouse
 
       - name: Upload artifacts to github
-        if: ${{env.DEPLOY == 'True'}}
-        uses: actions/upload-artifact@v1
+        uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: wheels-${{ matrix.os }}-3-${{ env.PYTHON_SUBVERSION }}
           path: ./wheelhouse
 
-  upload_wheels:
+  merge_wheels:
+    name: Merge wheel artifacts
+    runs-on: ubuntu-latest
     needs: build_wheels
+    steps:
+      - name: Merge wheels
+        uses: actions/upload-artifact/merge@v4
+        with:
+          name: wheels
+          pattern: wheels-*
+          delete-merged: true
+
+  upload_wheels:
+    needs: merge_wheels
     runs-on: ubuntu-latest
 
     env:
       PYPI_SERVER: ${{ secrets.PYPI_SERVER }}
       PYPI_USER: ${{ secrets.PYPI_USER }}
       PYPI_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v2
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.8
       - name: Set Additional Envs
         shell: bash
         run: |
           echo "DEPLOY=$( [[ $GITHUB_EVENT_NAME == 'push' && $GITHUB_REF == 'refs/tags'* ]] && echo 'True' || echo 'False' )" >> $GITHUB_ENV
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v4
         if: ${{env.DEPLOY == 'True'}}
         with:
           name: wheels
           path: ./wheelhouse
 
       - name: Release to pypi
         if: ${{env.DEPLOY == 'True'}}
```

### Comparing `scs-3.2.4.post1/LICENSE` & `scs-3.2.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/README.md` & `scs-3.2.4.post2/README.md`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/legacy_setup.py` & `scs-3.2.4.post2/legacy_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             extra_compile_args=list(extra_compile_args),
             extra_link_args=list(extra_link_args),
         )
         ext_modules += [_scs_mkl]
 
     setup(
         name="scs",
-        version="3.2.4.post1",
+        version="3.2.4.post2",
         author="Brendan O'Donoghue",
         author_email="bodonoghue85@gmail.com",
         url="http://github.com/cvxgrp/scs",
         description="scs: splitting conic solver",
         package_dir={"scs": "scs"},
         packages=["scs"],
         ext_modules=ext_modules,
```

### Comparing `scs-3.2.4.post1/meson.build` & `scs-3.2.4.post2/meson.build`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 project('scs', 'c')
 
 py = import('python').find_installation(pure: false)
 
 cc = meson.get_compiler('c')
 blas_deps = []
-if host_machine.system() == 'darwin'
-  blas_deps = [dependency('Accelerate')]
-else
-  blas_deps = [cc.find_library('openblas', static: get_option('link_blas_statically'), required : false)]
-  if not blas_deps[0].found()
-    blas_deps = [dependency(['openblas', 'OpenBLAS'], static: get_option('link_blas_statically'), required : false)]
-  endif
-endif
 
-# try to find blas/cblas (e.g., Linux)
-if not blas_deps[0].found()
-    blas_deps = [cc.find_library('blas', static: get_option('link_blas_statically'), required : false)]
+if get_option('link_mkl')
+    blas_deps = [cc.find_library('mkl_rt', required : false)]
     if not blas_deps[0].found()
-      blas_deps = [dependency('blas', static: get_option('link_blas_statically'), required : false)]
-    endif
-    lapack_dep = cc.find_library('lapack', static: get_option('link_blas_statically'), required : false)
-    if not lapack_dep.found()
-      lapack_dep = dependency('lapack', static: get_option('link_blas_statically'), required : false)
-    endif
-    if lapack_dep.found()
-        blas_deps += lapack_dep
-    endif
-    cblas_dep = cc.find_library('cblas', static: get_option('link_blas_statically'), required : false)
-    if not cblas_dep.found()
-      cblas_dep = dependency('cblas', static: get_option('link_blas_statically'), required : false)
+        blas_deps = [dependency('mkl-sdl', required : false)]
     endif
-    if cblas_dep.found()
-        blas_deps += cblas_dep
+else
+    if host_machine.system() == 'darwin'
+        blas_deps = [dependency('Accelerate')]
+    else
+        blas_deps = [cc.find_library('openblas', static: get_option('link_blas_statically'), required : false)]
+        if not blas_deps[0].found()
+            blas_deps = [dependency(['openblas', 'OpenBLAS'], static: get_option('link_blas_statically'), required : false)]
+        endif
     endif
-endif
 
-# We find anaconda blas on windows for github CI
-if host_machine.system() == 'windows' and not blas_deps[0].found()
-    message(run_command(py,['-c','''import os; print('CONDA LIB FOLDER'); print(os.listdir('C:/Miniconda/envs/test\\Library\\lib'))''']).stdout())
-    blas_deps = [cc.find_library('openblas',
-        dirs: ['C:/Miniconda/envs/test\\Library\\lib'], # this is the location on github CI
-        static: get_option('link_blas_statically'),
-        required : false)]
+    # try to find blas/cblas (e.g., Linux)
+    if not blas_deps[0].found()
+        blas_deps = [cc.find_library('blas', static: get_option('link_blas_statically'), required : false)]
+        if not blas_deps[0].found()
+            blas_deps = [dependency('blas', static: get_option('link_blas_statically'), required : false)]
+        endif
+        lapack_dep = cc.find_library('lapack', static: get_option('link_blas_statically'), required : false)
+        if not lapack_dep.found()
+            lapack_dep = dependency('lapack', static: get_option('link_blas_statically'), required : false)
+        endif
+        if lapack_dep.found()
+            blas_deps += lapack_dep
+        endif
+        cblas_dep = cc.find_library('cblas', static: get_option('link_blas_statically'), required : false)
+        if not cblas_dep.found()
+            cblas_dep = dependency('cblas', static: get_option('link_blas_statically'), required : false)
+        endif
+        if cblas_dep.found()
+            blas_deps += cblas_dep
+        endif
+    endif
 endif
 
 # Since nothing above was required, we stop here if failed
 if not blas_deps[0].found()
     error('OpenBLAS or Netlib BLAS/CBLAS is required on all platforms except Windows, and was not found.')
 endif
 
@@ -152,8 +151,44 @@
         incdir_numpy],
     install: true,
     c_args: c_args + ['-DPYTHON', '-DCTRLC=1', '-DPY_INDIRECT', '-DINDIRECT=1',
          '-DUSE_LAPACK=1', '-DDLONG=1'],
     dependencies: blas_deps,
 )
 
+if get_option('link_mkl')
+    py.extension_module(
+        '_scs_mkl',
+
+        'scs/scspy.c',
+        'scs_source/linsys/mkl/direct/private.c',
+
+        # scs_source/src:
+        'scs_source/src/aa.c',
+        'scs_source/src/cones.c',
+        'scs_source/src/ctrlc.c',
+        'scs_source/src/exp_cone.c',
+        'scs_source/src/linalg.c',
+        'scs_source/src/normalize.c',
+        'scs_source/src/rw.c',
+        'scs_source/src/scs_version.c',
+        'scs_source/src/scs.c',
+        'scs_source/src/util.c',
+
+        # scs_source/linsys:
+        'scs_source/linsys/scs_matrix.c',
+        'scs_source/linsys/csparse.c',
+
+        include_directories : [
+            'scs',
+            'scs_source/include',
+            'scs_source/linsys',
+            'scs_source/linsys/mkl/direct',
+            incdir_numpy],
+        install: true,
+        c_args: c_args + ['-DPYTHON', '-DCTRLC=1', '-DPY_MKL',
+             '-DUSE_LAPACK=1', '-DDLONG=1'],
+        dependencies: blas_deps,
+    )
+endif
+
 py.install_sources('scs/__init__.py', subdir: 'scs')
```

### Comparing `scs-3.2.4.post1/notebooks/analyze_csv_logs.ipynb` & `scs-3.2.4.post2/notebooks/analyze_csv_logs.ipynb`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/notebooks/scs_benchmarks.ipynb` & `scs-3.2.4.post2/notebooks/scs_benchmarks.ipynb`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/notebooks/scs_qp.ipynb` & `scs-3.2.4.post2/notebooks/scs_qp.ipynb`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs/__init__.py` & `scs-3.2.4.post2/scs/__init__.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs/scsmodule.h` & `scs-3.2.4.post2/scs/scsmodule.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs/scsobject.h` & `scs-3.2.4.post2/scs/scsobject.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs/scspy.c` & `scs-3.2.4.post2/scs/scspy.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/ISSUE_TEMPLATE.md` & `scs-3.2.4.post2/scs_source/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/build.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/build_mkl.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/build_mkl.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/buildpp.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/buildpp.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/cmake.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/cmake.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/cmake_mkl.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/cmake_mkl.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/cmake_openmp.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/cmake_openmp.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/coverage.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/docs.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/.github/workflows/valgrind.yml` & `scs-3.2.4.post2/scs_source/.github/workflows/valgrind.yml`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/CITATION.cff` & `scs-3.2.4.post2/scs_source/CITATION.cff`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/CMakeLists.txt` & `scs-3.2.4.post2/scs_source/CMakeLists.txt`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 message(STATUS "BLAS/LAPACK usage is ${USE_LAPACK}")
 
 # Enable OpenMP support
 option(USE_OPENMP "Compile with OpenMP support" OFF)
 message(STATUS "OpenMP parallelization is ${USE_OPENMP}")
 
 set(COMPILER_OPTS "-DCTRLC")
+set(LAPACK_LINK_LIBRARIES "")
 
 # Primitive types
 if(SFLOAT)
   set(SCS_FLOAT_TYPE "float")
   set(COMPILER_OPTS "-DSFLOAT ${COMPILER_OPTS}")
 else()
   set(SCS_FLOAT_TYPE "double")
@@ -151,14 +152,15 @@
 
 if(NO_READ_WRITE)
   set(COMPILER_OPTS "-DNO_READ_WRITE=1 ${COMPILER_OPTS}")
 endif()
 
 if (USE_LAPACK)
   set(COMPILER_OPTS "-DUSE_LAPACK ${COMPILER_OPTS}")
+  list(APPEND LAPACK_LINK_LIBRARIES "blas" "lapack")
 endif()
 
 if(USE_OPENMP)
   set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -fopenmp")
 endif()
 
 message(STATUS "COMPILER_OPTS = ${COMPILER_OPTS}")
@@ -238,16 +240,16 @@
   ${${PROJECT_NAME}_DIRECT}
   PUBLIC "$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>"
          "$<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}/scs>")
 
 # Compiled with blas and lapack, can solve LPs, SOCPs, SDPs, ECPs, and PCPs
 target_compile_definitions(${${PROJECT_NAME}_DIRECT} PRIVATE ${COMPILER_OPTS})
 
-# The library depends on math (m) blas and lapack
-target_link_libraries(${${PROJECT_NAME}_DIRECT} PRIVATE m blas lapack)
+# The library depends on math (m) and (optionally) blas and lapack
+target_link_libraries(${${PROJECT_NAME}_DIRECT} PRIVATE m ${LAPACK_LINK_LIBRARIES})
 
 # Set some properties
 set_target_properties(
   ${${PROJECT_NAME}_DIRECT}
   PROPERTIES VERSION ${scs_VERSION} PUBLIC_HEADER
                                     "${${PROJECT_NAME}_PUBLIC_HDR}")
 
@@ -286,16 +288,16 @@
   PUBLIC "$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>"
          "$<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}/scs>")
 
 # Compiled with blas and lapack, can solve LPs, SOCPs, SDPs, ECPs, and PCPs
 target_compile_definitions(${${PROJECT_NAME}_INDIRECT} PRIVATE ${COMPILER_OPTS}
                                                                -DINDIRECT)
 
-# The library depends on math (m) blas and lapack
-target_link_libraries(${${PROJECT_NAME}_INDIRECT} PUBLIC m blas lapack)
+# The library depends on math (m) and (optionally) blas and lapack
+target_link_libraries(${${PROJECT_NAME}_INDIRECT} PUBLIC m ${LAPACK_LINK_LIBRARIES})
 
 # Set some properties
 set_target_properties(
   ${${PROJECT_NAME}_INDIRECT}
   PROPERTIES VERSION ${scs_VERSION} PUBLIC_HEADER
                                     "${${PROJECT_NAME}_PUBLIC_HDR}")
```

### Comparing `scs-3.2.4.post1/scs_source/LICENSE.txt` & `scs-3.2.4.post2/scs_source/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/Makefile` & `scs-3.2.4.post2/scs_source/Makefile`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/README.md` & `scs-3.2.4.post2/scs_source/README.md`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/cmake/AddInstallRPATHSupport.cmake` & `scs-3.2.4.post2/scs_source/cmake/AddInstallRPATHSupport.cmake`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/cmake/AddUninstallTarget.cmake` & `scs-3.2.4.post2/scs_source/cmake/AddUninstallTarget.cmake`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/cmake/InstallBasicPackageFiles.cmake` & `scs-3.2.4.post2/scs_source/cmake/InstallBasicPackageFiles.cmake`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/Doxyfile` & `scs-3.2.4.post2/scs_source/docs/src/Doxyfile`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/Makefile` & `scs-3.2.4.post2/scs_source/docs/src/Makefile`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/_static/css/scs_theme.css` & `scs-3.2.4.post2/scs_source/docs/src/_static/css/scs_theme.css`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/_static/favicon.ico` & `scs-3.2.4.post2/scs_source/docs/src/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/_static/scs_logo.png` & `scs-3.2.4.post2/scs_source/docs/src/_static/scs_logo.png`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/_static/scs_logo_transparent.png` & `scs-3.2.4.post2/scs_source/docs/src/_static/scs_logo_transparent.png`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/acceleration.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/acceleration.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/equilibration.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/equilibration.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/relaxation.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/relaxation.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/scale.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/scale.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/algorithm/warm_start.rst` & `scs-3.2.4.post2/scs_source/docs/src/algorithm/warm_start.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/c.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/c.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/compile_flags.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/compile_flags.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/cones.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/cones.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/exit_flags.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/exit_flags.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/info.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/info.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/matlab.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/matlab.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/matrices.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/matrices.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/python.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/python.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/r.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/r.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/api/settings.rst` & `scs-3.2.4.post2/scs_source/docs/src/api/settings.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/blas_lapack/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/blas_lapack/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/citing/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/citing/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
       .. code:: latex
 
         @misc{scs,
             author       = {Brendan O'Donoghue and Eric Chu and Neal Parikh and Stephen Boyd},
             title        = {{SCS}: Splitting Conic Solver, version 3.2.4},
             howpublished = {\url{https://github.com/cvxgrp/scs}},
             month        = nov,
-            year         = 2022
+            year         = 2023
         }
 
   Anderson Acceleration
      The acceleration scheme we use is described in the `paper <https://web.stanford.edu/~boyd/papers/nonexp_global_aa1.html>`__.
 
       .. code:: latex
```

### Comparing `scs-3.2.4.post1/scs_source/docs/src/conf.py` & `scs-3.2.4.post2/scs_source/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/contributing/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/contributing/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/c.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/c.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/julia.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/julia.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.py` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.py.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.py.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/entropy.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/entropy.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.py` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.py.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.py.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/lasso.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/lasso.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.py` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.py.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.py.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mat_completion.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mat_completion.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.py` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.py.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.py.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/mpc.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/mpc.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/qp.py` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/qp.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/python/qp.py.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/python/qp.py.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/qp.c` & `scs-3.2.4.post2/scs_source/docs/src/examples/qp.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/qp.c.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/qp.c.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/qp.m` & `scs-3.2.4.post2/scs_source/docs/src/examples/qp.m`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/qp.m.out` & `scs-3.2.4.post2/scs_source/docs/src/examples/qp.m.out`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/qp.prob` & `scs-3.2.4.post2/scs_source/docs/src/examples/qp.prob`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/examples/r.rst` & `scs-3.2.4.post2/scs_source/docs/src/examples/r.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/files/windows1.png` & `scs-3.2.4.post2/scs_source/docs/src/files/windows1.png`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/files/windows2.png` & `scs-3.2.4.post2/scs_source/docs/src/files/windows2.png`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/files/windows3.png` & `scs-3.2.4.post2/scs_source/docs/src/files/windows3.png`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/help/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/help/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/install/c.rst` & `scs-3.2.4.post2/scs_source/docs/src/install/c.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/install/python.rst` & `scs-3.2.4.post2/scs_source/docs/src/install/python.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/linear_solver/index.rst` & `scs-3.2.4.post2/scs_source/docs/src/linear_solver/index.rst`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/docs/src/make.bat` & `scs-3.2.4.post2/scs_source/docs/src/make.bat`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/aa.h` & `scs-3.2.4.post2/scs_source/include/aa.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/cones.h` & `scs-3.2.4.post2/scs_source/include/cones.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/ctrlc.h` & `scs-3.2.4.post2/scs_source/include/ctrlc.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/glbopts.h` & `scs-3.2.4.post2/scs_source/include/glbopts.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/linalg.h` & `scs-3.2.4.post2/scs_source/include/linalg.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/linsys.h` & `scs-3.2.4.post2/scs_source/include/linsys.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/rw.h` & `scs-3.2.4.post2/scs_source/include/rw.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/scs.h` & `scs-3.2.4.post2/scs_source/include/scs.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/scs_blas.h` & `scs-3.2.4.post2/scs_source/include/scs_blas.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/scs_types.h` & `scs-3.2.4.post2/scs_source/include/scs_types.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/scs_work.h` & `scs-3.2.4.post2/scs_source/include/scs_work.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/include/util.h` & `scs-3.2.4.post2/scs_source/include/util.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/cpu/direct/private.c` & `scs-3.2.4.post2/scs_source/linsys/cpu/direct/private.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/cpu/direct/private.h` & `scs-3.2.4.post2/scs_source/linsys/cpu/direct/private.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/cpu/indirect/private.c` & `scs-3.2.4.post2/scs_source/linsys/cpu/indirect/private.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/cpu/indirect/private.h` & `scs-3.2.4.post2/scs_source/linsys/cpu/indirect/private.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/csparse.c` & `scs-3.2.4.post2/scs_source/linsys/csparse.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/csparse.h` & `scs-3.2.4.post2/scs_source/linsys/csparse.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/LICENSE.txt` & `scs-3.2.4.post2/scs_source/linsys/external/amd/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/SuiteSparse_config.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/SuiteSparse_config.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/SuiteSparse_config.h` & `scs-3.2.4.post2/scs_source/linsys/external/amd/SuiteSparse_config.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd.h` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_1.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_1.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_2.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_2.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_aat.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_aat.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_control.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_control.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_defaults.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_defaults.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_dump.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_dump.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_global.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_global.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_info.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_info.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_internal.h` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_internal.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_order.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_order.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_post_tree.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_post_tree.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_postorder.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_postorder.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_preprocess.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_preprocess.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/amd_valid.c` & `scs-3.2.4.post2/scs_source/linsys/external/amd/amd_valid.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/amd/changes` & `scs-3.2.4.post2/scs_source/linsys/external/amd/changes`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/qdldl/LICENSE` & `scs-3.2.4.post2/scs_source/linsys/external/qdldl/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/qdldl/README.md` & `scs-3.2.4.post2/scs_source/linsys/external/qdldl/README.md`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl.c` & `scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl.h` & `scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/external/qdldl/qdldl_types.h` & `scs-3.2.4.post2/scs_source/linsys/external/qdldl/qdldl_types.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/gpu/gpu.c` & `scs-3.2.4.post2/scs_source/linsys/gpu/gpu.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/gpu/gpu.h` & `scs-3.2.4.post2/scs_source/linsys/gpu/gpu.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/gpu/indirect/private.c` & `scs-3.2.4.post2/scs_source/linsys/gpu/indirect/private.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/gpu/indirect/private.h` & `scs-3.2.4.post2/scs_source/linsys/gpu/indirect/private.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/mkl/direct/private.c` & `scs-3.2.4.post2/scs_source/linsys/mkl/direct/private.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/mkl/direct/private.h` & `scs-3.2.4.post2/scs_source/linsys/mkl/direct/private.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/scs_matrix.c` & `scs-3.2.4.post2/scs_source/linsys/scs_matrix.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/linsys/scs_matrix.h` & `scs-3.2.4.post2/scs_source/linsys/scs_matrix.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/scs.mk` & `scs-3.2.4.post2/scs_source/scs.mk`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/aa.c` & `scs-3.2.4.post2/scs_source/src/aa.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/cones.c` & `scs-3.2.4.post2/scs_source/src/cones.c`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
   }
   return tmp;
 }
 
 static scs_int set_up_sd_cone_work_space(ScsConeWork *c, const ScsCone *k) {
   scs_int i;
 #ifdef USE_LAPACK
-  blas_int n_max = 0;
+  blas_int n_max = 1;
   blas_int neg_one = -1;
   blas_int info = 0;
   scs_float wkopt = 0.0;
 #if VERBOSITY > 0
 #define _STR_EXPAND(tok) #tok
 #define _STR(tok) _STR_EXPAND(tok)
   scs_printf("BLAS(func) = '%s'\n", _STR(BLAS(func)));
@@ -352,15 +352,15 @@
 
   /* workspace query */
   BLAS(syev)
   ("Vectors", "Lower", &n_max, c->Xs, &n_max, SCS_NULL, &wkopt, &neg_one,
    &info);
 
   if (info != 0) {
-    scs_printf("FATAL: syev failure, info = %li\n", (long)info);
+    scs_printf("FATAL: syev workspace query failure, info = %li\n", (long)info);
     return -1;
   }
   c->lwork = (blas_int)(wkopt + 1); /* +1 for int casting safety */
   c->work = (scs_float *)scs_calloc(c->lwork, sizeof(scs_float));
 
   if (!c->Xs || !c->Z || !c->e || !c->work) {
     return -1;
```

### Comparing `scs-3.2.4.post1/scs_source/src/ctrlc.c` & `scs-3.2.4.post2/scs_source/src/ctrlc.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/exp_cone.c` & `scs-3.2.4.post2/scs_source/src/exp_cone.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/linalg.c` & `scs-3.2.4.post2/scs_source/src/linalg.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/normalize.c` & `scs-3.2.4.post2/scs_source/src/normalize.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/rw.c` & `scs-3.2.4.post2/scs_source/src/rw.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/scs.c` & `scs-3.2.4.post2/scs_source/src/scs.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/src/util.c` & `scs-3.2.4.post2/scs_source/src/util.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/minunit.h` & `scs-3.2.4.post2/scs_source/test/minunit.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problem_utils.h` & `scs-3.2.4.post2/scs_source/test/problem_utils.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/degenerate.h` & `scs-3.2.4.post2/scs_source/test/problems/degenerate.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/hs21_tiny_qp.h` & `scs-3.2.4.post2/scs_source/test/problems/hs21_tiny_qp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/hs21_tiny_qp_rw.h` & `scs-3.2.4.post2/scs_source/test/problems/hs21_tiny_qp_rw.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/infeasible_tiny_qp.h` & `scs-3.2.4.post2/scs_source/test/problems/infeasible_tiny_qp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/max_ent` & `scs-3.2.4.post2/scs_source/test/problems/max_ent`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/qafiro_tiny_qp.h` & `scs-3.2.4.post2/scs_source/test/problems/qafiro_tiny_qp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/random_prob` & `scs-3.2.4.post2/scs_source/test/problems/random_prob`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/rob_gauss_cov_est.h` & `scs-3.2.4.post2/scs_source/test/problems/rob_gauss_cov_est.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/small_lp.h` & `scs-3.2.4.post2/scs_source/test/problems/small_lp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/small_qp.h` & `scs-3.2.4.post2/scs_source/test/problems/small_qp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/test_exp_cone.h` & `scs-3.2.4.post2/scs_source/test/problems/test_exp_cone.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/test_prob_from_data_file.h` & `scs-3.2.4.post2/scs_source/test/problems/test_prob_from_data_file.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/test_validation.h` & `scs-3.2.4.post2/scs_source/test/problems/test_validation.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/problems/unbounded_tiny_qp.h` & `scs-3.2.4.post2/scs_source/test/problems/unbounded_tiny_qp.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/random_socp_prob.c` & `scs-3.2.4.post2/scs_source/test/random_socp_prob.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/rng.h` & `scs-3.2.4.post2/scs_source/test/rng.h`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/run_from_file.c` & `scs-3.2.4.post2/scs_source/test/run_from_file.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/scs_source/test/run_tests.c` & `scs-3.2.4.post2/scs_source/test/run_tests.c`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/gen_random_cone_prob.py` & `scs-3.2.4.post2/test/gen_random_cone_prob.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/solve_random_cone_prob.py` & `scs-3.2.4.post2/test/solve_random_cone_prob.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/test_scs_basic.py` & `scs-3.2.4.post2/test/test_scs_basic.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/test_scs_object.py` & `scs-3.2.4.post2/test/test_scs_object.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/test_scs_rand.py` & `scs-3.2.4.post2/test/test_scs_rand.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/test_scs_sdp.py` & `scs-3.2.4.post2/test/test_scs_sdp.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/test/test_solve_random_cone_prob.py` & `scs-3.2.4.post2/test/test_solve_random_cone_prob.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         np.linalg.norm(data["A"] @ x - data["b"] + s), 1e-3
     )
     np.testing.assert_array_less(
         np.linalg.norm(data["A"].T @ y + data["c"]), 1e-3
     )
     np.testing.assert_almost_equal(s.T @ y, 0.0)
     np.testing.assert_almost_equal(s, tools.proj_cone(s, K), decimal=4)
-    np.testing.assert_almost_equal(y, tools.proj_dual_cone(y, K), decimal=4)
+    np.testing.assert_almost_equal(y, tools.proj_dual_cone(y, K), decimal=3)
 
 
 @pytest.mark.parametrize("use_indirect,gpu", flags)
 def test_solve_infeasible(use_indirect, gpu):
     data = tools.gen_infeasible(K, n=m // 2)
     solver = scs.SCS(data, K, use_indirect=use_indirect, gpu=gpu, **params)
     sol = solver.solve()
```

### Comparing `scs-3.2.4.post1/test/test_solve_random_cone_prob_mkl.py` & `scs-3.2.4.post2/test/test_solve_random_cone_prob_mkl.py`

 * *Files identical despite different names*

### Comparing `scs-3.2.4.post1/PKG-INFO` & `scs-3.2.4.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs
-Version: 3.2.4.post1
+Version: 3.2.4.post2
 Summary: Splitting conic solver
 Author-Email: Brendan O'Donoghue <bodonoghue85@gmail.com>
 License: MIT License
         
         Copyright (c) 2017 Brendan O'Donoghue
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

