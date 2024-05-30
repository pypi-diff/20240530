# Comparing `tmp/pystac_client-0.8.1.tar.gz` & `tmp/pystac_client-0.8.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac_client-0.8.1.tar", last modified: Thu May 23 14:51:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

