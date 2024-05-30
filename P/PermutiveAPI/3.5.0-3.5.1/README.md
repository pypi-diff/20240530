# Comparing `tmp/PermutiveAPI-3.5.0.tar.gz` & `tmp/PermutiveAPI-3.5.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PermutiveAPI-3.5.0.tar", last modified: Mon Feb 26 15:09:31 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

