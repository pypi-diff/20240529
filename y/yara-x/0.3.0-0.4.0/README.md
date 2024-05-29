# Comparing `tmp/yara_x-0.3.0.tar.gz` & `tmp/yara_x-0.4.0-pp38-pypy38_pp73-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

