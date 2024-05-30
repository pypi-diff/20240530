# Comparing `tmp/trafilatura-1.8.1.tar.gz` & `tmp/trafilatura-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trafilatura-1.8.1.tar", last modified: Wed Apr  3 11:42:46 2024, max compression
+gzip compressed data, was "trafilatura-1.9.0.tar", last modified: Thu May  2 10:13:42 2024, max compression
```

## Comparing `trafilatura-1.8.1.tar` & `trafilatura-1.9.0.tar`

### file list

```diff
@@ -1,134 +1,135 @@
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      796 2021-11-18 18:20:49.000000 trafilatura-1.8.1/CITATION.cff
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2129 2024-01-08 12:50:38.000000 trafilatura-1.8.1/CONTRIBUTING.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    13253 2024-04-03 11:38:12.000000 trafilatura-1.8.1/HISTORY.md
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-03-20 15:18:48.000000 trafilatura-1.8.1/LICENSE
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      489 2022-03-07 11:15:49.000000 trafilatura-1.8.1/MANIFEST.in
--rw-r--r--   0 adbar     (1000) adbar     (1000)    14947 2024-04-03 11:42:46.360365 trafilatura-1.8.1/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    11790 2024-03-20 15:18:48.000000 trafilatura-1.8.1/README.rst
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      634 2019-12-24 15:36:05.000000 trafilatura-1.8.1/docs/Makefile
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.348357 trafilatura-1.8.1/docs/_build/
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/_build/_images/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-count-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/_build/_images/dwds-treffer-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.1/docs/_build/_images/gui-screenshot.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.1/docs/_build/_images/software-ecosystem.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.1/docs/_build/_images/trafilatura-demo.gif
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/docs/_build/_static/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      286 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/file.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/minus.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2023-11-29 13:26:25.000000 trafilatura-1.8.1/docs/_build/_static/plus.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.1/docs/_build/_static/trafilatura-logo.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      285 2022-01-28 19:17:06.000000 trafilatura-1.8.1/docs/background.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    24721 2023-04-13 12:18:08.000000 trafilatura-1.8.1/docs/compendium.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4385 2024-01-08 14:28:11.000000 trafilatura-1.8.1/docs/conf.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1822 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/corefunctions.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3407 2022-01-13 18:52:09.000000 trafilatura-1.8.1/docs/corpus-data.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8180 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/crawls.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10317 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/downloads.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-count-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.8.1/docs/dwds-treffer-exportieren.jpg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16498 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/evaluation.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.8.1/docs/gui-screenshot.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9504 2024-03-20 15:18:48.000000 trafilatura-1.8.1/docs/index.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2740 2021-11-29 16:07:30.000000 trafilatura-1.8.1/docs/installation-gui.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5972 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/installation.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      795 2019-12-24 15:36:05.000000 trafilatura-1.8.1/docs/make.bat
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2608 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/quickstart.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      139 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/requirements.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5735 2024-01-08 12:50:38.000000 trafilatura-1.8.1/docs/settings.rst
--rw-------   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.8.1/docs/software-ecosystem.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10299 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/sources.rst
--rw-r--r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.8.1/docs/trafilatura-demo.gif
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.8.1/docs/trafilatura-logo.png
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4975 2024-03-25 12:40:36.000000 trafilatura-1.8.1/docs/troubleshooting.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7978 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial-dwds.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5416 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/tutorial-epsilla.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    10881 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial0.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4662 2023-11-08 15:59:34.000000 trafilatura-1.8.1/docs/tutorial1.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1447 2023-04-13 12:18:08.000000 trafilatura-1.8.1/docs/tutorial2.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2668 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/tutorials.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3782 2023-11-03 16:02:12.000000 trafilatura-1.8.1/docs/url-management.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2031 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-api.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    15049 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-cli.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      835 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-gui.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    14853 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-python.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     5697 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/usage-r.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      196 2024-01-25 12:45:59.000000 trafilatura-1.8.1/docs/usage.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16864 2024-02-27 12:25:00.000000 trafilatura-1.8.1/docs/used-by.rst
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-11-15 14:02:12.000000 trafilatura-1.8.1/pytest.ini
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-04-03 11:42:46.360365 trafilatura-1.8.1/setup.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4722 2024-04-02 17:40:04.000000 trafilatura-1.8.1/setup.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.352360 trafilatura-1.8.1/tests/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       84 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    20146 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/cli_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9187 2024-02-27 12:25:00.000000 trafilatura-1.8.1/tests/downloads_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9699 2023-12-15 15:05:15.000000 trafilatura-1.8.1/tests/feeds_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9834 2023-10-04 12:59:20.000000 trafilatura-1.8.1/tests/filters_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     1925 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/hashing_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    70093 2023-08-18 16:12:07.000000 trafilatura-1.8.1/tests/json_metadata_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    24025 2023-11-28 12:44:32.000000 trafilatura-1.8.1/tests/metadata_tests.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.356362 trafilatura-1.8.1/tests/resources/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7490 2021-11-08 11:56:03.000000 trafilatura-1.8.1/tests/resources/apache.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      416 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/exotic_tags.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      444 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/exotic_tags_tei.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    34299 2021-10-29 16:43:41.000000 trafilatura-1.8.1/tests/resources/feed.json
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      823 2020-12-22 14:28:05.000000 trafilatura-1.8.1/tests/resources/feed1.atom
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      668 2021-01-21 13:30:47.000000 trafilatura-1.8.1/tests/resources/feed2.rss
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4148 2023-01-04 17:43:29.000000 trafilatura-1.8.1/tests/resources/http_sample.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3741 2019-12-24 15:36:05.000000 trafilatura-1.8.1/tests/resources/httpbin_sample.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       93 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/list-discard.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       94 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/list-process.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      741 2023-10-24 14:50:14.000000 trafilatura-1.8.1/tests/resources/newsettings.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      154 2021-10-27 16:32:31.000000 trafilatura-1.8.1/tests/resources/redundant-urls.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    38705 2021-12-08 16:43:57.000000 trafilatura-1.8.1/tests/resources/scam.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     2056 2020-12-22 16:53:15.000000 trafilatura-1.8.1/tests/resources/sitemap-hreflang.xml
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8622 2020-09-25 15:03:42.000000 trafilatura-1.8.1/tests/resources/sitemap.xml
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      494 2020-11-27 17:14:37.000000 trafilatura-1.8.1/tests/resources/sitemap.xml.gz
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      397 2021-01-21 13:31:13.000000 trafilatura-1.8.1/tests/resources/sitemap2.xml
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    14388 2023-05-11 19:41:09.000000 trafilatura-1.8.1/tests/resources/utf8.html
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    23220 2021-10-27 11:17:58.000000 trafilatura-1.8.1/tests/resources/webpage.html.gz
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      725 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/resources/zerolength.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8437 2024-02-27 12:25:00.000000 trafilatura-1.8.1/tests/sitemaps_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     7725 2023-12-13 12:15:25.000000 trafilatura-1.8.1/tests/spider_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    67941 2024-04-02 17:40:04.000000 trafilatura-1.8.1/tests/unit_tests.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    20324 2024-01-24 17:14:34.000000 trafilatura-1.8.1/tests/xml_tei_tests.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.356362 trafilatura-1.8.1/trafilatura/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      608 2024-04-03 11:38:59.000000 trafilatura-1.8.1/trafilatura/__init__.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    13288 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/cli.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16486 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/cli_utils.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    50196 2024-04-02 17:55:15.000000 trafilatura-1.8.1/trafilatura/core.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/trafilatura/data/
--rw-rw-r--   0 adbar     (1000) adbar     (1000)   851312 2022-08-02 16:32:41.000000 trafilatura-1.8.1/trafilatura/data/jt-stopwords-pickle.lzma
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    80692 2022-08-02 16:32:41.000000 trafilatura-1.8.1/trafilatura/data/tei-schema-pickle.lzma
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    14538 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/downloads.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4943 2024-04-03 06:16:54.000000 trafilatura-1.8.1/trafilatura/external.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9664 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/feeds.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4917 2024-01-22 11:54:58.000000 trafilatura-1.8.1/trafilatura/filters.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     8103 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/gui.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4876 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/hashing.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    13435 2024-04-02 17:40:04.000000 trafilatura-1.8.1/trafilatura/htmlprocessing.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9844 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/json_metadata.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3671 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/lru.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      951 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/meta.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    21929 2024-02-27 12:25:00.000000 trafilatura-1.8.1/trafilatura/metadata.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     4359 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/metaxpaths.py
--rwxrwxr-x   0 adbar     (1000) adbar     (1000)    17877 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/readability_lxml.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      739 2024-02-05 15:30:45.000000 trafilatura-1.8.1/trafilatura/settings.cfg
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3130 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/settings.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9766 2024-03-20 15:18:48.000000 trafilatura-1.8.1/trafilatura/sitemaps.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     9013 2023-08-18 16:12:07.000000 trafilatura-1.8.1/trafilatura/spider.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    16004 2024-03-28 17:14:38.000000 trafilatura-1.8.1/trafilatura/utils.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    21940 2024-03-28 17:14:38.000000 trafilatura-1.8.1/trafilatura/xml.py
--rw-rw-r--   0 adbar     (1000) adbar     (1000)    11775 2024-04-03 11:34:41.000000 trafilatura-1.8.1/trafilatura/xpaths.py
-drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-04-03 11:42:46.360365 trafilatura-1.8.1/trafilatura.egg-info/
--rw-r--r--   0 adbar     (1000) adbar     (1000)    14947 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/PKG-INFO
--rw-rw-r--   0 adbar     (1000) adbar     (1000)     3075 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/SOURCES.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/dependency_links.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       92 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/entry_points.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/not-zip-safe
--rw-rw-r--   0 adbar     (1000) adbar     (1000)      581 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/requires.txt
--rw-rw-r--   0 adbar     (1000) adbar     (1000)       12 2024-04-03 11:42:46.000000 trafilatura-1.8.1/trafilatura.egg-info/top_level.txt
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.061855 trafilatura-1.9.0/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      796 2021-11-18 18:20:49.000000 trafilatura-1.9.0/CITATION.cff
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2112 2024-04-08 16:09:42.000000 trafilatura-1.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14198 2024-05-02 10:10:41.000000 trafilatura-1.9.0/HISTORY.md
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10173 2024-04-08 16:09:42.000000 trafilatura-1.9.0/LICENSE
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      489 2022-03-07 11:15:49.000000 trafilatura-1.9.0/MANIFEST.in
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    14081 2024-05-02 10:13:42.061855 trafilatura-1.9.0/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10884 2024-04-23 11:00:58.000000 trafilatura-1.9.0/README.md
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.049855 trafilatura-1.9.0/docs/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      634 2019-12-24 15:36:05.000000 trafilatura-1.9.0/docs/Makefile
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.037855 trafilatura-1.9.0/docs/_build/
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.049855 trafilatura-1.9.0/docs/_build/_images/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/_build/_images/dwds-count-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/_build/_images/dwds-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/_build/_images/dwds-treffer-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.9.0/docs/_build/_images/gui-screenshot.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.9.0/docs/_build/_images/software-ecosystem.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.9.0/docs/_build/_images/trafilatura-demo.gif
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.053855 trafilatura-1.9.0/docs/_build/_static/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      286 2024-04-26 15:41:14.000000 trafilatura-1.9.0/docs/_build/_static/file.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2024-04-26 15:41:14.000000 trafilatura-1.9.0/docs/_build/_static/minus.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       90 2024-04-26 15:41:14.000000 trafilatura-1.9.0/docs/_build/_static/plus.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.9.0/docs/_build/_static/trafilatura-logo.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      285 2022-01-28 19:17:06.000000 trafilatura-1.9.0/docs/background.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    24721 2023-04-13 12:18:08.000000 trafilatura-1.9.0/docs/compendium.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4418 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/conf.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1822 2024-04-08 10:32:42.000000 trafilatura-1.9.0/docs/corefunctions.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3407 2022-01-13 18:52:09.000000 trafilatura-1.9.0/docs/corpus-data.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9042 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/crawls.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10317 2024-01-25 12:45:59.000000 trafilatura-1.9.0/docs/downloads.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   140162 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/dwds-count-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   108871 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/dwds-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   171519 2020-06-17 16:47:44.000000 trafilatura-1.9.0/docs/dwds-treffer-exportieren.jpg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16498 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/evaluation.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    75098 2021-01-08 16:52:37.000000 trafilatura-1.9.0/docs/gui-screenshot.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9504 2024-04-08 16:09:42.000000 trafilatura-1.9.0/docs/index.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2740 2021-11-29 16:07:30.000000 trafilatura-1.9.0/docs/installation-gui.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5972 2024-01-08 12:50:38.000000 trafilatura-1.9.0/docs/installation.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      795 2019-12-24 15:36:05.000000 trafilatura-1.9.0/docs/make.bat
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2608 2024-01-08 12:50:38.000000 trafilatura-1.9.0/docs/quickstart.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      139 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/requirements.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     6012 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/settings.rst
+-rw-------   0 adbar     (1000) adbar     (1000)    96837 2021-09-16 16:27:51.000000 trafilatura-1.9.0/docs/software-ecosystem.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10299 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/sources.rst
+-rw-r--r--   0 adbar     (1000) adbar     (1000)   816558 2020-01-17 15:42:23.000000 trafilatura-1.9.0/docs/trafilatura-demo.gif
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23420 2022-01-25 15:28:24.000000 trafilatura-1.9.0/docs/trafilatura-logo.png
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5463 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/troubleshooting.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7979 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/tutorial-dwds.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5416 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/tutorial-epsilla.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    10881 2023-11-08 15:59:34.000000 trafilatura-1.9.0/docs/tutorial0.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4662 2023-11-08 15:59:34.000000 trafilatura-1.9.0/docs/tutorial1.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1447 2023-04-13 12:18:08.000000 trafilatura-1.9.0/docs/tutorial2.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2668 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/tutorials.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3782 2023-11-03 16:02:12.000000 trafilatura-1.9.0/docs/url-management.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2031 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/usage-api.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16159 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/usage-cli.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      835 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/usage-gui.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    15727 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/usage-python.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     5697 2024-02-27 12:25:00.000000 trafilatura-1.9.0/docs/usage-r.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      196 2024-01-25 12:45:59.000000 trafilatura-1.9.0/docs/usage.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    18148 2024-04-30 11:35:39.000000 trafilatura-1.9.0/docs/used-by.rst
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       40 2021-11-15 14:02:12.000000 trafilatura-1.9.0/pytest.ini
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       38 2024-05-02 10:13:42.061855 trafilatura-1.9.0/setup.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4646 2024-05-02 10:00:01.000000 trafilatura-1.9.0/setup.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.053855 trafilatura-1.9.0/tests/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       84 2023-08-18 16:12:07.000000 trafilatura-1.9.0/tests/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    20793 2024-04-23 11:26:18.000000 trafilatura-1.9.0/tests/cli_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9299 2024-04-23 11:13:31.000000 trafilatura-1.9.0/tests/downloads_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9699 2023-12-15 15:05:15.000000 trafilatura-1.9.0/tests/feeds_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9804 2024-04-11 16:43:13.000000 trafilatura-1.9.0/tests/filters_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1925 2023-08-18 16:12:07.000000 trafilatura-1.9.0/tests/hashing_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    70093 2023-08-18 16:12:07.000000 trafilatura-1.9.0/tests/json_metadata_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    24402 2024-04-19 15:19:03.000000 trafilatura-1.9.0/tests/metadata_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.057855 trafilatura-1.9.0/tests/resources/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7490 2021-11-08 11:56:03.000000 trafilatura-1.9.0/tests/resources/apache.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      416 2019-12-24 15:36:05.000000 trafilatura-1.9.0/tests/resources/exotic_tags.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      444 2019-12-24 15:36:05.000000 trafilatura-1.9.0/tests/resources/exotic_tags_tei.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    34299 2021-10-29 16:43:41.000000 trafilatura-1.9.0/tests/resources/feed.json
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      823 2020-12-22 14:28:05.000000 trafilatura-1.9.0/tests/resources/feed1.atom
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      668 2021-01-21 13:30:47.000000 trafilatura-1.9.0/tests/resources/feed2.rss
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4148 2023-01-04 17:43:29.000000 trafilatura-1.9.0/tests/resources/http_sample.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3741 2019-12-24 15:36:05.000000 trafilatura-1.9.0/tests/resources/httpbin_sample.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       93 2023-05-11 19:41:09.000000 trafilatura-1.9.0/tests/resources/list-discard.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       94 2023-05-11 19:41:09.000000 trafilatura-1.9.0/tests/resources/list-process.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      741 2023-10-24 14:50:14.000000 trafilatura-1.9.0/tests/resources/newsettings.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      154 2021-10-27 16:32:31.000000 trafilatura-1.9.0/tests/resources/redundant-urls.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    38705 2021-12-08 16:43:57.000000 trafilatura-1.9.0/tests/resources/scam.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     2056 2020-12-22 16:53:15.000000 trafilatura-1.9.0/tests/resources/sitemap-hreflang.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8622 2020-09-25 15:03:42.000000 trafilatura-1.9.0/tests/resources/sitemap.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      494 2020-11-27 17:14:37.000000 trafilatura-1.9.0/tests/resources/sitemap.xml.gz
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      397 2021-01-21 13:31:13.000000 trafilatura-1.9.0/tests/resources/sitemap2.xml
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14388 2023-05-11 19:41:09.000000 trafilatura-1.9.0/tests/resources/utf8.html
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    23220 2021-10-27 11:17:58.000000 trafilatura-1.9.0/tests/resources/webpage.html.gz
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      725 2024-01-24 17:14:34.000000 trafilatura-1.9.0/tests/resources/zerolength.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     8437 2024-02-27 12:25:00.000000 trafilatura-1.9.0/tests/sitemaps_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7725 2023-12-13 12:15:25.000000 trafilatura-1.9.0/tests/spider_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    70497 2024-04-24 09:53:37.000000 trafilatura-1.9.0/tests/unit_tests.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    20324 2024-01-24 17:14:34.000000 trafilatura-1.9.0/tests/xml_tei_tests.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.061855 trafilatura-1.9.0/trafilatura/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      629 2024-05-02 09:57:39.000000 trafilatura-1.9.0/trafilatura/__init__.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3114 2024-04-22 14:03:24.000000 trafilatura-1.9.0/trafilatura/baseline.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13629 2024-04-19 15:19:03.000000 trafilatura-1.9.0/trafilatura/cli.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16019 2024-04-23 11:13:31.000000 trafilatura-1.9.0/trafilatura/cli_utils.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16261 2024-04-24 09:53:37.000000 trafilatura-1.9.0/trafilatura/core.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.061855 trafilatura-1.9.0/trafilatura/data/
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)   851312 2022-08-02 16:32:41.000000 trafilatura-1.9.0/trafilatura/data/jt-stopwords-pickle.lzma
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    80692 2022-08-02 16:32:41.000000 trafilatura-1.9.0/trafilatura/data/tei-schema-pickle.lzma
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    14735 2024-04-30 11:35:41.000000 trafilatura-1.9.0/trafilatura/downloads.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7913 2024-04-24 09:53:37.000000 trafilatura-1.9.0/trafilatura/external.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9649 2024-04-09 17:44:20.000000 trafilatura-1.9.0/trafilatura/feeds.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4672 2024-04-11 16:43:13.000000 trafilatura-1.9.0/trafilatura/filters.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     1755 2024-04-15 13:16:04.000000 trafilatura-1.9.0/trafilatura/gui.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     4876 2023-08-18 16:12:07.000000 trafilatura-1.9.0/trafilatura/hashing.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    13097 2024-04-24 09:53:37.000000 trafilatura-1.9.0/trafilatura/htmlprocessing.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9844 2023-08-18 16:12:07.000000 trafilatura-1.9.0/trafilatura/json_metadata.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3702 2024-04-09 17:44:20.000000 trafilatura-1.9.0/trafilatura/lru.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    27179 2024-04-24 09:53:37.000000 trafilatura-1.9.0/trafilatura/main_extractor.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      951 2023-08-18 16:12:07.000000 trafilatura-1.9.0/trafilatura/meta.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    21713 2024-04-23 11:13:31.000000 trafilatura-1.9.0/trafilatura/metadata.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16792 2024-04-11 16:43:13.000000 trafilatura-1.9.0/trafilatura/readability_lxml.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      739 2024-02-05 15:30:45.000000 trafilatura-1.9.0/trafilatura/settings.cfg
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     7048 2024-04-24 09:53:37.000000 trafilatura-1.9.0/trafilatura/settings.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9766 2024-04-08 16:09:42.000000 trafilatura-1.9.0/trafilatura/sitemaps.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     9013 2024-04-15 10:58:10.000000 trafilatura-1.9.0/trafilatura/spider.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    15888 2024-04-11 16:43:13.000000 trafilatura-1.9.0/trafilatura/utils.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    22115 2024-04-23 11:00:58.000000 trafilatura-1.9.0/trafilatura/xml.py
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)    16127 2024-04-19 13:07:39.000000 trafilatura-1.9.0/trafilatura/xpaths.py
+drwxrwxr-x   0 adbar     (1000) adbar     (1000)        0 2024-05-02 10:13:42.061855 trafilatura-1.9.0/trafilatura.egg-info/
+-rw-r--r--   0 adbar     (1000) adbar     (1000)    14081 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/PKG-INFO
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)     3102 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/SOURCES.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/dependency_links.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       92 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/entry_points.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)        1 2024-05-02 10:13:41.000000 trafilatura-1.9.0/trafilatura.egg-info/not-zip-safe
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)      581 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/requires.txt
+-rw-rw-r--   0 adbar     (1000) adbar     (1000)       12 2024-05-02 10:13:42.000000 trafilatura-1.9.0/trafilatura.egg-info/top_level.txt
```

### Comparing `trafilatura-1.8.1/CITATION.cff` & `trafilatura-1.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/CONTRIBUTING.md` & `trafilatura-1.9.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,29 +16,29 @@
   * [List of currently open issues](https://github.com/adbar/trafilatura/issues) (no pretention to exhaustivity!)
   * [Roadmap and milestones](https://github.com/adbar/trafilatura/milestones)
   * [How to Contribute to Open Source](https://opensource.guide/how-to-contribute/)
 
 
 ## Submitting changes
 
-Please send a [GitHub Pull Request to trafilatura](https://github.com/adbar/trafilatura/pull/new/master) with a clear list of what you've done (read more about [pull requests](http://help.github.com/pull-requests/)).
+Please send a [GitHub Pull Request to trafilatura](https://github.com/adbar/trafilatura/pull/new/master) with a clear list of what you have done (read more about [pull requests](http://help.github.com/pull-requests/)).
 
 **Working on your first Pull Request?** See this tutorial: [How To Create a Pull Request on GitHub](https://www.digitalocean.com/community/tutorials/how-to-create-a-pull-request-on-github)
 
 
-A special thanks to all the [contributors](https://github.com/adbar/trafilatura/graphs/contributors) who have played a part in developing and enhancing Trafilatura.
+A special thanks to all the [contributors](https://github.com/adbar/trafilatura/graphs/contributors) who have played a part in Trafilatura.
 
 
 
 ## Testing and evaluating the code
 
 Here is how you can run the tests if you wish to correct the errors and further improve the code:
 
 - Run `pytest` from trafilatura's directory, or select a particular test suite, for example `realworld_tests.py`, and run `pytest realworld_tests.py` or simply `python3 realworld_tests.py`
-- Check how it performs on the benchmark in `tests/eval/` by running `tests/comparison.py`
+- Check how it performs on the benchmark in `tests/eval/` by running `tests/comparison_small.py`
 
 See also the [tests Readme](tests/README.rst) for more information on the evaluation.
 
 
 
 For further questions you can contact me by way of [GitHub issues](https://github.com/adbar/trafilatura/issues), [X](https://x.com/adbarbaresi) or [E-Mail](https://adrien.barbaresi.eu/).
```

### Comparing `trafilatura-1.8.1/HISTORY.md` & `trafilatura-1.9.0/HISTORY.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 ## History / Changelog
 
 
+### 1.9.0
+
+Extraction:
+- add markdown as explicit output (#550)
+- improve recall preset (#571)
+- speedup for readability-lxml (#547)
+- add global options object for extraction and use it in CLI (#552)
+- fix: better encoding detection (#548)
+- recall: fix for lists inside tables with @mikhainin (#534)
+- add symbol to preserve vertical spacing in Markdown (#499)
+- fix: table cell separators in non-XML output (#563)
+- slightly better accuracy and execution speed overall
+
+Metadata:
+- add file creation date (date extraction, JSON & XML-TEI) (#561)
+- fix: empty content in meta tag by @felipehertzer (#545)
+
+Maintenance:
+- restructure and simplify code (#543, #556)
+- CLI & downloads: revamp and use global options (#565)
+- eval: review code, add guidelines and small benchmark (#542)
+- fix: raise error if config file does not exist (#554)
+- deprecate `process_record()` (#549)
+- docs: convert readme to markdown and update info (#564, #578)
+
+
 ### 1.8.1
 
 Maintenance:
 - Pin LXML to prevent broken dependency (#535)
 
 Extraction:
 - Improve extraction accuracy for major news outlets (#530)
```

### Comparing `trafilatura-1.8.1/LICENSE` & `trafilatura-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/PKG-INFO` & `trafilatura-1.9.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trafilatura
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python package and command-line tool designed to gather text on the Web, includes all necessary discovery and text processing components to perform web crawling, downloads, scraping, and extraction of main texts, metadata and comments.
 Home-page: https://trafilatura.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Documentation, https://trafilatura.readthedocs.io
 Project-URL: Source, https://github.com/adbar/trafilatura
@@ -35,244 +35,260 @@
 Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
 Requires-Dist: charset_normalizer>=3.0.1; python_version < "3.7"
 Requires-Dist: charset_normalizer>=3.2.0; python_version >= "3.7"
-Requires-Dist: courlan>=1.0.0
-Requires-Dist: htmldate>=1.8.0
+Requires-Dist: courlan>=1.1.0
+Requires-Dist: htmldate>=1.8.1
 Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: justext>=3.0.0
 Requires-Dist: lxml==4.9.2; platform_system == "Darwin" and python_version <= "3.8"
 Requires-Dist: lxml<5.2.0,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 Provides-Extra: all
 Requires-Dist: brotli; extra == "all"
 Requires-Dist: cchardet>=2.1.7; python_version < "3.11" and extra == "all"
 Requires-Dist: faust-cchardet>=2.1.19; python_version >= "3.11" and extra == "all"
-Requires-Dist: htmldate[speed]>=1.8.0; extra == "all"
+Requires-Dist: htmldate[speed]>=1.8.1; extra == "all"
 Requires-Dist: py3langid>=0.2.2; extra == "all"
 Requires-Dist: pycurl>=7.45.3; extra == "all"
 Provides-Extra: gui
 Requires-Dist: Gooey>=1.0.1; extra == "gui"
 
-Trafilatura: Discover and Extract Text Data on the Web
-======================================================
+# Trafilatura: Discover and Extract Text Data on the Web
 
+<br/>
 
-.. image:: https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-logo.png
-   :alt: Trafilatura Logo
-   :align: center
-   :width: 60%
+<img alt="Trafilatura Logo" src="https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-logo.png" align="center" width="60%"/>
 
-|
+<br/>
 
-.. image:: https://img.shields.io/pypi/v/trafilatura.svg
-    :target: https://pypi.python.org/pypi/trafilatura
-    :alt: Python package
+[![Python package](https://img.shields.io/pypi/v/trafilatura.svg)](https://pypi.python.org/pypi/trafilatura)
+[![Python versions](https://img.shields.io/pypi/pyversions/trafilatura.svg)](https://pypi.python.org/pypi/trafilatura)
+[![Documentation Status](https://readthedocs.org/projects/trafilatura/badge/?version=latest)](http://trafilatura.readthedocs.org/en/latest/?badge=latest)
+[![Code Coverage](https://img.shields.io/codecov/c/github/adbar/trafilatura.svg)](https://codecov.io/gh/adbar/trafilatura)
+[![Downloads](https://static.pepy.tech/badge/trafilatura/month)](https://pepy.tech/project/trafilatura)
+[![Reference DOI: 10.18653/v1/2021.acl-demo.15](https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue)](https://aclanthology.org/2021.acl-demo.15/)
 
-.. image:: https://img.shields.io/pypi/pyversions/trafilatura.svg
-    :target: https://pypi.python.org/pypi/trafilatura
-    :alt: Python versions
+<br/>
 
-.. image:: https://readthedocs.org/projects/trafilatura/badge/?version=latest
-    :target: http://trafilatura.readthedocs.org/en/latest/?badge=latest
-    :alt: Documentation Status
+<img alt="Demo as GIF image" src="https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-demo.gif" align="center" width="80%"/>
 
-.. image:: https://img.shields.io/codecov/c/github/adbar/trafilatura.svg
-    :target: https://codecov.io/gh/adbar/trafilatura
-    :alt: Code Coverage
+<br/>
 
-.. image:: https://static.pepy.tech/badge/trafilatura/month
-    :target: https://pepy.tech/project/trafilatura
-    :alt: Downloads
 
-.. image:: https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue
-    :target: https://aclanthology.org/2021.acl-demo.15/
-    :alt: Reference DOI: 10.18653/v1/2021.acl-demo.15
+## Introduction
 
-|
+Trafilatura is a cutting-edge **Python package and command-line tool**
+designed to **gather text on the Web and simplify the process of turning
+raw HTML into structured, meaningful data**. It includes all necessary
+discovery and text processing components to perform **web crawling,
+downloads, scraping, and extraction** of main texts, metadata and
+comments. It aims at staying **handy and modular**: no database is
+required, the output can be converted to commonly used formats.
 
-.. image:: https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-demo.gif
-    :alt: Demo as GIF image
-    :align: center
-    :width: 85%
-    :target: https://trafilatura.readthedocs.org/
+Going from HTML bulk to essential parts can alleviate many problems
+related to text quality, by **focusing on the actual content**,
+**avoiding the noise** caused by recurring elements (headers, footers
+etc.), and **making sense of the data** with selected information. The
+extractor is designed to be **robust and reasonably fast**, it runs in
+production on millions of documents.
 
+The tool's versatility makes it **useful for quantitative and
+data-driven approaches**. It is used in the academic domain and beyond
+(e.g. in natural language processing, computational social science,
+search engine optimization, and information security).
 
-Introduction
-------------
 
-
-Trafilatura is a cutting-edge **Python package and command-line tool** designed to **gather text on the Web and simplify the process of turning raw HTML into structured, meaningful data**. It includes all necessary discovery and text processing components to perform **web crawling, downloads, scraping, and extraction** of main texts, metadata and comments. It aims at staying **handy and modular**: no database is required, the output can be converted to commonly used formats.
-
-Going from HTML bulk to essential parts can alleviate many problems related to text quality, by **focusing on the actual content**, **avoiding the noise** caused by recurring elements (headers, footers etc.), and **making sense of the data** with selected information. The extractor is designed to be **robust and reasonably fast**, it runs in production on millions of documents.
-
-The tool's versatility makes it **useful for quantitative and data-driven approaches**. It is used in the academic domain and beyond (e.g. in natural language processing, computational social science, search engine optimization, and information security).
-
-
-Features
-~~~~~~~~
+### Features
 
 - Advanced web crawling and text discovery:
    - Support for sitemaps (TXT, XML) and feeds (ATOM, JSON, RSS)
    - Smart crawling and URL management (filtering and deduplication)
+
 - Parallel processing of online and offline input:
    - Live URLs, efficient and polite processing of download queues
    - Previously downloaded HTML files and parsed HTML trees
+
 - Robust and configurable extraction of key elements:
    - Main text (common patterns and generic algorithms like jusText and readability)
    - Metadata (title, author, date, site name, categories and tags)
    - Formatting and structure: paragraphs, titles, lists, quotes, code, line breaks, in-line text formatting
    - Optional elements: comments, links, images, tables
+
 - Multiple output formats:
    - Text (minimal formatting or Markdown)
    - CSV (with metadata)
    - JSON (with metadata)
-   - XML or `XML-TEI <https://tei-c.org/>`_ (with metadata, text formatting and page structure)
+   - XML or [XML-TEI](https://tei-c.org/) (with metadata, text formatting and page structure)
+
 - Optional add-ons:
    - Language detection on extracted content
    - Graphical user interface (GUI)
    - Speed optimizations
+
 - Actively maintained with support from the open-source community:
    - Regular updates, feature additions, and optimizations
    - Comprehensive documentation
 
 
-Evaluation and alternatives
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Trafilatura consistently outperforms other open-source libraries in text extraction benchmarks, showcasing its efficiency and accuracy in extracting web content. The extractor tries to strike a balance between limiting noise and including all valid parts.
-
-For more information see the `benchmark section <https://trafilatura.readthedocs.io/en/latest/evaluation.html>`_ and the `evaluation readme <https://github.com/adbar/trafilatura/blob/master/tests/README.rst>`_ to reproduce the results.
-
-
-=============================== =========  ========== ========= ========= ======
-750 documents, 2236 text & 2250 boilerplate segments (2022-05-18), Python 3.8
---------------------------------------------------------------------------------
-Python Package                  Precision  Recall     Accuracy  F-Score   Diff.
-=============================== =========  ========== ========= ========= ======
-html_text 0.5.2                 0.529      **0.958**  0.554     0.682     2.2x
-inscriptis 2.2.0 (html to txt)  0.534      **0.959**  0.563     0.686     3.5x
-newspaper3k 0.2.8               0.895      0.593      0.762     0.713     12x
-justext 3.0.0 (custom)          0.865      0.650      0.775     0.742     5.2x
-boilerpy3 1.0.6 (article mode)  0.814      0.744      0.787     0.777     4.1x
-*baseline (text markup)*        0.757      0.827      0.781     0.790     **1x**
-goose3 3.1.9                    **0.934**  0.690      0.821     0.793     22x
-readability-lxml 0.8.1          0.891      0.729      0.820     0.801     5.8x
-news-please 1.5.22              0.898      0.734      0.826     0.808     61x
-readabilipy 0.2.0               0.877      0.870      0.874     0.874     248x
-trafilatura 1.2.2 (standard)    0.914      0.904      **0.910** **0.909** 7.1x
-=============================== =========  ========== ========= ========= ======
-
-
-Other evaluations:
-^^^^^^^^^^^^^^^^^^
-
-- Most efficient open-source library in *ScrapingHub*'s `article extraction benchmark <https://github.com/scrapinghub/article-extraction-benchmark>`_
-- Best overall tool according to `Bien choisir son outil d'extraction de contenu à partir du Web <https://hal.archives-ouvertes.fr/hal-02768510v3/document>`_ (Lejeune & Barbaresi 2020)
-- Best single tool by ROUGE-LSum Mean F1 Page Scores in `An Empirical Comparison of Web Content Extraction Algorithms <https://webis.de/downloads/publications/papers/bevendorff_2023b.pdf>`_ (Bevendorff et al. 2023)
-
-
-Usage and documentation
------------------------
-
-`Getting started with Trafilatura <https://trafilatura.readthedocs.io/en/latest/quickstart.html>`_ is straightforward. For more information and detailed guides, visit `Trafilatura's documentation <https://trafilatura.readthedocs.io/>`_:
-
-- `Installation <https://trafilatura.readthedocs.io/en/latest/installation.html>`_
-- Usage: `On the command-line <https://trafilatura.readthedocs.io/en/latest/usage-cli.html>`_, `With Python <https://trafilatura.readthedocs.io/en/latest/usage-python.html>`_, `With R <https://trafilatura.readthedocs.io/en/latest/usage-r.html>`_
-- `Core Python functions <https://trafilatura.readthedocs.io/en/latest/corefunctions.html>`_
-- Interactive Python Notebook: `Trafilatura Overview <docs/Trafilatura_Overview.ipynb>`_
-- `Tutorials and use cases <https://trafilatura.readthedocs.io/en/latest/tutorials.html>`_
+### Evaluation and alternatives
 
+Trafilatura consistently outperforms other open-source libraries in text
+extraction benchmarks, showcasing its efficiency and accuracy in
+extracting web content. The extractor tries to strike a balance between
+limiting noise and including all valid parts.
+
+For more information see the [benchmark section](https://trafilatura.readthedocs.io/en/latest/evaluation.html)
+and the [evaluation readme](https://github.com/adbar/trafilatura/blob/master/tests/README.rst)
+to reproduce the results.
+
+**750 documents, 2236 text & 2250 boilerplate segments (2022-05-18), Python 3.8**
+
+| Python Package | Precision | Recall | Accuracy | F-Score | Diff. |
+|----------------|-----------|--------|----------|---------|-------|
+| html_text 0.5.2 | 0.529 | **0.958** | 0.554 | 0.682 | 2.2x |
+| inscriptis 2.2.0 (html to txt) | 0.534 | **0.959** | 0.563 | 0.686 | 3.5x |
+| newspaper3k 0.2.8 | 0.895 | 0.593 | 0.762 | 0.713 | 12x |
+| justext 3.0.0 (custom) | 0.865 | 0.650 | 0.775 | 0.742 | 5.2x |
+| boilerpy3 1.0.6 (article mode) | 0.814 | 0.744 | 0.787 | 0.777 | 4.1x |
+| *baseline (text markup)* | 0.757 | 0.827 | 0.781 | 0.790 | **1x** |
+| goose3 3.1.9 | **0.934** | 0.690 | 0.821 | 0.793 | 22x |
+| readability-lxml 0.8.1 | 0.891 | 0.729 | 0.820 | 0.801 | 5.8x |
+| news-please 1.5.22 | 0.898 | 0.734 | 0.826 | 0.808 | 61x |
+| readabilipy 0.2.0 | 0.877 | 0.870 | 0.874 | 0.874 | 248x |
+| trafilatura 1.2.2 (standard) | 0.914 | 0.904 | **0.910** | **0.909** | 7.1x |
+
+
+#### Other evaluations:
+
+- Most efficient open-source library in *ScrapingHub*'s [article extraction benchmark](https://github.com/scrapinghub/article-extraction-benchmark)
+- Best overall tool according to [Bien choisir son outil d'extraction de contenu à partir du Web](https://hal.archives-ouvertes.fr/hal-02768510v3/document)
+  (Lejeune & Barbaresi 2020)
+- Best single tool by ROUGE-LSum Mean F1 Page Scores in [An Empirical Comparison of Web Content Extraction Algorithms](https://webis.de/downloads/publications/papers/bevendorff_2023b.pdf)
+  (Bevendorff et al. 2023)
+
+
+## Usage and documentation
+
+[Getting started with Trafilatura](https://trafilatura.readthedocs.io/en/latest/quickstart.html)
+is straightforward. For more information and detailed guides, visit
+[Trafilatura's documentation](https://trafilatura.readthedocs.io/):
+
+- [Installation](https://trafilatura.readthedocs.io/en/latest/installation.html)
+- Usage:
+  [On the command-line](https://trafilatura.readthedocs.io/en/latest/usage-cli.html),
+  [With Python](https://trafilatura.readthedocs.io/en/latest/usage-python.html),
+  [With R](https://trafilatura.readthedocs.io/en/latest/usage-r.html)
+- [Core Python functions](https://trafilatura.readthedocs.io/en/latest/corefunctions.html)
+- Interactive Python Notebook: [Trafilatura Overview](docs/Trafilatura_Overview.ipynb)
+- [Tutorials and use cases](https://trafilatura.readthedocs.io/en/latest/tutorials.html)
 
 Youtube playlist with video tutorials in several languages:
 
-- `Web scraping tutorials and how-tos <https://www.youtube.com/watch?v=8GkiOM17t0Q&list=PL-pKWbySIRGMgxXQOtGIz1-nbfYLvqrci>`_
+- [Web scraping tutorials and how-tos](https://www.youtube.com/watch?v=8GkiOM17t0Q&list=PL-pKWbySIRGMgxXQOtGIz1-nbfYLvqrci)
 
 
-License
--------
+## License
 
-This package is distributed under the `Apache 2.0 license <https://www.apache.org/licenses/LICENSE-2.0.html>`_.
+This package is distributed under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.html).
 
 Versions prior to v1.8.0 are under GPLv3+ license.
 
 
-Contributing
-------------
-
-Contributions of all kinds are welcome. Visit the `Contributing page <https://github.com/adbar/trafilatura/blob/master/CONTRIBUTING.md>`_ for more information. Bug reports can be filed on the `dedicated issue page <https://github.com/adbar/trafilatura/issues>`_.
-
-Many thanks to the `contributors <https://github.com/adbar/trafilatura/graphs/contributors>`_ who extended the docs or submitted bug reports, features and bugfixes!
-
-
-Context
--------
-
-Developed with practical applications of academic research in mind, this software is part of a broader effort to derive information from web documents. Extracting and pre-processing web texts to the exacting standards of scientific research presents a substantial challenge. This software package simplifies text data collection and enhances corpus quality, it is currently used to build `text databases for linguistic research <https://www.dwds.de/d/k-web>`_.
-
-*Trafilatura* is an Italian word for `wire drawing <https://en.wikipedia.org/wiki/Wire_drawing>`_ symbolizing the refinement and conversion process. It is also the way shapes of pasta are formed.
-
-
-Author
-~~~~~~
-
-Reach out via ia the software repository or the `contact page <https://adrien.barbaresi.eu/>`_ for inquiries, collaborations, or feedback. See also X or LinkedIn for the latest updates.
-
-This work started as a PhD project at the crossroads of linguistics and NLP, this expertise has been instrumental in shaping Trafilatura over the years. It has first been released under its current form in 2019, its development is referenced in the following publications:
-
-- Barbaresi, A. `Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction <https://aclanthology.org/2021.acl-demo.15/>`_, Proceedings of ACL/IJCNLP 2021: System Demonstrations, 2021, p. 122-131.
--  Barbaresi, A. "`Generic Web Content Extraction with Open-Source Software <https://hal.archives-ouvertes.fr/hal-02447264/document>`_", Proceedings of KONVENS 2019, Kaleidoscope Abstracts, 2019.
--  Barbaresi, A. "`Efficient construction of metadata-enhanced web corpora <https://hal.archives-ouvertes.fr/hal-01371704v2/document>`_", Proceedings of the `10th Web as Corpus Workshop (WAC-X) <https://www.sigwac.org.uk/wiki/WAC-X>`_, 2016.
-
-
-Citing Trafilatura
-~~~~~~~~~~~~~~~~~~
-
-Trafilatura is widely used in the academic domain, chiefly for data acquisition. Here is how to cite it:
-
-.. image:: https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue
-    :target: https://aclanthology.org/2021.acl-demo.15/
-    :alt: Reference DOI: 10.18653/v1/2021.acl-demo.15
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3460969.svg
-   :target: https://doi.org/10.5281/zenodo.3460969
-   :alt: Zenodo archive DOI: 10.5281/zenodo.3460969
-
-.. code-block:: shell
-
-    @inproceedings{barbaresi-2021-trafilatura,
-      title = {{Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction}},
-      author = "Barbaresi, Adrien",
-      booktitle = "Proceedings of the Joint Conference of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing: System Demonstrations",
-      pages = "122--131",
-      publisher = "Association for Computational Linguistics",
-      url = "https://aclanthology.org/2021.acl-demo.15",
-      year = 2021,
-    }
-
-
-Software ecosystem
-~~~~~~~~~~~~~~~~~~
-
-Case studies and publications are listed on the `Used By documentation page <https://trafilatura.readthedocs.io/en/latest/used-by.html>`_.
-
-Jointly developed plugins and additional packages also contribute to the field of web data extraction and analysis:
-
-
-.. image:: https://raw.githubusercontent.com/adbar/htmldate/master/docs/software-ecosystem.png
-    :alt: Software ecosystem
-    :align: center
-    :width: 65%
-
-
+## Contributing
 
-Corresponding posts can be found on `Bits of Language <https://adrien.barbaresi.eu/blog/tag/trafilatura.html>`_. The blog covers a range of topics from technical how-tos, updates on new features, to discussions on text mining challenges and solutions.
+Contributions of all kinds are welcome. Visit the [Contributing
+page](https://github.com/adbar/trafilatura/blob/master/CONTRIBUTING.md)
+for more information. Bug reports can be filed on the [dedicated issue
+page](https://github.com/adbar/trafilatura/issues).
+
+Many thanks to the
+[contributors](https://github.com/adbar/trafilatura/graphs/contributors)
+who extended the docs or submitted bug reports, features and bugfixes!
+
+
+## Context
+
+Developed with practical applications of academic research in mind, this
+software is part of a broader effort to derive information from web
+documents. Extracting and pre-processing web texts to the exacting
+standards of scientific research presents a substantial challenge. This
+software package simplifies text data collection and enhances corpus
+quality, it is currently used to build [text databases for linguistic
+research](https://www.dwds.de/d/k-web).
+
+*Trafilatura* is an Italian word for [wire
+drawing](https://en.wikipedia.org/wiki/Wire_drawing) symbolizing the
+refinement and conversion process. It is also the way shapes of pasta
+are formed.
+
+### Author
+
+Reach out via ia the software repository or the [contact
+page](https://adrien.barbaresi.eu/) for inquiries, collaborations, or
+feedback. See also X or LinkedIn for the latest updates.
+
+This work started as a PhD project at the crossroads of linguistics and
+NLP, this expertise has been instrumental in shaping Trafilatura over
+the years. It has first been released under its current form in 2019,
+its development is referenced in the following publications:
+
+-   Barbaresi, A. [Trafilatura: A Web Scraping Library and Command-Line
+    Tool for Text Discovery and
+    Extraction](https://aclanthology.org/2021.acl-demo.15/), Proceedings
+    of ACL/IJCNLP 2021: System Demonstrations, 2021, p. 122-131.
+-   Barbaresi, A. "[Generic Web Content Extraction with Open-Source
+    Software](https://hal.archives-ouvertes.fr/hal-02447264/document)",
+    Proceedings of KONVENS 2019, Kaleidoscope Abstracts, 2019.
+-   Barbaresi, A. "[Efficient construction of metadata-enhanced web
+    corpora](https://hal.archives-ouvertes.fr/hal-01371704v2/document)",
+    Proceedings of the [10th Web as Corpus Workshop
+    (WAC-X)](https://www.sigwac.org.uk/wiki/WAC-X), 2016.
+
+
+### Citing Trafilatura
+
+Trafilatura is widely used in the academic domain, chiefly for data
+acquisition. Here is how to cite it:
+
+[![Reference DOI: 10.18653/v1/2021.acl-demo.15](https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue)](https://aclanthology.org/2021.acl-demo.15/)
+[![Zenodo archive DOI: 10.5281/zenodo.3460969](https://zenodo.org/badge/DOI/10.5281/zenodo.3460969.svg)](https://doi.org/10.5281/zenodo.3460969)
+
+``` shell
+@inproceedings{barbaresi-2021-trafilatura,
+  title = {{Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction}},
+  author = "Barbaresi, Adrien",
+  booktitle = "Proceedings of the Joint Conference of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing: System Demonstrations",
+  pages = "122--131",
+  publisher = "Association for Computational Linguistics",
+  url = "https://aclanthology.org/2021.acl-demo.15",
+  year = 2021,
+}
+```
+
+
+### Software ecosystem
+
+Case studies and publications are listed on the [Used By documentation
+page](https://trafilatura.readthedocs.io/en/latest/used-by.html).
+
+Jointly developed plugins and additional packages also contribute to the
+field of web data extraction and analysis:
+
+<img alt="Software ecosystem" src="https://raw.githubusercontent.com/adbar/htmldate/master/docs/software-ecosystem.png" align="center" width="65%"/>
+
+Corresponding posts can be found on [Bits of
+Language](https://adrien.barbaresi.eu/blog/tag/trafilatura.html). The
+blog covers a range of topics from technical how-tos, updates on new
+features, to discussions on text mining challenges and solutions.
 
-Impressive, you have reached the end of the page: Thank you for your interest!
+Impressive, you have reached the end of the page: Thank you for your
+interest!
```

### Comparing `trafilatura-1.8.1/docs/Makefile` & `trafilatura-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/dwds-count-exportieren.jpg` & `trafilatura-1.9.0/docs/_build/_images/dwds-count-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/dwds-exportieren.jpg` & `trafilatura-1.9.0/docs/_build/_images/dwds-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/dwds-treffer-exportieren.jpg` & `trafilatura-1.9.0/docs/_build/_images/dwds-treffer-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/gui-screenshot.png` & `trafilatura-1.9.0/docs/_build/_images/gui-screenshot.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/software-ecosystem.png` & `trafilatura-1.9.0/docs/_build/_images/software-ecosystem.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_images/trafilatura-demo.gif` & `trafilatura-1.9.0/docs/_build/_images/trafilatura-demo.gif`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/_build/_static/trafilatura-logo.png` & `trafilatura-1.9.0/docs/_build/_static/trafilatura-logo.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/compendium.rst` & `trafilatura-1.9.0/docs/compendium.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/conf.py` & `trafilatura-1.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 ## pydata options
 html_theme_options = {
   "github_url": "https://github.com/adbar/trafilatura",
   "twitter_url": "https://twitter.com/adbarbaresi",
   "external_links": [
       {"name": "Blog", "url": "https://adrien.barbaresi.eu/blog/tag/trafilatura.html"},
   ],
+  "navigation_with_keys": False,
 #  "use_edit_page_button": True,
 #  "navigation_depth": 3,
 #  "show_toc_level": 3,
 }
 html_theme_options["analytics"] = {
   "google_analytics_id": "G-K3R5QCVDF1",
   "analytics_anonymize_ip": True,
```

### Comparing `trafilatura-1.8.1/docs/corefunctions.rst` & `trafilatura-1.9.0/docs/corefunctions.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/corpus-data.rst` & `trafilatura-1.9.0/docs/corpus-data.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/crawls.rst` & `trafilatura-1.9.0/docs/crawls.rst`

 * *Files 11% similar despite different names*

```diff
@@ -53,49 +53,54 @@
 
 With Python
 -----------
 
 Focused crawler
 ~~~~~~~~~~~~~~~
 
-The ``focused_crawler()`` function integrates all necessary components. It can be adjusted by a series of arguments:
+The ``focused_crawler()`` function integrates all necessary components and can be adjusted by a series of arguments. The following lines explain how to set up a focused crawler which will explore a given website to extract internal links.
 
 .. code-block:: python
 
     >>> from trafilatura.spider import focused_crawler
 
-    homepage = 'https://www.example.org'
-    # starting a crawl
-    >>> to_visit, known_urls = focused_crawler(homepage, max_seen_urls=10, max_known_urls=100000)
-    # resuming a crawl
-    >>> to_visit, known_urls = focused_crawler(homepage, max_seen_urls=10, max_known_urls=100000, todo=to_visit, known_links=known_urls)
+    >>> homepage = 'https://www.example.org'
+
+    # perform the first iteration (will not work with this website, there are no internal links)
+    >>> to_visit, known_links = focused_crawler("https://example.org", max_seen_urls=1)
+
+    # perform another iteration using previously collected information
+    >>> to_visit, known_links = focused_crawler("https://example.org", max_seen_urls=10, max_known_urls=100000, todo=to_visit, known=known_links)
+
 
 Here the crawler stops after seeing a maximum of 10 URLs or registering a total of 100000 URLs on the website, whichever comes first.
 
-The collected links can then be downloaded and processed. The links to visit (crawl frontier) are stored as a `deque <https://docs.python.org/3/library/collections.html#collections.deque>`_ (a double-ended queue) which mostly works like a list. The known URLs are stored as a set. Both can also be converted to a list if necessary:
+The collected links can then be downloaded and processed. The ``to_visit`` variable keeps track of what's ahead of the exploration. Using ``known_links`` makes sure the same pages are not visited twice.  The links to visit (crawl frontier) are stored as a `deque <https://docs.python.org/3/library/collections.html#collections.deque>`_ (a double-ended queue) which mostly works like a list. The known URLs are stored as a set. Both can also be converted to a list if necessary:
 
 .. code-block:: python
 
     to_visit, known_urls = list(to_visit), sorted(known_urls)
 
 
+As this requirement can vary depending on the use case (e.g. checking new pages every day on a homepage) these variables are optional. Other parameters include ``lang`` (target language), ``config`` (see settings file), and ``rules`` (politeness rules, defaults to the ones provided by the website or safe values).
+
 You can also use a custom configuration and pass politeness rules to the crawler. For more information see the `documentation of the function <corefunctions.html#trafilatura.spider.focused_crawler>`_.
 
 
 Navigation
 ~~~~~~~~~~
 
 .. hint::
     You may decide on the course of a crawl by determining if there are still navigation pages to visit:
 
 .. code-block:: python
 
-    from trafilatura.spider import is_still_navigation
+    >>> from trafilatura.spider import is_still_navigation
 
-    is_still_navigation(to_visit)
+    >>> is_still_navigation(to_visit)
     # returns True or False
 
 For more info please refer to the `core functions page <corefunctions.html>`_.
 
 
 On the command-line
 -------------------
@@ -110,15 +115,15 @@
 .. code-block:: bash
 
     $ trafilatura --crawl "https://www.example.org" > links.txt
 
 It can also crawl websites in parallel by reading a list of target sites from a list (``-i``/``--input-file`` option).
 
 .. note::
-    The ``--list`` option does not apply here. Unlike with the ``--sitemap`` or ``--feed`` options, the URLs are simply returned as a list instead of being retrieved and processed. This happens in order to give a chance to examine the collected URLs prior to further downloads.
+    The ``--list`` option does not apply here. Unlike with the ``--sitemap`` or ``--feed`` options, the URLs are simply returned as a list instead of being retrieved and processed. This happens in order to give a chance to examine the collected URLs prior to further downloads. For more information on how to refine and filter a URL collection, see the underlying `courlan package <https://github.com/adbar/courlan>`_. 
 
 
 References
 ----------
 
 Boldi, P., Codenotti, B., Santini, M., & Vigna, S. (2004). Ubicrawler: A scalable fully distributed web crawler. Software: Practice and Experience, 34(8), 711-726.
```

### Comparing `trafilatura-1.8.1/docs/downloads.rst` & `trafilatura-1.9.0/docs/downloads.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/dwds-count-exportieren.jpg` & `trafilatura-1.9.0/docs/dwds-count-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/dwds-exportieren.jpg` & `trafilatura-1.9.0/docs/dwds-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/dwds-treffer-exportieren.jpg` & `trafilatura-1.9.0/docs/dwds-treffer-exportieren.jpg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/evaluation.rst` & `trafilatura-1.9.0/docs/evaluation.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/gui-screenshot.png` & `trafilatura-1.9.0/docs/gui-screenshot.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/index.rst` & `trafilatura-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/installation-gui.rst` & `trafilatura-1.9.0/docs/installation-gui.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/installation.rst` & `trafilatura-1.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/make.bat` & `trafilatura-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/quickstart.rst` & `trafilatura-1.9.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/settings.rst` & `trafilatura-1.9.0/docs/settings.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 - Input
    * ``MAX_FILE_SIZE = 20000000`` maximum acceptable size of input (in bytes)
    * ``MIN_FILE_SIZE = 10`` minimum acceptable size of input (in bytes)
 - Extraction
    * ``MIN_EXTRACTED_SIZE = 250`` acceptable size in characters (used to trigger fallbacks)
    * ``MIN_OUTPUT_SIZE = 1`` absolute acceptable minimum for main text output
    * ``MIN_EXTRACTED_COMM_SIZE`` and ``MIN_OUTPUT_COMM_SIZE`` work the same for comment extraction
-   * ``EXTRACTION_TIMEOUT = 30`` now only affects processing on the command-line: drop extraction after 30 seconds to prevent malicious HTML bombs. Set to 0 if you see errors related to the ``signal`` module and/or use a module such as `defusedxml <https://github.com/tiran/defusedxml>`_
+   * ``EXTRACTION_TIMEOUT = 30`` only active on the command-line: drop extraction after 30 seconds to prevent CPU usage due to erroneous or malicious files. Set to 0 if you see errors related to the ``signal`` module and/or use a module such as `defusedxml <https://github.com/tiran/defusedxml>`_
 - Deduplication (not active by default)
    * ``MIN_DUPLCHECK_SIZE = 100`` minimum size in characters to run deduplication on
    * ``MAX_REPETITIONS = 2`` maximum number of duplicates allowed
 - Metadata
    * ``EXTENSIVE_DATE_SEARCH = on`` set to ``off`` to deactivate ``htmldate``'s opportunistic search (lower recall, higher precision)
 - Navigation
    * ``EXTERNAL_URLS = off`` do not take URLs from other websites in feeds and sitemaps (CLI mode)
@@ -119,7 +119,11 @@
 Here is how to change them:
 
 1. Find the locally installed version of the package or `clone the repository <https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository>`_
 2. Edit ``settings.py``
 3. Reinstall the package locally: ``pip install --no-deps -U .`` in the home directory of the cloned repository
 
 These remaining variables greatly alter the functioning of the package!
+
+
+.. hint::
+    Starting from version 1.9, most extraction parameters and options can be defined in an object which is then passed to the extraction functions instead of the arguments and (in some cases) instead of the config file. See ``settings.py`` for an example.
```

#### html2text {}

```diff
@@ -17,18 +17,18 @@
 (higher is better to avoid detection) * ``USER_AGENTS`` and ``COOKIE`` are
 empty by default - Input * ``MAX_FILE_SIZE = 20000000`` maximum acceptable size
 of input (in bytes) * ``MIN_FILE_SIZE = 10`` minimum acceptable size of input
 (in bytes) - Extraction * ``MIN_EXTRACTED_SIZE = 250`` acceptable size in
 characters (used to trigger fallbacks) * ``MIN_OUTPUT_SIZE = 1`` absolute
 acceptable minimum for main text output * ``MIN_EXTRACTED_COMM_SIZE`` and
 ``MIN_OUTPUT_COMM_SIZE`` work the same for comment extraction *
-``EXTRACTION_TIMEOUT = 30`` now only affects processing on the command-line:
-drop extraction after 30 seconds to prevent malicious HTML bombs. Set to 0 if
-you see errors related to the ``signal`` module and/or use a module such as
-`defusedxml
+``EXTRACTION_TIMEOUT = 30`` only active on the command-line: drop extraction
+after 30 seconds to prevent CPU usage due to erroneous or malicious files. Set
+to 0 if you see errors related to the ``signal`` module and/or use a module
+such as `defusedxml
 github.com/tiran/defusedxml>`_ - Deduplication (not active by default) *
 ``MIN_DUPLCHECK_SIZE = 100`` minimum size in characters to run deduplication on
 * ``MAX_REPETITIONS = 2`` maximum number of duplicates allowed - Metadata *
 ``EXTENSIVE_DATE_SEARCH = on`` set to ``off`` to deactivate ``htmldate``'s
 opportunistic search (lower recall, higher precision) - Navigation *
 ``EXTERNAL_URLS = off`` do not take URLs from other websites in feeds and
 sitemaps (CLI mode) * ``MAX_REDIRECTS = 2``: maximum number of `URL
@@ -71,8 +71,12 @@
 elements to accept or to discard - Configuration of parallel processing -
 Further download and deduplication settings - Files written in CLI mode Here is
 how to change them: 1. Find the locally installed version of the package or
 `clone the repository
 docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-
 repository>`_ 2. Edit ``settings.py`` 3. Reinstall the package locally: ``pip
 install --no-deps -U .`` in the home directory of the cloned repository These
-remaining variables greatly alter the functioning of the package!
+remaining variables greatly alter the functioning of the package! .. hint::
+Starting from version 1.9, most extraction parameters and options can be
+defined in an object which is then passed to the extraction functions instead
+of the arguments and (in some cases) instead of the config file. See
+``settings.py`` for an example.
```

### Comparing `trafilatura-1.8.1/docs/software-ecosystem.png` & `trafilatura-1.9.0/docs/software-ecosystem.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/sources.rst` & `trafilatura-1.9.0/docs/sources.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/trafilatura-demo.gif` & `trafilatura-1.9.0/docs/trafilatura-demo.gif`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/trafilatura-logo.png` & `trafilatura-1.9.0/docs/trafilatura-logo.png`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/troubleshooting.rst` & `trafilatura-1.9.0/docs/troubleshooting.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,42 @@
 
 .. meta::
     :description lang=en:
         This page explains how to solve common issues about content extraction and downloads.
         They include missing content, paywalls, cookies, and networks.
 
 
+
+.. hint::
+    Trafilatura evolves over time, make sure you have the latest version to benefit from all documentation pages. The software is thoroughly tested but rare problems remain difficult to replicate as they are linked to a particular setting/OS/IP. For the rest, see the `list of open issues <https://github.com/adbar/trafilatura/issues>`_
+
+
 Content extraction
 ------------------
 
 Something is missing
 ^^^^^^^^^^^^^^^^^^^^
 
 The extractor uses several fallbacks to make sure enough text is returned. Content extraction is a tradeoff between precision and recall, that is between desired and undesirable content. Being ready to accept more unwanted text makes it easier to gather more of the relevant text in the output. Here are ways to tackle the issue:
 
 - Opting for ``favor_recall`` (Python) or ``--recall`` (CLI)
 - Changing the minimum acceptable length in the settings
 - Using the more basic `baseline <corefunctions.html#baseline>`_ or `html2txt <corefunctions.html#html2txt>`_ functions instead (which is also faster)
 
 
+.. note::
+    Trafilatura is geared towards article pages, blog posts, main text parts, etc. Results vary wildly on link lists, galleries or catalogs.
+
+
 Beyond raw HTML
 ^^^^^^^^^^^^^^^
 
 While downloading and processing raw HTML documents is much faster, it can be necessary to fully render the web page before further processing, e.g. because a page makes exhaustive use of JavaScript or because content is injected from multiple sources.
 
-In such cases the way to go is to use a browser automation library like `Playwright <https://playwright.dev/python/>`_. For available alternatives see this `list of headless browsers <https://github.com/dhamaniasad/HeadlessBrowsers>`_.
+In such cases the way to go is to use a browser automation library like `Playwright <https://playwright.dev/python/docs/library/>`_. For available alternatives see this `list of headless browsers <https://github.com/dhamaniasad/HeadlessBrowsers>`_.
 
 For more refined masking and automation methods, see the `nodriver <https://github.com/ultrafunkamsterdam/nodriver>`_ and `browserforge <https://github.com/daijro/browserforge>`_ packages.
 
 
 
 Bypassing paywalls
 ^^^^^^^^^^^^^^^^^^
@@ -60,16 +69,16 @@
 ^^^^^^^^^^^^^^^^
 
 The standard library `cookiejar <https://docs.python.org/3/library/http.cookiejar.html>`_ can be used along ``urllib3`` in order to use cookies along with HTTP requests, see this `documentation pull request <https://github.com/urllib3/urllib3/pull/2474/files>`_.
 
 Alternatively, cookies can be manually specified in a ``settings.cfg`` config file, separated by semicolons, e.g. ``COOKIE = yummy_cookie=choco; tasty_cookie=strawberry``.
 
 
-Web page no longer available on the Internet
-^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Unavailable pages and link rot
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Download issues can be addressed by retrieving the files somewhere else, i.e. from already existing internet archives like the Internet Archive or the CommonCrawl.
 
 On the command-line you can use ``--archived`` to use the Internet Archive to retrieve pages for which download failed. A corresponding function in Python could look as follows:
 
 .. code-block:: python
```

### Comparing `trafilatura-1.8.1/docs/tutorial-dwds.rst` & `trafilatura-1.9.0/docs/tutorial-dwds.rst`

 * *Files 0% similar despite different names*

```diff
@@ -110,12 +110,12 @@
 
 Diese Linkliste kann zunächst gefiltert werden, um deutschsprachige, inhaltsreiche Webseiten zu bevorzugen. Der dafür nötige Softwareteil, `courlan <https://github.com/adbar/courlan>`_ wird mit *Trafilatura* installiert:
 
 ``courlan --language de --strict --inputfile linkliste-roh.txt --outputfile linkliste-gefiltert.txt``
 
 Die Ausgabe von *Trafilatura* erfolgt auf zweierlei Weise: die extrahierten Texte (TXT-Format) im Verzeichnis ``ausgabe`` und eine Kopie der heruntergeladenen Webseiten unter ``html-quellen`` (zur Archivierung und ggf. erneuten Verarbeitung):
 
-``trafilatura --input-file linkliste.txt --outputdir ausgabe/ --backup-dir html-quellen/``
+``trafilatura --input-file linkliste.txt --output-dir ausgabe/ --backup-dir html-quellen/``
 
 So werden TXT-Dateien ohne Metadaten ausgegeben. Wenn Sie ``--csv``, ``--json``, ``--xml`` oder ``--xmltei`` hinzufügen, werden Metadaten einbezogen und das entsprechende Format für die Ausgabe bestimmt. Zusätzliche Optionen sind verfügbar, siehe die passenden Dokumentationsseiten.
 
 Für bis zu einige Tausend URLs gelingt dieses Verfahren problemlos von einem Laptop aus, für mehr URLs kann ein Server notwendig sein, vor allem um lange Wartezeiten zu handhaben (zunächst werden die Seiten nämlich heruntergeladen).
```

### Comparing `trafilatura-1.8.1/docs/tutorial-epsilla.rst` & `trafilatura-1.9.0/docs/tutorial-epsilla.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/tutorial0.rst` & `trafilatura-1.9.0/docs/tutorial0.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/tutorial1.rst` & `trafilatura-1.9.0/docs/tutorial1.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/tutorial2.rst` & `trafilatura-1.9.0/docs/tutorial2.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/tutorials.rst` & `trafilatura-1.9.0/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/url-management.rst` & `trafilatura-1.9.0/docs/url-management.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/usage-api.rst` & `trafilatura-1.9.0/docs/usage-api.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/usage-cli.rst` & `trafilatura-1.9.0/docs/usage-cli.rst`

 * *Files 5% similar despite different names*

```diff
@@ -72,46 +72,50 @@
     Keep structural elements related to formatting (``<b>``/``<strong>``, ``<i>``/``<emph>`` etc.)
 ``--links``
     Keep link targets (in ``href="..."``), converting relative URLs to absolute where possible
 ``--images``
     Keep track of images along with their targets (``<img>`` attributes: alt, src, title)
 
 .. note::
-    Certain elements are only visible in the output if the chosen format allows it (e.g. images and XML).
-    
-    Including extra elements works best with conversion to XML/XML-TEI. If the output is buggy removing a constraint (e.g. formatting) can greatly improve the result.
+    Certain elements are only visible in the output if the chosen format allows it (e.g. images and XML). Including extra elements works best with conversion to XML/XML-TEI.
+
+    The heuristics used by the main algorithm change according to the presence of certain elements in the HTML. If the output seems odd removing a constraint (e.g. formatting) can greatly improve the result.
 
 
 Output format
 ~~~~~~~~~~~~~
 
 Output as TXT without metadata is the default, another format can be selected in two different ways:
 
--  ``--csv``, ``--json``, ``--xml`` or ``--xmltei``
--  ``-out`` or ``--output-format`` {txt,csv,json,xml,xmltei}
+-  ``--csv``, ``--json``, ``--markdown`` (from version 1.9 onwards), ``--xml`` or ``--xmltei``
+-  ``-out`` or ``--output-format`` {txt,csv,json,markdown,xml,xmltei}
 
 .. hint::
-    Combining TXT, CSV and JSON formats with certain structural elements (e.g. formatting or links) triggers output in TXT+Markdown format.
+    Combining TXT, CSV and JSON formats with certain structural elements (e.g. formatting or links) triggers output in TXT+Markdown format. Selecting markdown automatically includes text formatting.
 
 
 Optimizing for precision and recall
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-The arguments ``--precision`` & ``--recall`` can be passed to the extractor.
+The arguments ``--precision`` & ``--recall`` can be passed to the extractor. They affect processing and volume of textual output:
 
-They slightly affect processing and volume of textual output, respectively concerning precision/accuracy (i.e. more selective extraction, yielding less and more central elements) and recall (i.e. more opportunistic extraction, taking more elements into account).
+1. By focusing precision/accuracy, i.e. more selective extraction, yielding less and more central elements.
+   If you believe the results are too noisy, try focusing on precision.
+2. By enhancing recall, i.e. more opportunistic extraction, taking more elements into account.
+   If parts of the contents are still missing, see `troubleshooting <troubleshooting.html>`_.
 
 
 Language identification
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 Passing the argument ``--target-language`` along with a 2-letter code (`ISO 639-1 <https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes>`_) will trigger language filtering of the output if the identification component has been `installed <installation.html>`_ and if the target language is available.
 
 .. note::
-    Additional components are required: ``pip install trafilatura[all]``
+    Additional components are required: ``pip install trafilatura[all]``.
+    This feature currently uses the `py3langid package <https://github.com/adbar/py3langid>`_ and is dependent on language availability and performance of the original model.
 
 
 
 Changing default settings
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 See `documentation page on settings <settings.html>`_.
@@ -175,17 +179,17 @@
 
 There is a fair chance to find archived versions for larger websites, whereas pages of lesser-known websites may not have been preserved there. The retrieval process is slow as it depends on a single web portal only, it is best performed for a relatively small number of URLs.
 
 
 Link discovery
 --------------
 
-Link discovery can be performed over `web feeds <https://en.wikipedia.org/wiki/Web_feed>`_ (Atom and RSS) or `sitemaps <https://en.wikipedia.org/wiki/Sitemaps>`_.
+Link discovery can be performed over `web feeds <https://en.wikipedia.org/wiki/Web_feed>`_ (Atom and RSS, mostly for fresh content), `sitemaps <https://en.wikipedia.org/wiki/Sitemaps>`_ for exhaustivity (all potential pages as listed by the owners), and discovery by web crawling (i.e. by following the internal links, more experimental).
 
-Both homepages and particular sitemaps or feed URLs can be used as input.
+Both the homepage and a particular page can be used as input depending on the selected options (e.g. a sitemap or feed URL).
 
 The ``--list`` option is useful to list URLs prior to processing. This option can be combined with an input file (``-i``) containing a list of sources which will then be processed in parallel.
 
 For more information please refer to the `tutorial on content discovery <tutorial0.html#content-discovery>`_.
 
 Feeds
 ~~~~~
@@ -232,14 +236,22 @@
 
     <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/uWUyhxciTOs?start=330" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
 
 
 Youtube tutorial: `Listing all website contents with sitemaps <https://www.youtube.com/watch?v=uWUyhxciTOs&list=PL-pKWbySIRGMgxXQOtGIz1-nbfYLvqrci&index=3&t=330s>`_
 
 
+Web crawling
+~~~~~~~~~~~~
+
+Selecting the ``--crawl`` option automatically looks for pages by following a fixed number of internal links on the website, starting from the given URL and returning a list of links.
+
+See the `page on web crawling <crawls.html>`_ for more information.
+
+
 URL inspection prior to download and processing
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 
 .. code-block:: bash
 
     $ trafilatura --sitemap "https://www.sitemaps.org/" --list --url-filter "https://www.sitemaps.org/de"
@@ -261,73 +273,70 @@
 For all usage instructions see ``trafilatura -h``:
 
 .. code-block:: bash
 
     trafilatura [-h] [-i INPUTFILE | --input-dir INPUTDIR | -u URL]
                    [--parallel PARALLEL] [-b BLACKLIST] [--list]
                    [-o OUTPUTDIR] [--backup-dir BACKUP_DIR] [--keep-dirs]
-                   [--hash-as-name] [--feed [FEED] | --sitemap [SITEMAP] |
-                   --crawl [CRAWL] | --explore [EXPLORE]] [--archived]
+                   [--feed [FEED] | --sitemap [SITEMAP] | --crawl [CRAWL] |
+                   --explore [EXPLORE]] [--archived]
                    [--url-filter URL_FILTER [URL_FILTER ...]] [-f]
                    [--formatting] [--links] [--images] [--no-comments]
                    [--no-tables] [--only-with-metadata]
                    [--target-language TARGET_LANGUAGE] [--deduplicate]
-                   [--config-file CONFIG_FILE]
-                   [-out {txt,csv,json,xml,xmltei} | --csv | --json | --xml | --xmltei]
+                   [--config-file CONFIG_FILE] [--precision] [--recall]
+                   [-out {txt,csv,json,markdown,xml,xmltei} | --csv | --json |
+                   --markdown | --xml | --xmltei]
                    [--validate-tei] [-v] [--version]
 
 
 Command-line interface for Trafilatura
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --verbose         increase logging verbosity (-v or -vv)
   --version             show version information and exit
 
 Input:
   URLs, files or directories to process
 
-  -i INPUTFILE, --input-file INPUTFILE
+  -i INPUT_FILE, --input-file INPUT_FILE
                         name of input file for batch processing
-  --input-dir INPUTDIR   read files from a specified directory (relative path)
+  --input-dir INPUT_DIR
+                        read files from a specified directory (relative path)
   -u URL, --URL URL     custom URL download
   --parallel PARALLEL   specify a number of cores/threads for downloads and/or
                         processing
   -b BLACKLIST, --blacklist BLACKLIST
                         file containing unwanted URLs to discard during
                         processing
 
 Output:
   Determines if and how files will be written
 
   --list                display a list of URLs without downloading them
-  -o OUTPUTDIR, --output-dir OUTPUTDIR
+  -o OUTPUT_DIR, --output-dir OUTPUT_DIR
                         write results in a specified directory (relative path)
   --backup-dir BACKUP_DIR
                         preserve a copy of downloaded files in a backup
                         directory
   --keep-dirs           keep input directory structure and file names
-  --hash-as-name        use hash value as output file name instead of random
-                        default
 
 Navigation:
   Link discovery and web crawling
 
-  --feed URL            look for feeds and/or pass a feed URL as input
-  --sitemap URL         look for sitemaps for the given website and/or enter a
-                        sitemap URL
-  --crawl URL           crawl a fixed number of pages within a website
-                        starting from the given URL
-  --explore URL         explore the given websites (combination of sitemap and
-                        crawl)
-  --archived            try to fetch URLs from the Internet Archive if
-                        downloads fail
-  --url-filter URL_FILTER
-                        only process/output URLs containing these patterns
-                        (space-separated strings)
+.. code-block:: bash
+
+  --feed [FEED]         look for feeds and/or pass a feed URL as input
+  --sitemap [SITEMAP]   look for sitemaps for the given website and/or enter a sitemap URL
+  --crawl [CRAWL]       crawl a fixed number of pages within a website starting from the given URL
+  --explore [EXPLORE]   explore the given websites (combination of sitemap and crawl)
+  --probe [PROBE]       probe for extractable content (works best with target language)
+  --archived            try to fetch URLs from the Internet Archive if downloads fail
+  --url-filter URL_FILTER [URL_FILTER ...] only process/output URLs containing these patterns (space-separated strings)
 
 Extraction:
   Customization of text and metadata processing
 
   -f, --fast            fast (without fallback detection)
   --formatting          include text formatting (bold, italic, etc.)
   --links               include links along with their targets (experimental)
@@ -343,20 +352,20 @@
                         override standard extraction parameters with a custom
                         config file
   --precision           favor extraction precision (less noise, possibly less
                         text)
   --recall              favor extraction recall (more text, possibly more
                         noise)
 
-
 Format:
   Selection of the output format
 
-  -out, --output-format
-                        determine output format, possible choices:
-                        txt, csv, json, xml, xmltei
-  --csv                 CSV output
-  --json                JSON output
-  --xml                 XML output
-  --xmltei              XML TEI output
+.. code-block:: bash
+
+  -out {txt,csv,json,markdown,xml,xmltei}, --output-format {txt,csv,json,markdown,xml,xmltei} determine output format
+  --csv                 shorthand for CSV output
+  --json                shorthand for JSON output
+  --markdown            shorthand for MD output
+  --xml                 shorthand for XML output
+  --xmltei              shorthand for XML TEI output
   --validate-tei        validate XML TEI output
```

### Comparing `trafilatura-1.8.1/docs/usage-gui.rst` & `trafilatura-1.9.0/docs/usage-gui.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/usage-python.rst` & `trafilatura-1.9.0/docs/usage-python.rst`

 * *Files 3% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 Formats
 ^^^^^^^
 
 Default output is set to TXT (bare text) without metadata.
 
-The following formats are available: bare text, text with Markdown formatting, CSV, JSON, XML, and XML following the guidelines of the Text Encoding Initiative (TEI).
+The following formats are available: bare text, Markdown (from version 1.9 onwards), CSV, JSON, XML, and XML following the guidelines of the Text Encoding Initiative (TEI).
 
 
 .. hint::
     Combining TXT, CSV and JSON formats with certain structural elements (e.g. formatting or links) triggers output in TXT+Markdown format.
 
 The variables from the example above can be used further:
 
@@ -105,15 +105,15 @@
 
     # output with links
     >>> result = extract(downloaded, include_links=True)
     # and so on...
 
 
 .. note::
-    Including extra elements works best with conversion to XML formats (``output_format="xml"``) or ``bare_extraction()``. Both ways allow for direct display and manipulation of the elements. Certain elements are only visible in the output if the chosen format allows it (e.g. images and XML).
+    Including extra elements works best with conversion to XML formats (``output_format="xml"``) or ``bare_extraction()``. Both ways allow for direct display and manipulation of the elements. Certain elements are only visible in the output if the chosen format allows it (e.g. images and XML). Selecting markdown automatically includes text formatting.
 
 
 ``include_formatting=True``
     Keep structural elements related to formatting (``<b>``/``<strong>``, ``<i>``/``<emph>`` etc.)
 ``include_links=True``
     Keep link targets (in ``href="..."``)
 ``include_images=True``
@@ -122,28 +122,32 @@
     Extract text from HTML ``<table>`` elements.
 
 
 Only ``include_tables`` is activated by default.
 
 
 .. hint::
-    If the output is buggy removing a constraint (e.g. formatting) can greatly improve the result.
+    The heuristics used by the main algorithm change according to the presence of certain elements in the HTML. If the output seems odd removing a constraint (e.g. formatting) can greatly improve the result.
 
 
 Optimizing for precision and recall
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 The parameters ``favor_precision`` & ``favor_recall`` can be passed to the ``extract()`` & ``bare_extraction()`` functions:
 
 .. code-block:: python
 
     >>> result = extract(downloaded, url, favor_precision=True)
 
-They slightly affect processing and volume of textual output, respectively concerning precision/accuracy (i.e. more selective extraction, yielding less and more central elements) and recall (i.e. more opportunistic extraction, taking more elements into account).
+They affect processing and volume of textual output:
 
+1. By focusing precision/accuracy, i.e. more selective extraction, yielding less and more central elements.
+   If you believe the results are too noisy, try focusing on precision. Alternatively, you can supply a list of XPaths expressions to target precise HTML elements (``prune_xpath`` parameter of the extraction functions).
+2. By enhancing recall, i.e. more opportunistic extraction, taking more elements into account.
+   If parts of the contents are still missing, see `troubleshooting <troubleshooting.html>`_.
 
 
 html2txt
 ^^^^^^^^
 
 This function emulates the behavior of similar functions in other packages, it is normally used as a last resort during extraction but can be called specifically in order to output all possible text:
 
@@ -159,15 +163,16 @@
 The target language can also be set using 2-letter codes (`ISO 639-1 <https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes>`_), there will be no output if the detected language of the result does not match and no such filtering if the identification component has not been installed (see above `installation instructions <installation.html>`_) or if the target language is not available.
 
 .. code-block:: python
 
     >>> result = extract(downloaded, url, target_language="de")
 
 .. note::
-    Additional components are required: ``pip install trafilatura[all]``
+    Additional components are required: ``pip install trafilatura[all]``.
+    This feature currently uses the `py3langid package <https://github.com/adbar/py3langid>`_ and is dependent on language availability and performance of the original model.
 
 
 Optimizing for speed
 ^^^^^^^^^^^^^^^^^^^^
 
 Execution speed not only depends on the platform and on supplementary packages (``trafilatura[all]``, ``htmldate[speed]``), but also on the extraction strategy.
 
@@ -184,25 +189,14 @@
 
     >>> result = extract(downloaded, include_comments=False, include_tables=False, no_fallback=True)
 
 
 Content hashing
 ^^^^^^^^^^^^^^^
 
-Functions used to build content hashes can be found in `hashing.py <https://github.com/adbar/trafilatura/blob/master/trafilatura/hashing.py>`_.
-
-
-.. code-block:: python
-
-    # create a filename-safe string by hashing the given content
-    >>> from trafilatura.hashing import generate_hash_filename
-    >>> generate_hash_filename("This is a text.")
-    'qAgzZnskrcRgeftk'
-
-
 The `SimHash <https://en.wikipedia.org/wiki/SimHash>`_ method (also called Charikar's hash) allows for near-duplicate detection. It implements a `locality-sensitive hashing <https://en.wikipedia.org/wiki/Locality-sensitive_hashing>`_ method based on a rolling hash and comparisons using the hamming distance. Overall it is reasonably fast and accurate for web texts and can be used to detect near duplicates by fixing a similarity threshold.
 
 
 .. code-block:: python
 
     # create a Simhash for near-duplicate detection
     >>> from trafilatura.hashing import Simhash
@@ -213,32 +207,36 @@
 
     # use existing Simhash
     >>> first_copy = Simhash(existing_hash=first.hash)
     >>> first_copy.similarity(first)
     1.0
 
 
+Other convenience functions include generation of file names based on their content. Two identical or nearly identical files will then get the exact same file name or close enough.
+
+
+.. code-block:: python
+
+    # create a filename-safe string by hashing the given content
+    >>> from trafilatura.hashing import generate_hash_filename
+    >>> generate_hash_filename("This is a text.")
+    'qAgzZnskrcRgeftk'
+
+
 Extraction settings
 -------------------
 
 .. hint::
     See also `settings page <settings.html>`_.
 
 
-Disabling ``signal``
-^^^^^^^^^^^^^^^^^^^^
-
-A timeout exit during extraction can be turned off if malicious data are not an issue or if you run into an error like `signal only works in main thread <https://github.com/adbar/trafilatura/issues/202>`_. In this case, the following code can be useful as it explicitly changes the required setting:
-
-.. code-block:: python
+Function parameters
+^^^^^^^^^^^^^^^^^^^
 
-    >>> from trafilatura.settings import use_config
-    >>> newconfig = use_config()
-    >>> newconfig.set("DEFAULT", "EXTRACTION_TIMEOUT", "0")
-    >>> extract(downloaded, config=newconfig)
+Starting from version 1.9, an object gathering necessary arguments and parameters can be passed to the extraction functions. See `settings.py` for an example.
 
 
 Metadata extraction
 ^^^^^^^^^^^^^^^^^^^
 
 Date
 ~~~~
@@ -269,19 +267,19 @@
 .. code-block:: python
 
     # define a URL and download the example
     >>> url = "https://web.archive.org/web/20210613232513/https://www.thecanary.co/feature/2021/05/19/another-by-election-headache-is-incoming-for-keir-starmer/"
     >>> downloaded = fetch_url(url)
 
     # content discarded since necessary metadata couldn't be extracted
-    >>> bare_extraction(downloaded, with_metadata=True)
+    >>> bare_extraction(downloaded, only_with_metadata=True)
     >>>
 
     # date found in URL, extraction successful
-    >>> bare_extraction(downloaded, with_metadata=True, url=url)
+    >>> bare_extraction(downloaded, only_with_metadata=True, url=url)
 
 
 Memory use
 ^^^^^^^^^^
 
 Trafilatura uses caches to speed up extraction and cleaning processes. This may lead to memory leaks in some cases, particularly in large-scale applications. If that happens you can reset all cached information in order to release RAM:
 
@@ -343,18 +341,20 @@
     >>> extract(mytree)
     'Here is the main text.'
 
 
 Navigation
 ----------
 
+Three potential navigation strategies are currently available: feeds (mostly for fresh content), sitemaps (for exhaustivity, all potential pages as listed by the owners) and discovery by web crawling (i.e. by following the internal links, more experimental).
+
+
 Feeds
 ^^^^^
 
-
 The function ``find_feed_urls`` is a all-in-one utility that attemps to discover the feeds from a webpage if required and/or downloads and parses feeds. It returns the extracted links as list, more precisely as a sorted list of unique links.
 
 .. code-block:: python
 
     # import the feeds module
     >>> from trafilatura import feeds
 
@@ -408,7 +408,17 @@
     # automatically find sitemaps by providing the homepage
     >>> mylinks = sitemaps.sitemap_search('https://www.theguardian.com/')
 
     # the target_lang argument works as explained above
     >>> mylinks = sitemaps.sitemap_search('https://www.un.org/', target_lang='en')
 
 The links are also seamlessly filtered for patterns given by the user, e.g. using ``https://www.theguardian.com/society`` as argument implies taking all URLs corresponding to the society category.
+
+
+Web crawling
+^^^^^^^^^^^^
+
+See the `documentation page on web crawling <crawls.html>`_ for more information.
+
+
+.. hint::
+    For more information on how to refine and filter a URL collection, see the underlying `courlan <https://github.com/adbar/courlan>`_ library.
```

#### html2text {}

```diff
@@ -14,36 +14,37 @@
 successful False # extract information from HTML >>> result = extract
 (downloaded) >>> print(result) # newlines preserved, TXT output ... The only
 required argument is the input document (here a downloaded HTML file), the rest
 is optional. .. note:: For a hands-on tutorial see also the Python Notebook
 `Trafilatura Overview
 github.com/adbar/trafilatura/blob/master/docs/Trafilatura_Overview.ipynb>`_.
 Formats ^^^^^^^ Default output is set to TXT (bare text) without metadata. The
-following formats are available: bare text, text with Markdown formatting, CSV,
-JSON, XML, and XML following the guidelines of the Text Encoding Initiative
-(TEI). .. hint:: Combining TXT, CSV and JSON formats with certain structural
-elements (e.g. formatting or links) triggers output in TXT+Markdown format. The
-variables from the example above can be used further: .. code-block:: python #
-newlines preserved, TXT output >>> extract(downloaded) # TXT/Markdown output
->>> extract(downloaded, include_links=True) # some formatting preserved in
-basic XML structure >>> extract(downloaded, output_format='xml') # source URL
-provided for inclusion in metadata >>> extract(downloaded, output_format='xml',
-url=url) # links preserved in XML, converting relative links to absolute where
-possible >>> extract(downloaded, output_format='xml', include_links=True) #
-source URL must be provided to convert relative links to absolute with TXT
-output >>> extract(downloaded, include_links=True, url=url) Choice of HTML
-elements ^^^^^^^^^^^^^^^^^^^^^^^ Several elements can be included or discarded:
-* Text elements: comments, tables * Structural elements: formatting, images,
-links Their inclusion can be activated or deactivated using paramaters passed
-to the ``extract()`` function: .. code-block:: python # no comments in output
->>> result = extract(downloaded, include_comments=False) # skip tables
-examination >>> result = extract(downloaded, include_tables=False) # output
-with links >>> result = extract(downloaded, include_links=True) # and so on...
-.. note:: Including extra elements works best with conversion to XML formats
-(``output_format="xml"``) or ``bare_extraction()``. Both ways allow for direct
-display and manipulation of the elements. Certain elements are only visible in
-the output if the chosen format allows it (e.g. images and XML).
+following formats are available: bare text, Markdown (from version 1.9
+onwards), CSV, JSON, XML, and XML following the guidelines of the Text Encoding
+Initiative (TEI). .. hint:: Combining TXT, CSV and JSON formats with certain
+structural elements (e.g. formatting or links) triggers output in TXT+Markdown
+format. The variables from the example above can be used further: .. code-
+block:: python # newlines preserved, TXT output >>> extract(downloaded) # TXT/
+Markdown output >>> extract(downloaded, include_links=True) # some formatting
+preserved in basic XML structure >>> extract(downloaded, output_format='xml') #
+source URL provided for inclusion in metadata >>> extract(downloaded,
+output_format='xml', url=url) # links preserved in XML, converting relative
+links to absolute where possible >>> extract(downloaded, output_format='xml',
+include_links=True) # source URL must be provided to convert relative links to
+absolute with TXT output >>> extract(downloaded, include_links=True, url=url)
+Choice of HTML elements ^^^^^^^^^^^^^^^^^^^^^^^ Several elements can be
+included or discarded: * Text elements: comments, tables * Structural elements:
+formatting, images, links Their inclusion can be activated or deactivated using
+paramaters passed to the ``extract()`` function: .. code-block:: python # no
+comments in output >>> result = extract(downloaded, include_comments=False) #
+skip tables examination >>> result = extract(downloaded, include_tables=False)
+# output with links >>> result = extract(downloaded, include_links=True) # and
+so on... .. note:: Including extra elements works best with conversion to XML
+formats (``output_format="xml"``) or ``bare_extraction()``. Both ways allow for
+direct display and manipulation of the elements. Certain elements are only
+visible in the output if the chosen format allows it (e.g. images and XML).
+Selecting markdown automatically includes text formatting.
 ``include_formatting=True`` Keep structural elements related to formatting
 (``````//````````,, ````````//```````` eettcc..)) ````iinncclluuddee__lliinnkkss==TTrruuee```` KKeeeepp lliinnkk ttaarrggeettss ((iinn
 ````hhrreeff==""......""````)) ````iinncclluuddee__iimmaaggeess==TTrruuee```` KKeeeepp ttrraacckk ooff iimmaaggeess aalloonngg wwiitthh tthheeiirr
 ttaarrggeettss ((````[[IImmaaggee]]```` aattttrriibbuutteess:: aalltt,, ssrrcc,, ttiittllee)) ````iinncclluuddee__ttaabblleess==TTrruuee````
 EExxttrraacctt tteexxtt ffrroomm HHTTMMLL ````
```

### Comparing `trafilatura-1.8.1/docs/usage-r.rst` & `trafilatura-1.9.0/docs/usage-r.rst`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/docs/used-by.rst` & `trafilatura-1.9.0/docs/used-by.rst`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 
 Various software repositories
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 - `Benson <https://github.com/timoteostewart/benson>`_, to turn a list of URLs into mp3s of the contents of each web page
 - `CommonCrawl downloader <https://github.com/leogao2/commoncrawl_downloader>`_, to derive massive amounts of language data
 - `DataTrove <https://github.com/huggingface/datatrove>`_, to process, filter and deduplicate text data
+- `Ethical ad server <https://github.com/readthedocs/ethical-ad-server>`_ on ReadTheDocs (hosting these doc pages)
 - `GLAM Workbench <https://glam-workbench.github.io/web-archives/>`_ for cultural heritage (web archives section)
 - `llama-hub <https://github.com/emptycrown/llama-hub>`_, a library of data loaders for large language models
 - `LlamaIndex <https://github.com/run-llama/llama_index>`_, a data framework for LLM applications
 - `Obsei <https://obsei.com/>`_, a text collection and analysis tool
 - `Vulristics <https://github.com/leonov-av/vulristics>`_, a framework for analyzing publicly available information about vulnerabilities
 - `Website-to-Chatbot <https://github.com/Anil-matcha/Website-to-Chatbot>`_, a personalized chatbot
 
@@ -122,55 +123,61 @@
 - Bender, M., Bubenhofer, N., Dreesen, P., Georgi, C., Rüdiger, J. O., & Vogel, F. (2022). Techniken und Praktiken der Verdatung. Diskurse–digital, 135-158.
 - Bevendorff, J., Gupta, S., Kiesel, J., & Stein, B. (2023). An Empirical Comparison of Web Content Extraction Algorithms.
 - Book, L. (2023). Evaluating and comparing different key phrase-based web scraping methods for training domain-specific fasttext models, Master's thesis, KTH Royal Institute of Technology.
 - Bozarth, L., & Budak, C. (2021). "An Analysis of the Partnership between Retailers and Low-credibility News Publishers", Journal of Quantitative Description: Digital Media, 1.
 - Brandon, C., Doherty, A. J., Kelly, D., Leddin, D., & Margaria, T. (2023). HIPPP: Health Information Portal for Patients and Public. Applied Sciences, 13(16), 9453.
 - Braun, D. (2021). "Automated Semantic Analysis, Legal Assessment, and Summarization of Standard Form Contracts", PhD Thesis, Technische Universität München.
 - Chen, X., Zeynali, A., Camargo, C., Flöck, F., Gaffney, D., Grabowicz, P., ... & Samory, M. (2022). SemEval-2022 Task 8: Multilingual news article similarity. In Proceedings of the 16th International Workshop on Semantic Evaluation (SemEval-2022) (pp. 1094-1106).
+- Crummett, L. T., & Aslam, M. H. (2023). Diabetes websites lack information on dietary causes, risk factors, and preventions for type 2 diabetes. Frontiers in Public Health, 11, 1159024.
 - De Cesare, A. M. (2023). Assessing the quality of ChatGPT’s generated output in light of human-written texts: A corpus study based on textual parameters. CHIMERA: Revista de Corpus de Lenguas Romances y Estudios Lingüísticos, 10, 179-210.
 - Di Giovanni, M., Tasca, T., & Brambilla, M. (2022). DataScience-Polimi at SemEval-2022 Task 8: Stacking Language Models to Predict News Article Similarity. In Proceedings of the 16th International Workshop on Semantic Evaluation (SemEval-2022) (pp. 1229-1234).
 - Dumitru, V., Iorga, D., Ruseti, S., & Dascalu, M. (2023). Garbage in, garbage out: An analysis of HTML text extractors and their impact on NLP performance. In 2023 24th International Conference on Control Systems and Computer Science (CSCS) (pp. 403-410). IEEE.
 - Fröbe, M., Hagen, M., Bevendorff, J., Völske, M., Stein, B., Schröder, C., ... & Potthast, M. (2021). "The Impact of Main Content Extraction on Near-Duplicate Detection". arXiv preprint arXiv:2111.10864.
 - Gao, L., Biderman, S., Black, S., Golding, L., Hoppe, T., Foster, C., ... & Leahy, C. (2020). "The Pile: An 800GB Dataset of Diverse Text for Language Modeling", arXiv preprint arXiv:2101.00027.
-- Gopalakrishnan, S., Chen, V. Z., Dou, W., Hahn-Powell, G., Nedunuri, S., & Zadrozny, W. W. (2023). Text to Causal Knowledge Graph: A Framework to Synthesize Knowledge from Unstructured Business Texts into Causal Graphs.
+- Gopalakrishnan, S., Chen, V. Z., Dou, W., Hahn-Powell, G., Nedunuri, S., & Zadrozny, W. W. (2023). Text to Causal Knowledge Graph: A Framework to Synthesize Knowledge from Unstructured Business Texts into Causal Graphs. Information, 14(7), 367.
 - Harrando, I., & Troncy, R. (2021). "Explainable Zero-Shot Topic Extraction Using a Common-Sense Knowledge Graph", In 3rd Conference on Language, Data and Knowledge (LDK 2021). OpenAccess Series in Informatics, Dagstuhl Publishing.
 - Hartmann, S. (2023). Open Corpus Linguistics–or How to overcome common problems in dealing with corpus data by adopting open research practices.
-- Hunter, B., Mathews, F., & Weeds, J. (2023). Using hierarchical text classification to investigate the utility of machine learning in automating online analyses of wildlife exploitation. Ecological Informatics, 102076.
+- Hunter, S. B., Mathews, F., & Weeds, J. (2023). Using hierarchical text classification to investigate the utility of machine learning in automating online analyses of wildlife exploitation. Ecological Informatics, 75, 102076.
+- Hunter, S. B., Oedin, M., Weeds, J., & Mathews, F. (2024). Exploring the potential for online data sources to enhance species threat mapping through the case study of global bat exploitation. Conservation Biology, e14242.
 - Indig, B., Sárközi-Lindner, Z., & Nagy, M. (2022). Use the Metadata, Luke!–An Experimental Joint Metadata Search and N-gram Trend Viewer for Personal Web Archives. In Proceedings of the 2nd International Workshop on Natural Language Processing for Digital Humanities (pp. 47-52).
 - Johannsen, B. (2023). Fußball und safety: Eine framesemantische Perspektive auf Diskurse über trans Sportler* innen. Queere Vielfalt im Fußball, 176.
 - Jung, G., Han, S., Kim, H., Kim, K., & Cha, J. (2022). Extracting the Main Content of Web Pages Using the First Impression Area. IEEE Access, 10, 129958-129969
 - Jung, G., Cha, J. (2023). New Visual Features for HTML Main Content Extraction. Journal of Digital Contents Society.
 - Karabulut, M., & Mayda, İ. (2020). "Development of Browser Extension for HTML Web Page Content Extraction", In 2020 International Congress on Human-Computer Interaction, Optimization and Robotic Applications (HORA) (pp. 1-6). IEEE.
 - Khusainov, A., Suleymanov, D., Gilmullin, R., Minsafina, A., Kubedinova, L., & Abdurakhmonova, N. "First Results of the “TurkLang-7” Project: Creating Russian-Turkic Parallel Corpora and MT Systems", In CMCL (pp. 90-101).
+- Kliche, F., Heid, U., Knackstedt, R., & Klupp, T. (2023, September). An educational Gamebook on computational linguistic methods for the development of taxonomies. In Proceedings of the 1st Workshop on Teaching for NLP (pp. 37-43).
 - Küehn, P., Relke, D. N., & Reuter, C. (2023). Common Vulnerability Scoring System Prediction based on Open Source Intelligence Information Sources. Computers & Security, 103286.
 - Kuehn, P., Schmidt, M., & Reuter, C. (2023). ThreatCrawl: A BERT-based Focused Crawler for the Cybersecurity Domain. arXiv preprint arXiv:2304.11960.
 - Laippala, V., Rönnqvist, S., Hellström, S., Luotolahti, J., Repo, L., Salmela, A., ... & Pyysalo, S. (2020). "From Web Crawl to Clean Register-Annotated Corpora", Proceedings of the 12th Web as Corpus Workshop (pp. 14-22).
 - Laippala, V., Salmela, A., Rönnqvist, S., Aji, A. F., Chang, L. H., Dhifallah, A., ... & Pyysalo, S. (2022). Towards better structured and less noisy Web data: Oscar with Register annotations. In Proceedings of the Eighth Workshop on Noisy User-generated Text (W-NUT 2022) (pp. 215-221).
 - Luukkonen, R., Komulainen, V., Luoma, J., Eskelinen, A., Kanerva, J., Kupari, H. M., ... & Pyysalo, S. (2023). FinGPT: Large Generative Models for a Small Language. arXiv preprint arXiv:2311.05640.
 - Madrid-Morales, D. (2021). "Who Set the Narrative? Assessing the Influence of Chinese Media in News Coverage of COVID-19 in 30 African Countries", Global Media and China, 6(2), 129-151.
 - Meier-Vieracker, S. (2022). "Fußballwortschatz digital–Korpuslinguistische Ressourcen für den Sprachunterricht." Korpora Deutsch als Fremdsprache (KorDaF), 2022/01 (pre-print).
 - Meng, K. (2021). "An End-to-End Computational System for Monitoring and Verifying Factual Claims" (pre-print).
 - Miquelina, N., Quaresma, P., & Nogueira, V. B. (2022). Generating a European Portuguese BERT Based Model Using Content from Arquivo. pt Archive. In International Conference on Intelligent Data Engineering and Automated Learning (pp. 280-288). Springer, Cham.
 - Naira, A. M., & Benelallam, I. (2023). Evaluating ESG Impacts in African Cities through Topic-Level Sentiment Analysis. In 2023 10th International Conference on Wireless Networks and Mobile Communications (WINCOM) (pp. 1-6). IEEE.
 - Nguyen, Q.C., et al. (2024). Rosie, a Health Education Question-and-Answer Chatbot for New Mothers: Randomized Pilot Study. JMIR Formative Research, 8(1), e51361.
 - Nissopoulou, T. X. (2023). Web content classification analysis, MSc thesis, International Hellenic University.
 - Nolda, A., Barbaresi, A., & Geyken, A. (2023). Korpora für die lexikographische Beschreibung diatopischer Variation in der deutschen Standardsprache. Korpora in der germanistischen Sprachwissenschaft: Mündlich, schriftlich, multimedial, 29.
 - Öhman, J., Verlinden, S., Ekgren, A., Gyllensten, A. C., Isbister, T., Gogoulou, E., ... & Sahlgren, M. (2023). The Nordic Pile: A 1.2 TB Nordic Dataset for Language Modeling. arXiv preprint arXiv:2303.17183.
-- Penedo, G., Malartic, Q., Hesslow, D., Cojocaru, R., Cappelli, A., Pannier, B., ... & Launay, J. The RefinedWeb Dataset for Falcon LLM: Outperforming Curated Corpora with Web Data, and Web Data Only.
+- Paster, K., Santos, M. D., Azerbayev, Z., & Ba, J. (2023). Openwebmath: An open dataset of high-quality mathematical web text. arXiv preprint arXiv:2310.06786.
+- Penedo, G., Malartic, Q., Hesslow, D., Cojocaru, R., Alobeidli, H., Cappelli, A., ... & Launay, J. (2024). The RefinedWeb dataset for Falcon LLM: Outperforming curated corpora with web data only. Advances in Neural Information Processing Systems, 36.
 - Piskorski, J., Stefanovitch, N., Da San Martino, G., & Nakov, P. (2023). Semeval-2023 task 3: Detecting the category, the framing, and the persuasion techniques in online news in a multi-lingual setup. In Proceedings of the the 17th International Workshop on Semantic Evaluation (SemEval-2023) (pp. 2343-2361).
 - Pohlmann, J., Barbaresi, A., & Leinen, P. (2023). Platform regulation and “overblocking”–The NetzDG discourse in Germany. Communications, 48(3), 395-419.
 - Rastislav, K. (2024). Backend platformy pro sdílené ověřování faktů (Master's thesis, České vysoké učení technické v Praze. Vypočetní a informační centrum.)
+- Reina, L. A. V. (2023). NLP Meets Agronomy: Document Classification for Plant Health Surveillance, Master's thesis.
 - Robertson, F., Lagus, J., & Kajava, K. (2021). "A COVID-19 news coverage mood map of Europe", Proceedings of the EACL Hackashop on News Media Content Analysis and Automated Report Generation (pp. 110-115).
 - Salmela, A. (2022). "Distinguishing Noise and Main Text Content from Web-Sourced Plain Text Documents Using Sequential Neural Networks", Master's thesis, University of Turku.
 - Sawczyn, A., Binkowski, J., Janiak, D., Augustyniak, Ł., & Kajdanowicz, T. (2021). "Fact-checking: relevance assessment of references in the Polish political domain", Procedia Computer Science, 192, 1285-1293.
 - Schamel, T., Braun, D., & Matthes, F. (2022). Structured Extraction of Terms and Conditions from German and English Online Shops. In Proceedings of The Fifth Workshop on e-Commerce and NLP (ECNLP 5) (pp. 181-190).
 - Sutter, T., Bozkir, A. S., Gehring, B., & Berlich, P. (2022). Avoiding the Hook: Influential Factors of Phishing Awareness Training on Click-Rates and a Data-Driven Approach to Predict Email Difficulty Perception. IEEE Access, 10, 100540-100565.
 - Ter-Akopyan, B. (2022). "Identification of Political Leaning in German News", Master's thesis, Ludwig Maximilian University of Munich.
 - Varlamov, M., Galanin, D., Bedrin, P., Duda, S., Lazarev, V., & Yatskov, A. (2022). A Dataset for Information Extraction from News Web Pages. In 2022 Ivannikov Ispras Open Conference (ISPRAS) (pp. 100-106). IEEE.
 - Waheed, A., Qunaibi, S., Barradas, D., & Weinberg, Z. (2022). Darwin's Theory of Censorship: Analysing the Evolution of Censored Topics with Dynamic Topic Models. In Proceedings of the 21st Workshop on Privacy in the Electronic Society (pp. 103-108).
+- Xu, Z., Liu, Z., Yan, Y., Liu, Z., Xiong, C., & Yu, G. (2024). Cleaner Pretraining Corpus Curation with Neural Web Scraping. arXiv preprint arXiv:2402.14652.
 - Zinn, J. O., & Müller, M. (2021). "Understanding discourse and language of risk", Journal of Risk Research, 1-14.
 
 
 
 Publications citing Htmldate
 ----------------------------
```

### Comparing `trafilatura-1.8.1/setup.py` & `trafilatura-1.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,42 +13,40 @@
     "Return package version as listed in `__version__` in `init.py`"
     initfile = Path(package, "__init__.py").read_text()  # Python >= 3.5
     return re.search("__version__ = ['\"]([^'\"]+)['\"]", initfile)[1]
 
 
 def get_long_description():
     "Return the README"
-    with open("README.rst", "r", encoding="utf-8") as filehandle:
+    with open("README.md", "r", encoding="utf-8") as filehandle:
         long_description = filehandle.read()
-    # long_description += "\n\n"
-    # with open("CHANGELOG.md", encoding="utf8") as f:
-    #    long_description += f.read()
     return long_description
 
 
 # some problems with installation solved this way
 extras = {
     "all": [
         "brotli",
         "cchardet >= 2.1.7; python_version < '3.11'",  # build issue
         "faust-cchardet >= 2.1.19; python_version >= '3.11'",
-        "htmldate[speed] >= 1.8.0",
+        "htmldate[speed] >= 1.8.1",
         "py3langid >= 0.2.2",
         "pycurl >= 7.45.3",
     ],
     "gui": [
         "Gooey >= 1.0.1",
     ],
 }
 
 setup(
     name="trafilatura",
     version=get_version("trafilatura"),
     description="Python package and command-line tool designed to gather text on the Web, includes all necessary discovery and text processing components to perform web crawling, downloads, scraping, and extraction of main texts, metadata and comments.",
     long_description=get_long_description(),
+    long_description_content_type="text/markdown",
     classifiers=[
         # As from https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "Development Status :: 5 - Production/Stable",
         #'Development Status :: 6 - Mature',
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
@@ -107,16 +105,16 @@
     },
     include_package_data=True,
     python_requires=">=3.6",
     install_requires=[
         "certifi",
         "charset_normalizer >= 3.0.1; python_version < '3.7'",
         "charset_normalizer >= 3.2.0; python_version >= '3.7'",
-        "courlan >= 1.0.0",
-        "htmldate >= 1.8.0",
+        "courlan >= 1.1.0",
+        "htmldate >= 1.8.1",
         "importlib_metadata; python_version < '3.8'",
         "justext >= 3.0.0",
         # see tests on Github Actions
         "lxml == 4.9.2 ; platform_system == 'Darwin' and python_version <= '3.8'",
         "lxml >= 4.9.4, < 5.2.0; platform_system != 'Darwin' or python_version > '3.8'",
         "urllib3 >= 1.26, < 2; python_version < '3.7'",
         "urllib3 >= 1.26, < 3; python_version >= '3.7'",
```

### Comparing `trafilatura-1.8.1/tests/cli_tests.py` & `trafilatura-1.9.0/tests/cli_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 import pytest
 from courlan import UrlStore
 
 from trafilatura import cli, cli_utils, settings, spider
 from trafilatura.downloads import add_to_compressed_dict, fetch_url
 from trafilatura.filters import LANGID_FLAG
+from trafilatura.settings import args_to_extractor
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 RESOURCES_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'resources')
 
 
 def test_parser():
     '''test argument parsing for the command-line interface'''
@@ -39,14 +40,19 @@
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     assert args.fast is False
     assert args.verbose == 0
     assert args.output_format == 'csv'
     assert args.no_tables is False
     # test args mapping
+    testargs = ['', '--markdown']
+    with patch.object(sys, 'argv', testargs):
+        args = cli.parse_args(testargs)
+    args = cli.map_args(args)
+    assert args.output_format == 'markdown'
     testargs = ['', '--xml', '--no-comments', '--precision', '--recall']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     args = cli.map_args(args)
     assert args.output_format == 'xml' and args.no_comments is False
     # combination possible (?)
     assert args.precision is True and args.recall is True
@@ -184,15 +190,16 @@
     # test file writing
     testargs = ['', '--csv', '-o', '/dev/null/', '-b', '/dev/null/']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     result = 'DADIDA'
     cli_utils.write_result(result, args)
     # process with backup directory and no counter
-    assert cli_utils.process_result('DADIDA', args, None, None, settings.DEFAULT_CONFIG) is None
+    options = args_to_extractor(args)
+    assert cli_utils.process_result('DADIDA', args, None, options) is None
     # test keeping dir structure
     testargs = ['', '-i', 'myinputdir/', '-o', 'test/', '--keep-dirs']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     filepath, destdir = cli_utils.determine_output_path(args, 'testfile.txt', '')
     assert filepath == 'test/testfile.txt'
     # test hash as output file name
@@ -294,50 +301,60 @@
     # test JSON output
     testargs = ['', '-out', 'json', '--recall']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     with open(os.path.join(RESOURCES_DIR, 'httpbin_sample.html'), 'r', encoding="utf-8") as f:
         teststring = f.read()
     assert cli.examine(teststring, args) is not None
-    # dry-run file processing pipeline
-    testargs = ['', '--parallel', '1', '--input-dir', '/dev/null']
-    with patch.object(sys, 'argv', testargs):
-        args = cli.parse_args(testargs)
-    cli_utils.file_processing_pipeline(args)
-    # file processing pipeline on resources/
-    args.input_dir = RESOURCES_DIR
-    cli_utils.file_processing_pipeline(args)
     # sitemaps: tested in --explore
     testargs = ['', '--sitemap', 'https://sitemaps.org/sitemap.xml', '--list', '--parallel', '1']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     f = io.StringIO()
     with redirect_stdout(f):
         cli.process_args(args)
     assert f.getvalue().strip().endswith("https://www.sitemaps.org/zh_TW/terms.html")
-    # config file
-    testargs = ['', '--input-dir', '/dev/null', '--config-file', 'newsettings.cfg']
-    with patch.object(sys, 'argv', testargs):
-        args = cli.parse_args(testargs)
-    with open(os.path.join(RESOURCES_DIR, 'httpbin_sample.html'), 'r', encoding="utf-8") as f:
-        teststring = f.read()
-    args.config_file = os.path.join(RESOURCES_DIR, args.config_file)
-    # config = use_config(filename=args.config_file)
-    assert cli.examine(teststring, args) is None
     # CLI options
     testargs = ['', '--links', '--images']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
     with open(os.path.join(RESOURCES_DIR, 'http_sample.html'), 'r', encoding="utf-8") as f:
         teststring = f.read()
     result = cli.examine(teststring, args)
-    print(result)
     assert '[link](testlink.html)' in result and 'test.jpg' in result
 
 
+def test_file_processing():
+    "Test file processing pipeline on actual directories."
+    # dry-run file processing pipeline
+    testargs = ['', '--parallel', '1', '--input-dir', '/dev/null']
+    with patch.object(sys, 'argv', testargs):
+        args = cli.parse_args(testargs)
+    cli_utils.file_processing_pipeline(args)
+    # file processing pipeline on resources/
+    args.input_dir = RESOURCES_DIR
+    cli_utils.file_processing_pipeline(args)
+    # test manually
+    options = args_to_extractor(args)
+    for f in cli_utils.generate_filelist(args.input_dir):
+        cli_utils.file_processing(f, args, options=options)
+
+
+def test_cli_config_file():
+    "Test if the configuration file is loaded correctly from the CLI."
+    testargs = ['', '--input-dir', '/dev/null', '--config-file', 'newsettings.cfg']
+    with patch.object(sys, 'argv', testargs):
+        args = cli.parse_args(testargs)
+    with open(os.path.join(RESOURCES_DIR, 'httpbin_sample.html'), 'r', encoding="utf-8") as f:
+        teststring = f.read()
+    args.config_file = os.path.join(RESOURCES_DIR, args.config_file)
+    options = args_to_extractor(args)
+    assert cli.examine(teststring, args, options=options) is None
+
+
 def test_input_filtering():
     '''test internal functions to filter urls'''
     testargs = ['']
     with patch.object(sys, 'argv', testargs):
         args = cli.parse_args(testargs)
 
     # load dictionary
@@ -471,10 +488,12 @@
 if __name__ == '__main__':
     test_parser()
     test_climain()
     test_input_type()
     test_input_filtering()
     test_sysoutput()
     test_cli_pipeline()
+    test_file_processing()
+    test_cli_config_file()
     test_crawling()
     test_download()
     test_probing()
```

### Comparing `trafilatura-1.8.1/tests/downloads_tests.py` & `trafilatura-1.9.0/tests/downloads_tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,35 +22,37 @@
 from unittest.mock import patch
 
 from courlan import UrlStore
 
 from trafilatura.cli import parse_args
 from trafilatura.cli_utils import (download_queue_processing,
                                    url_processing_pipeline)
-from trafilatura.core import extract
+from trafilatura.core import Extractor, extract
 import trafilatura.downloads
 from trafilatura.downloads import (DEFAULT_HEADERS, USER_AGENT, Response,
                                    _determine_headers, _handle_response,
                                    _parse_config, _pycurl_is_live_page,
                                    _send_pycurl_request, _send_urllib_request,
                                    _urllib3_is_live_page,
                                    add_to_compressed_dict, fetch_url,
                                    is_live_page, load_download_buffer)
-from trafilatura.settings import DEFAULT_CONFIG, use_config
+from trafilatura.settings import DEFAULT_CONFIG, args_to_extractor, use_config
 from trafilatura.utils import decode_file, decode_response, load_html
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 
 ZERO_CONFIG = DEFAULT_CONFIG
 ZERO_CONFIG['DEFAULT']['MIN_OUTPUT_SIZE'] = '0'
 ZERO_CONFIG['DEFAULT']['MIN_EXTRACTED_SIZE'] = '0'
 
 RESOURCES_DIR = os.path.join(os.path.abspath(os.path.dirname(__file__)), 'resources')
 UA_CONFIG = use_config(filename=os.path.join(RESOURCES_DIR, 'newsettings.cfg'))
 
+DEFAULT_OPTS = Extractor(config=DEFAULT_CONFIG)
+
 
 def _reset_downloads_global_objects():
     """
     Force global objects to be re-created
     """
     trafilatura.downloads.HTTP_POOL = None
     trafilatura.downloads.NO_CERT_POOL = None
@@ -91,52 +93,52 @@
     # assert _send_urllib_request('https://expired.badssl.com/', False, False, DEFAULT_CONFIG) is not None
     if pycurl is not None:
         assert _send_pycurl_request('https://expired.badssl.com/', False, False, DEFAULT_CONFIG) is not None
     # no SSL, no decoding
     url = 'https://httpbun.com/status/200'
     for no_ssl in (True, False):
         response = _send_urllib_request('https://httpbun.com/status/200', no_ssl, True, DEFAULT_CONFIG)
-        assert response.data == b''
+        assert b"200" in response.data and b"OK" in response.data  # JSON
         assert response.headers["x-powered-by"].startswith("httpbun")
     if pycurl is not None:
         response1 = _send_pycurl_request('https://httpbun.com/status/200', True, True, DEFAULT_CONFIG)
         assert response1.headers["x-powered-by"].startswith("httpbun")
-        assert _handle_response(url, response1, False, DEFAULT_CONFIG) == _handle_response(url, response, False, DEFAULT_CONFIG)
-        assert _handle_response(url, response1, True, DEFAULT_CONFIG) == _handle_response(url, response, True, DEFAULT_CONFIG)
+        assert _handle_response(url, response1, False, DEFAULT_OPTS).data == _handle_response(url, response, False, DEFAULT_OPTS).data
+        assert _handle_response(url, response1, True, DEFAULT_OPTS) == _handle_response(url, response, True, DEFAULT_OPTS)
     # response object
     # too large response object
     data = ""
     status = 200
     url = 'https://httpbin.org/encoding/utf8'
     response = Response(data, status, url)
     # too large
     response.data = b'ABC'*10000000
-    assert _handle_response(response.url, response, False, DEFAULT_CONFIG) is None
+    assert _handle_response(response.url, response, False, DEFAULT_OPTS) is None
     # too small
     response.data = b'ABC'
-    assert _handle_response(response.url, response, False, DEFAULT_CONFIG) is None
+    assert _handle_response(response.url, response, False, DEFAULT_OPTS) is None
     # straight handling of response object
     with open(os.path.join(RESOURCES_DIR, 'utf8.html'), 'rb') as filehandle:
         response.data = filehandle.read()
-    assert _handle_response(response.url, response, False, DEFAULT_CONFIG) is not None
+    assert _handle_response(response.url, response, False, DEFAULT_OPTS) is not None
     assert load_html(response) is not None
     # nothing to see here
     assert extract(response, url=response.url, config=ZERO_CONFIG) is None
     # test handling redirects
-    res = fetch_url('http://httpbin.org/redirect/2')
+    res = fetch_url('https://httpbun.com/redirect/2')
     assert len(res) > 100  # We followed redirects and downloaded something in the end
     new_config = use_config()  # get a new config instance to avoid mutating the default one
     # Patch max directs: limit to 0. We won't fetch any page as a result
     new_config.set('DEFAULT', 'MAX_REDIRECTS', '0')
     _reset_downloads_global_objects()  # force Retry strategy and PoolManager to be recreated with the new config value
-    res = fetch_url('http://httpbin.org/redirect/1', config=new_config)
+    res = fetch_url('https://httpbun.com/redirect/1', config=new_config)
     assert res is None
     # Also test max redir implementation on pycurl if available
     if pycurl is not None:
-        assert _send_pycurl_request('http://httpbin.org/redirect/1', True, False, new_config) is None
+        assert _send_pycurl_request('https://httpbun.com/redirect/1', True, False, new_config) is None
     _reset_downloads_global_objects()  # reset global objects again to avoid affecting other tests
 
 def test_config():
     '''Test how configuration options are read and stored.'''
     # default config is none
     assert _parse_config(DEFAULT_CONFIG) == (None, None)
     # default accept-encoding
@@ -193,18 +195,18 @@
     testargs = ['', '-v']
     with patch.object(sys, 'argv', testargs):
         args = parse_args(testargs)
     inputurls = ['https://httpbun.com/status/301', 'https://httpbun.com/status/304', 'https://httpbun.com/status/200', 'https://httpbun.com/status/300', 'https://httpbun.com/status/400', 'https://httpbun.com/status/505']
     url_store = add_to_compressed_dict(inputurls)
     args.archived = True
     args.config_file = os.path.join(RESOURCES_DIR, 'newsettings.cfg')
-    config = use_config(filename=args.config_file)
-    config['DEFAULT']['SLEEP_TIME'] = '0.2'
-    results = download_queue_processing(url_store, args, None, config)
-    assert len(results[0]) == 6 and results[1] is None
+    options = args_to_extractor(args)
+    options.config['DEFAULT']['SLEEP_TIME'] = '0.2'
+    results = download_queue_processing(url_store, args, None, options)
+    assert len(results[0]) == 5 and results[1] is None
 
 
 if __name__ == '__main__':
     test_response_object()
     test_fetch()
     test_config()
     test_decode()
```

### Comparing `trafilatura-1.8.1/tests/feeds_tests.py` & `trafilatura-1.9.0/tests/feeds_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/filters_tests.py` & `trafilatura-1.9.0/tests/filters_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,15 @@
 from trafilatura.metadata import Document
 from trafilatura.settings import DEFAULT_CONFIG
 
 ZERO_CONFIG = DEFAULT_CONFIG
 ZERO_CONFIG['DEFAULT']['MIN_OUTPUT_SIZE'] = '0'
 ZERO_CONFIG['DEFAULT']['MIN_EXTRACTED_SIZE'] = '0'
 
-DEFAULT_OPTIONS = Extractor(*[False]*11)
-DEFAULT_OPTIONS.config = DEFAULT_CONFIG
+DEFAULT_OPTIONS = Extractor()
 
 SAMPLE_META = Document()
 
 
 def test_filters():
     '''Test content filtering'''
     if LANGID_FLAG is True:
@@ -106,47 +105,48 @@
 
 
 def test_lrucache():
     '''test basic duplicate detection'''
     lru_test = LRUCache(maxsize=2)
     trafilatura.filters.LRU_TEST = lru_test
     my_body = etree.Element('body')
+    
     ### element too short
     #my_element = html.fromstring('<p>AAAA BBBB</p>')
     #my_body.append(my_element)
     #put_in_cache(my_body)
     #assert duplicate_test(my_element, DEFAULT_CONFIG) is False
     ### cached element
     my_element = html.fromstring('<p>AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB AAAA BBBB</p>')
     my_body.append(my_element)
-    assert duplicate_test(my_element, DEFAULT_CONFIG) is False
-    assert duplicate_test(my_element, DEFAULT_CONFIG) is False
-    assert duplicate_test(my_body, DEFAULT_CONFIG) is False
-    assert duplicate_test(my_element, DEFAULT_CONFIG) is True
+    assert duplicate_test(my_element, DEFAULT_OPTIONS) is False
+    assert duplicate_test(my_element, DEFAULT_OPTIONS) is False
+    assert duplicate_test(my_body, DEFAULT_OPTIONS) is False
+    assert duplicate_test(my_element, DEFAULT_OPTIONS) is True
     other_body = etree.Element('body')
     other_element = html.fromstring('<p>CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD CCCC DDDD</p>')
     other_body.append(other_element)
-    assert duplicate_test(other_body, DEFAULT_CONFIG) is False
-    assert duplicate_test(other_element, DEFAULT_CONFIG) is False
-    assert duplicate_test(other_body, DEFAULT_CONFIG) is False
-    assert duplicate_test(other_element, DEFAULT_CONFIG) is True
+    assert duplicate_test(other_body, DEFAULT_OPTIONS) is False
+    assert duplicate_test(other_element, DEFAULT_OPTIONS) is False
+    assert duplicate_test(other_body, DEFAULT_OPTIONS) is False
+    assert duplicate_test(other_element, DEFAULT_OPTIONS) is True
     yet_another_body = etree.Element('body')
     yet_another_element = html.fromstring('<p>EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF EEEE FFFF</p>')
     yet_another_body.append(yet_another_element)
-    assert duplicate_test(yet_another_body, DEFAULT_CONFIG) is False
-    assert duplicate_test(yet_another_body, DEFAULT_CONFIG) is False
-    assert duplicate_test(yet_another_body, DEFAULT_CONFIG) is False
+    assert duplicate_test(yet_another_body, DEFAULT_OPTIONS) is False
+    assert duplicate_test(yet_another_body, DEFAULT_OPTIONS) is False
+    assert duplicate_test(yet_another_body, DEFAULT_OPTIONS) is False
     # 2 elements in cache, original element has been cleared?
     # print(LRU_TEST.maxsize, LRU_TEST.full)
-    assert duplicate_test(other_element, DEFAULT_CONFIG) is True
-    assert duplicate_test(yet_another_element, DEFAULT_CONFIG) is True
-    assert duplicate_test(my_element, DEFAULT_CONFIG) is False
+    assert duplicate_test(other_element, DEFAULT_OPTIONS) is True
+    assert duplicate_test(yet_another_element, DEFAULT_OPTIONS) is True
+    assert duplicate_test(my_element, DEFAULT_OPTIONS) is False
     # clear the cache
     lru_test.clear()
-    assert duplicate_test(other_element, DEFAULT_CONFIG) is False
+    assert duplicate_test(other_element, DEFAULT_OPTIONS) is False
     # get wrong key
     assert lru_test.get('tralala') == -1
 
 
 def test_prune_xpath():
     '''test xpath pruning (parameter in extract and bare_extraction)'''
     #create example html
@@ -175,8 +175,8 @@
     assert extract(doc2()) != ''
     assert extract(doc3()) != ''
 
 
 if __name__ == '__main__':
     test_filters()
     test_lrucache()
-    test_prune_xpath()
+    test_prune_xpath()
```

### Comparing `trafilatura-1.8.1/tests/hashing_tests.py` & `trafilatura-1.9.0/tests/hashing_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/json_metadata_tests.py` & `trafilatura-1.9.0/tests/json_metadata_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/metadata_tests.py` & `trafilatura-1.9.0/tests/metadata_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 
 
 def test_titles():
     '''Test the extraction of titles'''
     # too short/empty
     metadata = extract_metadata('<html><body><h3 class="title">T</h3><h3 id="title"></h3></body></html>')
     assert metadata.title is None
-
+    metadata = extract_metadata('<html><head><title>Test Title</title><meta property="og:title" content=" " /></head><body><h1>First</h1></body></html>')
+    assert metadata.title == 'First'
+    metadata = extract_metadata('<html><head><title>Test Title</title><meta name="title" content=" " /></head><body><h1>First</h1></body></html>')
+    assert metadata.title == 'First'
     metadata = extract_metadata('<html><head><title>Test Title</title></head><body></body></html>')
     assert metadata.title == 'Test Title'
     metadata = extract_metadata('<html><body><h1>First</h1><h1>Second</h1></body></html>')
     assert metadata.title == 'First'
     metadata = extract_metadata('<html><body><h1>   </h1><div class="post-title">Test Title</div></body></html>')
     assert metadata.title == 'Test Title'
     metadata = extract_metadata('<html><body><h2 class="block-title">Main menu</h2><h1 class="article-title">Test Title</h1></body></html>')
@@ -186,18 +189,18 @@
     metadata = extract_metadata('<html><head><meta property="og:published_time" content="2017-09-01"/></head><body></body></html>')
     assert metadata.date == '2017-09-01'
     metadata = extract_metadata('<html><head><meta property="og:url" content="https://example.org/2017/09/01/content.html"/></head><body></body></html>')
     assert metadata.date == '2017-09-01'
     metadata = extract_metadata('<html><head><meta property="og:url" content="https://example.org/2017/09/01/content.html"/></head><body></body></html>')
     assert metadata.date == '2017-09-01'
     mystring = '<html><body><p>Veröffentlicht am 1.9.17</p></body></html>'
-    metadata = extract_metadata(mystring, fastmode=False)
+    metadata = extract_metadata(mystring, extensive=True)
     assert metadata.date == '2017-09-01'
     # behavior for fastmode=True changed in htmldate==1.6.0. On 1.5.2 and earlier, result was None
-    metadata = extract_metadata(mystring, fastmode=True)
+    metadata = extract_metadata(mystring, extensive=False)
     assert metadata.date == '2017-09-01'
 
 
 def test_sitename():
     '''Test extraction of site name'''
     metadata = extract_metadata('<html><head><meta name="article:publisher" content="@"/></head><body/></html>')
     assert metadata.sitename is None
```

### Comparing `trafilatura-1.8.1/tests/resources/apache.html` & `trafilatura-1.9.0/tests/resources/apache.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/feed.json` & `trafilatura-1.9.0/tests/resources/feed.json`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/feed1.atom` & `trafilatura-1.9.0/tests/resources/feed1.atom`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/feed2.rss` & `trafilatura-1.9.0/tests/resources/feed2.rss`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/http_sample.html` & `trafilatura-1.9.0/tests/resources/http_sample.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/httpbin_sample.html` & `trafilatura-1.9.0/tests/resources/httpbin_sample.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/newsettings.cfg` & `trafilatura-1.9.0/tests/resources/newsettings.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/scam.html` & `trafilatura-1.9.0/tests/resources/scam.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/sitemap-hreflang.xml` & `trafilatura-1.9.0/tests/resources/sitemap-hreflang.xml`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/sitemap.xml` & `trafilatura-1.9.0/tests/resources/sitemap.xml`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/utf8.html` & `trafilatura-1.9.0/tests/resources/utf8.html`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/webpage.html.gz` & `trafilatura-1.9.0/tests/resources/webpage.html.gz`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/resources/zerolength.cfg` & `trafilatura-1.9.0/tests/resources/zerolength.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/sitemaps_tests.py` & `trafilatura-1.9.0/tests/sitemaps_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/spider_tests.py` & `trafilatura-1.9.0/tests/spider_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/tests/unit_tests.py` & `trafilatura-1.9.0/tests/unit_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # pylint:disable-msg=I1101,W1401
 """
 Unit tests for the trafilatura library.
 """
 
 import logging
-import os
 import sys
 import time
 
 from copy import copy
+from os import path
 
 import pytest
 
 from lxml import etree, html
 
 try:
     from cchardet import detect
@@ -24,55 +24,56 @@
     import py3langid
     LANGID_FLAG = True
 except ImportError:
     LANGID_FLAG = False
 
 import trafilatura.htmlprocessing
 from trafilatura import (bare_extraction, baseline, extract, html2txt,
-                         process_record, utils, xml)
-from trafilatura.core import (Extractor, handle_formatting, handle_image,
-                              handle_lists, handle_paragraphs, handle_quotes,
-                              handle_table, handle_textelem, sanitize_tree,
-                              trim)
-from trafilatura.external import try_justext
+                         process_record, xml)
+from trafilatura.core import Extractor
+from trafilatura.external import sanitize_tree, try_justext
 from trafilatura.filters import textfilter
+from trafilatura.main_extractor import (handle_formatting, handle_image,
+                                        handle_lists, handle_paragraphs, handle_quotes,
+                                        handle_table, handle_textelem)
 from trafilatura.meta import reset_caches
 from trafilatura.metadata import Document
 from trafilatura.settings import DEFAULT_CONFIG, TAG_CATALOG, use_config
+from trafilatura.utils import (detect_encoding, is_dubious_html, is_image_file, load_html,
+                               normalize_unicode, repair_faulty_html, sanitize, trim)
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 
 
-TEST_DIR = os.path.abspath(os.path.dirname(__file__))
-RESOURCES_DIR = os.path.join(TEST_DIR, 'resources')
+TEST_DIR = path.abspath(path.dirname(__file__))
+RESOURCES_DIR = path.join(TEST_DIR, 'resources')
 SAMPLE_META = Document()
 
 ZERO_CONFIG = DEFAULT_CONFIG
 ZERO_CONFIG['DEFAULT']['MIN_OUTPUT_SIZE'] = '0'
 ZERO_CONFIG['DEFAULT']['MIN_EXTRACTED_SIZE'] = '0'
 
-NEW_CONFIG = use_config(filename=os.path.join(RESOURCES_DIR, 'newsettings.cfg'))
+NEW_CONFIG = use_config(filename=path.join(RESOURCES_DIR, 'newsettings.cfg'))
 
 MOCK_PAGES = {
 'http://exotic_tags': 'exotic_tags.html',
 }
 
-DEFAULT_OPTIONS = Extractor(*[False]*11)
-DEFAULT_OPTIONS.config = DEFAULT_CONFIG
+DEFAULT_OPTIONS = Extractor()
 
 
 def load_mock_page(url, xml_flag=False, langcheck=None, tei_output=False):
     '''load mock page from samples'''
     try:
-        with open(os.path.join(TEST_DIR, 'resources', MOCK_PAGES[url]), 'r') as inputf:
+        with open(path.join(TEST_DIR, "resources", MOCK_PAGES[url]), "r", encoding="utf-8") as inputf:
             htmlstring = inputf.read()
     # encoding/windows fix for the tests
     except UnicodeDecodeError:
         # read as binary
-        with open(os.path.join(TEST_DIR, 'resources', MOCK_PAGES[url]), 'rb') as inputf:
+        with open(path.join(TEST_DIR, "resources", MOCK_PAGES[url]), "rb") as inputf:
             htmlbinary = inputf.read()
         guessed_encoding = detect(htmlbinary)['encoding']
         if guessed_encoding is not None:
             try:
                 htmlstring = htmlbinary.decode(guessed_encoding)
             except UnicodeDecodeError:
                 htmlstring = htmlbinary
@@ -99,66 +100,73 @@
     assert textfilter(my_elem) is False
     # my_elem.text = 'Tags: Arbeit, Urlaub'
     my_elem.text = 'Instagram'
     assert textfilter(my_elem) is True
     my_elem.text = '\t\t'
     assert textfilter(my_elem) is True
     # sanitize logic
-    assert utils.sanitize(None) is None
+    assert sanitize(None) is None
     # non-breaking spaces
-    print(utils.sanitize('Test&nbsp;Text'))
-    assert utils.sanitize('Test&nbsp;Text') == 'Test Text'
+    print(sanitize('Test&nbsp;Text'))
+    assert sanitize('Test&nbsp;Text') == 'Test Text'
     # clear cache
     # reset caches: examine_date_elements used above
     old_values = trim.cache_info()
     reset_caches()
     assert trim.cache_info() != old_values
 
 
 def test_input():
     '''test if loaded strings/trees are handled properly'''
-    assert utils.is_dubious_html("This is a string.") is True
+    teststring = "高山云雾出好茶".encode("utf-8")
+    assert detect_encoding(teststring) == ["utf-8"]
+    teststring = "高山云雾出好茶".encode("gb18030")
+    assert "gb18030" in detect_encoding(teststring)
+    assert "gb18030" in detect_encoding(teststring*1000)
+
+    assert is_dubious_html("This is a string.") is True
 
     htmlstring = "<!DOCTYPE html PUBLIC />\n<html></html>"
     beginning = htmlstring[:50].lower()
-    assert utils.repair_faulty_html(htmlstring, beginning) == "\n<html></html>"
+    assert repair_faulty_html(htmlstring, beginning) == "\n<html></html>"
 
     htmlstring = "<html>\n</html>"
     beginning = htmlstring[:50].lower()
-    assert utils.repair_faulty_html(htmlstring, beginning) == htmlstring
+    assert repair_faulty_html(htmlstring, beginning) == htmlstring
 
     htmlstring = "<html/>\n</html>"
     beginning = htmlstring[:50].lower()
-    assert utils.repair_faulty_html(htmlstring, beginning) == "<html>\n</html>"
+    assert repair_faulty_html(htmlstring, beginning) == "<html>\n</html>"
 
     htmlstring = '<!DOCTYPE html>\n<html lang="en-US"/>\n<head/>\n<body/>\n</html>'
     beginning = htmlstring[:50].lower()
     assert (
-        utils.repair_faulty_html(htmlstring, beginning)
+        repair_faulty_html(htmlstring, beginning)
         == '<!DOCTYPE html>\n<html lang="en-US">\n<head/>\n<body/>\n</html>'
     )
 
     with pytest.raises(TypeError) as err:
-        assert utils.load_html(123) is None
+        assert load_html(123) is None
     assert 'incompatible' in str(err.value)
-    assert utils.load_html('<html><body>ÄÖÜ</body></html>') is not None
-    assert utils.load_html(b'<html><body>\x2f\x2e\x9f</body></html>') is not None
-    assert utils.load_html('<html><body>\x2f\x2e\x9f</body></html>'.encode('latin-1')) is not None
-    #assert utils.load_html(b'0'*int(10e3)) is None
+    assert load_html('<html><body>ÄÖÜ</body></html>') is not None
+    assert load_html(b'<html><body>\x2f\x2e\x9f</body></html>') is not None
+    assert load_html('<html><body>\x2f\x2e\x9f</body></html>'.encode('latin-1')) is not None
+    #assert load_html(b'0'*int(10e3)) is None
     # old: with pytest.raises(TypeError) as err:
     assert extract(None, 'url', '0000', target_language=None) is None
     # legacy
-    assert process_record(None, 'url', '0000', target_language=None) is None
+    with pytest.raises(SystemExit):
+        assert process_record(None, 'url', '0000', target_language=None) is None
     # GZip
-    with open(os.path.join(RESOURCES_DIR, 'webpage.html.gz'), 'rb') as gzfile:
+    with open(path.join(RESOURCES_DIR, 'webpage.html.gz'), 'rb') as gzfile:
         myinput = gzfile.read()
     assert 'Long story short,' in extract(myinput)
 
     # unicode normalization
-    assert utils.normalize_unicode('A\u0308ffin') != 'A\u0308ffin'
+    assert normalize_unicode('A\u0308ffin') != 'A\u0308ffin'
     testresult = extract('<html><body><p>A\u0308ffin</p></body></html>', config=ZERO_CONFIG)
     assert testresult != 'A\u0308ffin' and testresult == 'Äffin'
 
 
 def test_xmltocsv():
     doc = Document()
     doc.body = etree.fromstring('<xml/>')
@@ -176,15 +184,15 @@
     comments = 'Test comment'
     doc.body = etree.fromstring(f'<p>{text}</p>')
     doc.commentsbody = etree.fromstring(f'<p>{comments}</p>')
 
     target = 'https://example.org\t1\tnull\texample.org\tTest title\thttps://example.org/image.jpg\tnull\tTest text\tTest comment\tCC BY-SA\tarticle\r\n'
 
     assert xml.xmltocsv(doc, False) == target
-    
+
     mystring = '<html><body><p>ÄÄÄÄÄÄÄÄÄÄÄÄÄÄ</p></body></html>'
     assert extract(mystring, output_format='csv', config=ZERO_CONFIG) is not None
     assert extract(mystring, output_format='csv', include_comments=False, config=ZERO_CONFIG).endswith('\tnull\r\n')
 
 
 def test_tojson():
     # test json
@@ -194,25 +202,25 @@
     assert extract(mystring, output_format='json', include_comments=False, config=ZERO_CONFIG).endswith('}')
 
 
 def test_python_output():
     # bare extraction for python
     mystring = '<html><body><p>ÄÄÄÄÄÄÄÄÄÄÄÄÄÄ</p></body></html>'
     result = bare_extraction(mystring, config=ZERO_CONFIG, as_dict=True)
-    assert isinstance(result, dict) and len(result) == 20
+    assert isinstance(result, dict) and len(result) == 21
 
 
 def test_exotic_tags(xmloutput=False):
     options = DEFAULT_OPTIONS
-    options.config = ZERO_CONFIG
+    options._add_config(ZERO_CONFIG)
     # cover some edge cases with a specially crafted file
     result = load_mock_page('http://exotic_tags', xml_flag=xmloutput, tei_output=True)
     assert 'Teletype text' in result and 'My new car is silver.' in result
-    filepath = os.path.join(TEST_DIR, 'resources', 'exotic_tags_tei.html')
-    with open(filepath) as f:
+    filepath = path.join(TEST_DIR, 'resources', 'exotic_tags_tei.html')
+    with open(filepath, "r", encoding="utf-8") as f:
         content = etree.fromstring(f.read())
     res = xml.check_tei(content, 'http://dummy')
     assert etree.tostring(res).startswith(b'<html>\n<text>\n<body>\n<div>\n\n<hi rend="uppercase">Hello</hi>\n<p>Teletype text</p>')
     # misformed HTML declaration
     htmlstring = '<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" 2012"http://www.w3.org/TR/html4/loose.dtd"><html><head></head><body><p>ABC</p></body></html>'
     # outputs '012"http://www.w3.org/TR/html4/loose.dtd">\nABC'
     assert 'ABC' in extract(htmlstring, config=ZERO_CONFIG)
@@ -286,32 +294,43 @@
     my_result = extract(my_document, output_format='xml', config=ZERO_CONFIG)
     assert 'lb' not in my_result
     # simple formatting
     my_document = html.fromstring('<html><body><p><b>This here is in bold font.</b></p></body></html>')
     my_result = extract(my_document, output_format='xml', include_formatting=True, config=ZERO_CONFIG)
     assert '<hi rend="#b">This here is in bold font.</hi>' in my_result
     # titles as markdown
-    my_document = html.fromstring('<html><body><article><h3>Title</h3><p><b>This here is in bold font.</b></p></article></body></html>')
+    my_string = '<html><body><article><h3>Title</h3><p><b>This here is in bold font.</b></p></article></body></html>'
+    my_document = html.fromstring(my_string)
     my_result = extract(my_document, output_format='txt', include_formatting=True, config=ZERO_CONFIG)
     assert my_result == '### Title\n**This here is in bold font.**'
+    assert extract(my_string, output_format='markdown', config=ZERO_CONFIG) == my_result
+    assert '<hi rend="#b">' in etree.tostring(bare_extraction(my_string, output_format='markdown', config=ZERO_CONFIG)["body"], encoding="unicode")
+
+    # space between paragraphs
+    my_document = html.fromstring('<html><body><article><h3>Title</h3><p>Paragraph 1</p><p>Paragraph 2</p></article></body></html>')
+    my_result = extract(my_document, output_format='txt', include_formatting=True, config=ZERO_CONFIG)
+    assert my_result.endswith('Paragraph 1\n\nParagraph 2')
+
     # code sections
     my_document = html.fromstring('<html><body><article><h3>Title</h3><p>Here is a code sample:</p><code>import trafilatura</code></p></article></body></html>')
     my_result = extract(my_document, output_format='txt', include_formatting=True, config=ZERO_CONFIG)
     assert my_result == """### Title
 Here is a code sample:
+
 `import trafilatura`"""
     my_document = html.fromstring('<html><body><article><h3>Title</h3><p>Here is a code sample:</p><code>import trafilatura\ntrafilatura.extract("")</code></p></article></body></html>')
     my_result = extract(my_document, output_format='txt', include_formatting=True, config=ZERO_CONFIG)
     assert my_result == """### Title
 Here is a code sample:
+
 ```
 import trafilatura
 trafilatura.extract("")
 ```"""
-    
+
     # nested
     my_document = html.fromstring('<html><body><p><b>This here is in bold and <i>italic</i> font.</b></p></body></html>')
     my_result = extract(my_document, output_format='xml', include_formatting=True, config=ZERO_CONFIG)
     assert '<hi rend="#b">This here is in bold and italic font.</hi>' in my_result
     # empty
     my_document = html.fromstring('<html><body><p><b><i></i></b></p></body></html>')
     my_result = extract(my_document, output_format='xml', include_formatting=True, config=ZERO_CONFIG)
@@ -334,15 +353,15 @@
     doc = html.fromstring('<html><body><p><br/>Here is the text.</p></body></html>')
     my_result = extract(doc, config=ZERO_CONFIG)
     assert my_result == 'Here is the text.'
     # handle formatting tails
     element = etree.Element("hi")
     element.text = 'Here is the text.'
     element.tail = 'And a tail.'
-    options.config = ZERO_CONFIG
+    options._add_config(ZERO_CONFIG)
     converted = handle_formatting(element, options)
     assert etree.tostring(converted) == b'<p><hi>Here is the text.</hi>And a tail.</p>'
     # empty elements
     my_document = html.fromstring('<html><body><div>\t\n</div><div>There is text here.</div></body></html>')
     my_result = extract(my_document, output_format='xml', config=ZERO_CONFIG)
     assert '<main>\n    <p>There is text here.</p>\n  </main>' in my_result
     # lists with links
@@ -438,39 +457,39 @@
     myelems = {element.tag for element in set(mytree.iter())}
     assert 'graphic' in myelems and 'ref' in myelems
     # test langid
     if LANGID_FLAG is True:
         doc = html.fromstring('<html><body>' + '<p>Non è inglese.</p>'*20 + '</body></html>')
         assert extract(doc, no_fallback=False, target_language='en', deduplicate=False) is None
     # no tables
-    with open(os.path.join(RESOURCES_DIR, 'apache.html')) as f:
+    with open(path.join(RESOURCES_DIR, "apache.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     assert 'localhost:80' in extract(teststring, no_fallback=False, include_tables=True)
     assert 'localhost:80' not in extract(teststring, no_fallback=False, include_tables=False)
-    with open(os.path.join(RESOURCES_DIR, 'scam.html')) as f:
+    with open(path.join(RESOURCES_DIR, "scam.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     assert extract(teststring, no_fallback=True, include_tables=False) == ''
     assert extract(teststring, no_fallback=False, include_tables=False) == ''
     # invalid XML attributes: namespace colon in attribute key (issue #375). Those attributes should be stripped
     bad_xml = 'Testing<ul style="" padding:1px; margin:15px""><b>Features:</b> <li>Saves the cost of two dedicated phone lines.</li> al station using Internet or cellular technology.</li> <li>Requires no change to the existing Fire Alarm Control Panel configuration. The IPGSM-4G connects directly to the primary and secondary telephone ports.</li>'
     res = extract(bad_xml, output_format='xml')
     assert "Features" in res
 
 def test_images():
     '''Test image extraction function'''
     # file type
-    assert utils.is_image_file('test.jpg') is True
-    assert utils.is_image_file('test.txt') is False
+    assert is_image_file('test.jpg') is True
+    assert is_image_file('test.txt') is False
     # tag with attributes
     assert handle_image(html.fromstring('<img src="test.jpg"/>')) is not None
     assert handle_image(html.fromstring('<img data-src="test.jpg" alt="text" title="a title"/>')) is not None
     assert handle_image(html.fromstring('<img other="test.jpg"/>')) is None
     # HTML conversion
     assert handle_textelem(etree.Element('graphic'), [], DEFAULT_OPTIONS) is None
-    with open(os.path.join(RESOURCES_DIR, 'http_sample.html')) as f:
+    with open(path.join(RESOURCES_DIR, "http_sample.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     assert '![Example image](test.jpg)' not in extract(teststring)
     assert '![Example image](test.jpg)' in extract(teststring, include_images=True, no_fallback=True)
     assert '<graphic src="test.jpg" title="Example image"/>' in extract(teststring, include_images=True, no_fallback=True, output_format='xml', config=ZERO_CONFIG)
     assert extract('<html><body><article><img data-src="test.jpg" alt="text" title="a title"/></article></body></html>', include_images=True, no_fallback=True) == '![a title text](test.jpg)'
 
     # CNN example
@@ -482,15 +501,15 @@
     myimage = handle_image(mydoc)
     assert myimage is not None and 'alt' in myimage.attrib and 'src' in myimage.attrib and myimage.get('src').startswith('http')
 
 
 def test_links():
     '''Test link extraction function'''
     options = DEFAULT_OPTIONS
-    options.config = ZERO_CONFIG
+    options._add_config(ZERO_CONFIG)
     assert handle_textelem(etree.Element('ref'), [], options) is None
     assert handle_formatting(html.fromstring('<a href="testlink.html">Test link text.</a>'), options) is not None
     # empty link
     mydoc = html.fromstring('<html><body><p><a></a><b>Some text.</b></p></body></html>')
     assert extract(mydoc) is not None
     # link with target
     mydoc = html.fromstring('<html><body><p><a href="testlink.html">Test link text.</a> This part of the text has to be long enough.</p></body></html>')
@@ -500,37 +519,37 @@
     assert '[Test link text.](https://www.example.com/testlink.html) This part of the text has to be long enough.' in extract(copy(mydoc), url='https://www.example.com/', include_links=True, no_fallback=True, config=ZERO_CONFIG)
     # link without target
     mydoc = html.fromstring('<html><body><p><a>Test link text.</a> This part of the text has to be long enough.</p></body></html>')
     assert '[Test link text.] This part of the text has to be long enough.' in extract(copy(mydoc), include_links=True, no_fallback=True, config=ZERO_CONFIG)
     mydoc = html.fromstring('<html><body><article><a>Segment 1</a><h1><a>Segment 2</a></h1><p>Segment 3</p></article></body></html>')
     result = extract(copy(mydoc), output_format='xml', include_links=True, no_fallback=True, config=ZERO_CONFIG)
     assert '1' in result and '2' in result and '3' in result
-    with open(os.path.join(RESOURCES_DIR, 'http_sample.html')) as f:
+    with open(path.join(RESOURCES_DIR, "http_sample.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     assert 'testlink.html' not in extract(teststring, config=ZERO_CONFIG)
     assert '[link](testlink.html)' in extract(teststring, include_links=True, no_fallback=True, config=ZERO_CONFIG)
     assert '<ref target="testlink.html">link</ref>' in extract(teststring, include_links=True, no_fallback=True, output_format='xml', config=ZERO_CONFIG)
     # test license link
     mydoc = html.fromstring('<html><body><p>Test text under <a rel="license" href="">CC BY-SA license</a>.</p></body></html>')
     assert 'license="CC BY-SA license"' in extract(mydoc, include_links=True, no_fallback=True, output_format='xml', config=ZERO_CONFIG)
 
 
 def test_tei():
     '''test TEI-related functions'''
     # open local resources to avoid redownloading at each run
-    with open(os.path.join(RESOURCES_DIR, 'httpbin_sample.html')) as f:
+    with open(path.join(RESOURCES_DIR, "httpbin_sample.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     # download, parse and validate simple html file
     result1 = extract(teststring, "mocked", no_fallback=True, output_format='xmltei', tei_validation=False)
     result2 = extract(teststring, "mocked", no_fallback=True, output_format='xmltei', tei_validation=True)
     assert result1 is not None and result1 == result2
     assert xml.validate_tei(etree.fromstring(result1)) is True
     assert xml.validate_tei(etree.fromstring(teststring)) is False
     # test with another file
-    with open(os.path.join(RESOURCES_DIR, 'http_sample.html')) as f:
+    with open(path.join(RESOURCES_DIR, "http_sample.html"), "r", encoding="utf-8") as f:
         teststring = f.read()
     # download, parse and validate simple html file
     result = extract(teststring, "mocked", no_fallback=True, include_comments=True, output_format='xmltei', tei_validation=False)
     assert result is not None # and '<p>license</p>' in result
     assert xml.validate_tei(etree.fromstring(result)) is True
     result = extract(teststring, "mocked", no_fallback=True, include_comments=False, output_format='xmltei', tei_validation=False)
     assert result is not None # and '<p>license</p>' in result
@@ -621,15 +640,15 @@
             <p><p>
               <span><p>content</p></span>
             </p></p>
         </body>
         </html>"""
     )
     tree = xml.remove_empty_elements(xml.strip_double_tags(tree))
-    result = utils.sanitize(etree.tostring(tree, encoding="unicode")).replace("\n", "")
+    result = sanitize(etree.tostring(tree, encoding="unicode")).replace("\n", "")
     assert result == "<html><body><p><span>content</span></p></body></html>"
     tree = html.fromstring(
     """
     <html>
         <body>
             <div>
                 <div>
@@ -780,44 +799,53 @@
 def test_extraction_options():
     '''Test the different parameters available in extract() and bare_extraction()'''
     my_html = '<html><head><meta http-equiv="content-language" content="EN"/></head><body><div="article-body"><p>Text.<!-- comment --></p></div></body></html>'
     with pytest.raises(NameError) as err:
         extract(my_html, json_output=True)
     assert extract(my_html, config=NEW_CONFIG) is None
     assert extract(my_html, config=ZERO_CONFIG) is not None
-    assert extract(my_html, with_metadata=True, output_format='xml', config=ZERO_CONFIG) is None
+    assert extract(my_html, with_metadata=True, output_format='xml', config=ZERO_CONFIG) is not None
     assert extract(my_html, only_with_metadata=True, output_format='xml', config=ZERO_CONFIG) is None
     assert extract(my_html, target_language='de', config=ZERO_CONFIG) is None
     assert etree.tostring(try_justext(html.fromstring(my_html), None, 'de')) == b'<body/>'
     # assert extract(my_html) is None
 
     my_html = '<html><head/><body>' + '<p>ABC def ghi jkl.</p>'*1000 + '<p>Posted on 1st Dec 2019<.</p></body></html>'
     assert bare_extraction(my_html, config=ZERO_CONFIG)["date"] is not None
     assert bare_extraction(my_html, config=NEW_CONFIG)["date"] is None
 
 
 def test_precision_recall():
     '''test precision- and recall-oriented settings'''
     # the test cases could be better
     my_document = html.fromstring('<html><body><p>This here is the text.</p></body></html>')
-    assert extract(my_document, favor_precision=True, config=ZERO_CONFIG, fast=True) is not None
-    assert extract(my_document, favor_recall=True, config=ZERO_CONFIG, fast=True) is not None
+    assert extract(copy(my_document), favor_precision=True, config=ZERO_CONFIG, fast=True) is not None
+    assert extract(copy(my_document), favor_recall=True, config=ZERO_CONFIG, fast=True) is not None
+
     my_document = html.fromstring('<html><body><div class="article-body"><div class="teaser-content"><p>This here is a teaser text.</p></div><div><p>This here is the text.</p></div></body></html>')
-    assert 'teaser text' in extract(my_document, favor_recall=True, config=ZERO_CONFIG, fast=True)
-    assert 'teaser text' not in extract(my_document, config=ZERO_CONFIG, fast=True)
-    assert 'teaser text' not in extract(my_document, favor_precision=True, config=ZERO_CONFIG, fast=True)
+    assert 'teaser text' in extract(copy(my_document), favor_recall=True, config=ZERO_CONFIG, fast=True)
+    assert 'teaser text' not in extract(copy(my_document), config=ZERO_CONFIG, fast=True)
+    assert 'teaser text' not in extract(copy(my_document), favor_precision=True, config=ZERO_CONFIG, fast=True)
+
     my_document = html.fromstring('<html><body><article><div><p><a href="test.html">1.</a><br/><a href="test2.html">2.</a></p></div></article></body></html>')
-    result = extract(my_document, favor_recall=True, config=ZERO_CONFIG, fast=True)
+    result = extract(copy(my_document), favor_recall=True, config=ZERO_CONFIG, fast=True)
     assert '1' not in result
-    result = extract(my_document, favor_precision=True, config=ZERO_CONFIG, fast=True)
+    result = extract(copy(my_document), favor_precision=True, config=ZERO_CONFIG, fast=True)
     assert '1' not in result
+
     my_document = html.fromstring('<html><body><div class="article-body"><p>content</p><h2>Test</h2></div></body></html>')
-    result = extract(my_document, favor_precision=True, config=ZERO_CONFIG, fast=True)
+    result = extract(copy(my_document), favor_precision=True, config=ZERO_CONFIG, fast=True)
     assert 'content' in result and 'Test' not in result
 
+    my_document = html.fromstring('<html><body><article><aside><p>Here is the text.</p></aside></article></body></html>')
+    result = extract(copy(my_document), favor_recall=False, config=ZERO_CONFIG, fast=True)
+    assert result != "Here is the text."
+    result = extract(copy(my_document), favor_recall=True, config=ZERO_CONFIG, fast=True)
+    assert result == "Here is the text."
+
 
 def test_table_processing():
     options = DEFAULT_OPTIONS
     table_simple_cell = html.fromstring(
         "<table><tr><td>cell1</td><td>cell2</td></tr><tr><td>cell3</td><td>cell4</td></tr></table>"
     )
     processed_table = handle_table(table_simple_cell, TAG_CATALOG, options)
@@ -860,14 +888,15 @@
             </html>"""
     )
     processed = extract(
         htmlstring, no_fallback=True, output_format='xml', config=DEFAULT_CONFIG, include_links=True
     )
     result = processed.replace('\n', '').replace(' ', '')
     assert """<table><row><cell>text<head>more_text</head></cell></row></table>""" in result
+
     table_cell_w_text_and_child = html.fromstring(
         "<table><tr><td>text<lb/><p>more text</p></td></tr></table>"
     )
     processed_table = handle_table(
         table_cell_w_text_and_child, TAG_CATALOG, options
     )
     assert (
@@ -900,14 +929,15 @@
         table_with_head, TAG_CATALOG, options
     )
     first_row = processed_table[0]
     assert len(processed_table) == 3
     assert [
         (child.tag, child.attrib, child.text) for child in first_row.iterdescendants()
     ] == [("cell", {"role": "head"}, "Month"), ("cell", {"role": "head"}, "Days")]
+
     table_with_head_spanning_two_cols = html.fromstring(
         """<table>
       <tr>
         <th>Name</th>
         <th>Adress</th>
         <th colspan="2">Phone</th>
       </tr>
@@ -959,14 +989,15 @@
         <cell>I buy</cell>
         <cell>you buy</cell>
         <cell>he/she/it buys</cell>
         <cell>we buy</cell>
         <cell>you buy</cell>
         <cell>they buy</cell>
       </row>''' in my_result
+    assert extract(htmlstring, no_fallback=True, output_format='txt').startswith("Present Tense | I buy | you buy |")
     # table with links
     # todo: further tests and adjustsments
     htmlstring = '<html><body><article><table><tr><td><a href="test.html">' + 'ABCD'*100 + '</a></td></tr></table></article></body></html>'
     result = extract(htmlstring, no_fallback=True, output_format='xml', config=ZERO_CONFIG, include_tables=True, include_links=True)
     assert 'ABCD' not in result
     # nested table
     htmlstring = '<html><body><article><table><th>1</th><table><tr><td>2</td></tr></table></table></article></body></html>'
@@ -1019,33 +1050,44 @@
     <list>
       <item>one</item>
       <item>two</item>
     </list>
     </td>
     </tr></table>
     """)
-    processed_table = handle_table(table_with_list, TAG_CATALOG, options)
+    processed_table = handle_table(copy(table_with_list), TAG_CATALOG, options)
     result = [
         (el.tag, el.text) if el.text is not None and el.text.strip() else el.tag
         for el in processed_table.iter()
     ]
-    # assert result == ["table", "row", "cell", ("p", "a list"), "list", ("item", "one"), ("item", "two"),]
     assert result == ['table', 'row', 'cell', ('p', 'a list'), 'list']
+
+    options.focus = "recall"
+    processed_table = handle_table(copy(table_with_list), TAG_CATALOG, options)
+    result = [
+        (el.tag, el.text) if el.text is not None and el.text.strip() else el.tag
+        for el in processed_table.iter()
+    ]
+    assert result == ["table", "row", "cell", ("p", "a list"), 'list', ("item", "one"), ("item", "two"),]
+
     broken_table = html.fromstring("<table><td>cell1</td><tr><td>cell2</td></tr></table>")
     processed_table = handle_table(broken_table, TAG_CATALOG, options)
     result = [el.tag for el in processed_table.iter()]
     assert result == ['table', 'row', 'cell', 'row', 'cell']
     broken_table = html.fromstring("<table><tr><p>text</p></tr><tr><td>cell</td></tr></table>")
     processed_table = handle_table(broken_table, TAG_CATALOG, options)
     result = [el.tag for el in processed_table.iter()]
     assert result == ["table", "row", "cell", ]
     # table nested in figure https://github.com/adbar/trafilatura/issues/301
     htmlstring = '<html><body><article><figure><table><th>1</th><tr><td>2</td></tr></table></figure></article></body></html>'
     result = extract(htmlstring, no_fallback=True, output_format='xml', config=ZERO_CONFIG, include_tables=True)
     assert "1" in result and "2" in result
+    # table headers in non-XML formats
+    htmlstring = '<html><body><article><table><tr><th>head 1</th><th>head 2</th></tr><tr><td>1</td><td>2</td></tr></table></article></body></html>'
+    assert "---|---|" in extract(htmlstring, no_fallback=True, output_format='txt', config=ZERO_CONFIG, include_tables=True)
 
 
 def test_list_processing():
     options = DEFAULT_OPTIONS
     # malformed lists (common error)
     result = etree.tostring(handle_lists(etree.fromstring('<list>Description of the list:<item>List item 1</item><item>List item 2</item><item>List item 3</item></list>'), options))
     assert result.count(b'List item') == 3
@@ -1243,15 +1285,25 @@
         ]
         for sample in samples:
             result = extract(sample['html'], no_fallback=False, config=ZERO_CONFIG)
             detected = py3langid.classify(result)[0]
             assert detected == sample['expected'], f"Lang detection failed for {sample['expected']}"
 
 
+def test_config_loading():
+    "Check if the config file is read correctly."
+    with pytest.raises(FileNotFoundError):
+        config = use_config(filename="/bogus-dir/bogus-file.txt")
+
+    config = use_config(filename=path.join(RESOURCES_DIR, "newsettings.cfg"))
+    assert config is not None
+
+
 if __name__ == '__main__':
+    test_config_loading()
     test_trim()
     test_input()
     test_formatting()
     test_exotic_tags()
     test_images()
     test_links()
     test_htmlprocessing()
```

### Comparing `trafilatura-1.8.1/tests/xml_tei_tests.py` & `trafilatura-1.9.0/tests/xml_tei_tests.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/__init__.py` & `trafilatura-1.9.0/trafilatura/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 """
 
 
 __title__ = 'trafilatura'
 __author__ = 'Adrien Barbaresi and contributors'
 __license__ = "Apache-2.0"
 __copyright__ = 'Copyright 2019-2024, Adrien Barbaresi'
-__version__ = '1.8.1'
+__version__ = '1.9.0'
 
 
 import logging
 
-from .core import bare_extraction, baseline, extract, html2txt, process_record
+from .baseline import baseline, html2txt
+from .core import bare_extraction, extract, process_record
 from .downloads import fetch_response, fetch_url
 from .metadata import extract_metadata
 from .utils import load_html
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
```

### Comparing `trafilatura-1.8.1/trafilatura/cli.py` & `trafilatura-1.9.0/trafilatura/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,17 +26,17 @@
     import codecs
     if sys.stdout.encoding != 'UTF-8':
         sys.stdout = codecs.getwriter('utf-8')(sys.stdout.buffer, 'strict')
     if sys.stderr.encoding != 'UTF-8':
         sys.stderr = codecs.getwriter('utf-8')(sys.stderr.buffer, 'strict')
 
 
-def parse_args(args):
-    """Define parser for command-line arguments"""
-    parser = argparse.ArgumentParser(description='Command-line interface for Trafilatura')
+def add_args(parser):
+    "Add argument groups and arguments to parser."
+
     group1 = parser.add_argument_group('Input', 'URLs, files or directories to process')
     group1_ex = group1.add_mutually_exclusive_group()
     group2 = parser.add_argument_group('Output', 'Determines if and how files will be written')
     group3 = parser.add_argument_group('Navigation', 'Link discovery and web crawling')
     group3_ex = group3.add_mutually_exclusive_group()
     group4 = parser.add_argument_group('Extraction', 'Customization of text and metadata processing')
     group5 = parser.add_argument_group('Format', 'Selection of the output format')
@@ -154,22 +154,25 @@
     group4.add_argument("--recall",
                         help="favor extraction recall (more text, possibly more noise)",
                         action="store_true")
 
     # https://docs.python.org/3/library/argparse.html#argparse.ArgumentParser.add_mutually_exclusive_group
     group5_ex.add_argument('-out', '--output-format',
                         help="determine output format",
-                        choices=['txt', 'csv', 'json', 'xml', 'xmltei'],
+                        choices=['txt', 'csv', 'json', 'markdown', 'xml', 'xmltei'],
                         default='txt')
     group5_ex.add_argument("--csv",
                         help="shorthand for CSV output",
                         action="store_true")
     group5_ex.add_argument("--json",
                         help="shorthand for JSON output",
                         action="store_true")
+    group5_ex.add_argument("--markdown",
+                        help="shorthand for MD output",
+                        action="store_true")
     group5_ex.add_argument("--xml",
                         help="shorthand for XML output",
                         action="store_true")
     group5_ex.add_argument("--xmltei",
                         help="shorthand for XML TEI output",
                         action="store_true")
     group5.add_argument("--validate-tei",
@@ -182,26 +185,34 @@
     parser.add_argument(
         "--version",
         help="show version information and exit",
         action="version",
         version=f"Trafilatura {__version__} - Python {python_version()}",
     )
 
+    return parser
 
+
+def parse_args(args):
+    """Define parser for command-line arguments"""
+    parser = argparse.ArgumentParser(description='Command-line interface for Trafilatura')
+    parser = add_args(parser)
     # wrap in mapping to prevent invalid input
     return map_args(parser.parse_args())
 
 
 def map_args(args):
     '''Map existing options to format and output choices.'''
     # formats
     if args.csv:
         args.output_format = 'csv'
     elif args.json:
         args.output_format = 'json'
+    elif args.markdown:
+        args.output_format = 'markdown'
     elif args.xml:
         args.output_format = 'xml'
     elif args.xmltei:
         args.output_format = 'xmltei'
     # output configuration
     if args.nocomments is False:
         args.no_comments = False
```

### Comparing `trafilatura-1.8.1/trafilatura/cli_utils.py` & `trafilatura-1.9.0/trafilatura/cli_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,36 @@
 import gzip
 import logging
 import random
 import re
 import string
 import sys
 import traceback
+
 from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
+from datetime import datetime
 from functools import partial
 from os import makedirs, path, walk
 
 from courlan import UrlStore, extract_domain, get_base_url  # validate_url
 
 from trafilatura import spider
 
-from .core import extract, html2txt
+from .baseline import html2txt
+from .core import extract
 from .downloads import (add_to_compressed_dict, buffered_downloads,
                         load_download_buffer)
 from .feeds import find_feed_urls
 from .filters import LANGID_FLAG, language_classifier
 from .hashing import generate_hash_filename
 from .meta import reset_caches
-from .settings import FILENAME_LEN, MAX_FILES_PER_DIRECTORY, use_config
+from .settings import FILENAME_LEN, MAX_FILES_PER_DIRECTORY, args_to_extractor
 from .sitemaps import sitemap_search
-from .utils import URL_BLACKLIST_REGEX, make_chunks, uniquify_list
+from .utils import URL_BLACKLIST_REGEX, make_chunks
+
 
 LOGGER = logging.getLogger(__name__)
 
 random.seed(345)  # make generated file names reproducible
 CHAR_CLASS = string.ascii_letters + string.digits
 
 STRIP_DIR = re.compile(r'[^/]+$')
@@ -63,15 +67,15 @@
                 input_urls = [getattr(args, arg)]
                 break
 
     if not input_urls:
         LOGGER.warning('No input provided')
 
     # uniq URLs while preserving order (important)
-    return uniquify_list(input_urls)
+    return list(dict.fromkeys(input_urls))
 
 
 def load_blacklist(filename):
     '''Read list of unwanted URLs'''
     with open(filename, 'r', encoding='utf-8') as inputfh:
         # if validate_url(url)[0] is True:
         blacklist = {URL_BLACKLIST_REGEX.sub('', line.strip()) for line in inputfh}
@@ -181,65 +185,67 @@
 def generate_filelist(inputdir):
     '''Walk the directory tree and output all file names'''
     for root, _, inputfiles in walk(inputdir):
         for fname in inputfiles:
             yield path.join(root, fname)
 
 
-def file_processing(filename, args, counter=None, config=None):
+def file_processing(filename, args, counter=None, options=None):
     '''Aggregated functions to process a file in a list'''
     with open(filename, 'rb') as inputf:
         htmlstring = inputf.read()
-    result = examine(htmlstring, args, url=args.URL, config=config)
+    options.source = filename
+    options.date_params["max_date"] = datetime.fromtimestamp(path.getctime(filename)).strftime("%Y-%m-%d")
+    result = examine(htmlstring, args, options=options)
     write_result(result, args, filename, counter, new_filename=None)
 
 
-def process_result(htmlstring, args, url, counter, config):
+def process_result(htmlstring, args, counter, options):
     '''Extract text and metadata from a download webpage and eventually write out the result'''
     # backup option
     fileslug = archive_html(htmlstring, args, counter) if args.backup_dir else None
     # process
-    result = examine(htmlstring, args, url=url, config=config)
+    result = examine(htmlstring, args, options=options)
     write_result(result, args, orig_filename=fileslug, counter=counter, new_filename=fileslug)
     # increment written file counter
     if counter is not None and result is not None:
         counter += 1
     return counter
 
 
-def download_queue_processing(url_store, args, counter, config):
+def download_queue_processing(url_store, args, counter, options):
     '''Implement a download queue consumer, single- or multi-threaded'''
-    sleep_time = config.getfloat('DEFAULT', 'SLEEP_TIME')
     errors = []
     while url_store.done is False:
-        bufferlist, url_store = load_download_buffer(url_store, sleep_time)
+        bufferlist, url_store = load_download_buffer(url_store, options.config.getfloat('DEFAULT', 'SLEEP_TIME'))
         # process downloads
-        for url, result in buffered_downloads(bufferlist, args.parallel):
+        for url, result in buffered_downloads(bufferlist, args.parallel, options=options):
             # handle result
             if result is not None:
-                counter = process_result(result, args, url, counter, config)
+                options.url = url
+                counter = process_result(result, args, counter, options)
             else:
                 LOGGER.warning('No result for URL: %s', url)
                 errors.append(url)
     return errors, counter
 
 
 def cli_discovery(args):
     "Group CLI functions dedicated to URL discovery."
     url_store = load_input_dict(args)
     input_urls = url_store.dump_urls()
     if args.list:
         url_store.reset()
 
-    config = use_config(filename=args.config_file)
+    options = args_to_extractor(args)
     func = partial(
                find_feed_urls if args.feed else sitemap_search,
                target_lang=args.target_language,
-               external=config.getboolean('DEFAULT', 'EXTERNAL_URLS'),
-               sleep_time=config.getfloat('DEFAULT', 'SLEEP_TIME')
+               external=options.config.getboolean('DEFAULT', 'EXTERNAL_URLS'),
+               sleep_time=options.config.getfloat('DEFAULT', 'SLEEP_TIME')
            )
 
     # link discovery and storage
     with ThreadPoolExecutor(max_workers=args.parallel) as executor:
         futures = (executor.submit(func, url) for url in input_urls)
         # process results from the parallel threads and add them
         # to the compressed URL dictionary for further processing
@@ -255,15 +261,15 @@
     # process the (rest of the) links found
     error_caught = url_processing_pipeline(args, url_store)
 
     # activate site explorer
     if args.explore:
         # add to compressed dict and crawl the remaining websites
         control_dict = build_exploration_dict(url_store, input_urls, args)
-        cli_crawler(args, url_store=control_dict)
+        cli_crawler(args, url_store=control_dict, options=options)
 
 
 def build_exploration_dict(url_store, input_urls, args):
     "Find domains for which nothing has been found and add info to the crawl dict."
     input_domains = {extract_domain(u) for u in input_urls}
     known_domains = {extract_domain(u) for u in url_store.get_known_domains()}
     still_to_crawl = input_domains - known_domains
@@ -273,19 +279,20 @@
                        blacklist=args.blacklist,
                        url_filter=args.url_filter,
                        verbose=args.verbose
                    )
     return control_dict
 
 
-def cli_crawler(args, n=30, url_store=None):
+def cli_crawler(args, n=30, url_store=None, options=None):
     '''Start a focused crawler which downloads a fixed number of URLs within a website
        and prints the links found in the process'''
-    config = use_config(filename=args.config_file)
-    sleep_time = config.getfloat('DEFAULT', 'SLEEP_TIME')
+    if not options:
+        options = args_to_extractor(args)
+    sleep_time = options.config.getfloat('DEFAULT', 'SLEEP_TIME')
     # counter = None
     # load input URLs
     if url_store is None:
         spider.URL_STORE.add_urls(load_input_urls(args))
     else:
         spider.URL_STORE = url_store
     # load crawl data
@@ -298,15 +305,15 @@
             # TODO: register changes?
             # if base_url != hostname:
             # ...
     # iterate until the threshold is reached
     while spider.URL_STORE.done is False:
         bufferlist, spider.URL_STORE = load_download_buffer(spider.URL_STORE, sleep_time)
         # start several threads
-        for url, result in buffered_downloads(bufferlist, args.parallel, decode=False):
+        for url, result in buffered_downloads(bufferlist, args.parallel, decode=False, options=options):
             base_url = get_base_url(url)
             # handle result
             if result is not None:
                 spider.process_response(result, base_url, args.target_language, rules=spider.URL_STORE.get_rules(base_url))
                 # just in case a crawl delay is specified in robots.txt
                 # sleep(spider.get_crawl_delay(spider.URL_STORE.get_rules(base_url)))
         # early exit if maximum count is reached
@@ -316,92 +323,86 @@
     print('\n'.join(u for u in spider.URL_STORE.dump_urls()))
     #return todo, known_links
 
 
 def probe_homepage(args):
     "Probe websites for extractable content and print the fitting ones."
     input_urls = load_input_urls(args)
-    config = use_config(filename=args.config_file)
-    min_length = config.getint('DEFAULT', 'MIN_EXTRACTED_SIZE')
+    options = args_to_extractor(args)
 
-    for url, result in buffered_downloads(input_urls, args.parallel):
+    for url, result in buffered_downloads(input_urls, args.parallel, options=options):
         if result is not None:
             result = html2txt(result)
-            if result and len(result) > min_length and any(c.isalpha() for c in result):
+            if result and len(result) > options.min_extracted_size and any(c.isalpha() for c in result):
                 if not LANGID_FLAG or not args.target_language or language_classifier(result, "") == args.target_language:
                     print(url, flush=True)
 
 
 def url_processing_pipeline(args, url_store):
     '''Aggregated functions to show a list and download and process an input list'''
     # print list without further processing
     if args.list:
         url_store.print_unvisited_urls()  # and not write_result()
         return False  # and not sys.exit(0)
-    # parse config
-    config = use_config(filename=args.config_file)
+
+    options = args_to_extractor(args)
+
     # initialize file counter if necessary
     if url_store.total_url_number() > MAX_FILES_PER_DIRECTORY:
         counter = 0
     else:
         counter = None
     # download strategy
-    errors, counter = download_queue_processing(url_store, args, counter, config)
+    errors, counter = download_queue_processing(url_store, args, counter, options)
     LOGGER.debug('%s URLs could not be found', len(errors))
     # option to retry
     if args.archived is True:
         url_store = UrlStore()
         url_store.add_urls(['https://web.archive.org/web/20/' + e for e in errors])
         if len(url_store.find_known_urls('https://web.archive.org')) > 0:
-            archived_errors, _ = download_queue_processing(url_store, args, counter, config)
+            archived_errors, _ = download_queue_processing(url_store, args, counter, options)
             LOGGER.debug('%s archived URLs out of %s could not be found', len(archived_errors), len(errors))
             # pass information along if URLs are missing
             return bool(archived_errors)
     # pass information along if URLs are missing
     return bool(errors)
 
 
 def file_processing_pipeline(args):
     '''Define batches for parallel file processing and perform the extraction'''
     filecounter = None
-    config = use_config(filename=args.config_file)
-    timeout = config.getint('DEFAULT', 'EXTRACTION_TIMEOUT') or None
+    options = args_to_extractor(args)
+    timeout = options.config.getint('DEFAULT', 'EXTRACTION_TIMEOUT')
 
     # max_tasks_per_child available in Python >= 3.11
     with ProcessPoolExecutor(max_workers=args.parallel) as executor:
         # chunk input: https://github.com/python/cpython/issues/74028
         for filebatch in make_chunks(generate_filelist(args.input_dir), MAX_FILES_PER_DIRECTORY):
             if filecounter is None and len(filebatch) >= MAX_FILES_PER_DIRECTORY:
                 filecounter = 0
-            worker = partial(file_processing, args=args, counter=filecounter, config=config)
+            worker = partial(file_processing, args=args, counter=filecounter, options=options)
             executor.map(worker, filebatch, chunksize=10, timeout=timeout)
             # update counter
             if filecounter is not None:
                 filecounter += len(filebatch)
 
 
-def examine(htmlstring, args, url=None, config=None):
+def examine(htmlstring, args, url=None, options=None):
     """Generic safeguards and triggers"""
     result = None
-    if config is None:
-        config = use_config(filename=args.config_file)
+    if not options:
+        options = args_to_extractor(args, url)
     # safety check
     if htmlstring is None:
         sys.stderr.write('ERROR: empty document\n')
-    elif len(htmlstring) > config.getint('DEFAULT', 'MAX_FILE_SIZE'):
+    elif len(htmlstring) > options.max_file_size:
         sys.stderr.write('ERROR: file too large\n')
-    elif len(htmlstring) < config.getint('DEFAULT', 'MIN_FILE_SIZE'):
+    elif len(htmlstring) < options.min_file_size:
         sys.stderr.write('ERROR: file too small\n')
     # proceed
     else:
         try:
-            result = extract(htmlstring, url=url, no_fallback=args.fast,
-                             include_comments=args.no_comments, include_tables=args.no_tables,
-                             include_formatting=args.formatting, include_links=args.links,
-                             include_images=args.images, only_with_metadata=args.only_with_metadata,
-                             output_format=args.output_format, tei_validation=args.validate_tei,
-                             target_language=args.target_language, deduplicate=args.deduplicate,
-                             favor_precision=args.precision, favor_recall=args.recall, config=config)
+            result = extract(htmlstring, options=options)
         # ugly but efficient
         except Exception as err:
             sys.stderr.write(f'ERROR: {str(err)}' + '\n' + traceback.format_exc() + '\n')
     return result
```

### Comparing `trafilatura-1.8.1/trafilatura/data/jt-stopwords-pickle.lzma` & `trafilatura-1.9.0/trafilatura/data/jt-stopwords-pickle.lzma`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/data/tei-schema-pickle.lzma` & `trafilatura-1.9.0/trafilatura/data/tei-schema-pickle.lzma`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/downloads.py` & `trafilatura-1.9.0/trafilatura/downloads.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 
 import logging
 import random
 import warnings
 
 from concurrent.futures import ThreadPoolExecutor, as_completed
+from functools import partial
 from io import BytesIO
 from time import sleep
 
 import certifi
 import urllib3
 
 try:
@@ -30,18 +31,16 @@
 from courlan.network import redirection_test
 
 try:  # Python 3.8+
     from importlib.metadata import version
 except ImportError:
     from importlib_metadata import version
 
-
-from .settings import DEFAULT_CONFIG
-from .utils import (URL_BLACKLIST_REGEX, decode_file,
-                    make_chunks, uniquify_list)
+from .settings import DEFAULT_CONFIG, Extractor
+from .utils import URL_BLACKLIST_REGEX, decode_file, make_chunks
 
 
 LOGGER = logging.getLogger(__name__)
 
 NUM_CONNECTIONS = 50
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
@@ -161,52 +160,55 @@
         if with_headers:
             resp.store_headers(response.headers)
         return resp
     # catchall
     return None
 
 
-def _handle_response(url, response, decode, config):
+def _handle_response(url, response, decode, options):
     'Internal function to run safety checks on response result.'
     lentest = len(response.html or response.data or "")
     if response.status != 200:
         LOGGER.error('not a 200 response: %s for URL %s', response.status, url)
-    elif lentest < config.getint('DEFAULT', 'MIN_FILE_SIZE'):
+    elif lentest < options.min_file_size:
         LOGGER.error('too small/incorrect for URL %s', url)
         # raise error instead?
-    elif lentest > config.getint('DEFAULT', 'MAX_FILE_SIZE'):
+    elif lentest > options.max_file_size:
         LOGGER.error('too large: length %s for URL %s', lentest, url)
         # raise error instead?
     else:
         return response.html if decode else response
     # catchall
     return None
 
 
-def fetch_url(url, decode=True, no_ssl=False, config=DEFAULT_CONFIG):
+def fetch_url(url, decode=True, no_ssl=False, config=DEFAULT_CONFIG, options=None):
     """Downloads a web page and seamlessly decodes the response.
 
     Args:
         url: URL of the page to fetch.
         no_ssl: Don't try to establish a secure connection (to prevent SSLError).
         config: Pass configuration values for output control.
+        options: Extraction options (supersedes config).
 
     Returns:
         Unicode string or None in case of failed downloads and invalid results.
 
     """
     if not decode:
         warnings.warn(
             """Raw response objects will be deprecated for fetch_url,
                use fetch_response instead.""",
              PendingDeprecationWarning
         )
     response = fetch_response(url, decode=decode, no_ssl=no_ssl, config=config)
     if response is not None and response != '':
-        return _handle_response(url, response, decode, config)
+        if not options:
+            options = Extractor(config=config)
+        return _handle_response(url, response, decode, options)
         # return '' (useful do discard further processing?)
         # return response
     return None
 
 
 def fetch_response(url, *, decode=False, no_ssl=False, with_headers=False, config=DEFAULT_CONFIG):
     """Downloads a web page and returns a full response object.
@@ -279,15 +281,15 @@
     if url_store is None:
         url_store = UrlStore(
                         compressed=compression,
                         strict=False,
                         verbose=verbose
                     )
 
-    inputlist = uniquify_list(inputlist)
+    inputlist = list(dict.fromkeys(inputlist))
 
     if blacklist:
         inputlist = [u for u in inputlist if URL_BLACKLIST_REGEX.sub('', u) not in blacklist]
 
     if url_filter:
         inputlist = [u for u in inputlist if any(f in u for f in url_filter)]
 
@@ -295,28 +297,29 @@
     return url_store
 
 
 def load_download_buffer(url_store, sleep_time=5):
     '''Determine threading strategy and draw URLs respecting domain-based back-off rules.'''
     bufferlist = []
     while not bufferlist:
-        bufferlist = url_store.get_download_urls(timelimit=sleep_time)
+        bufferlist = url_store.get_download_urls(time_limit=sleep_time, max_urls=10**5)
         # add emptiness test or sleep?
         if not bufferlist:
             if url_store.done is True:
                 break
             sleep(sleep_time)
     return bufferlist, url_store
 
 
-def buffered_downloads(bufferlist, download_threads, decode=True):
+def buffered_downloads(bufferlist, download_threads, decode=True, options=None):
     '''Download queue consumer, single- or multi-threaded.'''
+    worker = partial(fetch_url, decode=decode, options=options)
     with ThreadPoolExecutor(max_workers=download_threads) as executor:
         for chunk in make_chunks(bufferlist, 10000):
-            future_to_url = {executor.submit(fetch_url, url, decode): url for url in chunk}
+            future_to_url = {executor.submit(worker, url): url for url in chunk}
             for future in as_completed(future_to_url):
                 # url and download result
                 yield future_to_url[future], future.result()
 
 
 def _send_pycurl_request(url, no_ssl, with_headers, config):
     '''Experimental function using libcurl and pycurl to speed up downloads'''
```

### Comparing `trafilatura-1.8.1/trafilatura/feeds.py` & `trafilatura-1.9.0/trafilatura/feeds.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     fix_relative_urls,
     get_hostinfo,
     is_valid_url,
 )
 
 from .downloads import fetch_url
 from .settings import MAX_LINKS
-from .utils import is_similar_domain, load_html, uniquify_list
+from .utils import is_similar_domain, load_html
 
 LOGGER = logging.getLogger(__name__)
 
 # https://www.iana.org/assignments/media-types/media-types.xhtml
 # standard + potential types
 FEED_TYPES = {
     "application/atom",  # not IANA-compatible
@@ -194,15 +194,15 @@
     if not feed_urls:
         for linkelem in tree.xpath("//a[@href]"):
             link = linkelem.get("href", "")
             if LINK_VALIDATION_RE.search(link):
                 feed_urls.append(link)
     # refine
     output_urls = []
-    for link in uniquify_list(feed_urls):
+    for link in dict.fromkeys(feed_urls):
         link = fix_relative_urls(params.base, link)
         link = clean_url(link)
         if link is None or link == params.ref or not is_valid_url(link):
             continue
         if BLACKLIST.search(link):
             continue
         output_urls.append(link)
```

### Comparing `trafilatura-1.8.1/trafilatura/filters.py` & `trafilatura-1.9.0/trafilatura/filters.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,73 +17,69 @@
 from .settings import LRU_SIZE
 from .utils import trim
 
 LOGGER = logging.getLogger(__name__)
 
 LRU_TEST = LRUCache(maxsize=LRU_SIZE)
 
+# https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Language
+TARGET_LANG_ATTRS = ('http-equiv="content-language"', 'property="og:locale"')
 RE_HTML_LANG = re.compile(r'([a-z]{2})')
 
 # Mostly filters for social media
 RE_FILTER = re.compile(r'\W*(Drucken|E-?Mail|Facebook|Flipboard|Google|Instagram|'
                         'Linkedin|Mail|PDF|Pinterest|Pocket|Print|QQ|Reddit|Twitter|'
                         'WeChat|WeiBo|Whatsapp|Xing|Mehr zum Thema:?|More on this.{,8}$)$',
                        flags=re.IGNORECASE)
 # COMMENTS_BLACKLIST = ('( Abmelden / Ändern )') # Fill in your details below|Trage deine Daten unten|Kommentar verfassen|Bitte logge dich|Hinterlasse einen Kommentar| to %s| mit %s)
 
 
 def put_in_cache(teststring):
     '''Implement LRU cache'''
     cacheval = LRU_TEST.get(teststring)
     # if the value is already defined
-    if cacheval != -1:
-        # print(cacheval, teststring[:10] + '...')
-        LRU_TEST.put(teststring, cacheval + 1)
-    else:
-        # print(0, teststring[:10] + '...')
-        LRU_TEST.put(teststring, 1)
+    value = cacheval + 1 if cacheval != -1 else 1
+    LRU_TEST.put(teststring, value)
 
 
-def duplicate_test(element, config):
+def duplicate_test(element, options):
     '''Check for duplicate text with LRU cache'''
     teststring = trim(' '.join(element.itertext()))
     # teststring = element.text
-    if len(teststring) > config.getint('DEFAULT', 'MIN_DUPLCHECK_SIZE'):
+    if len(teststring) > options.min_duplcheck_size:
         # retrieve value from cache
         cacheval = LRU_TEST.get(teststring)
-        if cacheval > config.getint('DEFAULT', 'MAX_REPETITIONS'):  # non-existent key will return -1
+        if cacheval > options.max_repetitions:  # non-existent key will return -1
             LRU_TEST.put(teststring, cacheval + 1)
             return True
     put_in_cache(teststring)
     return False
 
 
 def check_html_lang(tree, target_language, strict=False):
-    '''Check HTML meta-elements for language information and split
-       the result in case there are several languages'''
-    # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Language
-    target_attrs = ['http-equiv="content-language"', 'property="og:locale"']
-    for attr in target_attrs:
-        target_elements = tree.findall(f'.//meta[@{attr}][@content]')
-        if target_elements:
-            for elem in target_elements:
-                if target_language in RE_HTML_LANG.split(elem.get('content', '').lower()):
-                    return True
-            LOGGER.debug('%s failed', attr)
+    """Check HTML meta-elements for language information and split
+       the result in case there are several languages."""
+    for attr in TARGET_LANG_ATTRS:
+        elems = tree.findall(f'.//meta[@{attr}][@content]')
+        if elems:
+            if any(target_language in RE_HTML_LANG.split(elem.get("content", "").lower()) for elem in elems):
+                return True
+            LOGGER.debug("%s lang attr failed", attr)
             return False
+
     # HTML lang attribute: sometimes a wrong indication
-    if strict is True:
-        target_elements = tree.xpath('//html[@lang]')
-        if target_elements:
-            for elem in target_elements:
-                if target_language in RE_HTML_LANG.split(elem.get('lang').lower()):
-                    return True
-            LOGGER.debug('HTML lang failed')
+    if strict:
+        elems = tree.xpath("//html[@lang]")
+        if elems:
+            if any(target_language in RE_HTML_LANG.split(elem.get("lang", "").lower()) for elem in elems):
+                return True
+            LOGGER.debug("HTML lang failed")
             return False
-    LOGGER.debug('No relevant lang elements found')
+
+    LOGGER.debug("No relevant lang elements found")
     return True
 
 
 def language_classifier(temp_text, temp_comments):
     '''Run external component (if installed) for language identification'''
     if LANGID_FLAG is True:
         result, _ = (
```

### Comparing `trafilatura-1.8.1/trafilatura/hashing.py` & `trafilatura-1.9.0/trafilatura/hashing.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/htmlprocessing.py` & `trafilatura-1.9.0/trafilatura/htmlprocessing.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 """
 
 import logging
 from collections import defaultdict
 from copy import deepcopy
 
 from courlan.urlutils import fix_relative_urls, get_base_url
-from lxml.etree import XPath, strip_tags
+from lxml.etree import strip_tags
 
 from .filters import duplicate_test, textfilter
 from .settings import CUT_EMPTY_ELEMS, MANUALLY_CLEANED, MANUALLY_STRIPPED
-from .utils import trim, uniquify_list
+from .utils import trim
+
 
 LOGGER = logging.getLogger(__name__)
 
 REND_TAG_MAPPING = {
     'em': '#i',
     'i': '#i',
     'b': '#b',
@@ -38,35 +39,44 @@
     except AttributeError:  # pragma: no cover
         element.getparent().remove(element)
 
 
 def tree_cleaning(tree, options):
     "Prune the tree by discarding unwanted elements."
     # determine cleaning strategy, use lists to keep it deterministic
+    favor_recall = options.focus == "recall"
     cleaning_list, stripping_list = \
         MANUALLY_CLEANED.copy(), MANUALLY_STRIPPED.copy()
-    if options.tables is False:
+    if not options.tables:
         cleaning_list.extend(['table', 'td', 'th', 'tr'])
     else:
         # prevent this issue: https://github.com/adbar/trafilatura/issues/301
         for elem in tree.xpath('.//figure[descendant::table]'):
             elem.tag = 'div'
-    if options.images is True:
+    if options.images:
         # Many websites have <img> inside <figure> or <picture> or <source> tag
         cleaning_list = [e for e in cleaning_list if e
                          not in ('figure', 'picture', 'source')]
         stripping_list.remove('img')
 
     # strip targeted elements
     strip_tags(tree, stripping_list)
 
+    # prevent removal of paragraphs
+    run_p_test = False
+    if options.focus == "recall" and tree.find('.//p') is not None:
+        tcopy = deepcopy(tree)
+        run_p_test = True
+
     # delete targeted elements
     for expression in cleaning_list:
         for element in tree.getiterator(expression):
             delete_element(element)
+    if run_p_test and tree.find('.//p') is None:
+        tree = tcopy
 
     return prune_html(tree)
 
 
 def prune_html(tree):
     "Delete selected empty elements to save space and processing time."
     # //comment() needed for date extraction
@@ -74,48 +84,47 @@
         if element.tag in CUT_EMPTY_ELEMS:
             delete_element(element)
     return tree
 
 
 def prune_unwanted_nodes(tree, nodelist, with_backup=False):
     '''Prune the HTML tree by removing unwanted sections.'''
-    if with_backup is True:
+    if with_backup:
         old_len = len(tree.text_content())  # ' '.join(tree.itertext())
         backup = deepcopy(tree)
+
     for expression in nodelist:
         for subtree in expression(tree):
             # preserve tail text from deletion
             if subtree.tail is not None:
-                previous = subtree.getprevious()
-                if previous is None:
-                    previous = subtree.getparent()
-                if previous is not None:
+                prev = subtree.getprevious()
+                if prev is None:
+                    prev = subtree.getparent()
+                if prev is not None:
                     # There is a previous node, append text to its tail
-                    if previous.tail is not None:
-                        previous.tail = ' '.join([previous.tail, subtree.tail])
-                    else:
-                        previous.tail = subtree.tail
+                    prev.tail = " ".join([prev.tail, subtree.tail]) if prev.tail else subtree.tail
             # remove the node
             subtree.getparent().remove(subtree)
-    if with_backup is False:
+
+    if not with_backup:
         return tree
-    # else:
+
     new_len = len(tree.text_content())
     # todo: adjust for recall and precision settings
     if new_len > old_len/7:
         return tree
     return backup
 
 
 def collect_link_info(links_xpath, favor_precision=False):
     '''Collect heuristics on link text'''
     # init
     shortelems, mylist = 0, []
     # longer strings impact recall in favor of precision
-    threshold = 10 if not favor_precision else 50
+    threshold = 50 if favor_precision else 10
     # examine the elements
     for subelem in links_xpath:
         subelemtext = trim(subelem.text_content())
         if subelemtext:
             mylist.append(subelemtext)
             if len(subelemtext) < threshold:
                 shortelems += 1
@@ -124,15 +133,15 @@
 
 
 def link_density_test(element, text, favor_precision=False):
     '''Remove sections which are rich in links (probably boilerplate)'''
     links_xpath, mylist = element.findall('.//ref'), []
     if links_xpath:
         if element.tag == 'p': #  and not element.getparent().tag == 'item'
-            if favor_precision is False:
+            if not favor_precision:
                 if element.getnext() is None:
                     limitlen, threshold = 60, 0.8
                 else:
                     limitlen, threshold = 30, 0.8
             else:
                 limitlen, threshold = 200, 0.8
             #if 'hi' in list(element):
@@ -181,179 +190,199 @@
 def delete_by_link_density(subtree, tagname, backtracking=False, favor_precision=False):
     '''Determine the link density of elements with respect to their length,
        and remove the elements identified as boilerplate.'''
     myelems, deletions = defaultdict(list), []
     for elem in subtree.iter(tagname):
         elemtext = trim(elem.text_content())
         result, templist = link_density_test(elem, elemtext, favor_precision)
-        if result is True:
+        if result:
             deletions.append(elem)
-        elif backtracking is True and len(templist) > 0:  # if?
+        elif backtracking and len(templist) > 0:  # if?
             myelems[elemtext].append(elem)
     # summing up
-    if backtracking is True:
-        if favor_precision is False:
-            threshold = 100
-        else:
-            threshold = 200
+    if backtracking:
+        threshold = 200 if favor_precision else 100
         for text, elem in myelems.items():
             if 0 < len(text) < threshold and len(elem) >= 3:
                 deletions.extend(elem)
                 # print('backtrack:', text)
             # else: # and not re.search(r'[?!.]', text):
             # print(elem.tag, templist)
-    for elem in uniquify_list(deletions):
-        try:
-            elem.getparent().remove(elem)
-        except AttributeError:
-            pass
+    for elem in dict.fromkeys(deletions):
+        parent = elem.getparent()
+        if parent is not None:
+            parent.remove(elem)
     return subtree
 
 
+def convert_lists(elem):
+    # ul/ol → list / li → item
+    elem.set("rend", elem.tag)
+    elem.tag = "list"
+    i = 1
+    for subelem in elem.iter("dd", "dt", "li"):
+        # keep track of dd/dt items
+        if subelem.tag in ("dd", "dt"):
+            subelem.set("rend", f"{subelem.tag}-{i}")
+            # increment counter after <dd> in description list
+            if subelem.tag == "dd":
+                i += 1
+        # convert elem tag
+        subelem.tag = "item"
+
+
+def convert_quotes(elem):
+    code_flag = False
+    if elem.tag == "pre":
+        # detect if there could be code inside
+        children = elem.getchildren()
+        # pre with a single span is more likely to be code
+        if len(children) == 1 and children[0].tag == "span":
+            code_flag = True
+        # find hljs elements to detect if it's code
+        code_elems = elem.xpath(".//span[starts-with(@class,'hljs')]")
+        if code_elems:
+            code_flag = True
+            for subelem in code_elems:
+                subelem.attrib.clear()
+    elem.tag = "code" if code_flag else "quote"
+
+
+def convert_headings(elem):
+    "Add head tags and delete attributes."
+    elem.attrib.clear()
+    elem.set("rend", elem.tag)
+    elem.tag = "head"
+
+
+def convert_line_breaks(elem):
+    "br → lb"
+    elem.tag = "lb"
+
+
+def convert_deletions(elem):
+    'del | s | strike → <del rend="overstrike">'
+    elem.tag = "del"
+    elem.set("rend", "overstrike")
+
+
+def convert_details(elem):
+    "Handle details and summary."
+    elem.tag = "div"
+    for subelem in elem.iter("summary"):
+        subelem.tag = "head"
+
+
+CONVERSIONS = {
+    "dl": convert_lists, "ol": convert_lists, "ul": convert_lists,
+    "h1": convert_headings, "h2": convert_headings, "h3": convert_headings,
+    "h4": convert_headings, "h5": convert_headings, "h6": convert_headings,
+    "br": convert_line_breaks, "hr": convert_line_breaks,
+    "blockquote": convert_quotes, "pre": convert_quotes, "q": convert_quotes,
+    "del": convert_deletions, "s": convert_deletions, "strike": convert_deletions,
+    "details": convert_details,
+}
+
+
 def convert_tags(tree, options, url=None):
     '''Simplify markup and convert relevant HTML tags to an XML standard'''
     # delete links for faster processing
-    if options.links is False:
+    if not options.links:
         xpath_expr = './/div//a|.//ul//a'  # .//p//a ?
-        if options.tables is True:
+        if options.tables:
             xpath_expr += '|.//table//a'
         # necessary for further detection
         for elem in tree.xpath(xpath_expr):
             elem.tag = 'ref'
         # strip the rest
         strip_tags(tree, 'a')
     else:
         # get base URL for converting relative URLs
         base_url = url and get_base_url(url)
         for elem in tree.iter('a', 'ref'):
             elem.tag = 'ref'
             # replace href attribute and delete the rest
             target = elem.get('href') # defaults to None
             elem.attrib.clear()
-            if target is not None:
+            if target:
                 # convert relative URLs
-                if base_url is not None:
+                if base_url:
                     target = fix_relative_urls(base_url, target)
                 elem.set('target', target)
-    # include_formatting
-    if options.formatting is False:
-        strip_tags(tree, *REND_TAG_MAPPING)
-    else:
-        for elem in tree.iter(list(REND_TAG_MAPPING)):
+
+    if options.formatting:
+        for elem in tree.iter(REND_TAG_MAPPING.keys()):
             attribute = REND_TAG_MAPPING[elem.tag]
             elem.tag = 'hi'
             elem.set('rend', attribute)
+    else:
+        strip_tags(tree, *REND_TAG_MAPPING)
+
     # iterate over all concerned elements
-    for elem in tree.iter('blockquote', 'br', 'del', 'details', 'dl', 'h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'hr', 'ol', 'pre', 'q', 's', 'strike', 'ul'):
-        # ul/ol → list / li → item
-        if elem.tag in ('dl', 'ol', 'ul'):
-            elem.set('rend', elem.tag)
-            elem.tag = 'list'
-            i = 1
-            for subelem in elem.iter('dd', 'dt', 'li'):
-                # keep track of dd/dt items
-                if subelem.tag in ('dd', 'dt'):
-                    subelem.set('rend', f"{subelem.tag}-{i}")
-                    # increment counter after <dd> in description list
-                    if subelem.tag == 'dd':
-                        i += 1
-                # convert elem tag
-                subelem.tag = 'item'
-        # head tags + delete attributes
-        elif elem.tag in ('h1', 'h2', 'h3', 'h4', 'h5', 'h6'):
-            elem.attrib.clear()
-            elem.set('rend', elem.tag)
-            elem.tag = 'head'
-        # br → lb
-        elif elem.tag in ('br', 'hr'):
-            elem.tag = 'lb'
+    for elem in tree.iter(CONVERSIONS.keys()):
+        CONVERSIONS[elem.tag](elem)
         # wbr
         # pre
         #elif elem.tag == 'pre':
         #    else:
         #        elem.tag = 'quote'
-        # blockquote, q → quote
-        elif elem.tag in ('blockquote', 'pre', 'q'):
-            code_flag = False
-            if elem.tag == 'pre':
-                # detect if there could be code inside
-                children = elem.getchildren()
-                # pre with a single span is more likely to be code
-                if len(children) == 1 and children[0].tag == 'span':
-                    code_flag = True
-            # find hljs elements to detect if it's code
-            code_elems = elem.xpath(".//span[starts-with(@class,'hljs')]")
-            if code_elems:
-                code_flag = True
-                for subelem in code_elems:
-                    subelem.attrib.clear()
-            if code_flag:
-                elem.tag = 'code'
-            else:
-                elem.tag = 'quote'
-        # del | s | strike → <del rend="overstrike">
-        elif elem.tag in ('del', 's', 'strike'):
-            elem.tag = 'del'
-            elem.set('rend', 'overstrike')
-        # details + summary
-        elif elem.tag == 'details':
-            elem.tag = 'div'
-            for subelem in elem.iter('summary'):
-                subelem.tag = 'head'
     # images
-    if options.images is True:
+    if options.images:
         for elem in tree.iter('img'):
             elem.tag = 'graphic'
     return tree
 
 
-def handle_textnode(element, options, comments_fix=True, preserve_spaces=False):
-    '''Convert, format, and probe potential text elements'''
-    if element.text is None and element.tail is None and len(element) == 0:
+def handle_textnode(elem, options, comments_fix=True, preserve_spaces=False):
+    "Convert, format, and probe potential text elements."
+    if elem.tag == "done" or (len(elem) == 0 and not elem.text and not elem.tail):
         return None
+
     # lb bypass
-    if comments_fix is False and element.tag == 'lb':
-        if preserve_spaces is False:
-            element.tail = trim(element.tail)
-        # if textfilter(element) is True:
+    if not comments_fix and elem.tag == "lb":
+        if not preserve_spaces:
+            elem.tail = trim(elem.tail)
+        # if textfilter(elem) is True:
         #     return None
         # duplicate_test(subelement)?
-        return element
-    if element.text is None and len(element) == 0:
+        return elem
+
+    if not elem.text and len(elem) == 0:
         # try the tail
-        # LOGGER.debug('using tail for element %s', element.tag)
-        element.text, element.tail = element.tail, ''
+        # LOGGER.debug('using tail for element %s', elem.tag)
+        elem.text, elem.tail = elem.tail, ""
         # handle differently for br/lb
-        if comments_fix and element.tag == 'lb':
-            element.tag = 'p'
+        if comments_fix and elem.tag == "lb":
+            elem.tag = "p"
+
     # trim
-    if preserve_spaces is False:
-        element.text = trim(element.text)
-        if element.tail:
-            element.tail = trim(element.tail)
+    if not preserve_spaces:
+        elem.text = trim(elem.text)
+        if elem.tail:
+            elem.tail = trim(elem.tail)
+
     # filter content
     # or not re.search(r'\w', element.text):  # text_content()?
-    if not element.text and textfilter(element) is True:
+    if not elem.text and textfilter(elem) or \
+        (options.dedup and duplicate_test(elem, options)):
         return None
-    if options.dedup and duplicate_test(element, options.config) is True:
-        return None
-    return element
+    return elem
 
 
-def process_node(element, options):
-    '''Convert, format, and probe potential text elements (light format)'''
-    if element.tag == 'done':
-        return None
-    if len(element) == 0 and not element.text and not element.tail:
+def process_node(elem, options):
+    "Convert, format, and probe potential text elements (light format)."
+    if elem.tag == "done" or (len(elem) == 0 and not elem.text and not elem.tail):
         return None
+
     # trim
-    element.text, element.tail = trim(element.text), trim(element.tail)
+    elem.text, elem.tail = trim(elem.text), trim(elem.tail)
+
     # adapt content string
-    if element.tag != 'lb' and not element.text and element.tail:
-        element.text, element.tail = element.tail, None
+    if elem.tag != "lb" and not elem.text and elem.tail:
+        elem.text, elem.tail = elem.tail, None
+
     # content checks
-    if element.text or element.tail:
-        if textfilter(element) is True:
-            return None
-        if options.dedup and duplicate_test(element, options.config) is True:
+    if elem.text or elem.tail:
+        if textfilter(elem) or (options.dedup and duplicate_test(elem, options)):
             return None
-    return element
+
+    return elem
```

### Comparing `trafilatura-1.8.1/trafilatura/json_metadata.py` & `trafilatura-1.9.0/trafilatura/json_metadata.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/lru.py` & `trafilatura-1.9.0/trafilatura/lru.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,69 +23,66 @@
         # initialize by pointing to self
         self.root[:] = [self.root, self.root, None, None]
         self.full = False
 
     def _move_link(self, link):
         # Move the link to the front of the circular queue
         link_prev, link_next, _key, result = link
-        link_prev[NEXT] = link_next
-        link_next[PREV] = link_prev
+        link_prev[NEXT], link_next[PREV] = link_next, link_prev
         last = self.root[PREV]
         last[NEXT] = self.root[PREV] = link
         link[PREV] = last
         link[NEXT] = self.root
         return result
 
     def get(self, key):
         '''Tests if the key that is asked for is in the cache
            and retrieve its value from the linked list'''
         with self.lock:
             link = self.cache.get(key)
-            if link is not None:
+            if link:
                 return self._move_link(link)
         return -1
 
     def put(self, key, value):
         '''Stores a given key in the cache'''
         # Size limited caching that tracks accesses by recency
         with self.lock:
             link = self.cache.get(key)
-            if link is not None:
+            if link:
                 self._move_link(link)
                 self.cache[key][RESULT] = value
-                return
-        with self.lock:
-            if self.full:
-                # Use the old root to store the new key and result.
-                oldroot = self.root
-                oldroot[KEY] = key
-                oldroot[RESULT] = value
-                # Empty the oldest link and make it the new root.
-                # Keep a reference to the old key and old result to
-                # prevent their ref counts from going to zero during the
-                # update. That will prevent potentially arbitrary object
-                # clean-up code (i.e. __del__) from running while we're
-                # still adjusting the links.
-                self.root = oldroot[NEXT]
-                oldkey = self.root[KEY]
-                self.root[KEY] = self.root[RESULT] = None
-                # Now update the cache dictionary.
-                del self.cache[oldkey]
-                # Save the potentially reentrant cache[key] assignment
-                # for last, after the root and links have been put in
-                # a consistent state.
-                self.cache[key] = oldroot
             else:
-                # Put result in a new link at the front of the queue.
-                last = self.root[PREV]
-                link = [last, self.root, key, value]
-                last[NEXT] = self.root[PREV] = self.cache[key] = link
-                # Use the cache_len bound method instead of the len() function
-                # which could potentially be wrapped in an lru_cache itself.
-                self.full = len(self.cache) >= self.maxsize
+                if self.full:
+                    # Use the old root to store the new key and result.
+                    oldroot = self.root
+                    oldroot[KEY], oldroot[RESULT] = key, value
+                    # Empty the oldest link and make it the new root.
+                    # Keep a reference to the old key and old result to
+                    # prevent their ref counts from going to zero during the
+                    # update. That will prevent potentially arbitrary object
+                    # clean-up code (i.e. __del__) from running while we're
+                    # still adjusting the links.
+                    self.root = oldroot[NEXT]
+                    oldkey = self.root[KEY]
+                    self.root[KEY] = self.root[RESULT] = None
+                    # Now update the cache dictionary.
+                    del self.cache[oldkey]
+                    # Save the potentially reentrant cache[key] assignment
+                    # for last, after the root and links have been put in
+                    # a consistent state.
+                    self.cache[key] = oldroot
+                else:
+                    # Put result in a new link at the front of the queue.
+                    last = self.root[PREV]
+                    link = [last, self.root, key, value]
+                    last[NEXT] = self.root[PREV] = self.cache[key] = link
+                    # Use the cache_len bound method instead of the len() function
+                    # which could potentially be wrapped in an lru_cache itself.
+                    self.full = len(self.cache) >= self.maxsize
 
     def clear(self):
         '''Delete all cache content'''
         with self.lock:
             self.cache.clear()
             self.root[:] = [self.root, self.root, None, None]
             self.full = False
```

### Comparing `trafilatura-1.8.1/trafilatura/meta.py` & `trafilatura-1.9.0/trafilatura/meta.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/metadata.py` & `trafilatura-1.9.0/trafilatura/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 """
 Module bundling all functions needed to scrape metadata from webpages.
 """
 
 import json
 import logging
 import re
+
 from copy import deepcopy
 
 from courlan import extract_domain, get_base_url, is_valid_url, normalize_url, validate_url
 from htmldate import find_date
 from lxml.html import tostring
 
 from .htmlprocessing import prune_unwanted_nodes
 from .json_metadata import (extract_json, extract_json_parse_error,
                             normalize_json)
-from .metaxpaths import (author_discard_xpaths, author_xpaths,
-                         categories_xpaths, tags_xpaths, title_xpaths)
+from .settings import set_date_params
 from .utils import (line_processing, load_html, normalize_authors,
-                    normalize_tags, trim, unescape, uniquify_list)
+                    normalize_tags, trim, unescape)
+from .xpaths import (AUTHOR_DISCARD_XPATHS, AUTHOR_XPATHS,
+                     CATEGORIES_XPATHS, TAGS_XPATHS, TITLE_XPATHS)
 
 LOGGER = logging.getLogger(__name__)
 logging.getLogger('htmldate').setLevel(logging.WARNING)
 
 
 class Document:
     "Defines a class to store all necessary data and metadata fields for extracted information."
     __slots__ = [
     'title', 'author', 'url', 'hostname', 'description', 'sitename',
     'date', 'categories', 'tags', 'fingerprint', 'id', 'license',
     'body', 'comments', 'commentsbody', 'raw_text', 'text',
-    'language', 'image', 'pagetype'  # 'locale'?
+    'language', 'image', 'pagetype', 'filedate'  # 'locale'?
     ]
     # consider dataclasses for Python 3.7+
     def __init__(self):
         for slot in self.__slots__:
             setattr(self, slot, None)
 
     def set_attributes(self, title, author, url, description, site_name, image, pagetype, tags):
@@ -68,23 +70,19 @@
                 # HTML entities, remove spaces and control characters
                 value = line_processing(unescape(value))
                 setattr(self, slot, value)
 
     def as_dict(self):
         "Convert the document to a dictionary."
         return {
-            attr: getattr(self, attr)
+            attr: getattr(self, attr, None)
             for attr in self.__slots__
-            if hasattr(self, attr)
         }
 
 
-HTMLDATE_CONFIG_FAST = {'extensive_search': False, 'original_date': True}
-HTMLDATE_CONFIG_EXTENSIVE = {'extensive_search': True, 'original_date': True}
-
 JSON_MINIFY = re.compile(r'("(?:\\"|[^"])*")|\s')
 
 HTMLTITLE_REGEX = re.compile(r'^(.+)?\s+[–•·—|⁄*⋆~‹«<›»>:-]\s+(.+)$')  # part without dots?
 HTML_STRIP_TAG = re.compile(r'(<!--.*?-->|<[^>]*>)')
 
 LICENSE_REGEX = re.compile(r'/(by-nc-nd|by-nc-sa|by-nc|by-nd|by-sa|by|zero)/([1-9]\.[0-9])')
 TEXT_LICENSE_REGEX = re.compile(r'(cc|creative commons) (by-nc-nd|by-nc-sa|by-nc|by-nd|by-sa|by|zero) ?([1-9]\.[0-9])?', re.I)
@@ -159,15 +157,15 @@
 
 def extract_opengraph(tree):
     '''Search meta tags following the OpenGraph guidelines (https://ogp.me/)'''
     title, author, url, description, site_name, image, pagetype = (None,) * 7
     # detect OpenGraph schema
     for elem in tree.xpath('.//head/meta[starts-with(@property, "og:")]'):
         # safeguard
-        if not elem.get('content'):
+        if not elem.get('content') or elem.get('content').isspace():
             continue
         # site name
         if elem.get('property') == 'og:site_name':
             site_name = elem.get('content')
         # blog title
         elif elem.get('property') == 'og:title':
             title = elem.get('content')
@@ -208,15 +206,15 @@
     if all((title, author, url, description, site_name, image)):
         metadata.set_attributes(title, author, url, description, site_name, image, pagetype, None)  # tags
         return metadata
     tags, backup_sitename = [], None
     # skim through meta tags
     for elem in tree.iterfind('.//head/meta[@content]'):
         # content
-        if not elem.get('content'):
+        if not elem.get('content') or elem.get('content').isspace():
             continue
         content_attr = HTML_STRIP_TAG.sub('', elem.get('content'))
         # image info
         # ...
         # property
         if 'property' in elem.attrib:
             # no opengraph a second time
@@ -316,15 +314,15 @@
     # only one h1-element: take it
     h1_results = tree.findall('.//h1')
     if len(h1_results) == 1:
         title = trim(h1_results[0].text_content())
         if len(title) > 0:
             return title
     # extract using x-paths
-    title = extract_metainfo(tree, title_xpaths)
+    title = extract_metainfo(tree, TITLE_XPATHS)
     if title is not None:
         return title
     # extract using title tag
     title, first, second = examine_title_element(tree)
     if first is not None and '.' not in first:
         return first
     if second is not None and '.' not in second:
@@ -338,16 +336,16 @@
     except IndexError:
         LOGGER.debug('no h2 title found')
     return title
 
 
 def extract_author(tree):
     '''Extract the document author(s)'''
-    subtree = prune_unwanted_nodes(deepcopy(tree), author_discard_xpaths)
-    author = extract_metainfo(subtree, author_xpaths, len_limit=120)
+    subtree = prune_unwanted_nodes(deepcopy(tree), AUTHOR_DISCARD_XPATHS)
+    author = extract_metainfo(subtree, AUTHOR_XPATHS, len_limit=120)
     if author:
         author = normalize_authors(None, author)
     # copyright?
     return author
 
 
 def extract_url(tree, default_url=None):
@@ -396,15 +394,15 @@
     return None
 
 
 def extract_catstags(metatype, tree):
     '''Find category and tag information'''
     results = []
     regexpr = '/' + metatype + '[s|ies]?/'
-    xpath_expression = categories_xpaths if metatype == 'category' else tags_xpaths
+    xpath_expression = CATEGORIES_XPATHS if metatype == 'category' else TAGS_XPATHS
     # search using custom expressions
     for catexpr in xpath_expression:
         results.extend(
             elem.text_content()
             for elem in catexpr(tree)
             if re.search(regexpr, elem.attrib['href'])
         )
@@ -414,16 +412,15 @@
     if metatype == 'category' and not results:
         for element in tree.xpath('.//head//meta[@property="article:section" or contains(@name, "subject")][@content]'):
             results.append(element.attrib['content'])
         # optional: search through links
         #if not results:
         #    for elem in tree.xpath('.//a[@href]'):
         #        search for 'category'
-    results = [line_processing(x) for x in results if x is not None]
-    return uniquify_list([x for x in results if x is not None])
+    return [r for r in dict.fromkeys(line_processing(x) for x in results if x) if r]
 
 
 def parse_license_element(element, strict=False):
     '''Probe a link for identifiable free license cues.
        Parse the href attribute first and then the link text.'''
    # look for Creative Commons elements
     match = LICENSE_REGEX.search(element.get('href'))
@@ -468,15 +465,15 @@
 
     for elem in tree.xpath('.//head/meta[@property="twitter:image" or @property="twitter:image:src"][@content]'):
         return elem.get('content')
 
     return None
 
 
-def extract_metadata(filecontent, default_url=None, date_config=None, fastmode=False, author_blacklist=None):
+def extract_metadata(filecontent, default_url=None, date_config=None, extensive=True, author_blacklist=None):
     """Main process for metadata extraction.
 
     Args:
         filecontent: HTML code as string.
         default_url: Previously known URL of the downloaded document.
         date_config: Provide extraction parameters to htmldate as dict().
         author_blacklist: Provide a blacklist of Author Names as set() to filter out authors.
@@ -484,14 +481,16 @@
     Returns:
         A trafilatura.metadata.Document containing the extracted metadata information or None.
         trafilatura.metadata.Document has .as_dict() method that will return a copy as a dict.
     """
     # init
     if author_blacklist is None:
         author_blacklist = set()
+    if not date_config:
+        date_config = set_date_params(extensive)
     # load contents
     tree = load_html(filecontent)
     if tree is None:
         return None
     # initialize dict and try to strip meta tags
     metadata = examine_meta(tree)
     # to check: remove it and replace with author_blacklist in test case
@@ -521,20 +520,14 @@
     # hostname
     if metadata.url is not None:
         metadata.hostname = extract_domain(metadata.url, fast=True)
     # image
     if metadata.image is None:
         metadata.image = extract_image(tree)
     # extract date with external module htmldate
-    if date_config is None:
-        # decide on fast mode
-        if fastmode is False:
-            date_config = HTMLDATE_CONFIG_EXTENSIVE
-        else:
-            date_config = HTMLDATE_CONFIG_FAST
     date_config['url'] = metadata.url
     metadata.date = find_date(tree, **date_config)
     # sitename
     if metadata.sitename is None:
         metadata.sitename = extract_sitename(tree)
     if metadata.sitename is not None:
         # fix: take 1st element (['Westdeutscher Rundfunk'])
@@ -566,10 +559,11 @@
         metadata.categories = extract_catstags('category', tree)
     # tags
     if not metadata.tags:
         metadata.tags = extract_catstags('tag', tree)
     # license
     metadata.license = extract_license(tree)
     # safety checks
+    metadata.filedate = date_config["max_date"]
     metadata.clean_and_trim()
     # return result
     return metadata
```

### Comparing `trafilatura-1.8.1/trafilatura/readability_lxml.py` & `trafilatura-1.9.0/trafilatura/readability_lxml.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,55 +10,50 @@
 Ruby port by starrhorne and iterationlabs
 Python port by gfxmonk
 
 For list of contributors see
 https://github.com/timbertson/python-readability
 https://github.com/buriy/python-readability
 
-License of forked code: Apache-2.0 License
+License of forked code: Apache-2.0.
 """
 
+
 import logging
 import re
 
+from operator import attrgetter
+
 from lxml.etree import tostring
 from lxml.html import fragment_fromstring
 
 from .utils import trim
 
 LOGGER = logging.getLogger(__name__)
 
 
-BAD_ATTRS = "|".join(["width", "height", "style", "[-a-z]*color", "background[-a-z]*", "on*"])
-QUOTES = '\'[^\']+\'|"[^"]+"'
-NON_SPACE = "[^ \"'>]+"
-HTMLSTRIP = re.compile(
-    "<"  # open
-    "([^>]+) "  # prefix
-    " (?:{BAD_ATTRS}) *"
-    + "= *(?:{NON_SPACE}|{QUOTES})"  # undesirable attributes
-    + "([^>]*)"  # value  # postfix
-    ">",  # end
-    re.I,
-)
-
 DOT_SPACE = re.compile(r"\.( |$)")
 
 
-def clean_attributes(html):
-    while HTMLSTRIP.search(html):
-        html = HTMLSTRIP.sub("<\\1\\2>", html)
-    return html
-
-
 def _tostring(string):
-    return tostring(string, encoding=str, method='xml')
+    return tostring(string, encoding=str, method="xml")
 
 
-DIV_TO_P_ELEMS = {'a', 'blockquote', 'dl', 'div', 'img', 'ol', 'p', 'pre', 'table', 'ul'}
+DIV_TO_P_ELEMS = {
+    "a",
+    "blockquote",
+    "dl",
+    "div",
+    "img",
+    "ol",
+    "p",
+    "pre",
+    "table",
+    "ul",
+}
 
 DIV_SCORES = {"div", "article"}
 BLOCK_SCORES = {"pre", "td", "blockquote"}
 BAD_ELEM_SCORES = {"address", "ol", "ul", "dl", "dd", "dt", "li", "form", "aside"}
 STRUCTURE_SCORES = {"h1", "h2", "h3", "h4", "h5", "h6", "th", "header", "footer", "nav"}
 
 TEXT_CLEAN_ELEMS = {"p", "img", "li", "a", "embed", "input"}
@@ -70,43 +65,46 @@
     ),
     "okMaybeItsACandidateRe": re.compile(r"and|article|body|column|main|shadow", re.I),
     "positiveRe": re.compile(
         r"article|body|content|entry|hentry|main|page|pagination|post|text|blog|story",
         re.I,
     ),
     "negativeRe": re.compile(
-        r"combx|comment|com-|contact|foot|footer|footnote|masthead|media|meta|outbrain|promo|related|scroll|shoutbox|sidebar|sponsor|shopping|tags|tool|widget",
+        r"button|combx|comment|com-|contact|figure|foot|footer|footnote|form|input|masthead|media|meta|outbrain|promo|related|scroll|shoutbox|sidebar|sponsor|shopping|tags|tool|widget",
         re.I,
     ),
     "divToPElementsRe": re.compile(
-        r"<(a|blockquote|dl|div|img|ol|p|pre|table|ul)", re.I
+        r"<(?:a|blockquote|dl|div|img|ol|p|pre|table|ul)", re.I
     ),
-    "videoRe": re.compile(r"https?:\/\/(www\.)?(youtube|vimeo)\.com", re.I),
+    "videoRe": re.compile(r"https?:\/\/(?:www\.)?(?:youtube|vimeo)\.com", re.I),
 }
 
-FRAME_TAGS = {'body', 'html'}
+FRAME_TAGS = {"body", "html"}
 LIST_TAGS = {"ol", "ul"}
 # DIV_TO_P_ELEMS = {'a', 'blockquote', 'dl', 'div', 'img', 'ol', 'p', 'pre', 'table', 'ul'}
 
+
 def text_length(elem):
+    "Return the length of the element with all its contents."
     return len(trim(elem.text_content()))
 
 
 class Candidate:
     "Defines a class to score candidate elements."
-    __slots__ = ['score', 'elem']
+    __slots__ = ["score", "elem"]
 
     def __init__(self, score, elem):
         self.score = score
         self.elem = elem
 
 
 class Document:
     """Class to build a etree document out of html."""
-    __slots__ = ['doc', 'min_text_length', 'retry_length']
+
+    __slots__ = ["doc", "min_text_length", "retry_length"]
 
     def __init__(self, doc, min_text_length=25, retry_length=250):
         """Generate the document
 
         :param doc: string of the html content.
         :param min_text_length: Set to a higher value for more precise detection of longer texts.
         :param retry_length: Set to a lower value for better detection of very small texts.
@@ -117,58 +115,54 @@
         API method:
         .summary() -- cleaned up content
         """
         self.doc = doc
         self.min_text_length = min_text_length
         self.retry_length = retry_length
 
-    def get_clean_html(self):
-        """
-        An internal method, which can be overridden in subclasses, for example,
-        to disable or to improve DOM-to-text conversion in .summary() method
-        """
-        return clean_attributes(_tostring(self.doc))
-
     def summary(self):
         """
         Given a HTML file, extracts the text of the article.
 
         Warning: It mutates internal DOM representation of the HTML document,
         so it is better to call other API methods before this one.
         """
+        for elem in self.doc.iter("script", "style"):
+            elem.drop_tree()
+
         ruthless = True
         while True:
-            for i in self.tags(self.doc, "script", "style"):
-                i.drop_tree()
-            for i in self.tags(self.doc, "body"):
-                i.set("id", "readabilityBody")
             if ruthless:
                 self.remove_unlikely_candidates()
             self.transform_misused_divs_into_paragraphs()
             candidates = self.score_paragraphs()
 
             best_candidate = self.select_best_candidate(candidates)
 
-            if best_candidate is not None:
+            if best_candidate:
                 article = self.get_article(candidates, best_candidate)
             else:
                 if ruthless is True:
                     ruthless = False
-                    LOGGER.debug("Ended up stripping too much - going for a safer parse")
+                    LOGGER.debug(
+                        "Ended up stripping too much - going for a safer parse"
+                    )
                     # try again
                     continue
                 # go ahead
-                LOGGER.debug("Ruthless and lenient parsing did not work. Returning raw html")
+                LOGGER.debug(
+                    "Ruthless and lenient parsing did not work. Returning raw html"
+                )
                 article = self.doc.find("body")
                 if article is None:
                     article = self.doc
 
             cleaned_article = self.sanitize(article, candidates)
             article_length = len(cleaned_article or "")
-            if ruthless is True and article_length < self.retry_length:
+            if ruthless and article_length < self.retry_length:
                 ruthless = False
                 # Loop through and try again.
                 continue
             return cleaned_article
 
     def get_article(self, candidates, best_candidate):
         # Now that we have the top candidate, look through its siblings for
@@ -180,99 +174,90 @@
         parent = best_candidate.elem.getparent()
         siblings = parent.getchildren() if parent is not None else [best_candidate.elem]
         for sibling in siblings:
             # in lxml there no concept of simple text
             # if isinstance(sibling, NavigableString): continue
             append = False
             # conditions
-            if sibling == best_candidate.elem:
-                append = True
-            elif (
+            if sibling == best_candidate.elem or (
                 sibling in candidates
                 and candidates[sibling].score >= sibling_score_threshold
             ):
                 append = True
             elif sibling.tag == "p":
                 link_density = self.get_link_density(sibling)
                 node_content = sibling.text or ""
                 node_length = len(node_content)
 
-                if node_length > 80 and link_density < 0.25:
-                    append = True
-                elif (
-                    node_length <= 80
-                    and link_density == 0
-                    and DOT_SPACE.search(node_content)
+                if (
+                    node_length > 80
+                    and link_density < 0.25
+                    or (
+                        node_length <= 80
+                        and link_density == 0
+                        and DOT_SPACE.search(node_content)
+                    )
                 ):
                     append = True
             # append to the output div
             if append:
                 output.append(sibling)
-        #if output is not None:
+        # if output is not None:
         #    output.append(best_candidate.elem)
         return output
 
     def select_best_candidate(self, candidates):
         if not candidates:
             return None
         sorted_candidates = sorted(
-            candidates.values(), key=lambda x: x.score, reverse=True
+            candidates.values(), key=attrgetter("score"), reverse=True
         )
-        for candidate in sorted_candidates[:5]:
-            LOGGER.debug("Top 5: %s %s", candidate.elem.tag, candidate.score)
-        # return best candidate
-        return sorted_candidates[0]
+        if LOGGER.isEnabledFor(logging.DEBUG):
+            for candidate in sorted_candidates[:5]:
+                LOGGER.debug("Top 5: %s %s", candidate.elem.tag, candidate.score)
+        return next(iter(sorted_candidates))
 
     def get_link_density(self, elem):
         total_length = text_length(elem) or 1
-        link_length = sum(text_length(elem) for elem in elem.findall(".//a"))
+        link_length = sum(text_length(link) for link in elem.findall(".//a"))
         return link_length / total_length
 
     def score_paragraphs(self):
         candidates = {}
-        ordered = []
-        for elem in self.tags(self.doc, "p", "pre", "td"):
+
+        for elem in self.doc.iter("p", "pre", "td"):
             parent_node = elem.getparent()
             if parent_node is None:
                 continue
             grand_parent_node = parent_node.getparent()
 
             elem_text = trim(elem.text_content())
             elem_text_len = len(elem_text)
 
-            # don't count too short paragraphs
+            # discard too short paragraphs
             if elem_text_len < self.min_text_length:
                 continue
 
-            if parent_node not in candidates:
-                candidates[parent_node] = self.score_node(parent_node)
-                ordered.append(parent_node)
-
-            if grand_parent_node is not None and grand_parent_node not in candidates:
-                candidates[grand_parent_node] = self.score_node(grand_parent_node)
-                ordered.append(grand_parent_node)
+            for node in (parent_node, grand_parent_node):
+                if node is not None and node not in candidates:
+                    candidates[node] = self.score_node(node)
 
             score = 1 + len(elem_text.split(",")) + min((elem_text_len / 100), 3)
-            #if elem not in candidates:
+            # if elem not in candidates:
             #    candidates[elem] = self.score_node(elem)
 
             candidates[parent_node].score += score
             if grand_parent_node is not None:
                 candidates[grand_parent_node].score += score / 2
 
         # Scale the final candidates score based on link density. Good content
         # should have a relatively small link density (5% or less) and be
         # mostly unaffected by this operation.
-        for elem in ordered:
-            candidate = candidates[elem]
-            density = self.get_link_density(elem)
-            # LOGGER.debug("Branch %6.3f link density %.3f -> %6.3f",
-            #    candidate.score, density, candidate.score * (1 - density)
-            #)
-            candidate.score *= 1 - density
+        for elem, candidate in candidates.items():
+            candidate.score *= 1 - self.get_link_density(elem)
 
         return candidates
 
     def class_weight(self, elem):
         weight = 0
         for attribute in filter(None, (elem.get("class"), elem.get("id"))):
             if REGEXES["negativeRe"].search(attribute):
@@ -292,106 +277,101 @@
             score -= 3
         elif name in STRUCTURE_SCORES:
             score -= 5
         return Candidate(score, elem)
 
     def remove_unlikely_candidates(self):
         for elem in self.doc.findall(".//*"):
-            attrs = ' '.join(filter(None, (elem.get("class"), elem.get("id"))))
+            attrs = " ".join(filter(None, (elem.get("class"), elem.get("id"))))
             if len(attrs) < 2:
                 continue
             if (
                 elem.tag not in FRAME_TAGS
                 and REGEXES["unlikelyCandidatesRe"].search(attrs)
                 and (not REGEXES["okMaybeItsACandidateRe"].search(attrs))
             ):
                 # LOGGER.debug("Removing unlikely candidate: %s", elem.tag)
                 elem.drop_tree()
 
     def transform_misused_divs_into_paragraphs(self):
-        for elem in self.tags(self.doc, "div"):
+        for elem in self.doc.findall(".//div"):
             # transform <div>s that do not contain other block elements into
             # <p>s
             # FIXME: The current implementation ignores all descendants that
             # are not direct children of elem
             # This results in incorrect results in case there is an <img>
             # buried within an <a> for example
-            #hurts precision:
-            #if not any(e.tag in DIV_TO_P_ELEMS for e in list(elem)):
+            # hurts precision:
+            # if not any(e.tag in DIV_TO_P_ELEMS for e in list(elem)):
             if not REGEXES["divToPElementsRe"].search(
-                ''.join([_tostring(e) for e in list(elem)])
+                "".join(map(_tostring, list(elem)))
             ):
                 elem.tag = "p"
 
-        for elem in self.tags(self.doc, "div"):
-            if elem.text is not None:
-                elem_text = elem.text.strip()
-                if elem_text:
-                    p_elem = fragment_fromstring("<p/>")
-                    p_elem.text = elem.text
-                    elem.text = None
-                    elem.insert(0, p_elem)
+        for elem in self.doc.findall(".//div"):
+            if elem.text and elem.text.strip():
+                p_elem = fragment_fromstring("<p/>")
+                p_elem.text, elem.text = elem.text, None
+                elem.insert(0, p_elem)
 
             for pos, child in sorted(enumerate(elem), reverse=True):
                 if child.tail and child.tail.strip():
                     p_elem = fragment_fromstring("<p/>")
-                    p_elem.text = child.tail
-                    child.tail = None
+                    p_elem.text, child.tail = child.tail, None
                     elem.insert(pos + 1, p_elem)
                 if child.tag == "br":
                     child.drop_tree()
 
-    def tags(self, node, *tag_names):
-        for tag_name in tag_names:
-            yield from node.findall(f".//{tag_name}")
-
-    def reverse_tags(self, node, *tag_names):
-        for tag_name in tag_names:
-            yield from reversed(node.findall(f".//{tag_name}"))
-
     def sanitize(self, node, candidates):
-        for header in self.tags(node, "h1", "h2", "h3", "h4", "h5", "h6"):
+        for header in node.iter("h1", "h2", "h3", "h4", "h5", "h6"):
             if self.class_weight(header) < 0 or self.get_link_density(header) > 0.33:
                 header.drop_tree()
 
-        for elem in self.tags(node, "form", "textarea"):
+        for elem in node.iter("form", "textarea"):
             elem.drop_tree()
 
-        for elem in self.tags(node, "iframe"):
+        for elem in node.iter("iframe"):
             if "src" in elem.attrib and REGEXES["videoRe"].search(elem.attrib["src"]):
                 elem.text = "VIDEO"  # ADD content to iframe text node to force <iframe></iframe> proper output
             else:
                 elem.drop_tree()
 
         allowed = set()
         # Conditionally clean <table>s, <ul>s, and <div>s
-        for elem in self.reverse_tags(
-            node, "table", "ul", "div", "aside", "header", "footer", "section"
-        ):
+        for elem in reversed(node.xpath("//table|//ul|//div|//aside|//header|//footer|//section")):
             if elem in allowed:
                 continue
             weight = self.class_weight(elem)
             score = candidates[elem].score if elem in candidates else 0
             if weight + score < 0:
-                LOGGER.debug("Removed %s with score %6.3f and weight %-3s",
-                    elem.tag, score, weight
+                LOGGER.debug(
+                    "Removed %s with score %6.3f and weight %-3s",
+                    elem.tag,
+                    score,
+                    weight,
                 )
                 elem.drop_tree()
             elif elem.text_content().count(",") < 10:
                 to_remove = False
-                counts = {kind: len(elem.findall(f".//{kind}")) for kind in TEXT_CLEAN_ELEMS}
+                counts = {
+                    kind: len(elem.findall(f".//{kind}")) for kind in TEXT_CLEAN_ELEMS
+                }
                 counts["li"] -= 100
                 counts["input"] -= len(elem.findall('.//input[@type="hidden"]'))
 
                 # Count the text length excluding any surrounding whitespace
                 content_length = text_length(elem)
                 link_density = self.get_link_density(elem)
                 parent_node = elem.getparent()
                 if parent_node is not None:
-                    score = candidates[parent_node].score if parent_node in candidates else 0
+                    score = (
+                        candidates[parent_node].score
+                        if parent_node in candidates
+                        else 0
+                    )
                 # if elem.tag == 'div' and counts["img"] >= 1:
                 #    continue
                 if counts["p"] and counts["img"] > 1 + counts["p"] * 1.3:
                     reason = f'too many images ({counts["img"]})'
                     to_remove = True
                 elif counts["li"] > counts["p"] and elem.tag not in LIST_TAGS:
                     reason = "more <li>s than <p>s"
@@ -399,24 +379,34 @@
                 elif counts["input"] > (counts["p"] / 3):
                     reason = "less than 3x <p>s than <input>s"
                     to_remove = True
                 elif content_length < self.min_text_length and counts["img"] == 0:
                     reason = f"too short content length {content_length} without a single image"
                     to_remove = True
                 elif content_length < self.min_text_length and counts["img"] > 2:
-                    reason = f"too short content length {content_length} and too many images"
+                    reason = (
+                        f"too short content length {content_length} and too many images"
+                    )
                     to_remove = True
                 elif weight < 25 and link_density > 0.2:
-                    reason = f"too many links {link_density:.3f} for its weight {weight}"
+                    reason = (
+                        f"too many links {link_density:.3f} for its weight {weight}"
+                    )
                     to_remove = True
                 elif weight >= 25 and link_density > 0.5:
-                    reason = f"too many links {link_density:.3f} for its weight {weight}"
+                    reason = (
+                        f"too many links {link_density:.3f} for its weight {weight}"
+                    )
                     to_remove = True
-                elif (counts["embed"] == 1 and content_length < 75) or counts["embed"] > 1:
-                    reason = "<embed>s with too short content length, or too many <embed>s"
+                elif (counts["embed"] == 1 and content_length < 75) or counts[
+                    "embed"
+                ] > 1:
+                    reason = (
+                        "<embed>s with too short content length, or too many <embed>s"
+                    )
                     to_remove = True
                 elif not content_length:
                     reason = "no content"
                     to_remove = True
 
                     # find x non empty preceding and succeeding siblings
                     siblings = []
@@ -431,22 +421,22 @@
                         sib_content_length = text_length(sib)
                         if sib_content_length:
                             siblings.append(sib_content_length)
                             if len(siblings) >= limit:
                                 break
                     if siblings and sum(siblings) > 1000:
                         to_remove = False
-                        for desnode in self.tags(elem, "table", "ul", "div", "section"):
-                            allowed.add(desnode)
+                        allowed.update(elem.iter("table", "ul", "div", "section"))
 
                 if to_remove:
-                    LOGGER.debug("Removed %6.3f %s with weight %s cause it has %s.",
-                        score, elem.tag, weight, reason or ""
-                    )
                     elem.drop_tree()
-                else:
-                    LOGGER.debug("Not removing %s of length %s",
-                        elem.tag, content_length
-                    )
+                    if LOGGER.isEnabledFor(logging.DEBUG):
+                        LOGGER.debug(
+                            "Removed %6.3f %s with weight %s cause it has %s.",
+                            score,
+                            elem.tag,
+                            weight,
+                            reason or "",
+                        )
 
         self.doc = node
-        return self.get_clean_html()
+        return _tostring(self.doc)
```

### Comparing `trafilatura-1.8.1/trafilatura/settings.cfg` & `trafilatura-1.9.0/trafilatura/settings.cfg`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/sitemaps.py` & `trafilatura-1.9.0/trafilatura/sitemaps.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/spider.py` & `trafilatura-1.9.0/trafilatura/spider.py`

 * *Files identical despite different names*

### Comparing `trafilatura-1.8.1/trafilatura/utils.py` & `trafilatura-1.9.0/trafilatura/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,15 +116,19 @@
     guesses = []
     # additional module
     if cchardet_detect is not None:
         cchardet_guess = cchardet_detect(bytesobject)['encoding']
         if cchardet_guess is not None:
             guesses.append(cchardet_guess.lower())
     # try charset_normalizer on first part, fallback on full document
-    detection_results = from_bytes(bytesobject[:15000]) or from_bytes(bytesobject)
+    if len(bytesobject) < 10000:
+        detection_results = from_bytes(bytesobject)
+    else:
+        detection_results = from_bytes(bytesobject[:5000] + bytesobject[-5000:]) or \
+                            from_bytes(bytesobject)
     # return alternatives
     if len(detection_results) > 0:
         guesses.extend([r.encoding for r in detection_results])
     # it cannot be utf-8 (tested above)
     return [g for g in guesses if g not in UNICODE_ALIASES]
 
 
@@ -277,15 +281,15 @@
 def sanitize(text, preserve_space=False, trailing_space=False):
     '''Convert text and discard incompatible and invalid characters'''
     # consider all text as a single line
     if trailing_space:
         return line_processing(text, preserve_space, True)
     # process line by line
     try:
-        return '\n'.join(filter(None, (line_processing(l, preserve_space) for l in text.splitlines())))
+        return '\n'.join(filter(None, (line_processing(l, preserve_space) for l in text.splitlines()))).replace('\u2424', '')
     except AttributeError:
         return None
 
 
 def sanitize_tree(tree):
     '''Trims spaces, removes control characters and normalizes unicode'''
     for elem in tree.iter():
@@ -377,24 +381,14 @@
         if author not in new_authors and (len(new_authors) == 0 or all(new_author not in author for new_author in new_authors)):
             new_authors.append(author)
     if len(new_authors) == 0:
         return current_authors
     return '; '.join(new_authors).strip('; ')
 
 
-def uniquify_list(l):
-    """
-    Remove duplicates from a list while keeping order in an efficient way.
-    Dictionaries preserve insertion order since Python 3.6.
-
-    https://www.peterbe.com/plog/fastest-way-to-uniquify-a-list-in-python-3.6
-    """
-    return list(dict.fromkeys(l))
-
-
 @lru_cache(maxsize=1024)
 def is_similar_domain(reference, new_string, threshold=0.5):
     "Return the similarity ratio between two short strings, here domain names."
     if new_string != reference:
         new_string = STRIP_EXTENSION.sub("", new_string)
         reference = STRIP_EXTENSION.sub("", reference)
         if SequenceMatcher(None, reference, new_string).ratio() < threshold:
```

### Comparing `trafilatura-1.8.1/trafilatura/xml.py` & `trafilatura-1.9.0/trafilatura/xml.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 # validation
 TEI_SCHEMA = str(Path(__file__).parent / 'data/tei-schema-pickle.lzma')
 TEI_VALID_TAGS = {'ab', 'body', 'cell', 'code', 'del', 'div', 'graphic', 'head', 'hi', \
                   'item', 'lb', 'list', 'p', 'quote', 'ref', 'row', 'table'}
 TEI_VALID_ATTRS = {'rend', 'rendition', 'role', 'target', 'type'}
 TEI_RELAXNG = None  # to be downloaded later if necessary
 TEI_REMOVE_TAIL = {"ab", "p"}
+TEI_DIV_SIBLINGS = {"p", "list", "table", "quote", "ab"}
 
 CONTROL_PARSER = XMLParser(remove_blank_text=True)
 
 NEWLINE_ELEMS = {
-    'cell': '|',
     'item': '\n- ',
     **{tag: '\n' for tag in ['code', 'graphic', 'head', 'lb', 'list', 'p', 'quote', 'row', 'table']}
 }
 SPECIAL_FORMATTING = {'del', 'head', 'hi', 'ref'}
 WITH_ATTRIBUTES = {'cell', 'del', 'graphic', 'head', 'hi', 'item', 'list', 'ref'}
 
 NESTING_WHITELIST = {"cell", "figure", "item", "note", "quote"}
@@ -119,32 +119,40 @@
         docmeta.commentsbody.tag = 'comments'
         output.append(clean_attributes(docmeta.commentsbody))
 # XML invalid characters
 # https://chase-seibert.github.io/blog/2011/05/20/stripping-control-characters-in-python.html
     return output
 
 
-def control_xml_output(output_tree, output_format, tei_validation, docmeta):
+def control_xml_output(document, options):
     '''Make sure the XML output is conform and valid if required'''
+    strip_double_tags(document.body)
+    remove_empty_elements(document.body)
+
+    func = build_xml_output if options.format == "xml" else build_tei_output
+    output_tree = func(document)
+
     output_tree = sanitize_tree(output_tree)
     # necessary for cleaning
     control_string = tostring(output_tree, encoding='unicode')
     output_tree = fromstring(control_string, CONTROL_PARSER)
+
     # validate
-    if output_format == 'xmltei' and tei_validation is True:
+    if options.format == 'xmltei' and options.tei_validation:
         result = validate_tei(output_tree)
-        LOGGER.debug('TEI validation result: %s %s %s', result, docmeta.id, docmeta.url)
+        LOGGER.debug('TEI validation result: %s %s', result, options.source)
+
     return tostring(output_tree, pretty_print=True, encoding='unicode').strip()
 
 
 def add_xml_meta(output, docmeta):
     '''Add extracted metadata to the XML output tree'''
     for attribute in META_ATTRIBUTES:
         value = getattr(docmeta, attribute, None)
-        if value is not None:
+        if value:
             output.set(attribute, value if isinstance(value, str) else ';'.join(value))
     return output
 
 
 def build_tei_output(docmeta):
     '''Build TEI-XML output tree based on extracted information'''
     # build TEI tree
@@ -165,38 +173,36 @@
         if len(elem) > 0:
             new_elem = _tei_handle_complex_head(elem)
             parent.replace(elem, new_elem)
             elem = new_elem
         if parent.tag == "p":
             _move_element_one_level_up(elem)
     # convert <lb/> when child of <div> to <p>
-    for element in xmldoc.findall(".//text/body//div/lb"):
-        if element.tail and element.tail.strip():
-            element.tag = 'p'
-            element.text = element.tail
-            element.tail = None
+    for elem in xmldoc.findall(".//text/body//div/lb"):
+        if elem.tail and elem.tail.strip():
+            elem.tag, elem.text, elem.tail = 'p', elem.tail, None
     # look for elements that are not valid
-    for element in xmldoc.findall('.//text/body//*'):
-        if element.tag in TEI_REMOVE_TAIL and element.tail and element.tail.strip():
-            _handle_unwanted_tails(element)
+    for elem in xmldoc.findall('.//text/body//*'):
+        if elem.tag in TEI_REMOVE_TAIL and elem.tail and elem.tail.strip():
+            _handle_unwanted_tails(elem)
         # check elements
-        if element.tag not in TEI_VALID_TAGS:
+        if elem.tag not in TEI_VALID_TAGS:
             # disable warnings for chosen categories
             # if element.tag not in ('div', 'span'):
-            LOGGER.warning('not a TEI element, removing: %s %s', element.tag, url)
-            merge_with_parent(element)
+            LOGGER.warning('not a TEI element, removing: %s %s', elem.tag, url)
+            merge_with_parent(elem)
             continue
-        if element.tag == "div":
-            _handle_text_content_of_div_nodes(element)
-            _wrap_unwanted_siblings_of_div(element)
+        if elem.tag == "div":
+            _handle_text_content_of_div_nodes(elem)
+            _wrap_unwanted_siblings_of_div(elem)
         # check attributes
-        for attribute in element.attrib:
+        for attribute in elem.attrib:
             if attribute not in TEI_VALID_ATTRS:
-                LOGGER.warning('not a valid TEI attribute, removing: %s in %s %s', attribute, element.tag, url)
-                element.attrib.pop(attribute)
+                LOGGER.warning('not a valid TEI attribute, removing: %s in %s %s', attribute, elem.tag, url)
+                elem.attrib.pop(attribute)
     return xmldoc
 
 
 def validate_tei(xmldoc):  # , filename=""
     '''Check if an XML document is conform to the guidelines of the Text Encoding Initiative'''
     global TEI_RELAXNG
     if TEI_RELAXNG is None:
@@ -207,68 +213,64 @@
     result = TEI_RELAXNG.validate(xmldoc)
     if result is False:
         LOGGER.warning('not a valid TEI document: %s', TEI_RELAXNG.error_log.last_error)
     return result
 
 
 def replace_element_text(element, include_formatting):
-    '''Determine element text based on **just the text** of the element. You must deal with the tail separately.'''
-    elem_text = element.text
+    "Determine element text based on just the text of the element. One must deal with the tail separately."
+    elem_text = element.text or ""
     # handle formatting: convert to markdown
-    if include_formatting is True and element.text is not None:
-        if element.tag in ('del', 'head'):
-            if element.tag == 'head':
-                try:
-                    number = int(element.get('rend')[1])
-                except (TypeError, ValueError):
-                    number = 2
-                elem_text = f'{"#" * number} {elem_text}'
-            elif element.tag == 'del':
-                elem_text = f'~~{elem_text}~~'
-        elif element.tag == 'hi':
-            rend = element.get('rend')
+    if include_formatting and element.text:
+        if element.tag == "head":
+            try:
+                number = int(element.get("rend")[1])
+            except (TypeError, ValueError):
+                number = 2
+            elem_text = f'{"#" * number} {elem_text}'
+        elif element.tag == "del":
+            elem_text = f"~~{elem_text}~~"
+        elif element.tag == "hi":
+            rend = element.get("rend")
             if rend in HI_FORMATTING:
-                elem_text = f'{HI_FORMATTING[rend]}{elem_text}{HI_FORMATTING[rend]}'
-        elif element.tag == 'code':
-            if '\n' in element.text:
-                elem_text = f'```\n{elem_text}\n```'
+                elem_text = f"{HI_FORMATTING[rend]}{elem_text}{HI_FORMATTING[rend]}"
+        elif element.tag == "code":
+            if "\n" in element.text:
+                elem_text = f"```\n{elem_text}\n```"
             else:
-                elem_text = f'`{elem_text}`'
+                elem_text = f"`{elem_text}`"
     # handle links
-    if element.tag == 'ref':
-        if elem_text is not None:
-            link_text = f'[{elem_text}]'
-            if element.get('target') is not None:
-                elem_text = f"{link_text}({element.get('target')})"
+    if element.tag == "ref":
+        if elem_text:
+            link_text = f"[{elem_text}]"
+            target = element.get("target")
+            if target:
+                elem_text = f"{link_text}({target})"
             else:
-                LOGGER.warning('missing link attribute: %s %s', elem_text, element.attrib)
+                LOGGER.warning("missing link attribute: %s %s'", elem_text, element.attrib)
                 elem_text = link_text
         else:
-            LOGGER.warning('empty link: %s %s', elem_text, element.attrib)
-    # handle text
-    return (elem_text or '')
+            LOGGER.warning("empty link: %s %s", elem_text, element.attrib)
+    return elem_text
 
 
 def merge_with_parent(element, include_formatting=False):
     '''Merge element with its parent and convert formatting to markdown.'''
     parent = element.getparent()
     if parent is None:
         return
 
     full_text = replace_element_text(element, include_formatting)
     if element.tail is not None:
-        full_text = f'{full_text}{element.tail}'
+        full_text += element.tail
 
     previous = element.getprevious()
     if previous is not None:
         # There is a previous node, append text to its tail
-        if previous.tail is not None:
-            previous.tail = f'{previous.tail} {full_text}'
-        else:
-            previous.tail = full_text
+        previous.tail = f'{previous.tail} {full_text}' if previous.tail else full_text
     elif parent.text is not None:
         parent.text = f'{parent.text} {full_text}'
     else:
         parent.text = full_text
     parent.remove(element)
 
 
@@ -284,23 +286,32 @@
 
     if element.text is None and element.tail is None:
         if element.tag == 'graphic':
             # add source, default to ''
             text = f'{element.get("title", "")} {element.get("alt", "")}'
             returnlist.extend(['![', text.strip(), ']', '(', element.get('src', ''), ')'])
         # newlines for textless elements
-        if element.tag in ('graphic', 'row', 'table'):
+        if element.tag in NEWLINE_ELEMS:
             returnlist.append('\n')
+            # add line after table head
+            if element.tag == "row":
+                num_cells = len(element.xpath("./cell[@role='head']"))
+                if num_cells > 0:
+                    returnlist.append("---|" * len(element.xpath(".//cell")) + "\n")
         return  # Nothing more to do with textless elements
 
     # Process text
 
     # Common elements (Now processes end-tag logic correctly)
-    if element.tag in NEWLINE_ELEMS:
+    if element.tag == 'p' and include_formatting:
+        returnlist.append('\n\u2424\n')
+    elif element.tag in NEWLINE_ELEMS:
         returnlist.extend([NEWLINE_ELEMS[element.tag], '\n'])
+    elif element.tag == 'cell':
+        returnlist.extend(" | ")
     elif element.tag == 'comments':
         returnlist.append('\n\n')
     else:
         if element.tag not in SPECIAL_FORMATTING:
             LOGGER.debug('unprocessed element in output: %s', element.tag)
             returnlist.extend([' '])
 
@@ -328,30 +339,27 @@
         commentstext = ""
 
     # output config
     output = StringIO()
     outputwriter = csv.writer(output, delimiter=delim, quoting=csv.QUOTE_MINIMAL)
 
     # organize fields
-    data = [d or null for d in (
-                document.url,
-                document.id,
-                document.fingerprint,
-                document.hostname,
-                document.title,
-                document.image,
-                document.date,
-                posttext,
-                commentstext,
-                document.license,
-                document.pagetype,
-                )
-            ]
+    data = (document.url,
+            document.id,
+            document.fingerprint,
+            document.hostname,
+            document.title,
+            document.image,
+            document.date,
+            posttext,
+            commentstext,
+            document.license,
+            document.pagetype)
 
-    outputwriter.writerow(data)
+    outputwriter.writerow([d if d else null for d in data])
     return output.getvalue()
 
 
 def write_teitree(docmeta):
     '''Bundle the extracted post and comments into a TEI tree'''
     teidoc = Element('TEI', xmlns='http://www.tei-c.org/ns/1.0')
     header = write_fullheader(teidoc, docmeta)
@@ -455,52 +463,50 @@
         keywords = SubElement(textclass, 'keywords')
         if len(docmeta.categories) > 0:
             cat_list = SubElement(keywords, 'term', type='categories')
             cat_list.text = ','.join(docmeta.categories)
         if len(docmeta.tags) > 0:
             tags_list = SubElement(keywords, 'term', type='tags')
             tags_list.text = ','.join(docmeta.tags)
+    creation = SubElement(profiledesc, 'creation')
+    date = SubElement(creation, 'date', type="download")
+    date.text = docmeta.filedate
     encodingdesc = SubElement(header, 'encodingDesc')
     appinfo = SubElement(encodingdesc, 'appInfo')
     application = SubElement(appinfo, 'application', version=PKG_VERSION, ident='Trafilatura')
     label = SubElement(application, 'label')
     label.text = 'Trafilatura'
     pointer = SubElement(application, 'ptr', target='https://github.com/adbar/trafilatura')
     return header
 
 
 def _handle_text_content_of_div_nodes(element):
     if element.text and element.text.strip():
-        if element.getchildren() and element[0].tag == 'p':
-            p_text = element[0].text or ""
-            element[0].text = f'{element.text} {p_text}'.strip()
+        if element.getchildren() and element[0].tag == "p":
+            element[0].text = f'{element.text} {element[0].text or ""}'.strip()
         else:
             new_child = Element("p")
             new_child.text = element.text
             element.insert(0, new_child)
         element.text = None
 
     if element.tail and element.tail.strip():
-        if element.getchildren() and element[-1].tag == 'p':
-            p_text = element[-1].text or ""
-            element[-1].text = f'{p_text} {element.tail}'.strip()
+        if element.getchildren() and element[-1].tag == "p":
+            element[-1].text = f'{element[-1].text or ""} {element.tail}'.strip()
         else:
             new_child = Element("p")
             new_child.text = element.tail
             element.append(new_child)
         element.tail = None
 
 
 def _handle_unwanted_tails(element):
     "Handle tail on p and ab elements"
-    if element.tag == 'p':
-        if element.text:
-            element.text += ' ' + element.tail.strip()
-        else:
-            element.text = element.tail
+    if element.tag == "p":
+        element.text = element.text + " " + element.tail.strip() if element.text else element.tail
     else:
         new_sibling = Element('p')
         new_sibling.text = element.tail.strip()
         parent = element.getparent()
         parent.insert(parent.index(element) + 1 , new_sibling)
     element.tail = None
 
@@ -515,39 +521,38 @@
                 if len(new_element) == 0 or new_element[-1].tail:
                     SubElement(new_element, 'lb')
                 new_element[-1].tail = child.text
             else:
                 new_element.text = child.text
         else:
             new_element.append(child)
-    if element.tail is not None and element.tail.strip():
+    if element.tail and element.tail.strip():
         new_element.tail = element.tail.strip()
     return new_element
 
 
 def _wrap_unwanted_siblings_of_div(div_element):
     new_sibling = Element("div")
     new_sibling_index = None
     parent = div_element.getparent()
     # check siblings after target element
     for sibling in div_element.itersiblings():
         if sibling.tag == "div":
             break
-        if sibling.tag in {"p", "list", "table", "quote", "ab"}:
-            if new_sibling_index is None:
-                new_sibling_index = parent.index(sibling)
+        if sibling.tag in TEI_DIV_SIBLINGS:
+            new_sibling_index = new_sibling_index or parent.index(sibling)
             new_sibling.append(sibling)
         # some elements (e.g. <lb/>) can appear next to div, but
         # order of elements should be kept, thus add and reset new_sibling
         else:
-            if new_sibling_index is not None and len(new_sibling) != 0:
+            if new_sibling_index and len(new_sibling) != 0:
                 parent.insert(new_sibling_index, new_sibling)
                 new_sibling = Element("div")
                 new_sibling_index = None
-    if new_sibling_index is not None and len(new_sibling) != 0:
+    if new_sibling_index and len(new_sibling) != 0:
         parent.insert(new_sibling_index, new_sibling)
 
 
 def _move_element_one_level_up(element):
     """
     Fix TEI compatibility issues by moving certain p-elems up in the XML tree.
     There is always a n+2 nesting for p-elements with the minimal structure ./TEI/text/body/p
```

### Comparing `trafilatura-1.8.1/trafilatura.egg-info/PKG-INFO` & `trafilatura-1.9.0/trafilatura.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trafilatura
-Version: 1.8.1
+Version: 1.9.0
 Summary: Python package and command-line tool designed to gather text on the Web, includes all necessary discovery and text processing components to perform web crawling, downloads, scraping, and extraction of main texts, metadata and comments.
 Home-page: https://trafilatura.readthedocs.io
 Author: Adrien Barbaresi
 Author-email: barbaresi@bbaw.de
 License: Apache-2.0
 Project-URL: Documentation, https://trafilatura.readthedocs.io
 Project-URL: Source, https://github.com/adbar/trafilatura
@@ -35,244 +35,260 @@
 Classifier: Topic :: Text Editors :: Text Processing
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Classifier: Topic :: Text Processing :: Markup :: XML
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: certifi
 Requires-Dist: charset_normalizer>=3.0.1; python_version < "3.7"
 Requires-Dist: charset_normalizer>=3.2.0; python_version >= "3.7"
-Requires-Dist: courlan>=1.0.0
-Requires-Dist: htmldate>=1.8.0
+Requires-Dist: courlan>=1.1.0
+Requires-Dist: htmldate>=1.8.1
 Requires-Dist: importlib_metadata; python_version < "3.8"
 Requires-Dist: justext>=3.0.0
 Requires-Dist: lxml==4.9.2; platform_system == "Darwin" and python_version <= "3.8"
 Requires-Dist: lxml<5.2.0,>=4.9.4; platform_system != "Darwin" or python_version > "3.8"
 Requires-Dist: urllib3<2,>=1.26; python_version < "3.7"
 Requires-Dist: urllib3<3,>=1.26; python_version >= "3.7"
 Provides-Extra: all
 Requires-Dist: brotli; extra == "all"
 Requires-Dist: cchardet>=2.1.7; python_version < "3.11" and extra == "all"
 Requires-Dist: faust-cchardet>=2.1.19; python_version >= "3.11" and extra == "all"
-Requires-Dist: htmldate[speed]>=1.8.0; extra == "all"
+Requires-Dist: htmldate[speed]>=1.8.1; extra == "all"
 Requires-Dist: py3langid>=0.2.2; extra == "all"
 Requires-Dist: pycurl>=7.45.3; extra == "all"
 Provides-Extra: gui
 Requires-Dist: Gooey>=1.0.1; extra == "gui"
 
-Trafilatura: Discover and Extract Text Data on the Web
-======================================================
+# Trafilatura: Discover and Extract Text Data on the Web
 
+<br/>
 
-.. image:: https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-logo.png
-   :alt: Trafilatura Logo
-   :align: center
-   :width: 60%
+<img alt="Trafilatura Logo" src="https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-logo.png" align="center" width="60%"/>
 
-|
+<br/>
 
-.. image:: https://img.shields.io/pypi/v/trafilatura.svg
-    :target: https://pypi.python.org/pypi/trafilatura
-    :alt: Python package
+[![Python package](https://img.shields.io/pypi/v/trafilatura.svg)](https://pypi.python.org/pypi/trafilatura)
+[![Python versions](https://img.shields.io/pypi/pyversions/trafilatura.svg)](https://pypi.python.org/pypi/trafilatura)
+[![Documentation Status](https://readthedocs.org/projects/trafilatura/badge/?version=latest)](http://trafilatura.readthedocs.org/en/latest/?badge=latest)
+[![Code Coverage](https://img.shields.io/codecov/c/github/adbar/trafilatura.svg)](https://codecov.io/gh/adbar/trafilatura)
+[![Downloads](https://static.pepy.tech/badge/trafilatura/month)](https://pepy.tech/project/trafilatura)
+[![Reference DOI: 10.18653/v1/2021.acl-demo.15](https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue)](https://aclanthology.org/2021.acl-demo.15/)
 
-.. image:: https://img.shields.io/pypi/pyversions/trafilatura.svg
-    :target: https://pypi.python.org/pypi/trafilatura
-    :alt: Python versions
+<br/>
 
-.. image:: https://readthedocs.org/projects/trafilatura/badge/?version=latest
-    :target: http://trafilatura.readthedocs.org/en/latest/?badge=latest
-    :alt: Documentation Status
+<img alt="Demo as GIF image" src="https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-demo.gif" align="center" width="80%"/>
 
-.. image:: https://img.shields.io/codecov/c/github/adbar/trafilatura.svg
-    :target: https://codecov.io/gh/adbar/trafilatura
-    :alt: Code Coverage
+<br/>
 
-.. image:: https://static.pepy.tech/badge/trafilatura/month
-    :target: https://pepy.tech/project/trafilatura
-    :alt: Downloads
 
-.. image:: https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue
-    :target: https://aclanthology.org/2021.acl-demo.15/
-    :alt: Reference DOI: 10.18653/v1/2021.acl-demo.15
+## Introduction
 
-|
+Trafilatura is a cutting-edge **Python package and command-line tool**
+designed to **gather text on the Web and simplify the process of turning
+raw HTML into structured, meaningful data**. It includes all necessary
+discovery and text processing components to perform **web crawling,
+downloads, scraping, and extraction** of main texts, metadata and
+comments. It aims at staying **handy and modular**: no database is
+required, the output can be converted to commonly used formats.
 
-.. image:: https://raw.githubusercontent.com/adbar/trafilatura/master/docs/trafilatura-demo.gif
-    :alt: Demo as GIF image
-    :align: center
-    :width: 85%
-    :target: https://trafilatura.readthedocs.org/
+Going from HTML bulk to essential parts can alleviate many problems
+related to text quality, by **focusing on the actual content**,
+**avoiding the noise** caused by recurring elements (headers, footers
+etc.), and **making sense of the data** with selected information. The
+extractor is designed to be **robust and reasonably fast**, it runs in
+production on millions of documents.
 
+The tool's versatility makes it **useful for quantitative and
+data-driven approaches**. It is used in the academic domain and beyond
+(e.g. in natural language processing, computational social science,
+search engine optimization, and information security).
 
-Introduction
-------------
 
-
-Trafilatura is a cutting-edge **Python package and command-line tool** designed to **gather text on the Web and simplify the process of turning raw HTML into structured, meaningful data**. It includes all necessary discovery and text processing components to perform **web crawling, downloads, scraping, and extraction** of main texts, metadata and comments. It aims at staying **handy and modular**: no database is required, the output can be converted to commonly used formats.
-
-Going from HTML bulk to essential parts can alleviate many problems related to text quality, by **focusing on the actual content**, **avoiding the noise** caused by recurring elements (headers, footers etc.), and **making sense of the data** with selected information. The extractor is designed to be **robust and reasonably fast**, it runs in production on millions of documents.
-
-The tool's versatility makes it **useful for quantitative and data-driven approaches**. It is used in the academic domain and beyond (e.g. in natural language processing, computational social science, search engine optimization, and information security).
-
-
-Features
-~~~~~~~~
+### Features
 
 - Advanced web crawling and text discovery:
    - Support for sitemaps (TXT, XML) and feeds (ATOM, JSON, RSS)
    - Smart crawling and URL management (filtering and deduplication)
+
 - Parallel processing of online and offline input:
    - Live URLs, efficient and polite processing of download queues
    - Previously downloaded HTML files and parsed HTML trees
+
 - Robust and configurable extraction of key elements:
    - Main text (common patterns and generic algorithms like jusText and readability)
    - Metadata (title, author, date, site name, categories and tags)
    - Formatting and structure: paragraphs, titles, lists, quotes, code, line breaks, in-line text formatting
    - Optional elements: comments, links, images, tables
+
 - Multiple output formats:
    - Text (minimal formatting or Markdown)
    - CSV (with metadata)
    - JSON (with metadata)
-   - XML or `XML-TEI <https://tei-c.org/>`_ (with metadata, text formatting and page structure)
+   - XML or [XML-TEI](https://tei-c.org/) (with metadata, text formatting and page structure)
+
 - Optional add-ons:
    - Language detection on extracted content
    - Graphical user interface (GUI)
    - Speed optimizations
+
 - Actively maintained with support from the open-source community:
    - Regular updates, feature additions, and optimizations
    - Comprehensive documentation
 
 
-Evaluation and alternatives
-~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Trafilatura consistently outperforms other open-source libraries in text extraction benchmarks, showcasing its efficiency and accuracy in extracting web content. The extractor tries to strike a balance between limiting noise and including all valid parts.
-
-For more information see the `benchmark section <https://trafilatura.readthedocs.io/en/latest/evaluation.html>`_ and the `evaluation readme <https://github.com/adbar/trafilatura/blob/master/tests/README.rst>`_ to reproduce the results.
-
-
-=============================== =========  ========== ========= ========= ======
-750 documents, 2236 text & 2250 boilerplate segments (2022-05-18), Python 3.8
---------------------------------------------------------------------------------
-Python Package                  Precision  Recall     Accuracy  F-Score   Diff.
-=============================== =========  ========== ========= ========= ======
-html_text 0.5.2                 0.529      **0.958**  0.554     0.682     2.2x
-inscriptis 2.2.0 (html to txt)  0.534      **0.959**  0.563     0.686     3.5x
-newspaper3k 0.2.8               0.895      0.593      0.762     0.713     12x
-justext 3.0.0 (custom)          0.865      0.650      0.775     0.742     5.2x
-boilerpy3 1.0.6 (article mode)  0.814      0.744      0.787     0.777     4.1x
-*baseline (text markup)*        0.757      0.827      0.781     0.790     **1x**
-goose3 3.1.9                    **0.934**  0.690      0.821     0.793     22x
-readability-lxml 0.8.1          0.891      0.729      0.820     0.801     5.8x
-news-please 1.5.22              0.898      0.734      0.826     0.808     61x
-readabilipy 0.2.0               0.877      0.870      0.874     0.874     248x
-trafilatura 1.2.2 (standard)    0.914      0.904      **0.910** **0.909** 7.1x
-=============================== =========  ========== ========= ========= ======
-
-
-Other evaluations:
-^^^^^^^^^^^^^^^^^^
-
-- Most efficient open-source library in *ScrapingHub*'s `article extraction benchmark <https://github.com/scrapinghub/article-extraction-benchmark>`_
-- Best overall tool according to `Bien choisir son outil d'extraction de contenu à partir du Web <https://hal.archives-ouvertes.fr/hal-02768510v3/document>`_ (Lejeune & Barbaresi 2020)
-- Best single tool by ROUGE-LSum Mean F1 Page Scores in `An Empirical Comparison of Web Content Extraction Algorithms <https://webis.de/downloads/publications/papers/bevendorff_2023b.pdf>`_ (Bevendorff et al. 2023)
-
-
-Usage and documentation
------------------------
-
-`Getting started with Trafilatura <https://trafilatura.readthedocs.io/en/latest/quickstart.html>`_ is straightforward. For more information and detailed guides, visit `Trafilatura's documentation <https://trafilatura.readthedocs.io/>`_:
-
-- `Installation <https://trafilatura.readthedocs.io/en/latest/installation.html>`_
-- Usage: `On the command-line <https://trafilatura.readthedocs.io/en/latest/usage-cli.html>`_, `With Python <https://trafilatura.readthedocs.io/en/latest/usage-python.html>`_, `With R <https://trafilatura.readthedocs.io/en/latest/usage-r.html>`_
-- `Core Python functions <https://trafilatura.readthedocs.io/en/latest/corefunctions.html>`_
-- Interactive Python Notebook: `Trafilatura Overview <docs/Trafilatura_Overview.ipynb>`_
-- `Tutorials and use cases <https://trafilatura.readthedocs.io/en/latest/tutorials.html>`_
+### Evaluation and alternatives
 
+Trafilatura consistently outperforms other open-source libraries in text
+extraction benchmarks, showcasing its efficiency and accuracy in
+extracting web content. The extractor tries to strike a balance between
+limiting noise and including all valid parts.
+
+For more information see the [benchmark section](https://trafilatura.readthedocs.io/en/latest/evaluation.html)
+and the [evaluation readme](https://github.com/adbar/trafilatura/blob/master/tests/README.rst)
+to reproduce the results.
+
+**750 documents, 2236 text & 2250 boilerplate segments (2022-05-18), Python 3.8**
+
+| Python Package | Precision | Recall | Accuracy | F-Score | Diff. |
+|----------------|-----------|--------|----------|---------|-------|
+| html_text 0.5.2 | 0.529 | **0.958** | 0.554 | 0.682 | 2.2x |
+| inscriptis 2.2.0 (html to txt) | 0.534 | **0.959** | 0.563 | 0.686 | 3.5x |
+| newspaper3k 0.2.8 | 0.895 | 0.593 | 0.762 | 0.713 | 12x |
+| justext 3.0.0 (custom) | 0.865 | 0.650 | 0.775 | 0.742 | 5.2x |
+| boilerpy3 1.0.6 (article mode) | 0.814 | 0.744 | 0.787 | 0.777 | 4.1x |
+| *baseline (text markup)* | 0.757 | 0.827 | 0.781 | 0.790 | **1x** |
+| goose3 3.1.9 | **0.934** | 0.690 | 0.821 | 0.793 | 22x |
+| readability-lxml 0.8.1 | 0.891 | 0.729 | 0.820 | 0.801 | 5.8x |
+| news-please 1.5.22 | 0.898 | 0.734 | 0.826 | 0.808 | 61x |
+| readabilipy 0.2.0 | 0.877 | 0.870 | 0.874 | 0.874 | 248x |
+| trafilatura 1.2.2 (standard) | 0.914 | 0.904 | **0.910** | **0.909** | 7.1x |
+
+
+#### Other evaluations:
+
+- Most efficient open-source library in *ScrapingHub*'s [article extraction benchmark](https://github.com/scrapinghub/article-extraction-benchmark)
+- Best overall tool according to [Bien choisir son outil d'extraction de contenu à partir du Web](https://hal.archives-ouvertes.fr/hal-02768510v3/document)
+  (Lejeune & Barbaresi 2020)
+- Best single tool by ROUGE-LSum Mean F1 Page Scores in [An Empirical Comparison of Web Content Extraction Algorithms](https://webis.de/downloads/publications/papers/bevendorff_2023b.pdf)
+  (Bevendorff et al. 2023)
+
+
+## Usage and documentation
+
+[Getting started with Trafilatura](https://trafilatura.readthedocs.io/en/latest/quickstart.html)
+is straightforward. For more information and detailed guides, visit
+[Trafilatura's documentation](https://trafilatura.readthedocs.io/):
+
+- [Installation](https://trafilatura.readthedocs.io/en/latest/installation.html)
+- Usage:
+  [On the command-line](https://trafilatura.readthedocs.io/en/latest/usage-cli.html),
+  [With Python](https://trafilatura.readthedocs.io/en/latest/usage-python.html),
+  [With R](https://trafilatura.readthedocs.io/en/latest/usage-r.html)
+- [Core Python functions](https://trafilatura.readthedocs.io/en/latest/corefunctions.html)
+- Interactive Python Notebook: [Trafilatura Overview](docs/Trafilatura_Overview.ipynb)
+- [Tutorials and use cases](https://trafilatura.readthedocs.io/en/latest/tutorials.html)
 
 Youtube playlist with video tutorials in several languages:
 
-- `Web scraping tutorials and how-tos <https://www.youtube.com/watch?v=8GkiOM17t0Q&list=PL-pKWbySIRGMgxXQOtGIz1-nbfYLvqrci>`_
+- [Web scraping tutorials and how-tos](https://www.youtube.com/watch?v=8GkiOM17t0Q&list=PL-pKWbySIRGMgxXQOtGIz1-nbfYLvqrci)
 
 
-License
--------
+## License
 
-This package is distributed under the `Apache 2.0 license <https://www.apache.org/licenses/LICENSE-2.0.html>`_.
+This package is distributed under the [Apache 2.0 license](https://www.apache.org/licenses/LICENSE-2.0.html).
 
 Versions prior to v1.8.0 are under GPLv3+ license.
 
 
-Contributing
-------------
-
-Contributions of all kinds are welcome. Visit the `Contributing page <https://github.com/adbar/trafilatura/blob/master/CONTRIBUTING.md>`_ for more information. Bug reports can be filed on the `dedicated issue page <https://github.com/adbar/trafilatura/issues>`_.
-
-Many thanks to the `contributors <https://github.com/adbar/trafilatura/graphs/contributors>`_ who extended the docs or submitted bug reports, features and bugfixes!
-
-
-Context
--------
-
-Developed with practical applications of academic research in mind, this software is part of a broader effort to derive information from web documents. Extracting and pre-processing web texts to the exacting standards of scientific research presents a substantial challenge. This software package simplifies text data collection and enhances corpus quality, it is currently used to build `text databases for linguistic research <https://www.dwds.de/d/k-web>`_.
-
-*Trafilatura* is an Italian word for `wire drawing <https://en.wikipedia.org/wiki/Wire_drawing>`_ symbolizing the refinement and conversion process. It is also the way shapes of pasta are formed.
-
-
-Author
-~~~~~~
-
-Reach out via ia the software repository or the `contact page <https://adrien.barbaresi.eu/>`_ for inquiries, collaborations, or feedback. See also X or LinkedIn for the latest updates.
-
-This work started as a PhD project at the crossroads of linguistics and NLP, this expertise has been instrumental in shaping Trafilatura over the years. It has first been released under its current form in 2019, its development is referenced in the following publications:
-
-- Barbaresi, A. `Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction <https://aclanthology.org/2021.acl-demo.15/>`_, Proceedings of ACL/IJCNLP 2021: System Demonstrations, 2021, p. 122-131.
--  Barbaresi, A. "`Generic Web Content Extraction with Open-Source Software <https://hal.archives-ouvertes.fr/hal-02447264/document>`_", Proceedings of KONVENS 2019, Kaleidoscope Abstracts, 2019.
--  Barbaresi, A. "`Efficient construction of metadata-enhanced web corpora <https://hal.archives-ouvertes.fr/hal-01371704v2/document>`_", Proceedings of the `10th Web as Corpus Workshop (WAC-X) <https://www.sigwac.org.uk/wiki/WAC-X>`_, 2016.
-
-
-Citing Trafilatura
-~~~~~~~~~~~~~~~~~~
-
-Trafilatura is widely used in the academic domain, chiefly for data acquisition. Here is how to cite it:
-
-.. image:: https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue
-    :target: https://aclanthology.org/2021.acl-demo.15/
-    :alt: Reference DOI: 10.18653/v1/2021.acl-demo.15
-
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3460969.svg
-   :target: https://doi.org/10.5281/zenodo.3460969
-   :alt: Zenodo archive DOI: 10.5281/zenodo.3460969
-
-.. code-block:: shell
-
-    @inproceedings{barbaresi-2021-trafilatura,
-      title = {{Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction}},
-      author = "Barbaresi, Adrien",
-      booktitle = "Proceedings of the Joint Conference of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing: System Demonstrations",
-      pages = "122--131",
-      publisher = "Association for Computational Linguistics",
-      url = "https://aclanthology.org/2021.acl-demo.15",
-      year = 2021,
-    }
-
-
-Software ecosystem
-~~~~~~~~~~~~~~~~~~
-
-Case studies and publications are listed on the `Used By documentation page <https://trafilatura.readthedocs.io/en/latest/used-by.html>`_.
-
-Jointly developed plugins and additional packages also contribute to the field of web data extraction and analysis:
-
-
-.. image:: https://raw.githubusercontent.com/adbar/htmldate/master/docs/software-ecosystem.png
-    :alt: Software ecosystem
-    :align: center
-    :width: 65%
-
-
+## Contributing
 
-Corresponding posts can be found on `Bits of Language <https://adrien.barbaresi.eu/blog/tag/trafilatura.html>`_. The blog covers a range of topics from technical how-tos, updates on new features, to discussions on text mining challenges and solutions.
+Contributions of all kinds are welcome. Visit the [Contributing
+page](https://github.com/adbar/trafilatura/blob/master/CONTRIBUTING.md)
+for more information. Bug reports can be filed on the [dedicated issue
+page](https://github.com/adbar/trafilatura/issues).
+
+Many thanks to the
+[contributors](https://github.com/adbar/trafilatura/graphs/contributors)
+who extended the docs or submitted bug reports, features and bugfixes!
+
+
+## Context
+
+Developed with practical applications of academic research in mind, this
+software is part of a broader effort to derive information from web
+documents. Extracting and pre-processing web texts to the exacting
+standards of scientific research presents a substantial challenge. This
+software package simplifies text data collection and enhances corpus
+quality, it is currently used to build [text databases for linguistic
+research](https://www.dwds.de/d/k-web).
+
+*Trafilatura* is an Italian word for [wire
+drawing](https://en.wikipedia.org/wiki/Wire_drawing) symbolizing the
+refinement and conversion process. It is also the way shapes of pasta
+are formed.
+
+### Author
+
+Reach out via ia the software repository or the [contact
+page](https://adrien.barbaresi.eu/) for inquiries, collaborations, or
+feedback. See also X or LinkedIn for the latest updates.
+
+This work started as a PhD project at the crossroads of linguistics and
+NLP, this expertise has been instrumental in shaping Trafilatura over
+the years. It has first been released under its current form in 2019,
+its development is referenced in the following publications:
+
+-   Barbaresi, A. [Trafilatura: A Web Scraping Library and Command-Line
+    Tool for Text Discovery and
+    Extraction](https://aclanthology.org/2021.acl-demo.15/), Proceedings
+    of ACL/IJCNLP 2021: System Demonstrations, 2021, p. 122-131.
+-   Barbaresi, A. "[Generic Web Content Extraction with Open-Source
+    Software](https://hal.archives-ouvertes.fr/hal-02447264/document)",
+    Proceedings of KONVENS 2019, Kaleidoscope Abstracts, 2019.
+-   Barbaresi, A. "[Efficient construction of metadata-enhanced web
+    corpora](https://hal.archives-ouvertes.fr/hal-01371704v2/document)",
+    Proceedings of the [10th Web as Corpus Workshop
+    (WAC-X)](https://www.sigwac.org.uk/wiki/WAC-X), 2016.
+
+
+### Citing Trafilatura
+
+Trafilatura is widely used in the academic domain, chiefly for data
+acquisition. Here is how to cite it:
+
+[![Reference DOI: 10.18653/v1/2021.acl-demo.15](https://img.shields.io/badge/DOI-10.18653%2Fv1%2F2021.acl--demo.15-blue)](https://aclanthology.org/2021.acl-demo.15/)
+[![Zenodo archive DOI: 10.5281/zenodo.3460969](https://zenodo.org/badge/DOI/10.5281/zenodo.3460969.svg)](https://doi.org/10.5281/zenodo.3460969)
+
+``` shell
+@inproceedings{barbaresi-2021-trafilatura,
+  title = {{Trafilatura: A Web Scraping Library and Command-Line Tool for Text Discovery and Extraction}},
+  author = "Barbaresi, Adrien",
+  booktitle = "Proceedings of the Joint Conference of the 59th Annual Meeting of the Association for Computational Linguistics and the 11th International Joint Conference on Natural Language Processing: System Demonstrations",
+  pages = "122--131",
+  publisher = "Association for Computational Linguistics",
+  url = "https://aclanthology.org/2021.acl-demo.15",
+  year = 2021,
+}
+```
+
+
+### Software ecosystem
+
+Case studies and publications are listed on the [Used By documentation
+page](https://trafilatura.readthedocs.io/en/latest/used-by.html).
+
+Jointly developed plugins and additional packages also contribute to the
+field of web data extraction and analysis:
+
+<img alt="Software ecosystem" src="https://raw.githubusercontent.com/adbar/htmldate/master/docs/software-ecosystem.png" align="center" width="65%"/>
+
+Corresponding posts can be found on [Bits of
+Language](https://adrien.barbaresi.eu/blog/tag/trafilatura.html). The
+blog covers a range of topics from technical how-tos, updates on new
+features, to discussions on text mining challenges and solutions.
 
-Impressive, you have reached the end of the page: Thank you for your interest!
+Impressive, you have reached the end of the page: Thank you for your
+interest!
```

### Comparing `trafilatura-1.8.1/trafilatura.egg-info/SOURCES.txt` & `trafilatura-1.9.0/trafilatura.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 CITATION.cff
 CONTRIBUTING.md
 HISTORY.md
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 pytest.ini
 setup.py
 docs/Makefile
 docs/background.rst
 docs/compendium.rst
 docs/conf.py
 docs/corefunctions.rst
@@ -84,29 +84,30 @@
 tests/resources/sitemap.xml
 tests/resources/sitemap.xml.gz
 tests/resources/sitemap2.xml
 tests/resources/utf8.html
 tests/resources/webpage.html.gz
 tests/resources/zerolength.cfg
 trafilatura/__init__.py
+trafilatura/baseline.py
 trafilatura/cli.py
 trafilatura/cli_utils.py
 trafilatura/core.py
 trafilatura/downloads.py
 trafilatura/external.py
 trafilatura/feeds.py
 trafilatura/filters.py
 trafilatura/gui.py
 trafilatura/hashing.py
 trafilatura/htmlprocessing.py
 trafilatura/json_metadata.py
 trafilatura/lru.py
+trafilatura/main_extractor.py
 trafilatura/meta.py
 trafilatura/metadata.py
-trafilatura/metaxpaths.py
 trafilatura/readability_lxml.py
 trafilatura/settings.cfg
 trafilatura/settings.py
 trafilatura/sitemaps.py
 trafilatura/spider.py
 trafilatura/utils.py
 trafilatura/xml.py
```

### Comparing `trafilatura-1.8.1/trafilatura.egg-info/requires.txt` & `trafilatura-1.9.0/trafilatura.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 certifi
-courlan>=1.0.0
-htmldate>=1.8.0
+courlan>=1.1.0
+htmldate>=1.8.1
 justext>=3.0.0
 
 [:platform_system != "Darwin" or python_version > "3.8"]
 lxml<5.2.0,>=4.9.4
 
 [:platform_system == "Darwin" and python_version <= "3.8"]
 lxml==4.9.2
@@ -18,15 +18,15 @@
 
 [:python_version >= "3.7"]
 charset_normalizer>=3.2.0
 urllib3<3,>=1.26
 
 [all]
 brotli
-htmldate[speed]>=1.8.0
+htmldate[speed]>=1.8.1
 py3langid>=0.2.2
 pycurl>=7.45.3
 
 [all:python_version < "3.11"]
 cchardet>=2.1.7
 
 [all:python_version >= "3.11"]
```

