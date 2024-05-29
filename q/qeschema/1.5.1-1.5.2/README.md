# Comparing `tmp/qeschema-1.5.1.tar.gz` & `tmp/qeschema-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qeschema-1.5.1.tar", last modified: Thu Feb 29 14:56:34 2024, max compression
+gzip compressed data, was "qeschema-1.5.2.tar", last modified: Wed May 29 10:09:37 2024, max compression
```

## Comparing `qeschema-1.5.1.tar` & `qeschema-1.5.2.tar`

### file list

```diff
@@ -1,204 +1,196 @@
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.843568 qeschema-1.5.1/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1185 2022-07-11 12:44:52.000000 qeschema-1.5.1/LICENSE
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      258 2022-06-15 14:09:20.000000 qeschema-1.5.1/MANIFEST.in
--rw-r--r--   0 pietro    (1001) pietro    (1001)     2938 2024-02-29 14:56:34.843568 qeschema-1.5.1/PKG-INFO
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1799 2024-02-29 13:17:10.000000 qeschema-1.5.1/README.rst
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.815569 qeschema-1.5.1/docs/
--rw-r--r--   0 pietro    (1001) pietro    (1001)    12288 2024-02-29 13:19:43.000000 qeschema-1.5.1/docs/.usage.rst.swp
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      634 2021-05-04 18:18:30.000000 qeschema-1.5.1/docs/Makefile
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2911 2022-07-11 12:44:52.000000 qeschema-1.5.1/docs/api.rst
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3962 2024-02-29 14:33:02.000000 qeschema-1.5.1/docs/conf.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      451 2021-05-04 18:18:30.000000 qeschema-1.5.1/docs/index.rst
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      108 2021-05-04 18:18:30.000000 qeschema-1.5.1/docs/intro.rst
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      795 2021-05-04 18:18:30.000000 qeschema-1.5.1/docs/make.bat
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1035 2024-02-29 13:19:34.000000 qeschema-1.5.1/docs/usage.rst
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.815569 qeschema-1.5.1/qeschema/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1245 2024-02-29 14:32:42.000000 qeschema-1.5.1/qeschema/__init__.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    16704 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/cards.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    48990 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/converters.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    27590 2024-02-20 16:18:48.000000 qeschema-1.5.1/qeschema/documents.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      717 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/exceptions.py
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.815569 qeschema-1.5.1/qeschema/hdf5/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3083 2022-07-11 12:44:52.000000 qeschema-1.5.1/qeschema/hdf5/__init__.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1526 2022-07-11 12:44:52.000000 qeschema-1.5.1/qeschema/namespaces.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    12869 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/options.py
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.819568 qeschema-1.5.1/qeschema/schemas/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8571 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/schemas/epw.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    30525 2021-11-22 14:42:16.000000 qeschema-1.5.1/qeschema/schemas/ph_xmlschema.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    58843 2024-02-29 12:54:58.000000 qeschema-1.5.1/qeschema/schemas/qes.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8832 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/qes_neb.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8841 2024-02-29 12:59:12.000000 qeschema-1.5.1/qeschema/schemas/qes_neb_test_ref.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3442 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/qes_spectrum.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    49802 2024-02-29 12:54:58.000000 qeschema-1.5.1/qeschema/schemas/qes_test_ref.xsd
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.823568 qeschema-1.5.1/qeschema/schemas/releases/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    30392 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/ph-20180511.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    30254 2021-11-22 14:42:16.000000 qeschema-1.5.1/qeschema/schemas/releases/ph-20210706.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    30392 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/ph_temp.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    36064 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes-20180510.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    39211 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes-20180511.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    42863 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_030920.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    40726 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_181201.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    41056 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_190207.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    41048 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_190304.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    41127 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_190719.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    41106 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_191206.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    42231 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_200420.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    42863 2021-12-17 09:34:55.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_210716.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    49802 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_211101.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    58843 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_230310.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8779 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_neb-20180511.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8833 2023-04-27 09:38:03.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_neb-211101.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3269 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_spectrum-20180511.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3442 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/qes_spectrum-20180517.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7890 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/tddfpt-20180511.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8049 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/releases/tddfpt-20180517.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8049 2021-05-04 18:18:30.000000 qeschema-1.5.1/qeschema/schemas/tddfpt.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     8075 2022-07-11 12:44:52.000000 qeschema-1.5.1/qeschema/schemas/xspectra.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4563 2022-06-15 14:09:20.000000 qeschema-1.5.1/qeschema/upf.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5174 2022-06-15 14:09:20.000000 qeschema-1.5.1/qeschema/utils.py
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.843568 qeschema-1.5.1/qeschema.egg-info/
--rw-r--r--   0 pietro    (1001) pietro    (1001)     2938 2024-02-29 14:56:34.000000 qeschema-1.5.1/qeschema.egg-info/PKG-INFO
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6533 2024-02-29 14:56:34.000000 qeschema-1.5.1/qeschema.egg-info/SOURCES.txt
--rw-rw-r--   0 pietro    (1001) pietro    (1001)        1 2024-02-29 14:56:34.000000 qeschema-1.5.1/qeschema.egg-info/dependency_links.txt
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       58 2024-02-29 14:56:34.000000 qeschema-1.5.1/qeschema.egg-info/requires.txt
--rw-rw-r--   0 pietro    (1001) pietro    (1001)        9 2024-02-29 14:56:34.000000 qeschema-1.5.1/qeschema.egg-info/top_level.txt
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      185 2024-02-29 12:54:58.000000 qeschema-1.5.1/requirements-dev.txt
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.823568 qeschema-1.5.1/scripts/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      231 2022-01-26 15:51:54.000000 qeschema-1.5.1/scripts/check.ipynb
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4510 2022-01-27 09:56:11.000000 qeschema-1.5.1/scripts/pwsmartpar.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     3141 2023-04-27 09:38:03.000000 qeschema-1.5.1/scripts/xml2qeinput.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     2952 2024-02-29 12:54:58.000000 qeschema-1.5.1/scripts/yaml2qeinput.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       38 2024-02-29 14:56:34.843568 qeschema-1.5.1/setup.cfg
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1914 2024-02-29 14:31:44.000000 qeschema-1.5.1/setup.py
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.823568 qeschema-1.5.1/tests/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)        0 2021-05-04 18:18:30.000000 qeschema-1.5.1/tests/__init__.py
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.811569 qeschema-1.5.1/tests/examples/
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.823568 qeschema-1.5.1/tests/examples/pw/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1865 2021-12-17 09:50:22.000000 qeschema-1.5.1/tests/examples/pw/Al001_relax_bfgs.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1653 2022-01-27 09:25:04.000000 qeschema-1.5.1/tests/examples/pw/CO_bgfs_relax.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1845 2021-06-28 17:39:41.000000 qeschema-1.5.1/tests/examples/pw/Fe_noncolin.in
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.811569 qeschema-1.5.1/tests/resources/
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.827569 qeschema-1.5.1/tests/resources/dummy/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      150 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/incomplete.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1111 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/incomplete.xsd
--rw-rw-r--   0 pietro    (1001) pietro    (1001)        2 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance.csv
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       38 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance.json
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      107 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       41 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance.yaml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       48 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance_json
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      107 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance_xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)       45 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/instance_yaml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      679 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/dummy/schema.xsd
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.827569 qeschema-1.5.1/tests/resources/epw/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      322 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/epw/epw_test1.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1057 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/epw/epw_test1.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      684 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/epw/epw_test2.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1566 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/epw/epw_test2.xml
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.827569 qeschema-1.5.1/tests/resources/neb/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2142 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/neb/Al001+H_pbc.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6085 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/neb/Al001+H_pbc.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2145 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/neb/Al001_plus_H_bc3.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6127 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/neb/Al001_plus_H_bc3.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1888 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/neb/H2+H.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7040 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/neb/H2+H.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1947 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/neb/H2+H_crystal.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7198 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/neb/H2+H_crystal.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2652 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5111 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.xml
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.831569 qeschema-1.5.1/tests/resources/ph/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      263 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/al.elph.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1135 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/al.elph.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      231 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/alas_ph.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      943 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/alas_ph.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      272 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/alas_recover.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1010 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/alas_recover.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      185 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/ch4_nm.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      802 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/ch4_nm.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      189 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/nat_todo.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      721 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/nat_todo.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      194 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/nat_todo_zero.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      675 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/nat_todo_zero.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      153 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_dielectric.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      671 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_dielectric.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      164 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_prova_disp.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      884 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_prova_disp.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      315 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_prova_qplot.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1460 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/ph/sio2_prova_qplot.xml
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.839568 qeschema-1.5.1/tests/resources/pw/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2708 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs-input.yml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1865 2024-02-29 14:54:29.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1866 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6331 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.json
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5503 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3661 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.yml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1784 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al001_rlx_damp.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5181 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Al001_rlx_damp.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1838 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al_bands.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7456 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Al_bands.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1600 2024-02-29 13:41:17.000000 qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4848 2024-02-29 13:34:03.000000 qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1770 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax_with_external_forces.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5124 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax_with_external_forces.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2780 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/ESM_2Dxy.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5112 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/ESM_2Dxy.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1780 2022-07-11 16:02:07.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1848 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6750 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1810 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard_230310.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6785 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard_230310.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1789 2022-07-11 16:02:51.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1857 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6762 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1792 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U_230310.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     6826 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U_230310.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1810 2022-07-11 16:03:30.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1878 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7477 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2028 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     7528 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1734 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Fe_Im-3m_0_dftd3.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3473 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Fe_Im-3m_0_dftd3.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1711 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Fe_crystal_crystal_positions.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     3382 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Fe_crystal_crystal_positions.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1809 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Fe_non_collinear_penalty.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5963 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Fe_non_collinear_penalty.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1726 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Fe_noncolin.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5710 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Fe_noncolin.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    43750 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Ni.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1820 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_BerryPhase.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5056 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_BerryPhase.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1839 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_bc3_fcp_opt.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4941 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_bc3_fcp_opt.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1717 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_scf.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4729 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/PbTiO3_scf.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1462 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Pt_spinorbit.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     4346 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Pt_spinorbit.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    63072 2024-02-29 13:12:59.000000 qeschema-1.5.1/tests/resources/pw/Si.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1977 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/pw/Si_md.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     5386 2024-02-29 12:54:58.000000 qeschema-1.5.1/tests/resources/pw/Si_md.xml
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.839568 qeschema-1.5.1/tests/resources/tddfpt/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      161 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/Ag.tddfpt-eels.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      708 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/Ag.tddfpt-eels.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      238 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/Benzene.dav.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      920 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/Benzene.dav.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      113 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      637 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      148 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt_pp.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      634 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt_pp.xml
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.839568 qeschema-1.5.1/tests/resources/upf/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)    25648 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/resources/upf/N.pz-vbc.UPF
-drwxrwxr-x   0 pietro    (1001) pietro    (1001)        0 2024-02-29 14:56:34.843568 qeschema-1.5.1/tests/resources/xspectra/
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      398 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/Cu_L23_xspectra.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1321 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/Cu_L23_xspectra.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      405 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/NiO_xspectra_dip.in.test
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1385 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/NiO_xspectra_dip.xml
--rw-rw-r--   0 pietro    (1001) pietro    (1001)      989 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/xspectra_example_full.in
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     2755 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/resources/xspectra/xspectra_example_full.xml
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)    25743 2023-04-27 09:38:03.000000 qeschema-1.5.1/tests/test_cards.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     5235 2024-02-29 14:25:09.000000 qeschema-1.5.1/tests/test_converters.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)    32204 2024-02-29 13:46:32.000000 qeschema-1.5.1/tests/test_documents.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     1268 2022-07-11 12:44:52.000000 qeschema-1.5.1/tests/test_hdf5.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)    14478 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/test_options.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     1328 2022-06-15 14:09:20.000000 qeschema-1.5.1/tests/test_upf.py
--rwxrwxr-x   0 pietro    (1001) pietro    (1001)     9104 2021-05-04 18:18:30.000000 qeschema-1.5.1/tests/test_utils.py
--rw-rw-r--   0 pietro    (1001) pietro    (1001)     1048 2024-02-29 12:54:58.000000 qeschema-1.5.1/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.830052 qeschema-1.5.2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1185 2023-04-21 10:24:12.000000 qeschema-1.5.2/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      258 2021-12-13 14:40:32.000000 qeschema-1.5.2/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2989 2024-05-29 10:09:37.830052 qeschema-1.5.2/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1799 2024-05-13 14:51:40.000000 qeschema-1.5.2/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.813053 qeschema-1.5.2/docs/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      634 2019-12-12 12:55:26.000000 qeschema-1.5.2/docs/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2911 2023-04-21 10:24:12.000000 qeschema-1.5.2/docs/api.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3962 2024-05-29 09:52:54.000000 qeschema-1.5.2/docs/conf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      451 2019-12-12 12:55:26.000000 qeschema-1.5.2/docs/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      108 2019-12-12 12:55:26.000000 qeschema-1.5.2/docs/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      795 2019-12-12 12:55:26.000000 qeschema-1.5.2/docs/make.bat
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1035 2024-05-13 14:51:40.000000 qeschema-1.5.2/docs/usage.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.814053 qeschema-1.5.2/qeschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1245 2024-05-29 09:52:54.000000 qeschema-1.5.2/qeschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16705 2024-05-29 09:52:54.000000 qeschema-1.5.2/qeschema/cards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    48990 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27872 2024-05-29 09:52:54.000000 qeschema-1.5.2/qeschema/documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      717 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/exceptions.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.814053 qeschema-1.5.2/qeschema/hdf5/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3083 2023-04-21 10:24:12.000000 qeschema-1.5.2/qeschema/hdf5/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1526 2023-04-21 10:24:12.000000 qeschema-1.5.2/qeschema/namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    12869 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/options.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.815053 qeschema-1.5.2/qeschema/schemas/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8571 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/schemas/epw.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30525 2021-12-13 13:49:21.000000 qeschema-1.5.2/qeschema/schemas/ph_xmlschema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    58843 2024-05-13 14:51:40.000000 qeschema-1.5.2/qeschema/schemas/qes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8832 2019-01-17 09:16:05.000000 qeschema-1.5.2/qeschema/schemas/qes_neb.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8841 2024-05-13 14:51:40.000000 qeschema-1.5.2/qeschema/schemas/qes_neb_test_ref.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3442 2018-06-29 13:43:25.000000 qeschema-1.5.2/qeschema/schemas/qes_spectrum.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49802 2024-05-13 14:51:40.000000 qeschema-1.5.2/qeschema/schemas/qes_test_ref.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.817052 qeschema-1.5.2/qeschema/schemas/releases/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30392 2018-06-29 15:21:39.000000 qeschema-1.5.2/qeschema/schemas/releases/ph-20180511.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30254 2021-12-13 13:49:21.000000 qeschema-1.5.2/qeschema/schemas/releases/ph-20210706.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30392 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/schemas/releases/ph_temp.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    36064 2018-06-29 13:25:01.000000 qeschema-1.5.2/qeschema/schemas/releases/qes-20180510.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    39211 2018-06-29 13:45:39.000000 qeschema-1.5.2/qeschema/schemas/releases/qes-20180511.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    42863 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_030920.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    40726 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_181201.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41056 2019-12-12 12:55:27.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_190207.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41048 2019-12-12 12:55:27.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_190304.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41127 2019-12-12 12:55:27.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_190719.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    41106 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_191206.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    42231 2020-12-30 17:40:32.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_200420.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49802 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_211101.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    58843 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_230310.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8779 2018-06-29 13:46:41.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_neb-20180511.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8833 2023-05-12 10:39:28.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_neb-211101.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3269 2018-06-29 13:51:55.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_spectrum-20180511.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3442 2018-06-29 13:43:25.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_spectrum-20180517.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    60146 2024-05-29 09:52:54.000000 qeschema-1.5.2/qeschema/schemas/releases/qes_test_240411.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7890 2018-06-29 13:49:39.000000 qeschema-1.5.2/qeschema/schemas/releases/tddfpt-20180511.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8049 2018-06-29 13:50:44.000000 qeschema-1.5.2/qeschema/schemas/releases/tddfpt-20180517.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8049 2018-06-29 13:50:44.000000 qeschema-1.5.2/qeschema/schemas/tddfpt.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8075 2023-04-21 10:24:12.000000 qeschema-1.5.2/qeschema/schemas/xspectra.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4563 2023-04-21 10:24:12.000000 qeschema-1.5.2/qeschema/upf.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5500 2024-05-29 09:52:54.000000 qeschema-1.5.2/qeschema/utils.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.830052 qeschema-1.5.2/qeschema.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2989 2024-05-29 10:09:37.000000 qeschema-1.5.2/qeschema.egg-info/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6279 2024-05-29 10:09:37.000000 qeschema-1.5.2/qeschema.egg-info/SOURCES.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        1 2024-05-29 10:09:37.000000 qeschema-1.5.2/qeschema.egg-info/dependency_links.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       58 2024-05-29 10:09:37.000000 qeschema-1.5.2/qeschema.egg-info/requires.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        9 2024-05-29 10:09:37.000000 qeschema-1.5.2/qeschema.egg-info/top_level.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      185 2024-05-29 09:52:54.000000 qeschema-1.5.2/requirements-dev.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.818053 qeschema-1.5.2/scripts/
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3141 2023-05-12 10:39:28.000000 qeschema-1.5.2/scripts/xml2qeinput.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2952 2024-05-13 14:51:40.000000 qeschema-1.5.2/scripts/yaml2qeinput.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-05-29 10:09:37.830052 qeschema-1.5.2/setup.cfg
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1964 2024-05-29 09:52:54.000000 qeschema-1.5.2/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.819053 qeschema-1.5.2/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2018-06-29 12:30:41.000000 qeschema-1.5.2/tests/__init__.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.811053 qeschema-1.5.2/tests/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.819053 qeschema-1.5.2/tests/examples/pw/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1865 2021-12-13 14:16:16.000000 qeschema-1.5.2/tests/examples/pw/Al001_relax_bfgs.in
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.812053 qeschema-1.5.2/tests/resources/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.820052 qeschema-1.5.2/tests/resources/dummy/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      150 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/incomplete.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1111 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/incomplete.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        2 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance.csv
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      107 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       41 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance.yaml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       48 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance_json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      107 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance_xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       45 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/instance_yaml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      679 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/dummy/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.820052 qeschema-1.5.2/tests/resources/epw/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/epw/epw_test1.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1057 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/epw/epw_test1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      684 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/epw/epw_test2.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1566 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/epw/epw_test2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.822053 qeschema-1.5.2/tests/resources/neb/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2142 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/neb/Al001+H_pbc.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6085 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/neb/Al001+H_pbc.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2145 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/neb/Al001_plus_H_bc3.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6127 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/neb/Al001_plus_H_bc3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1888 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/neb/H2+H.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7040 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/neb/H2+H.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1947 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/neb/H2+H_crystal.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7198 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/neb/H2+H_crystal.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2652 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5111 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.823053 qeschema-1.5.2/tests/resources/ph/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      263 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/al.elph.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1135 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/al.elph.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      231 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/alas_ph.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      943 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/alas_ph.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/alas_recover.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1010 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/alas_recover.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      185 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/ch4_nm.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      802 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/ch4_nm.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      189 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/nat_todo.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      721 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/nat_todo.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      194 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/nat_todo_zero.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/nat_todo_zero.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      153 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_dielectric.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      671 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_dielectric.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      164 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_prova_disp.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_prova_disp.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      315 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_prova_qplot.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1460 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/ph/sio2_prova_qplot.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.828052 qeschema-1.5.2/tests/resources/pw/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2708 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs-input.yml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1865 2024-05-29 10:07:22.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1866 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6331 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5503 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.yml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1784 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al001_rlx_damp.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5181 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Al001_rlx_damp.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1838 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al_bands.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7456 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Al_bands.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1600 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4848 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1770 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax_with_external_forces.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5124 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax_with_external_forces.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2780 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/ESM_2Dxy.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5112 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/ESM_2Dxy.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1848 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6750 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1810 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard_230310.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6785 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard_230310.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1857 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6762 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1792 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U_230310.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6826 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U_230310.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1878 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7477 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2028 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7528 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1734 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Fe_Im-3m_0_dftd3.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3473 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Fe_Im-3m_0_dftd3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1711 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Fe_crystal_crystal_positions.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3382 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Fe_crystal_crystal_positions.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1809 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Fe_non_collinear_penalty.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5963 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Fe_non_collinear_penalty.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1726 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Fe_noncolin.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5710 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Fe_noncolin.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    43750 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Ni.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1820 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_BerryPhase.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5056 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_BerryPhase.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1839 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_bc3_fcp_opt.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4941 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_bc3_fcp_opt.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1717 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_scf.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4729 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/PbTiO3_scf.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1462 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Pt_spinorbit.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4346 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Pt_spinorbit.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63072 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Si.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1977 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/pw/Si_md.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5386 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/resources/pw/Si_md.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.829052 qeschema-1.5.2/tests/resources/tddfpt/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      161 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/Ag.tddfpt-eels.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/Ag.tddfpt-eels.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      238 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/Benzene.dav.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      920 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/Benzene.dav.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      113 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      637 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      148 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt_pp.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      634 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt_pp.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.829052 qeschema-1.5.2/tests/resources/upf/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    25648 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/upf/N.pz-vbc.UPF
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-05-29 10:09:37.830052 qeschema-1.5.2/tests/resources/xspectra/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      398 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/Cu_L23_xspectra.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1321 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/Cu_L23_xspectra.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      405 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/NiO_xspectra_dip.in.test
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1385 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/NiO_xspectra_dip.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      989 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/xspectra_example_full.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2755 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/resources/xspectra/xspectra_example_full.xml
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    25743 2023-05-12 10:39:28.000000 qeschema-1.5.2/tests/test_cards.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     5235 2024-05-13 14:51:40.000000 qeschema-1.5.2/tests/test_converters.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    32250 2024-05-29 09:52:54.000000 qeschema-1.5.2/tests/test_documents.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     1268 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/test_hdf5.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)    14478 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/test_options.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     1328 2023-04-21 10:24:12.000000 qeschema-1.5.2/tests/test_upf.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     9104 2019-12-12 12:55:27.000000 qeschema-1.5.2/tests/test_utils.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1327 2024-05-29 09:52:54.000000 qeschema-1.5.2/tox.ini
```

### Comparing `qeschema-1.5.1/LICENSE` & `qeschema-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/PKG-INFO` & `qeschema-1.5.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qeschema
-Version: 1.5.1
+Version: 1.5.2
 Summary: Schema-based tools and interfaces for Quantum Espresso data
 Home-page: https://github.com/QEF/qeschema
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,19 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 License-File: LICENSE
-Requires-Dist: xmlschema<2.4.0,>=1.6.4
+Requires-Dist: xmlschema<4.0.0,>=2.5.1
 Requires-Dist: numpy
 Provides-Extra: hdf5
 Requires-Dist: h5py; extra == "hdf5"
 Provides-Extra: yaml
 Requires-Dist: pyyaml; extra == "yaml"
 
 =====================================================
