# Comparing `tmp/kcli-99.0.202405291755.tar.gz` & `tmp/kcli-99.0.202405291925-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kcli-99.0.202405291755.tar", last modified: Wed May 29 17:55:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

