# Comparing `tmp/plone_app_contenttypes-3.0.7.tar.gz` & `tmp/plone_app_contenttypes-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone_app_contenttypes-3.0.7.tar", last modified: Thu Apr 25 19:34:07 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