```

### Comparing `qeschema-1.5.1/README.rst` & `qeschema-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/docs/Makefile` & `qeschema-1.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/docs/api.rst` & `qeschema-1.5.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/docs/conf.py` & `qeschema-1.5.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'qeschema'
-copyright = '2015-2023, Quantum Espresso Foundation and SISSA'
+copyright = '2015-2024, Quantum Espresso Foundation and SISSA'
 author = 'Davide Brunato, Pietro Delugas'
 
 # The full version, including alpha/beta/rc tags
-release = '1.5.1'
+release = '1.5.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `qeschema-1.5.1/docs/make.bat` & `qeschema-1.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/docs/usage.rst` & `qeschema-1.5.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/__init__.py` & `qeschema-1.5.2/qeschema/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     NebDocument, TdDocument, TdSpectrumDocument, XSpectraDocument, EPWDocument
 from .converters import RawInputConverter, PwInputConverter, \
     PhononInputConverter, NebInputConverter, TdInputConverter, \
     TdSpectrumInputConverter, XSpectraInputConverter, EPWInputConverter
 from .exceptions import QESchemaError, XmlDocumentError
 from .utils import set_logger
 
-__version__ = '1.5.1'
+__version__ = '1.5.2'
 
 __all__ = [
     'XmlDocument', 'QeDocument', 'PwDocument', 'PhononDocument', 'NebDocument',
     'TdDocument', 'TdSpectrumDocument', 'EPWDocument', 'RawInputConverter',
     'PwInputConverter', 'PhononInputConverter', 'TdInputConverter',
     'TdSpectrumInputConverter', 'NebInputConverter', 'QESchemaError',
     'XmlDocumentError', 'set_logger', 'hdf5', 'XSpectraDocument',
```

### Comparing `qeschema-1.5.1/qeschema/cards.py` & `qeschema-1.5.2/qeschema/cards.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
                 background = value['@background']
                 if label == 'not found':
                     def labnl(nnum, lnum):
                         return f"{nnum}{llabels[lnum-1]}"
 
                     label = labnl(value['n2_number'], value['l2_number'])
                     if 'two' in background:
-                        label = f"{label}-{labnl(value['n3_number'],value['l3_number'])}"
+                        label = f"{label}-{labnl(value['n3_number'], value['l3_number'])}"
                     lines.append(f"U {specie}-{label}  {value['$']:8.3f}")
             elif tag == 'V':
                 speclab1 = f"{value['@specie1']}-{value['@label1']}"
                 speclab2 = f"{value['@specie2']}-{value['@label2']}"
                 index1 = value['@index1']
                 index2 = value['@index2']
                 lines.append(f"{tag} {speclab1} {speclab2} {index1} {index2} {value['$']:8.3f}")
```

### Comparing `qeschema-1.5.1/qeschema/converters.py` & `qeschema-1.5.2/qeschema/converters.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/documents.py` & `qeschema-1.5.2/qeschema/documents.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 import json
 from abc import ABCMeta
 from functools import wraps
 from xml.etree import ElementTree
 import xmlschema
 from xmlschema import etree_tostring
 
-
 try:
     import yaml
 except ImportError:
     yaml = None
 
 from .namespaces import XSD_NAMESPACE
 from .converters import RawInputConverter, PwInputConverter, PhononInputConverter, \
     NebInputConverter, TdInputConverter, TdSpectrumInputConverter, \
     XSpectraInputConverter, EPWInputConverter
 from .exceptions import XmlDocumentError
-from .utils import etree_iter_path
+from .utils import etree_iter_path, get_target_prefix
 
 logger = logging.getLogger('qeschema')
 
 SCHEMAS_DIR = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'schemas')
 
 
 def requires_xml_data(method):
@@ -44,15 +43,15 @@
     return check_xml_data
 
 
 def removeprefix(s, prefix):
     return s[len(prefix):] if s.startswith(prefix) else s
 
 
-class XmlDocument(object):
+class XmlDocument:
     """
     Base class for a generic XML document based on an XSD schema. The schema
     associated is used for checking types, validation of the XML data and for
     lookup of default values. XML data is loaded into memory into an ElementTree
     structure. Data files can be also in JSON or YAML format, in these cases the
     data source is converted to XML when loading.
 
@@ -114,19 +113,23 @@
         if source is not None:
             self.from_xml(source, validation='lax')
 
     @property
     def namespaces(self):
         """
         XML data namespaces map, a dictionary that maps prefixes to URI. An empty
-        dictionary if the XML data file is not loaded or it doesn't contain any
+        dictionary if the XML data file is not loaded or if it doesn't contain any
         namespace declaration.
         """
         return {k: v for k, v in self._namespaces.items()}
 
+    @property
+    def default_namespace(self):
+        return self._namespaces.get('', '')
+
     @classmethod
     def fetch_schema(cls, filename):
         filename = filename.strip()
         if os.path.isfile(filename):
             return filename
 
         if not filename.startswith('/'):
@@ -438,28 +441,33 @@
     def __init__(self, source=None, schema=None, input_builder=None):
         super(QeDocument, self).__init__(source, schema)
 
         if input_builder is None:
             self.input_builder = self.DEFAULT_INPUT_BUILDER
         elif not isinstance(input_builder, type) or \
                 not issubclass(input_builder, RawInputConverter):
-            msg = "3rd argument must be a {!r} subclass"
-            raise XmlDocumentError(msg.format(RawInputConverter))
+            raise XmlDocumentError(f"3rd argument must be a {RawInputConverter!r} subclass")
         else:
             self.input_builder = input_builder
 
-        self.default_namespace = self.schema.target_namespace
-        qe_prefixes = ['qes', 'neb', 'qes_ph', 'qes_lr', 'qes_spectrum',
-                       'qes_xspectra', 'epw']
-        qe_nslist = list(map(self.schema.namespaces.get, qe_prefixes))
-        if self.default_namespace not in qe_nslist:
+        self._xpath_namespaces = {k: v for k, v in self.schema.namespaces.items() if k}
+
+        prefix = get_target_prefix(self.schema.namespaces, self.schema.target_namespace)
+        if prefix not in ('qes', 'neb', 'qes_ph', 'qes_lr',
+                          'qes_spectrum', 'qes_xspectra', 'epw'):
             raise NotImplementedError(
-                "Converter not implemented for this schema {}".format(self.default_namespace)
+                f"Converter not implemented for namespace {self.schema.target_namespace!r}"
             )
 
+    def _xsd_find(self, path, xsd_element=None):
+        if xsd_element is None:
+            return self.schema.find(path, self._xpath_namespaces)
+        else:
+            return xsd_element.find(path, self._xpath_namespaces)
+
     @property
     def input_path(self):
         """The path to XML input section."""
         return 'input'
 
     @property
     def output_path(self):
@@ -487,23 +495,23 @@
         input_path = './%s' % self.input_path
 
         input_root = self.find(input_path)
         if input_root is None:
             raise XmlDocumentError("Missing input {!r} in XML data!".format(input_path))
 
         for schema_root in self.schema.elements.values():
-            if schema_root.find(input_path):
+            if self._xsd_find(input_path, schema_root):
                 break
         else:
             raise XmlDocumentError("Missing input element in XSD schema!")
 
         # Extract values from input's subtree of the XML document
         for elem, path in etree_iter_path(input_root, path=input_path):
             rel_path = path.replace(input_path, '.')
-            xsd_element = schema_root.find(path)
+            xsd_element = self._xsd_find(path, schema_root)
             if xsd_element is None:
                 logger.error("%r doesn't match any element!", path)
                 continue
             else:
                 value = xsd_element.decode(elem, use_defaults=use_defaults)
                 if isinstance(value, str):
                     value = value.strip()
@@ -542,15 +550,15 @@
         Gets atomic symbols and atomic positions from XML output data.
 
         :return: the list of atomic symbols and a nested list containing the coordinates
         """
         path = './/output//atomic_positions'
         elem = self.find(path)
         if elem is not None:
-            atomic_positions = self.schema.find(path).decode(elem)
+            atomic_positions = self._xsd_find(path).decode(elem)
             atoms = atomic_positions.get('atom')
             if not isinstance(atoms, list):
                 atoms = [atoms]
             symbols = [a['@name'] for a in atoms]
             positions = [a['$'] for a in atoms]
             return symbols, positions
 
@@ -560,28 +568,28 @@
         Gets cell parameters from an XML output data.
 
         :return: a nested list containing the cell vectors in Bohr atomic units
         """
         path = './/output//cell'
         elem = self.find(path)
         if elem is not None:
-            cell = self.schema.find(path).decode(elem)
+            cell = self._xsd_find(path).decode(elem)
             return [cell['a1'], cell['a2'], cell['a3']]
 
     @requires_xml_data
     def get_stress(self):
         """
         Gets stress tensor from the XML output data, if present.
 
         :return: nested list containing the stress tensor in C order
         """
         path = './/output//stress'
         elem = self.find(path)
         if elem is not None:
-            stress = self.schema.find(path).decode(elem)
+            stress = self._xsd_find(path).decode(elem)
             try:
                 stress = stress['$']
             except TypeError:
                 pass
             return [stress[::3], stress[1::3], stress[2::3]]
 
     @requires_xml_data
@@ -591,18 +599,17 @@
 
         :return: the list of atomic symbols plus a nested list with the forces \
         in atomic units
         """
         path = './/output/forces'
         elem = self.find(path)
         if elem is not None:
-            forces = self.schema.find(path).decode(elem)
+            forces = self._xsd_find(path).decode(elem)
             path = './/output//atomic_positions'
-            breakpoint()
-            atomic_positions = self.schema.find(path).decode(self.find(path))
+            atomic_positions = self._xsd_find(path).decode(self.find(path))
             atoms = atomic_positions.get('atom', [])
             if not isinstance(atoms, list):
                 atoms = [atoms]
             symbols = [a['@name'] for a in atoms]
             i0 = range(3 * len(atoms))[::3]
             i1 = range(3 * len(atoms) + 1)[3::3]
             forces = [forces['$'][i:j] for i, j in zip(i0, i1)]
@@ -612,27 +619,27 @@
     def get_k_points(self):
         """
         Extracts the k_points list from the XML output data.
 
         :return: nested list with k_points
         """
         path = './/output//ks_energies/k_point'
-        return [self.schema.find(path).decode(e)['$'] for e in self.findall(path)]
+        return [self._xsd_find(path).decode(e)['$'] for e in self.findall(path)]
 
     @requires_xml_data
     def get_ks_eigenvalues(self):
         """
         Extracts the eigenvalues from the XML output data.
 
         :return: nested list of KS eigenvalues for each k_point in Hartree Units
         """
         path = './/output//ks_energies/eigenvalues'
         eigenvalues = []
         for e in self.findall(path):
