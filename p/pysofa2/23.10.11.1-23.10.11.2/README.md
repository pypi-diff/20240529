# Comparing `tmp/pysofa2-23.10.11.1.tar.gz` & `tmp/pysofa2-23.10.11.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysofa2-23.10.11.1.tar", last modified: Fri Nov  3 00:21:08 2023, max compression
+gzip compressed data, was "pysofa2-23.10.11.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pysofa2-23.10.11.1.tar` & `pysofa2-23.10.11.2.tar`

### file list

```diff
@@ -1,273 +1,259 @@
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2023-11-03 00:21:08.506555 pysofa2-23.10.11.1/
--rw-r--r--   0 duncan     (501) staff       (20)     1075 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/LICENSE
--rw-r--r--   0 duncan     (501) staff       (20)      121 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/MANIFEST.in
--rw-r--r--   0 duncan     (501) staff       (20)     1453 2023-11-03 00:21:08.506445 pysofa2-23.10.11.1/PKG-INFO
--rw-r--r--   0 duncan     (501) staff       (20)     1901 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/README.md
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2023-11-03 00:21:08.499342 pysofa2-23.10.11.1/pysofa2/
--rw-r--r--   0 duncan     (501) staff       (20)     1426 2023-11-03 00:13:17.000000 pysofa2-23.10.11.1/pysofa2/__about__.py
--rw-r--r--   0 duncan     (501) staff       (20)       62 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/pysofa2/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)   132475 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/pysofa2/sofa_wrapper.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2023-11-03 00:21:08.500401 pysofa2-23.10.11.1/pysofa2.egg-info/
--rw-r--r--   0 duncan     (501) staff       (20)     1453 2023-11-03 00:21:08.000000 pysofa2-23.10.11.1/pysofa2.egg-info/PKG-INFO
--rw-r--r--   0 duncan     (501) staff       (20)     6716 2023-11-03 00:21:08.000000 pysofa2-23.10.11.1/pysofa2.egg-info/SOURCES.txt
--rw-r--r--   0 duncan     (501) staff       (20)        1 2023-11-03 00:21:08.000000 pysofa2-23.10.11.1/pysofa2.egg-info/dependency_links.txt
--rw-r--r--   0 duncan     (501) staff       (20)       21 2023-11-03 00:21:08.000000 pysofa2-23.10.11.1/pysofa2.egg-info/requires.txt
--rw-r--r--   0 duncan     (501) staff       (20)       14 2023-11-03 00:21:08.000000 pysofa2-23.10.11.1/pysofa2.egg-info/top_level.txt
--rw-r--r--   0 duncan     (501) staff       (20)       20 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/requirements.txt
--rw-r--r--   0 duncan     (501) staff       (20)       38 2023-11-03 00:21:08.506585 pysofa2-23.10.11.1/setup.cfg
--rw-r--r--   0 duncan     (501) staff       (20)     1289 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/setup.py
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2023-11-03 00:21:08.505103 pysofa2-23.10.11.1/src/
--rw-r--r--   0 duncan     (501) staff       (20)     6491 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/a2af.c
--rw-r--r--   0 duncan     (501) staff       (20)     6397 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/a2tf.c
--rw-r--r--   0 duncan     (501) staff       (20)     6632 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ab.c
--rw-r--r--   0 duncan     (501) staff       (20)     7187 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ae2hd.c
--rw-r--r--   0 duncan     (501) staff       (20)     6122 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/af2a.c
--rw-r--r--   0 duncan     (501) staff       (20)     4990 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/anp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5018 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/anpm.c
--rw-r--r--   0 duncan     (501) staff       (20)     9173 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apcg.c
--rw-r--r--   0 duncan     (501) staff       (20)     9278 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apcg13.c
--rw-r--r--   0 duncan     (501) staff       (20)     9669 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apci.c
--rw-r--r--   0 duncan     (501) staff       (20)     9959 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apci13.c
--rw-r--r--   0 duncan     (501) staff       (20)    13488 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apco.c
--rw-r--r--   0 duncan     (501) staff       (20)    14195 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apco13.c
--rw-r--r--   0 duncan     (501) staff       (20)    11026 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apcs.c
--rw-r--r--   0 duncan     (501) staff       (20)     9686 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apcs13.c
--rw-r--r--   0 duncan     (501) staff       (20)     8285 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/aper.c
--rw-r--r--   0 duncan     (501) staff       (20)     9207 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/aper13.c
--rw-r--r--   0 duncan     (501) staff       (20)    11101 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apio.c
--rw-r--r--   0 duncan     (501) staff       (20)    12863 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/apio13.c
--rw-r--r--   0 duncan     (501) staff       (20)     7258 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atcc13.c
--rw-r--r--   0 duncan     (501) staff       (20)     7554 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atccq.c
--rw-r--r--   0 duncan     (501) staff       (20)     8253 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atci13.c
--rw-r--r--   0 duncan     (501) staff       (20)     7928 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atciq.c
--rw-r--r--   0 duncan     (501) staff       (20)     9820 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atciqn.c
--rw-r--r--   0 duncan     (501) staff       (20)     7729 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atciqz.c
--rw-r--r--   0 duncan     (501) staff       (20)    12497 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atco13.c
--rw-r--r--   0 duncan     (501) staff       (20)     7924 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atic13.c
--rw-r--r--   0 duncan     (501) staff       (20)     8735 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/aticq.c
--rw-r--r--   0 duncan     (501) staff       (20)    10631 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/aticqn.c
--rw-r--r--   0 duncan     (501) staff       (20)    11505 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atio13.c
--rw-r--r--   0 duncan     (501) staff       (20)    11523 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atioq.c
--rw-r--r--   0 duncan     (501) staff       (20)    12054 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atoc13.c
--rw-r--r--   0 duncan     (501) staff       (20)    11941 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atoi13.c
--rw-r--r--   0 duncan     (501) staff       (20)    11162 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/atoiq.c
--rw-r--r--   0 duncan     (501) staff       (20)     6712 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/bi00.c
--rw-r--r--   0 duncan     (501) staff       (20)     8475 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/bp00.c
--rw-r--r--   0 duncan     (501) staff       (20)     7301 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/bp06.c
--rw-r--r--   0 duncan     (501) staff       (20)     5826 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/bpn2xy.c
--rw-r--r--   0 duncan     (501) staff       (20)     7379 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2i00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7366 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2i00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     7169 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2i06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7596 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2ibpn.c
--rw-r--r--   0 duncan     (501) staff       (20)     7166 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2ixy.c
--rw-r--r--   0 duncan     (501) staff       (20)     6392 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2ixys.c
--rw-r--r--   0 duncan     (501) staff       (20)     5324 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2s.c
--rw-r--r--   0 duncan     (501) staff       (20)     8087 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2t00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7997 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2t00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     7958 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2t06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6654 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2tcio.c
--rw-r--r--   0 duncan     (501) staff       (20)     6681 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2teqx.c
--rw-r--r--   0 duncan     (501) staff       (20)     8787 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2tpe.c
--rw-r--r--   0 duncan     (501) staff       (20)     8250 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/c2txy.c
--rw-r--r--   0 duncan     (501) staff       (20)     6996 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/cal2jd.c
--rw-r--r--   0 duncan     (501) staff       (20)     4901 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/cp.c
--rw-r--r--   0 duncan     (501) staff       (20)     4994 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/cpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     4979 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/cr.c
--rw-r--r--   0 duncan     (501) staff       (20)     9830 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/d2dtf.c
--rw-r--r--   0 duncan     (501) staff       (20)     7262 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/d2tf.c
--rw-r--r--   0 duncan     (501) staff       (20)    13414 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/dat.c
--rw-r--r--   0 duncan     (501) staff       (20)    63581 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/dtdb.c
--rw-r--r--   0 duncan     (501) staff       (20)     9411 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/dtf2d.c
--rw-r--r--   0 duncan     (501) staff       (20)     7250 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eceq06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7268 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ecm06.c
--rw-r--r--   0 duncan     (501) staff       (20)     6946 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ee00.c
--rw-r--r--   0 duncan     (501) staff       (20)     7122 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ee00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7460 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ee00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     6649 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ee06a.c
--rw-r--r--   0 duncan     (501) staff       (20)    12393 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eect00.c
--rw-r--r--   0 duncan     (501) staff       (20)     6723 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eform.c
--rw-r--r--   0 duncan     (501) staff       (20)     7020 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eo06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6111 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eors.c
--rw-r--r--   0 duncan     (501) staff       (20)     6092 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/epb.c
--rw-r--r--   0 duncan     (501) staff       (20)     5363 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/epb2jd.c
--rw-r--r--   0 duncan     (501) staff       (20)     6023 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/epj.c
--rw-r--r--   0 duncan     (501) staff       (20)     5352 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/epj2jd.c
--rw-r--r--   0 duncan     (501) staff       (20)   152035 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/epv00.c
--rw-r--r--   0 duncan     (501) staff       (20)     7251 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eqec06.c
--rw-r--r--   0 duncan     (501) staff       (20)     6985 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/eqeq94.c
--rw-r--r--   0 duncan     (501) staff       (20)     7013 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/era00.c
--rw-r--r--   0 duncan     (501) staff       (20)     5824 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fad03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5791 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fae03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5917 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/faf03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5803 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/faju03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5793 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fal03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5793 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/falp03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5795 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fama03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5805 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fame03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5666 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fane03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5863 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/faom03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5770 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fapa03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5800 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fasa03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5664 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/faur03.c
--rw-r--r--   0 duncan     (501) staff       (20)     5799 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fave03.c
--rw-r--r--   0 duncan     (501) staff       (20)    12351 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk425.c
--rw-r--r--   0 duncan     (501) staff       (20)     9872 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk45z.c
--rw-r--r--   0 duncan     (501) staff       (20)    12409 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk524.c
--rw-r--r--   0 duncan     (501) staff       (20)     7423 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk52h.c
--rw-r--r--   0 duncan     (501) staff       (20)     7285 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk54z.c
--rw-r--r--   0 duncan     (501) staff       (20)     6217 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk5hip.c
--rw-r--r--   0 duncan     (501) staff       (20)     8113 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fk5hz.c
--rw-r--r--   0 duncan     (501) staff       (20)     7068 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fw2m.c
--rw-r--r--   0 duncan     (501) staff       (20)     6147 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/fw2xy.c
--rw-r--r--   0 duncan     (501) staff       (20)     8407 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/g2icrs.c
--rw-r--r--   0 duncan     (501) staff       (20)     6741 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gc2gd.c
--rw-r--r--   0 duncan     (501) staff       (20)     8370 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gc2gde.c
--rw-r--r--   0 duncan     (501) staff       (20)     6827 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gd2gc.c
--rw-r--r--   0 duncan     (501) staff       (20)     7015 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gd2gce.c
--rw-r--r--   0 duncan     (501) staff       (20)     7739 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gmst00.c
--rw-r--r--   0 duncan     (501) staff       (20)     7372 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gmst06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7720 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gmst82.c
--rw-r--r--   0 duncan     (501) staff       (20)     7490 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gst00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7791 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gst00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     7556 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gst06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7194 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gst06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7121 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/gst94.c
--rw-r--r--   0 duncan     (501) staff       (20)     7615 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/h2fk5.c
--rw-r--r--   0 duncan     (501) staff       (20)     7400 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/hd2ae.c
--rw-r--r--   0 duncan     (501) staff       (20)     6333 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/hd2pa.c
--rw-r--r--   0 duncan     (501) staff       (20)     8701 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/hfk5z.c
--rw-r--r--   0 duncan     (501) staff       (20)     8392 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/icrs2g.c
--rw-r--r--   0 duncan     (501) staff       (20)     4974 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ir.c
--rw-r--r--   0 duncan     (501) staff       (20)     8320 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/jd2cal.c
--rw-r--r--   0 duncan     (501) staff       (20)     7634 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/jdcalf.c
--rw-r--r--   0 duncan     (501) staff       (20)     7683 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ld.c
--rw-r--r--   0 duncan     (501) staff       (20)     8851 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ldn.c
--rw-r--r--   0 duncan     (501) staff       (20)     5982 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ldsun.c
--rw-r--r--   0 duncan     (501) staff       (20)     7027 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/lteceq.c
--rw-r--r--   0 duncan     (501) staff       (20)     7599 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ltecm.c
--rw-r--r--   0 duncan     (501) staff       (20)     7015 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/lteqec.c
--rw-r--r--   0 duncan     (501) staff       (20)     6520 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ltp.c
--rw-r--r--   0 duncan     (501) staff       (20)     6615 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ltpb.c
--rw-r--r--   0 duncan     (501) staff       (20)     7633 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ltpecl.c
--rw-r--r--   0 duncan     (501) staff       (20)     7912 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ltpequ.c
--rw-r--r--   0 duncan     (501) staff       (20)    28049 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/makefile
--rw-r--r--   0 duncan     (501) staff       (20)    25246 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/moon98.c
--rw-r--r--   0 duncan     (501) staff       (20)     6732 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/num00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6717 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/num00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     6664 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/num06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6061 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/numat.c
--rw-r--r--   0 duncan     (501) staff       (20)   119826 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/nut00a.c
--rw-r--r--   0 duncan     (501) staff       (20)    19043 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/nut00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     7846 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/nut06a.c
--rw-r--r--   0 duncan     (501) staff       (20)    16318 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/nut80.c
--rw-r--r--   0 duncan     (501) staff       (20)     6477 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/nutm80.c
--rw-r--r--   0 duncan     (501) staff       (20)     6449 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/obl06.c
--rw-r--r--   0 duncan     (501) staff       (20)     6494 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/obl80.c
--rw-r--r--   0 duncan     (501) staff       (20)    13817 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/p06e.c
--rw-r--r--   0 duncan     (501) staff       (20)     5033 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/p2pv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5280 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/p2s.c
--rw-r--r--   0 duncan     (501) staff       (20)     6784 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pap.c
--rw-r--r--   0 duncan     (501) staff       (20)     5654 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pas.c
--rw-r--r--   0 duncan     (501) staff       (20)     7834 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pb06.c
--rw-r--r--   0 duncan     (501) staff       (20)     5024 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pdp.c
--rw-r--r--   0 duncan     (501) staff       (20)     7987 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pfw06.c
--rw-r--r--   0 duncan     (501) staff       (20)    23269 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/plan94.c
--rw-r--r--   0 duncan     (501) staff       (20)     4902 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pm.c
--rw-r--r--   0 duncan     (501) staff       (20)     6583 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmat00.c
--rw-r--r--   0 duncan     (501) staff       (20)     6847 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmat06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7571 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmat76.c
--rw-r--r--   0 duncan     (501) staff       (20)     5094 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmp.c
--rw-r--r--   0 duncan     (501) staff       (20)     7071 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmpx.c
--rw-r--r--   0 duncan     (501) staff       (20)    10209 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pmsafe.c
--rw-r--r--   0 duncan     (501) staff       (20)     5499 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn.c
--rw-r--r--   0 duncan     (501) staff       (20)     9150 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn00.c
--rw-r--r--   0 duncan     (501) staff       (20)     8833 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     8824 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     9275 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn06.c
--rw-r--r--   0 duncan     (501) staff       (20)     8282 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pn06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6814 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pnm00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6801 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pnm00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     6858 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pnm06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6793 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pnm80.c
--rw-r--r--   0 duncan     (501) staff       (20)     6454 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pom00.c
--rw-r--r--   0 duncan     (501) staff       (20)     5091 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ppp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5279 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ppsp.c
--rw-r--r--   0 duncan     (501) staff       (20)     7836 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pr00.c
--rw-r--r--   0 duncan     (501) staff       (20)     8042 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/prec76.c
--rw-r--r--   0 duncan     (501) staff       (20)     4962 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pv2p.c
--rw-r--r--   0 duncan     (501) staff       (20)     6865 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pv2s.c
--rw-r--r--   0 duncan     (501) staff       (20)     5591 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvdpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5077 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvm.c
--rw-r--r--   0 duncan     (501) staff       (20)     5186 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvmpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5181 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvppv.c
--rw-r--r--   0 duncan     (501) staff       (20)    10033 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvstar.c
--rw-r--r--   0 duncan     (501) staff       (20)     7733 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvtob.c
--rw-r--r--   0 duncan     (501) staff       (20)     5377 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvu.c
--rw-r--r--   0 duncan     (501) staff       (20)     5284 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvup.c
--rw-r--r--   0 duncan     (501) staff       (20)     5846 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pvxpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5238 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/pxp.c
--rw-r--r--   0 duncan     (501) staff       (20)    11858 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/refco.c
--rw-r--r--   0 duncan     (501) staff       (20)     5990 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rm2v.c
--rw-r--r--   0 duncan     (501) staff       (20)     6001 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rv2m.c
--rw-r--r--   0 duncan     (501) staff       (20)     5811 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rx.c
--rw-r--r--   0 duncan     (501) staff       (20)     5302 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rxp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5419 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rxpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5341 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rxr.c
--rw-r--r--   0 duncan     (501) staff       (20)     5852 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ry.c
--rw-r--r--   0 duncan     (501) staff       (20)     5821 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/rz.c
--rw-r--r--   0 duncan     (501) staff       (20)    15650 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s00.c
--rw-r--r--   0 duncan     (501) staff       (20)     7797 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7788 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s00b.c
--rw-r--r--   0 duncan     (501) staff       (20)    15477 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7815 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     5077 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s2c.c
--rw-r--r--   0 duncan     (501) staff       (20)     5213 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s2p.c
--rw-r--r--   0 duncan     (501) staff       (20)     5640 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s2pv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5286 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/s2xpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5893 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sepp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5440 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/seps.c
--rw-r--r--   0 duncan     (501) staff       (20)    28715 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sofa.h
--rw-r--r--   0 duncan     (501) staff       (20)     7294 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sofam.h
--rw-r--r--   0 duncan     (501) staff       (20)     6592 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sp00.c
--rw-r--r--   0 duncan     (501) staff       (20)    10713 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/starpm.c
--rw-r--r--   0 duncan     (501) staff       (20)    11954 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/starpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5042 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sxp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5105 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/sxpv.c
--rw-r--r--   0 duncan     (501) staff       (20)   243734 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/t_sofa_c.c
--rw-r--r--   0 duncan     (501) staff       (20)     5880 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/taitt.c
--rw-r--r--   0 duncan     (501) staff       (20)     5936 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/taiut1.c
--rw-r--r--   0 duncan     (501) staff       (20)     7509 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/taiutc.c
--rw-r--r--   0 duncan     (501) staff       (20)     7022 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tcbtdb.c
--rw-r--r--   0 duncan     (501) staff       (20)     5879 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tcgtt.c
--rw-r--r--   0 duncan     (501) staff       (20)     7144 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tdbtcb.c
--rw-r--r--   0 duncan     (501) staff       (20)     6388 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tdbtt.c
--rw-r--r--   0 duncan     (501) staff       (20)     6097 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tf2a.c
--rw-r--r--   0 duncan     (501) staff       (20)     6101 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tf2d.c
--rw-r--r--   0 duncan     (501) staff       (20)     8685 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tpors.c
--rw-r--r--   0 duncan     (501) staff       (20)     8649 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tporv.c
--rw-r--r--   0 duncan     (501) staff       (20)     6534 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tpsts.c
--rw-r--r--   0 duncan     (501) staff       (20)     7337 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tpstv.c
--rw-r--r--   0 duncan     (501) staff       (20)     7253 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tpxes.c
--rw-r--r--   0 duncan     (501) staff       (20)     7927 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tpxev.c
--rw-r--r--   0 duncan     (501) staff       (20)     5140 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tr.c
--rw-r--r--   0 duncan     (501) staff       (20)     5268 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/trxp.c
--rw-r--r--   0 duncan     (501) staff       (20)     5584 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/trxpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     5876 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tttai.c
--rw-r--r--   0 duncan     (501) staff       (20)     5948 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tttcg.c
--rw-r--r--   0 duncan     (501) staff       (20)     6380 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/tttdb.c
--rw-r--r--   0 duncan     (501) staff       (20)     5829 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ttut1.c
--rw-r--r--   0 duncan     (501) staff       (20)     5933 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ut1tai.c
--rw-r--r--   0 duncan     (501) staff       (20)     5833 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ut1tt.c
--rw-r--r--   0 duncan     (501) staff       (20)     8814 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/ut1utc.c
--rw-r--r--   0 duncan     (501) staff       (20)     8318 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/utctai.c
--rw-r--r--   0 duncan     (501) staff       (20)     7472 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/utcut1.c
--rw-r--r--   0 duncan     (501) staff       (20)   133697 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/xy06.c
--rw-r--r--   0 duncan     (501) staff       (20)     7028 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/xys00a.c
--rw-r--r--   0 duncan     (501) staff       (20)     7014 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/xys00b.c
--rw-r--r--   0 duncan     (501) staff       (20)     7060 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/xys06a.c
--rw-r--r--   0 duncan     (501) staff       (20)     4829 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/zp.c
--rw-r--r--   0 duncan     (501) staff       (20)     4883 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/zpv.c
--rw-r--r--   0 duncan     (501) staff       (20)     4971 2023-10-12 01:49:05.000000 pysofa2-23.10.11.1/src/zr.c
-drwxr-xr-x   0 duncan     (501) staff       (20)        0 2023-11-03 00:21:08.506106 pysofa2-23.10.11.1/tests/
--rw-r--r--   0 duncan     (501) staff       (20)        0 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/tests/__init__.py
--rw-r--r--   0 duncan     (501) staff       (20)    12665 2023-11-02 23:34:45.000000 pysofa2-23.10.11.1/tests/test_all.py
+-rw-r--r--   0        0        0     4366 2024-05-29 16:13:16.902807 pysofa2-23.10.11.2/CMakeLists.txt
+-rw-r--r--   0        0        0     1075 2024-05-28 21:32:49.970457 pysofa2-23.10.11.2/LICENSE
+-rw-r--r--   0        0        0     1901 2024-05-28 21:32:49.970615 pysofa2-23.10.11.2/README.md
+-rw-r--r--   0        0        0     1236 2024-05-29 16:13:28.743005 pysofa2-23.10.11.2/pyproject.toml
+-rw-r--r--   0        0        0     1426 2024-05-28 21:32:49.970806 pysofa2-23.10.11.2/pysofa2/__about__.py
+-rw-r--r--   0        0        0       62 2024-05-28 21:32:49.970877 pysofa2-23.10.11.2/pysofa2/__init__.py
+-rw-r--r--   0        0        0   132478 2024-05-29 16:13:16.903494 pysofa2-23.10.11.2/pysofa2/sofa_wrapper.py
+-rw-r--r--   0        0        0     6491 2024-05-28 21:32:49.971695 pysofa2-23.10.11.2/src/a2af.c
+-rw-r--r--   0        0        0     6397 2024-05-28 21:32:49.971846 pysofa2-23.10.11.2/src/a2tf.c
+-rw-r--r--   0        0        0     6632 2024-05-28 21:32:49.971962 pysofa2-23.10.11.2/src/ab.c
+-rw-r--r--   0        0        0     7187 2024-05-28 21:32:49.972076 pysofa2-23.10.11.2/src/ae2hd.c
+-rw-r--r--   0        0        0     6122 2024-05-28 21:32:49.972253 pysofa2-23.10.11.2/src/af2a.c
+-rw-r--r--   0        0        0     4990 2024-05-28 21:32:49.972409 pysofa2-23.10.11.2/src/anp.c
+-rw-r--r--   0        0        0     5018 2024-05-28 21:32:49.972547 pysofa2-23.10.11.2/src/anpm.c
+-rw-r--r--   0        0        0     9173 2024-05-28 21:32:49.972658 pysofa2-23.10.11.2/src/apcg.c
+-rw-r--r--   0        0        0     9278 2024-05-28 21:32:49.972942 pysofa2-23.10.11.2/src/apcg13.c
+-rw-r--r--   0        0        0     9669 2024-05-28 21:32:49.973041 pysofa2-23.10.11.2/src/apci.c
+-rw-r--r--   0        0        0     9959 2024-05-28 21:32:49.973156 pysofa2-23.10.11.2/src/apci13.c
+-rw-r--r--   0        0        0    13488 2024-05-28 21:32:49.973293 pysofa2-23.10.11.2/src/apco.c
+-rw-r--r--   0        0        0    14195 2024-05-28 21:32:49.973460 pysofa2-23.10.11.2/src/apco13.c
+-rw-r--r--   0        0        0    11026 2024-05-28 21:32:49.973588 pysofa2-23.10.11.2/src/apcs.c
+-rw-r--r--   0        0        0     9686 2024-05-28 21:32:49.973694 pysofa2-23.10.11.2/src/apcs13.c
+-rw-r--r--   0        0        0     8285 2024-05-28 21:32:49.973822 pysofa2-23.10.11.2/src/aper.c
+-rw-r--r--   0        0        0     9207 2024-05-28 21:32:49.973942 pysofa2-23.10.11.2/src/aper13.c
+-rw-r--r--   0        0        0    11101 2024-05-28 21:32:49.974038 pysofa2-23.10.11.2/src/apio.c
+-rw-r--r--   0        0        0    12863 2024-05-28 21:32:49.974159 pysofa2-23.10.11.2/src/apio13.c
+-rw-r--r--   0        0        0     7258 2024-05-28 21:32:49.974322 pysofa2-23.10.11.2/src/atcc13.c
+-rw-r--r--   0        0        0     7554 2024-05-28 21:32:49.974476 pysofa2-23.10.11.2/src/atccq.c
+-rw-r--r--   0        0        0     8253 2024-05-28 21:32:49.974582 pysofa2-23.10.11.2/src/atci13.c
+-rw-r--r--   0        0        0     7928 2024-05-28 21:32:49.974682 pysofa2-23.10.11.2/src/atciq.c
+-rw-r--r--   0        0        0     9820 2024-05-28 21:32:49.974782 pysofa2-23.10.11.2/src/atciqn.c
+-rw-r--r--   0        0        0     7729 2024-05-28 21:32:49.974925 pysofa2-23.10.11.2/src/atciqz.c
+-rw-r--r--   0        0        0    12497 2024-05-28 21:32:49.975042 pysofa2-23.10.11.2/src/atco13.c
+-rw-r--r--   0        0        0     7924 2024-05-28 21:32:49.975160 pysofa2-23.10.11.2/src/atic13.c
+-rw-r--r--   0        0        0     8735 2024-05-28 21:32:49.975274 pysofa2-23.10.11.2/src/aticq.c
+-rw-r--r--   0        0        0    10631 2024-05-28 21:32:49.975373 pysofa2-23.10.11.2/src/aticqn.c
+-rw-r--r--   0        0        0    11505 2024-05-28 21:32:49.975458 pysofa2-23.10.11.2/src/atio13.c
+-rw-r--r--   0        0        0    11523 2024-05-28 21:32:49.975538 pysofa2-23.10.11.2/src/atioq.c
+-rw-r--r--   0        0        0    12054 2024-05-28 21:32:49.975660 pysofa2-23.10.11.2/src/atoc13.c
+-rw-r--r--   0        0        0    11941 2024-05-28 21:32:49.975747 pysofa2-23.10.11.2/src/atoi13.c
+-rw-r--r--   0        0        0    11162 2024-05-28 21:32:49.975861 pysofa2-23.10.11.2/src/atoiq.c
+-rw-r--r--   0        0        0     6712 2024-05-28 21:32:49.976011 pysofa2-23.10.11.2/src/bi00.c
+-rw-r--r--   0        0        0     8475 2024-05-28 21:32:49.976161 pysofa2-23.10.11.2/src/bp00.c
+-rw-r--r--   0        0        0     7301 2024-05-28 21:32:49.976288 pysofa2-23.10.11.2/src/bp06.c
+-rw-r--r--   0        0        0     5826 2024-05-28 21:32:49.976414 pysofa2-23.10.11.2/src/bpn2xy.c
+-rw-r--r--   0        0        0     7379 2024-05-28 21:32:49.976582 pysofa2-23.10.11.2/src/c2i00a.c
+-rw-r--r--   0        0        0     7366 2024-05-28 21:32:49.976691 pysofa2-23.10.11.2/src/c2i00b.c
+-rw-r--r--   0        0        0     7169 2024-05-28 21:32:49.976785 pysofa2-23.10.11.2/src/c2i06a.c
+-rw-r--r--   0        0        0     7596 2024-05-28 21:32:49.976904 pysofa2-23.10.11.2/src/c2ibpn.c
+-rw-r--r--   0        0        0     7166 2024-05-28 21:32:49.976997 pysofa2-23.10.11.2/src/c2ixy.c
+-rw-r--r--   0        0        0     6392 2024-05-28 21:32:49.977105 pysofa2-23.10.11.2/src/c2ixys.c
+-rw-r--r--   0        0        0     5324 2024-05-28 21:32:49.977239 pysofa2-23.10.11.2/src/c2s.c
+-rw-r--r--   0        0        0     8087 2024-05-28 21:32:49.977339 pysofa2-23.10.11.2/src/c2t00a.c
+-rw-r--r--   0        0        0     7997 2024-05-28 21:32:49.977443 pysofa2-23.10.11.2/src/c2t00b.c
+-rw-r--r--   0        0        0     7958 2024-05-28 21:32:49.977557 pysofa2-23.10.11.2/src/c2t06a.c
+-rw-r--r--   0        0        0     6654 2024-05-28 21:32:49.977674 pysofa2-23.10.11.2/src/c2tcio.c
+-rw-r--r--   0        0        0     6681 2024-05-28 21:32:49.977786 pysofa2-23.10.11.2/src/c2teqx.c
+-rw-r--r--   0        0        0     8787 2024-05-28 21:32:49.977881 pysofa2-23.10.11.2/src/c2tpe.c
+-rw-r--r--   0        0        0     8250 2024-05-28 21:32:49.977968 pysofa2-23.10.11.2/src/c2txy.c
+-rw-r--r--   0        0        0     6996 2024-05-28 21:32:49.978074 pysofa2-23.10.11.2/src/cal2jd.c
+-rw-r--r--   0        0        0     4901 2024-05-28 21:32:49.978177 pysofa2-23.10.11.2/src/cp.c
+-rw-r--r--   0        0        0     4994 2024-05-28 21:32:49.978282 pysofa2-23.10.11.2/src/cpv.c
+-rw-r--r--   0        0        0     4979 2024-05-28 21:32:49.978383 pysofa2-23.10.11.2/src/cr.c
+-rw-r--r--   0        0        0     9830 2024-05-28 21:32:49.978527 pysofa2-23.10.11.2/src/d2dtf.c
+-rw-r--r--   0        0        0     7262 2024-05-28 21:32:49.978627 pysofa2-23.10.11.2/src/d2tf.c
+-rw-r--r--   0        0        0    13414 2024-05-28 21:32:49.978752 pysofa2-23.10.11.2/src/dat.c
+-rw-r--r--   0        0        0    63581 2024-05-28 21:32:49.978856 pysofa2-23.10.11.2/src/dtdb.c
+-rw-r--r--   0        0        0     9411 2024-05-28 21:32:49.978973 pysofa2-23.10.11.2/src/dtf2d.c
+-rw-r--r--   0        0        0     7250 2024-05-28 21:32:49.979074 pysofa2-23.10.11.2/src/eceq06.c
+-rw-r--r--   0        0        0     7268 2024-05-28 21:32:49.979179 pysofa2-23.10.11.2/src/ecm06.c
+-rw-r--r--   0        0        0     6946 2024-05-28 21:32:49.979301 pysofa2-23.10.11.2/src/ee00.c
+-rw-r--r--   0        0        0     7122 2024-05-28 21:32:49.979414 pysofa2-23.10.11.2/src/ee00a.c
+-rw-r--r--   0        0        0     7460 2024-05-28 21:32:49.979533 pysofa2-23.10.11.2/src/ee00b.c
+-rw-r--r--   0        0        0     6649 2024-05-28 21:32:49.979632 pysofa2-23.10.11.2/src/ee06a.c
+-rw-r--r--   0        0        0    12393 2024-05-28 21:32:49.979734 pysofa2-23.10.11.2/src/eect00.c
+-rw-r--r--   0        0        0     6723 2024-05-28 21:32:49.979835 pysofa2-23.10.11.2/src/eform.c
+-rw-r--r--   0        0        0     7020 2024-05-28 21:32:49.979935 pysofa2-23.10.11.2/src/eo06a.c
+-rw-r--r--   0        0        0     6111 2024-05-28 21:32:49.980038 pysofa2-23.10.11.2/src/eors.c
+-rw-r--r--   0        0        0     6092 2024-05-28 21:32:49.980142 pysofa2-23.10.11.2/src/epb.c
+-rw-r--r--   0        0        0     5363 2024-05-28 21:32:49.980232 pysofa2-23.10.11.2/src/epb2jd.c
+-rw-r--r--   0        0        0     6023 2024-05-28 21:32:49.980330 pysofa2-23.10.11.2/src/epj.c
+-rw-r--r--   0        0        0     5352 2024-05-28 21:32:49.980424 pysofa2-23.10.11.2/src/epj2jd.c
+-rw-r--r--   0        0        0   152035 2024-05-28 21:32:49.980785 pysofa2-23.10.11.2/src/epv00.c
+-rw-r--r--   0        0        0     7251 2024-05-28 21:32:49.980923 pysofa2-23.10.11.2/src/eqec06.c
+-rw-r--r--   0        0        0     6985 2024-05-28 21:32:49.981029 pysofa2-23.10.11.2/src/eqeq94.c
+-rw-r--r--   0        0        0     7013 2024-05-28 21:32:49.981132 pysofa2-23.10.11.2/src/era00.c
+-rw-r--r--   0        0        0     5824 2024-05-28 21:32:49.981243 pysofa2-23.10.11.2/src/fad03.c
+-rw-r--r--   0        0        0     5791 2024-05-28 21:32:49.981345 pysofa2-23.10.11.2/src/fae03.c
+-rw-r--r--   0        0        0     5917 2024-05-28 21:32:49.981435 pysofa2-23.10.11.2/src/faf03.c
+-rw-r--r--   0        0        0     5803 2024-05-28 21:32:49.981540 pysofa2-23.10.11.2/src/faju03.c
+-rw-r--r--   0        0        0     5793 2024-05-28 21:32:49.981630 pysofa2-23.10.11.2/src/fal03.c
+-rw-r--r--   0        0        0     5793 2024-05-28 21:32:49.981717 pysofa2-23.10.11.2/src/falp03.c
+-rw-r--r--   0        0        0     5795 2024-05-28 21:32:49.981808 pysofa2-23.10.11.2/src/fama03.c
+-rw-r--r--   0        0        0     5805 2024-05-28 21:32:49.981896 pysofa2-23.10.11.2/src/fame03.c
+-rw-r--r--   0        0        0     5666 2024-05-28 21:32:49.981988 pysofa2-23.10.11.2/src/fane03.c
+-rw-r--r--   0        0        0     5863 2024-05-28 21:32:49.982085 pysofa2-23.10.11.2/src/faom03.c
+-rw-r--r--   0        0        0     5770 2024-05-28 21:32:49.982180 pysofa2-23.10.11.2/src/fapa03.c
+-rw-r--r--   0        0        0     5800 2024-05-28 21:32:49.982273 pysofa2-23.10.11.2/src/fasa03.c
+-rw-r--r--   0        0        0     5664 2024-05-28 21:32:49.982367 pysofa2-23.10.11.2/src/faur03.c
+-rw-r--r--   0        0        0     5799 2024-05-28 21:32:49.982456 pysofa2-23.10.11.2/src/fave03.c
+-rw-r--r--   0        0        0    12351 2024-05-28 21:32:49.982598 pysofa2-23.10.11.2/src/fk425.c
+-rw-r--r--   0        0        0     9872 2024-05-28 21:32:49.982681 pysofa2-23.10.11.2/src/fk45z.c
+-rw-r--r--   0        0        0    12409 2024-05-28 21:32:49.982804 pysofa2-23.10.11.2/src/fk524.c
+-rw-r--r--   0        0        0     7423 2024-05-28 21:32:49.982924 pysofa2-23.10.11.2/src/fk52h.c
+-rw-r--r--   0        0        0     7285 2024-05-28 21:32:49.983028 pysofa2-23.10.11.2/src/fk54z.c
+-rw-r--r--   0        0        0     6217 2024-05-28 21:32:49.983130 pysofa2-23.10.11.2/src/fk5hip.c
+-rw-r--r--   0        0        0     8113 2024-05-28 21:32:49.983231 pysofa2-23.10.11.2/src/fk5hz.c
+-rw-r--r--   0        0        0     7068 2024-05-28 21:32:49.983339 pysofa2-23.10.11.2/src/fw2m.c
+-rw-r--r--   0        0        0     6147 2024-05-28 21:32:49.983436 pysofa2-23.10.11.2/src/fw2xy.c
+-rw-r--r--   0        0        0     8407 2024-05-28 21:32:49.983541 pysofa2-23.10.11.2/src/g2icrs.c
+-rw-r--r--   0        0        0     6741 2024-05-28 21:32:49.983643 pysofa2-23.10.11.2/src/gc2gd.c
+-rw-r--r--   0        0        0     8370 2024-05-28 21:32:49.983734 pysofa2-23.10.11.2/src/gc2gde.c
+-rw-r--r--   0        0        0     6827 2024-05-28 21:32:49.983844 pysofa2-23.10.11.2/src/gd2gc.c
+-rw-r--r--   0        0        0     7015 2024-05-28 21:32:49.983948 pysofa2-23.10.11.2/src/gd2gce.c
+-rw-r--r--   0        0        0     7739 2024-05-28 21:32:49.984064 pysofa2-23.10.11.2/src/gmst00.c
+-rw-r--r--   0        0        0     7372 2024-05-28 21:32:49.984177 pysofa2-23.10.11.2/src/gmst06.c
+-rw-r--r--   0        0        0     7720 2024-05-28 21:32:49.984305 pysofa2-23.10.11.2/src/gmst82.c
+-rw-r--r--   0        0        0     7490 2024-05-28 21:32:49.984410 pysofa2-23.10.11.2/src/gst00a.c
+-rw-r--r--   0        0        0     7791 2024-05-28 21:32:49.984513 pysofa2-23.10.11.2/src/gst00b.c
+-rw-r--r--   0        0        0     7556 2024-05-28 21:32:49.984621 pysofa2-23.10.11.2/src/gst06.c
+-rw-r--r--   0        0        0     7194 2024-05-28 21:32:49.984715 pysofa2-23.10.11.2/src/gst06a.c
+-rw-r--r--   0        0        0     7121 2024-05-28 21:32:49.984807 pysofa2-23.10.11.2/src/gst94.c
+-rw-r--r--   0        0        0     7615 2024-05-28 21:32:49.984907 pysofa2-23.10.11.2/src/h2fk5.c
+-rw-r--r--   0        0        0     7400 2024-05-28 21:32:49.985023 pysofa2-23.10.11.2/src/hd2ae.c
+-rw-r--r--   0        0        0     6333 2024-05-28 21:32:49.985134 pysofa2-23.10.11.2/src/hd2pa.c
+-rw-r--r--   0        0        0     8701 2024-05-28 21:32:49.985253 pysofa2-23.10.11.2/src/hfk5z.c
+-rw-r--r--   0        0        0     8392 2024-05-28 21:32:49.985360 pysofa2-23.10.11.2/src/icrs2g.c
+-rw-r--r--   0        0        0     4974 2024-05-28 21:32:49.985450 pysofa2-23.10.11.2/src/ir.c
+-rw-r--r--   0        0        0     8320 2024-05-28 21:32:49.985537 pysofa2-23.10.11.2/src/jd2cal.c
+-rw-r--r--   0        0        0     7634 2024-05-28 21:32:49.985645 pysofa2-23.10.11.2/src/jdcalf.c
+-rw-r--r--   0        0        0     7683 2024-05-28 21:32:49.985759 pysofa2-23.10.11.2/src/ld.c
+-rw-r--r--   0        0        0     8851 2024-05-28 21:32:49.985859 pysofa2-23.10.11.2/src/ldn.c
+-rw-r--r--   0        0        0     5982 2024-05-28 21:32:49.985961 pysofa2-23.10.11.2/src/ldsun.c
+-rw-r--r--   0        0        0     7027 2024-05-28 21:32:49.986065 pysofa2-23.10.11.2/src/lteceq.c
+-rw-r--r--   0        0        0     7599 2024-05-28 21:32:49.986166 pysofa2-23.10.11.2/src/ltecm.c
+-rw-r--r--   0        0        0     7015 2024-05-28 21:32:49.986259 pysofa2-23.10.11.2/src/lteqec.c
+-rw-r--r--   0        0        0     6520 2024-05-28 21:32:49.986348 pysofa2-23.10.11.2/src/ltp.c
+-rw-r--r--   0        0        0     6615 2024-05-28 21:32:49.986443 pysofa2-23.10.11.2/src/ltpb.c
+-rw-r--r--   0        0        0     7633 2024-05-28 21:32:49.986546 pysofa2-23.10.11.2/src/ltpecl.c
+-rw-r--r--   0        0        0     7912 2024-05-28 21:32:49.986647 pysofa2-23.10.11.2/src/ltpequ.c
+-rw-r--r--   0        0        0    28049 2024-05-28 21:32:49.986733 pysofa2-23.10.11.2/src/makefile
+-rw-r--r--   0        0        0    25246 2024-05-28 21:32:49.986817 pysofa2-23.10.11.2/src/moon98.c
+-rw-r--r--   0        0        0     6732 2024-05-28 21:32:49.986934 pysofa2-23.10.11.2/src/num00a.c
+-rw-r--r--   0        0        0     6717 2024-05-28 21:32:49.987033 pysofa2-23.10.11.2/src/num00b.c
+-rw-r--r--   0        0        0     6664 2024-05-28 21:32:49.987125 pysofa2-23.10.11.2/src/num06a.c
+-rw-r--r--   0        0        0     6061 2024-05-28 21:32:49.987227 pysofa2-23.10.11.2/src/numat.c
+-rw-r--r--   0        0        0   119826 2024-05-28 21:32:49.987543 pysofa2-23.10.11.2/src/nut00a.c
+-rw-r--r--   0        0        0    19043 2024-05-28 21:32:49.987654 pysofa2-23.10.11.2/src/nut00b.c
+-rw-r--r--   0        0        0     7846 2024-05-28 21:32:49.987770 pysofa2-23.10.11.2/src/nut06a.c
+-rw-r--r--   0        0        0    16318 2024-05-28 21:32:49.987869 pysofa2-23.10.11.2/src/nut80.c
+-rw-r--r--   0        0        0     6477 2024-05-28 21:32:49.987950 pysofa2-23.10.11.2/src/nutm80.c
+-rw-r--r--   0        0        0     6449 2024-05-28 21:32:49.988050 pysofa2-23.10.11.2/src/obl06.c
+-rw-r--r--   0        0        0     6494 2024-05-28 21:32:49.988144 pysofa2-23.10.11.2/src/obl80.c
+-rw-r--r--   0        0        0    13817 2024-05-28 21:32:49.988234 pysofa2-23.10.11.2/src/p06e.c
+-rw-r--r--   0        0        0     5033 2024-05-28 21:32:49.988323 pysofa2-23.10.11.2/src/p2pv.c
+-rw-r--r--   0        0        0     5280 2024-05-28 21:32:49.988411 pysofa2-23.10.11.2/src/p2s.c
+-rw-r--r--   0        0        0     6784 2024-05-28 21:32:49.988506 pysofa2-23.10.11.2/src/pap.c
+-rw-r--r--   0        0        0     5654 2024-05-28 21:32:49.988588 pysofa2-23.10.11.2/src/pas.c
+-rw-r--r--   0        0        0     7834 2024-05-28 21:32:49.988688 pysofa2-23.10.11.2/src/pb06.c
+-rw-r--r--   0        0        0     5024 2024-05-28 21:32:49.988784 pysofa2-23.10.11.2/src/pdp.c
+-rw-r--r--   0        0        0     7987 2024-05-28 21:32:49.988887 pysofa2-23.10.11.2/src/pfw06.c
+-rw-r--r--   0        0        0    23269 2024-05-28 21:32:49.989011 pysofa2-23.10.11.2/src/plan94.c
+-rw-r--r--   0        0        0     4902 2024-05-28 21:32:49.989129 pysofa2-23.10.11.2/src/pm.c
+-rw-r--r--   0        0        0     6583 2024-05-28 21:32:49.989216 pysofa2-23.10.11.2/src/pmat00.c
+-rw-r--r--   0        0        0     6847 2024-05-28 21:32:49.989305 pysofa2-23.10.11.2/src/pmat06.c
+-rw-r--r--   0        0        0     7571 2024-05-28 21:32:49.989408 pysofa2-23.10.11.2/src/pmat76.c
+-rw-r--r--   0        0        0     5094 2024-05-28 21:32:49.989497 pysofa2-23.10.11.2/src/pmp.c
+-rw-r--r--   0        0        0     7071 2024-05-28 21:32:49.989601 pysofa2-23.10.11.2/src/pmpx.c
+-rw-r--r--   0        0        0    10209 2024-05-28 21:32:49.989689 pysofa2-23.10.11.2/src/pmsafe.c
+-rw-r--r--   0        0        0     5499 2024-05-28 21:32:49.989772 pysofa2-23.10.11.2/src/pn.c
+-rw-r--r--   0        0        0     9150 2024-05-28 21:32:49.989856 pysofa2-23.10.11.2/src/pn00.c
+-rw-r--r--   0        0        0     8833 2024-05-28 21:32:49.989948 pysofa2-23.10.11.2/src/pn00a.c
+-rw-r--r--   0        0        0     8824 2024-05-28 21:32:49.990043 pysofa2-23.10.11.2/src/pn00b.c
+-rw-r--r--   0        0        0     9275 2024-05-28 21:32:49.990125 pysofa2-23.10.11.2/src/pn06.c
+-rw-r--r--   0        0        0     8282 2024-05-28 21:32:49.990215 pysofa2-23.10.11.2/src/pn06a.c
+-rw-r--r--   0        0        0     6814 2024-05-28 21:32:49.990326 pysofa2-23.10.11.2/src/pnm00a.c
+-rw-r--r--   0        0        0     6801 2024-05-28 21:32:49.990427 pysofa2-23.10.11.2/src/pnm00b.c
+-rw-r--r--   0        0        0     6858 2024-05-28 21:32:49.990538 pysofa2-23.10.11.2/src/pnm06a.c
+-rw-r--r--   0        0        0     6793 2024-05-28 21:32:49.990623 pysofa2-23.10.11.2/src/pnm80.c
+-rw-r--r--   0        0        0     6454 2024-05-28 21:32:49.990754 pysofa2-23.10.11.2/src/pom00.c
+-rw-r--r--   0        0        0     5091 2024-05-28 21:32:49.990838 pysofa2-23.10.11.2/src/ppp.c
+-rw-r--r--   0        0        0     5279 2024-05-28 21:32:49.990934 pysofa2-23.10.11.2/src/ppsp.c
+-rw-r--r--   0        0        0     7836 2024-05-28 21:32:49.991018 pysofa2-23.10.11.2/src/pr00.c
+-rw-r--r--   0        0        0     8042 2024-05-28 21:32:49.991124 pysofa2-23.10.11.2/src/prec76.c
+-rw-r--r--   0        0        0     4962 2024-05-28 21:32:49.991208 pysofa2-23.10.11.2/src/pv2p.c
+-rw-r--r--   0        0        0     6865 2024-05-28 21:32:49.991293 pysofa2-23.10.11.2/src/pv2s.c
+-rw-r--r--   0        0        0     5591 2024-05-28 21:32:49.991377 pysofa2-23.10.11.2/src/pvdpv.c
+-rw-r--r--   0        0        0     5077 2024-05-28 21:32:49.991462 pysofa2-23.10.11.2/src/pvm.c
+-rw-r--r--   0        0        0     5186 2024-05-28 21:32:49.991546 pysofa2-23.10.11.2/src/pvmpv.c
+-rw-r--r--   0        0        0     5181 2024-05-28 21:32:49.991624 pysofa2-23.10.11.2/src/pvppv.c
+-rw-r--r--   0        0        0    10033 2024-05-28 21:32:49.991720 pysofa2-23.10.11.2/src/pvstar.c
+-rw-r--r--   0        0        0     7733 2024-05-28 21:32:49.991814 pysofa2-23.10.11.2/src/pvtob.c
+-rw-r--r--   0        0        0     5377 2024-05-28 21:32:49.991912 pysofa2-23.10.11.2/src/pvu.c
+-rw-r--r--   0        0        0     5284 2024-05-28 21:32:49.992016 pysofa2-23.10.11.2/src/pvup.c
+-rw-r--r--   0        0        0     5846 2024-05-28 21:32:49.992111 pysofa2-23.10.11.2/src/pvxpv.c
+-rw-r--r--   0        0        0     5238 2024-05-28 21:32:49.992195 pysofa2-23.10.11.2/src/pxp.c
+-rw-r--r--   0        0        0    11858 2024-05-28 21:32:49.992308 pysofa2-23.10.11.2/src/refco.c
+-rw-r--r--   0        0        0     5990 2024-05-28 21:32:49.992428 pysofa2-23.10.11.2/src/rm2v.c
+-rw-r--r--   0        0        0     6001 2024-05-28 21:32:49.992517 pysofa2-23.10.11.2/src/rv2m.c
+-rw-r--r--   0        0        0     5811 2024-05-28 21:32:49.992612 pysofa2-23.10.11.2/src/rx.c
+-rw-r--r--   0        0        0     5302 2024-05-28 21:32:49.992716 pysofa2-23.10.11.2/src/rxp.c
+-rw-r--r--   0        0        0     5419 2024-05-28 21:32:49.992809 pysofa2-23.10.11.2/src/rxpv.c
+-rw-r--r--   0        0        0     5341 2024-05-28 21:32:49.992920 pysofa2-23.10.11.2/src/rxr.c
+-rw-r--r--   0        0        0     5852 2024-05-28 21:32:49.993008 pysofa2-23.10.11.2/src/ry.c
+-rw-r--r--   0        0        0     5821 2024-05-28 21:32:49.993099 pysofa2-23.10.11.2/src/rz.c
+-rw-r--r--   0        0        0    15650 2024-05-28 21:32:49.993216 pysofa2-23.10.11.2/src/s00.c
+-rw-r--r--   0        0        0     7797 2024-05-28 21:32:49.993328 pysofa2-23.10.11.2/src/s00a.c
+-rw-r--r--   0        0        0     7788 2024-05-28 21:32:49.993423 pysofa2-23.10.11.2/src/s00b.c
+-rw-r--r--   0        0        0    15477 2024-05-28 21:32:49.993528 pysofa2-23.10.11.2/src/s06.c
+-rw-r--r--   0        0        0     7815 2024-05-28 21:32:49.993626 pysofa2-23.10.11.2/src/s06a.c
+-rw-r--r--   0        0        0     5077 2024-05-28 21:32:49.993744 pysofa2-23.10.11.2/src/s2c.c
+-rw-r--r--   0        0        0     5213 2024-05-28 21:32:49.993842 pysofa2-23.10.11.2/src/s2p.c
+-rw-r--r--   0        0        0     5640 2024-05-28 21:32:49.993937 pysofa2-23.10.11.2/src/s2pv.c
+-rw-r--r--   0        0        0     5286 2024-05-28 21:32:49.994033 pysofa2-23.10.11.2/src/s2xpv.c
+-rw-r--r--   0        0        0     5893 2024-05-28 21:32:49.994136 pysofa2-23.10.11.2/src/sepp.c
+-rw-r--r--   0        0        0     5440 2024-05-28 21:32:49.994254 pysofa2-23.10.11.2/src/seps.c
+-rw-r--r--   0        0        0    28715 2024-05-28 21:32:49.994330 pysofa2-23.10.11.2/src/sofa.h
+-rw-r--r--   0        0        0     7294 2024-05-28 21:32:49.994462 pysofa2-23.10.11.2/src/sofam.h
+-rw-r--r--   0        0        0     6592 2024-05-28 21:32:49.994558 pysofa2-23.10.11.2/src/sp00.c
+-rw-r--r--   0        0        0    10713 2024-05-28 21:32:49.994657 pysofa2-23.10.11.2/src/starpm.c
+-rw-r--r--   0        0        0    11954 2024-05-28 21:32:49.994746 pysofa2-23.10.11.2/src/starpv.c
+-rw-r--r--   0        0        0     5042 2024-05-28 21:32:49.994836 pysofa2-23.10.11.2/src/sxp.c
+-rw-r--r--   0        0        0     5105 2024-05-28 21:32:49.994925 pysofa2-23.10.11.2/src/sxpv.c
+-rw-r--r--   0        0        0   243734 2024-05-28 21:32:49.995305 pysofa2-23.10.11.2/src/t_sofa_c.c
+-rw-r--r--   0        0        0     5880 2024-05-28 21:32:49.995444 pysofa2-23.10.11.2/src/taitt.c
+-rw-r--r--   0        0        0     5936 2024-05-28 21:32:49.995556 pysofa2-23.10.11.2/src/taiut1.c
+-rw-r--r--   0        0        0     7509 2024-05-28 21:32:49.995666 pysofa2-23.10.11.2/src/taiutc.c
+-rw-r--r--   0        0        0     7022 2024-05-28 21:32:49.995809 pysofa2-23.10.11.2/src/tcbtdb.c
+-rw-r--r--   0        0        0     5879 2024-05-28 21:32:49.995911 pysofa2-23.10.11.2/src/tcgtt.c
+-rw-r--r--   0        0        0     7144 2024-05-28 21:32:49.996017 pysofa2-23.10.11.2/src/tdbtcb.c
+-rw-r--r--   0        0        0     6388 2024-05-28 21:32:49.996110 pysofa2-23.10.11.2/src/tdbtt.c
+-rw-r--r--   0        0        0     6097 2024-05-28 21:32:49.996188 pysofa2-23.10.11.2/src/tf2a.c
+-rw-r--r--   0        0        0     6101 2024-05-28 21:32:49.996276 pysofa2-23.10.11.2/src/tf2d.c
+-rw-r--r--   0        0        0     8685 2024-05-28 21:32:49.996386 pysofa2-23.10.11.2/src/tpors.c
+-rw-r--r--   0        0        0     8649 2024-05-28 21:32:49.996502 pysofa2-23.10.11.2/src/tporv.c
+-rw-r--r--   0        0        0     6534 2024-05-28 21:32:49.996586 pysofa2-23.10.11.2/src/tpsts.c
+-rw-r--r--   0        0        0     7337 2024-05-28 21:32:49.996679 pysofa2-23.10.11.2/src/tpstv.c
+-rw-r--r--   0        0        0     7253 2024-05-28 21:32:49.996779 pysofa2-23.10.11.2/src/tpxes.c
+-rw-r--r--   0        0        0     7927 2024-05-28 21:32:49.996878 pysofa2-23.10.11.2/src/tpxev.c
+-rw-r--r--   0        0        0     5140 2024-05-28 21:32:49.996967 pysofa2-23.10.11.2/src/tr.c
+-rw-r--r--   0        0        0     5268 2024-05-28 21:32:49.997048 pysofa2-23.10.11.2/src/trxp.c
+-rw-r--r--   0        0        0     5584 2024-05-28 21:32:49.997137 pysofa2-23.10.11.2/src/trxpv.c
+-rw-r--r--   0        0        0     5876 2024-05-28 21:32:49.997223 pysofa2-23.10.11.2/src/tttai.c
+-rw-r--r--   0        0        0     5948 2024-05-28 21:32:49.997316 pysofa2-23.10.11.2/src/tttcg.c
+-rw-r--r--   0        0        0     6380 2024-05-28 21:32:49.997404 pysofa2-23.10.11.2/src/tttdb.c
+-rw-r--r--   0        0        0     5829 2024-05-28 21:32:49.997498 pysofa2-23.10.11.2/src/ttut1.c
+-rw-r--r--   0        0        0     5933 2024-05-28 21:32:49.997599 pysofa2-23.10.11.2/src/ut1tai.c
+-rw-r--r--   0        0        0     5833 2024-05-28 21:32:49.997683 pysofa2-23.10.11.2/src/ut1tt.c
+-rw-r--r--   0        0        0     8814 2024-05-28 21:32:49.997781 pysofa2-23.10.11.2/src/ut1utc.c
+-rw-r--r--   0        0        0     8318 2024-05-28 21:32:49.997859 pysofa2-23.10.11.2/src/utctai.c
+-rw-r--r--   0        0        0     7472 2024-05-28 21:32:49.997946 pysofa2-23.10.11.2/src/utcut1.c
+-rw-r--r--   0        0        0   133697 2024-05-28 21:32:49.998050 pysofa2-23.10.11.2/src/xy06.c
+-rw-r--r--   0        0        0     7028 2024-05-28 21:32:49.998148 pysofa2-23.10.11.2/src/xys00a.c
+-rw-r--r--   0        0        0     7014 2024-05-28 21:32:49.998236 pysofa2-23.10.11.2/src/xys00b.c
+-rw-r--r--   0        0        0     7060 2024-05-28 21:32:49.998321 pysofa2-23.10.11.2/src/xys06a.c
+-rw-r--r--   0        0        0     4829 2024-05-28 21:32:49.998396 pysofa2-23.10.11.2/src/zp.c
+-rw-r--r--   0        0        0     4883 2024-05-28 21:32:49.998475 pysofa2-23.10.11.2/src/zpv.c
+-rw-r--r--   0        0        0     4971 2024-05-28 21:32:49.998552 pysofa2-23.10.11.2/src/zr.c
+-rw-r--r--   0        0        0     2568 1970-01-01 00:00:00.000000 pysofa2-23.10.11.2/PKG-INFO
```

