# Comparing `tmp/dataos-pyflare-0.1.6.tar.gz` & `tmp/dataos_pyflare-0.1.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/mayanksharma/workspace/modern/dataos_pyspark_sdk/dist/.tmp-emq9zexm/dataos-pyflare-0.1.6.tar", last modified: Tue Jan  2 12:46:58 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