-            obj = self.schema.find(path).decode(e)
+            obj = self._xsd_find(path).decode(e)
             if isinstance(obj, dict):
                 eigenvalues.append(obj['$'])  # pragma: no cover
             else:
                 eigenvalues.append(obj)
 
         return eigenvalues
 
@@ -640,15 +647,15 @@
     def get_total_energy(self):
         """
         Extracts the total energy from the  XML output data.
 
         :return: total energy in Hartree Units
         """
         path = './/output//etot'
-        return self.schema.find(path).decode(self.find(path))
+        return self._xsd_find(path).decode(self.find(path))
 
 
 class PhononDocument(QeDocument):
     """
     Class to manage Phonon XML documents.
     """
     DEFAULT_SCHEMA = 'ph_xmlschema.xsd'
```

### Comparing `qeschema-1.5.1/qeschema/exceptions.py` & `qeschema-1.5.2/qeschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/hdf5/__init__.py` & `qeschema-1.5.2/qeschema/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/namespaces.py` & `qeschema-1.5.2/qeschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/options.py` & `qeschema-1.5.2/qeschema/options.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/epw.xsd` & `qeschema-1.5.2/qeschema/schemas/epw.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/ph_xmlschema.xsd` & `qeschema-1.5.2/qeschema/schemas/ph_xmlschema.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/qes.xsd` & `qeschema-1.5.2/qeschema/schemas/qes.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/qes_neb.xsd` & `qeschema-1.5.2/qeschema/schemas/qes_neb.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/qes_neb_test_ref.xsd` & `qeschema-1.5.2/qeschema/schemas/qes_neb_test_ref.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/qes_spectrum.xsd` & `qeschema-1.5.2/qeschema/schemas/qes_spectrum.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/qes_test_ref.xsd` & `qeschema-1.5.2/qeschema/schemas/qes_test_ref.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/ph-20180511.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/ph-20180511.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/ph-20210706.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/ph-20210706.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/ph_temp.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/ph_temp.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes-20180510.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes-20180510.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes-20180511.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes-20180511.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_030920.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_030920.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_181201.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_181201.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_190207.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_190207.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_190304.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_190304.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_190719.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_190719.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_191206.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_191206.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_200420.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_200420.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_210716.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_211101.xsd`

 * *Files 7% similar despite different names*

#### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_210716.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_211101.xsd`

```diff
@@ -1,26 +1,29 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
 Copyright (c), 2015-2016, Quantum Espresso Foundation. All rights reserved.
 This file is distributed under the terms of the MIT License. See the
 file 'LICENSE' in the root directory of the present distribution, or
 http://opensource.org/licenses/MIT.
 Authors: Antonio Zambon, Paolo Giannozzi, Pietro Delugas
+datecode 211101
 -->
 <schema xmlns="http://www.w3.org/2001/XMLSchema" xmlns:qes="http://www.quantum-espresso.org/ns/qes/qes-1.0" targetNamespace="http://www.quantum-espresso.org/ns/qes/qes-1.0">
   <!-- ESPRESSO (root element) -->
   <element name="espresso" type="qes:espressoType"/>
   <complexType name="espressoType">
     <sequence>
       <element type="qes:general_infoType" name="general_info" minOccurs="0"/>
       <element type="qes:parallel_infoType" name="parallel_info" minOccurs="0"/>
-      <element type="qes:inputType" name="input"/>
+      <element type="qes:inputType" name="input" minOccurs="0"/>
       <element type="qes:stepType" name="step" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:outputType" name="output" minOccurs="0"/>
-      <element type="qes:statusType" name="status" minOccurs="0"/>
+      <element type="qes:cpstatusType" name="STATUS" minOccurs="0"/>
+      <element type="qes:cptimestepsType" name="TIMESTEPS" minOccurs="0"/>
+      <element type="qes:statusType" name="exit_status" minOccurs="0" maxOccurs="1"/>
       <choice minOccurs="1">
         <element type="nonNegativeInteger" name="cputime" minOccurs="0"/>
         <element type="qes:timingType" name="timing_info" minOccurs="0"/>
       </choice>
       <element type="qes:closedType" name="closed" minOccurs="0"/>
     </sequence>
     <attribute name="Units" type="string" use="optional"/>
@@ -90,15 +93,15 @@
       <element type="qes:algorithmic_infoType" name="algorithmic_info"/>
       <element type="qes:atomic_speciesType" name="atomic_species"/>
       <element type="qes:atomic_structureType" name="atomic_structure"/>
       <element type="qes:symmetriesType" name="symmetries" minOccurs="0" maxOccurs="1"/>
       <element type="qes:basis_setType" name="basis_set"/>
       <element type="qes:dftType" name="dft"/>
       <element type="qes:outputPBCType" name="boundary_conditions" minOccurs="0"/>
-      <element type="qes:magnetizationType" name="magnetization"/>
+      <element type="qes:magnetizationType" name="magnetization" minOccurs="0"/>
       <element type="qes:total_energyType" name="total_energy"/>
       <element type="qes:band_structureType" name="band_structure"/>
       <element type="qes:matrixType" name="forces" minOccurs="0"/>
       <element type="qes:matrixType" name="stress" minOccurs="0"/>
       <element type="qes:outputElectricFieldType" name="electric_field" minOccurs="0"/>
       <element type="double" name="FCP_force" minOccurs="0"/>
       <element type="double" name="FCP_tot_charge" minOccurs="0"/>
@@ -281,20 +284,25 @@
       <pattern value="[vV][dD][wW]-[dD][fF]-[cC]09"/>
       <pattern value="[vV][dD][wW]-[dD][fF]-[oO][bB]86"/>
       <pattern value="[vV][dD][wW]-[dD][fF]-[oO][bB][kK]8"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2-[cC]09"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2-[bB]86[rR]"/>
       <pattern value="[rR][vV][vV]10"/>
+      <pattern value="[bB][eE][eE][fF]"/>
+      <pattern value="[sS][Cc][Aa][nN]"/>
+      <pattern value="[rR]2[sS][cC][aA][nN]"/>
+      <pattern value="[A-Z]{2,4}\p{Zs}{1,3}[A-Z]{1,4}\p{Zs}{1,3}[A-Z]{1,4}\p{Zs}{1,4}[A-Z]{1,4}"/>
       <pattern value=".*[xX][cC]_[lL][Dd][Aa]_[xX][cC]?_.*"/>
       <pattern value=".*[xX][cC]_[mM]?[gG][Gg][Aa]_[xX][cC]?_.*"/>
       <pattern value=".*[xX][cC]_[hH][yY][bB]_[mM]?[gG][Gg][Aa]_[xX][cC]?_.*"/>
       <pattern value=".*[xX][cC]_[lL][Dd][Aa]_[cC]_.*"/>
       <pattern value=".*[xX][cC]_[mM]?[gG][Gg][Aa]_[kKcC]_.*"/>
       <pattern value=".*[xX][cC]_[hH][yY][bB]_[mM]?[gG][Gg][Aa]_[kKcC]?_.*"/>
+      <pattern value="XC(-[0-9][0-9][0-9][iL]){6}"/>
     </restriction>
   </simpleType>
   <complexType name="hybridType">
     <sequence>
       <element type="qes:qpoint_gridType" name="qpoint_grid" minOccurs="0"/>
       <element type="double" name="ecutfock" minOccurs="0"/>
       <element type="double" name="exx_fraction" minOccurs="0"/>
@@ -335,22 +343,40 @@
     <simpleContent>
       <extension base="double">
         <attribute type="string" name="specie"/>
         <attribute type="string" name="label" use="optional"/>
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="SiteMomentType">
+    <simpleContent>
+      <extension base="double">
+        <attribute type="string" name="species"/>
+        <attribute type="integer" name="atom"/>
+        <attribute type="double" name="charge"/>
+      </extension>
+    </simpleContent>
+  </complexType>
   <complexType name="HubbardJType">
     <simpleContent>
       <extension base="qes:d3vectorType">
         <attribute type="string" name="specie"/>
         <attribute type="string" name="label"/>
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="SitMagType">
+    <simpleContent>
+      <extension base="qes:d3vectorType">
+        <attribute type="string" name="species"/>
+        <attribute type="integer" name="atom"/>
+        <attribute type="double" name="charge"/>
+      </extension>
+    </simpleContent>
+  </complexType>
   <complexType name="starting_nsType">
     <simpleContent>
       <extension base="qes:vectorType">
         <attribute type="string" name="specie"/>
         <attribute type="string" name="label"/>
         <attribute type="positiveInteger" name="spin"/>
       </extension>
@@ -455,14 +481,15 @@
     <sequence>
       <element type="boolean" name="gamma_only" minOccurs="0"/>
       <element type="double" name="ecutwfc"/>
       <element type="double" name="ecutrho" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_grid" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_smooth" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_box" minOccurs="0"/>
+      <element type="boolean" name="spline_ps" minOccurs="0" maxOccurs="1"/>
     </sequence>
   </complexType>
   <complexType name="basis_setType">
     <sequence>
       <element type="boolean" name="gamma_only" minOccurs="0"/>
       <element type="double" name="ecutwfc"/>
       <element type="double" name="ecutrho" minOccurs="0"/>
@@ -504,28 +531,33 @@
       <element type="boolean" name="tq_smoothing"/>
       <element type="boolean" name="tbeta_smoothing"/>
       <element type="double" name="diago_thr_init"/>
       <element type="boolean" name="diago_full_acc"/>
       <element type="nonNegativeInteger" name="diago_cg_maxiter" minOccurs="0"/>
       <element type="nonNegativeInteger" name="diago_ppcg_maxiter" minOccurs="0"/>
       <element type="positiveInteger" name="diago_david_ndim" minOccurs="0"/>
+      <element type="positiveInteger" name="diago_rmm_ndim" minOccurs="0" default="4"/>
+      <element type="positiveInteger" name="diago_gs_nblock" minOccurs="0" default="16"/>
+      <element type=" boolean" name="diago_rmm_conv" minOccurs="0" default="false"/>
     </sequence>
   </complexType>
   <simpleType name="mixingModeType">
     <restriction base="string">
       <enumeration value="plain"/>
       <enumeration value="TF"/>
       <enumeration value="local-TF"/>
     </restriction>
   </simpleType>
   <simpleType name="diagoType">
     <restriction base="string">
       <enumeration value="davidson"/>
       <enumeration value="cg"/>
       <enumeration value="ppcg"/>
+      <enumeration value="paro"/>
+      <enumeration value="rmm(-davidson){0,1}(-paro){01}"/>
     </restriction>
   </simpleType>
   <complexType name="k_points_IBZType">
     <choice minOccurs="1" maxOccurs="1">
       <element type="qes:monkhorst_packType" name="monkhorst_pack" minOccurs="0" maxOccurs="1"/>
       <sequence>
         <element type="positiveInteger" name="nk" minOccurs="0"/>
@@ -587,20 +619,40 @@
   </complexType>
   <complexType name="cell_controlType">
     <sequence>
       <element type="string" name="cell_dynamics"/>
       <element type="double" name="pressure" default="0.0"/>
       <element type="double" name="wmass" minOccurs="0"/>
       <element type="double" name="cell_factor" minOccurs="0"/>
-      <element type="boolean" name="fix_volume" minOccurs="0"/>
-      <element type="boolean" name="fix_area" minOccurs="0"/>
-      <element type="boolean" name="isotropic" minOccurs="0"/>
-      <element type="qes:integerMatrixType" name="free_cell" minOccurs="0"/>
+      <choice minOccurs="0" maxOccurs="1">
+        <element type="qes:celldofreeType" name="cell_do_free" minOccurs="0"/>
+        <sequence>
+          <!-- legacy deprecated choice -->
+          <element type="boolean" name="fix_volume" minOccurs="0"/>
+          <element type="boolean" name="fix_area" minOccurs="0"/>
+          <element type="boolean" name="isotropic" minOccurs="0"/>
+          <element type="qes:integerMatrixType" name="free_cell" minOccurs="0"/>
+        </sequence>
+      </choice>
     </sequence>
   </complexType>
+  <simpleType name="celldofreeType">
+    <restriction base="string">
+      <pattern value="all"/>
+      <pattern value="ibrav(\+all)"/>
+      <pattern value="(ibrav\+){0,1}[xyz]"/>
+      <pattern value="(ibrav\+){0,1}x[yz]"/>
+      <pattern value="(ibrav\+)xyz"/>
+      <pattern value="(ibrav\+){0,1}shape"/>
+      <pattern value="(ibrav\+){0,1}volume"/>
+      <pattern value="(ibrav\+){0,1}2Dxy"/>
+      <pattern value="(ibrav\+){0,1}2DShape"/>
+      <pattern value="(ibrav\+){0,1}epitaxial_[ab][bc]"/>
+    </restriction>
+  </simpleType>
   <complexType name="symmetry_flagsType">
     <sequence>
       <element type="boolean" name="nosym"/>
       <element type="boolean" name="nosym_evc"/>
       <element type="boolean" name="noinv"/>
       <element type="boolean" name="no_t_rev"/>
       <element type="boolean" name="force_symmorphic"/>
@@ -848,16 +900,23 @@
     </sequence>
   </complexType>
   <complexType name="magnetizationType">
     <sequence>
       <element type="boolean" name="lsda"/>
       <element type="boolean" name="noncolin"/>
       <element type="boolean" name="spinorbit"/>
-      <element type="double" name="total"/>
+      <choice>
+        <element type="double" name="total" minOccurs="0"/>
+        <element type="qes:d3vectorType" name="total_vec" minOccurs="0"/>
+      </choice>
       <element type="double" name="absolute"/>
+      <choice minOccurs="0" maxOccurs="1">
+        <element type="qes:scalmagsType" name="Scalar_Site_Magnetic_Moments" minOccurs="0"/>
+        <element type="qes:d3magsType" name="Site_Magnetizations" minOccurs="0"/>
+      </choice>
       <element type="boolean" name="do_magnetization" minOccurs="0"/>
     </sequence>
   </complexType>
   <complexType name="total_energyType">
     <sequence>
       <element type="double" name="etot"/>
       <element type="double" name="eband" minOccurs="0"/>
@@ -906,14 +965,109 @@
     <simpleContent>
       <extension base="string">
         <attribute type="string" name="DATE"/>
         <attribute type="string" name="TIME"/>
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="cpstatusType">
+    <sequence>
+      <element type="qes:cpnumstepType" name="STEP" minOccurs="1" maxOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="TIME" minOccurs="1" maxOccurs="1"/>
+      <element type="string" name="TITLE" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="KINETIC_ENERGY" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="HARTREE_ENERGY" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="EWALD_TERM" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="GAUSS_SELFINT" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="LPSP_ENERGY" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="NLPSP_ENERGY" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="EXC_ENERGY" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="AVERAGE_POT" minOccurs="1"/>
+      <element type="qes:scalarQuantityType" name="ENTHALPY" minOccurs="1"/>
+    </sequence>
+  </complexType>
+  <complexType name="cpnumstepType">
+    <simpleContent>
+      <extension base="qes:emptyType">
+        <attribute name="ITERATION" type="integer"/>
+      </extension>
+    </simpleContent>
+  </complexType>
+  <simpleType name="emptyType">
+    <restriction base="string">
+      <enumeration value=""/>
+      <enumeration value="iteration number"/>
+    </restriction>
+  </simpleType>
+  <complexType name="cptimestepsType">
+    <sequence>
+      <element name="STEP0" type="qes:cpstepType" minOccurs="1"/>
+      <element name="STEPM" type="qes:cpstepType" minOccurs="1"/>
+    </sequence>
+    <attribute name="nt" type="integer"/>
+  </complexType>
+  <complexType name="cpstepType">
+    <sequence>
+      <element name="ACCUMULATORS" type="qes:doubleListType" minOccurs="0"/>
+      <element name="IONS_POSITIONS" type="qes:cp_ionPosType" minOccurs="1"/>
+      <element name="IONS_NOSE" type="qes:cp_ionsNoseType" minOccurs="1"/>
+      <element name="ekincm" type="double" minOccurs="0"/>
+      <element name="ELECTRONS_NOSE" type="qes:cp_elecNoseType" minOccurs="1"/>
+      <element name="CELL_PARAMETERS" type="qes:cp_cellType" minOccurs="1"/>
+      <element name="CELL_NOSE" type="qes:cp_cellNoseType" minOccurs="1"/>
+    </sequence>
+  </complexType>
+  <complexType name="cp_ionPosType">
+    <sequence>
+      <element name="stau" type="qes:doubleListType" minOccurs="1"/>
+      <element name="svel" type="qes:doubleListType" minOccurs="1"/>
+      <element name="taui" type="qes:doubleListType" minOccurs="0"/>
+      <element name="cdmi" type="qes:d3vectorType" minOccurs="0"/>
+      <element name="force" type="qes:doubleListType" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="cp_ionsNoseType">
+    <sequence>
+      <element type="integer" name="nhpcl" minOccurs="1"/>
+      <element type="integer" name="nhpdim" minOccurs="1"/>
+      <element type="double" name="xnhp" minOccurs="1"/>
+      <element type="double" name="vnhp" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="cp_elecNoseType">
+    <sequence>
+      <element name="xnhe" type="double" minOccurs="1"/>
+      <element name="vnhe" type="double" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="cp_cellType">
+    <sequence>
+      <element name="ht" type="qes:doubleListType" minOccurs="1"/>
+      <element name="htvel" type="qes:doubleListType" minOccurs="0"/>
+      <element name="gvel" type="qes:doubleListType" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="cp_cellNoseType">
+    <sequence>
+      <element type="qes:doubleListType" name="xnhh" minOccurs="1"/>
+      <element type="qes:doubleListType" name="vnhh" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="scalmagsType">
+    <sequence>
+      <element type="qes:SiteMomentType" name="SiteMagnetization" minOccurs="1" maxOccurs="unbounded"/>
+    </sequence>
+    <attribute name="nat" type="integer"/>
+  </complexType>
+  <complexType name="d3magsType">
+    <sequence>
+      <element type="qes:SitMagType" name="SiteMagnetization" minOccurs="1" maxOccurs="unbounded"/>
+    </sequence>
+    <attribute type="integer" name="nat"/>
+  </complexType>
   <simpleType name="statusType">
     <restriction base="integer">
       <enumeration value="-1"/>
       <enumeration value="0"/>
       <enumeration value="1"/>
       <enumeration value="2"/>
       <enumeration value="3"/>
@@ -965,17 +1119,17 @@
         <attribute name="size" type="integer" use="required"/>
       </extension>
     </simpleContent>
   </complexType>
   <complexType name="matrixType">
     <simpleContent>
       <extension base="qes:doubleListType">
-        <attribute name="rank" type="positiveInteger"/>
-        <attribute name="dims" type="qes:integerListType"/>
-        <attribute name="order">
+        <attribute name="rank" type="positiveInteger" use="required"/>
+        <attribute name="dims" type="qes:integerListType" use="required"/>
+        <attribute name="order" use="optional">
           <simpleType>
             <restriction base="string">
               <enumeration value="F"/>
               <enumeration value="C"/>
             </restriction>
           </simpleType>
         </attribute>
@@ -998,11 +1152,12 @@
       </extension>
     </simpleContent>
   </complexType>
   <complexType name="scalarQuantityType">
     <simpleContent>
       <extension base="double">
         <attribute type="string" name="Units"/>
+        <attribute type="string" name="UNITS"/>
       </extension>
     </simpleContent>
   </complexType>
 </schema>
```

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_211101.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_test_240411.xsd`

 * *Files 24% similar despite different names*

#### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_211101.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_test_240411.xsd`

