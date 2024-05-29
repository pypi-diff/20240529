# Comparing `tmp/sdss-coordio-1.9.2.tar.gz` & `tmp/sdss-coordio-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss-coordio-1.9.2.tar", last modified: Tue Jan 16 05:41:36 2024, max compression
+gzip compressed data, was "sdss-coordio-1.9.3.tar", last modified: Sun Feb 18 22:32:36 2024, max compression
```

## Comparing `sdss-coordio-1.9.2.tar` & `sdss-coordio-1.9.3.tar`

### file list

```diff
@@ -1,330 +1,330 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.827607 sdss-coordio-1.9.2/
--rw-r--r--   0 runner     (501) staff       (20)     1504 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/LICENSE.md
--rw-r--r--   0 runner     (501) staff       (20)       62 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     2885 2024-01-16 05:41:36.827437 sdss-coordio-1.9.2/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      796 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.723676 sdss-coordio-1.9.2/cextern/
--rw-r--r--   0 runner     (501) staff       (20)      343 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/README.md
--rw-r--r--   0 runner     (501) staff       (20)    12507 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/conv.cpp
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.728784 sdss-coordio-1.9.2/cextern/dimage/
--rw-r--r--   0 runner     (501) staff       (20)     3150 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dallpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     1295 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dcen3x3.c
--rw-r--r--   0 runner     (501) staff       (20)     3239 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dfind.c
--rw-r--r--   0 runner     (501) staff       (20)     2553 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dfloodfill.c
--rw-r--r--   0 runner     (501) staff       (20)     1407 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dimage.h
--rw-r--r--   0 runner     (501) staff       (20)     6057 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dmedsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)     1351 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dobjects.c
--rw-r--r--   0 runner     (501) staff       (20)     3798 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dpeaks.c
--rw-r--r--   0 runner     (501) staff       (20)     2856 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/drefine.c
--rw-r--r--   0 runner     (501) staff       (20)     1872 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dselip.c
--rw-r--r--   0 runner     (501) staff       (20)     1252 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dsigma.c
--rw-r--r--   0 runner     (501) staff       (20)     3854 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/dsmooth.c
--rw-r--r--   0 runner     (501) staff       (20)       58 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/readme.txt
--rw-r--r--   0 runner     (501) staff       (20)     1984 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/dimage/simplexy.c
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.808676 sdss-coordio-1.9.2/cextern/sofa/
--rw-r--r--   0 runner     (501) staff       (20)     6468 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/a2af.c
--rw-r--r--   0 runner     (501) staff       (20)     6374 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/a2tf.c
--rw-r--r--   0 runner     (501) staff       (20)     6611 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ab.c
--rw-r--r--   0 runner     (501) staff       (20)     7187 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ae2hd.c
--rw-r--r--   0 runner     (501) staff       (20)     6087 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/af2a.c
--rw-r--r--   0 runner     (501) staff       (20)     4955 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/anp.c
--rw-r--r--   0 runner     (501) staff       (20)     4983 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/anpm.c
--rw-r--r--   0 runner     (501) staff       (20)     9173 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apcg.c
--rw-r--r--   0 runner     (501) staff       (20)     9278 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apcg13.c
--rw-r--r--   0 runner     (501) staff       (20)     9669 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apci.c
--rw-r--r--   0 runner     (501) staff       (20)     9954 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apci13.c
--rw-r--r--   0 runner     (501) staff       (20)    12864 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apco.c
--rw-r--r--   0 runner     (501) staff       (20)    14172 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apco13.c
--rw-r--r--   0 runner     (501) staff       (20)    11004 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apcs.c
--rw-r--r--   0 runner     (501) staff       (20)     9686 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apcs13.c
--rw-r--r--   0 runner     (501) staff       (20)     8285 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/aper.c
--rw-r--r--   0 runner     (501) staff       (20)     9207 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/aper13.c
--rw-r--r--   0 runner     (501) staff       (20)    10588 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apio.c
--rw-r--r--   0 runner     (501) staff       (20)    12842 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/apio13.c
--rw-r--r--   0 runner     (501) staff       (20)     8257 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atci13.c
--rw-r--r--   0 runner     (501) staff       (20)     7978 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atciq.c
--rw-r--r--   0 runner     (501) staff       (20)     9826 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atciqn.c
--rw-r--r--   0 runner     (501) staff       (20)     7729 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atciqz.c
--rw-r--r--   0 runner     (501) staff       (20)    12474 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atco13.c
--rw-r--r--   0 runner     (501) staff       (20)     7919 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atic13.c
--rw-r--r--   0 runner     (501) staff       (20)     8735 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/aticq.c
--rw-r--r--   0 runner     (501) staff       (20)    10634 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/aticqn.c
--rw-r--r--   0 runner     (501) staff       (20)    11485 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atio13.c
--rw-r--r--   0 runner     (501) staff       (20)    11389 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atioq.c
--rw-r--r--   0 runner     (501) staff       (20)    12003 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atoc13.c
--rw-r--r--   0 runner     (501) staff       (20)    11902 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atoi13.c
--rw-r--r--   0 runner     (501) staff       (20)    11115 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/atoiq.c
--rw-r--r--   0 runner     (501) staff       (20)     6640 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/bi00.c
--rw-r--r--   0 runner     (501) staff       (20)     8454 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/bp00.c
--rw-r--r--   0 runner     (501) staff       (20)     7280 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/bp06.c
--rw-r--r--   0 runner     (501) staff       (20)     5822 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/bpn2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     7375 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2i00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7362 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2i00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7165 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2i06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7592 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2ibpn.c
--rw-r--r--   0 runner     (501) staff       (20)     7162 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2ixy.c
--rw-r--r--   0 runner     (501) staff       (20)     6391 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2ixys.c
--rw-r--r--   0 runner     (501) staff       (20)     5320 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2s.c
--rw-r--r--   0 runner     (501) staff       (20)     8083 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2t00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7985 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2t00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7970 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2t06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6652 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2tcio.c
--rw-r--r--   0 runner     (501) staff       (20)     6679 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2teqx.c
--rw-r--r--   0 runner     (501) staff       (20)     8786 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2tpe.c
--rw-r--r--   0 runner     (501) staff       (20)     8249 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/c2txy.c
--rw-r--r--   0 runner     (501) staff       (20)     6962 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/cal2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     4897 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/cp.c
--rw-r--r--   0 runner     (501) staff       (20)     4990 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/cpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4974 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/cr.c
--rw-r--r--   0 runner     (501) staff       (20)     9794 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/d2dtf.c
--rw-r--r--   0 runner     (501) staff       (20)     7240 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/d2tf.c
--rw-r--r--   0 runner     (501) staff       (20)    13394 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/dat.c
--rw-r--r--   0 runner     (501) staff       (20)    63548 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/dtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     9375 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/dtf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     7237 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eceq06.c
--rw-r--r--   0 runner     (501) staff       (20)     7251 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ecm06.c
--rw-r--r--   0 runner     (501) staff       (20)     6929 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ee00.c
--rw-r--r--   0 runner     (501) staff       (20)     7105 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ee00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7436 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ee00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6632 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ee06a.c
--rw-r--r--   0 runner     (501) staff       (20)    12358 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eect00.c
--rw-r--r--   0 runner     (501) staff       (20)     6688 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eform.c
--rw-r--r--   0 runner     (501) staff       (20)     7000 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eo06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6082 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eors.c
--rw-r--r--   0 runner     (501) staff       (20)     5398 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/epb.c
--rw-r--r--   0 runner     (501) staff       (20)     5342 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/epb2jd.c
--rw-r--r--   0 runner     (501) staff       (20)     5327 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/epj.c
--rw-r--r--   0 runner     (501) staff       (20)     5330 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/epj2jd.c
--rw-r--r--   0 runner     (501) staff       (20)   152024 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/epv00.c
--rw-r--r--   0 runner     (501) staff       (20)     7238 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eqec06.c
--rw-r--r--   0 runner     (501) staff       (20)     6953 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/eqeq94.c
--rw-r--r--   0 runner     (501) staff       (20)     6978 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/era00.c
--rw-r--r--   0 runner     (501) staff       (20)     5789 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fad03.c
--rw-r--r--   0 runner     (501) staff       (20)     5756 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fae03.c
--rw-r--r--   0 runner     (501) staff       (20)     5883 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/faf03.c
--rw-r--r--   0 runner     (501) staff       (20)     5768 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/faju03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fal03.c
--rw-r--r--   0 runner     (501) staff       (20)     5758 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/falp03.c
--rw-r--r--   0 runner     (501) staff       (20)     5760 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fama03.c
--rw-r--r--   0 runner     (501) staff       (20)     5770 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fame03.c
--rw-r--r--   0 runner     (501) staff       (20)     5631 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fane03.c
--rw-r--r--   0 runner     (501) staff       (20)     5826 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/faom03.c
--rw-r--r--   0 runner     (501) staff       (20)     5754 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fapa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5765 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fasa03.c
--rw-r--r--   0 runner     (501) staff       (20)     5629 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/faur03.c
--rw-r--r--   0 runner     (501) staff       (20)     5764 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fave03.c
--rw-r--r--   0 runner     (501) staff       (20)    12333 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk425.c
--rw-r--r--   0 runner     (501) staff       (20)     9855 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk45z.c
--rw-r--r--   0 runner     (501) staff       (20)    12391 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk524.c
--rw-r--r--   0 runner     (501) staff       (20)     7422 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk52h.c
--rw-r--r--   0 runner     (501) staff       (20)     7286 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk54z.c
--rw-r--r--   0 runner     (501) staff       (20)     6198 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk5hip.c
--rw-r--r--   0 runner     (501) staff       (20)     8093 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fk5hz.c
--rw-r--r--   0 runner     (501) staff       (20)     7061 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fw2m.c
--rw-r--r--   0 runner     (501) staff       (20)     6147 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/fw2xy.c
--rw-r--r--   0 runner     (501) staff       (20)     8396 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/g2icrs.c
--rw-r--r--   0 runner     (501) staff       (20)     6710 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gc2gd.c
--rw-r--r--   0 runner     (501) staff       (20)     8338 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gc2gde.c
--rw-r--r--   0 runner     (501) staff       (20)     6783 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gd2gc.c
--rw-r--r--   0 runner     (501) staff       (20)     6968 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gd2gce.c
--rw-r--r--   0 runner     (501) staff       (20)     7699 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gmst00.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gmst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7688 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gmst82.c
--rw-r--r--   0 runner     (501) staff       (20)     7470 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gst00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7770 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gst00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7536 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gst06.c
--rw-r--r--   0 runner     (501) staff       (20)     7174 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gst06a.c
--rw-r--r--   0 runner     (501) staff       (20)     7099 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/gst94.c
--rw-r--r--   0 runner     (501) staff       (20)     7614 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/h2fk5.c
--rw-r--r--   0 runner     (501) staff       (20)     7382 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/hd2ae.c
--rw-r--r--   0 runner     (501) staff       (20)     6333 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/hd2pa.c
--rw-r--r--   0 runner     (501) staff       (20)     8684 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/hfk5z.c
--rw-r--r--   0 runner     (501) staff       (20)     8382 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/icrs2g.c
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ir.c
--rw-r--r--   0 runner     (501) staff       (20)     8269 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/jd2cal.c
--rw-r--r--   0 runner     (501) staff       (20)     7559 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/jdcalf.c
--rw-r--r--   0 runner     (501) staff       (20)     7662 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ld.c
--rw-r--r--   0 runner     (501) staff       (20)     8829 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ldn.c
--rw-r--r--   0 runner     (501) staff       (20)     5982 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ldsun.c
--rw-r--r--   0 runner     (501) staff       (20)     7014 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/lteceq.c
--rw-r--r--   0 runner     (501) staff       (20)     7567 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ltecm.c
--rw-r--r--   0 runner     (501) staff       (20)     7019 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/lteqec.c
--rw-r--r--   0 runner     (501) staff       (20)     6500 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ltp.c
--rw-r--r--   0 runner     (501) staff       (20)     6581 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ltpb.c
--rw-r--r--   0 runner     (501) staff       (20)     7601 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ltpecl.c
--rw-r--r--   0 runner     (501) staff       (20)     7880 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ltpequ.c
--rw-r--r--   0 runner     (501) staff       (20)    27755 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/makefile
--rw-r--r--   0 runner     (501) staff       (20)     6728 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/num00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6713 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/num00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6660 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/num06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6057 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/numat.c
--rw-r--r--   0 runner     (501) staff       (20)   119801 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/nut00a.c
--rw-r--r--   0 runner     (501) staff       (20)    19020 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/nut00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7823 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/nut06a.c
--rw-r--r--   0 runner     (501) staff       (20)    16295 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/nut80.c
--rw-r--r--   0 runner     (501) staff       (20)     6473 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/nutm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6414 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/obl06.c
--rw-r--r--   0 runner     (501) staff       (20)     6459 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/obl80.c
--rw-r--r--   0 runner     (501) staff       (20)    13793 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/p06e.c
--rw-r--r--   0 runner     (501) staff       (20)     5029 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/p2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5276 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/p2s.c
--rw-r--r--   0 runner     (501) staff       (20)     6768 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pap.c
--rw-r--r--   0 runner     (501) staff       (20)     5638 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pas.c
--rw-r--r--   0 runner     (501) staff       (20)     7817 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pb06.c
--rw-r--r--   0 runner     (501) staff       (20)     5008 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pdp.c
--rw-r--r--   0 runner     (501) staff       (20)     7964 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pfw06.c
--rw-r--r--   0 runner     (501) staff       (20)    23180 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/plan94.c
--rw-r--r--   0 runner     (501) staff       (20)     4887 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pm.c
--rw-r--r--   0 runner     (501) staff       (20)     6579 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmat00.c
--rw-r--r--   0 runner     (501) staff       (20)     6683 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmat06.c
--rw-r--r--   0 runner     (501) staff       (20)     7548 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmat76.c
--rw-r--r--   0 runner     (501) staff       (20)     5090 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmp.c
--rw-r--r--   0 runner     (501) staff       (20)     7054 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmpx.c
--rw-r--r--   0 runner     (501) staff       (20)    10220 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pmsafe.c
--rw-r--r--   0 runner     (501) staff       (20)     5495 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn.c
--rw-r--r--   0 runner     (501) staff       (20)     9146 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn00.c
--rw-r--r--   0 runner     (501) staff       (20)     8833 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn00a.c
--rw-r--r--   0 runner     (501) staff       (20)     8825 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn00b.c
--rw-r--r--   0 runner     (501) staff       (20)     9253 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn06.c
--rw-r--r--   0 runner     (501) staff       (20)     8282 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pn06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6802 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pnm00a.c
--rw-r--r--   0 runner     (501) staff       (20)     6797 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pnm00b.c
--rw-r--r--   0 runner     (501) staff       (20)     6835 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pnm06a.c
--rw-r--r--   0 runner     (501) staff       (20)     6778 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pnm80.c
--rw-r--r--   0 runner     (501) staff       (20)     6453 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pom00.c
--rw-r--r--   0 runner     (501) staff       (20)     5087 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ppp.c
--rw-r--r--   0 runner     (501) staff       (20)     5275 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ppsp.c
--rw-r--r--   0 runner     (501) staff       (20)     7813 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pr00.c
--rw-r--r--   0 runner     (501) staff       (20)     8023 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/prec76.c
--rw-r--r--   0 runner     (501) staff       (20)     4958 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pv2p.c
--rw-r--r--   0 runner     (501) staff       (20)     6861 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pv2s.c
--rw-r--r--   0 runner     (501) staff       (20)     5587 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvdpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvm.c
--rw-r--r--   0 runner     (501) staff       (20)     5182 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvmpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5177 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvppv.c
--rw-r--r--   0 runner     (501) staff       (20)    10128 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvstar.c
--rw-r--r--   0 runner     (501) staff       (20)     7712 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvtob.c
--rw-r--r--   0 runner     (501) staff       (20)     5373 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvu.c
--rw-r--r--   0 runner     (501) staff       (20)     5280 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvup.c
--rw-r--r--   0 runner     (501) staff       (20)     5842 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pvxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5234 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/pxp.c
--rw-r--r--   0 runner     (501) staff       (20)    11663 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/refco.c
--rw-r--r--   0 runner     (501) staff       (20)     5989 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rm2v.c
--rw-r--r--   0 runner     (501) staff       (20)     5996 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rv2m.c
--rw-r--r--   0 runner     (501) staff       (20)     5807 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rx.c
--rw-r--r--   0 runner     (501) staff       (20)     5298 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5144 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5337 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rxr.c
--rw-r--r--   0 runner     (501) staff       (20)     5848 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ry.c
--rw-r--r--   0 runner     (501) staff       (20)     5817 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/rz.c
--rw-r--r--   0 runner     (501) staff       (20)    15540 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s00.c
--rw-r--r--   0 runner     (501) staff       (20)     7781 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7772 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s00b.c
--rw-r--r--   0 runner     (501) staff       (20)    15442 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s06.c
--rw-r--r--   0 runner     (501) staff       (20)     7799 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s06a.c
--rw-r--r--   0 runner     (501) staff       (20)     5073 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s2c.c
--rw-r--r--   0 runner     (501) staff       (20)     5209 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s2p.c
--rw-r--r--   0 runner     (501) staff       (20)     5636 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s2pv.c
--rw-r--r--   0 runner     (501) staff       (20)     5282 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/s2xpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5877 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sepp.c
--rw-r--r--   0 runner     (501) staff       (20)     5424 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/seps.c
--rw-r--r--   0 runner     (501) staff       (20)    26863 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sofa.h
--rw-r--r--   0 runner     (501) staff       (20)     8772 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sofam.h
--rw-r--r--   0 runner     (501) staff       (20)     6557 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sp00.c
--rw-r--r--   0 runner     (501) staff       (20)    10677 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/starpm.c
--rw-r--r--   0 runner     (501) staff       (20)    11959 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/starpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5038 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5101 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/sxpv.c
--rw-r--r--   0 runner     (501) staff       (20)   241327 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/t_sofa_c.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/taitt.c
--rw-r--r--   0 runner     (501) staff       (20)     5901 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/taiut1.c
--rw-r--r--   0 runner     (501) staff       (20)     7493 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/taiutc.c
--rw-r--r--   0 runner     (501) staff       (20)     6987 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tcbtdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5845 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tcgtt.c
--rw-r--r--   0 runner     (501) staff       (20)     7109 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tdbtcb.c
--rw-r--r--   0 runner     (501) staff       (20)     6353 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tdbtt.c
--rw-r--r--   0 runner     (501) staff       (20)     6062 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tf2a.c
--rw-r--r--   0 runner     (501) staff       (20)     6066 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tf2d.c
--rw-r--r--   0 runner     (501) staff       (20)     8685 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tpors.c
--rw-r--r--   0 runner     (501) staff       (20)     8649 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tporv.c
--rw-r--r--   0 runner     (501) staff       (20)     6534 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tpsts.c
--rw-r--r--   0 runner     (501) staff       (20)     7337 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tpstv.c
--rw-r--r--   0 runner     (501) staff       (20)     7253 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tpxes.c
--rw-r--r--   0 runner     (501) staff       (20)     7927 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tpxev.c
--rw-r--r--   0 runner     (501) staff       (20)     5136 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tr.c
--rw-r--r--   0 runner     (501) staff       (20)     5263 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/trxp.c
--rw-r--r--   0 runner     (501) staff       (20)     5291 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/trxpv.c
--rw-r--r--   0 runner     (501) staff       (20)     5841 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tttai.c
--rw-r--r--   0 runner     (501) staff       (20)     5913 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tttcg.c
--rw-r--r--   0 runner     (501) staff       (20)     6345 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/tttdb.c
--rw-r--r--   0 runner     (501) staff       (20)     5794 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ttut1.c
--rw-r--r--   0 runner     (501) staff       (20)     5898 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ut1tai.c
--rw-r--r--   0 runner     (501) staff       (20)     5798 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ut1tt.c
--rw-r--r--   0 runner     (501) staff       (20)     8782 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/ut1utc.c
--rw-r--r--   0 runner     (501) staff       (20)     8283 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/utctai.c
--rw-r--r--   0 runner     (501) staff       (20)     7458 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/utcut1.c
--rw-r--r--   0 runner     (501) staff       (20)   133674 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/xy06.c
--rw-r--r--   0 runner     (501) staff       (20)     7028 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/xys00a.c
--rw-r--r--   0 runner     (501) staff       (20)     7010 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/xys00b.c
--rw-r--r--   0 runner     (501) staff       (20)     7056 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/xys06a.c
--rw-r--r--   0 runner     (501) staff       (20)     4820 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/zp.c
--rw-r--r--   0 runner     (501) staff       (20)     4874 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/zpv.c
--rw-r--r--   0 runner     (501) staff       (20)     4967 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/cextern/sofa/zr.c
--rw-r--r--   0 runner     (501) staff       (20)     2370 2024-01-16 05:41:36.828602 sdss-coordio-1.9.2/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2697 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.720839 sdss-coordio-1.9.2/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.816001 sdss-coordio-1.9.2/src/coordio/
--rw-r--r--   0 runner     (501) staff       (20)     1178 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12342 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/astrometry.py
--rw-r--r--   0 runner     (501) staff       (20)     5635 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/calibration.py
--rw-r--r--   0 runner     (501) staff       (20)    51063 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/conv.py
--rw-r--r--   0 runner     (501) staff       (20)     9926 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     7570 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/defaults.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.816563 sdss-coordio-1.9.2/src/coordio/etc/
--rw-r--r--   0 runner     (501) staff       (20)       73 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/etc/astrometrynet.cfg
--rw-r--r--   0 runner     (501) staff       (20)      366 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/etc/coordio.yml
--rw-r--r--   0 runner     (501) staff       (20)      722 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    12748 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/extraction.py
--rwxr-xr-x   0 runner     (501) staff       (20)    13362 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/fitData.py
--rw-r--r--   0 runner     (501) staff       (20)    30968 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/guide.py
--rw-r--r--   0 runner     (501) staff       (20)     5870 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/iers.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.816843 sdss-coordio-1.9.2/src/coordio/include/
--rw-r--r--   0 runner     (501) staff       (20)     1992 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/include/coordio.h
--rw-r--r--   0 runner     (501) staff       (20)     4013 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     4146 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/site.py
--rw-r--r--   0 runner     (501) staff       (20)    14255 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/sky.py
--rw-r--r--   0 runner     (501) staff       (20)     6440 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/sofa_bindings.py
--rw-r--r--   0 runner     (501) staff       (20)    10661 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/tangent.py
--rw-r--r--   0 runner     (501) staff       (20)    13390 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     6451 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/time.py
--rw-r--r--   0 runner     (501) staff       (20)    54616 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/transforms.py
--rw-r--r--   0 runner     (501) staff       (20)    38856 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/utils.py
--rw-r--r--   0 runner     (501) staff       (20)     3734 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/wok.py
--rw-r--r--   0 runner     (501) staff       (20)    14872 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/zernike.py
--rw-r--r--   0 runner     (501) staff       (20)    13102 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/src/coordio/zhaoburge.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.825029 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2885 2024-01-16 05:41:36.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6867 2024-01-16 05:41:36.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-16 05:41:36.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-16 05:40:59.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      465 2024-01-16 05:41:36.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        8 2024-01-16 05:41:36.000000 sdss-coordio-1.9.2/src/sdss_coordio.egg-info/top_level.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-16 05:41:36.824581 sdss-coordio-1.9.2/tests/
--rw-r--r--   0 runner     (501) staff       (20)    13006 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_conv.py
--rw-r--r--   0 runner     (501) staff       (20)     7006 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_coordinate.py
--rw-r--r--   0 runner     (501) staff       (20)     1386 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_fpScale.py
--rw-r--r--   0 runner     (501) staff       (20)     4290 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_guide.py
--rw-r--r--   0 runner     (501) staff       (20)     1418 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_iers.py
--rw-r--r--   0 runner     (501) staff       (20)    11447 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_libcoordio.py
--rw-r--r--   0 runner     (501) staff       (20)    10522 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_offset.py
--rw-r--r--   0 runner     (501) staff       (20)     8074 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_plPlug.py
--rw-r--r--   0 runner     (501) staff       (20)     5525 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_positioner.py
--rw-r--r--   0 runner     (501) staff       (20)     1105 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_site.py
--rw-r--r--   0 runner     (501) staff       (20)     5302 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_sky.py
--rw-r--r--   0 runner     (501) staff       (20)     1171 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_sofa.py
--rw-r--r--   0 runner     (501) staff       (20)     3340 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_tangent.py
--rw-r--r--   0 runner     (501) staff       (20)     2738 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_tangentToPositioner2.py
--rw-r--r--   0 runner     (501) staff       (20)    13872 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_telescope.py
--rw-r--r--   0 runner     (501) staff       (20)     1407 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_time.py
--rw-r--r--   0 runner     (501) staff       (20)     2588 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_wok.py
--rw-r--r--   0 runner     (501) staff       (20)     1363 2024-01-16 05:40:42.000000 sdss-coordio-1.9.2/tests/test_zern.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:36.021638 sdss-coordio-1.9.3/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1504 2021-07-27 18:49:37.000000 sdss-coordio-1.9.3/LICENSE.md
+-rw-r--r--   0 gallegoj   (501) staff       (20)       62 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/MANIFEST.in
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2940 2024-02-18 22:32:36.021338 sdss-coordio-1.9.3/PKG-INFO
+-rw-r--r--   0 gallegoj   (501) staff       (20)      796 2023-01-05 16:32:23.000000 sdss-coordio-1.9.3/README.md
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.579561 sdss-coordio-1.9.3/cextern/
+-rw-r--r--   0 gallegoj   (501) staff       (20)      343 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/README.md
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12507 2021-12-09 05:30:29.000000 sdss-coordio-1.9.3/cextern/conv.cpp
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.596288 sdss-coordio-1.9.3/cextern/dimage/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3150 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dallpeaks.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1295 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dcen3x3.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3239 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dfind.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2553 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dfloodfill.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1407 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dimage.h
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6057 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dmedsmooth.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1351 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dobjects.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3798 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dpeaks.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2856 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/drefine.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1872 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dselip.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1252 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dsigma.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3854 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/dsmooth.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)       58 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/readme.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1984 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/dimage/simplexy.c
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.971255 sdss-coordio-1.9.3/cextern/sofa/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6468 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/a2af.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6374 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/a2tf.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6611 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ab.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7187 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ae2hd.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6087 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/af2a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4955 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/anp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4983 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/anpm.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9173 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apcg.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9278 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apcg13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9669 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apci.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9954 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apci13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12864 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apco.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    14172 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apco13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11004 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apcs.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9686 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apcs13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8285 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/aper.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9207 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/aper13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10588 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apio.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12842 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/apio13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8257 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atci13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7978 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atciq.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9826 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atciqn.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7729 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atciqz.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12474 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atco13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7919 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atic13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8735 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/aticq.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10634 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/aticqn.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11485 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atio13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11389 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atioq.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12003 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atoc13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11902 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atoi13.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11115 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/atoiq.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6640 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/bi00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8454 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/bp00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7280 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/bp06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5822 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/bpn2xy.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7375 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2i00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7362 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2i00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7165 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2i06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7592 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2ibpn.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7162 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2ixy.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6391 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2ixys.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5320 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2s.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8083 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2t00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7985 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2t00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7970 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2t06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6652 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2tcio.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6679 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2teqx.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8786 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2tpe.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8249 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/c2txy.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6962 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/cal2jd.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4897 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/cp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4990 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/cpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4974 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/cr.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9794 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/d2dtf.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7240 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/d2tf.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13394 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/dat.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    63548 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/dtdb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9375 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/dtf2d.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7237 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eceq06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7251 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ecm06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6929 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ee00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7105 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ee00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7436 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ee00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6632 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ee06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12358 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eect00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6688 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eform.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7000 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eo06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6082 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eors.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5398 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/epb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5342 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/epb2jd.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5327 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/epj.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5330 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/epj2jd.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)   152024 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/epv00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7238 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eqec06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6953 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/eqeq94.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6978 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/era00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5789 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fad03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5756 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fae03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5883 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/faf03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5768 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/faju03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5758 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fal03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5758 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/falp03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5760 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fama03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5770 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fame03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5631 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fane03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5826 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/faom03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5754 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fapa03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5765 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fasa03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5629 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/faur03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5764 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fave03.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12333 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk425.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9855 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk45z.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12391 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk524.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7422 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk52h.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7286 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk54z.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6198 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk5hip.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8093 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fk5hz.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7061 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fw2m.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6147 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/fw2xy.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8396 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/g2icrs.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6710 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gc2gd.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8338 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gc2gde.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6783 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gd2gc.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6968 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gd2gce.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7699 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gmst00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7337 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gmst06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7688 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gmst82.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7470 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gst00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7770 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gst00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7536 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gst06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7174 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gst06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7099 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/gst94.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7614 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/h2fk5.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7382 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/hd2ae.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6333 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/hd2pa.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8684 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/hfk5z.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8382 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/icrs2g.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4970 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ir.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8269 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/jd2cal.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7559 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/jdcalf.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7662 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ld.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8829 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ldn.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5982 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ldsun.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7014 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/lteceq.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7567 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ltecm.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7019 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/lteqec.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6500 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ltp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6581 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ltpb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7601 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ltpecl.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7880 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ltpequ.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    27755 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/makefile
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6728 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/num00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6713 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/num00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6660 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/num06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6057 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/numat.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)   119801 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/nut00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    19020 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/nut00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7823 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/nut06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    16295 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/nut80.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6473 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/nutm80.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6414 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/obl06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6459 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/obl80.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13793 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/p06e.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5029 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/p2pv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5276 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/p2s.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6768 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pap.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5638 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pas.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7817 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pb06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5008 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pdp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7964 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pfw06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    23180 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/plan94.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4887 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pm.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6579 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmat00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6683 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmat06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7548 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmat76.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5090 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7054 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmpx.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10220 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pmsafe.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5495 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9146 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8833 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8825 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9253 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8282 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pn06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6802 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pnm00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6797 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pnm00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6835 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pnm06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6778 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pnm80.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6453 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pom00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5087 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ppp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5275 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ppsp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7813 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pr00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8023 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/prec76.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4958 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pv2p.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6861 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pv2s.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5587 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvdpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5073 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvm.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5182 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvmpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5177 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvppv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10128 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvstar.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7712 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvtob.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5373 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvu.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5280 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvup.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5842 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pvxpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5234 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/pxp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11663 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/refco.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5989 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rm2v.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5996 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rv2m.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5807 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rx.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5298 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rxp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5144 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rxpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5337 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rxr.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5848 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ry.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5817 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/rz.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    15540 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7781 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7772 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    15442 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7799 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5073 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s2c.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5209 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s2p.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5636 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s2pv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5282 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/s2xpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5877 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sepp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5424 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/seps.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    26863 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sofa.h
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8772 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sofam.h
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6557 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sp00.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10677 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/starpm.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11959 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/starpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5038 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sxp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5101 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/sxpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)   241327 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/cextern/sofa/t_sofa_c.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5845 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/taitt.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5901 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/taiut1.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7493 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/taiutc.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6987 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tcbtdb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5845 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tcgtt.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7109 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tdbtcb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6353 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tdbtt.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6062 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tf2a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6066 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tf2d.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8685 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tpors.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8649 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tporv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6534 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tpsts.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7337 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tpstv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7253 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tpxes.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7927 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tpxev.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5136 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tr.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5263 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/trxp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5291 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/trxpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5841 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tttai.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5913 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tttcg.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6345 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/tttdb.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5794 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ttut1.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5898 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ut1tai.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5798 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ut1tt.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8782 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/ut1utc.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8283 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/utctai.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7458 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/utcut1.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)   133674 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/xy06.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7028 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/xys00a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7010 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/xys00b.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7056 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/xys06a.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4820 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/zp.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4874 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/zpv.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4967 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/cextern/sofa/zr.c
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2409 2024-02-18 22:32:36.022905 sdss-coordio-1.9.3/setup.cfg
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2697 2022-08-15 20:15:07.000000 sdss-coordio-1.9.3/setup.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.573748 sdss-coordio-1.9.3/src/
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.990271 sdss-coordio-1.9.3/src/coordio/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1178 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/src/coordio/__init__.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12342 2022-09-12 00:37:15.000000 sdss-coordio-1.9.3/src/coordio/astrometry.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5635 2021-12-06 03:38:17.000000 sdss-coordio-1.9.3/src/coordio/calibration.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    51063 2023-12-08 00:45:32.000000 sdss-coordio-1.9.3/src/coordio/conv.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     9926 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/coordinate.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7570 2022-09-08 17:28:46.000000 sdss-coordio-1.9.3/src/coordio/defaults.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.992143 sdss-coordio-1.9.3/src/coordio/etc/
+-rw-r--r--   0 gallegoj   (501) staff       (20)       73 2022-08-31 19:49:44.000000 sdss-coordio-1.9.3/src/coordio/etc/astrometrynet.cfg
+-rw-r--r--   0 gallegoj   (501) staff       (20)      366 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/etc/coordio.yml
+-rw-r--r--   0 gallegoj   (501) staff       (20)      722 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/exceptions.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    12748 2023-01-15 17:17:06.000000 sdss-coordio-1.9.3/src/coordio/extraction.py
+-rwxr-xr-x   0 gallegoj   (501) staff       (20)    13362 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/fitData.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    30968 2023-12-08 00:45:43.000000 sdss-coordio-1.9.3/src/coordio/guide.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5870 2024-01-10 22:25:27.000000 sdss-coordio-1.9.3/src/coordio/iers.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:35.993412 sdss-coordio-1.9.3/src/coordio/include/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1992 2021-12-09 05:30:29.000000 sdss-coordio-1.9.3/src/coordio/include/coordio.h
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4013 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/src/coordio/positioner.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4146 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/site.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    16443 2024-01-27 21:17:54.000000 sdss-coordio-1.9.3/src/coordio/sky.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6700 2024-01-27 21:17:54.000000 sdss-coordio-1.9.3/src/coordio/sofa_bindings.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10661 2021-12-07 23:46:12.000000 sdss-coordio-1.9.3/src/coordio/tangent.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13390 2023-04-15 20:54:50.000000 sdss-coordio-1.9.3/src/coordio/telescope.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6451 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/time.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    54616 2024-01-16 05:38:48.000000 sdss-coordio-1.9.3/src/coordio/transforms.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    38856 2024-01-10 21:05:03.000000 sdss-coordio-1.9.3/src/coordio/utils.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3734 2022-01-14 22:57:26.000000 sdss-coordio-1.9.3/src/coordio/wok.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    14872 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/src/coordio/zernike.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13102 2023-08-07 22:52:10.000000 sdss-coordio-1.9.3/src/coordio/zhaoburge.py
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:36.015345 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2940 2024-02-18 22:32:35.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/PKG-INFO
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6867 2024-02-18 22:32:35.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/SOURCES.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-02-18 22:32:35.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/dependency_links.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)        1 2024-01-10 21:42:15.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/not-zip-safe
+-rw-r--r--   0 gallegoj   (501) staff       (20)      481 2024-02-18 22:32:35.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/requires.txt
+-rw-r--r--   0 gallegoj   (501) staff       (20)        8 2024-02-18 22:32:35.000000 sdss-coordio-1.9.3/src/sdss_coordio.egg-info/top_level.txt
+drwxr-xr-x   0 gallegoj   (501) staff       (20)        0 2024-02-18 22:32:36.014230 sdss-coordio-1.9.3/tests/
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13006 2022-01-14 22:57:26.000000 sdss-coordio-1.9.3/tests/test_conv.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     7006 2021-11-13 22:19:46.000000 sdss-coordio-1.9.3/tests/test_coordinate.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1386 2022-01-14 22:57:26.000000 sdss-coordio-1.9.3/tests/test_fpScale.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     4290 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/tests/test_guide.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1418 2024-01-10 22:14:05.000000 sdss-coordio-1.9.3/tests/test_iers.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    11447 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/tests/test_libcoordio.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    10522 2023-09-26 21:23:48.000000 sdss-coordio-1.9.3/tests/test_offset.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     8074 2022-09-08 17:28:46.000000 sdss-coordio-1.9.3/tests/test_plPlug.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     5525 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/tests/test_positioner.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1105 2022-09-08 17:28:46.000000 sdss-coordio-1.9.3/tests/test_site.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     6867 2024-01-27 21:17:54.000000 sdss-coordio-1.9.3/tests/test_sky.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1171 2021-01-26 01:53:15.000000 sdss-coordio-1.9.3/tests/test_sofa.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     3340 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/tests/test_tangent.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2738 2022-01-04 17:25:16.000000 sdss-coordio-1.9.3/tests/test_tangentToPositioner2.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)    13872 2023-04-15 20:54:50.000000 sdss-coordio-1.9.3/tests/test_telescope.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1407 2024-01-10 22:14:00.000000 sdss-coordio-1.9.3/tests/test_time.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     2588 2021-11-14 04:33:40.000000 sdss-coordio-1.9.3/tests/test_wok.py
+-rw-r--r--   0 gallegoj   (501) staff       (20)     1363 2022-01-04 17:48:06.000000 sdss-coordio-1.9.3/tests/test_zern.py
```

### Comparing `sdss-coordio-1.9.2/LICENSE.md` & `sdss-coordio-1.9.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/PKG-INFO` & `sdss-coordio-1.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.9.2
+Version: 1.9.3
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
@@ -30,14 +30,15 @@
 Requires-Dist: scipy>=1.2.1
 Requires-Dist: pybind11>=2.6.2
 Requires-Dist: scikit-image>=0.17.2
 Requires-Dist: sdss-sep>=1.2.3
 Requires-Dist: astropy<5.0.0; python_version <= "3.7"
 Requires-Dist: astropy>=5.0.0; python_version > "3.7"
 Requires-Dist: seaborn>=0.12.1
