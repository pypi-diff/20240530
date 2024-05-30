# Comparing `tmp/centercitypcs_utils-0.2.5.tar.gz` & `tmp/centercitypcs_utils-0.2.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centercitypcs_utils-0.2.5.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