```diff
@@ -1,17 +1,17 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!--
-Copyright (c), 2015-2016, Quantum Espresso Foundation. All rights reserved.
+Copyright (c), 2021-2024, Quantum Espresso Foundation. All rights reserved.
 This file is distributed under the terms of the MIT License. See the
 file 'LICENSE' in the root directory of the present distribution, or
 http://opensource.org/licenses/MIT.
 Authors: Antonio Zambon, Paolo Giannozzi, Pietro Delugas
-datecode 211101
+datecode 240408
 -->
-<schema xmlns="http://www.w3.org/2001/XMLSchema" xmlns:qes="http://www.quantum-espresso.org/ns/qes/qes-1.0" targetNamespace="http://www.quantum-espresso.org/ns/qes/qes-1.0">
+<schema xmlns="http://www.w3.org/2001/XMLSchema" xmlns:qes="http://www.quantum-espresso.org/ns/qes/qes-1.0" targetNamespace="http://www.quantum-espresso.org/ns/qes/qes-1.0" version="240408">
   <!-- ESPRESSO (root element) -->
   <element name="espresso" type="qes:espressoType"/>
   <complexType name="espressoType">
     <sequence>
       <element type="qes:general_infoType" name="general_info" minOccurs="0"/>
       <element type="qes:parallel_infoType" name="parallel_info" minOccurs="0"/>
       <element type="qes:inputType" name="input" minOccurs="0"/>
@@ -60,33 +60,37 @@
       <element type="qes:basisType" name="basis"/>
       <element type="qes:electron_controlType" name="electron_control"/>
       <element type="qes:k_points_IBZType" name="k_points_IBZ"/>
       <element type="qes:ion_controlType" name="ion_control"/>
       <element type="qes:cell_controlType" name="cell_control"/>
       <element type="qes:symmetry_flagsType" name="symmetry_flags" minOccurs="0"/>
       <element type="qes:boundary_conditionsType" name="boundary_conditions" minOccurs="0"/>
+      <element type="qes:fcpType" name="fcp_settings" minOccurs="0"/>
+      <element type="qes:rismType" name="rism_settings" minOccurs="0"/>
+      <element type="qes:solventsType" name="solvents" minOccurs="0" maxOccurs="1"/>
       <element type="qes:ekin_functionalType" name="ekin_functional" minOccurs="0"/>
       <element type="qes:matrixType" name="external_atomic_forces" minOccurs="0"/>
       <element type="qes:integerMatrixType" name="free_positions" minOccurs="0"/>
       <element type="qes:matrixType" name="starting_atomic_velocities" minOccurs="0"/>
       <element type="qes:electric_fieldType" name="electric_field" minOccurs="0"/>
       <element type="qes:atomic_constraintsType" name="atomic_constraints" minOccurs="0"/>
       <element type="qes:spin_constraintsType" name="spin_constraints" minOccurs="0"/>
+      <element type="qes:two_chemType" name="twoch_" minOccurs="0"/>
     </sequence>
   </complexType>
   <!-- STEP TYPE -->
   <complexType name="stepType">
     <sequence>
       <element type="qes:scf_convType" name="scf_conv"/>
       <element type="qes:atomic_structureType" name="atomic_structure"/>
       <element type="qes:total_energyType" name="total_energy"/>
       <element type="qes:matrixType" name="forces"/>
       <element type="qes:matrixType" name="stress" minOccurs="0"/>
-      <element type="double" name="FCP_force" minOccurs="0"/>
-      <element type="double" name="FCP_tot_charge" minOccurs="0"/>
+      <element type="double" name="fcp_force" minOccurs="0"/>
+      <element type="double" name="fcp_tot_charge" minOccurs="0"/>
     </sequence>
     <attribute type="positiveInteger" name="n_step"/>
   </complexType>
   <!-- OUTPUT TYPE -->
   <complexType name="outputType">
     <sequence>
       <element type="qes:convergence_infoType" name="convergence_info" minOccurs="0"/>
@@ -99,16 +103,18 @@
       <element type="qes:outputPBCType" name="boundary_conditions" minOccurs="0"/>
       <element type="qes:magnetizationType" name="magnetization" minOccurs="0"/>
       <element type="qes:total_energyType" name="total_energy"/>
       <element type="qes:band_structureType" name="band_structure"/>
       <element type="qes:matrixType" name="forces" minOccurs="0"/>
       <element type="qes:matrixType" name="stress" minOccurs="0"/>
       <element type="qes:outputElectricFieldType" name="electric_field" minOccurs="0"/>
-      <element type="double" name="FCP_force" minOccurs="0"/>
-      <element type="double" name="FCP_tot_charge" minOccurs="0"/>
+      <element type="double" name="fcp_force" minOccurs="0"/>
+      <element type="double" name="fcp_tot_charge" minOccurs="0"/>
+      <element type="qes:rism3dType" name="rism3d" minOccurs="0"/>
+      <element type="qes:rismlaueType" name="rismlaue" minOccurs="0"/>
     </sequence>
   </complexType>
   <!-- Timing Info -->
   <complexType name="timingType">
     <sequence>
       <element type="qes:clockType" name="total" minOccurs="1" maxOccurs="1"/>
       <element type="qes:clockType" name="partial" minOccurs="0" maxOccurs="unbounded"/>
@@ -138,14 +144,16 @@
       <element type="positiveInteger" name="max_seconds"/>
       <element type="positiveInteger" name="nstep" minOccurs="0"/>
       <element type="double" name="etot_conv_thr" default="1.0e-5"/>
       <element type="double" name="forc_conv_thr" default="1.0e-3"/>
       <element type="double" name="press_conv_thr" default="5e-1"/>
       <element type="qes:lowhighType" name="verbosity" default="low"/>
       <element type="positiveInteger" name="print_every"/>
+      <element type="boolean" name="fcp"/>
+      <element type="boolean" name="rism"/>
     </sequence>
   </complexType>
   <!-- COMMON TYPES -->
   <!-- GENERAL INFO -->
   <complexType name="xml_formatType">
     <simpleContent>
       <extension base="string">
@@ -188,14 +196,19 @@
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
       <enumeration value="high"/>
+      <enumeration value="medium"/>
+      <enumeration value="minimum"/>
+      <enumeration value="debug"/>
+      <enumeration value="none"/>
+      <enumeration value="nowf"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
@@ -218,14 +231,15 @@
         <element type="qes:atomic_positionsType" name="atomic_positions" minOccurs="0"/>
         <element type="qes:wyckoff_positionsType" name="wyckoff_positions" minOccurs="0"/>
         <element type="qes:atomic_positionsType" name="crystal_positions" minOccurs="0"/>
       </choice>
       <element type="qes:cellType" name="cell"/>
     </sequence>
     <attribute type="positiveInteger" name="nat"/>
+    <attribute type="integer" name="num_of_atomic_wfc" use="optional"/>
     <attribute type="double" name="alat" use="optional"/>
     <attribute type="positiveInteger" name="bravais_index" use="optional"/>
     <attribute type="string" name="alternative_axes" use="optional"/>
   </complexType>
   <complexType name="atomic_positionsType">
     <sequence>
       <element type="qes:atomType" name="atom" maxOccurs="unbounded"/>
@@ -284,14 +298,15 @@
       <pattern value="[vV][dD][wW]-[dD][fF]-[cC]09"/>
       <pattern value="[vV][dD][wW]-[dD][fF]-[oO][bB]86"/>
       <pattern value="[vV][dD][wW]-[dD][fF]-[oO][bB][kK]8"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2-[cC]09"/>
       <pattern value="[vV][dD][wW]-[dD][fF]2-[bB]86[rR]"/>
       <pattern value="[rR][vV][vV]10"/>
+      <pattern value="[rR][sS][cC][aA][nN]"/>
       <pattern value="[bB][eE][eE][fF]"/>
       <pattern value="[sS][Cc][Aa][nN]"/>
       <pattern value="[rR]2[sS][cC][aA][nN]"/>
       <pattern value="[A-Z]{2,4}\p{Zs}{1,3}[A-Z]{1,4}\p{Zs}{1,3}[A-Z]{1,4}\p{Zs}{1,4}[A-Z]{1,4}"/>
       <pattern value=".*[xX][cC]_[lL][Dd][Aa]_[xX][cC]?_.*"/>
       <pattern value=".*[xX][cC]_[mM]?[gG][Gg][Aa]_[xX][cC]?_.*"/>
       <pattern value=".*[xX][cC]_[hH][yY][bB]_[mM]?[gG][Gg][Aa]_[xX][cC]?_.*"/>
@@ -321,36 +336,50 @@
         <attribute type="positiveInteger" name="nqx3"/>
       </extension>
     </simpleContent>
   </complexType>
   <complexType name="dftUType">
     <sequence>
       <element type="unsignedByte" name="lda_plus_u_kind" minOccurs="0"/>
+      <element type="qes:HubbardOccType" name="Hubbard_Occ" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardCommonType" name="Hubbard_U" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardCommonType" name="Hubbard_J0" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardCommonType" name="Hubbard_alpha" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardCommonType" name="Hubbard_beta" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardJType" name="Hubbard_J" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:starting_nsType" name="starting_ns" minOccurs="0" maxOccurs="unbounded"/>
+      <element type="qes:HubbardInterSpecieVType" name="Hubbard_V" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:Hubbard_nsType" name="Hubbard_ns" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardProjType" name="U_projection_type" minOccurs="0"/>
       <element type="qes:HubbardBackType" name="Hubbard_back" minOccurs="0" maxOccurs="unbounded"/>
-      <element type="qes:HubbardCommonType" name="Hubbard_U_back" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:HubbardCommonType" name="Hubbard_alpha_back" minOccurs="0" maxOccurs="unbounded"/>
       <element type="qes:Hubbard_nsType" name="Hubbard_ns_nc" minOccurs="0" maxOccurs="unbounded"/>
     </sequence>
+    <attribute type="boolean" name="new_format"/>
   </complexType>
   <complexType name="HubbardCommonType">
     <simpleContent>
       <extension base="double">
         <attribute type="string" name="specie"/>
         <attribute type="string" name="label" use="optional"/>
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="HubbardInterSpecieVType">
+    <simpleContent>
+      <extension base="double">
+        <attribute type="string" name="specie1" use="required"/>
+        <attribute type="integer" name="index1" use="required"/>
+        <attribute type="string" name="label1"/>
+        <attribute type="string" name="specie2" use="required"/>
+        <attribute type="integer" name="index2" use="required"/>
+        <attribute type="string" name="label2"/>
+      </extension>
+    </simpleContent>
+  </complexType>
   <complexType name="SiteMomentType">
     <simpleContent>
       <extension base="double">
         <attribute type="string" name="species"/>
         <attribute type="integer" name="atom"/>
         <attribute type="double" name="charge"/>
       </extension>
@@ -360,14 +389,28 @@
     <simpleContent>
       <extension base="qes:d3vectorType">
         <attribute type="string" name="specie"/>
         <attribute type="string" name="label"/>
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="ChannelOccType">
+    <simpleContent>
+      <extension base="qes:HubbardCommonType">
+        <attribute type="integer" name="index" use="required"/>
+      </extension>
+    </simpleContent>
+  </complexType>
+  <complexType name="HubbardOccType">
+    <sequence>
+      <element type="qes:ChannelOccType" name="channel_occ" minOccurs="1" maxOccurs="3"/>
+    </sequence>
+    <attribute type="positiveInteger" name="channels" use="required"/>
+    <attribute type="string" name="specie" use="required"/>
+  </complexType>
   <complexType name="SitMagType">
     <simpleContent>
       <extension base="qes:d3vectorType">
         <attribute type="string" name="species"/>
         <attribute type="integer" name="atom"/>
         <attribute type="double" name="charge"/>
       </extension>
@@ -395,36 +438,36 @@
   <simpleType name="HubbardProjType">
     <restriction base="string">
       <enumeration value="atomic"/>
       <enumeration value="ortho-atomic"/>
       <enumeration value="norm-atomic"/>
       <enumeration value="pseudo"/>
       <enumeration value="file"/>
+      <enumeration value="wf"/>
+      <enumeration value="wannier"/>
     </restriction>
   </simpleType>
   <complexType name="HubbardBackType">
     <sequence>
-      <element type="qes:backrestrType" name="background" minOccurs="1" maxOccurs="1"/>
-      <element type="qes:backLType" name="l_number" minOccurs="1" maxOccurs="unbounded"/>
+      <element type="double" name="Hubbard_U2" minOccurs="1" maxOccurs="1"/>
+      <element type="positiveInteger" name="n2_number" minOccurs="1" maxOccurs="1"/>
+      <element type="positiveInteger" name="l2_number" minOccurs="1" maxOccurs="1"/>
+      <element type="positiveInteger" name="n3_number" minOccurs="0" maxOccurs="1"/>
+      <element type="positiveInteger" name="l3_number" minOccurs="0" maxOccurs="1"/>
     </sequence>
+    <attribute type="qes:backrestrType" name="background" use="required"/>
+    <attribute type="string" name="label"/>
     <attribute type="string" name="species"/>
   </complexType>
   <simpleType name="backrestrType">
     <restriction base="string">
       <enumeration value="two_orbitals"/>
       <enumeration value="one_orbital"/>
     </restriction>
   </simpleType>
-  <complexType name="backLType">
-    <simpleContent>
-      <extension base="nonNegativeInteger">
-        <attribute name="l_index" type="nonNegativeInteger"/>
-      </extension>
-    </simpleContent>
-  </complexType>
   <complexType name="vdWType">
     <sequence>
       <element type="string" name="vdw_corr" minOccurs="0"/>
       <element type="integer" name="dftd3_version" minOccurs="0"/>
       <element type="boolean" name="dftd3_threebody" minOccurs="0"/>
       <element type="string" name="non_local_term" minOccurs="0"/>
       <element type="string" name="functional" minOccurs="0"/>
@@ -481,15 +524,14 @@
     <sequence>
       <element type="boolean" name="gamma_only" minOccurs="0"/>
       <element type="double" name="ecutwfc"/>
       <element type="double" name="ecutrho" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_grid" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_smooth" minOccurs="0"/>
       <element type="qes:basisSetItemType" name="fft_box" minOccurs="0"/>
-      <element type="boolean" name="spline_ps" minOccurs="0" maxOccurs="1"/>
     </sequence>
   </complexType>
   <complexType name="basis_setType">
     <sequence>
       <element type="boolean" name="gamma_only" minOccurs="0"/>
       <element type="double" name="ecutwfc"/>
       <element type="double" name="ecutrho" minOccurs="0"/>
@@ -522,42 +564,125 @@
     <sequence>
       <element type="qes:diagoType" name="diagonalization"/>
       <element type="qes:mixingModeType" name="mixing_mode"/>
       <element type="double" name="mixing_beta"/>
       <element type="double" name="conv_thr"/>
       <element type="positiveInteger" name="mixing_ndim"/>
       <element type="positiveInteger" name="max_nstep"/>
+      <element type="positiveInteger" name="exx_nstep" minOccurs="0"/>
       <element type="boolean" name="real_space_q" minOccurs="0" default="false"/>
       <element type="boolean" name="real_space_beta" minOccurs="0" default="false"/>
       <element type="boolean" name="tq_smoothing"/>
       <element type="boolean" name="tbeta_smoothing"/>
       <element type="double" name="diago_thr_init"/>
       <element type="boolean" name="diago_full_acc"/>
       <element type="nonNegativeInteger" name="diago_cg_maxiter" minOccurs="0"/>
       <element type="nonNegativeInteger" name="diago_ppcg_maxiter" minOccurs="0"/>
       <element type="positiveInteger" name="diago_david_ndim" minOccurs="0"/>
       <element type="positiveInteger" name="diago_rmm_ndim" minOccurs="0" default="4"/>
       <element type="positiveInteger" name="diago_gs_nblock" minOccurs="0" default="16"/>
       <element type=" boolean" name="diago_rmm_conv" minOccurs="0" default="false"/>
     </sequence>
   </complexType>
+  <complexType name="fcpType">
+    <sequence>
+      <element type="double" name="fcp_mu" minOccurs="0"/>
+      <element type="string" name="fcp_dynamics" minOccurs="0"/>
+      <element type="double" name="fcp_conv_thr" minOccurs="0"/>
+      <element type="integer" name="fcp_ndiis" minOccurs="0"/>
+      <element type="double" name="fcp_rdiis" minOccurs="0"/>
+      <element type="double" name="fcp_mass" minOccurs="0"/>
+      <element type="double" name="fcp_velocity" minOccurs="0"/>
+      <element type="string" name="fcp_temperature" minOccurs="0"/>
+      <element type="double" name="fcp_tempw" minOccurs="0"/>
+      <element type="double" name="fcp_tolp" minOccurs="0"/>
+      <element type="double" name="fcp_delta_t" minOccurs="0"/>
+      <element type="integer" name="fcp_nraise" minOccurs="0"/>
+      <element type="boolean" name="freeze_all_atoms" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="rismType">
+    <sequence>
+      <element type="integer" name="nsolv" minOccurs="1"/>
+      <element type="qes:soluteType" name="solute" minOccurs="1" maxOccurs="unbounded"/>
+      <element type="string" name="closure" minOccurs="0"/>
+      <element type="double" name="tempv" minOccurs="0"/>
+      <element type="double" name="ecutsolv" minOccurs="0"/>
+      <element type="double" name="rmax_lj" minOccurs="0"/>
+      <element type="double" name="rmax1d" minOccurs="0"/>
+      <element type="string" name="starting1d" minOccurs="0"/>
+      <element type="string" name="starting3d" minOccurs="0"/>
+      <element type="double" name="smear1d" minOccurs="0"/>
+      <element type="double" name="smear3d" minOccurs="0"/>
+      <element type="integer" name="rism1d_maxstep" minOccurs="0"/>
+      <element type="integer" name="rism3d_maxstep" minOccurs="0"/>
+      <element type="double" name="rism1d_conv_thr" minOccurs="0"/>
+      <element type="double" name="rism3d_conv_thr" minOccurs="0"/>
+      <element type="integer" name="mdiis1d_size" minOccurs="0"/>
+      <element type="integer" name="mdiis3d_size" minOccurs="0"/>
+      <element type="double" name="mdiis1d_step" minOccurs="0"/>
+      <element type="double" name="mdiis3d_step" minOccurs="0"/>
+      <element type="double" name="rism1d_bond_width" minOccurs="0"/>
+      <element type="double" name="rism1d_dielectric" minOccurs="0"/>
+      <element type="double" name="rism1d_molesize" minOccurs="0"/>
+      <element type="integer" name="rism1d_nproc" minOccurs="0"/>
+      <element type="integer" name="rism1d_nproc_switch" minOccurs="0"/>
+      <element type="double" name="rism3d_conv_level" minOccurs="0"/>
+      <element type="boolean" name="rism3d_planar_average" minOccurs="0"/>
+      <element type="integer" name="laue_nfit" minOccurs="0"/>
+      <element type="double" name="laue_expand_right" minOccurs="0"/>
+      <element type="double" name="laue_expand_left" minOccurs="0"/>
+      <element type="double" name="laue_starting_right" minOccurs="0"/>
+      <element type="double" name="laue_starting_left" minOccurs="0"/>
+      <element type="double" name="laue_buffer_right" minOccurs="0"/>
+      <element type="double" name="laue_buffer_right_solu" minOccurs="0"/>
+      <element type="double" name="laue_buffer_right_solv" minOccurs="0"/>
+      <element type="double" name="laue_buffer_left" minOccurs="0"/>
+      <element type="double" name="laue_buffer_left_solu" minOccurs="0"/>
+      <element type="double" name="laue_buffer_left_solv" minOccurs="0"/>
+      <element type="boolean" name="laue_both_hands" minOccurs="0"/>
+      <element type="string" name="laue_reference" minOccurs="0"/>
+      <element type="string" name="laue_wall" minOccurs="0"/>
+      <element type="double" name="laue_wall_z" minOccurs="0"/>
+      <element type="double" name="laue_wall_rho" minOccurs="0"/>
+      <element type="double" name="laue_wall_epsilon" minOccurs="0"/>
+      <element type="double" name="laue_wall_sigma" minOccurs="0"/>
+      <element type="boolean" name="laue_wall_lj6" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="soluteType">
+    <sequence>
+      <element type="string" name="solute_lj" minOccurs="1"/>
+      <element type="double" name="epsilon" minOccurs="1"/>
+      <element type="double" name="sigma" minOccurs="1"/>
+    </sequence>
+  </complexType>
+  <complexType name="solventType">
+    <sequence>
+      <element type="string" name="label" minOccurs="1"/>
+      <element type="string" name="molec_file" minOccurs="1"/>
+      <element type="double" name="density1" minOccurs="1"/>
+      <element type="double" name="density2" minOccurs="0"/>
+      <element type="string" name="unit" minOccurs="0"/>
+    </sequence>
+  </complexType>
   <simpleType name="mixingModeType">
     <restriction base="string">
       <enumeration value="plain"/>
       <enumeration value="TF"/>
       <enumeration value="local-TF"/>
     </restriction>
   </simpleType>
   <simpleType name="diagoType">
     <restriction base="string">
-      <enumeration value="davidson"/>
-      <enumeration value="cg"/>
-      <enumeration value="ppcg"/>
-      <enumeration value="paro"/>
-      <enumeration value="rmm(-davidson){0,1}(-paro){01}"/>
+      <pattern value="davidson"/>
+      <pattern value="cg"/>
+      <pattern value="ppcg"/>
+      <pattern value="paro"/>
+      <pattern value="\s*rmm(-davidson|-paro)\s*"/>
     </restriction>
   </simpleType>
   <complexType name="k_points_IBZType">
     <choice minOccurs="1" maxOccurs="1">
       <element type="qes:monkhorst_packType" name="monkhorst_pack" minOccurs="0" maxOccurs="1"/>
       <sequence>
         <element type="positiveInteger" name="nk" minOccurs="0"/>
@@ -633,24 +758,24 @@
           <element type="qes:integerMatrixType" name="free_cell" minOccurs="0"/>
         </sequence>
       </choice>
     </sequence>
   </complexType>
   <simpleType name="celldofreeType">
     <restriction base="string">
-      <pattern value="all"/>
-      <pattern value="ibrav(\+all)"/>
-      <pattern value="(ibrav\+){0,1}[xyz]"/>
-      <pattern value="(ibrav\+){0,1}x[yz]"/>
-      <pattern value="(ibrav\+)xyz"/>
-      <pattern value="(ibrav\+){0,1}shape"/>
-      <pattern value="(ibrav\+){0,1}volume"/>
-      <pattern value="(ibrav\+){0,1}2Dxy"/>
-      <pattern value="(ibrav\+){0,1}2DShape"/>
-      <pattern value="(ibrav\+){0,1}epitaxial_[ab][bc]"/>
+      <pattern value="\s*all\s*"/>
+      <pattern value="\s*ibrav(\+all)\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}[xyz]\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}x[yz]\s*"/>
+      <pattern value="\s*(ibrav\+)xyz\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}shape\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}volume\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}2Dxy\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}2DShape\s*"/>
+      <pattern value="\s*(ibrav\+){0,1}epitaxial_[ab][bc]\s*"/>
     </restriction>
   </simpleType>
   <complexType name="symmetry_flagsType">
     <sequence>
       <element type="boolean" name="nosym"/>
       <element type="boolean" name="nosym_evc"/>
       <element type="boolean" name="noinv"/>
@@ -659,24 +784,42 @@
       <element type="boolean" name="use_all_frac"/>
     </sequence>
   </complexType>
   <complexType name="boundary_conditionsType">
     <sequence>
       <element type="string" name="assume_isolated"/>
       <element type="qes:esmType" name="esm" minOccurs="0"/>
-      <element type="boolean" name="fcp_opt" minOccurs="0"/>
-      <element type="double" name="fcp_mu" minOccurs="0"/>
+      <element type="qes:gcscfType" name="gcscf" minOccurs="0"/>
     </sequence>
   </complexType>
   <complexType name="esmType">
     <sequence>
       <element type="string" name="bc"/>
-      <element type="positiveInteger" name="nfit"/>
-      <element type="double" name="w"/>
-      <element type="double" name="efield"/>
+      <element type="positiveInteger" name="nfit" minOccurs="0"/>
+      <element type="double" name="w" minOccurs="0"/>
+      <element type="double" name="efield" minOccurs="0"/>
+      <element type="double" name="a" minOccurs="0"/>
+      <element type="double" name="zb" minOccurs="0"/>
+      <element type="boolean" name="debug" minOccurs="0"/>
+      <element type="integer" name="debug_gpmax" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="gcscfType">
+    <sequence>
+      <element type="boolean" name="ignore_mun" minOccurs="0"/>
+      <element type="double" name="mu" minOccurs="0"/>
+      <element type="double" name="conv_thr" minOccurs="0"/>
+      <element type="double" name="gk" minOccurs="0"/>
+      <element type="double" name="gh" minOccurs="0"/>
+      <element type="double" name="beta" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="solventsType">
+    <sequence>
+      <element type="qes:solventType" name="solvent" minOccurs="1" maxOccurs="unbounded"/>
     </sequence>
   </complexType>
   <complexType name="ekin_functionalType">
     <sequence>
       <element type="double" name="ecfixed"/>
       <element type="double" name="qcutz"/>
       <element type="double" name="q2sigma"/>
@@ -729,33 +872,35 @@
       <element type="qes:atomic_constraintType" name="atomic_constraint" minOccurs="1" maxOccurs="unbounded"/>
     </sequence>
   </complexType>
   <complexType name="atomic_constraintType">
     <sequence>
       <element type="qes:constr_parms_listType" name="constr_parms"/>
       <element type="qes:constr_typeType" name="constr_type"/>
-      <element type="double" name="constr_target"/>
+      <element type="double" name="constr_target" minOccurs="0"/>
     </sequence>
   </complexType>
   <simpleType name="constr_parms_listType">
     <restriction>
       <simpleType>
         <list itemType="double"/>
       </simpleType>
-      <length value="4"/>
+      <minLength value="2"/>
+      <maxLength value="4"/>
     </restriction>
   </simpleType>
   <simpleType name="constr_typeType">
     <restriction base="string">
       <enumeration value="type_coord"/>
       <enumeration value="atom_coord"/>
       <enumeration value="distance"/>
       <enumeration value="planar_angle"/>
       <enumeration value="torsional_angle"/>
       <enumeration value="bennet_proj"/>
+      <enumeration value="potential_wall"/>
     </restriction>
   </simpleType>
   <complexType name="inputOccupationsType">
     <simpleContent>
       <extension base="qes:vectorType">
         <attribute type="positiveInteger" name="ispin"/>
         <attribute type="double" name="spin_factor"/>
@@ -834,14 +979,16 @@
       <element name="gatefieldEnergy" type="double" minOccurs="1" maxOccurs="1"/>
     </sequence>
   </complexType>
   <complexType name="convergence_infoType">
     <sequence>
       <element type="qes:scf_convType" name="scf_conv"/>
       <element type="qes:opt_convType" name="opt_conv" minOccurs="0"/>
+      <!-- element optional for back-compatibility but always present-->
+      <element type="boolean" name="wf_collected" minOccurs="0"/>
     </sequence>
   </complexType>
   <complexType name="scf_convType">
     <sequence>
       <element type="boolean" name="convergence_achieved"/>
       <element type="positiveInteger" name="n_scf_steps"/>
       <element type="double" name="scf_error"/>
@@ -893,14 +1040,15 @@
         <attribute type="boolean" name="time_reversal" use="optional"/>
       </extension>
     </simpleContent>
   </complexType>
   <complexType name="outputPBCType">
     <sequence>
       <element type="string" name="assume_isolated"/>
+      <element type="qes:esmType" name="esm" minOccurs="0"/>
     </sequence>
   </complexType>
   <complexType name="magnetizationType">
     <sequence>
       <element type="boolean" name="lsda"/>
       <element type="boolean" name="noncolin"/>
       <element type="boolean" name="spinorbit"/>
@@ -925,30 +1073,36 @@
       <element type="double" name="etxc" minOccurs="0"/>
       <element type="double" name="ewald" minOccurs="0"/>
       <element type="double" name="demet" minOccurs="0"/>
       <element type="double" name="efieldcorr" minOccurs="0"/>
       <element type="double" name="potentiostat_contr" minOccurs="0"/>
       <element type="double" name="gatefield_contr" minOccurs="0"/>
       <element type="double" name="vdW_term" minOccurs="0"/>
+      <element type="double" name="esol" minOccurs="0"/>
+      <element type="double" name="levelshift_contr" minOccurs="0"/>
     </sequence>
   </complexType>
   <complexType name="band_structureType">
     <sequence>
       <element type="boolean" name="lsda"/>
       <element type="boolean" name="noncolin"/>
       <element type="boolean" name="spinorbit"/>
       <element type="positiveInteger" name="nbnd" minOccurs="0"/>
       <element type="nonNegativeInteger" name="nbnd_up" minOccurs="0"/>
       <element type="nonNegativeInteger" name="nbnd_dw" minOccurs="0"/>
       <element type="double" name="nelec"/>
+      <!-- wf_collected and num_of_atomic_wfc are kept as optional for back-compatibility but never more used, 
+        they are removed from the fortran type to work around a bug of Intel <21.0.3 
+        comment the 2 lines below before building the qes_modules-->
       <element type="integer" name="num_of_atomic_wfc" minOccurs="0"/>
-      <element type="boolean" name="wf_collected"/>
+      <element type="boolean" name="wf_collected" minOccurs="0"/>
       <element type="double" name="fermi_energy" minOccurs="0"/>
       <element type="double" name="highestOccupiedLevel" minOccurs="0"/>
       <element type="double" name="lowestUnoccupiedLevel" minOccurs="0"/>
+      <element type="qes:two_chemType" name="twochem" minOccurs="0"/>
       <element name="two_fermi_energies" type="qes:d2vectorType" minOccurs="0"/>
       <element type="qes:k_points_IBZType" name="starting_k_points"/>
       <element type="positiveInteger" name="nks"/>
       <element type="qes:occupationsType" name="occupations_kind"/>
       <element type="qes:smearingType" name="smearing" minOccurs="0"/>
       <element type="qes:ks_energiesType" name="ks_energies" maxOccurs="unbounded"/>
     </sequence>
@@ -1152,12 +1306,46 @@
       </extension>
     </simpleContent>
   </complexType>
   <complexType name="scalarQuantityType">
     <simpleContent>
       <extension base="double">
         <attribute type="string" name="Units"/>
-        <attribute type="string" name="UNITS"/>
+        <!--attribute type="string" name="UNITS"/-->
       </extension>
     </simpleContent>
   </complexType>
+  <complexType name="rism3dType">
+    <sequence>
+      <element type="integer" name="nmol" minOccurs="1"/>
+      <element type="string" name="molec_dir" minOccurs="0"/>
+      <element type="qes:solventType" name="solvent" minOccurs="1" maxOccurs="unbounded"/>
+      <element type="double" name="ecutsolv" minOccurs="1"/>
+    </sequence>
+  </complexType>
+  <complexType name="rismlaueType">
+    <sequence>
+      <element type="boolean" name="both_hands" minOccurs="0"/>
+      <element type="integer" name="nfit" minOccurs="0"/>
+      <element type="integer" name="pot_ref" minOccurs="0"/>
+      <element type="double" name="charge" minOccurs="0"/>
+      <element type="double" name="right_start" minOccurs="0"/>
+      <element type="double" name="right_expand" minOccurs="0"/>
+      <element type="double" name="right_buffer" minOccurs="0"/>
+      <element type="double" name="right_buffer_u" minOccurs="0"/>
+      <element type="double" name="right_buffer_v" minOccurs="0"/>
+      <element type="double" name="left_start" minOccurs="0"/>
+      <element type="double" name="left_expand" minOccurs="0"/>
+      <element type="double" name="left_buffer" minOccurs="0"/>
+      <element type="double" name="left_buffer_u" minOccurs="0"/>
+      <element type="double" name="left_buffer_v" minOccurs="0"/>
+    </sequence>
+  </complexType>
+  <complexType name="two_chemType">
+    <sequence>
+      <element type="boolean" name="twochem" default="true" minOccurs="1"/>
+      <element type="integer" name="nbnd_cond" minOccurs="1"/>
+      <element type="double" name="degauss_cond" minOccurs="1"/>
+      <element type="integer" name="nelec_cond" minOccurs="1"/>
+    </sequence>
+  </complexType>
 </schema>
```

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_230310.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_230310.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_neb-20180511.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_neb-20180511.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_neb-211101.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_neb-211101.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_spectrum-20180511.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_spectrum-20180511.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/qes_spectrum-20180517.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/qes_spectrum-20180517.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/tddfpt-20180511.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/tddfpt-20180511.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/releases/tddfpt-20180517.xsd` & `qeschema-1.5.2/qeschema/schemas/releases/tddfpt-20180517.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/tddfpt.xsd` & `qeschema-1.5.2/qeschema/schemas/tddfpt.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/schemas/xspectra.xsd` & `qeschema-1.5.2/qeschema/schemas/xspectra.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/upf.py` & `qeschema-1.5.2/qeschema/upf.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/qeschema/utils.py` & `qeschema-1.5.2/qeschema/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,14 +90,25 @@
     elif isinstance(value, str):
         return repr(value.strip())
     elif isinstance(value, bytes):
         return repr(value.decode('utf-8').strip())
     return str(value)
 
 