+Requires-Dist: pyarrow>=15.0.0; python_version > "3.7"
 Provides-Extra: dev
 Requires-Dist: flake8>=3.7.9; extra == "dev"
 Requires-Dist: doc8>=0.8.0; extra == "dev"
 Requires-Dist: pytest>=5.2.2; extra == "dev"
 Requires-Dist: pytest-cov>=2.8.1; extra == "dev"
 Requires-Dist: pytest-mock>=1.13.0; extra == "dev"
 Requires-Dist: pytest-sugar>=0.9.2; extra == "dev"
```

### Comparing `sdss-coordio-1.9.2/README.md` & `sdss-coordio-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/conv.cpp` & `sdss-coordio-1.9.3/cextern/conv.cpp`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dallpeaks.c` & `sdss-coordio-1.9.3/cextern/dimage/dallpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dcen3x3.c` & `sdss-coordio-1.9.3/cextern/dimage/dcen3x3.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dfind.c` & `sdss-coordio-1.9.3/cextern/dimage/dfind.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dfloodfill.c` & `sdss-coordio-1.9.3/cextern/dimage/dfloodfill.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dimage.h` & `sdss-coordio-1.9.3/cextern/dimage/dimage.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dmedsmooth.c` & `sdss-coordio-1.9.3/cextern/dimage/dmedsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dobjects.c` & `sdss-coordio-1.9.3/cextern/dimage/dobjects.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dpeaks.c` & `sdss-coordio-1.9.3/cextern/dimage/dpeaks.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/drefine.c` & `sdss-coordio-1.9.3/cextern/dimage/drefine.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dselip.c` & `sdss-coordio-1.9.3/cextern/dimage/dselip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dsigma.c` & `sdss-coordio-1.9.3/cextern/dimage/dsigma.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/dsmooth.c` & `sdss-coordio-1.9.3/cextern/dimage/dsmooth.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/dimage/simplexy.c` & `sdss-coordio-1.9.3/cextern/dimage/simplexy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/a2af.c` & `sdss-coordio-1.9.3/cextern/sofa/a2af.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/a2tf.c` & `sdss-coordio-1.9.3/cextern/sofa/a2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ab.c` & `sdss-coordio-1.9.3/cextern/sofa/ab.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ae2hd.c` & `sdss-coordio-1.9.3/cextern/sofa/ae2hd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/af2a.c` & `sdss-coordio-1.9.3/cextern/sofa/af2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/anp.c` & `sdss-coordio-1.9.3/cextern/sofa/anp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/anpm.c` & `sdss-coordio-1.9.3/cextern/sofa/anpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apcg.c` & `sdss-coordio-1.9.3/cextern/sofa/apcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apcg13.c` & `sdss-coordio-1.9.3/cextern/sofa/apcg13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apci.c` & `sdss-coordio-1.9.3/cextern/sofa/apci.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apci13.c` & `sdss-coordio-1.9.3/cextern/sofa/apci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apco.c` & `sdss-coordio-1.9.3/cextern/sofa/apco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apco13.c` & `sdss-coordio-1.9.3/cextern/sofa/apco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apcs.c` & `sdss-coordio-1.9.3/cextern/sofa/apcs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apcs13.c` & `sdss-coordio-1.9.3/cextern/sofa/apcs13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/aper.c` & `sdss-coordio-1.9.3/cextern/sofa/aper.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/aper13.c` & `sdss-coordio-1.9.3/cextern/sofa/aper13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apio.c` & `sdss-coordio-1.9.3/cextern/sofa/apio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/apio13.c` & `sdss-coordio-1.9.3/cextern/sofa/apio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atci13.c` & `sdss-coordio-1.9.3/cextern/sofa/atci13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atciq.c` & `sdss-coordio-1.9.3/cextern/sofa/atciq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atciqn.c` & `sdss-coordio-1.9.3/cextern/sofa/atciqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atciqz.c` & `sdss-coordio-1.9.3/cextern/sofa/atciqz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atco13.c` & `sdss-coordio-1.9.3/cextern/sofa/atco13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atic13.c` & `sdss-coordio-1.9.3/cextern/sofa/atic13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/aticq.c` & `sdss-coordio-1.9.3/cextern/sofa/aticq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/aticqn.c` & `sdss-coordio-1.9.3/cextern/sofa/aticqn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atio13.c` & `sdss-coordio-1.9.3/cextern/sofa/atio13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atioq.c` & `sdss-coordio-1.9.3/cextern/sofa/atioq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atoc13.c` & `sdss-coordio-1.9.3/cextern/sofa/atoc13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atoi13.c` & `sdss-coordio-1.9.3/cextern/sofa/atoi13.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/atoiq.c` & `sdss-coordio-1.9.3/cextern/sofa/atoiq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/bi00.c` & `sdss-coordio-1.9.3/cextern/sofa/bi00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/bp00.c` & `sdss-coordio-1.9.3/cextern/sofa/bp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/bp06.c` & `sdss-coordio-1.9.3/cextern/sofa/bp06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/bpn2xy.c` & `sdss-coordio-1.9.3/cextern/sofa/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2i00a.c` & `sdss-coordio-1.9.3/cextern/sofa/c2i00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2i00b.c` & `sdss-coordio-1.9.3/cextern/sofa/c2i00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2i06a.c` & `sdss-coordio-1.9.3/cextern/sofa/c2i06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2ibpn.c` & `sdss-coordio-1.9.3/cextern/sofa/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2ixy.c` & `sdss-coordio-1.9.3/cextern/sofa/c2ixy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2ixys.c` & `sdss-coordio-1.9.3/cextern/sofa/c2ixys.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2s.c` & `sdss-coordio-1.9.3/cextern/sofa/c2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2t00a.c` & `sdss-coordio-1.9.3/cextern/sofa/c2t00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2t00b.c` & `sdss-coordio-1.9.3/cextern/sofa/c2t00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2t06a.c` & `sdss-coordio-1.9.3/cextern/sofa/c2t06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2tcio.c` & `sdss-coordio-1.9.3/cextern/sofa/c2tcio.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2teqx.c` & `sdss-coordio-1.9.3/cextern/sofa/c2teqx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2tpe.c` & `sdss-coordio-1.9.3/cextern/sofa/c2tpe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/c2txy.c` & `sdss-coordio-1.9.3/cextern/sofa/c2txy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/cal2jd.c` & `sdss-coordio-1.9.3/cextern/sofa/cal2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/cp.c` & `sdss-coordio-1.9.3/cextern/sofa/cp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/cpv.c` & `sdss-coordio-1.9.3/cextern/sofa/cpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/cr.c` & `sdss-coordio-1.9.3/cextern/sofa/cr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/d2dtf.c` & `sdss-coordio-1.9.3/cextern/sofa/d2dtf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/d2tf.c` & `sdss-coordio-1.9.3/cextern/sofa/d2tf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/dat.c` & `sdss-coordio-1.9.3/cextern/sofa/dat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/dtdb.c` & `sdss-coordio-1.9.3/cextern/sofa/dtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/dtf2d.c` & `sdss-coordio-1.9.3/cextern/sofa/dtf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eceq06.c` & `sdss-coordio-1.9.3/cextern/sofa/eceq06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ecm06.c` & `sdss-coordio-1.9.3/cextern/sofa/ecm06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ee00.c` & `sdss-coordio-1.9.3/cextern/sofa/ee00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ee00a.c` & `sdss-coordio-1.9.3/cextern/sofa/ee00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ee00b.c` & `sdss-coordio-1.9.3/cextern/sofa/ee00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ee06a.c` & `sdss-coordio-1.9.3/cextern/sofa/ee06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eect00.c` & `sdss-coordio-1.9.3/cextern/sofa/eect00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eform.c` & `sdss-coordio-1.9.3/cextern/sofa/eform.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eo06a.c` & `sdss-coordio-1.9.3/cextern/sofa/eo06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eors.c` & `sdss-coordio-1.9.3/cextern/sofa/eors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/epb.c` & `sdss-coordio-1.9.3/cextern/sofa/epb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/epb2jd.c` & `sdss-coordio-1.9.3/cextern/sofa/epb2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/epj.c` & `sdss-coordio-1.9.3/cextern/sofa/epj.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/epj2jd.c` & `sdss-coordio-1.9.3/cextern/sofa/epj2jd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/epv00.c` & `sdss-coordio-1.9.3/cextern/sofa/epv00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eqec06.c` & `sdss-coordio-1.9.3/cextern/sofa/eqec06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/eqeq94.c` & `sdss-coordio-1.9.3/cextern/sofa/eqeq94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/era00.c` & `sdss-coordio-1.9.3/cextern/sofa/era00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fad03.c` & `sdss-coordio-1.9.3/cextern/sofa/fad03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fae03.c` & `sdss-coordio-1.9.3/cextern/sofa/fae03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/faf03.c` & `sdss-coordio-1.9.3/cextern/sofa/faf03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/faju03.c` & `sdss-coordio-1.9.3/cextern/sofa/faju03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fal03.c` & `sdss-coordio-1.9.3/cextern/sofa/fal03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/falp03.c` & `sdss-coordio-1.9.3/cextern/sofa/falp03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fama03.c` & `sdss-coordio-1.9.3/cextern/sofa/fama03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fame03.c` & `sdss-coordio-1.9.3/cextern/sofa/fame03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fane03.c` & `sdss-coordio-1.9.3/cextern/sofa/fane03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/faom03.c` & `sdss-coordio-1.9.3/cextern/sofa/faom03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fapa03.c` & `sdss-coordio-1.9.3/cextern/sofa/fapa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fasa03.c` & `sdss-coordio-1.9.3/cextern/sofa/fasa03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/faur03.c` & `sdss-coordio-1.9.3/cextern/sofa/faur03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fave03.c` & `sdss-coordio-1.9.3/cextern/sofa/fave03.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk425.c` & `sdss-coordio-1.9.3/cextern/sofa/fk425.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk45z.c` & `sdss-coordio-1.9.3/cextern/sofa/fk45z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk524.c` & `sdss-coordio-1.9.3/cextern/sofa/fk524.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk52h.c` & `sdss-coordio-1.9.3/cextern/sofa/fk52h.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk54z.c` & `sdss-coordio-1.9.3/cextern/sofa/fk54z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk5hip.c` & `sdss-coordio-1.9.3/cextern/sofa/fk5hip.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fk5hz.c` & `sdss-coordio-1.9.3/cextern/sofa/fk5hz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fw2m.c` & `sdss-coordio-1.9.3/cextern/sofa/fw2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/fw2xy.c` & `sdss-coordio-1.9.3/cextern/sofa/fw2xy.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/g2icrs.c` & `sdss-coordio-1.9.3/cextern/sofa/g2icrs.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gc2gd.c` & `sdss-coordio-1.9.3/cextern/sofa/gc2gd.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gc2gde.c` & `sdss-coordio-1.9.3/cextern/sofa/gc2gde.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gd2gc.c` & `sdss-coordio-1.9.3/cextern/sofa/gd2gc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gd2gce.c` & `sdss-coordio-1.9.3/cextern/sofa/gd2gce.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gmst00.c` & `sdss-coordio-1.9.3/cextern/sofa/gmst00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gmst06.c` & `sdss-coordio-1.9.3/cextern/sofa/gmst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gmst82.c` & `sdss-coordio-1.9.3/cextern/sofa/gmst82.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gst00a.c` & `sdss-coordio-1.9.3/cextern/sofa/gst00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gst00b.c` & `sdss-coordio-1.9.3/cextern/sofa/gst00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gst06.c` & `sdss-coordio-1.9.3/cextern/sofa/gst06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gst06a.c` & `sdss-coordio-1.9.3/cextern/sofa/gst06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/gst94.c` & `sdss-coordio-1.9.3/cextern/sofa/gst94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/h2fk5.c` & `sdss-coordio-1.9.3/cextern/sofa/h2fk5.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/hd2ae.c` & `sdss-coordio-1.9.3/cextern/sofa/hd2ae.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/hd2pa.c` & `sdss-coordio-1.9.3/cextern/sofa/hd2pa.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/hfk5z.c` & `sdss-coordio-1.9.3/cextern/sofa/hfk5z.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/icrs2g.c` & `sdss-coordio-1.9.3/cextern/sofa/icrs2g.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ir.c` & `sdss-coordio-1.9.3/cextern/sofa/ir.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/jd2cal.c` & `sdss-coordio-1.9.3/cextern/sofa/jd2cal.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/jdcalf.c` & `sdss-coordio-1.9.3/cextern/sofa/jdcalf.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ld.c` & `sdss-coordio-1.9.3/cextern/sofa/ld.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ldn.c` & `sdss-coordio-1.9.3/cextern/sofa/ldn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ldsun.c` & `sdss-coordio-1.9.3/cextern/sofa/ldsun.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/lteceq.c` & `sdss-coordio-1.9.3/cextern/sofa/lteceq.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ltecm.c` & `sdss-coordio-1.9.3/cextern/sofa/ltecm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/lteqec.c` & `sdss-coordio-1.9.3/cextern/sofa/lteqec.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ltp.c` & `sdss-coordio-1.9.3/cextern/sofa/ltp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ltpb.c` & `sdss-coordio-1.9.3/cextern/sofa/ltpb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ltpecl.c` & `sdss-coordio-1.9.3/cextern/sofa/ltpecl.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ltpequ.c` & `sdss-coordio-1.9.3/cextern/sofa/ltpequ.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/makefile` & `sdss-coordio-1.9.3/cextern/sofa/makefile`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/num00a.c` & `sdss-coordio-1.9.3/cextern/sofa/num00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/num00b.c` & `sdss-coordio-1.9.3/cextern/sofa/num00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/num06a.c` & `sdss-coordio-1.9.3/cextern/sofa/num06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/numat.c` & `sdss-coordio-1.9.3/cextern/sofa/numat.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/nut00a.c` & `sdss-coordio-1.9.3/cextern/sofa/nut00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/nut00b.c` & `sdss-coordio-1.9.3/cextern/sofa/nut00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/nut06a.c` & `sdss-coordio-1.9.3/cextern/sofa/nut06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/nut80.c` & `sdss-coordio-1.9.3/cextern/sofa/nut80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/nutm80.c` & `sdss-coordio-1.9.3/cextern/sofa/nutm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/obl06.c` & `sdss-coordio-1.9.3/cextern/sofa/obl06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/obl80.c` & `sdss-coordio-1.9.3/cextern/sofa/obl80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/p06e.c` & `sdss-coordio-1.9.3/cextern/sofa/p06e.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/p2pv.c` & `sdss-coordio-1.9.3/cextern/sofa/p2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/p2s.c` & `sdss-coordio-1.9.3/cextern/sofa/p2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pap.c` & `sdss-coordio-1.9.3/cextern/sofa/pap.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pas.c` & `sdss-coordio-1.9.3/cextern/sofa/pas.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pb06.c` & `sdss-coordio-1.9.3/cextern/sofa/pb06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pdp.c` & `sdss-coordio-1.9.3/cextern/sofa/pdp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pfw06.c` & `sdss-coordio-1.9.3/cextern/sofa/pfw06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/plan94.c` & `sdss-coordio-1.9.3/cextern/sofa/plan94.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pm.c` & `sdss-coordio-1.9.3/cextern/sofa/pm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmat00.c` & `sdss-coordio-1.9.3/cextern/sofa/pmat00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmat06.c` & `sdss-coordio-1.9.3/cextern/sofa/pmat06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmat76.c` & `sdss-coordio-1.9.3/cextern/sofa/pmat76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmp.c` & `sdss-coordio-1.9.3/cextern/sofa/pmp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmpx.c` & `sdss-coordio-1.9.3/cextern/sofa/pmpx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pmsafe.c` & `sdss-coordio-1.9.3/cextern/sofa/pmsafe.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn.c` & `sdss-coordio-1.9.3/cextern/sofa/pn.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn00.c` & `sdss-coordio-1.9.3/cextern/sofa/pn00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn00a.c` & `sdss-coordio-1.9.3/cextern/sofa/pn00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn00b.c` & `sdss-coordio-1.9.3/cextern/sofa/pn00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn06.c` & `sdss-coordio-1.9.3/cextern/sofa/pn06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pn06a.c` & `sdss-coordio-1.9.3/cextern/sofa/pn06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pnm00a.c` & `sdss-coordio-1.9.3/cextern/sofa/pnm00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pnm00b.c` & `sdss-coordio-1.9.3/cextern/sofa/pnm00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pnm06a.c` & `sdss-coordio-1.9.3/cextern/sofa/pnm06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pnm80.c` & `sdss-coordio-1.9.3/cextern/sofa/pnm80.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pom00.c` & `sdss-coordio-1.9.3/cextern/sofa/pom00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ppp.c` & `sdss-coordio-1.9.3/cextern/sofa/ppp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ppsp.c` & `sdss-coordio-1.9.3/cextern/sofa/ppsp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pr00.c` & `sdss-coordio-1.9.3/cextern/sofa/pr00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/prec76.c` & `sdss-coordio-1.9.3/cextern/sofa/prec76.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pv2p.c` & `sdss-coordio-1.9.3/cextern/sofa/pv2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pv2s.c` & `sdss-coordio-1.9.3/cextern/sofa/pv2s.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvdpv.c` & `sdss-coordio-1.9.3/cextern/sofa/pvdpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvm.c` & `sdss-coordio-1.9.3/cextern/sofa/pvm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvmpv.c` & `sdss-coordio-1.9.3/cextern/sofa/pvmpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvppv.c` & `sdss-coordio-1.9.3/cextern/sofa/pvppv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvstar.c` & `sdss-coordio-1.9.3/cextern/sofa/pvstar.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvtob.c` & `sdss-coordio-1.9.3/cextern/sofa/pvtob.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvu.c` & `sdss-coordio-1.9.3/cextern/sofa/pvu.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvup.c` & `sdss-coordio-1.9.3/cextern/sofa/pvup.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pvxpv.c` & `sdss-coordio-1.9.3/cextern/sofa/pvxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/pxp.c` & `sdss-coordio-1.9.3/cextern/sofa/pxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/refco.c` & `sdss-coordio-1.9.3/cextern/sofa/refco.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rm2v.c` & `sdss-coordio-1.9.3/cextern/sofa/rm2v.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rv2m.c` & `sdss-coordio-1.9.3/cextern/sofa/rv2m.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rx.c` & `sdss-coordio-1.9.3/cextern/sofa/rx.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rxp.c` & `sdss-coordio-1.9.3/cextern/sofa/rxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rxpv.c` & `sdss-coordio-1.9.3/cextern/sofa/rxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rxr.c` & `sdss-coordio-1.9.3/cextern/sofa/rxr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ry.c` & `sdss-coordio-1.9.3/cextern/sofa/ry.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/rz.c` & `sdss-coordio-1.9.3/cextern/sofa/rz.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s00.c` & `sdss-coordio-1.9.3/cextern/sofa/s00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s00a.c` & `sdss-coordio-1.9.3/cextern/sofa/s00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s00b.c` & `sdss-coordio-1.9.3/cextern/sofa/s00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s06.c` & `sdss-coordio-1.9.3/cextern/sofa/s06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s06a.c` & `sdss-coordio-1.9.3/cextern/sofa/s06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s2c.c` & `sdss-coordio-1.9.3/cextern/sofa/s2c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s2p.c` & `sdss-coordio-1.9.3/cextern/sofa/s2p.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s2pv.c` & `sdss-coordio-1.9.3/cextern/sofa/s2pv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/s2xpv.c` & `sdss-coordio-1.9.3/cextern/sofa/s2xpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sepp.c` & `sdss-coordio-1.9.3/cextern/sofa/sepp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/seps.c` & `sdss-coordio-1.9.3/cextern/sofa/seps.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sofa.h` & `sdss-coordio-1.9.3/cextern/sofa/sofa.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sofam.h` & `sdss-coordio-1.9.3/cextern/sofa/sofam.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sp00.c` & `sdss-coordio-1.9.3/cextern/sofa/sp00.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/starpm.c` & `sdss-coordio-1.9.3/cextern/sofa/starpm.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/starpv.c` & `sdss-coordio-1.9.3/cextern/sofa/starpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sxp.c` & `sdss-coordio-1.9.3/cextern/sofa/sxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/sxpv.c` & `sdss-coordio-1.9.3/cextern/sofa/sxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/t_sofa_c.c` & `sdss-coordio-1.9.3/cextern/sofa/t_sofa_c.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/taitt.c` & `sdss-coordio-1.9.3/cextern/sofa/taitt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/taiut1.c` & `sdss-coordio-1.9.3/cextern/sofa/taiut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/taiutc.c` & `sdss-coordio-1.9.3/cextern/sofa/taiutc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tcbtdb.c` & `sdss-coordio-1.9.3/cextern/sofa/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tcgtt.c` & `sdss-coordio-1.9.3/cextern/sofa/tcgtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tdbtcb.c` & `sdss-coordio-1.9.3/cextern/sofa/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tdbtt.c` & `sdss-coordio-1.9.3/cextern/sofa/tdbtt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tf2a.c` & `sdss-coordio-1.9.3/cextern/sofa/tf2a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tf2d.c` & `sdss-coordio-1.9.3/cextern/sofa/tf2d.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tpors.c` & `sdss-coordio-1.9.3/cextern/sofa/tpors.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tporv.c` & `sdss-coordio-1.9.3/cextern/sofa/tporv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tpsts.c` & `sdss-coordio-1.9.3/cextern/sofa/tpsts.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tpstv.c` & `sdss-coordio-1.9.3/cextern/sofa/tpstv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tpxes.c` & `sdss-coordio-1.9.3/cextern/sofa/tpxes.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tpxev.c` & `sdss-coordio-1.9.3/cextern/sofa/tpxev.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tr.c` & `sdss-coordio-1.9.3/cextern/sofa/tr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/trxp.c` & `sdss-coordio-1.9.3/cextern/sofa/trxp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/trxpv.c` & `sdss-coordio-1.9.3/cextern/sofa/trxpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tttai.c` & `sdss-coordio-1.9.3/cextern/sofa/tttai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tttcg.c` & `sdss-coordio-1.9.3/cextern/sofa/tttcg.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/tttdb.c` & `sdss-coordio-1.9.3/cextern/sofa/tttdb.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ttut1.c` & `sdss-coordio-1.9.3/cextern/sofa/ttut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ut1tai.c` & `sdss-coordio-1.9.3/cextern/sofa/ut1tai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ut1tt.c` & `sdss-coordio-1.9.3/cextern/sofa/ut1tt.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/ut1utc.c` & `sdss-coordio-1.9.3/cextern/sofa/ut1utc.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/utctai.c` & `sdss-coordio-1.9.3/cextern/sofa/utctai.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/utcut1.c` & `sdss-coordio-1.9.3/cextern/sofa/utcut1.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/xy06.c` & `sdss-coordio-1.9.3/cextern/sofa/xy06.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/xys00a.c` & `sdss-coordio-1.9.3/cextern/sofa/xys00a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/xys00b.c` & `sdss-coordio-1.9.3/cextern/sofa/xys00b.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/xys06a.c` & `sdss-coordio-1.9.3/cextern/sofa/xys06a.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/zp.c` & `sdss-coordio-1.9.3/cextern/sofa/zp.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/zpv.c` & `sdss-coordio-1.9.3/cextern/sofa/zpv.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/cextern/sofa/zr.c` & `sdss-coordio-1.9.3/cextern/sofa/zr.c`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/setup.cfg` & `sdss-coordio-1.9.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sdss-coordio
-version = 1.9.2
+version = 1.9.3
 author = Conor Sayres
 author_email = csayres@uw.edu
 description = Coordinate conversion for SDSS-V
 url = https://github.com/sdss/coordio
 project_urls = 
 	Repository = https://github.com/sdss/coordio
 	Documentation = https://sdss-coordio.readthedocs.org
@@ -44,14 +44,15 @@
 	scipy>=1.2.1
 	pybind11>=2.6.2
 	scikit-image>=0.17.2
 	sdss-sep>=1.2.3
 	astropy<5.0.0; python_version<='3.7'
 	astropy>=5.0.0; python_version>'3.7'
 	seaborn>=0.12.1
+	pyarrow>=15.0.0; python_version>'3.7'
 
 [options.packages.find]
 where = 
 	src
 exclude = 
 	*.tests
```

