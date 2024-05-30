# Comparing `tmp/streamlit-deephaven-0.0.6.tar.gz` & `tmp/streamlit_deephaven-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deephaven-0.0.6.tar", last modified: Tue May 28 19:50:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