+def get_target_prefix(namespaces, target_namespace):
+    """Returns the longest prefix that maps the target namespace."""
+    prefix = None
+    for k, v in namespaces.items():
+        if v == target_namespace:
+            if prefix is None or len(k) > len(prefix):
+                prefix = k
+    else:
+        return prefix
+
+
 class BiunivocalMap(MutableMapping):
     """
     A dictionary that implements a bijective correspondence, namely with constraints
     of uniqueness both on keys and on values. Both keys and values must be hashable.
     """
     def __init__(self, *args, **kwargs):
         self.__map = {}
```

### Comparing `qeschema-1.5.1/qeschema.egg-info/PKG-INFO` & `qeschema-1.5.2/qeschema.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qeschema
-Version: 1.5.1
+Version: 1.5.2
 Summary: Schema-based tools and interfaces for Quantum Espresso data
 Home-page: https://github.com/QEF/qeschema
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,19 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Utilities
 License-File: LICENSE
-Requires-Dist: xmlschema<2.4.0,>=1.6.4
+Requires-Dist: xmlschema<4.0.0,>=2.5.1
 Requires-Dist: numpy
 Provides-Extra: hdf5
 Requires-Dist: h5py; extra == "hdf5"
 Provides-Extra: yaml
 Requires-Dist: pyyaml; extra == "yaml"
 
 =====================================================
