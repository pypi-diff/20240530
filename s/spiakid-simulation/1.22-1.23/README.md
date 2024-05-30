# Comparing `tmp/spiakid_simulation-1.22.tar.gz` & `tmp/spiakid_simulation-1.23-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spiakid_simulation-1.22.tar", last modified: Thu May 16 12:51:41 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

