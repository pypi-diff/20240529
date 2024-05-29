# Comparing `tmp/xcoll-0.3.6.tar.gz` & `tmp/xcoll-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcoll-0.3.6.tar", max compression
+gzip compressed data, was "xcoll-0.4.0.tar", max compression
```

## Comparing `xcoll-0.3.6.tar` & `xcoll-0.4.0.tar`

### file list

```diff
@@ -1,109 +1,124 @@
--rw-r--r--   0        0        0    11357 2024-03-03 12:36:30.690976 xcoll-0.3.6/LICENSE
--rw-r--r--   0        0        0       74 2024-03-03 12:36:30.690976 xcoll-0.3.6/NOTICE
--rw-r--r--   0        0        0     1713 2024-03-03 12:36:30.690976 xcoll-0.3.6/README.md
--rw-r--r--   0        0        0      996 2024-05-02 14:27:33.660461 xcoll-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      642 2024-05-02 14:14:15.108567 xcoll-0.3.6/xcoll/__init__.py
--rw-r--r--   0        0        0      776 2024-05-02 14:14:15.108567 xcoll-0.3.6/xcoll/beam_elements/__init__.py
--rw-r--r--   0        0        0     1260 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/absorber.py
--rw-r--r--   0        0        0    15785 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/base.py
--rw-r--r--   0        0        0     5502 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/absorber.h
--rw-r--r--   0        0        0     5596 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_block.h
--rw-r--r--   0        0        0     6296 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_collimator.h
--rw-r--r--   0        0        0     5164 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_crystal.h
--rw-r--r--   0        0        0    11369 2024-05-02 14:14:15.109567 xcoll-0.3.6/xcoll/beam_elements/everest.py
--rw-r--r--   0        0        0    49476 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/colldb.py
--rw-r--r--   0        0        0    17015 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/collimator_settings.py
--rw-r--r--   0        0        0      525 2024-05-02 14:27:33.660461 xcoll-0.3.6/xcoll/general.py
--rw-r--r--   0        0        0     1586 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/headers/checks.h
--rw-r--r--   0        0        0      844 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/headers/particle_states.h
--rw-r--r--   0        0        0       39 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/__init__.py
--rw-r--r--   0        0        0     3953 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/impacts.py
--rw-r--r--   0        0        0     5950 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/impacts_src/impacts.h
--rw-r--r--   0        0        0     2493 2024-05-02 14:14:15.110567 xcoll-0.3.6/xcoll/impacts/interaction_types.py
--rw-r--r--   0        0        0    45052 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/manager.py
--rw-r--r--   0        0        0     8936 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/rf_sweep.py
--rw-r--r--   0        0        0      286 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/everest/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-29 13:36:30.200438 xcoll-0.3.6/xcoll/scattering_routines/everest/constants.h
--rw-r--r--   0        0        0    54119 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/crystal.h
--rw-r--r--   0        0        0     3743 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/everest.h
--rw-r--r--   0        0        0     1306 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/everest.py
--rw-r--r--   0        0        0     7308 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/jaw.h
--rw-r--r--   0        0        0     9410 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/everest/materials.py
--rw-r--r--   0        0        0     4518 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h
--rw-r--r--   0        0        0     6585 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/everest/properties.h
--rw-r--r--   0        0        0     6333 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/scatter.h
--rw-r--r--   0        0        0     9455 2024-05-02 14:14:15.111567 xcoll-0.3.6/xcoll/scattering_routines/everest/scatter_crystal.h
--rw-r--r--   0        0        0     2270 2024-04-29 13:36:30.199438 xcoll-0.3.6/xcoll/scattering_routines/fluka/build_fluka_input.py
--rw-r--r--   0        0        0       73 2024-03-02 17:23:41.394367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/.git
--rw-r--r--   0        0        0       12 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/.gitignore
--rw-r--r--   0        0        0      591 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt
--rw-r--r--   0        0        0     5951 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile
--rw-r--r--   0        0        0     3404 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/Makefile
--rw-r--r--   0        0        0      611 2024-03-02 17:23:41.402367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/README
--rw-r--r--   0        0        0    65455 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile
--rw-r--r--   0        0        0    45517 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc
--rw-r--r--   0        0        0   138089 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub
--rw-r--r--   0        0        0    74567 2024-03-02 17:23:41.403367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html
--rw-r--r--   0        0        0   233955 2024-03-02 17:23:41.404367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf
--rw-r--r--   0        0        0    36021 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png
--rw-r--r--   0        0        0     2904 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png
--rw-r--r--   0        0        0    23826 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png
--rw-r--r--   0        0        0     3956 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png
--rw-r--r--   0        0        0     7017 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png
--rw-r--r--   0        0        0    33614 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png
--rw-r--r--   0        0        0    51182 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png
--rw-r--r--   0        0        0      146 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Makefile
--rw-r--r--   0        0        0    74068 2024-03-02 17:23:41.405367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl
--rw-r--r--   0        0        0     2793 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Connection.h
--rw-r--r--   0        0        0     1976 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h
--rw-r--r--   0        0        0      757 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h
--rw-r--r--   0        0        0     5954 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h
--rw-r--r--   0        0        0     1731 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Message.h
--rw-r--r--   0        0        0     1328 2024-04-29 13:36:30.201439 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h
--rw-r--r--   0        0        0    82884 2024-03-02 17:23:41.756364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a
--rwxr-xr-x   0        0        0    66688 2024-03-02 17:23:41.780364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so
--rw-r--r--   0        0        0     2907 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c
--rw-r--r--   0        0        0     2330 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c
--rw-r--r--   0        0        0     3629 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f
--rw-r--r--   0        0        0     2995 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f
--rw-r--r--   0        0        0     5769 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.c
--rw-r--r--   0        0        0     5882 2024-03-02 17:23:41.434367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.d
--rw-r--r--   0        0        0    13008 2024-03-02 17:23:41.473366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.o
--rw-r--r--   0        0        0     4804 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c
--rw-r--r--   0        0        0     3829 2024-03-02 17:23:41.487366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d
--rw-r--r--   0        0        0    12440 2024-03-02 17:23:41.517366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o
--rw-r--r--   0        0        0     1541 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c
--rw-r--r--   0        0        0     2445 2024-03-02 17:23:41.529366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d
--rw-r--r--   0        0        0      288 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.h
--rw-r--r--   0        0        0     7664 2024-03-02 17:23:41.549366 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o
--rw-r--r--   0        0        0     1925 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c
--rw-r--r--   0        0        0     5905 2024-03-02 17:23:41.566365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d
--rw-r--r--   0        0        0     7536 2024-03-02 17:23:41.597365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o
--rw-r--r--   0        0        0      396 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer_private.h
--rw-r--r--   0        0        0      421 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO_private.h
--rw-r--r--   0        0        0    11512 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c
--rw-r--r--   0        0        0     3240 2024-03-02 17:23:41.610365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d
--rw-r--r--   0        0        0    23400 2024-03-02 17:23:41.654365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o
--rw-r--r--   0        0        0     6361 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c
--rw-r--r--   0        0        0     5716 2024-03-02 17:23:41.671365 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d
--rw-r--r--   0        0        0      902 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h
--rw-r--r--   0        0        0    16816 2024-03-02 17:23:41.710364 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o
--rw-r--r--   0        0        0    14484 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/tags
--rw-r--r--   0        0        0      166 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/AllTests.cpp
--rw-r--r--   0        0        0      152 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/CommonTest.h
--rw-r--r--   0        0        0     2464 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp
--rw-r--r--   0        0        0     1851 2024-03-02 17:23:41.406367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp
--rw-r--r--   0        0        0    11293 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp
--rw-r--r--   0        0        0    14331 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp
--rw-r--r--   0        0        0      526 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c
--rw-r--r--   0        0        0      226 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.h
--rw-r--r--   0        0        0     2244 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c
--rw-r--r--   0        0        0     1660 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h
--rw-r--r--   0        0        0      549 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c
--rw-r--r--   0        0        0      395 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.h
--rw-r--r--   0        0        0      360 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.c
--rw-r--r--   0        0        0      280 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.h
--rw-r--r--   0        0        0      330 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFortranFlukaIO.h
--rw-r--r--   0        0        0     1452 2024-03-02 17:23:41.407367 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c
--rw-r--r--   0        0        0      906 2024-04-29 13:36:30.202438 xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h
--rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 xcoll-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-03 12:36:30.690976 xcoll-0.4.0/LICENSE
+-rw-r--r--   0        0        0       74 2024-03-03 12:36:30.690976 xcoll-0.4.0/NOTICE
+-rw-r--r--   0        0        0     1713 2024-03-03 12:36:30.690976 xcoll-0.4.0/README.md
+-rw-r--r--   0        0        0      996 2024-05-29 00:59:12.034854 xcoll-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      929 2024-05-29 00:59:12.655848 xcoll-0.4.0/xcoll/__init__.py
+-rw-r--r--   0        0        0      981 2024-05-29 00:59:12.655848 xcoll-0.4.0/xcoll/beam_elements/__init__.py
+-rw-r--r--   0        0        0     2508 2024-05-29 00:59:12.656848 xcoll-0.4.0/xcoll/beam_elements/absorber.py
+-rw-r--r--   0        0        0    49646 2024-05-29 00:59:12.656848 xcoll-0.4.0/xcoll/beam_elements/base.py
+-rw-r--r--   0        0        0     4478 2024-05-29 00:59:12.656848 xcoll-0.4.0/xcoll/beam_elements/collimators_src/black_absorber.h
+-rw-r--r--   0        0        0     4082 2024-05-29 00:59:12.657848 xcoll-0.4.0/xcoll/beam_elements/collimators_src/black_crystal.h
+-rw-r--r--   0        0        0     5970 2024-05-29 00:59:12.657848 xcoll-0.4.0/xcoll/beam_elements/collimators_src/everest_block.h
+-rw-r--r--   0        0        0     9857 2024-05-29 00:59:12.657848 xcoll-0.4.0/xcoll/beam_elements/collimators_src/everest_collimator.h
+-rw-r--r--   0        0        0    11822 2024-05-29 00:59:12.657848 xcoll-0.4.0/xcoll/beam_elements/collimators_src/everest_crystal.h
+-rw-r--r--   0        0        0     8405 2024-05-29 00:59:12.657848 xcoll-0.4.0/xcoll/beam_elements/everest.py
+-rw-r--r--   0        0        0    29822 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/colldb.py
+-rw-r--r--   0        0        0      525 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/general.py
+-rw-r--r--   0        0        0     1582 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/headers/checks.h
+-rw-r--r--   0        0        0      840 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/headers/particle_states.h
+-rw-r--r--   0        0        0     7858 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/initial_distribution.py
+-rw-r--r--   0        0        0     7552 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/install.py
+-rw-r--r--   0        0        0       50 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/interaction_record/__init__.py
+-rw-r--r--   0        0        0    10733 2024-05-29 00:59:12.658848 xcoll-0.4.0/xcoll/interaction_record/interaction_record.py
+-rw-r--r--   0        0        0     5949 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/interaction_record/interaction_record_src/interaction_record.h
+-rw-r--r--   0        0        0     2894 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/interaction_record/interaction_types.py
+-rw-r--r--   0        0        0     3250 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/line_tools.py
+-rw-r--r--   0        0        0     7486 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/lossmap.py
+-rw-r--r--   0        0        0      343 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/manager.py
+-rw-r--r--   0        0        0     8936 2024-05-29 00:59:12.659848 xcoll-0.4.0/xcoll/rf_sweep.py
+-rw-r--r--   0        0        0      286 2024-05-28 10:15:09.965053 xcoll-0.4.0/xcoll/scattering_routines/everest/__init__.py
+-rw-r--r--   0        0        0    10424 2024-05-29 00:59:12.660848 xcoll-0.4.0/xcoll/scattering_routines/everest/amorphous.h
+-rw-r--r--   0        0        0    11313 2024-05-29 00:59:12.660848 xcoll-0.4.0/xcoll/scattering_routines/everest/channeling.h
+-rw-r--r--   0        0        0     1390 2024-05-23 14:28:17.563372 xcoll-0.4.0/xcoll/scattering_routines/everest/constants.h
+-rw-r--r--   0        0        0     5416 2024-05-29 00:59:12.660848 xcoll-0.4.0/xcoll/scattering_routines/everest/crystal_parameters.h
+-rw-r--r--   0        0        0     2658 2024-05-29 00:59:12.660848 xcoll-0.4.0/xcoll/scattering_routines/everest/everest.h
+-rw-r--r--   0        0        0     1460 2024-05-29 00:59:12.660848 xcoll-0.4.0/xcoll/scattering_routines/everest/everest.py
+-rw-r--r--   0        0        0     2270 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/everest/jaw.h
+-rw-r--r--   0        0        0     9524 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/everest/materials.py
+-rw-r--r--   0        0        0     5400 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/everest/multiple_coulomb_scattering.h
+-rw-r--r--   0        0        0     3113 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/everest/nuclear_interaction.h
+-rw-r--r--   0        0        0     6585 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/everest/properties.h
+-rw-r--r--   0        0        0     2270 2024-05-28 10:15:09.966054 xcoll-0.4.0/xcoll/scattering_routines/fluka/build_fluka_input.py
+-rw-r--r--   0        0        0       73 2024-03-02 17:23:41.394367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/.git
+-rw-r--r--   0        0        0       12 2024-03-02 17:23:41.402367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/.gitignore
+-rw-r--r--   0        0        0      591 2024-03-02 17:23:41.402367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt
+-rw-r--r--   0        0        0     5951 2024-03-02 17:23:41.402367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile
+-rw-r--r--   0        0        0     3404 2024-03-02 17:23:41.402367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/Makefile
+-rw-r--r--   0        0        0      611 2024-03-02 17:23:41.402367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/README
+-rw-r--r--   0        0        0    65455 2024-03-02 17:23:41.403367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile
+-rw-r--r--   0        0        0    45517 2024-03-02 17:23:41.403367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc
+-rw-r--r--   0        0        0   138089 2024-03-02 17:23:41.403367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub
+-rw-r--r--   0        0        0    74567 2024-03-02 17:23:41.403367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html
+-rw-r--r--   0        0        0   233955 2024-03-02 17:23:41.404367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf
+-rw-r--r--   0        0        0    36021 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png
+-rw-r--r--   0        0        0     2904 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png
+-rw-r--r--   0        0        0    23826 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png
+-rw-r--r--   0        0        0     3956 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png
+-rw-r--r--   0        0        0     7017 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png
+-rw-r--r--   0        0        0    33614 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png
+-rw-r--r--   0        0        0    51182 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png
+-rw-r--r--   0        0        0      146 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/Makefile
+-rw-r--r--   0        0        0    74068 2024-03-02 17:23:41.405367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl
+-rw-r--r--   0        0        0     2793 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/Connection.h
+-rw-r--r--   0        0        0     1976 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h
+-rw-r--r--   0        0        0      757 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h
+-rw-r--r--   0        0        0     5954 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h
+-rw-r--r--   0        0        0     1731 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/Message.h
+-rw-r--r--   0        0        0     1328 2024-05-23 14:28:17.564372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h
+-rw-r--r--   0        0        0    82884 2024-03-02 17:23:41.756364 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a
+-rwxr-xr-x   0        0        0    66688 2024-03-02 17:23:41.780364 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so
+-rw-r--r--   0        0        0     2907 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c
+-rw-r--r--   0        0        0     2330 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c
+-rw-r--r--   0        0        0     3629 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f
+-rw-r--r--   0        0        0     2995 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f
+-rw-r--r--   0        0        0     5769 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.c
+-rw-r--r--   0        0        0     5882 2024-03-02 17:23:41.434367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.d
+-rw-r--r--   0        0        0    13008 2024-03-02 17:23:41.473366 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.o
+-rw-r--r--   0        0        0     4804 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c
+-rw-r--r--   0        0        0     3829 2024-03-02 17:23:41.487366 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d
+-rw-r--r--   0        0        0    12440 2024-03-02 17:23:41.517366 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o
+-rw-r--r--   0        0        0     1541 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c
+-rw-r--r--   0        0        0     2445 2024-03-02 17:23:41.529366 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d
+-rw-r--r--   0        0        0      288 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.h
+-rw-r--r--   0        0        0     7664 2024-03-02 17:23:41.549366 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o
+-rw-r--r--   0        0        0     1925 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c
+-rw-r--r--   0        0        0     5905 2024-03-02 17:23:41.566365 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d
+-rw-r--r--   0        0        0     7536 2024-03-02 17:23:41.597365 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o
+-rw-r--r--   0        0        0      396 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer_private.h
+-rw-r--r--   0        0        0      421 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO_private.h
+-rw-r--r--   0        0        0    11512 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c
+-rw-r--r--   0        0        0     3240 2024-03-02 17:23:41.610365 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d
+-rw-r--r--   0        0        0    23400 2024-03-02 17:23:41.654365 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o
+-rw-r--r--   0        0        0     6361 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c
+-rw-r--r--   0        0        0     5716 2024-03-02 17:23:41.671365 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d
+-rw-r--r--   0        0        0      902 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h
+-rw-r--r--   0        0        0    16816 2024-03-02 17:23:41.710364 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o
+-rw-r--r--   0        0        0    14484 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/tags
+-rw-r--r--   0        0        0      166 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/AllTests.cpp
+-rw-r--r--   0        0        0      152 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/CommonTest.h
+-rw-r--r--   0        0        0     2464 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp
+-rw-r--r--   0        0        0     1851 2024-03-02 17:23:41.406367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp
+-rw-r--r--   0        0        0    11293 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp
+-rw-r--r--   0        0        0    14331 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp
+-rw-r--r--   0        0        0      526 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c
+-rw-r--r--   0        0        0      226 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.h
+-rw-r--r--   0        0        0     2244 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c
+-rw-r--r--   0        0        0     1660 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h
+-rw-r--r--   0        0        0      549 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c
+-rw-r--r--   0        0        0      395 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.h
+-rw-r--r--   0        0        0      360 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.c
+-rw-r--r--   0        0        0      280 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOServer.h
+-rw-r--r--   0        0        0      330 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFortranFlukaIO.h
+-rw-r--r--   0        0        0     1452 2024-03-02 17:23:41.407367 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c
+-rw-r--r--   0        0        0      906 2024-05-23 14:28:17.565372 xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h
+-rw-r--r--   0        0        0      221 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/geometry/__init__.py
+-rw-r--r--   0        0        0     7887 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/geometry/collimator_geometry.h
+-rw-r--r--   0        0        0     4887 2024-05-29 00:59:12.661848 xcoll-0.4.0/xcoll/scattering_routines/geometry/crystal_geometry.h
+-rw-r--r--   0        0        0     1102 2024-05-29 00:59:12.662848 xcoll-0.4.0/xcoll/scattering_routines/geometry/geometry.py
+-rw-r--r--   0        0        0     2947 2024-05-29 00:59:12.662848 xcoll-0.4.0/xcoll/scattering_routines/geometry/get_s.h
+-rw-r--r--   0        0        0     3747 2024-05-29 00:59:12.662848 xcoll-0.4.0/xcoll/scattering_routines/geometry/methods.h
+-rw-r--r--   0        0        0     5499 2024-05-29 00:59:12.662848 xcoll-0.4.0/xcoll/scattering_routines/geometry/objects.h
+-rw-r--r--   0        0        0      701 2024-05-29 00:59:12.663848 xcoll-0.4.0/xcoll/scattering_routines/geometry/rotation.h
+-rw-r--r--   0        0        0     7667 2024-05-29 00:59:12.663848 xcoll-0.4.0/xcoll/scattering_routines/geometry/segments.h
+-rw-r--r--   0        0        0     5763 2024-05-29 00:59:12.663848 xcoll-0.4.0/xcoll/scattering_routines/geometry/sort.h
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 xcoll-0.4.0/PKG-INFO
```

### Comparing `xcoll-0.3.6/LICENSE` & `xcoll-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/README.md` & `xcoll-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/pyproject.toml` & `xcoll-0.4.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcoll"
-version = "0.3.6"
+version = "0.4.0"
 description = "Xsuite collimation package"
 homepage = "https://github.com/xsuite/xcoll"
 repository = "https://github.com/xsuite/xcoll"
 authors = [
            "Frederik F. Van der Veken <frederik@cern.ch>",
            "Despina Demetriadou <despina.demetriadou@cern.ch>",
            "Andrey Abramov <andrey.abramov@cern.ch>",
```

### Comparing `xcoll-0.3.6/xcoll/beam_elements/collimators_src/everest_block.h` & `xcoll-0.4.0/xcoll/beam_elements/collimators_src/everest_block.h`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         coll->csref[5] = MaterialData_get_cross_section(material, 5);
         coll->only_mcs = MaterialData_get__only_mcs(material);
 
         // Impact table
         coll->record = EverestBlockData_getp_internal_record(el, part0);
         coll->record_index = NULL;
         if (coll->record){
-            coll->record_index = CollimatorImpactsData_getp__index(coll->record);
+            coll->record_index = InteractionRecordData_getp__index(coll->record);
         }
     }
 
     return coll;
 }
 
 
@@ -80,50 +80,62 @@
             Drift_single_particle(part, length);
 
         } else {
             // Check collimator initialisation
             int8_t is_valid = xcoll_check_particle_init(coll->rng, part);
 
             if (is_valid) {
-                EverestData everest     = EverestBlock_init_data(part, coll);
-                double const e0         = LocalParticle_get_energy0(part) / 1.e9;        // Reference energy in GeV
-                double const p0         = LocalParticle_get_p0c(part) / 1e9;            // Reference momentum in GeV
+                // Store s-location of start of block
+                double s_block = LocalParticle_get_s(part);
+                LocalParticle_set_s(part, 0);
+
+                // Store initial coordinates for updating later
+                double const e0         = LocalParticle_get_energy0(part);
+                double const p0         = LocalParticle_get_p0c(part);
+                double const ptau_in    = LocalParticle_get_ptau(part);
+                double const rvv_in     = LocalParticle_get_rvv(part);
+#ifdef XCOLL_USE_EXACT
+                double const xp_in      = LocalParticle_get_exact_xp(part);
+                double const yp_in      = LocalParticle_get_exact_yp(part);
+#else
+                double const xp_in      = LocalParticle_get_xp(part);
+                double const yp_in      = LocalParticle_get_yp(part);
+#endif
+                double const zeta_in    = LocalParticle_get_zeta(part);
                 double const mass_ratio = LocalParticle_get_charge_ratio(part) / LocalParticle_get_chi(part);   // m/m0
-                double energy = (LocalParticle_get_ptau(part)*p0 + e0) * mass_ratio;    // energy in GeV
-                int is_abs = 0;
-                double const rpp_in  = LocalParticle_get_rpp(part);
-                double const rvv_in  = LocalParticle_get_rvv(part);
-                double const px_in   = LocalParticle_get_px(part);
-                double const py_in   = LocalParticle_get_py(part);
-
-                double* result = jaw(everest, part, energy, length, 0);
-                energy = result[0];
-                if (result[1] == 1){ is_abs = 1; }
-                double s_out = result[2];
-                free(result);
+                double energy           = (p0*ptau_in + e0) * mass_ratio;
+
+                EverestData everest = EverestBlock_init_data(part, coll);
+                energy = jaw(everest, part, energy, length, 0);
                 free(everest);
 
-                double ptau_out = (energy/mass_ratio - e0) / p0;
-                LocalParticle_update_ptau(part, ptau_out);
-                if (is_abs==0){
-                    double px  = LocalParticle_get_px(part);
-                    double py  = LocalParticle_get_py(part);
+                LocalParticle_add_to_s(part, s_block);
+
+                LocalParticle_set_zeta(part, zeta_in);
+                // Survived particles need correcting:
+                if (LocalParticle_get_state(part)>0){
+                    // Update energy
+                    double ptau_out = (energy/mass_ratio - e0) / p0;
+                    LocalParticle_update_ptau(part, ptau_out);
+                    // Update zeta
+#ifdef XCOLL_USE_EXACT
+                    double xp  = LocalParticle_get_exact_xp(part);
+                    double yp  = LocalParticle_get_exact_yp(part);
+#else
+                    double xp  = LocalParticle_get_xp(part);
+                    double yp  = LocalParticle_get_yp(part);
+#endif
                     double rvv = LocalParticle_get_rvv(part);
-                    double rpp = LocalParticle_get_rpp(part);
                     // First we drift half the length with the old angles:
-                    LocalParticle_add_to_zeta(part, drift_zeta_single(rvv_in, px_in*rpp_in, py_in*rpp_in, length/2) );
+                    LocalParticle_add_to_zeta(part, drift_zeta_single(rvv_in, xp_in, yp_in, length/2) );
                     // then half the length with the new angles:
-                    LocalParticle_add_to_zeta(part, drift_zeta_single(rvv, px*rpp, py*rpp, length/2) );
-                } else {
-                    LocalParticle_set_s(part, s_out);
-                    LocalParticle_set_state(part, XC_LOST_ON_EVEREST_BLOCK);
+                    LocalParticle_add_to_zeta(part, drift_zeta_single(rvv, xp, yp, length/2) );
                 }
             }
         }
     //end_per_particle_block
-
     free(coll);
 }
 
 
 
 #endif /* XCOLL_EVEREST_BLOCK_H */
```

### Comparing `xcoll-0.3.6/xcoll/colldb.py` & `xcoll-0.4.0/xcoll/beam_elements/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,1110 +1,1324 @@
 # copyright ############################### #
 # This file is part of the Xcoll Package.   #
-# Copyright (c) CERN, 2023.                 #
+# Copyright (c) CERN, 2024.                 #
 # ######################################### #
 
-import io
-import json
 import numpy as np
-import pandas as pd
 
+import xobjects as xo
+import xtrack as xt
 
-#TODO: niet-active collimators op non-active etc (ook crystals)
+from ..interaction_record import InteractionRecord
+from ..general import _pkg_root
+from ..scattering_routines.geometry import XcollGeometry
 
-def load_SixTrack_colldb(filename, *, emit):
-    print("Warning: Using 'xcoll.load_SixTrack_colldb()' is deprecated! "
-        + "Use 'xcoll.CollimatorDatabase.from_SixTrack()' instead.")
-    return CollimatorDatabase.from_SixTrack(file=filename, nemitt_x=emit, nemitt_y=emit)
-
-
-def _initialise_None(collimator):
-    fields = {'s_center':None, 'align_to': None, 's_align_front': None, 's_align_back': None }
-    fields.update({'gap_L': None, 'gap_R': None, 'angle_L': 0, 'angle_R': 0, 'offset': 0, 'parking': 1})
-    fields.update({'jaw_LU': None, 'jaw_RU': None, 'jaw_LD': None, 'jaw_RD': None, 'family': None, 'overwritten_keys': []})
-    fields.update({'side': 'both', 'material': None, 'stage': None, 'collimator_type': None, 'active': True})
-    fields.update({'active_length': 0, 'inactive_front': 0, 'inactive_back': 0, 'sigmax': None, 'sigmay': None})
-    fields.update({'crystal': None, 'bending_radius': None, 'xdim': 0, 'ydim': 0, 'miscut': 0, 'thick': 0})
-    for f, val in fields.items():
-        if f not in collimator.keys():
-            collimator[f] = val
-    for key in collimator.keys():
-        if key not in fields.keys():
-            raise ValueError(f"Illegal setting {key} in collimator!")
-
-
-def _dict_keys_to_lower(dct):
-    if isinstance(dct, dict):
-        return {k.lower(): _dict_keys_to_lower(v) for k,v in dct.items()}
-    else:
-        return dct
-
-
-def _get_coll_dct_by_beam(coll, beam):
-    # The dictionary can be a CollimatorDatabase for a single beam (beam=None)
-    # or for both beams (beam='b1' or beam='b2)
-    if beam is not None:
-        if isinstance(beam, int) or len(beam) == 1:
-            beam = f'b{beam}'
-        beam = beam.lower()
-    beam_in_db = list(coll.keys())
-    
-    if beam_in_db == ['b1','b2']:
-        if beam is None:
-            raise ValueError("Need to specify a beam, because the given dict is for both beams!")
-        return coll[beam]
-
-    elif len(beam_in_db) == 1:
-        if beam is None:
-            beam = beam_in_db[0].lower()
-        elif beam != beam_in_db[0].lower():
-            raise ValueError("Variable 'beam' does not match beam specified in CollimatorDatabase!")
-        return coll[beam]
-
-    elif beam is not None:
-        print("Warning: Specified a beam, but the CollimatorDatabase is for a single beam only!")
-    return coll
-
-
-class CollimatorDatabase:
-
-    _init_vars = ['collimator_dict', 'family_dict', 'beam', 'nemitt_x', 'nemitt_y', '_yaml_merged', 'ignore_crystals']
-    _init_var_defaults = {'family_dict': {}, 'beam': None, '_yaml_merged': False, 'ignore_crystals': True}
-
-    # -------------------------------
-    # ------ Loading functions ------
-    # -------------------------------
-    
-    @classmethod
-    def from_yaml(cls, file, **kwargs):
-
-        # Only do the import here, as to not force people to install
-        # ruamel if they don't load CollimatorDatabase yaml's
-        from ruamel.yaml import YAML
-        yaml = YAML(typ='safe')
-        if isinstance(file, io.IOBase):
-            dct = yaml.load(file)
-        else:
-            with open(file, 'r') as fid:
-                dct = yaml.load(fid)
-        dct = _dict_keys_to_lower(dct)
-
-        # If the CollimatorDatabase uses YAML merging, we need a bit of hackery to get the
-        # family names from the tags (anchors/aliases)
-        _yaml_merged = False
-        if 'families' in dct.keys() and not isinstance(dct['families'], dict):
-            _yaml_merged = True
-
-            # First we load a round-trip yaml
-            yaml = YAML()
-            if isinstance(file, io.IOBase):
-                full_dct = yaml.load(file)
-            else:
-                with open(file, 'r') as fid:
-                    full_dct = yaml.load(fid)
-            famkey = [key for key in full_dct.keys() if key.lower() == 'families'][0]
-            collkey = [key for key in full_dct.keys() if key.lower() == 'collimators'][0]
-            families = {}
-
-            # We loop over family names to get the name tag ('anchor') of each family
-            for fam, full_fam in zip(dct['families'], full_dct[famkey]):
-                if full_fam.anchor.value is None:
-                    raise ValueError("Missing name tag / anchor in "
-                                   + "CollimatorDatabase['families']!")
-                # We get the anchor from the rt yaml, and use it as key in the families dict
-                families[full_fam.anchor.value.lower()] = {f.lower(): v for f, v in fam.items()}
-            dct['families'] = families
-
-            # Now we need to loop over each collimator, and verify which family was used
-            beam = kwargs.get('beam', None)
-            coll_dct = _get_coll_dct_by_beam(dct['collimators'], beam)
-            full_coll_dct = _get_coll_dct_by_beam(full_dct[collkey], beam)
-            for coll, full_coll in zip(coll_dct.values(), full_coll_dct.values()):
-                if 'family' in coll.keys():
-                    raise ValueError(f"Error in {coll}: Cannot use merging for families "
-                                    + "and manually specify family as well!")
-                elif len(full_coll.merge) > 0:
-                    coll['family'] = full_coll.merge[0][1].anchor.value.lower()
-                    # Check if some family settings are overwritten for this collimator
-                    overwritten_keys = [key.lower() for key in full_coll.keys()
-                                        if full_coll._unmerged_contains(key)
-                                        and key.lower() in families[coll['family']].keys()]
-                    if len(overwritten_keys) > 0:
-                        coll['overwritten_keys'] = overwritten_keys
-                else:
-                    coll['family'] = None
 
-        return cls.from_dict(dct, _yaml_merged=_yaml_merged, **kwargs)
+OPEN_JAW = 3.
+OPEN_GAP = 999.
 
 
-    @classmethod
-    def from_json(cls, file, **kwargs):
-        if isinstance(file, io.IOBase):
-            dct = json.load(file)
-        else:
-            with open(file, 'r') as fid:
-                dct = json.load(fid)
-        dct = _dict_keys_to_lower(dct)
-        return cls.from_dict(dct, **kwargs)
-
-
-    @classmethod
-    def from_dict(cls, dct, beam=None, _yaml_merged=False, nemitt_x=None, nemitt_y=None, ignore_crystals=True):
-        # We make all keys case-insensitive to avoid confusion between different conventions
-        # The families are optional
-        fam = {}
-        dct = _dict_keys_to_lower(dct)
-
-        # Get the emittance
-        if nemitt_x is None and nemitt_y is None:
-            if 'emittance' not in dct.keys():
-                raise ValueError("Missing emittance info! Add 'emittance' as a key to "
-                               + "the CollimatorDatabase file, or specify it as 'nemitt_x' "
-                               + "and 'nemitt_y' to the loader!")
-            nemitt_x = dct['emittance']['x']
-            nemitt_y = dct['emittance']['y']
-        elif nemitt_x is None or nemitt_y is None:
-            raise ValueError("Need to provide both 'nemitt_x' and 'nemitt_y'!")
-        elif 'emittance' in dct.keys():
-            if dct['emittance']['x'] != nemitt_x or dct['emittance']['y'] != nemitt_y:
-                raise ValueError("Emittance in CollimatorDatabase file different from "
-                               + "'nemitt_x' and 'nemitt_y'!")
-
-        # Get family and collimator dicts
-        if 'families' in dct.keys():
-            if not 'collimators' in dct.keys():
-                raise ValueError("Could not find 'collimators' dict in CollimatorDatabase!")
-            fam  = dct['families']
-            coll = dct['collimators']
-        elif 'collimators' in dct.keys():
-            coll = dct['collimators']
-        else:
-            coll = dct
+class InvalidXcoll(xt.BeamElement):
+    _xofields = {
+        'length': xo.Float64
+    }
 
-        return cls(collimator_dict=coll, family_dict=fam, nemitt_x=nemitt_x, nemitt_y=nemitt_y,
-                   beam=beam, _yaml_merged=_yaml_merged, ignore_crystals=ignore_crystals)
+    isthick = True
+    behaves_like_drift = True
+    allow_track = False
+    skip_in_loss_location_refinement = True
+    allow_loss_refinement = True
 
+    # InvalidXcoll catches unallowed cases, like backtracking through a collimator
+    _extra_c_sources = [
+        _pkg_root.joinpath('headers','particle_states.h'),
+        _pkg_root.joinpath('headers','checks.h')
+    ]
 
-    @classmethod
-    def from_SixTrack(cls, file, ignore_crystals=True, **kwargs):
-        # only import regex here
-        import re
-        with open(file, 'r') as infile:
-            coll_data_string = ''
-            family_settings = {}
-            family_types = {}
-            side = {}
-            cry_fields = ['bending_radius', 'xdim', 'ydim', 'thick', 'miscut', 'crystal']
-            cry = {}
-
-            for l_no, line in enumerate(infile):
-                if line.startswith('#'):
-                    continue # Comment
-                sline = line.split()
-                if len(sline) > 0:
-                    if sline[0].lower() == 'nsig_fam':
-                        family_settings[sline[1]] = float(sline[2])
-                        family_types[sline[1]] = sline[3]
-                    elif sline[0].lower() == 'onesided':
-                        side[sline[1]] = int(sline[2])
-                    elif sline[0].lower() == "crystal":
-                        cry[sline[1]] = {}
-                        for i, key in enumerate(cry_fields):
-                            idx = i+2 if i < 4 else i+3  # we skip "tilt"
-                            if i < 5:
-                                cry[sline[1]][key] = float(sline[idx])
-                            else:
-                                cry[sline[1]][key] = int(sline[idx])
-                    elif sline[0].lower() == 'settings':
-                        pass # Acknowledge and ignore this line
-                    elif len(sline) == 6:
-                        # Standard collimator definition
-                        coll_data_string += line
-                    else:
-                        print(f"Unknown setting {line}")
-
-        defaults = {}
-        _initialise_None(defaults)
-
-        famdct = {key: {'gap': family_settings[key], 'stage': family_types[key]} for key in family_settings}
-        names = ['name', 'gap', 'material', 'active_length', 'angle', 'offset']
-
-        df = pd.read_csv(io.StringIO(coll_data_string), sep=r'\s+', index_col=False, names=names)
-        df['family'] = df['gap'].copy()
-        df['family'] = df['family'].apply(lambda s: None if re.match(r'^-?\d+(\.\d+)?$', str(s)) else s)
-        df.insert(5,'stage', df['gap'].apply(lambda s: family_types.get(s, 'UNKNOWN')))
-
-        df['gap'] = df['gap'].apply(lambda s: float(family_settings.get(s, s)))
-        # TODO this breaks code if a key has upper case, e.g. gap_L
-        df['name'] = df['name'].str.lower() # Make the names lowercase for easy processing
-        df['parking'] = 0.025
-        if ignore_crystals:
-            df = df[~df.name.isin(list(cry.keys()))]
-        else:
-            for key in cry_fields:
-                df[key] = [cry[name][key] if name in cry else defaults[key]
-                           for name in df['name']]
-            df['crystal'] = ['strip' if s==1 else s for s in df['crystal']]
-            df['crystal'] = ['quasi-mosaic' if s==2 else s for s in df['crystal']]
-        df['side'] = [side[name] if name in side else defaults['side']
-                      for name in df['name']]
-        df['side'] = ['both'  if s==0 else s for s in df['side']]
-        df['side'] = ['left'  if s==1 else s for s in df['side']]
-        df['side'] = ['right' if s==2 else s for s in df['side']]
-        df = df.set_index('name')
-
-        return cls.from_dict({'collimators': df.transpose().to_dict(), 'families': famdct}, \
-                             ignore_crystals=ignore_crystals, **kwargs)
-
-
-    def write_to_yaml(self, out, lhc_style=True):
-        """
-        Writes a colldb in memory to disk in the yaml format.
-
-        > colldb_object.write_to_yaml(<path+name>, lhc_style=Bool)
-
-        if lhc_style == True, it will add comments assuming that the collimators are named
-        as in the lhc.
-
-        The function can dump b1, b2 and a general bx, however multi-beam functionality is not yet
-        added to the collmanager. TODO
-
-        If any of the dumped keys contains capital letters (e.g. gap_L), it will not be possible
-        to load it back into xcoll, since all keys are set to lowercase when importing TODO
-        """
-        # Dumps collimator database to a YAML file with optional LHC style formatting
-        import re
-
-        # Local helper functions
-        def _format_dict_entry(key, value, spacing='', mapping=False, key_width=15):
-            # Formats a dictionary entry into a string for YAML output
-            formatted_values = ',    '.join(f"{k}: {v}" for k, v in value.items())
-            formatted_values = re.sub(r'none', 'null', formatted_values, flags=re.IGNORECASE)
-            # Ensure key has a fixed width for alignment
-            if mapping:
-                formatted_key = f'{key}'.ljust(key_width)
-            else:
-                formatted_key = f'{key}:'.ljust(key_width)
-            #formatted_values = formatted_values.ljust(key_width)
-            return f"{spacing}{formatted_key} {{ {formatted_values} }}\n"
-        
-        def _print_values(keys, dct, file, spacing='', mapping=False):
-            # Writes formatted dictionary entries to a file
-            for key in keys:
-                file.write(_format_dict_entry(key, dct[key], spacing=spacing, mapping=mapping))
-        
-        def _print_colls(colls, dcts, beam, file):
-            # Filters and formats collimator data, then writes to a file
-            coll_items_to_print = ['<<','gap','angle','material','active','length','side']
-            file.write(f'  {beam}:\n')
-            for coll in colls:
-                coll_dict = dcts._colldb.transpose().to_dict()[coll]
-                fam = coll_dict['family']
-                fam_keys = []
-                if fam is not None:
-                    fam_keys = dcts._family_dict[fam].keys()
-                    coll_dict = {**{'<<': '*'+fam}, **coll_dict}
-                temp_items_to_print = []
-                if coll_dict['crystal'] and str(coll_dict['crystal'])!='nan':
-                    temp_items_to_print = ['bending_radius','xdim','ydim','miscut','crystal', 'thick']
-                if coll_dict['angle_L'] == coll_dict['angle_R']:
-                    coll_dict.update({'angle': coll_dict['angle_L']})
-                else:
-                    temp_items_to_print = temp_items_to_print + ['angle_L','angle_R']
-                if coll_dict['gap_L'] == coll_dict['gap_R']:
-                    coll_dict.update({'gap': coll_dict['gap_L']})
-                elif coll_dict['gap_L'] is None and coll_dict['gap_R'] is not None:
-                    coll_dict.update({'gap': coll_dict['gap_R']})
-                elif coll_dict['gap_L'] is not None and coll_dict['gap_R'] is None:
-                    coll_dict.update({'gap': coll_dict['gap_L']})
-                else:
-                    temp_items_to_print = temp_items_to_print + ['gap_L','gap_R']
-                value = {}
-                overwritten_keys = coll_dict['overwritten_keys']
-                for key, val in coll_dict.items():
-                    if key == 'active_length':
-                        key = 'length' 
-                    if (key in coll_items_to_print+temp_items_to_print) and (key not in (set(fam_keys)-set(overwritten_keys))) and (val != 'both'):
-                        value.update({key: val})
-                file.write(_format_dict_entry(coll, value, spacing='    '))
-            file.write('\n')   
-                                
-
-        LHC_families = ['tcp3', 'tcsg3', 'tcsm3', 'tcla3', 'tcp7', 'tcsg7', 'tcsm7', 'tcla7', 'tcli', 'tdi', 'tcdq', 'tcstcdq', 'tcth1', 'tcth2', 'tcth5', 'tcth8', 'tctv1', 'tctv2', 'tctv5', 'tctv8', 'tclp', 'tcxrp', 'tcryo', 'tcl4', 'tcl5', 'tcl6', 'tct15', 'tct2', 'tct8', 'tcsp', 'tcld']
-        with open(f'{out}.yaml', 'w') as file:
-            if '_family_dict' in self.__dict__.keys():
-                file.write('families:\n')
-                if lhc_style:
-                    printed_families = []
-                    fams_in_dict = self._family_dict.keys()
-
-                    # Momentum cleaning
-                    file.write('  # Momentum cleaning\n')
-                    sel_fam = [fam for fam in LHC_families if re.match('.*3', fam) and (fam in fams_in_dict)]
-                    printed_families += sel_fam
-                    _print_values(sel_fam, self._family_dict, file, spacing='  - &', mapping=True)
-
-                    # Betatron cleaning
-                    file.write('  # Betatron cleaning\n')
-                    sel_fam = [fam for fam in LHC_families if re.match('.*7', fam) and (fam in fams_in_dict)]
-                    printed_families += sel_fam
-                    _print_values(sel_fam, self._family_dict, file, spacing='  - &', mapping=True)
-
-                    # Injection protection
-                    file.write('  # Injection protection\n')
-                    sel_fam = [fam for fam in LHC_families if (fam in ['tcli', 'tdi']) and (fam in fams_in_dict)]
-                    printed_families += sel_fam
-                    _print_values(sel_fam, self._family_dict, file, spacing='  - &', mapping=True)
-
-                    # Dump protection
-                    file.write('  # Dump protection\n')
-                    sel_fam = [fam for fam in LHC_families if (fam in ['tcdq', 'tcsp', 'tcstcdq']) and (fam in fams_in_dict)]
-                    printed_families += sel_fam
-                    _print_values(sel_fam, self._family_dict, file, spacing='  - &', mapping=True)
-
-                    # Physics background / debris
-                    file.write('  # Physics background / debris\n')
-                    sel_fam = [fam for fam in LHC_families if ((re.match('tc[lt][0-9dp].*', fam)) or (fam in ['tcryo', 'tcxrp'])) and (fam in fams_in_dict)]
-                    printed_families += sel_fam
-                    _print_values(sel_fam, self._family_dict, file, spacing='  - &', mapping=True)
-
-                    # Other families
-                    if set(printed_families) != set(fams_in_dict):
-                        file.write('  # Other families\n')
-                        _print_values(set(fams_in_dict) - set(printed_families), self._family_dict, file, spacing='  - &', mapping=True)
-                else:
-                    file.write('  # Families\n')
-                    _print_values(self._family_dict.keys(), self._family_dict, file, spacing='  - &', mapping=True)
+    _depends_on = [xt.RandomRutherford]  # Needed for checks
 
-            # Emittance section
-            ex = self.emittance[0]
-            ey = self.emittance[1]
-            file.write(f'\nemittance:\n  x: {ex}\n  y: {ey}\n')
-
-            # Collimators section
-            file.write('\ncollimators:\n')
-            b1_colls, b2_colls, bx_colls = [], [], []
-            for coll in self._colldb.index:
-                if coll == 'tclia.4r2' or coll == 'tclia.4l8':
-                    b1_colls.append(coll)
-                    b2_colls.append(coll)
-                elif coll[-2:] == 'b1':
-                    b1_colls.append(coll)
-                elif coll[-2:] == 'b2':
-                    b2_colls.append(coll)
-                else:
-                    bx_colls.append(coll)
-            
-            # Handle special cases for collimators
-            if (('tclia.4r2' in b1_colls) or ('tclia.4l8' in b1_colls)) and (len(b1_colls) <= 2):
-                b1_colls = []
-            if (('tclia.4r2' in b2_colls) or ('tclia.4l8' in b2_colls)) and (len(b2_colls) <= 2):
-                b2_colls = []
-
-            # Print collimators for each beam
-            if len(b1_colls) > 0:
-                _print_colls(b1_colls, self, 'b1', file)
-            if len(b2_colls) > 0:
-                _print_colls(b2_colls, self, 'b2', file)
-            if len(bx_colls) > 0:
-                _print_colls(bx_colls, self, 'bx', file)
-                print('WARNING -- some collimators could not be assigned to b1 or b2. Tracking might not work with those collimators. Please manually change the output file if necessary.')
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
 
+    def get_backtrack_element(self, _context=None, _buffer=None, _offset=None):
+        return self.__class__(length=-self.length,
+                              _context=_context, _buffer=_buffer, _offset=_offset)
+
+
+class BaseBlock(xt.BeamElement):
+    _xofields = {
+        'length':             xo.Float64,
+        'active':             xo.Int8,
+        'record_touches':     xo.Int8,
+        'record_scatterings': xo.Int8
+    }
+
+    isthick = True
+    allow_track = False
+    behaves_like_drift = True
+    skip_in_loss_location_refinement = True
+
+    _depends_on = [InvalidXcoll]
+
+    _internal_record_class = InteractionRecord
+
+    # This is an abstract class and cannot be instantiated
+    def __new__(cls, *args, **kwargs):
+        if cls == BaseBlock:
+            raise Exception("Abstract class `BaseBlock` cannot be instantiated!")
+        instance = super().__new__(cls)
+        return instance
+
+    def enable_scattering(self):
+        if hasattr(self, '_tracking'):
+            self._tracking = True
+
+    def disable_scattering(self):
+        if hasattr(self, '_tracking'):
+            self._tracking = False
+
+    def get_backtrack_element(self, _context=None, _buffer=None, _offset=None):
+        return InvalidXcoll(length=-self.length,
+                              _context=_context, _buffer=_buffer, _offset=_offset)
+
+
+class BaseCollimator(BaseBlock):
+    _xofields = {**BaseBlock._xofields,
+        # Collimator angle
+        '_sin_zL':        xo.Float64,
+        '_cos_zL':        xo.Float64,
+        '_sin_zR':        xo.Float64,
+        '_cos_zR':        xo.Float64,
+        '_sin_zDiff':     xo.Float64, # Angle of right jaw: difference with respect to angle of left jaw
+        '_cos_zDiff':     xo.Float64,
+        '_jaws_parallel': xo.Int8,
+        # Jaw corners (this is the x-coordinate in the rotated frame)
+        '_jaw_LU':        xo.Float64,  # left upstream
+        '_jaw_RU':        xo.Float64,  # right upstream
+        '_jaw_LD':        xo.Float64,  # left downstream
+        '_jaw_RD':        xo.Float64,  # right downstream
+        # Tilts (superfluous but added to speed up calculations)
+        '_sin_yL':        xo.Float64,
+        '_cos_yL':        xo.Float64,
+        '_tan_yL':        xo.Float64,
+        '_sin_yR':        xo.Float64,
+        '_cos_yR':        xo.Float64,
+        '_tan_yR':        xo.Float64,
+        # Other
+        '_side':          xo.Int8,
+        # These are not used in C, but need to be an xofield to get them in the to_dict:
+        '_align':         xo.Int8,
+        '_gap_L':         xo.Float64,
+        '_gap_R':         xo.Float64,
+        '_nemitt_x':      xo.Float64,
+        '_nemitt_y':      xo.Float64
+    }
+
+    isthick = BaseBlock.isthick
+    allow_track = BaseBlock.allow_track
+    behaves_like_drift = BaseBlock.behaves_like_drift
+    skip_in_loss_location_refinement = BaseBlock.skip_in_loss_location_refinement
+    allow_double_sided = True
+
+    _skip_in_to_dict  = [f for f in _xofields if f.startswith('_')]
+    _store_in_to_dict = ['angle', 'jaw', 'tilt', 'gap', 'side', 'align', 'emittance']
+
+    _depends_on = [BaseBlock]
+
+    _internal_record_class = BaseBlock._internal_record_class
+
+
+    # This is an abstract class and cannot be instantiated
+    def __new__(cls, *args, **kwargs):
+        if cls == BaseCollimator:
+            raise Exception("Abstract class `BaseCollimator` cannot be instantiated!")
+        instance = super().__new__(cls)
+        return instance
 
     def __init__(self, **kwargs):
-        # Get all arguments
-        for var in self._init_vars:
-            if var in self._init_var_defaults:
-                kwargs.setdefault(var, self._init_var_defaults[var])
-            elif var not in kwargs.keys():
-                raise ValueError(f"CollimatorDatabase is missing required argument '{var}'!")
-
-        self._optics = pd.DataFrame(columns=['x', 'px', 'y', 'py', 'betx', 'bety', 'alfx', 'alfy', 'dx', 'dy'])
-        self._parse_dict(kwargs['collimator_dict'], kwargs['family_dict'],
-                         kwargs['beam'], kwargs['_yaml_merged'], kwargs.get('ignore_crystals', True))
-        self.emittance = [kwargs['nemitt_x'], kwargs['nemitt_y']]
-        self._beta_gamma_rel = None
-
-
-    def __getitem__(self, name):
-        return CollimatorSettings(name, self._colldb)
-
-    def to_pandas(self):
-        return pd.DataFrame({
-                's_center':        self.s_center,
-                'gap':             self.gap,
-                'jaw':             self.jaw,
-                'beam_size':       self.beam_size,
-                'aligned_to':      self.align_to,
-                'angle':           self.angle,
-                'material':        self.material,
-#                 'offset':          self.offset,
-#                 'tilt':            self.tilt,
-                'stage':           self.stage,
-                'active_length':   self.active_length,
-                'collimator_type': self.collimator_type,
-            }, index=self.name)
-
-
-    def _parse_dict(self, coll, fam, beam=None, _yaml_merged=False, ignore_crystals=True):
-
-        # We make all keys case-insensitive to avoid confusion between different conventions
-        coll = _dict_keys_to_lower(coll)
-        fam  = _dict_keys_to_lower(fam)
-
-        # The dictionary can be a CollimatorDatabase for a single beam (beam=None)
-        # or for both beams (beam='b1' or beam='b2)
-        coll = _get_coll_dct_by_beam(coll, beam)
-
-        # Apply family settings
-        crystals = []
-        for thiscoll, settings in coll.items():
-            settings = {k.lower(): v for k,v in settings.items()}
-            if 'family' in settings.keys() and settings['family'] is not None:
-                settings['family'] = settings['family'].lower()
-                thisfam = settings['family']
-                if thisfam not in fam.keys():
-                    raise ValueError(f"Collimator {thiscoll} depends on family {thisfam}, "
-                                   + f"but the latter is not defined!")
-
-                # Check if some family settings are overwritten for this collimator
-                # Only do this check if we didn't do a YAML merge earlier (because then it
-                # is already taken care of)
-                if not _yaml_merged:
-                    overwritten_keys = [key.lower() for key in settings.keys() if key in fam[thisfam]]
-                    if len(overwritten_keys) > 0:
-                        settings['overwritten_keys'] = overwritten_keys
-
-                # Load family settings, potentially overwriting settings for this collimator
-                settings = {**fam[thisfam], **settings}
+        to_assign = {}
+        if '_xobject' not in kwargs:
+            # Set side
+            to_assign['side'] = kwargs.pop('side', 'both')
+
+            # Set angle
+            if 'angle' in kwargs:
+                for key in ['angle_L', 'angle_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `angle` and `{key}`!")
+                to_assign['angle'] = kwargs.pop('angle')
+            else:
+                to_assign['angle_L'] = kwargs.pop('angle_L', 0)
+                to_assign['angle_R'] = kwargs.pop('angle_R', 0)
 
+            # Set jaw
+            if 'jaw' in kwargs:
+                for key in ['jaw_L', 'jaw_R', 'jaw_LU', 'jaw_LD', 'jaw_RU', 'jaw_RD', 'gap', 'gap_L', 'gap_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `jaw` and `{key}`!")
+                to_assign['jaw'] = kwargs.pop('jaw')
+            elif 'jaw_L' in kwargs or 'jaw_R' in kwargs:
+                for key in ['jaw_LU', 'jaw_LD', 'jaw_RU', 'jaw_RD', 'gap', 'gap_L', 'gap_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use `jaw_L` or `jaw_R` together with `{key}`!")
+                to_assign['jaw_L'] = kwargs.pop('jaw_L', None)
+                to_assign['jaw_R'] = kwargs.pop('jaw_R', None)
+            elif 'jaw_LU' in kwargs or 'jaw_LD' in kwargs or 'jaw_RU' in kwargs or 'jaw_RD' in kwargs:
+                for key in ['tilt', 'tilt_L', 'tilt_R', 'gap', 'gap_L', 'gap_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `jaw_LU` etc with `{key}`!")
+                to_assign['jaw_LU'] = kwargs.pop('jaw_LU', None)
+                to_assign['jaw_RU'] = kwargs.pop('jaw_RU', None)
+                to_assign['jaw_LD'] = kwargs.pop('jaw_LD', None)
+                to_assign['jaw_RD'] = kwargs.pop('jaw_RD', None)
+            kwargs.setdefault('_jaw_LU', OPEN_JAW)   # Important that these are initialised, in 
+            kwargs.setdefault('_jaw_RU', -OPEN_JAW)  # order to keep a tilt (given together with
+            kwargs.setdefault('_jaw_LD', OPEN_JAW)   # a gap) when optics are not known yet.
+            kwargs.setdefault('_jaw_RD', -OPEN_JAW)
+
+            # Set tilt
+            if 'tilt' in kwargs:
+                for key in ['tilt_L', 'tilt_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `tilt` and `{key}`!")
+                to_assign['tilt'] = kwargs.pop('tilt')
             else:
-                settings['family'] = None
-            coll[thiscoll] = settings
+                to_assign['tilt_L'] = kwargs.pop('tilt_L', 0)
+                to_assign['tilt_R'] = kwargs.pop('tilt_R', 0)
 
-            # Save list of crystals
-            if 'crystal' in settings:
-                if settings['crystal'] != 0.0:
-                    crystals += [thiscoll]
-                else: 
-                    settings['crystal'] = None
-
-        # Remove crystals from colldb
-        if ignore_crystals:
-            for thiscoll in crystals:
-                del coll[thiscoll]
-
-        # Check that all collimators have gap settings
-        if not np.all(['gap' in val.keys() or 'opening' in val.keys() for val in coll.values()]):
-            raise ValueError("Ill-defined CollimatorDatabase: Not all collimators have a gap or "
-                           + "opening setting, (or the keys / structure of the dictionary is wrong)!")
-
-        # Update collimators with default values for missing keys
-        for collimator in coll.values():
-            # Change all values to lower case
-            for key, val in collimator.items():
-                collimator[key] = val.lower() if isinstance(val, str) else val
-            if 'length' in collimator.keys():
-                collimator['active_length'] = collimator.pop('length')
-            if 'gap' in collimator.keys():
-                if collimator['gap'] is not None and collimator['gap'] > 900:
-                    collimator['gap'] = None
-                if 'side' in collimator.keys() and collimator['side'] == 'left':
-                    collimator['gap_L'] = collimator.pop('gap')
-                    collimator['gap_R'] = None
-                elif 'side' in collimator.keys() and collimator['side'] == 'right':
-                    collimator['gap_L'] = None
-                    collimator['gap_R'] = collimator.pop('gap')
-                else:
-                    collimator['gap_L'] = collimator['gap']
-                    collimator['gap_R'] = collimator.pop('gap')
-            if 'angle' in collimator.keys():
-                collimator['angle_L'] = collimator['angle']
-                collimator['angle_R'] = collimator.pop('angle')
-            _initialise_None(collimator)
-
-        self._collimator_dict = coll
-        self._family_dict = fam
-        self._colldb = pd.DataFrame(coll).transpose()
+            # Set gap
+            if 'gap' in kwargs:
+                for key in ['jaw', 'jaw_L', 'jaw_R', 'jaw_LU', 'jaw_LD', 'jaw_RU', 'jaw_RD', 'gap_L', 'gap_R']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `gap` and `{key}`!")
+                to_assign['gap'] = kwargs.pop('gap')
+            elif 'gap_L' in kwargs or 'gap_R' in kwargs:
+                for key in ['jaw', 'jaw_L', 'jaw_R', 'jaw_LU', 'jaw_LD', 'jaw_RU', 'jaw_RD', 'gap']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `gap` and `{key}`!")
+                to_assign['gap_L'] = kwargs.pop('gap_L', None)
+                to_assign['gap_R'] = kwargs.pop('gap_R', None)
+            kwargs.setdefault('_gap_L', OPEN_GAP)
+            kwargs.setdefault('_gap_R', -OPEN_GAP)
+
+            # Set others
+            to_assign['align'] = kwargs.pop('align', 'upstream')
+            to_assign['emittance'] = kwargs.pop('emittance', None)
+            kwargs.setdefault('active', True)
+            kwargs.setdefault('record_touches', False)
+            kwargs.setdefault('record_scatterings', False)
+
+        super().__init__(**kwargs)
+        # Careful: non-xofields are not passed correctly between copy's / to_dict. This messes with flags etc..
+        # We also have to manually initialise them for xobject generation
+        if not hasattr(self, '_optics'):
+            self._optics = None
+        for key, val in to_assign.items():
+            setattr(self, key, val)
+        self._verify_consistency()
 
 
-    @property
-    def name(self):
-        return self._colldb.index.values
-
-
-    # TODO: - VALIDATION OF TYPES (e.g. material, stage, align, ..)
-    #       - IMPLEMENTATION OF TILT
-    #       - CRYSTAL PROPERTIES: only valid if crystal == True (add mask to _set_property?)
-    #         make second dataframe for crystals
-    #       - show as __repr__
-
-    # The CollimatorDatabase class has the following fields (those marked
-    # with an * are set automatically and cannot be overwritten):
-    #   - name
-    #   - gap
-    #   - jaw *
-    #   - beam_size *
-    #   - s_center *
-    #   - angle
-    #   - material
-    #   - offset
-    #   - tilt
-    #   - stage
-    #   - side
-    #   - active_length
-    #   - inactive_front
-    #   - inactive_back
-    #   - total_length *
-    #   - collimator_type *
-    #   - betx
-    #   - bety
-    #   - x
-    #   - px
-    #   - y
-    #   - py
-    #   - gamma_rel
-    #   - emit
+    # Main collimator angle
+    # =====================
 
     @property
     def angle(self):
-#         angles = np.array([self._colldb.angle_L.values,self._colldb.angle_R.values])
-#         return pd.Series([ L if L == R else [L,R] for L, R in angles.T ], index=self._colldb.index, dtype=object)
-        return self._colldb['angle_L']
+        return self.angle_L if self.angle_L==self.angle_R else [self.angle_L, self.angle_R]
 
     @angle.setter
-    def angle(self, angle):
-        self._set_property_LR('angle', angle)
-        self._compute_jaws()
+    def angle(self, val):
+        if not hasattr(val, '__iter__'):
+            self.angle_L = val
+            self.angle_R = val
+        elif len(val) == 1:
+            self.angle_L = val[0]
+            self.angle_R = val[0]
+        elif len(val) == 2:
+            self.angle_L = val[0]
+            self.angle_R = val[1]
+        else:
+            raise ValueError(f"The attribute `angle` should be of the form LR or [L, R] "
+                           + f"but got {val}.")
 
     @property
-    def material(self):
-        return self._colldb['material']
+    def angle_L(self):
+        return round(np.rad2deg(np.arctan2(self._sin_zL, self._cos_zL)), 10)
 
-    @material.setter
-    def material(self, material):
-        self._set_property('material', material)
+    @angle_L.setter
+    def angle_L(self, angle_L):
+        self._sin_zL = np.sin(np.deg2rad(angle_L))
+        self._cos_zL = np.cos(np.deg2rad(angle_L))
+        if np.isclose(self.angle_R, angle_L):
+            self._jaws_parallel = True
+            self._sin_zDiff = 0.
+            self._cos_zDiff = 1.
+        else:
+            self._jaws_parallel = False
+            self._sin_zDiff = np.sin(np.deg2rad(self.angle_R - angle_L))
+            self._cos_zDiff = np.cos(np.deg2rad(self.angle_R - angle_L))
+        self._apply_optics()
+
+    @property
+    def angle_R(self):
+        return round(np.rad2deg(np.arctan2(self._sin_zL, self._cos_zL)), 10)
+
+    @angle_R.setter
+    def angle_R(self, angle_R):
+        self._sin_zR = np.sin(np.deg2rad(angle_R))
+        self._cos_zR = np.cos(np.deg2rad(angle_R))
+        if np.isclose(self.angle_L, angle_R):
+            self._jaws_parallel = True
+            self._sin_zDiff = 0.
+            self._cos_zDiff = 1.
+        else:
+            self._jaws_parallel = False
+            self._sin_zDiff = np.sin(np.deg2rad(angle_R - self.angle_L))
+            self._cos_zDiff = np.cos(np.deg2rad(angle_R - self.angle_L))
+        self._apply_optics()
+
+
+    # Jaw attributes
+    # ==============
 
     @property
-    def offset(self):
-        return self._colldb['offset']
+    def jaw(self):
+        if self.jaw_L is None and self.jaw_R is None:
+            return None
+        elif (self.side == 'left'  and self.tilt_L == 0) \
+        or   (self.side == 'right' and self.tilt_R == 0) \
+        or   (self.tilt_L == 0 and self.tilt_R == 0):
+            return [self.jaw_L, self.jaw_R]
+        else:
+            return [[self.jaw_LU, self.jaw_RU], [self.jaw_LD, self.jaw_RD]]
+
+    @jaw.setter   # Keeps the tilts unless all 4 corners are specified
+    def jaw(self, val):
+        if not hasattr(val, '__iter__') or len(val) == 1:
+            val = val[0] if hasattr(val, '__iter__') else val
+            if self.side == 'left':
+                self.jaw_L = val
+            elif self.side == 'right':
+                # self.jaw_R = -val if val is not None else None
+                self.jaw_R = val
+            else:
+                self.jaw_L = val
+                self.jaw_R = -val if val is not None else None
+            return
+        elif len(val) == 2:
+            if hasattr(val[0], '__iter__'):
+                if hasattr(val[1], '__iter__') and len(val[0]) == 2 and len(val[1]) == 2:
+                    self.jaw_LU = val[0][0]
+                    self.jaw_RU = val[0][1]
+                    self.jaw_LD = val[1][0]
+                    self.jaw_RD = val[1][1]
+                    return
+            else:
+                self.jaw_L = val[0]
+                self.jaw_R = val[1]
+                return
+        # If we got here, val is incompatible
+        raise ValueError(f"The attribute `jaw` should be of the form [L, R] or "
+                       + f"[[LU, RU], [LD, RD], but got {val}.")
+
+    @property
+    def jaw_L(self):
+        jaw_L = (self._jaw_LU + self._jaw_LD) / 2
+        if not np.isclose(jaw_L, OPEN_JAW, atol=1.e-10):  # open position
+            return jaw_L
+
+    @jaw_L.setter   # This moves both jaw_LU and jaw_LD in parallel
+    def jaw_L(self, val):
+        if self.side == 'right' and val is not None:
+            val = None
+            print("Warning: Ignored value for jaw_L (right-sided collimator).")
+        if val is None:
+            val = OPEN_JAW
+            self._gap_L = OPEN_GAP
+        diff = val - (self._jaw_LU + self._jaw_LD) / 2
+        self._jaw_LU += diff
+        self._jaw_LD += diff
+        self._update_gaps()
+
+    @property
+    def jaw_R(self):
+        jaw_R = (self._jaw_RU + self._jaw_RD) / 2
+        if not np.isclose(jaw_R, -OPEN_JAW, atol=1.e-10):  # open position
+            return jaw_R
+
+    @jaw_R.setter   # This moves both jaw_RU and jaw_RD in parallel
+    def jaw_R(self, val):
+        if self.side == 'left' and val is not None:
+            val = None
+            print("Warning: Ignored value for jaw_R (left-sided collimator).")
+        if val is None:
+            val = -OPEN_JAW
+            self._gap_R = OPEN_GAP
+        diff = val - (self._jaw_RU + self._jaw_RD) / 2
+        self._jaw_RU += diff
+        self._jaw_RD += diff
+        self._update_gaps()
+
+    @property
+    def jaw_LU(self):
+        if not self.jaw_L is None:
+            return self._jaw_LU
+
+    @jaw_LU.setter   # This assumes jaw_LD remains fixed, hence both jaw_L and the tilt change
+    def jaw_LU(self, val):
+        if self.side == 'right':
+            if val is not None:
+                print("Warning: Ignored value for jaw_LU (right-sided collimator).")
+            return
+        if val is None:
+            raise ValueError("Cannot set corner to None! Use open_jaws() or set jaw_L to None.")
+        self._jaw_LU = val
+        self._update_tilts()   # Extra, to update tilts which are also in C for efficiency
+        self._update_gaps()
+
+    @property
+    def jaw_LD(self):
+        if not self.jaw_L is None:
+            return self._jaw_LD
+
+    @jaw_LD.setter   # This assumes jaw_LU remains fixed, hence both jaw_L and the tilt change
+    def jaw_LD(self, val):
+        if self.side == 'right':
+            if val is not None:
+                print("Warning: Ignored value for jaw_LD (right-sided collimator).")
+            return
+        if val is None:
+            raise ValueError("Cannot set corner to None! Use open_jaws() or set jaw_L to None.")
+        self._jaw_LD = val
+        self._update_tilts()   # Extra, to update tilts which are also in C for efficiency
+        self._update_gaps()
+
+    @property
+    def jaw_RU(self):
+        if not self.jaw_R is None:
+            return self._jaw_RU
+
+    @jaw_RU.setter   # This assumes jaw_RD remains fixed, hence both jaw_R and the tilt change
+    def jaw_RU(self, val):
+        if self.side == 'left':
+            if val is not None:
+                print("Warning: Ignored value for jaw_RU (left-sided collimator).")
+            return
+        if val is None:
+            raise ValueError("Cannot set corner to None! Use open_jaws() or set jaw_R to None.")
+        self._jaw_RU = val
+        self._update_tilts()   # Extra, to update tilts which are also in C for efficiency
+        self._update_gaps()
+
+    @property
+    def jaw_RD(self):
+        if not self.jaw_R is None:
+            return self._jaw_RD
+
+    @jaw_RD.setter   # This assumes jaw_RU remains fixed, hence both jaw_R and the tilt change
+    def jaw_RD(self, val):
+        if self.side == 'left':
+            if val is not None:
+                print("Warning: Ignored value for jaw_RD (left-sided collimator).")
+            return
+        if val is None:
+            raise ValueError("Cannot set corner to None! Use open_jaws() or set jaw_R to None.")
+        self._jaw_RD = val
+        self._update_tilts()   # Extra, to update tilts which are also in C for efficiency
+        self._update_gaps()
+
+    def open_jaws(self, keep_tilts=False):
+        self.jaw_L = None
+        self.jaw_R = None
+        if not keep_tilts:
+            self.tilt = 0
+
+    def _update_tilts(self):
+        if self.side != 'right':
+            self._sin_yL = (self.jaw_LD - self.jaw_LU) / self.length
+            self._cos_yL = np.sqrt(1 - self._sin_yL**2)
+            self._tan_yL = self._sin_yL / self._cos_yL
+        if self.side != 'left':
+            self._sin_yR = (self.jaw_RD - self.jaw_RU) / self.length
+            self._cos_yR = np.sqrt(1 - self._sin_yR**2)
+            self._tan_yR = self._sin_yR / self._cos_yR
+
+    def _update_gaps(self):
+        # If we had set a value for the gap manually, this needs to be updated
+        # as well after setting the jaw
+        if self._gap_L_set_manually():
+            self._gap_L = self.gap_L
+        if self._gap_R_set_manually():
+            self._gap_R = self.gap_R
 
-    @offset.setter
-    def offset(self, offset):
-        self._set_property('offset', offset, single_default_allowed=True)
-        self._compute_jaws()
+
+    # Tilt attributes
+    # ===============
+
+    # TODO: tilts are in rad! Do we want that? It's a bit inconsistent with angle which is in deg...
 
     @property
     def tilt(self):
-        tilts = np.array([self._colldb.tilt_L.values,self._colldb.tilt_R.values])
-        return pd.Series([ L if L == R else [L,R] for L, R in tilts.T ], index=self._colldb.index, dtype=object)
+        if self.side == 'left':
+            return self.tilt_L
+        elif self.side == 'right':
+            return self.tilt_R
+        else:
+            return self.tilt_L if self.tilt_L==self.tilt_R else [self.tilt_L, self.tilt_R]
 
     @tilt.setter
-    def tilt(self, tilts):
-        self._set_property_LR('tilt', tilts)
-        self._compute_jaws()
+    def tilt(self, val):
+        if not hasattr(val, '__iter__') or len(val) == 1:
+            val = val[0] if hasattr(val, '__iter__') else val
+            if self.side == 'left':
+                self.tilt_L = val
+            elif self.side == 'right':
+                self.tilt_R = val
+            else:
+                self.tilt_L = val
+                self.tilt_R = val
+        elif len(val) == 2:
+            self.tilt_L = val[0]
+            self.tilt_R = val[1]
+        else:
+            raise ValueError
 
     @property
-    def stage(self):
-        return self._colldb['stage']
+    def tilt_L(self):
+        if self.side != 'right':
+            return round(np.arctan2(self._sin_yL, self._cos_yL), 10)
+
+    @tilt_L.setter   # This assumes jaw_L remains fixed (hence jaw_LU and jaw_LD change)
+    def tilt_L(self, val):
+        if self.side == 'right' and val != 0:
+            val = 0
+            print("Warning: Ignored value for tilt_L (right-sided collimator).")
+        if val != 0:
+            print("Warning: Setting a tilt does not preserve the hierarchy, as there "
+                + "will always be one corner that tightens (the tilt is applied at "
+                + "the centre of the jaw).")
+        self._sin_yL = np.sin(val)
+        self._cos_yL = np.cos(val)
+        self._tan_yL = np.tan(val)
+        jaw_L = (self._jaw_LU + self._jaw_LD) / 2
+        self._jaw_LD = jaw_L + self._sin_yL * self.length / 2.
+        self._jaw_LU = jaw_L - self._sin_yL * self.length / 2.
+
+    @property
+    def tilt_R(self):
+        if self.side != 'left':
+            return round(np.arctan2(self._sin_yR, self._cos_yR), 10)
+
+    @tilt_R.setter   # This assumes jaw_R remains fixed (hence jaw_RU and jaw_RD change)
+    def tilt_R(self, val):
+        if self.side == 'left' and val != 0:
+            val = 0
+            print("Warning: Ignored value for tilt_R (left-sided collimator).")
+        if val != 0:
+            print("Warning: Setting a tilt does not preserve the hierarchy, as there "
+                + "will always be one corner that tightens (the tilt is applied at "
+                + "the centre of the jaw).")
+        self._sin_yR = np.sin(val)
+        self._cos_yR = np.cos(val)
+        self._tan_yR = np.tan(val)
+        jaw_R = (self._jaw_RU + self._jaw_RD) / 2
+        self._jaw_RD = jaw_R + self._sin_yR * self.length / 2.
+        self._jaw_RU = jaw_R - self._sin_yR * self.length / 2.
+
+
+    # Optics
+    # ======
+
+    @property
+    def optics(self):
+        return self._optics
+
+    def optics_ready(self):
+        return self.emittance is not None and self.optics is not None
+
+    def assign_optics(self, *, nemitt_x=None, nemitt_y=None, beta_gamma_rel=None, name=None, twiss=None,
+                      twiss_upstream=None, twiss_downstream=None):
+        from xcoll import element_classes
+        if not isinstance(self, element_classes):
+            raise ValueError("Please install collimator before assigning optics.")
+        if nemitt_x is None:
+            if self.nemitt_x is None:
+                raise ValueError("Need to provide `nemitt_x`.")
+        else:
+            self.nemitt_x = nemitt_x
+        if nemitt_y is None:
+            if self.nemitt_y is None:
+                raise ValueError("Need to provide `nemitt_y`.")
+        else:
+            self.nemitt_y = nemitt_y
+        if beta_gamma_rel is None:
+            raise ValueError("Need to provide `beta_gamma_rel`.")
+        if twiss is None:
+            if twiss_upstream is None or twiss_downstream is None:
+                raise ValueError("Use either `twiss` or `twiss_upstream` and `twiss_downstream`.")
+            if name is None:
+                if len(twiss_upstream.name) > 1 or len(twiss_downstream.name) > 1:
+                    raise ValueError("Need to provide `name` or twisses that are a single row each.")
+                tw_up   = twiss_upstream
+                tw_down = twiss_downstream
+            else:
+                tw_up   = twiss_upstream.rows[name]
+                tw_down = twiss_downstream.rows[name]
+        elif twiss_downstream is not None or twiss_downstream is not None:
+            raise ValueError("Use either `twiss` or `twiss_upstream` and `twiss_downstream`.")
+        elif name is None:
+            raise ValueError("When using `twiss`, need to provide the name as well.")
+        else:
+            tw_up   = twiss.rows[name]
+            tw_down = twiss.rows[twiss.mask[[name]]+1]
+        if not np.isclose(tw_up.s[0] + self.length, tw_down.s[0]):
+            raise ValueError(f"Downstream twiss not compatible with length {self.length}m.")
+        self._optics = {
+            'upstream': tw_up,
+            'downstream': tw_down,
+            'beta_gamma_rel': beta_gamma_rel
+        }
+        self._apply_optics()
 
-    @stage.setter
-    def stage(self, stage):
-        self._set_property('stage', stage)
+    @property
+    def nemitt_x(self):
+        if self._nemitt_x == 0:
+            return None
+        return self._nemitt_x
+
+    @nemitt_x.setter
+    def nemitt_x(self, val):
+        if val is None:
+            self._nemitt_x = 0
+        if val <= 0:
+            raise ValueError(f"The field `nemitt_x` should be positive, but got {val}.")
+        self._nemitt_x = val
+        self._apply_optics()
 
     @property
-    def parking(self):
-        return self._colldb['parking']
+    def nemitt_y(self):
+        if self._nemitt_y == 0:
+            return None
+        return self._nemitt_y
 
-    @parking.setter
-    def parking(self, parking):
-        self._set_property('parking', parking, single_default_allowed=True)
-        self._compute_jaws()
+    @nemitt_y.setter
+    def nemitt_y(self, val):
+        if val is None:
+            self._nemitt_y = 0
+        else:
+            if val <= 0:
+                raise ValueError(f"The field `nemitt_y` should be positive, but got {val}.")
+            self._nemitt_y = val
+            self._apply_optics()
 
     @property
-    def active(self):
-        return self._colldb['active']
+    def emittance(self):
+        if self.nemitt_x is not None and self.nemitt_y is not None:
+            if np.isclose(self.nemitt_x, self.nemitt_y):
+                return self.nemitt_x
+            else:
+                return [self.nemitt_x, self.nemitt_y]
 
-    @active.setter
-    def active(self, active):
-        self._set_property('active', active, single_default_allowed=True)
+    @emittance.setter
+    def emittance(self, val):
+        if val is None:
+            self._nemitt_x = 0
+            self._nemitt_y = 0
+        else:
+            if not hasattr(val, '__iter__'):
+                val = [val]
+            if len(val) == 1:
+                val = [val[0], val[0]]
+            assert len(val) == 2
+            if val[0] <= 0 or val[1] <= 0:
+                raise ValueError(f"The field `emittance` should be positive, but got {val}.")
+            self._nemitt_x = val[0]
+            self._nemitt_y = val[1]
+            self._apply_optics()
+
+    @property
+    def sigma(self):
+        if self.optics_ready():
+            betx = self.optics[self.align]['betx'][0]
+            bety = self.optics[self.align]['bety'][0]
+            sigma_x = np.sqrt(betx*self.nemitt_x/self.optics['beta_gamma_rel'])
+            sigma_y = np.sqrt(bety*self.nemitt_y/self.optics['beta_gamma_rel'])
+            if hasattr(self, '_cos_zL'):
+                sigma_L = np.sqrt((sigma_x*self._cos_zL)**2 + (sigma_y*self._sin_zL)**2)
+                sigma_R = np.sqrt((sigma_x*self._cos_zR)**2 + (sigma_y*self._sin_zR)**2)
+                return [sigma_L, sigma_R], [sigma_x, sigma_y]
+            else:
+                sigma = np.sqrt((sigma_x*self._cos_z)**2 + (sigma_y*self._sin_z)**2)
+                return sigma, [sigma_x, sigma_y]
+
+    @property
+    def co(self):
+        if self.optics_ready():
+            x = self.optics[self.align]['x'][0]
+            y = self.optics[self.align]['y'][0]
+            if hasattr(self, '_cos_zL'):
+                co_L = x*self._cos_zL + y*self._sin_zL
+                co_R = x*self._cos_zR + y*self._sin_zR
+                return [co_L, co_R], [x, y]
+            else:
+                co = x*self._cos_z + y*self._sin_z
+                return co, [x, y]
 
-#     @property
-#     def crystal(self):
-#         return self._colldb['crystal']
+    @property
+    def divergence(self):
+        if self.optics_ready():
+            alfx = self.optics[self.align]['alfx'][0]
+            alfy = self.optics[self.align]['alfy'][0]
+            betx = self.optics[self.align]['betx'][0]
+            bety = self.optics[self.align]['bety'][0]
+            divx = -np.sqrt(self.nemitt_x/self.optics['beta_gamma_rel']/betx)*alfx
+            divy = -np.sqrt(self.nemitt_y/self.optics['beta_gamma_rel']/bety)*alfy
+            if hasattr(self, '_cos_zL'):
+                if self.side != 'right':
+                    return divx if abs(self.angle_L) < 1e-6 else divy
+                else:
+                    return divx if abs(self.angle_R) < 1e-6 else divy
+            else:
+                return divx if abs(self.angle) < 1e-6 else divy
 
-#     @crystal.setter
-#     def crystal(self, crystal):
-#         self._set_property('crystal', crystal)
+    @property
+    def align(self):
+        if self._align == 0:
+            return 'upstream'
+        elif self._align == 1:
+            return 'downstream'
+        else:
+            raise ValueError(f"The attribute `align` can only be 'upstream' or "
+                            +f"'downstream', but stored as {self._align}.")
 
-#     @property
-#     def bend(self):
-#         return self._colldb['bend']
+    @align.setter
+    def align(self, val):
+        if val == 'upstream':
+            self._align = 0
+        elif val == 'downstream':
+            self._align = 1
+        else:
+            raise ValueError(f"The attribute `align` can only be 'upstream' or "
+                            +f"'downstream', but got {val}.")
+        self._apply_optics()
 
-#     @bend.setter
-#     def bend(self, bend):
-#         self._set_property('bend', bend)
 
-#     @property
-#     def xdim(self):
-#         return self._colldb['xdim']
+    # Gap attributes
+    # ==============
 
-#     @xdim.setter
-#     def xdim(self, xdim):
-#         self._set_property('xdim', xdim)
+    @property
+    def gap(self):
+        if self.gap_L is None and self.gap_R is None:
+            return None
+        elif self.gap_R is not None and self.gap_L == -self.gap_R:
+            return self.gap_L
+        else:
+            return [self.gap_L, self.gap_R]
 
-#     @property
-#     def ydim(self):
-#         return self._colldb['ydim']
+    @gap.setter
+    def gap(self, val):
+        if not hasattr(val, '__iter__') or len(val) == 1:
+            val = val[0] if hasattr(val, '__iter__') else val
+            if self.side == 'left':
+                self.gap_L = val
+            elif self.side == 'right':
+                # self.gap_R = -val if val is not None else None
+                self.gap_R = val
+            else:
+                self.gap_L = val
+                self.gap_R = -val if val is not None else None
+            return
+        elif len(val) == 2:
+            if not hasattr(val[0], '__iter__') \
+            and not hasattr(val[1], '__iter__'):
+                if val[0] is not None and val[1] is not None:
+                    if val[0] <= val[1]:
+                        raise ValueError(f"The attribute `gap_L` should be larger "
+                                       + f"than `gap_R` but got {val}.")
+                self.gap_L = val[0]
+                self.gap_R = val[1]
+                return
+        # If we got here, val is incompatible
+        raise ValueError(f"The attribute `gap` should be of the form `gap` or "
+                       + f"`[gap_L, gap_R]`, but got {val}.")
+
+    @property
+    def gap_L(self):
+        if self.side != 'right':
+            if self.optics_ready() and self.jaw_L is not None:
+                return round((self.jaw_L - self.co[0][0])/self.sigma[0][0], 6)
+            elif not self._gap_L_set_manually():
+                return None
+            else:
+                return self._gap_L
 
-#     @ydim.setter
-#     def ydim(self, ydim):
-#         self._set_property('ydim', ydim)
+    @gap_L.setter
+    def gap_L(self, val):
+        if val is None:
+            val = OPEN_GAP
+            self.jaw_L = None
+        if val <= 0:
+            raise ValueError(f"The field `gap_L` should be positive, but got {val}.")
+        self._gap_L = val
+        self._apply_optics()
+
+    @property
+    def gap_R(self):
+        if self.side != 'left':
+            if self.optics_ready() and self.jaw_R is not None:
+                return round((self.jaw_R - self.co[0][1])/self.sigma[0][1], 6)
+            elif not self._gap_R_set_manually():
+                return None
+            else:
+                return self._gap_R
 
-#     @property
-#     def miscut(self):
-#         return self._colldb['miscut']
+    @gap_R.setter
+    def gap_R(self, val):
+        if val is None:
+            val = -OPEN_GAP
+            self.jaw_R = None
+        if val >= 0:
+            raise ValueError(f"The field `gap_R` should be negative, but got {val}.")
+        self._gap_R = val
+        self._apply_optics()
 
-#     @miscut.setter
-#     def miscut(self, miscut):
-#         self._set_property('miscut', miscut)
+    @property
+    def gap_LU(self):
+        if self.gap_L is not None and self.optics_ready():
+            return round(self._gap_L - self._sin_yL * self.length / 2. / self.sigma[0][0], 6)
 
-#     @property
-#     def thick(self):
-#         return self._colldb['thick']
+    @property
+    def gap_LD(self):
+        if self.gap_L is not None and self.optics_ready():
+            return round(self._gap_L + self._sin_yL * self.length / 2. / self.sigma[0][0], 6)
 
-#     @thick.setter
-#     def thick(self, thick):
-#         self._set_property('thick', thick)
+    @property
+    def gap_RU(self):
+        if self.gap_R is not None and self.optics_ready():
+            return round(self._gap_R - self._sin_yR * self.length / 2. / self.sigma[0][1], 6)
 
     @property
-    def s_center(self):
-        return self._colldb['s_center']
+    def gap_RD(self):
+        if self.gap_R is not None and self.optics_ready():
+            return round(self._gap_R + self._sin_yR * self.length / 2. / self.sigma[0][1], 6)
+
+    def _gap_L_set_manually(self):
+        return not np.isclose(self._gap_L, OPEN_GAP)
+
+    def _gap_R_set_manually(self):
+        return not np.isclose(self._gap_R, -OPEN_GAP)
+
+    def _apply_optics(self):
+        if self.optics_ready():
+            # Only if we have set a value for the gap manually, this needs to be updated
+            if self._gap_L_set_manually():
+                self.jaw_L = self._gap_L * self.sigma[0][0] + self.co[0][0]
+            if self._gap_R_set_manually():
+                self.jaw_R = self._gap_R * self.sigma[0][1] + self.co[0][1]
+
+
+    # Other attributes
+    # ================
 
     @property
-    def collimator_type(self):
-        return self._colldb['collimator_type']
+    def side(self):
+        if self._side == 0:
+            return 'both'
+        elif self._side == 1:
+            return 'left'
+        elif self._side == -1:
+            return 'right'
+
+    @side.setter
+    def side(self, val):
+        if isinstance(val, str):
+            if val.lower() == 'both' or val == '+-' or val == '-+':
+                self._side = 0
+                return
+            elif val.lower() == 'left' or val.lower() == 'l' or val == '+':
+                self._side = 1
+                self.gap_R = None
+                return
+            elif val.lower() == 'right' or val.lower() == 'r' or val == '-':
+                self._side = -1
+                self.gap_L = None
+                return
+        raise ValueError(f"Unkown setting {val} for 'side'! Choose from "
+                       + f"('left', 'L', '+'), ('right', 'R', '-'), or ('both', '+-').")
 
     @property
     def active_length(self):
-        return self._colldb['active_length']
-
-    @active_length.setter
-    def active_length(self, length):
-        self._set_property('active_length', length)
-        self.align_to = {}
+        raise ValueError("`active_length`is deprecated. Please use `length`.")
 
     @property
     def inactive_front(self):
-        return self._colldb['inactive_front']
-
-    @inactive_front.setter
-    def inactive_front(self, length):
-        self._set_property('inactive_front', length)
+        raise ValueError("`inactive_front`is deprecated. Collimators now only "
+                       + "contain their active length (implemented as `length`).")
 
     @property
     def inactive_back(self):
-        return self._colldb['inactive_back']
+        raise ValueError("`inactive_back`is deprecated. Collimators now only "
+                       + "contain their active length (implemented as `length`).")
 
-    @inactive_back.setter
-    def inactive_back(self, length):
-        self._set_property('inactive_back', length)
 
-    @property
-    def total_length(self):
-        return self._colldb['active_length'] +  self._colldb['inactive_front'] + self._colldb['inactive_back']
+    # Methods
+    # =======
 
-    @property
-    def gap(self):
-        gaps = np.array([self._colldb.gap_L.values,self._colldb.gap_R.values])
-        return pd.Series([ L if L == R else [L,R] for L, R in gaps.T ], index=self._colldb.index, dtype=object)
+    def enable_scattering(self):
+        if hasattr(self, '_tracking'):
+            if self.optics is None:
+                raise ValueError("Optics not assigned! Cannot enable scattering.")
+            self._tracking = True
+
+    def disable_scattering(self):
+        if hasattr(self, '_tracking'):
+            self._tracking = False
+
+    def _verify_consistency(self):
+        # Verify angles
+        if abs(self.angle_L - self.angle_R) >= 90.:
+            raise ValueError("Angles of both jaws differ more than 90 degrees!")
+        ang = abs(np.arccos(self._cos_zL))
+        ang = np.pi - ang if ang > np.pi/2 else ang
+        assert np.isclose(ang, abs(np.arcsin(self._sin_zL)))
+        ang = abs(np.arccos(self._cos_zR))
+        ang = np.pi - ang if ang > np.pi/2 else ang
+        assert np.isclose(ang, abs(np.arcsin(self._sin_zR)))
+        if np.isclose(self.angle_L, self.angle_R):
+            assert self._jaws_parallel == True
+            assert np.isclose(self._sin_zL, self._sin_zR)
+            assert np.isclose(self._cos_zL, self._cos_zR)
+            assert np.isclose(self._sin_zDiff, 0.)
+            assert np.isclose(self._cos_zDiff, 1.)
+        else:
+            assert self._jaws_parallel == False
+            assert np.isclose(self._sin_zDiff, self._cos_zL*self._sin_zR - self._sin_zL*self._cos_zR)
+            assert np.isclose(self._cos_zDiff, self._cos_zL*self._cos_zR + self._sin_zL*self._sin_zR)
+        if self.side == 'both' and abs(self.tilt_L - self.tilt_R) >= 90.:
+            raise ValueError("Tilts of both jaws differ more than 90 degrees!")
+        if self.side != 'right':
+            ang = abs(np.arccos(self._cos_yL))
+            ang = np.pi - ang if ang > np.pi/2 else ang
+            assert np.isclose(ang, abs(np.arcsin(self._sin_yL)))
+            assert np.isclose(self._sin_yL/self._cos_yL, self._tan_yL)
+        if self.side != 'left':
+            ang = abs(np.arccos(self._cos_yR))
+            ang = np.pi - ang if ang > np.pi/2 else ang
+            assert np.isclose(ang, abs(np.arcsin(self._sin_yR)))
+            assert np.isclose(self._sin_yR/self._cos_yR, self._tan_yR)
+
+        # Verify bools
+        assert self._side in [-1, 1, 0]
+        assert isinstance(self._jaws_parallel, bool) or self._jaws_parallel in [0, 1]
+        assert isinstance(self.active, bool) or self.active in [0, 1]
+        assert isinstance(self.record_touches, bool) or self.record_touches in [0, 1]
+        assert isinstance(self.record_scatterings, bool) or self.record_scatterings in [0, 1]
+
+    def jaw_func(self, pos):
+        positions = ['LU', 'RU', 'LD', 'RD']
+        if pos[0] == 'L': 
+            other_pos = 'R' 
+        else: 
+            other_pos = 'L'
+        point_x = ((getattr(self, 'jaw_' + pos[0]) * getattr(self, 'cos_z' + pos[0]) 
+                    + getattr(self, 'jaw_' + other_pos) * getattr(self, 'cos_z' + other_pos))/2)
+        point_y = ((getattr(self, 'jaw_' + pos[0]) * getattr(self, 'sin_z' + pos[0]) 
+                    + getattr(self, 'jaw_' + other_pos) * getattr(self, 'sin_z' + other_pos))/2)
+        if not pos in positions:
+            raise ValueError(f"Parameter {pos} needs to be one of {positions}!")
+        sinz    = getattr(self, 'sin_z' + pos[0])
+        cosz    = getattr(self, 'cos_z' + pos[0])
+        # Shift to the jaw, whose location is given as the shortest distance:
+        point_x += getattr(self, 'jaw_' + pos) * cosz
+        point_y += getattr(self, 'jaw_' + pos) * sinz
+        return lambda t: (point_x - t*sinz, point_y + t*cosz)
+
+
+class BaseCrystal(BaseBlock):
+    _xofields = {**BaseBlock._xofields,
+        # Collimator angle
+        '_sin_z':             xo.Float64,
+        '_cos_z':             xo.Float64,
+        # Jaw corners (this is the x-coordinate in the rotated frame)
+        '_jaw_U':             xo.Float64,
+        # Tilts (not superfluous)
+        '_sin_y':             xo.Float64,
+        '_cos_y':             xo.Float64,
+        '_tan_y':             xo.Float64,
+        # Other
+        '_side':              xo.Int8,
+        # These are not used in C, but need to be an xofield to get them in the to_dict:
+        '_align':             xo.Int8,
+        '_gap':               xo.Float64,
+        '_nemitt_x':          xo.Float64,
+        '_nemitt_y':          xo.Float64,
+        # Crystal specific
+        '_bending_radius':    xo.Float64,
+        '_bending_angle':     xo.Float64,
+        'width':              xo.Float64,
+        'height':             xo.Float64
+        # 'thick':              xo.Float64
+    }
+
+    isthick = BaseBlock.isthick
+    allow_track = BaseBlock.allow_track
+    behaves_like_drift = BaseBlock.behaves_like_drift
+    skip_in_loss_location_refinement = BaseBlock.skip_in_loss_location_refinement
+    allow_double_sided = False
+
+    _skip_in_to_dict  = [f for f in _xofields if f.startswith('_')]
+    _store_in_to_dict = ['angle', 'jaw', 'tilt', 'gap', 'side', 'align', 'emittance',
+                         'bending_radius', 'bending_angle']
+
+    _depends_on = [BaseCollimator]
+
+    _internal_record_class = BaseBlock._internal_record_class
+
+    # This is an abstract class and cannot be instantiated
+    def __new__(cls, *args, **kwargs):
+        if cls == BaseCrystal:
+            raise Exception("Abstract class `BaseCrystal` cannot be instantiated!")
+        instance = super().__new__(cls)
+        return instance
 
-    @gap.setter
-    def gap(self, gaps):
-        df = self._colldb
-        correct_format = False
-        # The variable gaps is a Series or a list
-        if isinstance(gaps, pd.Series) or isinstance(gaps, list) or isinstance(gaps, np.ndarray):
-            correct_format = True
-            if len(gaps) != len(self.name):
-                raise ValueError("The variable 'gaps' has a different length than the number "
-                                + "of collimators in the CollimatorDatabase. Use a dictionary instead.")
-            # Some of the gaps are list (e.g. two different values for both gaps): loop over gaps as dict
-            if any(hasattr(gap, '__iter__') for gap in gaps):
-                gaps = dict(zip(self.name, gaps))
-            # All gaps are single values: use pandas-style assignment
+    def __init__(self, **kwargs):
+        to_assign = {}
+        if '_xobject' not in kwargs:
+            # Set side
+            to_assign['side'] = kwargs.pop('side', 'left')
+
+            # Set angle
+            to_assign['angle'] = kwargs.pop('angle', 0)
+
+            # Set jaw
+            if 'jaw' in kwargs:
+                for key in ['jaw_U', 'jaw_D', 'gap']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `jaw` and `{key}`!")
+                to_assign['jaw'] = kwargs.pop('jaw')
+            elif 'jaw_D' in kwargs:
+                for key in ['tilt', 'gap']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `jaw_D` with `{key}`!")
+                if not 'jaw_U' in kwargs:
+                    raise ValueError("Need to provide `jaw_U` when setting `jaw_D`!")
+                to_assign['jaw_U'] = kwargs.pop('jaw_U')
+                to_assign['jaw_D'] = kwargs.pop('jaw_D')
+            elif 'jaw_U' in kwargs:
+                if 'gap' in kwargs:
+                    raise ValueError(f"Cannot use both `jaw_U` and `gap`!")
+                to_assign['jaw_U'] = kwargs.pop('jaw_U')
+            # TODO: correct sign if right-sided
+            kwargs.setdefault('_jaw_U', OPEN_JAW)
+
+            # Set gap
+            if 'gap' in kwargs:
+                for key in ['jaw', 'jaw_U', 'jaw_D']:
+                    if key in kwargs:
+                        raise ValueError(f"Cannot use both `gap` and `{key}`!")
+                to_assign['gap'] = kwargs.pop('gap')
+            # TODO: correct sign if right-sided
+            kwargs.setdefault('_gap', OPEN_GAP)
+
+            # Set tilt
+            if 'jaw_D' not in kwargs:
+                to_assign['tilt'] = kwargs.pop('tilt', 0)
+
+            # Set others
+            to_assign['align'] = kwargs.pop('align', 'upstream')
+            to_assign['emittance'] = kwargs.pop('emittance', None)
+            kwargs.setdefault('active', True)
+            kwargs.setdefault('record_touches', False)
+            kwargs.setdefault('record_scatterings', False)
+
+            # Set crystal specific
+            if 'bending_angle' in kwargs:
+                if 'bending_radius' in kwargs:
+                    raise ValueError("Need to choose between 'bending_radius' and 'bending_angle'!")
+                to_assign['bending_angle'] = kwargs.pop('bending_angle')
             else:
-                # mask those that have an active side for the gap under consideration
-                # and have a setting less than 900; the others are set to None
-                mask_L = np.logical_and(df.side.isin(['both','left']), ~(gaps >= 900))
-                mask_R = np.logical_and(df.side.isin(['both','right']), ~(gaps >= 900))
-                df.loc[mask_L, 'gap_L'] = gaps[mask_L]
-                df.loc[~mask_L, 'gap_L'] = None
-                df.loc[mask_R, 'gap_R'] = gaps[mask_R]
-                df.loc[~mask_R, 'gap_R'] = None
-
-        # The variable gaps is a dictionary
-        if isinstance(gaps, dict):
-            correct_format = True
-            for name, gap in gaps.items():
-                if name not in self.name:
-                    raise ValueError(f"Collimator {name} not found in CollimatorDatabase!")
-                side = df.side[name]
-                if hasattr(gap, '__iter__'):
-                    if isinstance(gap, str):
-                        raise ValueError("The gap setting has to be a number!")
-                    elif len(gap) == 2:
-                        gap_L = gap[0]
-                        gap_R = gap[1]
-                        if side != 'both':
-                            if side == 'left' and gap_R is not None:
-                                print(f"Warning: collimator {name} is left-sided but a finite right gap is specified. "
-                                      + "Verify that this is what you want.")
-                            elif side == 'right' and gap_L is not None:
-                                print(f"Warning: collimator {name} is right-sided but a finite left gap is specified. "
-                                      + "Verify that this is what you want.")
-                    elif len(gap) == 1:
-                        gap_L = gap[0] if side in ['both','left'] else None
-                        gap_R = gap[0] if side in ['both','right'] else None
-                    else:
-                        raise ValueError("The gap setting must have one or two values (for the left and the right jaw)!")
-                else:
-                    gap_L = gap if side in ['both','left'] else None
-                    gap_R = gap if side in ['both','right'] else None
-                gap_L = None if (gap_L is not None and gap_L >= 900) else gap_L
-                gap_R = None if (gap_R is not None and gap_R >= 900) else gap_R
-                df.loc[name, 'gap_L'] = gap_L
-                df.loc[name, 'gap_R'] = gap_R
-
-        if not correct_format:
-            raise ValueError("Variable 'gaps' needs to be a pandas Series, dict, numpy array, or list!")
-
-        df.gap_L = df.gap_L.astype('object', copy=False)
-        df.gap_R = df.gap_R.astype('object', copy=False)
-        self._compute_jaws()
+                to_assign['bending_radius'] = kwargs.pop('bending_radius', 1)
+            kwargs.setdefault('width', 0)
+            kwargs.setdefault('height', 0)
+
+        xt.BeamElement.__init__(self, **kwargs)
+        # Careful: non-xofields are not passed correctly between copy's / to_dict. This messes with flags etc..
+        # We also have to manually initialise them for xobject generation
+        if not hasattr(self, '_optics'):
+            self._optics = None
+        for key, val in to_assign.items():
+            setattr(self, key, val)
+        if self.side == 'right':
+            if np.isclose(self._jaw_U, OPEN_JAW):
+                self._jaw_U *= -1
+            if np.isclose(self._gap, OPEN_GAP):
+                self._gap *= -1
+        self._verify_consistency()
+
+
+    # Main crystal angle
+    # ==================
+
+    @property
+    def angle(self):
+        return round(np.rad2deg(np.arctan2(self._sin_z, self._cos_z)), 10)
+
+    @angle.setter
+    def angle(self, val):
+        self._sin_z = np.sin(np.deg2rad(val))
+        self._cos_z = np.cos(np.deg2rad(val))
+        self._apply_optics()
+
+
+    # Jaw attributes
+    # ==============
 
     @property
     def jaw(self):
-        jaws = list(np.array([
-                        self._colldb.jaw_LU.values,
-                        self._colldb.jaw_RU.values,
-                        self._colldb.jaw_LD.values,
-                        self._colldb.jaw_RD.values
-                    ]).T)
-        # Need special treatment if there are None's
-        def flip(jaw):
-            return None if jaw is None else -jaw
-        for i, jaw in enumerate(jaws):
-            # All 4 jaw points are the same
-            if jaw[0] == flip(jaw[1]) == jaw[2] == flip(jaw[3]):
-                jaws[i] = jaw[0]
-            # Upstream and downstream jaws are the same
-            # (all cases except angular alignment and/or tilt)
-            elif jaw[0] == jaw[2] and jaw[1] == jaw[3]:
-                jaws[i] = [ jaw[0], jaw[1] ]
-            else:
-                jaws[i] = [ [jaw[0],jaw[1]], [jaw[2],jaw[3]] ]
-        return pd.Series(jaws, index=self._colldb.index, dtype=object)
+        return self.jaw_U
+
+    @jaw.setter
+    def jaw(self, val):
+        if val is None:
+            val = self._side*OPEN_JAW
+        self.jaw_U = val
+
+    @property
+    def jaw_U(self):
+        if not np.isclose(self._jaw_U, self._side*OPEN_JAW, atol=1.e-10):  # open position
+            return self._jaw_U
+
+    @jaw_U.setter   # This moves both jaw_LU and jaw_LD in parallel
+    def jaw_U(self, val):
+        if val is None:
+            raise ValueError("Cannot set corner to None! Use open_jaws() or set jaw to None.")
+        self._jaw_U = val
+        self._update_gaps()
+
+    @property
+    def jaw_D(self):
+        if not np.isclose(self._jaw_U, self._side*OPEN_JAW, atol=1.e-10):  # open position
+            length = self.length
+            if self._side*self.bending_radius < 0:
+                # Correction for inner corner point
+                length -= self.width*np.sin(abs(self._bending_angle))
+            shift = np.tan(self._bending_angle/2)*self._cos_y + self._sin_y
+            return self._jaw_U + length*shift
+
+    @jaw_D.setter   # This moves both jaw_LU and jaw_LD in parallel
+    def jaw_D(self, val):
+        if val is None:
+            self.tilt = 0
+        else:
+            shift = (val - self._jaw_U )/self.length * np.cos(self._bending_angle/2)
+            self._sin_y  = shift*np.cos(self._bending_angle/2)
+            self._sin_y -= np.sin(self._bending_angle/2)*np.sqrt(1 - shift**2)
+            self._cos_y  = np.sqrt(1 - self._sin_y**2)
+            self._tan_y = self._sin_y / self._cos_y
+        self._update_gaps()
+
+    def open_jaws(self, keep_tilts=False):
+        self.jaw = None
+        if not keep_tilts:
+            self.tilt = 0
+
+    def _update_gaps(self):
+        # If we had set a value for the gap manually, this needs to be updated
+        # as well after setting the jaw
+        if self._gap_set_manually():
+            self._gap = self.gap
+
+
+    # Tilt attributes
+    # ===============
+
+    # TODO: tilts are in rad! Do we want that? It's a bit inconsistent with angle which is in deg...
 
     @property
-    def side(self):
-        return self._colldb.side
+    def tilt(self):
+        return round(np.arctan2(self._sin_y, self._cos_y), 10)
+
+    @tilt.setter   # This assumes jaw_U remains fixed (hence jaw_D changes)
+    def tilt(self, val):
+        if self.side == 'left':
+            if val < min(0, self.bending_angle/2):
+                print("Warning: Setting a negative tilt does not preserve the hierarchy, as the "
+                    + "crystal tightens towards the beam.")
+        elif self.side == 'right':
+            if val > min(0, -self.bending_angle/2):
+                print("Warning: Setting a positive tilt does not preserve the hierarchy, as the "
+                    + "crystal tightens towards the beam.")
+        self._sin_y = np.sin(val)
+        self._cos_y = np.cos(val)
+        self._tan_y = np.tan(val)
 
-    @side.setter
-    def side(self, sides):
-        self._set_property('side', sides, single_default_allowed=True)
-        self.gap = self.gap
+
+    # Optics
+    # ======
 
     @property
-    def gamma_rel(self):
-        return np.sqrt(self._beta_gamma_rel**2+1)
-
-    @gamma_rel.setter
-    def gamma_rel(self, gamma_rel):
-        self._beta_gamma_rel = np.sqrt(gamma_rel**2-1)
-        self._compute_jaws()
+    def optics(self):
+        return self._optics
+
+    def optics_ready(self):
+        return BaseCollimator.optics_ready(self)
+
+    def assign_optics(self, *, nemitt_x=None, nemitt_y=None, beta_gamma_rel=None, name=None, twiss=None,
+                      twiss_upstream=None, twiss_downstream=None):
+        return BaseCollimator.assign_optics(self, nemitt_x=nemitt_x, nemitt_y=nemitt_y,
+                                            beta_gamma_rel=beta_gamma_rel, name=name, twiss=twiss,
+                                            twiss_upstream=twiss_upstream, twiss_downstream=twiss_downstream)
+
+    @property
+    def nemitt_x(self):
+        return BaseCollimator.nemitt_x.fget(self)
+
+    @nemitt_x.setter
+    def nemitt_x(self, val):
+        BaseCollimator.nemitt_x.fset(self, val)
+
+    @property
+    def nemitt_y(self):
+        return BaseCollimator.nemitt_y.fget(self)
+
+    @nemitt_y.setter
+    def nemitt_y(self, val):
+        BaseCollimator.nemitt_y.fset(self, val)
 
     @property
     def emittance(self):
-        return [self._emitx, self._emity]
+        return BaseCollimator.emittance.fget(self)
 
     @emittance.setter
-    def emittance(self, emit):
-        if hasattr(emit, '__iter__'):
-            if isinstance(emit, str):
-                raise ValueError(f"The 'emit' setting has to be a number!")
-            elif len(emit) == 2:
-                self._emitx = emit[0]
-                self._emity = emit[1]
-            elif len(emit) == 1:
-                self._emitx = emit[0]
-                self._emity = emit[0]
-            else:
-                raise ValueError(f"The 'emit' setting must have one or two values (for emitx and emity)!")
-        else:
-            self._emitx = emit
-            self._emity = emit
-        self._compute_jaws()
-
-    @property
-    def align_to(self):
-        return self._colldb.align_to
-
-    @align_to.setter
-    def align_to(self, align):
-        self._set_property('align_to', align, single_default_allowed=True, limit_to=['front', 'center', 'back', 'angular'])
-        if np.any(self.align_to == 'maximum'):
-            raise NotImplementedError
-        s_front = self.s_center - self.active_length/2
-        s_center = self.s_center
-        s_back = self.s_center + self.active_length/2
-        mask = self.align_to == 'front'
-        self._colldb.loc[mask,'s_align_front'] = s_front[mask]
-        self._colldb.loc[mask,'s_align_back']  = s_front[mask]
-        mask = self.align_to == 'center'
-        self._colldb.loc[mask,'s_align_front'] = s_center[mask]
-        self._colldb.loc[mask,'s_align_back']  = s_center[mask]
-        mask = self.align_to == 'back'
-        self._colldb.loc[mask,'s_align_front'] = s_back[mask]
-        self._colldb.loc[mask,'s_align_back']  = s_back[mask]
-        mask = self.align_to == 'angular'
-        self._colldb.loc[mask,'s_align_front'] = s_front[mask]
-        self._colldb.loc[mask,'s_align_back']  = s_back[mask]
-        self._compute_jaws()
-
-    # TODO: when does this need to be unset?
-    @property
-    def _optics_is_ready(self):
-        pos = set(self._colldb.s_align_front.values) | set(self._colldb.s_align_back.values)
-        return np.all([s in self._optics.index for s in pos]) and self._beta_gamma_rel is not None
-
-    @property
-    def betx(self):
-        vals = np.array([
-            [ self._optics.loc[s,'betx'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'betx'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def bety(self):
-        vals = np.array([
-            [ self._optics.loc[s,'bety'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'bety'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def alfx(self):
-        vals = np.array([
-            [ self._optics.loc[s,'alfx'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'alfx'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)   
-
-    @property
-    def alfy(self):
-        vals = np.array([
-            [ self._optics.loc[s,'alfy'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'alfy'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-    
-    @property
-    def dx(self):
-        vals = np.array([
-            [ self._optics.loc[s,'dx'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'dx'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def dy(self):
-        vals = np.array([
-            [ self._optics.loc[s,'dy'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'dy'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-    
-    @property
-    def x(self):
-        vals = np.array([
-            [ self._optics.loc[s,'x'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'x'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def px(self):
-        vals = np.array([
-            [ self._optics.loc[s,'px'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'px'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def y(self):
-        vals = np.array([
-            [ self._optics.loc[s,'y'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'y'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def py(self):
-        vals = np.array([
-            [ self._optics.loc[s,'py'] if s in self._optics.index else None for s in self._colldb.s_align_front.values ],
-            [ self._optics.loc[s,'py'] if s in self._optics.index else None for s in self._colldb.s_align_back.values ]
-        ])
-        return pd.Series([ F if F == B else [F,B] for F,B in vals.T ], index=self._colldb.index, dtype=object)
-
-    @property
-    def beam_size(self):
-        if self._optics_is_ready:
-            beam_size = np.array([self._beam_size_front,self._beam_size_back])
-            return pd.Series([ F if F == B else [F,B] for F, B in beam_size.T ], index=self._colldb.index, dtype=object)
-        else:
-            return None
+    def emittance(self, val):
+        BaseCollimator.emittance.fset(self, val)
+
+    @property
+    def sigma(self):
+        return BaseCollimator.sigma.fget(self)
+
+    @property
+    def co(self):
+        return BaseCollimator.co.fget(self)
+
+    @property
+    def divergence(self):
+        return BaseCollimator.divergence.fget(self)
 
     @property
-    def _beam_size_front(self):
-        # TODO: curretnly only for angle_L
-        df = self._colldb
-        opt = self._optics
-        betx = opt.loc[df.s_align_front,'betx'].astype(float)
-        bety = opt.loc[df.s_align_front,'bety'].astype(float)
-        sigmax = np.sqrt(betx*self._emitx/self._beta_gamma_rel)
-        sigmay = np.sqrt(bety*self._emity/self._beta_gamma_rel)
-        result = np.sqrt(
-                    (sigmax*np.cos(np.float_(df.angle_L.values)*np.pi/180))**2
-                    + (sigmay*np.sin(np.float_(df.angle_L.values)*np.pi/180))**2
-                )
-        result.index = self._colldb.index
-        return result
-
-    @property
-    def _beam_size_back(self):
-        # TODO: curretnly only for angle_L
-        df = self._colldb
-        opt = self._optics
-        betx = opt.loc[df.s_align_back,'betx'].astype(float)
-        bety = opt.loc[df.s_align_back,'bety'].astype(float)
-        sigmax = np.sqrt(betx*self._emitx/self._beta_gamma_rel)
-        sigmay = np.sqrt(bety*self._emity/self._beta_gamma_rel)
-        result = np.sqrt(
-                    (sigmax*np.cos(np.float_(df.angle_L.values)*np.pi/180))**2
-                    + (sigmay*np.sin(np.float_(df.angle_L.values)*np.pi/180))**2
-                )
-        result.index = self._colldb.index
-        return result
-
-    # parking is defined with respect to closed orbit
-    # TODO: tilt
-    # 'upstr'  =>  'front'  en   'downstr'  =>  'back'
-    def _compute_jaws(self):
-        if self._optics_is_ready:
-            df = self._colldb
-            beam_size_front = self._beam_size_front
-            beam_size_back  = self._beam_size_back
-            jaw_LU = df['gap_L']*beam_size_front + self.offset
-            jaw_RU = df['gap_R']*beam_size_front - self.offset
-            jaw_LD = df['gap_L']*beam_size_back  + self.offset
-            jaw_RD = df['gap_R']*beam_size_back  - self.offset
-            df['jaw_LU'] = df['parking'] if df['gap_L'] is None else np.minimum(jaw_LU,df['parking'])
-            df['jaw_RU'] = -df['parking'] if df['gap_R'] is None else -np.minimum(jaw_RU,df['parking'])
-            df['jaw_LD'] = df['parking'] if df['gap_L'] is None else np.minimum(jaw_LD,df['parking'])
-            df['jaw_RD'] = -df['parking'] if df['gap_R'] is None else -np.minimum(jaw_RD,df['parking'])
-            # align crystals
-            opt = self._optics
-            df['align_angle'] = None
-            cry_mask = [c is not None for c in df.crystal]
-            df_cry = df[cry_mask]
-            if len(df_cry) > 0:
-                alfx = opt.loc[df_cry.s_align_front,'alfx'].astype(float).values
-                alfy = opt.loc[df_cry.s_align_front,'alfy'].astype(float).values
-                betx = opt.loc[df_cry.s_align_front,'betx'].astype(float).values
-                bety = opt.loc[df_cry.s_align_front,'bety'].astype(float).values
-                align_angle_x = -np.sqrt(self._emitx/self._beta_gamma_rel/betx)*alfx
-                align_angle_y = -np.sqrt(self._emity/self._beta_gamma_rel/bety)*alfy
-                align_angle = np.array([x if abs(ang) < 1e-6 else y
-                                        for x,y,ang in zip(align_angle_x,align_angle_y,df_cry.angle_L.values)])
-                df.loc[cry_mask, 'align_angle'] = align_angle*df_cry['gap_L']
-
-
-    # ---------------------------------------
-    # ------ Property setter functions ------
-    # ---------------------------------------
-
-    def _set_property(self, prop, vals, single_default_allowed=False, limit_to=[]):
-        df = self._colldb
-        if not isinstance(limit_to, (list, tuple, set)):
-            limit_to = [limit_to]
-        if isinstance(vals, dict):
-            for name, val in vals.items():
-                if name not in self.name:
-                    raise ValueError(f"Collimator {name} not found in CollimatorDatabase!")
-                if limit_to!=[] and val not in limit_to:
-                    raise ValueError(f"Cannot set {prop} to {val}. Choose from {limit_to}!")
-                df.loc[name, prop] = val
-        elif isinstance(vals, pd.Series) or isinstance(vals, list) or isinstance(vals, np.ndarray):
-            if len(vals) != len(self.name):
-                raise ValueError(f"The variable '{prop}' has a different length than the number of "
-                                + "collimators in the CollimatorDatabase. Use a dictionary instead.")
-            if limit_to!=[] and np.any([val not in limit_to for val in vals]):
-                raise ValueError(f"Cannot set {prop} to {vals}. Choose from {limit_to}!")
-            df[prop] = vals
+    def align(self):
+        return BaseCollimator.align.fget(self)
+
+    @align.setter
+    def align(self, val):
+        if val != 'upstream':
+            raise NotImplementedError("Crystals cannot be aligned to the downstream optics!")
+        BaseCollimator.align.fset(self, val)
+
+    def align_to_beam_divergence(self):
+        if not self.optics_ready():
+            raise ValueError("Optics not assigned! Cannot align to beam divergence.")
+        if self.gap is None:
+            raise ValueError("Need to set `gap` to align to beam divergence.")
+        self.tilt = self.divergence * self.gap
+
+
+    # Gap attributes
+    # ==============
+
+    @property
+    def gap(self):
+        if self.optics_ready() and self.jaw_U is not None:
+            return round((self.jaw_U - self.co[0])/self.sigma[0], 6)
+        elif not self._gap_set_manually():
+            return None
         else:
-            if single_default_allowed:
-                if limit_to!=[] and vals not in limit_to:
-                    raise ValueError(f"Cannot set {prop} to {vals}. Choose from {limit_to}!")
-                df[prop] = vals
-            else:
-                raise ValueError(f"Variable '{prop}' needs to be a pandas Series, dict, numpy array, or list!")
+            return self._gap
 
+    # Gap is always positive, irrespective of the side
+    @gap.setter
+    def gap(self, val):
+        if val is None:
+            val = OPEN_GAP
+            self.jaw = None
+        if hasattr(val, '__iter__'):
+            raise ValueError("The attribute `gap` should be a single value, not a list.")
+        if val <= 0:
+            raise ValueError(f"The field `gap` should be positive, but got {val}.")
+        self._gap = val
+        self._apply_optics()
+
+    def _gap_set_manually(self):
+        return not np.isclose(self._gap, OPEN_GAP)
+
+    def _apply_optics(self):
+        if self.optics_ready():
+            # Only if we have set a value for the gap manually, this needs to be updated
+            if self._gap_set_manually():
+                self.jaw_U = self._gap * self.sigma[0] + self.co[0]
+
+
+    # Other attributes
+    # ================
+
+    @property
+    def bending_radius(self):
+        return self._bending_radius
+
+    @bending_radius.setter
+    def bending_radius(self, bending_radius):
+        bending_angle = np.arcsin(self.length/bending_radius)
+        if abs(bending_angle) > np.pi/2:
+            raise ValueError("Bending angle cannot be larger than 90 degrees!")
+        self._bending_radius = bending_radius
+        self._bending_angle = bending_angle
+
+    @property
+    def bending_angle(self):
+        return self._bending_angle
+
+    @bending_angle.setter
+    def bending_angle(self, bending_angle):
+        if abs(bending_angle) > np.pi/2:
+            raise ValueError("Bending angle cannot be larger than 90 degrees!")
+        self._bending_angle = bending_angle
+        self._bending_radius = self.length / np.sin(bending_angle)
+
+    @property
+    def side(self):
+        return BaseCollimator.side.fget(self)
+
+    @side.setter
+    def side(self, val):
+        temp = self._side
+        BaseCollimator.side.fset(self, val)
+        if self._side == 0:
+            self._side = temp
+            raise ValueError("Crystal cannot be two-sided! Please set `side` "
+                           + "to 'left' or 'right'.")
+
+
+    # Methods
+    # =======
+
+    def enable_scattering(self):
+        BaseCollimator.enable_scattering(self)
+
+    def disable_scattering(self):
+        BaseCollimator.disable_scattering(self)
+
+    def _verify_consistency(self):
+        # Verify angles
+        ang = abs(np.arccos(self._cos_z))
+        ang = np.pi - ang if ang > np.pi/2 else ang
+        assert np.isclose(ang, abs(np.arcsin(self._sin_z)))
+        ang = abs(np.arccos(self._cos_y))
+        ang = np.pi - ang if ang > np.pi/2 else ang
+        assert np.isclose(ang, abs(np.arcsin(self._sin_y)))
+        assert np.isclose(self._sin_y/self._cos_y, self._tan_y)
+        # Verify bools
+        assert self._side in [-1, 1, 0]
+        assert isinstance(self.active, bool) or self.active in [0, 1]
+        assert isinstance(self.record_touches, bool) or self.record_touches in [0, 1]
+        assert isinstance(self.record_scatterings, bool) or self.record_scatterings in [0, 1]
+        # Crystal specific
+        assert np.isclose(self._bending_angle, np.arcsin(self.length/self._bending_radius))
 
-    def _set_property_LR(self, prop, vals):
-        df = self._colldb
-        correct_format = False
-        # The variable vals is a Series or a list
-        if isinstance(vals, pd.Series) or isinstance(vals, list) or isinstance(vals, np.ndarray):
-            correct_format = True
-            if len(vals) != len(self.name):
-                raise ValueError(f"The variable '{prop}' has a different length than the number of "
-                                + "collimators in the CollimatorDatabase. Use a dictionary instead.")
-            # Some of the vals are list (e.g. two different values for both gaps): loop over vals as dict
-            if any(hasattr(val, '__iter__') for val in vals):
-                vals = dict(zip(self.name, vals))
-            # All gaps are single values: use pandas-style assignment
-            else:
-                df[prop + "_L"] = vals
-                df[prop + "_R"] = vals
-        
-        # The variable vals is a dictionary
-        if isinstance(vals, dict):
-            correct_format = True
-            for name, val in vals.items():
-                if name not in self.name:
-                    raise ValueError(f"Collimator {name} not found in CollimatorDatabase!")
-                if hasattr(val, '__iter__'):
-                    if isinstance(val, str):
-                        raise ValueError(f"The '{prop}' setting has to be a number!")
-                    elif len(val) == 2:
-                        val_L = val[0]
-                        val_R = val[1]
-                    elif len(val) == 1:
-                        val_L = val[0]
-                        val_R = val[0]
-                    else:
-                        raise ValueError(f"The '{prop}' setting must have one or two values (for the left and the right jaw)!")
-                else:
-                    val_L = val
-                    val_R = val
-                df.loc[name, prop + "_L"] = val_L
-                df.loc[name, prop + "_R"] = val_R
-
-        if not correct_format:
-            raise ValueError("Variable '{prop}' needs to be a pandas Series, dict, numpy array, or list!")
-
-        df[prop + "_L"] = df[prop + "_L"].astype('object', copy=False)
-        df[prop + "_R"] = df[prop + "_R"].astype('object', copy=False)
-        # Check if collimator active
-        # Check if gap is list (assymetric jaws)
```

### Comparing `xcoll-0.3.6/xcoll/general.py` & `xcoll-0.4.0/xcoll/general.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # copyright ############################### #
 # This file is part of the Xcoll Package.   #
-# Copyright (c) CERN, 2023.                 #
+# Copyright (c) CERN, 2024.                 #
 # ######################################### #
 
 from pathlib import Path
 
 _pkg_root = Path(__file__).parent.absolute()
 
 citation = "F.F. Van der Veken, et al.: Recent Developments with the New Tools for Collimation Simulations in Xsuite, Proceedings of HB2023, Geneva, Switzerland."
 
 # ===================
 # Do not change
 # ===================
-__version__ = '0.3.6'
+__version__ = '0.4.0'
 # ===================
```

### Comparing `xcoll-0.3.6/xcoll/headers/checks.h` & `xcoll-0.4.0/xcoll/headers/checks.h`

 * *Files 4% similar despite different names*

```diff
@@ -27,9 +27,9 @@
     int8_t ruth_is_set = assert_rutherford_set(rng, part, RNG_ERR_RUTH_NOT_SET);
     if (!ruth_is_set){
         printf("Rutherford random generator not initialised!"); //only_for_context cpu_serial
         fflush(stdout);                                         //only_for_context cpu_serial
     }
     return is_tracking*rng_is_set*ruth_is_set;
 }
-    
+
 #endif /* XCOLL_CHECKS_H */
```

### Comparing `xcoll-0.3.6/xcoll/headers/particle_states.h` & `xcoll-0.4.0/xcoll/headers/particle_states.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 // copyright ############################### #
 // This file is part of the Xcoll Package.   #
-// Copyright (c) CERN, 2023.                 #
+// Copyright (c) CERN, 2024.                 #
 // ######################################### #
 
 #ifndef XCOLL_STATES_H
 #define XCOLL_STATES_H
 
 #define  XC_LOST_ON_EVEREST_BLOCK   -330
 #define  XC_LOST_ON_EVEREST_COLL    -331
@@ -17,9 +17,9 @@
 #define  XC_LOST_ON_GEANT4_CRYSTAL  -338
 #define  XC_LOST_ON_ABSORBER        -340
 
 #define  XC_ERR_INVALID_TRACK       -390
 #define  XC_ERR_NOT_IMPLEMENTED     -391
 #define  XC_ERR_INVALID_XOFIELD     -392
 #define  XC_ERR                     -399
-    
+
 #endif /* XCOLL_STATES_H */
```

### Comparing `xcoll-0.3.6/xcoll/impacts/interaction_types.py` & `xcoll-0.4.0/xcoll/interaction_record/interaction_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # copyright ############################### #
 # This file is part of the Xcoll Package.   #
-# Copyright (c) CERN, 2023.                 #
+# Copyright (c) CERN, 2024.                 #
 # ######################################### #
 
 
 source = r'''
 #ifndef XCOLL_INTERACTIONS_H
 #define XCOLL_INTERACTIONS_H
 
 #define  XC_UNITIALISED                     0        // NAN  // Do not use
 
-#define  XC_ENTER_JAW                      -1        // JI   // point (no children)    Set ds > 0 if entering later
-#define  XC_EXIT_JAW                       -2        // JO   // point (no children)
+#define  XC_ENTER_JAW_L                    -1        // JI   // point (no children)    Set ds > 0 if entering later
+#define  XC_ENTER_JAW_R                    -2        // JI   // point (no children)    Set ds > 0 if entering later
+#define  XC_EXIT_JAW                       -3        // JO   // point (no children)
+#define  XC_ENTER_JAW                      -4        // JI   // point (no children)    Set ds > 0 if entering later    still here for compatibility
 #define  XC_ABSORBED                        1        // A    // point (no children)    Don't use 0 (is default for unitialised)
 #define  XC_MULTIPLE_COULOMB_SCATTERING    13        // MCS  // continuous
 #define  XC_PN_ELASTIC                     14        // PN   // point (no children)
 #define  XC_PP_ELASTIC                     15        // PP   // point (no children)
 #define  XC_SINGLE_DIFFRACTIVE             16        // SD   // point (no children)
 #define  XC_COULOMB                        17        // C    // point (no children)
-#define  XC_RUTHERFORD                     18        // RU   // point (no children)
 #define  XC_CHANNELING                    100        // CH   // continuous
 #define  XC_DECHANNELING                  101        // DCH  // point (no children)
 #define  XC_VOLUME_REFLECTION_TRANS_CH    102        // VRCH // point (no children)    Transition region around +-xpcrit
 #define  XC_VOLUME_REFLECTION             103        // VR   // point (no children)
 #define  XC_VOLUME_REFLECTION_TRANS_MCS   104        // VRAM // point (no children)    Transition region around t_P
 #define  XC_MULTIPLE_COULOMB_TRANS_VR     105        // AMVR // continuous             Transition region around t_P + 2 xpcrit
 #define  XC_VOLUME_CAPTURE                106        // VC   // point (no children)
@@ -39,7 +40,13 @@
 }
 
 shortcuts = {
     int(line.split()[2]): line.split()[4]
     for line in source.split('\n')
     if len(line.split()) > 1 and line.split()[1][:3] == 'XC_' # select the source lines with the definitions
 }
+
+is_point = {
+    int(line.split()[2]): line.split()[6].lower() == 'point'
+    for line in source.split('\n')
+    if len(line.split()) > 1 and line.split()[1][:3] == 'XC_' # select the source lines with the definitions
+}
```

### Comparing `xcoll-0.3.6/xcoll/rf_sweep.py` & `xcoll-0.4.0/xcoll/rf_sweep.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # copyright ############################### #
 # This file is part of the Xcoll Package.   #
-# Copyright (c) CERN, 2023.                 #
+# Copyright (c) CERN, 2024.                 #
 # ######################################### #
 
 import numpy as np
 import scipy.constants as sc
 from time import perf_counter
 
 import xtrack as xt
```

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/everest/constants.h` & `xcoll-0.4.0/xcoll/scattering_routines/everest/constants.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/everest/jaw.h` & `xcoll-0.4.0/xcoll/scattering_routines/everest/properties.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,235 +1,175 @@
 // copyright ############################### #
 // This file is part of the Xcoll Package.   #
 // Copyright (c) CERN, 2023.                 #
 // ######################################### #
 
-#ifndef XCOLL_EVEREST_JAW_H
-#define XCOLL_EVEREST_JAW_H
+#ifndef XCOLL_EVEREST_PROP_H
+#define XCOLL_EVEREST_PROP_H
+#include <stdlib.h>
 #include <math.h>
 #include <stdio.h>
 
 
-
 /*gpufun*/
-double* tetat(LocalParticle* part, double t, double p) {
-    double teta = sqrt(t)/p;
-    double va = 0;
-    double vb  = 0;
-    double va2 = 0;
-    double vb2 = 0;
-    double r2  = 0;
-    double* result = (double*)malloc(2 * sizeof(double));
-    
-    while (1) {
-        va  = 2*RandomUniform_generate(part) - 1;
-        vb  = RandomUniform_generate(part);
-        va2 = pow(va,2);
-        vb2 = pow(vb,2);
-        r2  = va2 + vb2;
-        if(r2 < 1) {
-            break;
-        }
+void calculate_scattering(EverestData restrict everest, double p) {
+
+    // Material properties
+    double const anuc  = everest->coll->anuc;
+    double const rho   = everest->coll->rho;
+    double const bnref = everest->coll->bnref;
+    double csref[6];
+    csref[0] = everest->coll->csref[0];
+    csref[1] = everest->coll->csref[1];
+    csref[5] = everest->coll->csref[5];
+
+    double csect[6];
+
+    everest->ecmsq = 2*XC_PROTON_MASS*1.0e-3*p;
+    double ecmsq = everest->ecmsq;
+    everest->xln15s = log(0.15*ecmsq);
+
+    // Claudia Fit from COMPETE collaboration points "arXiv:hep-ph/0206172v1 19Jun2002"
+    double pptot = 0.041084 - 0.0023302*log(ecmsq) + 0.00031514*pow(log(ecmsq), 2.);
+
+    // Claudia used the fit from TOTEM for ppel (in barn)
+    double ppel = (11.7 - 1.59*log(ecmsq) + 0.134*pow(log(ecmsq), 2.))/1e3;   // TODO /1.e3
+
+    // Claudia updated SD cross that cointains renormalized pomeron flux (in barn)
+    double ppsd = (4.3 + 0.3*log(ecmsq))/1e3;
+
+    // Claudia new fit for the slope parameter with new data at sqrt(s)=7 TeV from TOTEM
+    everest->bpp = 7.156 + 1.439*log(sqrt(ecmsq));
+
+    // freep: number of nucleons involved in single scattering
+    double freep = XC_FREE_CO * pow(anuc,(1./3.));
+
+    // Rescale reference cross sections (only used for crystals)
+    csref[0] = csref[0]*everest->rescale_scattering;
+    csref[1] = csref[1]*everest->rescale_scattering;
+
+    // compute pp and pn el+single diff contributions to cross-section
+    // (both added : quasi-elastic or qel later)
+    csect[3] = freep * ppel;
+    csect[4] = freep * ppsd;
+
+    // correct TOT-CSec for energy dependence of qel
+    // TOT CS is here without a Coulomb contribution
+    csect[0] = csref[0] + freep * (pptot - XC_PP_CS_REF);
+    //Also correct inel-CS
+    if(csref[0] == 0) {   // TODO: is this needed?
+        csect[1] = 0;   // TODO: Is this correct? It seems as if it should be huge instead
+        everest->bn = 1.e10;
+    } else {
+        csect[1] = csref[1] * csect[0] / csref[0];
+        everest->bn = bnref * csect[0] / csref[0];
     }
-        
-    result[0] = (teta*((2*va)*vb))/r2;
-    result[1]  = (teta*(va2 - vb2))/r2;
-    return result;
-}
 
+    // Nuclear Elastic is TOT-inel-qel ( see definition in RPP)
+    csect[2] = csect[0] - csect[1] - csect[3] - csect[4];
+    csect[5] = csref[5];
 
-/*gpufun*/
-double* gettran(EverestData restrict everest, LocalParticle* part, double inter, double p) {
+    // Now add Coulomb
+    csect[0] += csect[5];
 
-    double* res = (double*)malloc(2 * sizeof(double));
+    // Interaction length in meter
+    everest->xintl = 1.0e-2*anuc/(XC_AVOGADRO*rho*csect[0]*1e-24);
 
-    // Neither if-statements below have an else, so defaulting function return to zero.
-    double result = 0;
-
-    if (inter==2) { // Nuclear Elastic
-        result = RandomExponential_generate(part)/everest->bn;
-
-    } else if (inter==3) { // pp Elastic
-        result = RandomExponential_generate(part)/everest->bpp;
-
-    } else if (inter==4) { // Single Diffractive
-        double xm2 = exp(RandomUniform_generate(part) * everest->xln15s);
-        double bsd = 0;
-        p = p * (1 - xm2/everest->ecmsq);
-    
-        if (xm2 < 2) {
-            bsd = 2 * everest->bpp;
-        } else if ((xm2 >= 2) & (xm2 <= 5)) {
-            bsd = ((106.0 - 17.0*xm2)*everest->bpp)/36.0;
-        } else {
-            bsd = (7*everest->bpp)/12.0;
+    // Filling CProb with cumulated normalised Cross-sections
+    int i;
+    everest->cprob[0] = 0;
+    if(csect[0] == 0) {   // TODO: is this needed?
+        for (i=1; i<5; ++i){
+            everest->cprob[i] = everest->cprob[i-1];  // TODO: seems wrong
+        }
+    } else {
+        for (i=1; i<5; ++i){
+            everest->cprob[i] = everest->cprob[i-1] + csect[i]/csect[0];
         }
-        result = RandomExponential_generate(part)/bsd;
-
-    } else if (inter==5) { // Coulomb
-        result = RandomRutherford_generate(everest->coll->rng, part);
     }
-
-    res[0] = result;
-    res[1] = p;
-    return res;
+    everest->cprob[5] = 1;
 }
 
 
 /*gpufun*/
-int ichoix(EverestData restrict everest, LocalParticle* part) {
+void calculate_ionisation_properties(EverestData restrict everest, double pc) {
 
-    double aran = RandomUniform_generate(part);
-    int i;
-    for (i = 0; i < 5; ++i) {
-        if (aran < everest->cprob[i]) {
-            break;
-        }
-    }
-    return i;
+    // Material properties
+    double const exenergy = everest->coll->exenergy;
+    double const rho      = everest->coll->rho;
+    double const anuc     = everest->coll->anuc;
+    double const zatom    = everest->coll->zatom;
+
+    // Energy variables
+    double momentum = pc*1.0e3;   // [MeV]
+    double energy   = sqrt(pow(momentum, 2.) + pow(XC_PROTON_MASS, 2.)); // [MeV]
+    double gammar   = energy/XC_PROTON_MASS;
+    double betar    = momentum/energy;
+    double bgr      = betar*gammar;
+    double mep      = XC_ELECTRON_MASS/XC_PROTON_MASS;  // Electron/proton
+
+    // tmax is max energy loss from kinematics
+    double tmax = 2.*XC_ELECTRON_MASS*pow(bgr, 2.)/ (1. + 2.*gammar*mep + pow(mep, 2.));  // [MeV]
+    double plen = sqrt(rho*zatom/anuc)*28.816e-6; // [MeV]
+
+    everest->energy_loss = 0.5*log(2.*XC_ELECTRON_MASS*bgr*bgr*tmax/pow(exenergy, 2.)) + 0.5;
+    everest->energy_loss -= pow(betar, 2.);
+    everest->energy_loss -= log(plen/exenergy);
+    everest->energy_loss -= log(bgr);
+    everest->energy_loss *= XC_BETHE_BLOCH*zatom/(anuc* pow(betar, 2.))*rho*1.0e-1; // [GeV/m]
+
+    everest->energy_loss_tail = 0.5*log(2*XC_ELECTRON_MASS*bgr*bgr*tmax/pow(exenergy, 2.)) + 0.5;
+    everest->energy_loss_tail -= pow(betar, 2.);
+    everest->energy_loss_tail -= log(plen/exenergy);
+    everest->energy_loss_tail -= log(bgr);
+    everest->energy_loss_tail += pow(tmax, 2.)/(8.*pow(energy, 2.));
+    everest->energy_loss_tail *= XC_BETHE_BLOCH*zatom/(anuc*pow(betar, 2.))*rho*1.0e-1; // [GeV/m]
+
+    double Tt = everest->energy_loss*1.0e3 + XC_BETHE_BLOCH*zatom*4.0e2*rho/(anuc*pow(betar, 2.)); // [MeV/m]
+
+    // Calculate different coefficients for terms in dz (length) to get the tail probability
+    double const prob_factor = rho*1.e2*XC_BETHE_BLOCH*zatom/(anuc*pow(betar, 2.));
+    everest->prob_tail_c1 = prob_factor * 0.5 / Tt;
+    everest->prob_tail_c2 = prob_factor * (
+                        tmax/(4.*pow(energy, 2.)) - 0.5/tmax
+                        - log(tmax/Tt)*pow(betar,2.)/(2.*tmax)
+                   );  // * dz
+    everest->prob_tail_c3 = prob_factor * pow(betar,2.)/(2.*tmax);  // * dz * log(dz)
+    everest->prob_tail_c4 = -prob_factor * Tt/(4.*pow(energy, 2.));  // * dz * dz
 }
 
 
 /*gpufun*/
-double* jaw(EverestData restrict everest, LocalParticle* part, double p, double zlm, int edge_check) {
+double calcionloss(EverestData restrict everest, LocalParticle* part, double length) {
 
-    double* result = (double*)malloc(3 * sizeof(double));
+#ifdef XCOLL_REFINE_ENERGY
+    calculate_ionisation_properties(everest, pc);
+#endif
 
-    double s;
-    double nabs = 0;
-    double rlen = zlm;
-    double m_dpodx = 0.;
-    double t;
-    double tx; 
-    double tz;
-
-    double rpp_in = LocalParticle_get_rpp(part);
-    double x  = LocalParticle_get_x(part);
-    double xp = LocalParticle_get_px(part)*rpp_in;
-    double z  = LocalParticle_get_y(part);
-    double zp = LocalParticle_get_py(part)*rpp_in;
-
-    if (everest->coll->only_mcs) {
-        double* res = mcs(everest, part, zlm, p, x, xp, z, zp, edge_check);
-        s = res[0];
-        x = res[1];
-        xp = res[2];
-        z = res[3];
-        zp = res[4];
-        free(res);
+    double prob_tail = everest->prob_tail_c1 + everest->prob_tail_c2 * length
+                     + everest->prob_tail_c3 * length * log(length) + everest->prob_tail_c4 * length * length;
 
+    if (RandomUniform_generate(part) < prob_tail) {
+        return everest->energy_loss_tail;
     } else {
-        // Do a step for a point-like interaction.
-        // Get monte-carlo interaction length.
-        while (1) {
-
-            calculate_ionisation_properties(everest, p);
-            double zlm1 = everest->xintl*RandomExponential_generate(part);
-
-            // If the monte-carlo interaction length is longer than the
-            // remaining collimator length, then put it to the remaining
-            // length, do multiple coulomb scattering and return.
-            // LAST STEP IN ITERATION LOOP
-            if (zlm1 > rlen) {
-                zlm1 = rlen;
-                double* res = mcs(everest, part, zlm1, p, x, xp, z, zp, edge_check);
-                s = res[0];
-                x = res[1];
-                xp = res[2];
-                z = res[3];
-                zp = res[4];
-                free(res);
-
-                s = zlm - rlen + s;
-                m_dpodx = calcionloss(everest, part, rlen);  // DM routine to include tail // TODO: should not be rlen but s after updating
-                p = p-m_dpodx*s; // This is correct: ionisation loss is only calculated and applied at end of while (break)
-                break;
-            }
-            // Otherwise do multi-coulomb scattering.
-            // REGULAR STEP IN ITERATION LOOP
-            double* res1 = mcs(everest, part, zlm1, p, x, xp, z, zp, edge_check);
-            s = res1[0];
-            x = res1[1];
-            xp = res1[2];
-            z = res1[3];
-            zp = res1[4];
-            free(res1);
-
-            // Check if particle is outside of collimator (X.LT.0) after
-            // MCS. If yes, calculate output longitudinal position (s),
-            // reduce momentum (output as dpop) and return.
-            // PARTICLE LEFT COLLIMATOR BEFORE ITS END.
-
-            if(x <= 0) {
-                s = zlm - rlen + s;
-                m_dpodx = calcionloss(everest, part, rlen);  // TODO: should not be rlen but s after updating
-                p = p-m_dpodx*s;  // correct
-                break;
-            }
-
-            // Check whether particle is absorbed. If yes, calculate output
-            // longitudinal position (s), reduce momentum (output as dpop)
-            // and return.
-            // PARTICLE WAS ABSORBED INSIDE COLLIMATOR DURING MCS.
-
-            int inter = ichoix(everest, part);
-            nabs = inter;
-            if (inter == 1) {
-                s = zlm - rlen + zlm1;
-                m_dpodx = calcionloss(everest, part, rlen);
-                p = p-m_dpodx*s;
-                break;
-            }
-
-
-            // Now treat the other types of interaction, as determined by ICHOIX:
-
-            // Nuclear-Elastic:          inter = 2
-            // pp Elastic:               inter = 3
-            // Single-Diffractive:       inter = 4    (changes momentum p)
-            // Coulomb:                  inter = 5
-
-            // Gettran returns some monte carlo number, that, as I believe, gives the rms transverse momentum transfer.
-
-            double* res2 = gettran(everest, part, inter, p);
-            t = res2[0];
-            p = res2[1];
-            free(res2);
-
-            // Tetat calculates from the rms transverse momentum transfer in
-            // monte-carlo fashion the angle changes for x and z planes. The
-            // angle change is proportional to SQRT(t) and 1/p, as expected.
-
-            double* res3 = tetat(part, t, p);
-            tx = res3[0];
-            tz = res3[1];
-            free(res3);
-
-            // Apply angle changes
-            xp = xp + tx;
-            zp = zp + tz;
-
-            // Treat single-diffractive scattering.    TODO: this does nothing??
-            if(inter == 4) {
-                // added update for s
-                s = zlm - rlen + zlm1;
-            }
-
-            // Calculate the remaining interaction length and close the iteration loop.
-            rlen = rlen - zlm1;
-        }
+        return everest->energy_loss;
     }
+}
+
+
+/*gpufun*/
+double calculate_dechanneling_length(EverestData restrict everest, double pc) {
+    // Material properties
+    double const exenergy = everest->coll->exenergy;
+
+    // Energy variables
+    double momentum = pc*1.0e3;   // [MeV]
+    double energy   = sqrt(pow(momentum, 2.) + pow(XC_PROTON_MASS, 2.)); // [MeV]
+    double gammar   = energy/XC_PROTON_MASS;
+
+    double const_dech = 256.0/(9.*pow(M_PI, 2.)) / (log(2.*XC_ELECTRON_MASS*gammar/exenergy) - 1.);
+    const_dech       *= (XC_SCREENING*XC_PLANE_DISTANCE)/(XC_CRADE*XC_ELECTRON_MASS)*1.0e3; // [m/GeV]
+    return const_dech;
+}
 
-    LocalParticle_set_x(part, x);
-    LocalParticle_set_px(part, xp/rpp_in);
-    LocalParticle_set_y(part, z);
-    LocalParticle_set_py(part, zp/rpp_in);
-    LocalParticle_add_to_s(part, s);  // TODO: is this correct with tilt etc?
-
-    result[0] = p;
-    result[1] = nabs;
-    result[2] = s;
-    return result;
-}  
-  
 
-#endif /* XCOLL_EVEREST_JAW_H */
+#endif /* XCOLL_EVEREST_PROP_H */
```

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/everest/materials.py` & `xcoll-0.4.0/xcoll/scattering_routines/everest/materials.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 
 # CLASS INHERITANCE DOES NOT WORK WITH DYNAMIC XOFIELDS
 # Because then the memory offsets between parent and child might no longer be the same,
 # as xobjects enforces a strict order: static fields first, and then dynamic fields.
 # See struct.py, in __new__ of MetaStruct
 
+# A HybridClass needs something to depend on, otherwise the class is added twice in the cdefs during compilation
+
 class GeneralMaterial(xo.HybridClass):
     _xofields = {
         'Z':                        xo.Float64,     # zatom
         'A':                        xo.Float64,     # anuc
         'density':                  xo.Float64,     # rho (g cm-3)
         'excitation_energy':        xo.Float64,     # exenergy
         'nuclear_radius':           xo.Float64,     # emr
```

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/build_fluka_input.py` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/build_fluka_input.py`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/ComponentMakefile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/Makefile` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/Makefile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/README` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/README`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.asciidoc`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.epub`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.html`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO.pdf`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__1.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__2.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__3.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__4.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__5.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__6.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/FlukaIO__7.png`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/doc/docbook.xsl`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Connection.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/Connection.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FlukaIOServer.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/FortranFlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/Message.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/Message.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/include/ParticleInfo.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.a`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/lib/libFlukaIO64.so`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/ClientTest.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/ServerTest.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/fclient.f`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/samples/fserver.f`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/Connection.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/Connection.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOHandshake.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FlukaIOServer.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/FortranFlukaIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.d`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/NetIO.o`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/src/tags` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/src/tags`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/ConnectionTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOServerTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FlukaIOTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/FortranFlukaIOTest.cpp`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeConnection.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeFlukaIOHandshake.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.c`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h` & `xcoll-0.4.0/xcoll/scattering_routines/fluka/flukaio/tests/fakes/FakeNetIO.h`

 * *Files identical despite different names*

### Comparing `xcoll-0.3.6/PKG-INFO` & `xcoll-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcoll
-Version: 0.3.6
+Version: 0.4.0
 Summary: Xsuite collimation package
 Home-page: https://github.com/xsuite/xcoll
 License: Apache 2.0
 Author: Frederik F. Van der Veken
 Author-email: frederik@cern.ch
 Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
```