```

### Comparing `qeschema-1.5.1/qeschema.egg-info/SOURCES.txt` & `qeschema-1.5.2/qeschema.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements-dev.txt
 setup.py
 tox.ini
-docs/.usage.rst.swp
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/index.rst
 docs/intro.rst
 docs/make.bat
 docs/usage.rst
@@ -44,38 +43,34 @@
 qeschema/schemas/releases/qes_030920.xsd
 qeschema/schemas/releases/qes_181201.xsd
 qeschema/schemas/releases/qes_190207.xsd
 qeschema/schemas/releases/qes_190304.xsd
 qeschema/schemas/releases/qes_190719.xsd
 qeschema/schemas/releases/qes_191206.xsd
 qeschema/schemas/releases/qes_200420.xsd
-qeschema/schemas/releases/qes_210716.xsd
 qeschema/schemas/releases/qes_211101.xsd
 qeschema/schemas/releases/qes_230310.xsd
 qeschema/schemas/releases/qes_neb-20180511.xsd
 qeschema/schemas/releases/qes_neb-211101.xsd
 qeschema/schemas/releases/qes_spectrum-20180511.xsd
 qeschema/schemas/releases/qes_spectrum-20180517.xsd
+qeschema/schemas/releases/qes_test_240411.xsd
 qeschema/schemas/releases/tddfpt-20180511.xsd
 qeschema/schemas/releases/tddfpt-20180517.xsd
-scripts/check.ipynb
-scripts/pwsmartpar.py
 scripts/xml2qeinput.py
 scripts/yaml2qeinput.py
 tests/__init__.py
 tests/test_cards.py
 tests/test_converters.py
 tests/test_documents.py
 tests/test_hdf5.py
 tests/test_options.py
 tests/test_upf.py
 tests/test_utils.py
 tests/examples/pw/Al001_relax_bfgs.in
-tests/examples/pw/CO_bgfs_relax.in
-tests/examples/pw/Fe_noncolin.in
 tests/resources/dummy/incomplete.xml
 tests/resources/dummy/incomplete.xsd
 tests/resources/dummy/instance.csv
 tests/resources/dummy/instance.json
 tests/resources/dummy/instance.xml
 tests/resources/dummy/instance.yaml
 tests/resources/dummy/instance_json
@@ -126,25 +121,22 @@
 tests/resources/pw/Al_bands.xml
 tests/resources/pw/CO_bgfs_relax.in.test
 tests/resources/pw/CO_bgfs_relax.xml
 tests/resources/pw/CO_bgfs_relax_with_external_forces.in.test
 tests/resources/pw/CO_bgfs_relax_with_external_forces.xml
 tests/resources/pw/ESM_2Dxy.in.test
 tests/resources/pw/ESM_2Dxy.xml
-tests/resources/pw/FeO_LDAU_standard.in
 tests/resources/pw/FeO_LDAU_standard.in.test
 tests/resources/pw/FeO_LDAU_standard.xml
 tests/resources/pw/FeO_LDAU_standard_230310.in.test
 tests/resources/pw/FeO_LDAU_standard_230310.xml
-tests/resources/pw/FeO_LDAU_with_no_U.in
 tests/resources/pw/FeO_LDAU_with_no_U.in.test
 tests/resources/pw/FeO_LDAU_with_no_U.xml
 tests/resources/pw/FeO_LDAU_with_no_U_230310.in.test
 tests/resources/pw/FeO_LDAU_with_no_U_230310.xml
-tests/resources/pw/FeO_LDAU_with_starting_ns.in
 tests/resources/pw/FeO_LDAU_with_starting_ns.in.test
 tests/resources/pw/FeO_LDAU_with_starting_ns.xml
 tests/resources/pw/FeO_LDAU_with_starting_ns_230210.in.test
 tests/resources/pw/FeO_LDAU_with_starting_ns_230210.xml
 tests/resources/pw/Fe_Im-3m_0_dftd3.in.test
 tests/resources/pw/Fe_Im-3m_0_dftd3.xml
 tests/resources/pw/Fe_crystal_crystal_positions.in.test
```

### Comparing `qeschema-1.5.1/scripts/xml2qeinput.py` & `qeschema-1.5.2/scripts/xml2qeinput.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/scripts/yaml2qeinput.py` & `qeschema-1.5.2/scripts/yaml2qeinput.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/setup.py` & `qeschema-1.5.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from setuptools import setup
 
 with open("README.rst") as readme:
     long_description = readme.read()
 
 setup(
     name='qeschema',
-    version='1.5.1',
-    install_requires=['xmlschema>=1.6.4,<2.4.0', 'numpy'],
+    version='1.5.2',
+    install_requires=['xmlschema>=2.5.1,<4.0.0', 'numpy'],
     extras_require={
         'HDF5': ['h5py'],
         'YAML': ['pyyaml'],
     },
     packages=['qeschema', 'qeschema.hdf5'],
     package_data={'qeschema': ['schemas/*.xsd', 'schemas/releases/*.xsd']},
     scripts = ['scripts/xml2qeinput.py', 'scripts/yaml2qeinput.py'],
@@ -39,12 +39,13 @@
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Utilities',
     ]
 )
```

### Comparing `qeschema-1.5.1/tests/examples/pw/Al001_relax_bfgs.in` & `qeschema-1.5.2/tests/examples/pw/Al001_relax_bfgs.in`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/examples/pw/CO_bgfs_relax.in` & `qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax.in.test`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 &CONTROL
  calculation='relax'
  disk_io='low'
- etot_conv_thr=0.0001
- forc_conv_thr=0.001
+ etot_conv_thr=5e-05
+ forc_conv_thr=0.0005
  input_xml_schema_file='CO_bgfs_relax.xml'
  iprint=100000
  max_seconds=10000000
- outdir='/scratch/pdelugas/espresso-xsd/tempdir'
+ nstep=50
+ outdir='./'
  prefix='CO'
- pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo'
+ pseudo_dir='./'
  restart_mode='from_scratch'
  title='CO bfgs relaxation'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- ecutrho=144.0
- ecutwfc=24.0
+ ecutrho=72.0
+ ecutwfc=12.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
  nat=2
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
  nspin=1
  ntyp=2
  occupations='fixed'
- spline_ps=.true.
  starting_magnetization(1)=0.0
  starting_magnetization(2)=0.0
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-07
+ conv_thr=5e-08
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
  mixing_beta=0.7
  mixing_mode='plain'
@@ -61,24 +61,24 @@
  trust_radius_max=0.8
  trust_radius_min=0.0001
  upscale=100.0
  w_1=0.01
  w_2=0.5
 /
 &CELL
+ cell_dofree = 'all'
  cell_dynamics='none'
- cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=1822.888
+ wmass=0.0
 /
 ATOMIC_SPECIES
- O 1.0 O.pz-rrkjus.UPF
- C 1.0 C.pz-rrkjus.UPF
+ O 1.0 O.pbesol-n-kjpaw_psl.0.1.UPF
+ C 1.0 C.pbesol-n-kjpaw_psl.1.0.0.UPF
 ATOMIC_POSITIONS bohr
 C      0.18800000    0.00000000    0.00000000
 O      0.00000000    0.00000000    0.00000000    0   0   0
 K_POINTS gamma
 CELL_PARAMETERS bohr
-  1.00000000   0.00000000   0.00000000 
-  0.00000000   1.00000000   0.00000000 
-  0.00000000   0.00000000   1.00000000 
+ 10.00000000   0.00000000   0.00000000 
+  0.00000000  10.00000000   0.00000000 
+  0.00000000   0.00000000  10.00000000
```

### Comparing `qeschema-1.5.1/tests/examples/pw/Fe_noncolin.in` & `qeschema-1.5.2/tests/resources/pw/Fe_non_collinear_penalty.in.test`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 &CONTROL
  calculation='scf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='Fe_noncolin.xml'
+ input_xml_schema_file='Fe_non_collinear_penalty.xml'
  iprint=100000
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
  prefix='fe'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='Fe_non_collinear'
+ title=''
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
+ constrained_magnetization='atomic'
  degauss=0.05
  ecutrho=200.0
  ecutwfc=25.0
+ fixed_magnetization=[0.0, 0.0, 0.0]
  force_symmorphic=.false.
-ibrav = 3
-A =     0.458280, B =     0.458280, C =     0.458280, COSAB =      0.33333, COSBC =     -0.33333, COSAC =      0.33333
+ ibrav=0
  input_dft='PZ'
+ lambda=1.0
  lspinorb=.false.
  nat=1
  no_t_rev=.false.
  noinv=.false.
- noncolin=.true.
+ noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
- nspin=4
+ nspin=1
  ntyp=1
  occupations='smearing'
  smearing='mv'
  starting_magnetization(1)=0.5
  tot_charge=0.0
  use_all_frac=.false.
 /
@@ -81,8 +83,8 @@
  0.0625 0.0625 0.9375 3.0
  0.0625 0.1875 0.1875 3.0
  0.0625 0.1875 0.3125 6.0
  0.0625 0.1875 0.4375 6.0
 CELL_PARAMETERS bohr
   0.50000000   0.50000000   0.50000000 
  -0.50000000   0.50000000   0.50000000 
- -0.50000000  -0.50000000   0.50000000 
+ -0.50000000  -0.50000000   0.50000000
```

### Comparing `qeschema-1.5.1/tests/resources/dummy/incomplete.xsd` & `qeschema-1.5.2/tests/resources/dummy/incomplete.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/dummy/schema.xsd` & `qeschema-1.5.2/tests/resources/dummy/schema.xsd`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/epw/epw_test1.xml` & `qeschema-1.5.2/tests/resources/epw/epw_test1.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/epw/epw_test2.in.test` & `qeschema-1.5.2/tests/resources/epw/epw_test2.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/epw/epw_test2.xml` & `qeschema-1.5.2/tests/resources/epw/epw_test2.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/Al001+H_pbc.in.test` & `qeschema-1.5.2/tests/resources/neb/Al001+H_pbc.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/Al001+H_pbc.xml` & `qeschema-1.5.2/tests/resources/neb/Al001+H_pbc.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/Al001_plus_H_bc3.in.test` & `qeschema-1.5.2/tests/resources/neb/Al001_plus_H_bc3.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/Al001_plus_H_bc3.xml` & `qeschema-1.5.2/tests/resources/neb/Al001_plus_H_bc3.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/H2+H.in.test` & `qeschema-1.5.2/tests/resources/neb/H2+H.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/H2+H.xml` & `qeschema-1.5.2/tests/resources/neb/H2+H.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/H2+H_crystal.in.test` & `qeschema-1.5.2/tests/resources/neb/H2+H_crystal.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/H2+H_crystal.xml` & `qeschema-1.5.2/tests/resources/neb/H2+H_crystal.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.in.test` & `qeschema-1.5.2/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.xml` & `qeschema-1.5.2/tests/resources/neb/periodic_dft_65_WaterP1_0_neb_0.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/al.elph.xml` & `qeschema-1.5.2/tests/resources/ph/al.elph.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/alas_ph.xml` & `qeschema-1.5.2/tests/resources/ph/alas_ph.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/alas_recover.xml` & `qeschema-1.5.2/tests/resources/ph/alas_recover.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/ch4_nm.xml` & `qeschema-1.5.2/tests/resources/ph/ch4_nm.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/nat_todo.xml` & `qeschema-1.5.2/tests/resources/ph/nat_todo.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/nat_todo_zero.xml` & `qeschema-1.5.2/tests/resources/ph/nat_todo_zero.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/sio2_dielectric.xml` & `qeschema-1.5.2/tests/resources/ph/sio2_dielectric.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/sio2_prova_disp.xml` & `qeschema-1.5.2/tests/resources/ph/sio2_prova_disp.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/ph/sio2_prova_qplot.xml` & `qeschema-1.5.2/tests/resources/ph/sio2_prova_qplot.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs-input.yml` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs-input.yml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.in` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.in`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.in.test` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.json` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.json`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.xml` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_relax_bfgs.yml` & `qeschema-1.5.2/tests/resources/pw/Al001_relax_bfgs.yml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_rlx_damp.in.test` & `qeschema-1.5.2/tests/resources/pw/Al001_rlx_damp.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al001_rlx_damp.xml` & `qeschema-1.5.2/tests/resources/pw/Al001_rlx_damp.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al_bands.in.test` & `qeschema-1.5.2/tests/resources/pw/Al_bands.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Al_bands.xml` & `qeschema-1.5.2/tests/resources/pw/Al_bands.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax.in.test` & `qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax_with_external_forces.in.test`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 &CONTROL
  calculation='relax'
  disk_io='low'
- etot_conv_thr=5e-05
- forc_conv_thr=0.0005
- input_xml_schema_file='CO_bgfs_relax.xml'
+ etot_conv_thr=0.0001
+ forc_conv_thr=0.001
+ input_xml_schema_file='CO_bgfs_relax_with_external_forces.xml'
  iprint=100000
  max_seconds=10000000
