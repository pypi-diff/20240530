# Comparing `tmp/bcqa-1.0.7.tar.gz` & `tmp/bcqa-1.0.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcqa-1.0.7.tar", last modified: Thu May 30 19:09:54 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