### Comparing `pysofa2-23.10.11.1/LICENSE` & `pysofa2-23.10.11.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/PKG-INFO` & `pysofa2-23.10.11.2/pysofa2/__about__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,14 @@
-Metadata-Version: 2.1
-Name: pysofa2
-Version: 23.10.11.1
-Summary: A wrapper of the International Astronomical Union's SOFA lbrary.
-Home-page: https://gitlab.com/deddy/pysofa2
-Author: Duncan Eddy
-Author-email: duncan.eddy@gmail.com
-Maintainer: Duncan Eddy
-Maintainer-email: duncan.eddy@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-*pysofa2* is a module for using International Astronomical
+__version__      = "23.10.11.1"
+__author__       = "Duncan Eddy"
+__author_email__ = "duncan.eddy@gmail.com"
+__description__  = "A wrapper of the International Astronomical Union\'s SOFA lbrary."
+__url__          = "https://gitlab.com/deddy/pysofa2"
+__long_description_content_type__ = 'text/markdown'
+__long_description__ = '''*pysofa2* is a module for using International Astronomical
  Union's (<http://www.iau.org/>) SOFA library (<http://www.iausofa.org/>) in 
 python. It is inspired by original [pysofa](https://pypi.org/project/pysofa/)
 implementation of Frederic Grollier. It extends the original pysofa module by
 distributing and building the SOFA C library with the package, eliminiting the
 need for the end-user to build the libraries separaetly from the package 
 installtion.
 
@@ -23,8 +17,8 @@
 all delegated to the underlying SOFA_C library.
 
 *pysofa2* not endorsed by the International Astronomical Union. 
 In addition to *pysofa2*'s MIT license, any use of this module should comply 
 with SOFA's license and [terms of use](http://www.iausofa.org/copyr.pdf). 
 Especially, but not exclusively, any published work or commercial products 
 which includes results achieved by using *pysofa* shall acknowledge that the 
-SOFA software was used in obtaining those results.
+SOFA software was used in obtaining those results.'''
```

### Comparing `pysofa2-23.10.11.1/README.md` & `pysofa2-23.10.11.2/README.md`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/pysofa2/sofa_wrapper.py` & `pysofa2-23.10.11.2/pysofa2/sofa_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 import warnings as _warnings
 import os as _os
 import numpy as _np
 import pathlib as _pathlib
 import glob as _glob
 
+
 # Import CTypes for interfacing
 import ctypes as _ct
 # from   ctypes.util import find_library as _find_library
 from   numpy.ctypeslib import ndpointer as _ndpointer
 
 
 # Attempt to find sofa library to load
-_sofalib_filename = _glob.glob(str(_pathlib.Path(__file__).parent) + '/_sofa_c*')
+_sofalib_filename = _glob.glob(str(_pathlib.Path(__file__).parent) + '/_sofa_c.*')
 
 if len(_sofalib_filename) == 0:
     raise ImportError('Unable to find the shared C library "pysofa2._sofa_c".')
 
 _sofa = _ct.CDLL(_sofalib_filename[0])
 
+
 # Require C Shape
 def _req_shape_c(a, dtype=None, shape=None, req=None):
     return _np.require(a, dtype=dtype, requirements=req).reshape(shape, order='C')
 
 
 ##########################
 # SOFA Function Wrappers #
```

