# Comparing `tmp/upm - micro project manager-0.3.1.tar.gz` & `tmp/upm_micro_project_manager-0.4.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upm - micro project manager-0.3.1.tar", last modified: Tue Dec  6 10:10:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

