# Comparing `tmp/django_formset-1.4.4.tar.gz` & `tmp/django_formset-1.4.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_formset-1.4.4.tar", last modified: Mon May 13 09:49:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

