# Comparing `tmp/sora_sdk-2024.3.0.dev3.tar.gz` & `tmp/sora_sdk-2024.3.0.dev4-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sora_sdk-2024.3.0.dev3.tar", last modified: Tue May 28 08:20:40 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

