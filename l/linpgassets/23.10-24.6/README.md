# Comparing `tmp/linpgassets-23.10.tar.gz` & `tmp/linpgassets-24.6-cp312-cp312-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linpgassets-23.10.tar", last modified: Thu Oct 26 19:35:04 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

