# Comparing `tmp/simpleaug-0.0.2.1.tar.gz` & `tmp/SimpleAUG-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaug-0.0.2.1.tar", last modified: Wed May 29 09:15:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

