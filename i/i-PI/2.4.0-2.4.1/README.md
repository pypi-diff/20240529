# Comparing `tmp/i-PI-2.4.0.tar.gz` & `tmp/i_PI-2.4.1-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i-PI-2.4.0.tar", last modified: Fri Mar 19 12:37:28 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

