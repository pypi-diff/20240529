# Comparing `tmp/onchainpay_api-0.0.3.tar.gz` & `tmp/onchainpay_api-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/onchainpay_api-0.0.3.tar", last modified: Tue May 28 09:43:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

