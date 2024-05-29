# Comparing `tmp/nnef-1.0.4.tar.gz` & `tmp/nnef-1.0.5-cp38-cp38-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnef-1.0.4.tar", last modified: Fri May 24 13:22:05 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

