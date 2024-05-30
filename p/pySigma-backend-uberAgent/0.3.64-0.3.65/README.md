# Comparing `tmp/pysigma_backend_uberagent-0.3.64.tar.gz` & `tmp/pysigma_backend_uberagent-0.3.65-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysigma_backend_uberagent-0.3.64.tar", max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

