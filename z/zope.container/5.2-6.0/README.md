# Comparing `tmp/zope.container-5.2.tar.gz` & `tmp/zope.container-6.0-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.container-5.2.tar", last modified: Fri Oct  6 05:31:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

