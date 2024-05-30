# Comparing `tmp/primerforge-1.0.2.tar.gz` & `tmp/primerforge-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primerforge-1.0.2.tar", last modified: Mon Apr 22 20:05:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

