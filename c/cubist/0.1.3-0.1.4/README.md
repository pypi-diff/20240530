# Comparing `tmp/cubist-0.1.3.tar.gz` & `tmp/cubist-0.1.4-cp38-cp38-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubist-0.1.3.tar", last modified: Thu Mar 21 02:34:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

