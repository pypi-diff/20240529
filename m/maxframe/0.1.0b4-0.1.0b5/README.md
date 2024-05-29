# Comparing `tmp/maxframe-0.1.0b4.tar.gz` & `tmp/maxframe-0.1.0b5-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxframe-0.1.0b4.tar", last modified: Tue Apr 23 08:34:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

