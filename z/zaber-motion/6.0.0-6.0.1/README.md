# Comparing `tmp/zaber_motion-6.0.0.tar.gz` & `tmp/zaber_motion-6.0.1-py3-none-manylinux_2_27_armv7l.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zaber_motion-6.0.0.tar", last modified: Tue May 21 23:06:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