### Comparing `sdss-coordio-1.9.2/setup.py` & `sdss-coordio-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/__init__.py` & `sdss-coordio-1.9.3/src/coordio/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/astrometry.py` & `sdss-coordio-1.9.3/src/coordio/astrometry.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/calibration.py` & `sdss-coordio-1.9.3/src/coordio/calibration.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/conv.py` & `sdss-coordio-1.9.3/src/coordio/conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/coordinate.py` & `sdss-coordio-1.9.3/src/coordio/coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/defaults.py` & `sdss-coordio-1.9.3/src/coordio/defaults.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/exceptions.py` & `sdss-coordio-1.9.3/src/coordio/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/extraction.py` & `sdss-coordio-1.9.3/src/coordio/extraction.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/fitData.py` & `sdss-coordio-1.9.3/src/coordio/fitData.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/guide.py` & `sdss-coordio-1.9.3/src/coordio/guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/iers.py` & `sdss-coordio-1.9.3/src/coordio/iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/include/coordio.h` & `sdss-coordio-1.9.3/src/coordio/include/coordio.h`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/positioner.py` & `sdss-coordio-1.9.3/src/coordio/positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/site.py` & `sdss-coordio-1.9.3/src/coordio/site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/sky.py` & `sdss-coordio-1.9.3/src/coordio/sky.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 
 # IAU-defined sky coordinate systems and transformations.
 
 from __future__ import annotations
 
 import ctypes
 import warnings
