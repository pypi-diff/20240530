# Comparing `tmp/manifestly-0.2.2.tar.gz` & `tmp/manifestly-0.2.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manifestly-0.2.2.tar", last modified: Thu May 30 19:49:26 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

