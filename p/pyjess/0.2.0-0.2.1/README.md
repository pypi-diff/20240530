# Comparing `tmp/pyjess-0.2.0.tar.gz` & `tmp/pyjess-0.2.1-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjess-0.2.0.tar", last modified: Fri May 24 14:27:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