-from copy import deepcopy
 from typing import TYPE_CHECKING
 
 import numpy
 
 from . import conv, defaults, sofa
 from .coordinate import Coordinate, Coordinate2D, verifySite, verifyWavelength
 from .exceptions import CoordIOError, CoordIOUserWarning
 from .time import Time
 
-
 if TYPE_CHECKING:
     from .site import Site
 
 
 __all__ = ['ICRS', 'Observed']
 
 
@@ -420,7 +418,70 @@
             # earth rotation angle (from SOFA docs)
             # https://www.iausofa.org/2017_0420_C/sofa/sofa_ast_c.pdf
             era = sofa.iauEra00(ut1, 0)  # time is sum of the 2 args
             _ra = numpy.degrees(era + rlong - ha_obs.value)
             _ra = _ra % 360  # wrap ra
 
             self.ra[ii] = _ra
+
+    @classmethod
+    def fromEquatorial(cls, coords, hadec=False, site=None, **kwargs):
+        """Initialises `.Observed` coordinates  from equatorial topocentric.
+
+        Parameters
+        ----------
+        coords : numpy.ndarray
+            Nx2 Numpy array with the RA and Dec coordinates of the targets.
+            These must be topocentric equatorial coordinates that will be
+            converted to horizontal topocentric used to initialise `.Observed`.
+            Alternatively, if ``hadec=True`` then the first column in the array
+            must be the hour angle in degrees.
+        hadec : bool
+            Whether the coordinates are HA and declination.
+        site : .Site
+            The site from where observations will occur, along with the time
+            of the observation.  Mandatory argument.
+        kwargs
+            Other arguments to pass to `.Observed`.
+
+        """
+
+        coords = numpy.array(coords)
+
+        if len(coords.shape) != 2 or coords.shape[1] != 2:
+            raise CoordIOError('coords must be Nx2 array.')
+
+        if site is None:
+            raise CoordIOError('A site must be specified.')
+
+        lat_r = numpy.radians(site.latitude)
+        dec_d = coords[:, 1]
+        dec_r = numpy.radians(dec_d)
+
+        if hadec is False:
+            ra_d = coords[:, 0]
+            ra_r = numpy.radians(ra_d)
+
+            ut = site.time.to_ut1()
+            tt = site.time.to_tt()
+
+            gmst = sofa.iauGmst00(ut, 0.0, tt, 0.0)
+            lst_r = gmst + numpy.radians(site.longitude)
+
+            ha_r = lst_r - ra_r
+
+        else:
+            ha_r = numpy.radians(coords[:, 0])
+
+        # h = altitude, A = azimuth
+        sin_h = (numpy.sin(dec_r) * numpy.sin(lat_r) +
+                 numpy.cos(dec_r) * numpy.cos(lat_r) * numpy.cos(ha_r))
+        h_r = numpy.arcsin(sin_h)
+        h_d = numpy.degrees(h_r)
+
+        sin_A = -numpy.sin(ha_r) * numpy.cos(dec_r) / numpy.cos(h_r)
+        cos_A = ((numpy.sin(dec_r) - numpy.sin(lat_r) * numpy.sin(h_r)) /
+                 (numpy.cos(lat_r) * numpy.cos(h_r)))
+        A_r = numpy.arctan2(sin_A, cos_A)
+        A_d = numpy.degrees(A_r) % 360
+
+        return cls(numpy.array([h_d, A_d]).T, site=site, **kwargs)
```

### Comparing `sdss-coordio-1.9.2/src/coordio/sofa_bindings.py` & `sdss-coordio-1.9.3/src/coordio/sofa_bindings.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 import ctypes
 import datetime
 import importlib
 import os
 from ctypes import POINTER, c_char_p, c_double, c_int
 
