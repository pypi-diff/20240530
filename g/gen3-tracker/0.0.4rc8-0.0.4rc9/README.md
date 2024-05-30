# Comparing `tmp/gen3_tracker-0.0.4rc8.tar.gz` & `tmp/gen3_tracker-0.0.4rc9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_tracker-0.0.4rc8.tar", last modified: Sat May 25 13:55:30 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

