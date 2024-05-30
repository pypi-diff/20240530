# Comparing `tmp/azizkitten-11.2.0.tar.gz` & `tmp/AzizKitten-11.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azizkitten-11.2.0.tar", last modified: Sat May 25 15:42:04 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