- nstep=50
- outdir='./'
+ outdir='/scratch/pdelugas/espresso-xsd/tempdir'
  prefix='CO'
- pseudo_dir='./'
+ pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo'
  restart_mode='from_scratch'
  title='CO bfgs relaxation'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- ecutrho=72.0
- ecutwfc=12.0
+ ecutrho=144.0
+ ecutwfc=24.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
  nat=2
  no_t_rev=.false.
  noinv=.false.
@@ -35,15 +34,15 @@
  occupations='fixed'
  starting_magnetization(1)=0.0
  starting_magnetization(2)=0.0
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=5e-08
+ conv_thr=1e-07
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
  mixing_beta=0.7
  mixing_mode='plain'
@@ -61,24 +60,27 @@
  trust_radius_max=0.8
  trust_radius_min=0.0001
  upscale=100.0
  w_1=0.01
  w_2=0.5
 /
 &CELL
- cell_dofree = 'all'
  cell_dynamics='none'
+ cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=0.0
+ wmass=1822.888
 /
 ATOMIC_SPECIES
- O 1.0 O.pbesol-n-kjpaw_psl.0.1.UPF
- C 1.0 C.pbesol-n-kjpaw_psl.1.0.0.UPF
+ O 1.0 O.pz-rrkjus.UPF
+ C 1.0 C.pz-rrkjus.UPF
 ATOMIC_POSITIONS bohr
 C      0.18800000    0.00000000    0.00000000
 O      0.00000000    0.00000000    0.00000000    0   0   0
 K_POINTS gamma
 CELL_PARAMETERS bohr
- 10.00000000   0.00000000   0.00000000 
-  0.00000000  10.00000000   0.00000000 
-  0.00000000   0.00000000  10.00000000 
+  1.00000000   0.00000000   0.00000000 
+  0.00000000   1.00000000   0.00000000 
+  0.00000000   0.00000000   1.00000000 
+ATOMIC_FORCES
+C        0.10000000     0.00000000     0.00000000
+O       -0.10000000     0.00000000     0.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax.xml` & `qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax_with_external_forces.in.test` & `qeschema-1.5.2/tests/resources/pw/Fe_noncolin.in.test`

 * *Files 19% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 &CONTROL
- calculation='relax'
+ calculation='scf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='CO_bgfs_relax_with_external_forces.xml'
+ input_xml_schema_file='Fe_noncolin.xml'
  iprint=100000
  max_seconds=10000000
- outdir='/scratch/pdelugas/espresso-xsd/tempdir'
- prefix='CO'
- pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo'
+ outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
+ prefix='fe'
+ pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='CO bfgs relaxation'
+ title='Fe_non_collinear'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- ecutrho=144.0
- ecutwfc=24.0
+ degauss=0.05
+ ecutrho=200.0
+ ecutwfc=25.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
- nat=2
+ nat=1
  no_t_rev=.false.
  noinv=.false.
- noncolin=.false.
+ noncolin=.true.
  nosym=.false.
  nosym_evc=.false.
- nspin=1
- ntyp=2
- occupations='fixed'
- starting_magnetization(1)=0.0
- starting_magnetization(2)=0.0
+ nspin=4
+ ntyp=1
+ occupations='smearing'
+ smearing='mv'
+ starting_magnetization(1)=0.5
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-07
+ conv_thr=1e-08
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.7
+ mixing_beta=0.2
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
- bfgs_ndim=1
- ion_dynamics='bfgs'
+ ion_dynamics='none'
  refold_pos=.false.
  remove_rigid_rot=.false.
- trust_radius_ini=0.5
- trust_radius_max=0.8
- trust_radius_min=0.0001
- upscale=100.0
- w_1=0.01
- w_2=0.5
 /
 &CELL
  cell_dynamics='none'
  cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=1822.888
+ wmass=50901.43
 /
 ATOMIC_SPECIES
- O 1.0 O.pz-rrkjus.UPF
- C 1.0 C.pz-rrkjus.UPF
+ Fe 55.847 Fe.pz-nd-rrkjus.UPF
 ATOMIC_POSITIONS bohr
-C      0.18800000    0.00000000    0.00000000
-O      0.00000000    0.00000000    0.00000000    0   0   0
-K_POINTS gamma
+Fe     0.00000000    0.00000000    0.00000000
+K_POINTS
+ 11
+ 0.0625 0.0625 0.0625 1.0
+ 0.0625 0.0625 0.1875 3.0
+ 0.0625 0.0625 0.3125 3.0
+ 0.0625 0.0625 0.4375 3.0
+ 0.0625 0.0625 0.5625 3.0
+ 0.0625 0.0625 0.6875 3.0
+ 0.0625 0.0625 0.8125 3.0
+ 0.0625 0.0625 0.9375 3.0
+ 0.0625 0.1875 0.1875 3.0
+ 0.0625 0.1875 0.3125 6.0
+ 0.0625 0.1875 0.4375 6.0
 CELL_PARAMETERS bohr
-  1.00000000   0.00000000   0.00000000 
-  0.00000000   1.00000000   0.00000000 
-  0.00000000   0.00000000   1.00000000 
-ATOMIC_FORCES
-C        0.10000000     0.00000000     0.00000000
-O       -0.10000000     0.00000000     0.00000000
+  2.60850000   2.60850000   2.60850000 
+ -2.60850000   2.60850000   2.60850000 
+ -2.60850000  -2.60850000   2.60850000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/CO_bgfs_relax_with_external_forces.xml` & `qeschema-1.5.2/tests/resources/pw/CO_bgfs_relax_with_external_forces.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/ESM_2Dxy.in.test` & `qeschema-1.5.2/tests/resources/pw/ESM_2Dxy.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/ESM_2Dxy.xml` & `qeschema-1.5.2/tests/resources/pw/ESM_2Dxy.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.in` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U_230310.in.test`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 &CONTROL
  calculation='scf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='FeO_LDAU_standard.xml'
+ input_xml_schema_file='FeO_LDAU_with_no_U_230310.xml'
  iprint=100000
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
  prefix='feo_af'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='FeO_LDA+U'
+ title='FeO_LDA+U=0'
  tprnfor=.true.
  tstress=.true.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
  degauss=0.01
@@ -79,9 +79,9 @@
 K_POINTS automatic
  2 2 2 0 0 0
 CELL_PARAMETERS bohr
   0.50000000   0.50000000   1.00000000 
   0.50000000   1.00000000   0.50000000 
   1.00000000   0.50000000   0.50000000 
 HUBBARD atomic
-U Fe1-3d 0.3160442
-U Fe2-3d 0.3160442
+U  Fe1-3d     0.000
+U  Fe2-3d     0.000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.in.test` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard_230310.in.test` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard_230310.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_standard_230310.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_standard_230310.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.in` & `qeschema-1.5.2/tests/resources/pw/Pt_spinorbit.in.test`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 &CONTROL
  calculation='scf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='FeO_LDAU_with_no_U.xml'
+ input_xml_schema_file='Pt_spinorbit.xml'
  iprint=100000
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
- prefix='feo_af'
+ prefix='Pt'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='FeO_LDA+U=0'
+ title='Pt_fullyRelativistic'
  tprnfor=.true.
  tstress=.true.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- degauss=0.01
- ecutrho=240.0
+ degauss=0.02
+ ecutrho=250.0
  ecutwfc=30.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
- lspinorb=.false.
- nat=4
- nbnd=20
+ lspinorb=.true.
+ nat=1
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
- nspin=2
- ntyp=3
+ nspin=1
+ ntyp=1
  occupations='smearing'
- smearing='gaussian'
+ smearing='mp'
  starting_magnetization(1)=0.0
- starting_magnetization(2)=0.5
- starting_magnetization(3)=-0.5
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-06
+ conv_thr=1e-08
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.3
+ mixing_beta=0.7
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
@@ -61,27 +58,19 @@
  remove_rigid_rot=.false.
 /
 &CELL
  cell_dynamics='none'
  cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=3645.777
+ wmass=177802.7
 /
 ATOMIC_SPECIES
- O1 1.0 O.pz-rrkjus.UPF
- Fe1 1.0 Fe.pz-nd-rrkjus.UPF
- Fe2 1.0 Fe.pz-nd-rrkjus.UPF
+ Pt 0.0 Pt.rel-pz-n-rrkjus.UPF
 ATOMIC_POSITIONS bohr
-O1     0.50000000    0.50000000    0.50000000
-O1     1.50000000    1.50000000    1.50000000
-Fe1    0.00000000    0.00000000    0.00000000
-Fe2    1.00000000    1.00000000    1.00000000
+Pt     0.00000000    0.00000000    0.00000000
 K_POINTS automatic
- 2 2 2 0 0 0
+ 4 4 4 1 1 1
 CELL_PARAMETERS bohr
-  0.50000000   0.50000000   1.00000000 
-  0.50000000   1.00000000   0.50000000 
-  1.00000000   0.50000000   0.50000000 
-HUBBARD atomic
-U Fe1-3d 7.349865e-10
-U Fe2-3d 7.349865e-10
+ -0.50000000   0.00000000   0.50000000 
+  0.00000000   0.50000000   0.50000000 
+ -0.50000000   0.50000000   0.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.in.test` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U_230310.in.test` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_BerryPhase.in.test`

 * *Files 14% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 &CONTROL
- calculation='scf'
+ calculation='nscf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='FeO_LDAU_with_no_U_230310.xml'
+ gdir=3
+ input_xml_schema_file='PbTiO3_BerryPhase.xml'
  iprint=100000
+ lberry=.true.
+ lelfield=.false.
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
- prefix='feo_af'
+ prefix='pwscf'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='FeO_LDA+U=0'
- tprnfor=.true.
- tstress=.true.
+ tefield=.false.
+ title='PbTiO_3_BerryPhase'
+ tprnfor=.false.
+ tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- degauss=0.01
- ecutrho=240.0
  ecutwfc=30.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
- nat=4
- nbnd=20
+ nat=5
+ nbnd=22
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
- nspin=2
+ nspin=1
  ntyp=3
- occupations='smearing'
- smearing='gaussian'
+ occupations='fixed'
  starting_magnetization(1)=0.0
- starting_magnetization(2)=0.5
- starting_magnetization(3)=-0.5
+ starting_magnetization(2)=0.0
+ starting_magnetization(3)=0.0
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-06
+ conv_thr=1e-05
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
+ efield_cart=[0.0, 0.0, 0.0]
  electron_maxstep=100
  mixing_beta=0.3
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
@@ -61,27 +63,25 @@
  remove_rigid_rot=.false.
 /
 &CELL
  cell_dynamics='none'
  cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=3645.777
+ wmass=276227.0
 /
 ATOMIC_SPECIES
- O1 1.0 O.pz-rrkjus.UPF
- Fe1 1.0 Fe.pz-nd-rrkjus.UPF
- Fe2 1.0 Fe.pz-nd-rrkjus.UPF
+ Pb 207.2 Pb.pz-d-van.UPF
+ Ti 47.867 Ti.pz-sp-van_ak.UPF
+ O 15.9994 O.pz-van_ak.UPF
 ATOMIC_POSITIONS bohr
-O1     0.50000000    0.50000000    0.50000000
-O1     1.50000000    1.50000000    1.50000000
-Fe1    0.00000000    0.00000000    0.00000000
-Fe2    1.00000000    1.00000000    1.00000000
+Pb     0.00000000    0.00000000    0.00135687
+Ti     0.06784353    0.06784353    0.06784353
+O      0.00000000    0.06784353    0.06784353
+O      0.06784353    0.06784353    0.00000000
+O      0.06784353    0.00000000    0.06784353
 K_POINTS automatic
- 2 2 2 0 0 0
+ 4 4 7 1 1 1
 CELL_PARAMETERS bohr
-  0.50000000   0.50000000   1.00000000 
-  0.50000000   1.00000000   0.50000000 
-  1.00000000   0.50000000   0.50000000 
-HUBBARD atomic
-U  Fe1-3d     0.000
-U  Fe2-3d     0.000
+  1.00000000   0.00000000   0.00000000 
+  0.00000000   1.00000000   0.00000000 
+  0.00000000   0.00000000   1.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_no_U_230310.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_no_U_230310.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.in` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns.in.test`

 * *Files 9% similar despite different names*

```diff
@@ -17,16 +17,20 @@
  wf_collect=.false.
 /
 &SYSTEM
  degauss=0.01
  ecutrho=240.0
  ecutwfc=30.0
  force_symmorphic=.false.
+ Hubbard_U(2)=0.3160442
+ Hubbard_U(3)=0.3160442
  ibrav=0
  input_dft='PZ'
+ lda_plus_u = .true.
+ lda_plus_u_kind = 0
  lspinorb=.false.
  nat=4
  nbnd=20
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
@@ -37,14 +41,15 @@
  smearing='gaussian'
  starting_magnetization(1)=0.0
  starting_magnetization(2)=0.5
  starting_magnetization(3)=-0.5
  starting_ns_eigenvalue(3,1,3)=1.0
  starting_ns_eigenvalue(3,2,2)=1.0
  tot_charge=0.0
+ U_projection_type = 'atomic'
  use_all_frac=.false.
 /
 &ELECTRONS
  conv_thr=1e-08
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
@@ -80,10 +85,7 @@
 Fe2    8.19000000    8.19000000    8.19000000
 K_POINTS automatic
  2 2 2 0 0 0
 CELL_PARAMETERS bohr
   4.09500000   4.09500000   8.19000000 
   4.09500000   8.19000000   4.09500000 
   8.19000000   4.09500000   4.09500000 
-HUBBARD atomic
-U Fe1-3d 0.3160442
-U Fe2-3d 0.3160442
```

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.in.test` & `qeschema-1.5.2/tests/resources/pw/Fe_Im-3m_0_dftd3.in.test`

 * *Files 14% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 &CONTROL
- calculation='scf'
+ calculation='relax'
  disk_io='low'
- etot_conv_thr=0.0001
+ dt=41.3414
+ etot_conv_thr=1e-05
  forc_conv_thr=0.001
- input_xml_schema_file='FeO_LDAU_with_starting_ns.xml'
+ input_xml_schema_file='Fe_Im-3m_0_dftd3.xml'
  iprint=100000
  max_seconds=10000000
+ nstep=50
  outdir='./'
- prefix='pwscf'
- pseudo_dir='/u/cm/pdelugas/espresso/pseudo/'
+ prefix='Fe_Im-3m_0_dftd3'
+ pseudo_dir='./'
  restart_mode='from_scratch'
- title='uffa'
+ title='Fe_Im-3m_0_dftd3'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
  degauss=0.01
- ecutrho=240.0
- ecutwfc=30.0
+ dftd3_threebody=.true.
+ dftd3_version=4
+ ecutrho=100.0
+ ecutwfc=20.0
  force_symmorphic=.false.
- Hubbard_U(2)=0.3160442
- Hubbard_U(3)=0.3160442
  ibrav=0
- input_dft='PZ'
- lda_plus_u = .true.
- lda_plus_u_kind = 0
+ input_dft='PBE'
  lspinorb=.false.
- nat=4
- nbnd=20
+ nat=2
+ nbnd=26
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
  nspin=2
- ntyp=3
+ ntyp=2
  occupations='smearing'
  smearing='gaussian'
- starting_magnetization(1)=0.0
- starting_magnetization(2)=0.5
- starting_magnetization(3)=-0.5
- starting_ns_eigenvalue(3,1,3)=1.0
- starting_ns_eigenvalue(3,2,2)=1.0
+ spline_ps=.false.
+ starting_magnetization(1)=0.4
+ starting_magnetization(2)=0.6
  tot_charge=0.0
- U_projection_type = 'atomic'
+ tot_magnetization=-1.0
  use_all_frac=.false.
+ vdw_corr='DFT-D3'
 /
 &ELECTRONS
- conv_thr=1e-08
+ conv_thr=1e-06
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.3
+ mixing_beta=0.7
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
- ion_dynamics='none'
- refold_pos=.false.
- remove_rigid_rot=.false.
+ delta_t=1.0
+ ion_dynamics='bfgs'
+ ion_temperature='rescale-v'
+ nraise=1
+ pot_extrapolation='atomic'
+ tempw=300.0
+ tolp=100.0
+ wfc_extrapolation='none'
 /
 &CELL
- cell_dynamics='none'
- cell_factor=0.0
+ cell_dynamics='bfgs'
+ cell_factor=2.0
  press=0.0
  press_conv_thr=0.5
- wmass=3645.777
 /
 ATOMIC_SPECIES
