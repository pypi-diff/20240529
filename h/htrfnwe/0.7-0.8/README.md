# Comparing `tmp/htrfnwe-0.7.tar.gz` & `tmp/htrfnwe-0.8-cp37-cp37m-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/htrfnwe-0.7.tar", last modified: Thu May 23 08:19:28 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