-
 # List of argument times for some of the SOFA functions.
 ARGTYPES = [
 
     # const char *scale, int iy, int im, int id,
     #   int ihr, int imn, double sec,
     #   double *d1, double *d2
     ('iauDtf2d', (c_char_p, c_int, c_int, c_int,
@@ -86,15 +85,18 @@
     # args: double jd, double 0
     ('iauEra00', (c_double, c_double)),
 
     # Determine the constants A and B in the atmospheric refraction model
     # dZ = A tan Z + B tan^3 Z.
     # args: double phpa, double tc, double rh, double wl, double *refa, double *refb
     ('iauRefco', (c_double, c_double, c_double, c_double,
-                  POINTER(c_double), POINTER(c_double)))
+                  POINTER(c_double), POINTER(c_double))),
+    # Greenwich mean sidereal time (model consistent with IAU 2000 resolutions).
+    # args: double uta, double utb, double tta, double ttb
+    ('iauGmst00', (c_double, c_double, c_double, c_double))
 ]
 
 
 class SOFA(ctypes.CDLL):
     """Load the SOFA C extension.
 
     Parameters
@@ -131,14 +133,15 @@
             func.argtypes = argtypes
 
         # Some special cases of function that do not return
         # an integer error check.
         self.iauDtdb.restype = c_double
         self.iauHd2pa.restype = c_double
         self.iauEra00.restype = c_double
+        self.iauGmst00.restype = c_double
 
     def get_internal_date(self, date=None, scale='UTC'):
         """Returns the internal representation of a date.
 
         Parameters
         ----------
         date : ~datetime.datetime