### Comparing `pysofa2-23.10.11.1/src/a2af.c` & `pysofa2-23.10.11.2/src/a2af.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/a2tf.c` & `pysofa2-23.10.11.2/src/a2tf.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ab.c` & `pysofa2-23.10.11.2/src/ab.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ae2hd.c` & `pysofa2-23.10.11.2/src/ae2hd.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/af2a.c` & `pysofa2-23.10.11.2/src/af2a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/anp.c` & `pysofa2-23.10.11.2/src/anp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/anpm.c` & `pysofa2-23.10.11.2/src/anpm.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apcg.c` & `pysofa2-23.10.11.2/src/apcg.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apcg13.c` & `pysofa2-23.10.11.2/src/apcg13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apci.c` & `pysofa2-23.10.11.2/src/apci.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apci13.c` & `pysofa2-23.10.11.2/src/apci13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apco.c` & `pysofa2-23.10.11.2/src/apco.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apco13.c` & `pysofa2-23.10.11.2/src/apco13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apcs.c` & `pysofa2-23.10.11.2/src/apcs.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apcs13.c` & `pysofa2-23.10.11.2/src/apcs13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/aper.c` & `pysofa2-23.10.11.2/src/aper.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/aper13.c` & `pysofa2-23.10.11.2/src/aper13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apio.c` & `pysofa2-23.10.11.2/src/apio.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/apio13.c` & `pysofa2-23.10.11.2/src/apio13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atcc13.c` & `pysofa2-23.10.11.2/src/atcc13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atccq.c` & `pysofa2-23.10.11.2/src/atccq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atci13.c` & `pysofa2-23.10.11.2/src/atci13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atciq.c` & `pysofa2-23.10.11.2/src/atciq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atciqn.c` & `pysofa2-23.10.11.2/src/atciqn.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atciqz.c` & `pysofa2-23.10.11.2/src/atciqz.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atco13.c` & `pysofa2-23.10.11.2/src/atco13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atic13.c` & `pysofa2-23.10.11.2/src/atic13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/aticq.c` & `pysofa2-23.10.11.2/src/aticq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/aticqn.c` & `pysofa2-23.10.11.2/src/aticqn.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atio13.c` & `pysofa2-23.10.11.2/src/atio13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atioq.c` & `pysofa2-23.10.11.2/src/atioq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atoc13.c` & `pysofa2-23.10.11.2/src/atoc13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atoi13.c` & `pysofa2-23.10.11.2/src/atoi13.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/atoiq.c` & `pysofa2-23.10.11.2/src/atoiq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/bi00.c` & `pysofa2-23.10.11.2/src/bi00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/bp00.c` & `pysofa2-23.10.11.2/src/bp00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/bp06.c` & `pysofa2-23.10.11.2/src/bp06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/bpn2xy.c` & `pysofa2-23.10.11.2/src/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2i00a.c` & `pysofa2-23.10.11.2/src/c2i00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2i00b.c` & `pysofa2-23.10.11.2/src/c2i00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2i06a.c` & `pysofa2-23.10.11.2/src/c2i06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2ibpn.c` & `pysofa2-23.10.11.2/src/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2ixy.c` & `pysofa2-23.10.11.2/src/c2ixy.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2ixys.c` & `pysofa2-23.10.11.2/src/c2ixys.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2s.c` & `pysofa2-23.10.11.2/src/c2s.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2t00a.c` & `pysofa2-23.10.11.2/src/c2t00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2t00b.c` & `pysofa2-23.10.11.2/src/c2t00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2t06a.c` & `pysofa2-23.10.11.2/src/c2t06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2tcio.c` & `pysofa2-23.10.11.2/src/c2tcio.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2teqx.c` & `pysofa2-23.10.11.2/src/c2teqx.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2tpe.c` & `pysofa2-23.10.11.2/src/c2tpe.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/c2txy.c` & `pysofa2-23.10.11.2/src/c2txy.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/cal2jd.c` & `pysofa2-23.10.11.2/src/cal2jd.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/cp.c` & `pysofa2-23.10.11.2/src/cp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/cpv.c` & `pysofa2-23.10.11.2/src/cpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/cr.c` & `pysofa2-23.10.11.2/src/cr.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/d2dtf.c` & `pysofa2-23.10.11.2/src/d2dtf.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/d2tf.c` & `pysofa2-23.10.11.2/src/d2tf.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/dat.c` & `pysofa2-23.10.11.2/src/dat.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/dtdb.c` & `pysofa2-23.10.11.2/src/dtdb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/dtf2d.c` & `pysofa2-23.10.11.2/src/dtf2d.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eceq06.c` & `pysofa2-23.10.11.2/src/eceq06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ecm06.c` & `pysofa2-23.10.11.2/src/ecm06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ee00.c` & `pysofa2-23.10.11.2/src/ee00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ee00a.c` & `pysofa2-23.10.11.2/src/ee00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ee00b.c` & `pysofa2-23.10.11.2/src/ee00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ee06a.c` & `pysofa2-23.10.11.2/src/ee06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eect00.c` & `pysofa2-23.10.11.2/src/eect00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eform.c` & `pysofa2-23.10.11.2/src/eform.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eo06a.c` & `pysofa2-23.10.11.2/src/eo06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eors.c` & `pysofa2-23.10.11.2/src/eors.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/epb.c` & `pysofa2-23.10.11.2/src/epb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/epb2jd.c` & `pysofa2-23.10.11.2/src/epb2jd.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/epj.c` & `pysofa2-23.10.11.2/src/epj.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/epj2jd.c` & `pysofa2-23.10.11.2/src/epj2jd.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/epv00.c` & `pysofa2-23.10.11.2/src/epv00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eqec06.c` & `pysofa2-23.10.11.2/src/eqec06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/eqeq94.c` & `pysofa2-23.10.11.2/src/eqeq94.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/era00.c` & `pysofa2-23.10.11.2/src/era00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fad03.c` & `pysofa2-23.10.11.2/src/fad03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fae03.c` & `pysofa2-23.10.11.2/src/fae03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/faf03.c` & `pysofa2-23.10.11.2/src/faf03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/faju03.c` & `pysofa2-23.10.11.2/src/faju03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fal03.c` & `pysofa2-23.10.11.2/src/fal03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/falp03.c` & `pysofa2-23.10.11.2/src/falp03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fama03.c` & `pysofa2-23.10.11.2/src/fama03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fame03.c` & `pysofa2-23.10.11.2/src/fame03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fane03.c` & `pysofa2-23.10.11.2/src/fane03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/faom03.c` & `pysofa2-23.10.11.2/src/faom03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fapa03.c` & `pysofa2-23.10.11.2/src/fapa03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fasa03.c` & `pysofa2-23.10.11.2/src/fasa03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/faur03.c` & `pysofa2-23.10.11.2/src/faur03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fave03.c` & `pysofa2-23.10.11.2/src/fave03.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk425.c` & `pysofa2-23.10.11.2/src/fk425.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk45z.c` & `pysofa2-23.10.11.2/src/fk45z.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk524.c` & `pysofa2-23.10.11.2/src/fk524.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk52h.c` & `pysofa2-23.10.11.2/src/fk52h.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk54z.c` & `pysofa2-23.10.11.2/src/fk54z.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk5hip.c` & `pysofa2-23.10.11.2/src/fk5hip.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fk5hz.c` & `pysofa2-23.10.11.2/src/fk5hz.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fw2m.c` & `pysofa2-23.10.11.2/src/fw2m.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/fw2xy.c` & `pysofa2-23.10.11.2/src/fw2xy.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/g2icrs.c` & `pysofa2-23.10.11.2/src/g2icrs.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gc2gd.c` & `pysofa2-23.10.11.2/src/gc2gd.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gc2gde.c` & `pysofa2-23.10.11.2/src/gc2gde.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gd2gc.c` & `pysofa2-23.10.11.2/src/gd2gc.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gd2gce.c` & `pysofa2-23.10.11.2/src/gd2gce.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gmst00.c` & `pysofa2-23.10.11.2/src/gmst00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gmst06.c` & `pysofa2-23.10.11.2/src/gmst06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gmst82.c` & `pysofa2-23.10.11.2/src/gmst82.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gst00a.c` & `pysofa2-23.10.11.2/src/gst00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gst00b.c` & `pysofa2-23.10.11.2/src/gst00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gst06.c` & `pysofa2-23.10.11.2/src/gst06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gst06a.c` & `pysofa2-23.10.11.2/src/gst06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/gst94.c` & `pysofa2-23.10.11.2/src/gst94.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/h2fk5.c` & `pysofa2-23.10.11.2/src/h2fk5.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/hd2ae.c` & `pysofa2-23.10.11.2/src/hd2ae.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/hd2pa.c` & `pysofa2-23.10.11.2/src/hd2pa.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/hfk5z.c` & `pysofa2-23.10.11.2/src/hfk5z.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/icrs2g.c` & `pysofa2-23.10.11.2/src/icrs2g.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ir.c` & `pysofa2-23.10.11.2/src/ir.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/jd2cal.c` & `pysofa2-23.10.11.2/src/jd2cal.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/jdcalf.c` & `pysofa2-23.10.11.2/src/jdcalf.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ld.c` & `pysofa2-23.10.11.2/src/ld.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ldn.c` & `pysofa2-23.10.11.2/src/ldn.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ldsun.c` & `pysofa2-23.10.11.2/src/ldsun.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/lteceq.c` & `pysofa2-23.10.11.2/src/lteceq.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ltecm.c` & `pysofa2-23.10.11.2/src/ltecm.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/lteqec.c` & `pysofa2-23.10.11.2/src/lteqec.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ltp.c` & `pysofa2-23.10.11.2/src/ltp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ltpb.c` & `pysofa2-23.10.11.2/src/ltpb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ltpecl.c` & `pysofa2-23.10.11.2/src/ltpecl.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ltpequ.c` & `pysofa2-23.10.11.2/src/ltpequ.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/makefile` & `pysofa2-23.10.11.2/src/makefile`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/moon98.c` & `pysofa2-23.10.11.2/src/moon98.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/num00a.c` & `pysofa2-23.10.11.2/src/num00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/num00b.c` & `pysofa2-23.10.11.2/src/num00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/num06a.c` & `pysofa2-23.10.11.2/src/num06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/numat.c` & `pysofa2-23.10.11.2/src/numat.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/nut00a.c` & `pysofa2-23.10.11.2/src/nut00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/nut00b.c` & `pysofa2-23.10.11.2/src/nut00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/nut06a.c` & `pysofa2-23.10.11.2/src/nut06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/nut80.c` & `pysofa2-23.10.11.2/src/nut80.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/nutm80.c` & `pysofa2-23.10.11.2/src/nutm80.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/obl06.c` & `pysofa2-23.10.11.2/src/obl06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/obl80.c` & `pysofa2-23.10.11.2/src/obl80.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/p06e.c` & `pysofa2-23.10.11.2/src/p06e.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/p2pv.c` & `pysofa2-23.10.11.2/src/p2pv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/p2s.c` & `pysofa2-23.10.11.2/src/p2s.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pap.c` & `pysofa2-23.10.11.2/src/pap.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pas.c` & `pysofa2-23.10.11.2/src/pas.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pb06.c` & `pysofa2-23.10.11.2/src/pb06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pdp.c` & `pysofa2-23.10.11.2/src/pdp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pfw06.c` & `pysofa2-23.10.11.2/src/pfw06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/plan94.c` & `pysofa2-23.10.11.2/src/plan94.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pm.c` & `pysofa2-23.10.11.2/src/pm.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmat00.c` & `pysofa2-23.10.11.2/src/pmat00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmat06.c` & `pysofa2-23.10.11.2/src/pmat06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmat76.c` & `pysofa2-23.10.11.2/src/pmat76.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmp.c` & `pysofa2-23.10.11.2/src/pmp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmpx.c` & `pysofa2-23.10.11.2/src/pmpx.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pmsafe.c` & `pysofa2-23.10.11.2/src/pmsafe.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn.c` & `pysofa2-23.10.11.2/src/pn.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn00.c` & `pysofa2-23.10.11.2/src/pn00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn00a.c` & `pysofa2-23.10.11.2/src/pn00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn00b.c` & `pysofa2-23.10.11.2/src/pn00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn06.c` & `pysofa2-23.10.11.2/src/pn06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pn06a.c` & `pysofa2-23.10.11.2/src/pn06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pnm00a.c` & `pysofa2-23.10.11.2/src/pnm00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pnm00b.c` & `pysofa2-23.10.11.2/src/pnm00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pnm06a.c` & `pysofa2-23.10.11.2/src/pnm06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pnm80.c` & `pysofa2-23.10.11.2/src/pnm80.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pom00.c` & `pysofa2-23.10.11.2/src/pom00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ppp.c` & `pysofa2-23.10.11.2/src/ppp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ppsp.c` & `pysofa2-23.10.11.2/src/ppsp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pr00.c` & `pysofa2-23.10.11.2/src/pr00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/prec76.c` & `pysofa2-23.10.11.2/src/prec76.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pv2p.c` & `pysofa2-23.10.11.2/src/pv2p.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pv2s.c` & `pysofa2-23.10.11.2/src/pv2s.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvdpv.c` & `pysofa2-23.10.11.2/src/pvdpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvm.c` & `pysofa2-23.10.11.2/src/pvm.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvmpv.c` & `pysofa2-23.10.11.2/src/pvmpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvppv.c` & `pysofa2-23.10.11.2/src/pvppv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvstar.c` & `pysofa2-23.10.11.2/src/pvstar.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvtob.c` & `pysofa2-23.10.11.2/src/pvtob.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvu.c` & `pysofa2-23.10.11.2/src/pvu.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvup.c` & `pysofa2-23.10.11.2/src/pvup.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pvxpv.c` & `pysofa2-23.10.11.2/src/pvxpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/pxp.c` & `pysofa2-23.10.11.2/src/pxp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/refco.c` & `pysofa2-23.10.11.2/src/refco.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rm2v.c` & `pysofa2-23.10.11.2/src/rm2v.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rv2m.c` & `pysofa2-23.10.11.2/src/rv2m.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rx.c` & `pysofa2-23.10.11.2/src/rx.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rxp.c` & `pysofa2-23.10.11.2/src/rxp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rxpv.c` & `pysofa2-23.10.11.2/src/rxpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rxr.c` & `pysofa2-23.10.11.2/src/rxr.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ry.c` & `pysofa2-23.10.11.2/src/ry.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/rz.c` & `pysofa2-23.10.11.2/src/rz.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s00.c` & `pysofa2-23.10.11.2/src/s00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s00a.c` & `pysofa2-23.10.11.2/src/s00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s00b.c` & `pysofa2-23.10.11.2/src/s00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s06.c` & `pysofa2-23.10.11.2/src/s06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s06a.c` & `pysofa2-23.10.11.2/src/s06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s2c.c` & `pysofa2-23.10.11.2/src/s2c.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s2p.c` & `pysofa2-23.10.11.2/src/s2p.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s2pv.c` & `pysofa2-23.10.11.2/src/s2pv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/s2xpv.c` & `pysofa2-23.10.11.2/src/s2xpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sepp.c` & `pysofa2-23.10.11.2/src/sepp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/seps.c` & `pysofa2-23.10.11.2/src/seps.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sofa.h` & `pysofa2-23.10.11.2/src/sofa.h`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sofam.h` & `pysofa2-23.10.11.2/src/sofam.h`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sp00.c` & `pysofa2-23.10.11.2/src/sp00.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/starpm.c` & `pysofa2-23.10.11.2/src/starpm.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/starpv.c` & `pysofa2-23.10.11.2/src/starpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sxp.c` & `pysofa2-23.10.11.2/src/sxp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/sxpv.c` & `pysofa2-23.10.11.2/src/sxpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/t_sofa_c.c` & `pysofa2-23.10.11.2/src/t_sofa_c.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/taitt.c` & `pysofa2-23.10.11.2/src/taitt.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/taiut1.c` & `pysofa2-23.10.11.2/src/taiut1.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/taiutc.c` & `pysofa2-23.10.11.2/src/taiutc.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tcbtdb.c` & `pysofa2-23.10.11.2/src/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tcgtt.c` & `pysofa2-23.10.11.2/src/tcgtt.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tdbtcb.c` & `pysofa2-23.10.11.2/src/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tdbtt.c` & `pysofa2-23.10.11.2/src/tdbtt.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tf2a.c` & `pysofa2-23.10.11.2/src/tf2a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tf2d.c` & `pysofa2-23.10.11.2/src/tf2d.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tpors.c` & `pysofa2-23.10.11.2/src/tpors.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tporv.c` & `pysofa2-23.10.11.2/src/tporv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tpsts.c` & `pysofa2-23.10.11.2/src/tpsts.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tpstv.c` & `pysofa2-23.10.11.2/src/tpstv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tpxes.c` & `pysofa2-23.10.11.2/src/tpxes.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tpxev.c` & `pysofa2-23.10.11.2/src/tpxev.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tr.c` & `pysofa2-23.10.11.2/src/tr.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/trxp.c` & `pysofa2-23.10.11.2/src/trxp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/trxpv.c` & `pysofa2-23.10.11.2/src/trxpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tttai.c` & `pysofa2-23.10.11.2/src/tttai.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tttcg.c` & `pysofa2-23.10.11.2/src/tttcg.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/tttdb.c` & `pysofa2-23.10.11.2/src/tttdb.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ttut1.c` & `pysofa2-23.10.11.2/src/ttut1.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ut1tai.c` & `pysofa2-23.10.11.2/src/ut1tai.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ut1tt.c` & `pysofa2-23.10.11.2/src/ut1tt.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/ut1utc.c` & `pysofa2-23.10.11.2/src/ut1utc.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/utctai.c` & `pysofa2-23.10.11.2/src/utctai.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/utcut1.c` & `pysofa2-23.10.11.2/src/utcut1.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/xy06.c` & `pysofa2-23.10.11.2/src/xy06.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/xys00a.c` & `pysofa2-23.10.11.2/src/xys00a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/xys00b.c` & `pysofa2-23.10.11.2/src/xys00b.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/xys06a.c` & `pysofa2-23.10.11.2/src/xys06a.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/zp.c` & `pysofa2-23.10.11.2/src/zp.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/zpv.c` & `pysofa2-23.10.11.2/src/zpv.c`

 * *Files identical despite different names*

### Comparing `pysofa2-23.10.11.1/src/zr.c` & `pysofa2-23.10.11.2/src/zr.c`

 * *Files identical despite different names*