- O1 1.0 O.pz-rrkjus.UPF
- Fe1 1.0 Fe.pz-nd-rrkjus.UPF
- Fe2 1.0 Fe.pz-nd-rrkjus.UPF
-ATOMIC_POSITIONS bohr
-O1     4.09500000    4.09500000    4.09500000
-O1    12.28500000   12.28500000   12.28500000
-Fe1    0.00000000    0.00000000    0.00000000
-Fe2    8.19000000    8.19000000    8.19000000
+ Fe 55.845 fe_pbe_v1.5.uspp.F.UPF
+ Fe1 55.845 fe_pbe_v1.5.uspp.F.UPF
+ATOMIC_POSITIONS crystal
+Fe     0.00000000    0.00000000    0.00000000
+Fe1    0.50000000    0.50000000    0.50000000
 K_POINTS automatic
- 2 2 2 0 0 0
+ 2 2 2 1 1 1
 CELL_PARAMETERS bohr
-  4.09500000   4.09500000   8.19000000 
-  4.09500000   8.19000000   4.09500000 
-  8.19000000   4.09500000   4.09500000 
+  5.40650600   0.00000000   0.00000000 
+  0.00000000   5.40650600   0.00000000 
+  0.00000000   0.00000000   5.40650600
```

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.in.test` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.in.test`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.xml` & `qeschema-1.5.2/tests/resources/pw/FeO_LDAU_with_starting_ns_230210.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_Im-3m_0_dftd3.in.test` & `qeschema-1.5.2/tests/resources/pw/Fe_crystal_crystal_positions.in.test`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 &CONTROL
  calculation='relax'
  disk_io='low'
  dt=41.3414
  etot_conv_thr=1e-05
  forc_conv_thr=0.001
- input_xml_schema_file='Fe_Im-3m_0_dftd3.xml'
+ input_xml_schema_file='Fe_crystal_crystal_positions.xml'
  iprint=100000
  max_seconds=10000000
  nstep=50
  outdir='./'
- prefix='Fe_Im-3m_0_dftd3'
+ prefix='Fe_crystal_crystal_positions'
  pseudo_dir='./'
  restart_mode='from_scratch'
- title='Fe_Im-3m_0_dftd3'
+ title='Fe_crystal_crystal_positions'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
  degauss=0.01
- dftd3_threebody=.true.
- dftd3_version=4
  ecutrho=100.0
  ecutwfc=20.0
  force_symmorphic=.false.
  ibrav=0
- input_dft='PBE'
+ input_dft='BLYP'
  lspinorb=.false.
  nat=2
  nbnd=26
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
@@ -41,15 +39,14 @@
  smearing='gaussian'
  spline_ps=.false.
  starting_magnetization(1)=0.4
  starting_magnetization(2)=0.6
  tot_charge=0.0
  tot_magnetization=-1.0
  use_all_frac=.false.
- vdw_corr='DFT-D3'
 /
 &ELECTRONS
  conv_thr=1e-06
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
```

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_Im-3m_0_dftd3.xml` & `qeschema-1.5.2/tests/resources/pw/Fe_Im-3m_0_dftd3.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_crystal_crystal_positions.in.test` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_bc3_fcp_opt.in.test`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,91 @@
 &CONTROL
- calculation='relax'
+ calculation='scf'
  disk_io='low'
- dt=41.3414
- etot_conv_thr=1e-05
+ etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='Fe_crystal_crystal_positions.xml'
+ input_xml_schema_file='PbTiO3_bc3_fcp_opt.xml'
  iprint=100000
+ lfcp=.true.
  max_seconds=10000000
- nstep=50
- outdir='./'
- prefix='Fe_crystal_crystal_positions'
- pseudo_dir='./'
+ outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
+ prefix='pwscf'
+ pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='Fe_crystal_crystal_positions'
+ title='PBTiO3_scf'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- degauss=0.01
- ecutrho=100.0
- ecutwfc=20.0
+ assume_isolated='esm'
+ ecutwfc=30.0
+ esm_bc='bc3'
+ esm_efield=0.1
+ esm_nfit=5
+ esm_w=1.2
  force_symmorphic=.false.
  ibrav=0
- input_dft='BLYP'
+ input_dft='PZ'
  lspinorb=.false.
- nat=2
- nbnd=26
+ nat=5
+ nbnd=25
  no_t_rev=.false.
  noinv=.false.
  noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
- nspin=2
- ntyp=2
- occupations='smearing'
- smearing='gaussian'
- spline_ps=.false.
- starting_magnetization(1)=0.4
- starting_magnetization(2)=0.6
+ nspin=1
+ ntyp=3
+ occupations='fixed'
+ starting_magnetization(1)=0.0
+ starting_magnetization(2)=0.0
+ starting_magnetization(3)=0.0
  tot_charge=0.0
- tot_magnetization=-1.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-06
+ conv_thr=1e-12
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.7
+ mixing_beta=0.3
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
- delta_t=1.0
- ion_dynamics='bfgs'
- ion_temperature='rescale-v'
- nraise=1
- pot_extrapolation='atomic'
- tempw=300.0
- tolp=100.0
- wfc_extrapolation='none'
+ ion_dynamics='none'
+ refold_pos=.false.
+ remove_rigid_rot=.false.
 /
 &CELL
- cell_dynamics='bfgs'
- cell_factor=2.0
+ cell_dynamics='none'
+ cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
+ wmass=276227.0
+/
+&FCP
+ fcp_mu=-0.036749
 /
 ATOMIC_SPECIES
- Fe 55.845 fe_pbe_v1.5.uspp.F.UPF
- Fe1 55.845 fe_pbe_v1.5.uspp.F.UPF
-ATOMIC_POSITIONS crystal
-Fe     0.00000000    0.00000000    0.00000000
-Fe1    0.50000000    0.50000000    0.50000000
+ Pb 207.2 Pb.pz-d-van.UPF
+ Ti 47.867 Ti.pz-sp-van_ak.UPF
+ O 15.9994 O.pz-van_ak.UPF
+ATOMIC_POSITIONS bohr
+Pb     0.00000000    0.00000000    0.00135687
+Ti     0.06784353    0.06784353    0.06784353
+O      0.00000000    0.06784353    0.06784353
+O      0.06784353    0.06784353    0.00000000
+O      0.06784353    0.00000000    0.06784353
 K_POINTS automatic
- 2 2 2 1 1 1
+ 4 4 4 1 1 1
 CELL_PARAMETERS bohr
-  5.40650600   0.00000000   0.00000000 
-  0.00000000   5.40650600   0.00000000 
-  0.00000000   0.00000000   5.40650600 
+  1.00000000   0.00000000   0.00000000 
+  0.00000000   1.00000000   0.00000000 
+  0.00000000   0.00000000   1.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_crystal_crystal_positions.xml` & `qeschema-1.5.2/tests/resources/pw/Fe_crystal_crystal_positions.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_non_collinear_penalty.xml` & `qeschema-1.5.2/tests/resources/pw/Fe_non_collinear_penalty.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_noncolin.in.test` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_scf.in.test`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 &CONTROL
  calculation='scf'
  disk_io='low'
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='Fe_noncolin.xml'
+ input_xml_schema_file='PbTiO3_scf.xml'
  iprint=100000
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
- prefix='fe'
+ prefix='pwscf'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='Fe_non_collinear'
+ title='PBTiO3_scf'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- degauss=0.05
- ecutrho=200.0
- ecutwfc=25.0
+ ecutwfc=30.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
- nat=1
+ nat=5
+ nbnd=25
  no_t_rev=.false.
  noinv=.false.
- noncolin=.true.
+ noncolin=.false.
  nosym=.false.
  nosym_evc=.false.
- nspin=4
- ntyp=1
- occupations='smearing'
- smearing='mv'
- starting_magnetization(1)=0.5
+ nspin=1
+ ntyp=3
+ occupations='fixed'
+ starting_magnetization(1)=0.0
+ starting_magnetization(2)=0.0
+ starting_magnetization(3)=0.0
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-08
+ conv_thr=1e-12
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.2
+ mixing_beta=0.3
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
@@ -58,30 +58,25 @@
  remove_rigid_rot=.false.
 /
 &CELL
  cell_dynamics='none'
  cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=50901.43
+ wmass=276227.0
 /
 ATOMIC_SPECIES
- Fe 55.847 Fe.pz-nd-rrkjus.UPF
+ Pb 207.2 Pb.pz-d-van.UPF
+ Ti 47.867 Ti.pz-sp-van_ak.UPF
+ O 15.9994 O.pz-van_ak.UPF
 ATOMIC_POSITIONS bohr
-Fe     0.00000000    0.00000000    0.00000000
-K_POINTS
- 11
- 0.0625 0.0625 0.0625 1.0
- 0.0625 0.0625 0.1875 3.0
- 0.0625 0.0625 0.3125 3.0
- 0.0625 0.0625 0.4375 3.0
- 0.0625 0.0625 0.5625 3.0
- 0.0625 0.0625 0.6875 3.0
- 0.0625 0.0625 0.8125 3.0
- 0.0625 0.0625 0.9375 3.0
- 0.0625 0.1875 0.1875 3.0
- 0.0625 0.1875 0.3125 6.0
- 0.0625 0.1875 0.4375 6.0
+Pb     0.00000000    0.00000000    0.00135687
+Ti     0.06784353    0.06784353    0.06784353
+O      0.00000000    0.06784353    0.06784353
+O      0.06784353    0.06784353    0.00000000
+O      0.06784353    0.00000000    0.06784353
+K_POINTS automatic
+ 4 4 4 1 1 1
 CELL_PARAMETERS bohr
-  2.60850000   2.60850000   2.60850000 
- -2.60850000   2.60850000   2.60850000 
- -2.60850000  -2.60850000   2.60850000 
+  1.00000000   0.00000000   0.00000000 
+  0.00000000   1.00000000   0.00000000 
+  0.00000000   0.00000000   1.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/Fe_noncolin.xml` & `qeschema-1.5.2/tests/resources/pw/Fe_noncolin.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Ni.xml` & `qeschema-1.5.2/tests/resources/pw/Ni.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/PbTiO3_BerryPhase.xml` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_BerryPhase.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/PbTiO3_bc3_fcp_opt.xml` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_bc3_fcp_opt.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/PbTiO3_scf.in.test` & `qeschema-1.5.2/tests/resources/pw/Si_md.in.test`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 &CONTROL
- calculation='scf'
- disk_io='low'
+ calculation='md'
+ disk_io='high'
+ dt=20.0
  etot_conv_thr=0.0001
  forc_conv_thr=0.001
- input_xml_schema_file='PbTiO3_scf.xml'
+ input_xml_schema_file='Si_md.xml'
  iprint=100000
  max_seconds=10000000
  outdir='/scratch/pdelugas/espresso-xsd/tempdir/'
  prefix='pwscf'
  pseudo_dir='/scratch/pdelugas/espresso-xsd/pseudo/'
  restart_mode='from_scratch'
- title='PBTiO3_scf'
+ title='Si_molecular_dynamics'
  tprnfor=.false.
  tstress=.false.
  verbosity='low'
  wf_collect=.false.
 /
 &SYSTEM
- ecutwfc=30.0
+ ecutwfc=8.0
  force_symmorphic=.false.
  ibrav=0
  input_dft='PZ'
  lspinorb=.false.
- nat=5
- nbnd=25
- no_t_rev=.false.
- noinv=.false.
+ nat=8
+ no_t_rev=.true.
+ noinv=.true.
  noncolin=.false.
- nosym=.false.
- nosym_evc=.false.
+ nosym=.true.
+ nosym_evc=.true.
  nspin=1
- ntyp=3
+ ntyp=1
  occupations='fixed'
  starting_magnetization(1)=0.0
- starting_magnetization(2)=0.0
- starting_magnetization(3)=0.0
  tot_charge=0.0
  use_all_frac=.false.
 /
 &ELECTRONS
- conv_thr=1e-12
+ conv_thr=1e-08
  diago_cg_maxiter=20
  diago_full_acc=.false.
  diago_thr_init=0.0
  diagonalization='davidson'
  electron_maxstep=100
- mixing_beta=0.3
+ mixing_beta=0.7
  mixing_mode='plain'
  mixing_ndim=8
  tbeta_smoothing=.false.
  tq_smoothing=.false.
  tqr=.false.
 /
 &IONS
- ion_dynamics='none'
+ delta_t=1.0
+ ion_dynamics='verlet'
+ ion_temperature='not_controlled'
+ nraise=1
+ pot_extrapolation='second-order'
  refold_pos=.false.
  remove_rigid_rot=.false.
+ tempw=300.0
+ tolp=100.0
+ wfc_extrapolation='second-order'
 /
 &CELL
  cell_dynamics='none'
  cell_factor=0.0
  press=0.0
  press_conv_thr=0.5
- wmass=276227.0
+ wmass=204790.6
 /
 ATOMIC_SPECIES
- Pb 207.2 Pb.pz-d-van.UPF
- Ti 47.867 Ti.pz-sp-van_ak.UPF
- O 15.9994 O.pz-van_ak.UPF
+ Si 28.086 Si.pz-vbc.UPF
 ATOMIC_POSITIONS bohr
-Pb     0.00000000    0.00000000    0.00135687
-Ti     0.06784353    0.06784353    0.06784353
-O      0.00000000    0.06784353    0.06784353
-O      0.06784353    0.06784353    0.00000000
-O      0.06784353    0.00000000    0.06784353
+Si    -0.01208251   -0.01208251   -0.01208251    1   0   1
+Si     0.03703340    0.03703340   -0.01208251    1   0   1
+Si     0.03703340   -0.01208251    0.03703340
+Si    -0.01208251    0.03703340    0.03703340    1   0   1
+Si     0.01208251    0.01208251    0.01208251    1   0   1
+Si     0.06119843    0.06119843    0.01208251    1   0   1
+Si     0.06119843    0.01208251    0.06119843    1   0   1
+Si     0.01208251    0.06119843    0.06119843    1   0   1
 K_POINTS automatic
- 4 4 4 1 1 1
+ 1 1 1 0 0 0
 CELL_PARAMETERS bohr
   1.00000000   0.00000000   0.00000000 
   0.00000000   1.00000000   0.00000000 
-  0.00000000   0.00000000   1.00000000 
+  0.00000000   0.00000000   1.00000000
```

### Comparing `qeschema-1.5.1/tests/resources/pw/PbTiO3_scf.xml` & `qeschema-1.5.2/tests/resources/pw/PbTiO3_scf.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Pt_spinorbit.xml` & `qeschema-1.5.2/tests/resources/pw/Pt_spinorbit.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Si.xml` & `qeschema-1.5.2/tests/resources/pw/Si.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/pw/Si_md.xml` & `qeschema-1.5.2/tests/resources/pw/Si_md.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/tddfpt/Ag.tddfpt-eels.xml` & `qeschema-1.5.2/tests/resources/tddfpt/Ag.tddfpt-eels.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/tddfpt/Benzene.dav.xml` & `qeschema-1.5.2/tests/resources/tddfpt/Benzene.dav.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt.xml` & `qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/tddfpt/CH4.tddfpt_pp.xml` & `qeschema-1.5.2/tests/resources/tddfpt/CH4.tddfpt_pp.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/upf/N.pz-vbc.UPF` & `qeschema-1.5.2/tests/resources/upf/N.pz-vbc.UPF`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/xspectra/Cu_L23_xspectra.xml` & `qeschema-1.5.2/tests/resources/xspectra/Cu_L23_xspectra.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/xspectra/NiO_xspectra_dip.xml` & `qeschema-1.5.2/tests/resources/xspectra/NiO_xspectra_dip.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/xspectra/xspectra_example_full.in` & `qeschema-1.5.2/tests/resources/xspectra/xspectra_example_full.in`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/resources/xspectra/xspectra_example_full.xml` & `qeschema-1.5.2/tests/resources/xspectra/xspectra_example_full.xml`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_cards.py` & `qeschema-1.5.2/tests/test_cards.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_converters.py` & `qeschema-1.5.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_documents.py` & `qeschema-1.5.2/tests/test_documents.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,14 +727,15 @@
         source = os.path.join(self.test_dir, 'resources/pw/Al001_relax_bfgs.xml')
         document = PwDocument(source)
         stress = document.get_stress()
         self.assertIsNone(stress)
 
         source = os.path.join(self.test_dir, 'resources/pw/Si.xml')
         document = PwDocument(source)
+        self.assertIsNotNone(document.schema)
         stress = document.get_stress()
         self.assertListEqual(
             stress,
             [
                 [0.0001200028001026682, -3.388131789017201e-20, 1.355252715606881e-20],
                 [-3.388131789017201e-20, 0.0001200028001026682, -1.355252715606881e-20],
                 [6.776263578034403e-21, -6.776263578034403e-21, 0.0001200028001026683]
```

### Comparing `qeschema-1.5.1/tests/test_hdf5.py` & `qeschema-1.5.2/tests/test_hdf5.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_options.py` & `qeschema-1.5.2/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_upf.py` & `qeschema-1.5.2/tests/test_upf.py`

 * *Files identical despite different names*

### Comparing `qeschema-1.5.1/tests/test_utils.py` & `qeschema-1.5.2/tests/test_utils.py`

 * *Files identical despite different names*

