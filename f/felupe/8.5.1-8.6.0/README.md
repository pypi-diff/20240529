# Comparing `tmp/felupe-8.5.1.tar.gz` & `tmp/felupe-8.6.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "felupe-8.5.1.tar", last modified: Wed May  8 14:42:00 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

