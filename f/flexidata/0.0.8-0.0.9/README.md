# Comparing `tmp/flexidata-0.0.8.tar.gz` & `tmp/flexidata-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexidata-0.0.8.tar", last modified: Wed May 29 20:19:50 2024, max compression
+gzip compressed data, was "flexidata-0.0.9.tar", last modified: Thu May 30 14:34:37 2024, max compression
```

## Comparing `flexidata-0.0.8.tar` & `flexidata-0.0.9.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/
--rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    16451 2024-05-29 20:19:50.323192 flexidata-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.231415 flexidata-0.0.8/examples/
--rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.8/examples/__init__.py
--rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.8/examples/run.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.233414 flexidata-0.0.8/flexidata/
--rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.8/flexidata/Logger.py
--rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.8/flexidata/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.262797 flexidata-0.0.8/flexidata/models/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.8/flexidata/models/__init__.py
--rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.8/flexidata/models/base.py
--rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.8/flexidata/models/detectron2.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.274170 flexidata-0.0.8/flexidata/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.8/flexidata/ocr/__init__.py
--rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.8/flexidata/ocr/agent.py
--rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.8/flexidata/ocr/google_vision.py
--rw-rw-rw-   0        0        0     6251 2024-05-29 17:31:51.000000 flexidata-0.0.8/flexidata/ocr/paddle.py
--rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.8/flexidata/ocr/tesseract.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.290571 flexidata-0.0.8/flexidata/parser/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.8/flexidata/parser/__init__.py
--rw-rw-rw-   0        0        0     2852 2024-05-29 16:41:38.000000 flexidata-0.0.8/flexidata/parser/doc.py
--rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.8/flexidata/parser/document.py
--rw-rw-rw-   0        0        0    11056 2024-05-29 20:14:24.000000 flexidata-0.0.8/flexidata/parser/docx.py
--rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.8/flexidata/parser/epub.py
--rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.8/flexidata/parser/html.py
--rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.8/flexidata/parser/image.py
--rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.8/flexidata/parser/md.py
--rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.8/flexidata/parser/odt.py
--rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.8/flexidata/parser/org.py
--rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.8/flexidata/parser/pdf.py
--rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.8/flexidata/parser/pptx.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.8/flexidata/parser/rst.py
--rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.8/flexidata/parser/rtf.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.290571 flexidata-0.0.8/flexidata/preprocessor/
--rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.8/flexidata/preprocessor/__init__.py
--rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.8/flexidata/preprocessor/base.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.306553 flexidata-0.0.8/flexidata/reader/
--rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.8/flexidata/reader/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.8/flexidata/reader/factory.py
--rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.8/flexidata/reader/file_reader.py
--rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.8/flexidata/reader/google_drive.py
--rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.8/flexidata/reader/handlers.py
--rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.8/flexidata/reader/local.py
--rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.8/flexidata/reader/s3.py
--rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.8/flexidata/reader/web.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.306553 flexidata-0.0.8/flexidata/text_processing/
--rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.8/flexidata/text_processing/__init__.py
--rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.8/flexidata/text_processing/classification.py
--rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.8/flexidata/text_processing/convert_file.py
--rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.8/flexidata/text_processing/text_block.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/flexidata/utils/
--rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.8/flexidata/utils/__init__.py
--rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.8/flexidata/utils/common.py
--rw-rw-rw-   0        0        0     5510 2024-05-29 20:10:38.000000 flexidata-0.0.8/flexidata/utils/constants.py
--rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.8/flexidata/utils/decorators.py
--rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.8/flexidata/utils/pdf.py
--rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.8/flexidata/utils/text.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/flexidata.egg-info/
--rw-rw-rw-   0        0        0    16451 2024-05-29 20:19:50.000000 flexidata-0.0.8/flexidata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1609 2024-05-29 20:19:50.000000 flexidata-0.0.8/flexidata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 20:19:50.000000 flexidata-0.0.8/flexidata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      541 2024-05-29 20:19:50.000000 flexidata-0.0.8/flexidata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2024-05-29 20:19:50.000000 flexidata-0.0.8/flexidata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      799 2024-05-29 20:19:19.000000 flexidata-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 20:19:50.323192 flexidata-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/tests/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.8/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/tests/ocr/
--rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.8/tests/ocr/__init__.py
--rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.8/tests/ocr/test_agent.py
-drwxrwxrwx   0        0        0        0 2024-05-29 20:19:50.323192 flexidata-0.0.8/tests/utils/
--rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.8/tests/utils/__init__.py
--rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.8/tests/utils/test_common.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.558990 flexidata-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-05-01 19:03:09.000000 flexidata-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-17 18:22:13.000000 flexidata-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    16451 2024-05-30 14:34:37.556346 flexidata-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-05-23 17:24:07.000000 flexidata-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.465622 flexidata-0.0.9/examples/
+-rw-rw-rw-   0        0        0        0 2024-05-24 13:32:36.000000 flexidata-0.0.9/examples/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-05-24 13:40:12.000000 flexidata-0.0.9/examples/run.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.467621 flexidata-0.0.9/flexidata/
+-rw-rw-rw-   0        0        0     1838 2024-05-05 15:00:12.000000 flexidata-0.0.9/flexidata/Logger.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 08:52:21.000000 flexidata-0.0.9/flexidata/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.489330 flexidata-0.0.9/flexidata/config/
+-rw-rw-rw-   0        0        0        0 2024-05-30 14:32:56.000000 flexidata-0.0.9/flexidata/config/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-05-12 06:59:05.000000 flexidata-0.0.9/flexidata/config/config.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.489330 flexidata-0.0.9/flexidata/models/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:01:08.000000 flexidata-0.0.9/flexidata/models/__init__.py
+-rw-rw-rw-   0        0        0      562 2024-05-02 08:41:23.000000 flexidata-0.0.9/flexidata/models/base.py
+-rw-rw-rw-   0        0        0     3117 2024-05-02 08:39:53.000000 flexidata-0.0.9/flexidata/models/detectron2.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.503838 flexidata-0.0.9/flexidata/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:25.000000 flexidata-0.0.9/flexidata/ocr/__init__.py
+-rw-rw-rw-   0        0        0     2141 2024-05-20 17:02:29.000000 flexidata-0.0.9/flexidata/ocr/agent.py
+-rw-rw-rw-   0        0        0     4692 2024-05-20 16:54:30.000000 flexidata-0.0.9/flexidata/ocr/google_vision.py
+-rw-rw-rw-   0        0        0     6251 2024-05-29 17:31:51.000000 flexidata-0.0.9/flexidata/ocr/paddle.py
+-rw-rw-rw-   0        0        0     4119 2024-05-20 16:51:15.000000 flexidata-0.0.9/flexidata/ocr/tesseract.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.519483 flexidata-0.0.9/flexidata/parser/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:51.000000 flexidata-0.0.9/flexidata/parser/__init__.py
+-rw-rw-rw-   0        0        0     2927 2024-05-30 14:19:00.000000 flexidata-0.0.9/flexidata/parser/doc.py
+-rw-rw-rw-   0        0        0     6605 2024-05-29 15:32:56.000000 flexidata-0.0.9/flexidata/parser/document.py
+-rw-rw-rw-   0        0        0    11281 2024-05-30 14:19:36.000000 flexidata-0.0.9/flexidata/parser/docx.py
+-rw-rw-rw-   0        0        0     3299 2024-05-25 16:05:03.000000 flexidata-0.0.9/flexidata/parser/epub.py
+-rw-rw-rw-   0        0        0    16674 2024-05-24 07:55:28.000000 flexidata-0.0.9/flexidata/parser/html.py
+-rw-rw-rw-   0        0        0     3557 2024-05-23 17:55:38.000000 flexidata-0.0.9/flexidata/parser/image.py
+-rw-rw-rw-   0        0        0     3117 2024-05-25 16:05:03.000000 flexidata-0.0.9/flexidata/parser/md.py
+-rw-rw-rw-   0        0        0     2813 2024-05-25 16:03:16.000000 flexidata-0.0.9/flexidata/parser/odt.py
+-rw-rw-rw-   0        0        0     3289 2024-05-25 16:15:35.000000 flexidata-0.0.9/flexidata/parser/org.py
+-rw-rw-rw-   0        0        0    23691 2024-05-25 16:05:03.000000 flexidata-0.0.9/flexidata/parser/pdf.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 07:08:45.000000 flexidata-0.0.9/flexidata/parser/pptx.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.9/flexidata/parser/rst.py
+-rw-rw-rw-   0        0        0     3283 2024-05-25 16:05:03.000000 flexidata-0.0.9/flexidata/parser/rtf.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.519483 flexidata-0.0.9/flexidata/preprocessor/
+-rw-rw-rw-   0        0        0        0 2024-05-20 14:04:01.000000 flexidata-0.0.9/flexidata/preprocessor/__init__.py
+-rw-rw-rw-   0        0        0     4776 2024-05-20 18:39:57.000000 flexidata-0.0.9/flexidata/preprocessor/base.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.519483 flexidata-0.0.9/flexidata/reader/
+-rw-rw-rw-   0        0        0        0 2024-05-18 19:45:52.000000 flexidata-0.0.9/flexidata/reader/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-05-25 16:28:25.000000 flexidata-0.0.9/flexidata/reader/factory.py
+-rw-rw-rw-   0        0        0     1375 2024-05-25 16:30:14.000000 flexidata-0.0.9/flexidata/reader/file_reader.py
+-rw-rw-rw-   0        0        0     2087 2024-05-25 16:32:02.000000 flexidata-0.0.9/flexidata/reader/google_drive.py
+-rw-rw-rw-   0        0        0    11869 2024-05-29 16:41:34.000000 flexidata-0.0.9/flexidata/reader/handlers.py
+-rw-rw-rw-   0        0        0     2024 2024-05-25 16:33:01.000000 flexidata-0.0.9/flexidata/reader/local.py
+-rw-rw-rw-   0        0        0     2588 2024-05-25 16:34:34.000000 flexidata-0.0.9/flexidata/reader/s3.py
+-rw-rw-rw-   0        0        0     2102 2024-05-25 16:36:23.000000 flexidata-0.0.9/flexidata/reader/web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.532421 flexidata-0.0.9/flexidata/text_processing/
+-rw-rw-rw-   0        0        0        0 2024-05-20 16:07:28.000000 flexidata-0.0.9/flexidata/text_processing/__init__.py
+-rw-rw-rw-   0        0        0    18502 2024-05-25 16:52:41.000000 flexidata-0.0.9/flexidata/text_processing/classification.py
+-rw-rw-rw-   0        0        0     4700 2024-05-29 16:18:43.000000 flexidata-0.0.9/flexidata/text_processing/convert_file.py
+-rw-rw-rw-   0        0        0     5583 2024-05-25 16:58:06.000000 flexidata-0.0.9/flexidata/text_processing/text_block.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.544493 flexidata-0.0.9/flexidata/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-02 06:00:39.000000 flexidata-0.0.9/flexidata/utils/__init__.py
+-rw-rw-rw-   0        0        0     1316 2024-05-25 16:59:21.000000 flexidata-0.0.9/flexidata/utils/common.py
+-rw-rw-rw-   0        0        0     5510 2024-05-29 20:10:38.000000 flexidata-0.0.9/flexidata/utils/constants.py
+-rw-rw-rw-   0        0        0     4344 2024-05-25 17:02:07.000000 flexidata-0.0.9/flexidata/utils/decorators.py
+-rw-rw-rw-   0        0        0     4083 2024-05-25 17:10:18.000000 flexidata-0.0.9/flexidata/utils/pdf.py
+-rw-rw-rw-   0        0        0     1586 2024-05-25 17:05:01.000000 flexidata-0.0.9/flexidata/utils/text.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.544493 flexidata-0.0.9/flexidata.egg-info/
+-rw-rw-rw-   0        0        0    16451 2024-05-30 14:34:37.000000 flexidata-0.0.9/flexidata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1665 2024-05-30 14:34:37.000000 flexidata-0.0.9/flexidata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 14:34:37.000000 flexidata-0.0.9/flexidata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      541 2024-05-30 14:34:37.000000 flexidata-0.0.9/flexidata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2024-05-30 14:34:37.000000 flexidata-0.0.9/flexidata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      799 2024-05-30 14:33:37.000000 flexidata-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      571 2024-05-23 17:06:15.000000 flexidata-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 14:34:37.559485 flexidata-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      360 2024-05-17 18:24:25.000000 flexidata-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.544493 flexidata-0.0.9/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:55:43.000000 flexidata-0.0.9/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.544493 flexidata-0.0.9/tests/ocr/
+-rw-rw-rw-   0        0        0        0 2024-05-24 06:46:08.000000 flexidata-0.0.9/tests/ocr/__init__.py
+-rw-rw-rw-   0        0        0      935 2024-05-24 06:51:56.000000 flexidata-0.0.9/tests/ocr/test_agent.py
+drwxrwxrwx   0        0        0        0 2024-05-30 14:34:37.544493 flexidata-0.0.9/tests/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 18:25:44.000000 flexidata-0.0.9/tests/utils/__init__.py
+-rw-rw-rw-   0        0        0      324 2024-05-23 18:39:43.000000 flexidata-0.0.9/tests/utils/test_common.py
```

### Comparing `flexidata-0.0.8/LICENSE` & `flexidata-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/PKG-INFO` & `flexidata-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.8
+Version: 0.0.9
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.8/README.md` & `flexidata-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/Logger.py` & `flexidata-0.0.9/flexidata/Logger.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/models/base.py` & `flexidata-0.0.9/flexidata/models/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/models/detectron2.py` & `flexidata-0.0.9/flexidata/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/ocr/agent.py` & `flexidata-0.0.9/flexidata/ocr/agent.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/ocr/google_vision.py` & `flexidata-0.0.9/flexidata/ocr/google_vision.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/ocr/paddle.py` & `flexidata-0.0.9/flexidata/ocr/paddle.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/ocr/tesseract.py` & `flexidata-0.0.9/flexidata/ocr/tesseract.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/doc.py` & `flexidata-0.0.9/flexidata/parser/doc.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
     @validate_file_type_method([FileType.DOC])
     def parse(self, extract_image: bool = False) -> List[TextBlock]:
         """Parse the Doc file to extract text and possibly tables.
 
         Returns:
             List[TextBlock]: A list of TextBlock objects containing the extracted data.
         """
