# Comparing `tmp/loopies-scraper-0.0.5.tar.gz` & `tmp/loopies_scraper-0.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopies-scraper-0.0.5.tar", last modified: Tue May 21 20:12:19 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

