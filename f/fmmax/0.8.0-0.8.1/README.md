# Comparing `tmp/fmmax-0.8.0.tar.gz` & `tmp/fmmax-0.8.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmmax-0.8.0.tar", last modified: Fri Mar 29 19:37:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

