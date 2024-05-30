# Comparing `tmp/taskbridge-0.1.2b0.tar.gz` & `tmp/taskbridge-0.1.2b1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskbridge-0.1.2b0.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