@@ -151,15 +154,15 @@
         -------
         d1, d2 : `float`
             The two-part Julian date.
 
         """
 
         if date is None:
-            date = datetime.datetime.utcnow()
+            date = datetime.datetime.now(datetime.timezone.utc)
             scale = 'UTC'
 
         d1 = c_double()
         d2 = c_double()
 
         res = self.iauDtf2d(scale.upper().encode(), date.year, date.month,
                             date.day, date.hour, date.minute,
```

### Comparing `sdss-coordio-1.9.2/src/coordio/tangent.py` & `sdss-coordio-1.9.3/src/coordio/tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/telescope.py` & `sdss-coordio-1.9.3/src/coordio/telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/time.py` & `sdss-coordio-1.9.3/src/coordio/time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/transforms.py` & `sdss-coordio-1.9.3/src/coordio/transforms.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/utils.py` & `sdss-coordio-1.9.3/src/coordio/utils.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/wok.py` & `sdss-coordio-1.9.3/src/coordio/wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/zernike.py` & `sdss-coordio-1.9.3/src/coordio/zernike.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/coordio/zhaoburge.py` & `sdss-coordio-1.9.3/src/coordio/zhaoburge.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/src/sdss_coordio.egg-info/PKG-INFO` & `sdss-coordio-1.9.3/src/sdss_coordio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-coordio
-Version: 1.9.2
+Version: 1.9.3
 Summary: Coordinate conversion for SDSS-V
 Home-page: https://github.com/sdss/coordio
 Author: Conor Sayres
 Author-email: csayres@uw.edu
 License: BSD 3-Clause License
 Project-URL: Repository, https://github.com/sdss/coordio
 Project-URL: Documentation, https://sdss-coordio.readthedocs.org
@@ -30,14 +30,15 @@
 Requires-Dist: scipy>=1.2.1
 Requires-Dist: pybind11>=2.6.2
 Requires-Dist: scikit-image>=0.17.2
 Requires-Dist: sdss-sep>=1.2.3
 Requires-Dist: astropy<5.0.0; python_version <= "3.7"
 Requires-Dist: astropy>=5.0.0; python_version > "3.7"
 Requires-Dist: seaborn>=0.12.1
+Requires-Dist: pyarrow>=15.0.0; python_version > "3.7"
 Provides-Extra: dev
 Requires-Dist: flake8>=3.7.9; extra == "dev"
 Requires-Dist: doc8>=0.8.0; extra == "dev"
 Requires-Dist: pytest>=5.2.2; extra == "dev"
 Requires-Dist: pytest-cov>=2.8.1; extra == "dev"
 Requires-Dist: pytest-mock>=1.13.0; extra == "dev"
 Requires-Dist: pytest-sugar>=0.9.2; extra == "dev"
```

### Comparing `sdss-coordio-1.9.2/src/sdss_coordio.egg-info/SOURCES.txt` & `sdss-coordio-1.9.3/src/sdss_coordio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_conv.py` & `sdss-coordio-1.9.3/tests/test_conv.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_coordinate.py` & `sdss-coordio-1.9.3/tests/test_coordinate.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_fpScale.py` & `sdss-coordio-1.9.3/tests/test_fpScale.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_guide.py` & `sdss-coordio-1.9.3/tests/test_guide.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_iers.py` & `sdss-coordio-1.9.3/tests/test_iers.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_libcoordio.py` & `sdss-coordio-1.9.3/tests/test_libcoordio.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_offset.py` & `sdss-coordio-1.9.3/tests/test_offset.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_plPlug.py` & `sdss-coordio-1.9.3/tests/test_plPlug.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_positioner.py` & `sdss-coordio-1.9.3/tests/test_positioner.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_site.py` & `sdss-coordio-1.9.3/tests/test_site.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_sky.py` & `sdss-coordio-1.9.3/tests/test_sky.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,18 +9,16 @@
 import sys
 
 import astropy.time
 import numpy
 import pytest
 from astropy import units as u
 from astropy.coordinates import AltAz, Distance, EarthLocation, SkyCoord
-
 from coordio import ICRS, CoordIOError, Observed, Site
 
-
 wavelength = 7000
 
 icrs = ICRS([[100, 10], [101., 11]],
             pmra=[100, 0.1], pmdec=[-15, -0.5],
             parallax=[10., 10.], rvel=[100, 1000],
             epoch=[2451545, 2451545])
 
@@ -141,7 +139,47 @@
     observed = Observed(icrs, site=site)
     _icrs = ICRS(observed)
 
     a1 = SkyCoord(ra=icrs[:, 0] * u.deg, dec=icrs[:, 1] * u.deg)
     a2 = SkyCoord(ra=_icrs[:, 0] * u.deg, dec=_icrs[:, 1] * u.deg)
     sep = a1.separation(a2)
     assert numpy.max(numpy.array(sep) * 3600) < 0.5
+
+
+@pytest.mark.skipif(sys.version_info < (3, 8), reason='requires python 3.8+ for HADec')
+@pytest.mark.parametrize('hadec', [True, False])
+def test_observed_from_equatorial(hadec):
+    from astropy.coordinates import HADec
+
+    time = 2451545
+    site.set_time(time, scale='TAI')
+
+    ras = numpy.random.uniform(0, 360, 100)
+    decs = numpy.random.uniform(-90, 90, 100)
+
+    # Get HA for cases when hadec=True
+    astropy_time = astropy.time.Time(time, format='jd', scale='tai',
+                                     location=astropy_location)
+    astropy_lst = astropy_time.sidereal_time('mean').deg
+
+    ha_d = astropy_lst - ras
+    if hadec:
+        eqs = numpy.array((ha_d, decs)).T
+    else:
+        eqs = numpy.array([ras, decs]).T
+
+    observed = Observed.fromEquatorial(eqs, hadec=hadec, site=site,
+                                       wavelength=wavelength)
+
+    assert observed.shape == (100, 2)
+    assert numpy.all(observed[:, 0] > -90) and numpy.all(observed[:, 0] < 90)
+    assert numpy.all(observed[:, 1] > 0) and numpy.all(observed[:, 1] < 360)
+
+    # Now calculate the same using astropy and compare.
+    hadec_coords = HADec(ha=ha_d * u.deg, dec=decs * u.deg,
+                         obstime=astropy_time, location=astropy_location)
+
+    astropy_altaz = hadec_coords.transform_to(AltAz(location=astropy_location,
+                                                    obstime=astropy_time))
+
+    assert numpy.allclose(observed[:, 0], astropy_altaz.alt.deg, atol=1e-6)
+    assert numpy.allclose(observed[:, 1], astropy_altaz.az.deg % 360, atol=1e-6)
```

### Comparing `sdss-coordio-1.9.2/tests/test_sofa.py` & `sdss-coordio-1.9.3/tests/test_sofa.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_tangent.py` & `sdss-coordio-1.9.3/tests/test_tangent.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_tangentToPositioner2.py` & `sdss-coordio-1.9.3/tests/test_tangentToPositioner2.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_telescope.py` & `sdss-coordio-1.9.3/tests/test_telescope.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_time.py` & `sdss-coordio-1.9.3/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_wok.py` & `sdss-coordio-1.9.3/tests/test_wok.py`

 * *Files identical despite different names*

### Comparing `sdss-coordio-1.9.2/tests/test_zern.py` & `sdss-coordio-1.9.3/tests/test_zern.py`

 * *Files identical despite different names*

