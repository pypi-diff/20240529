# Comparing `tmp/bigsansar-2.6.5.tar.gz` & `tmp/Bigsansar-2.6.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bigsansar-2.6.5.tar", last modified: Sun May 12 07:44:09 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

