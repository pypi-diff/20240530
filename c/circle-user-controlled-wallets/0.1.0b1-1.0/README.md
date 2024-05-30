# Comparing `tmp/circle_user_controlled_wallets-0.1.0b1.tar.gz` & `tmp/circle_user_controlled_wallets-1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circle_user_controlled_wallets-0.1.0b1.tar", last modified: Fri May 24 20:25:14 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