+        if extract_image:
+            self.extract_image = extract_image
         temp_directory = self._create_temp_directory()
         FileConversion.convet_doc_to_docx(self.file_path, temp_directory.name)
         _, filename_no_path = os.path.split(os.path.abspath(self.file_path))
         base_filename, _ = os.path.splitext(filename_no_path)
         target_file_path = os.path.join(temp_directory.name, f"{base_filename}.docx")
         parser = DocxParser(
             file_path=target_file_path,
```

### Comparing `flexidata-0.0.8/flexidata/parser/document.py` & `flexidata-0.0.9/flexidata/parser/document.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/docx.py` & `flexidata-0.0.9/flexidata/parser/docx.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from flexidata.utils.decorators import validate_file_type_method
 import re
 from os.path import basename
 import numpy as np
 from PIL import Image
 import io
 
+
 class DocxParser(FileHandler):
     """Initialize the DocxParser with file handling and parsing options.
 
     Args:
         file_path (Optional[str]): Local path to the file, if the source is local.
         file_url (Optional[str]): URL of the file, if the source is a web URL.
         source (FileReaderSource): Type of file source.
@@ -48,14 +49,16 @@
     @validate_file_type_method([FileType.DOCX])
     def parse(self, extract_image: bool = False) -> List[TextBlock]:
         """Parse the DOCX file to extract text and possibly tables.
 
         Returns:
             List[TextBlock]: A list of TextBlock objects containing the extracted data.
         """
+        if extract_image:
+            self.extract_image = extract_image
         document = docx.Document(cast(BinaryIO, self.get_file_content()))
         page_number = 1
         text_blocks = []
         table_index = 0
         for element in document.element.body:
             if element.tag.endswith("tbl") and self.extract_table:
                 table = document.tables[table_index]
@@ -71,15 +74,16 @@
                     extraction_source="docx",
                 )
                 text_block = TextBlock(text_table, metadata, TextType.TABLES)
                 text_blocks.append(text_block)
                 self._process_inner_table(table, page_number, text_blocks, document)
             if element.tag.endswith("p"):
                 paragraph = docx.text.paragraph.Paragraph(element, document)
-                image_texts = self._process_image(paragraph, document)
+                if self.extract_image:
+                    image_texts = self._process_image(paragraph, document)
                 if len(paragraph.text.strip()):
                     metadata = TextBlockMetadata(
                         file_path=self.get_file_path_by_source(),
                         languages=["eng"],
                         filetype=FileType.DOCX,
                         page_number=page_number,
                         extraction_source="docx",
@@ -168,21 +172,22 @@
                             page_number=page_number,
                             extraction_source="docx",
                         )
                         text_block = TextBlock(
                             text_inner_table, metadata, TextType.TABLES
                         )
                         text_blocks.append(text_block)
-                        self._process_inner_table(item, page_number, text_blocks, document)
+                        self._process_inner_table(
+                            item, page_number, text_blocks, document
+                        )
                     else:
-                        image_texts = self._process_image(item, document)
-                        text_blocks.extend(image_texts)
-                        
-                        
-    
+                        if self.extract_image:
+                            image_texts = self._process_image(item, document)
+                            text_blocks.extend(image_texts)
+
     def _process_image(self, paragraph: Any, document: Any) -> List[TextBlock]:
         """
         Extracts and processes image data embedded in a document paragraph, performing OCR on images.
 
         This method iterates over each run in the paragraph, searching for runs that contain references to images
         (denoted by empty text and specific content IDs). It retrieves the image data from the document's related parts,
         checks if the content type is an image (excluding specific types like 'image/x-wmf'), and uses OCR to convert
@@ -197,28 +202,30 @@
 
         Note:
             This function can potentially raise a KeyError if an image reference cannot be found within the document's parts.
             This function uses a predefined regex pattern, Patterns.DOCX_IMAGE_PATTERN, to locate image references in the XML.
         """
         image_texts = []
         for run in paragraph.runs:
-            if run.text == '':
+            if run.text == "":
                 try:
-                    contentID = Patterns.DOCX_IMAGE_PATTERN.search(run.element.xml).group(0)
+                    contentID = Patterns.DOCX_IMAGE_PATTERN.search(
+                        run.element.xml
+                    ).group(0)
                     contentType = document.part.related_parts[contentID].content_type
                 except KeyError as e:
                     print(e)
                     continue
                 except:
                     continue
-                if not contentType.startswith('image'):
+                if not contentType.startswith("image"):
                     continue
                 imgName = basename(document.part.related_parts[contentID].partname)
                 imgData = document.part.related_parts[contentID].blob
-                if contentType != 'image/x-wmf':
+                if contentType != "image/x-wmf":
                     image = np.array(Image.open(io.BytesIO(imgData)))
                     ocr_factory = OCRAgentFactory()
                     ocr_agent = ocr_factory.get_ocr_agent()
                     elements = ocr_agent.image_to_text(
                         np.array(image),
                         lang="eng",
                         page_number=1,
```

### Comparing `flexidata-0.0.8/flexidata/parser/epub.py` & `flexidata-0.0.9/flexidata/parser/epub.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/html.py` & `flexidata-0.0.9/flexidata/parser/html.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/image.py` & `flexidata-0.0.9/flexidata/parser/image.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/md.py` & `flexidata-0.0.9/flexidata/parser/md.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/odt.py` & `flexidata-0.0.9/flexidata/parser/odt.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/org.py` & `flexidata-0.0.9/flexidata/parser/org.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/pdf.py` & `flexidata-0.0.9/flexidata/parser/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/rst.py` & `flexidata-0.0.9/flexidata/parser/rst.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/parser/rtf.py` & `flexidata-0.0.9/flexidata/parser/rtf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/preprocessor/base.py` & `flexidata-0.0.9/flexidata/preprocessor/base.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/factory.py` & `flexidata-0.0.9/flexidata/reader/factory.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/file_reader.py` & `flexidata-0.0.9/flexidata/reader/file_reader.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/google_drive.py` & `flexidata-0.0.9/flexidata/reader/google_drive.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/handlers.py` & `flexidata-0.0.9/flexidata/reader/handlers.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/local.py` & `flexidata-0.0.9/flexidata/reader/local.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/s3.py` & `flexidata-0.0.9/flexidata/reader/s3.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/reader/web.py` & `flexidata-0.0.9/flexidata/reader/web.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/text_processing/classification.py` & `flexidata-0.0.9/flexidata/text_processing/classification.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/text_processing/convert_file.py` & `flexidata-0.0.9/flexidata/text_processing/convert_file.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/text_processing/text_block.py` & `flexidata-0.0.9/flexidata/text_processing/text_block.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/utils/common.py` & `flexidata-0.0.9/flexidata/utils/common.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/utils/constants.py` & `flexidata-0.0.9/flexidata/utils/constants.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/utils/decorators.py` & `flexidata-0.0.9/flexidata/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/utils/pdf.py` & `flexidata-0.0.9/flexidata/utils/pdf.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata/utils/text.py` & `flexidata-0.0.9/flexidata/utils/text.py`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/flexidata.egg-info/PKG-INFO` & `flexidata-0.0.9/flexidata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexidata
-Version: 0.0.8
+Version: 0.0.9
 Summary: FlexiData is an open-source Python package designed for processing unstructured data.
 Author-email: Kalyanakannan Padivasu <Kalyanakannan.p@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `flexidata-0.0.8/flexidata.egg-info/SOURCES.txt` & `flexidata-0.0.9/flexidata.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 flexidata/Logger.py
 flexidata/__init__.py
 flexidata.egg-info/PKG-INFO
 flexidata.egg-info/SOURCES.txt
 flexidata.egg-info/dependency_links.txt
 flexidata.egg-info/requires.txt
 flexidata.egg-info/top_level.txt
+flexidata/config/__init__.py
+flexidata/config/config.py
 flexidata/models/__init__.py
 flexidata/models/base.py
 flexidata/models/detectron2.py
 flexidata/ocr/__init__.py
 flexidata/ocr/agent.py
 flexidata/ocr/google_vision.py
 flexidata/ocr/paddle.py
```

### Comparing `flexidata-0.0.8/flexidata.egg-info/requires.txt` & `flexidata-0.0.9/flexidata.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/pyproject.toml` & `flexidata-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "flexidata"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Kalyanakannan Padivasu", email="Kalyanakannan.p@gmail.com" },
 ]
 description = "FlexiData is an open-source Python package designed for processing unstructured data."
 readme = "README.md"
 license = { file = "LICENSE" }
 keywords = ["PDF,DOCX document parsing"]
```

### Comparing `flexidata-0.0.8/requirements.txt` & `flexidata-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `flexidata-0.0.8/tests/ocr/test_agent.py` & `flexidata-0.0.9/tests/ocr/test_agent.py`

 * *Files identical despite different names*

