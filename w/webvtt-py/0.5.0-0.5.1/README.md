# Comparing `tmp/webvtt-py-0.5.0.tar.gz` & `tmp/webvtt-py-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webvtt-py-0.5.0.tar", last modified: Wed May 15 16:02:39 2024, max compression
+gzip compressed data, was "webvtt-py-0.5.1.tar", last modified: Thu May 30 13:40:01 2024, max compression
```

## Comparing `webvtt-py-0.5.0.tar` & `webvtt-py-0.5.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-15 16:02:39.438855 webvtt-py-0.5.0/
--rw-r--r--   0 amendez    (501) staff       (20)     1072 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/LICENSE
--rw-r--r--   0 amendez    (501) staff       (20)      100 2021-01-27 19:12:00.000000 webvtt-py-0.5.0/MANIFEST.in
--rw-r--r--   0 amendez    (501) staff       (20)     4146 2024-05-15 16:02:39.439647 webvtt-py-0.5.0/PKG-INFO
--rw-r--r--   0 amendez    (501) staff       (20)     2407 2024-05-15 15:38:13.000000 webvtt-py-0.5.0/README.rst
--rw-r--r--   0 amendez    (501) staff       (20)      605 2024-05-15 16:02:39.441667 webvtt-py-0.5.0/setup.cfg
--rw-r--r--   0 amendez    (501) staff       (20)     1576 2024-05-15 15:38:26.000000 webvtt-py-0.5.0/setup.py
-drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-15 16:02:39.361935 webvtt-py-0.5.0/tests/
--rw-r--r--   0 amendez    (501) staff       (20)        0 2021-01-27 19:12:00.000000 webvtt-py-0.5.0/tests/__init__.py
-drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-15 16:02:39.412338 webvtt-py-0.5.0/tests/samples/
--rw-r--r--   0 amendez    (501) staff       (20)      197 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/captions_with_bom.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      395 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/comments.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      234 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/cue_tags.vtt
--rw-r--r--   0 amendez    (501) staff       (20)        0 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/empty.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      327 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid.vtt
--rw-r--r--   0 amendez    (501) staff       (20)        9 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_format.sbv
--rw-r--r--   0 amendez    (501) staff       (20)        1 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_format1.srt
--rw-r--r--   0 amendez    (501) staff       (20)        9 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_format2.srt
--rw-r--r--   0 amendez    (501) staff       (20)       11 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_format3.srt
--rw-r--r--   0 amendez    (501) staff       (20)       39 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_format4.srt
--rw-r--r--   0 amendez    (501) staff       (20)      203 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_timeframe.sbv
--rw-r--r--   0 amendez    (501) staff       (20)      243 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_timeframe.srt
--rw-r--r--   0 amendez    (501) staff       (20)      335 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_timeframe.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      177 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/invalid_timeframe_in_cue_text.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      128 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/metadata_headers.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      190 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/metadata_headers_multiline.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      187 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_caption_text.sbv
--rw-r--r--   0 amendez    (501) staff       (20)      228 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_caption_text.srt
--rw-r--r--   0 amendez    (501) staff       (20)      225 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_caption_text.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      179 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_timeframe.sbv
--rw-r--r--   0 amendez    (501) staff       (20)      213 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_timeframe.srt
--rw-r--r--   0 amendez    (501) staff       (20)      305 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/missing_timeframe.vtt
--rwxr-xr-x   0 amendez    (501) staff       (20)   120238 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/netflix_chicas_del_cable.vtt
--rw-r--r--   0 amendez    (501) staff       (20)        6 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/no_captions.vtt
--rw-r--r--   0 amendez    (501) staff       (20)       47 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/one_caption.srt
--rw-r--r--   0 amendez    (501) staff       (20)       53 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/one_caption.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      237 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/sample.sbv
--rw-r--r--   0 amendez    (501) staff       (20)      243 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/sample.srt
--rw-r--r--   0 amendez    (501) staff       (20)      765 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/sample.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      205 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/styles.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      343 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/styles_with_comments.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      114 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/two_captions.sbv
--rw-r--r--   0 amendez    (501) staff       (20)      305 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/using_identifiers.vtt
--rw-r--r--   0 amendez    (501) staff       (20)      649 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/samples/youtube_dl.vtt
--rw-r--r--   0 amendez    (501) staff       (20)     6067 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_cli.py
--rw-r--r--   0 amendez    (501) staff       (20)    13226 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_models.py
--rw-r--r--   0 amendez    (501) staff       (20)     4071 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_sbv.py
--rw-r--r--   0 amendez    (501) staff       (20)    10159 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_segmenter.py
--rw-r--r--   0 amendez    (501) staff       (20)     4510 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_srt.py
--rw-r--r--   0 amendez    (501) staff       (20)      875 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_utils.py
--rw-r--r--   0 amendez    (501) staff       (20)    16025 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/tests/test_vtt.py
--rw-r--r--   0 amendez    (501) staff       (20)    39127 2024-05-15 15:38:13.000000 webvtt-py-0.5.0/tests/test_webvtt.py
-drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-15 16:02:39.426325 webvtt-py-0.5.0/webvtt/
--rw-r--r--   0 amendez    (501) staff       (20)      461 2024-05-15 15:38:13.000000 webvtt-py-0.5.0/webvtt/__init__.py
--rw-r--r--   0 amendez    (501) staff       (20)     1338 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/cli.py
--rw-r--r--   0 amendez    (501) staff       (20)      279 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/errors.py
--rw-r--r--   0 amendez    (501) staff       (20)     6942 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/models.py
--rw-r--r--   0 amendez    (501) staff       (20)     2917 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/sbv.py
--rw-r--r--   0 amendez    (501) staff       (20)     3669 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/segmenter.py
--rw-r--r--   0 amendez    (501) staff       (20)     3723 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/srt.py
--rw-r--r--   0 amendez    (501) staff       (20)     2901 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/utils.py
--rw-r--r--   0 amendez    (501) staff       (20)    10823 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/vtt.py
--rw-r--r--   0 amendez    (501) staff       (20)    11292 2024-05-14 10:27:10.000000 webvtt-py-0.5.0/webvtt/webvtt.py
-drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-15 16:02:39.437521 webvtt-py-0.5.0/webvtt_py.egg-info/
--rw-r--r--   0 amendez    (501) staff       (20)     4146 2024-05-15 16:02:39.000000 webvtt-py-0.5.0/webvtt_py.egg-info/PKG-INFO
--rw-r--r--   0 amendez    (501) staff       (20)     1693 2024-05-15 16:02:39.000000 webvtt-py-0.5.0/webvtt_py.egg-info/SOURCES.txt
--rw-r--r--   0 amendez    (501) staff       (20)        1 2024-05-15 16:02:39.000000 webvtt-py-0.5.0/webvtt_py.egg-info/dependency_links.txt
--rw-r--r--   0 amendez    (501) staff       (20)       44 2024-05-15 16:02:39.000000 webvtt-py-0.5.0/webvtt_py.egg-info/entry_points.txt
--rw-r--r--   0 amendez    (501) staff       (20)        7 2024-05-15 16:02:39.000000 webvtt-py-0.5.0/webvtt_py.egg-info/top_level.txt
+drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-30 13:40:01.226490 webvtt-py-0.5.1/
+-rw-r--r--   0 amendez    (501) staff       (20)     1072 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/LICENSE
+-rw-r--r--   0 amendez    (501) staff       (20)      100 2021-01-27 19:12:00.000000 webvtt-py-0.5.1/MANIFEST.in
+-rw-r--r--   0 amendez    (501) staff       (20)     4146 2024-05-30 13:40:01.226897 webvtt-py-0.5.1/PKG-INFO
+-rw-r--r--   0 amendez    (501) staff       (20)     2407 2024-05-15 15:38:13.000000 webvtt-py-0.5.1/README.rst
+-rw-r--r--   0 amendez    (501) staff       (20)      605 2024-05-30 13:40:01.229045 webvtt-py-0.5.1/setup.cfg
+-rw-r--r--   0 amendez    (501) staff       (20)     1576 2024-05-15 15:38:26.000000 webvtt-py-0.5.1/setup.py
+drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-30 13:40:01.162787 webvtt-py-0.5.1/tests/
+-rw-r--r--   0 amendez    (501) staff       (20)        0 2021-01-27 19:12:00.000000 webvtt-py-0.5.1/tests/__init__.py
+drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-30 13:40:01.208316 webvtt-py-0.5.1/tests/samples/
+-rw-r--r--   0 amendez    (501) staff       (20)      197 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/captions_with_bom.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      395 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/comments.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      234 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/cue_tags.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)        0 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/empty.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      327 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)        9 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_format.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)        1 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_format1.srt
+-rw-r--r--   0 amendez    (501) staff       (20)        9 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_format2.srt
+-rw-r--r--   0 amendez    (501) staff       (20)       11 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_format3.srt
+-rw-r--r--   0 amendez    (501) staff       (20)       39 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_format4.srt
+-rw-r--r--   0 amendez    (501) staff       (20)      203 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_timeframe.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)      243 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_timeframe.srt
+-rw-r--r--   0 amendez    (501) staff       (20)      335 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_timeframe.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      177 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/invalid_timeframe_in_cue_text.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      128 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/metadata_headers.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      190 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/metadata_headers_multiline.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      187 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_caption_text.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)      228 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_caption_text.srt
+-rw-r--r--   0 amendez    (501) staff       (20)      225 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_caption_text.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      179 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_timeframe.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)      213 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_timeframe.srt
+-rw-r--r--   0 amendez    (501) staff       (20)      305 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/missing_timeframe.vtt
+-rwxr-xr-x   0 amendez    (501) staff       (20)   120238 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/netflix_chicas_del_cable.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)        6 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/no_captions.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)       47 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/one_caption.srt
+-rw-r--r--   0 amendez    (501) staff       (20)       53 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/one_caption.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      237 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/sample.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)      243 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/sample.srt
+-rw-r--r--   0 amendez    (501) staff       (20)      765 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/sample.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      205 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/styles.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      343 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/styles_with_comments.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      114 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/two_captions.sbv
+-rw-r--r--   0 amendez    (501) staff       (20)      305 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/using_identifiers.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)      649 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/samples/youtube_dl.vtt
+-rw-r--r--   0 amendez    (501) staff       (20)     6067 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_cli.py
+-rw-r--r--   0 amendez    (501) staff       (20)    15171 2024-05-27 10:16:26.000000 webvtt-py-0.5.1/tests/test_models.py
+-rw-r--r--   0 amendez    (501) staff       (20)     4071 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_sbv.py
+-rw-r--r--   0 amendez    (501) staff       (20)    10159 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_segmenter.py
+-rw-r--r--   0 amendez    (501) staff       (20)     4510 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_srt.py
+-rw-r--r--   0 amendez    (501) staff       (20)      875 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_utils.py
+-rw-r--r--   0 amendez    (501) staff       (20)    16025 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/tests/test_vtt.py
+-rw-r--r--   0 amendez    (501) staff       (20)    46224 2024-05-30 13:18:13.000000 webvtt-py-0.5.1/tests/test_webvtt.py
+drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-30 13:40:01.221130 webvtt-py-0.5.1/webvtt/
+-rw-r--r--   0 amendez    (501) staff       (20)      461 2024-05-30 13:20:41.000000 webvtt-py-0.5.1/webvtt/__init__.py
+-rw-r--r--   0 amendez    (501) staff       (20)     1338 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/webvtt/cli.py
+-rw-r--r--   0 amendez    (501) staff       (20)      279 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/webvtt/errors.py
+-rw-r--r--   0 amendez    (501) staff       (20)     7322 2024-05-27 10:16:26.000000 webvtt-py-0.5.1/webvtt/models.py
+-rw-r--r--   0 amendez    (501) staff       (20)     2917 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/webvtt/sbv.py
+-rw-r--r--   0 amendez    (501) staff       (20)     3669 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/webvtt/segmenter.py
+-rw-r--r--   0 amendez    (501) staff       (20)     3735 2024-05-17 15:08:24.000000 webvtt-py-0.5.1/webvtt/srt.py
+-rw-r--r--   0 amendez    (501) staff       (20)     2901 2024-05-14 10:27:10.000000 webvtt-py-0.5.1/webvtt/utils.py
+-rw-r--r--   0 amendez    (501) staff       (20)    10878 2024-05-30 09:26:27.000000 webvtt-py-0.5.1/webvtt/vtt.py
+-rw-r--r--   0 amendez    (501) staff       (20)    11962 2024-05-30 13:18:13.000000 webvtt-py-0.5.1/webvtt/webvtt.py
+drwxr-xr-x   0 amendez    (501) staff       (20)        0 2024-05-30 13:40:01.225715 webvtt-py-0.5.1/webvtt_py.egg-info/
+-rw-r--r--   0 amendez    (501) staff       (20)     4146 2024-05-30 13:40:01.000000 webvtt-py-0.5.1/webvtt_py.egg-info/PKG-INFO
+-rw-r--r--   0 amendez    (501) staff       (20)     1693 2024-05-30 13:40:01.000000 webvtt-py-0.5.1/webvtt_py.egg-info/SOURCES.txt
+-rw-r--r--   0 amendez    (501) staff       (20)        1 2024-05-30 13:40:01.000000 webvtt-py-0.5.1/webvtt_py.egg-info/dependency_links.txt
+-rw-r--r--   0 amendez    (501) staff       (20)       44 2024-05-30 13:40:01.000000 webvtt-py-0.5.1/webvtt_py.egg-info/entry_points.txt
+-rw-r--r--   0 amendez    (501) staff       (20)        7 2024-05-30 13:40:01.000000 webvtt-py-0.5.1/webvtt_py.egg-info/top_level.txt
```

### Comparing `webvtt-py-0.5.0/LICENSE` & `webvtt-py-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/PKG-INFO` & `webvtt-py-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webvtt-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: WebVTT reader, writer and segmenter
 Home-page: https://github.com/glut23/webvtt-py
 Author: Alejandro Mendez
 Author-email: amendez23@gmail.com
 License: MIT
 Description: webvtt-py
         =========
```

### Comparing `webvtt-py-0.5.0/README.rst` & `webvtt-py-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/setup.cfg` & `webvtt-py-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/setup.py` & `webvtt-py-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/samples/netflix_chicas_del_cable.vtt` & `webvtt-py-0.5.1/tests/samples/netflix_chicas_del_cable.vtt`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/samples/sample.vtt` & `webvtt-py-0.5.1/tests/samples/sample.vtt`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/samples/youtube_dl.vtt` & `webvtt-py-0.5.1/tests/samples/youtube_dl.vtt`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_cli.py` & `webvtt-py-0.5.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_models.py` & `webvtt-py-0.5.1/tests/test_models.py`

 * *Files 13% similar despite different names*

```diff
@@ -399,14 +399,58 @@
     def test_malformed_start_timestamp(self):
         self.assertRaises(
             MalformedCaptionError,
             Caption,
             '01:00'
             )
 
+    def test_voice_span(self):
+        caption = Caption(text='<v Homer Simpson>Hello there!</v>')
+        self.assertEqual(caption.text, 'Hello there!')
+        self.assertEqual(caption.raw_text, '<v Homer Simpson>Hello there!</v>')
+        self.assertEqual(caption.voice, 'Homer Simpson')
+
+    def test_voice_span_with_classes(self):
+        caption = Caption(text='<v.quiet.slow Lisa Simpson>I am Lisa</v>')
+        self.assertEqual(caption.text, 'I am Lisa')
+        self.assertEqual(
+            caption.raw_text,
+            '<v.quiet.slow Lisa Simpson>I am Lisa</v>'
+            )
+        self.assertEqual(caption.voice, 'Lisa Simpson')
+
+    def test_voice_span_is_invalid(self):
+        caption = Caption(text='<v Lets eat donuts')
+        self.assertEqual(caption.text, '<v Lets eat donuts')
+        self.assertEqual(
+            caption.raw_text,
+            '<v Lets eat donuts'
+            )
+        self.assertIsNone(caption.voice)
+
+    def test_voice_span_injected(self):
+        caption = Caption(text='This is a test')
+        self.assertEqual(caption.text, 'This is a test')
+        self.assertEqual(caption.raw_text, 'This is a test')
+        self.assertIsNone(caption.voice)
+        caption.text = '<v Homer Simpson>I like tests</v>'
+        self.assertEqual(caption.text, 'I like tests')
+        self.assertEqual(caption.raw_text, '<v Homer Simpson>I like tests</v>')
+        self.assertEqual(caption.voice, 'Homer Simpson')
+
+    def test_voice_span_removed(self):
+        caption = Caption(text='<v Homer Simpson>I like tests</v>')
+        self.assertEqual(caption.text, 'I like tests')
+        self.assertEqual(caption.raw_text, '<v Homer Simpson>I like tests</v>')
+        self.assertEqual(caption.voice, 'Homer Simpson')
+        caption.text = 'This is a test'
+        self.assertEqual(caption.text, 'This is a test')
+        self.assertEqual(caption.raw_text, 'This is a test')
+        self.assertIsNone(caption.voice)
+
 
 class TestStyle(unittest.TestCase):
 
     def test_instantiation(self):
         style = Style(text='::cue(b) {\ncolor: peachpuff;\n}')
         self.assertEqual(style.text, '::cue(b) {\ncolor: peachpuff;\n}')
         self.assertListEqual(
```

### Comparing `webvtt-py-0.5.0/tests/test_sbv.py` & `webvtt-py-0.5.1/tests/test_sbv.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_segmenter.py` & `webvtt-py-0.5.1/tests/test_segmenter.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_srt.py` & `webvtt-py-0.5.1/tests/test_srt.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_utils.py` & `webvtt-py-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_vtt.py` & `webvtt-py-0.5.1/tests/test_vtt.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/tests/test_webvtt.py` & `webvtt-py-0.5.1/tests/test_webvtt.py`

 * *Files 16% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
                 00:00:00.500 --> 00:00:07.000
                 Caption text #1
 
                 00:00:07.000 --> 00:00:11.890
                 New caption text line1
                 New caption text line2
-            ''').strip()
+            ''').strip() + '\n'
             )
 
     def test_write_captions_in_srt(self):
         out = io.StringIO()
         vtt = webvtt.read(PATH_TO_SAMPLES / 'one_caption.vtt')
         new_caption = Caption(start='00:00:07.000',
                               end='00:00:11.890',
@@ -104,14 +104,38 @@
                 2
                 00:00:07,000 --> 00:00:11,890
                 New caption text line1
                 New caption text line2
             ''').strip()
             )
 
+    def test_write_captions_in_srt_no_cuetags(self):
+        """https://github.com/glut23/webvtt-py/issues/56"""
+        out = io.StringIO()
+        vtt = webvtt.read(PATH_TO_SAMPLES / 'cue_tags.vtt')
+        vtt.write(out, format='srt')
+
+        out.seek(0)
+        self.assertEqual(
+            out.read(),
+            textwrap.dedent('''
+            1
+            00:00:16,500 --> 00:00:18,500
+            When the moon hits your eye
+
+            2
+            00:00:18,500 --> 00:00:20,500
+            Like a big-a pizza pie
+
+            3
+            00:00:20,500 --> 00:00:21,500
+            That's amore
+            ''').strip()
+            )
+
     def test_write_captions_in_unsupported_format(self):
         self.assertRaises(
             ValueError,
             webvtt.WebVTT().write,
             io.StringIO(),
             format='ttt'
             )
@@ -139,15 +163,15 @@
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
 
                     00:00:07.000 --> 00:00:11.890
                     New caption text line1
                     New caption text line2
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_srt_conversion(self):
         with tempfile.TemporaryDirectory() as td:
             with open(pathlib.Path(td) / 'one_caption.srt', 'w') as f:
                 f.write((PATH_TO_SAMPLES / 'one_caption.srt').read_text())
 
@@ -161,15 +185,15 @@
             self.assertEqual(
                 (pathlib.Path(td) / 'one_caption.vtt').read_text(),
                 textwrap.dedent('''
                     WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_sbv_conversion(self):
         with tempfile.TemporaryDirectory() as td:
             with open(pathlib.Path(td) / 'two_captions.sbv', 'w') as f:
                 f.write(
                     (PATH_TO_SAMPLES / 'two_captions.sbv').read_text()
@@ -189,15 +213,15 @@
 
                     00:00:00.378 --> 00:00:11.378
                     Caption text #1
 
                     00:00:11.378 --> 00:00:12.305
                     Caption text #2 (line 1)
                     Caption text #2 (line 2)
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_to_other_location(self):
         with tempfile.TemporaryDirectory() as td:
             webvtt.read(
                 PATH_TO_SAMPLES / 'one_caption.vtt'
                 ).save(td)
@@ -228,18 +252,37 @@
 
             self.assertTrue(
                 os.path.exists(pathlib.Path(td) / 'one_caption_new.vtt')
                 )
 
     def test_from_buffer(self):
         with open(PATH_TO_SAMPLES / 'sample.vtt', 'r', encoding='utf-8') as f:
-            self.assertIsInstance(
-                webvtt.from_buffer(f).captions,
-                list
-                )
+            vtt = webvtt.from_buffer(f)
+            self.assertEqual(len(vtt), 16)
+            self.assertEqual(
+                str(vtt),
+                textwrap.dedent('''
+                    00:00:00.500 00:00:07.000 Caption text #1
+                    00:00:07.000 00:00:11.890 Caption text #2
+                    00:00:11.890 00:00:16.320 Caption text #3
+                    00:00:16.320 00:00:21.580 Caption text #4
+                    00:00:21.580 00:00:23.880 Caption text #5
+                    00:00:23.880 00:00:27.280 Caption text #6
+                    00:00:27.280 00:00:30.280 Caption text #7
+                    00:00:30.280 00:00:36.510 Caption text #8
+                    00:00:36.510 00:00:38.870 Caption text #9
+                    00:00:38.870 00:00:45.000 Caption text #10
+                    00:00:45.000 00:00:47.000 Caption text #11
+                    00:00:47.000 00:00:50.970 Caption text #12
+                    00:00:50.970 00:00:54.440 Caption text #13
+                    00:00:54.440 00:00:58.600 Caption text #14
+                    00:00:58.600 00:01:01.350 Caption text #15
+                    00:01:01.350 00:01:04.300 Caption text #16
+                    '''
+                    ).strip())
 
     def test_deprecated_read_buffer(self):
         with open(PATH_TO_SAMPLES / 'sample.vtt', 'r', encoding='utf-8') as f:
             with warnings.catch_warnings(record=True) as warns:
                 warnings.simplefilter('always')
                 vtt = webvtt.read_buffer(f)
 
@@ -283,14 +326,142 @@
     def test_read_malformed_buffer(self):
         malformed_payloads = ['', 'MOCK MALFORMED CONTENT']
         for payload in malformed_payloads:
             buffer = io.StringIO(payload)
             with self.assertRaises(MalformedFileError):
                 webvtt.from_buffer(buffer)
 
+    def test_read_buffer_for_vtt_content(self):
+        buffer = io.StringIO(textwrap.dedent('''\
+            WEBVTT\r
+            \r
+            00:00:00.500 --> 00:00:07.000\r
+            Caption text #1\r
+            \r
+            00:00:07.000 --> 00:00:11.890\r
+            Caption text #2\r
+            \r
+            00:00:11.890 --> 00:00:16.320\r
+            Caption text #3\r
+            ''')
+            )
+        vtt = webvtt.from_buffer(buffer, format='vtt')
+        self.assertEqual(len(vtt), 3)
+
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.500 00:00:07.000 Caption text #1'
+            )
+        self.assertEqual(
+            str(vtt[1]),
+            '00:00:07.000 00:00:11.890 Caption text #2'
+            )
+        self.assertEqual(
+            str(vtt[2]),
+            '00:00:11.890 00:00:16.320 Caption text #3'
+            )
+
+    def test_read_buffer_for_srt_content(self):
+        buffer = io.StringIO(textwrap.dedent('''\
+            0\r
+            00:00:00,500 --> 00:00:07,000\r
+            Caption text #1\r
+            \r
+            1\r
+            00:00:07,000 --> 00:00:11,890\r
+            Caption text #2\r
+            \r
+            2\r
+            00:00:11,890 --> 00:00:16,320\r
+            Caption text #3\r
+            ''')
+            )
+        vtt = webvtt.from_buffer(buffer, format='srt')
+        self.assertEqual(len(vtt), 3)
+
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.500 00:00:07.000 Caption text #1'
+            )
+        self.assertEqual(
+            str(vtt[1]),
+            '00:00:07.000 00:00:11.890 Caption text #2'
+            )
+        self.assertEqual(
+            str(vtt[2]),
+            '00:00:11.890 00:00:16.320 Caption text #3'
+            )
+
+    def test_read_buffer_for_sbv_content(self):
+        buffer = io.StringIO(textwrap.dedent('''\
+            00:00:00.500,00:00:07.000\r
+            Caption text #1\r
+            \r
+            00:00:07.000,00:00:11.890\r
+            Caption text #2\r
+            \r
+            00:00:11.890,00:00:16.320\r
+            Caption text #3\r
+            ''')
+            )
+        vtt = webvtt.from_buffer(buffer, format='sbv')
+        self.assertEqual(len(vtt), 3)
+
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.500 00:00:07.000 Caption text #1'
+            )
+        self.assertEqual(
+            str(vtt[1]),
+            '00:00:07.000 00:00:11.890 Caption text #2'
+            )
+        self.assertEqual(
+            str(vtt[2]),
+            '00:00:11.890 00:00:16.320 Caption text #3'
+            )
+
+    def test_read_buffer_unsupported_format(self):
+        self.assertRaises(
+            ValueError,
+            webvtt.from_buffer,
+            io.StringIO(),
+            format='ttt'
+            )
+
+    def test_read_bytesio_buffer_for_srt_content(self):
+        buffer = io.BytesIO(textwrap.dedent('''\
+            0\r
+            00:00:00,500 --> 00:00:07,000\r
+            Caption text #1\r
+            \r
+            1\r
+            00:00:07,000 --> 00:00:11,890\r
+            Caption text #2\r
+            \r
+            2\r
+            00:00:11,890 --> 00:00:16,320\r
+            Caption text #3\r
+            ''').encode('utf-8')
+            )
+        vtt = webvtt.from_buffer(buffer, format='srt')
+        self.assertEqual(len(vtt), 3)
+
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.500 00:00:07.000 Caption text #1'
+            )
+        self.assertEqual(
+            str(vtt[1]),
+            '00:00:07.000 00:00:11.890 Caption text #2'
+            )
+        self.assertEqual(
+            str(vtt[2]),
+            '00:00:11.890 00:00:16.320 Caption text #3'
+            )
+
     def test_captions(self):
         captions = webvtt.read(PATH_TO_SAMPLES / 'sample.vtt').captions
         self.assertIsInstance(
             captions,
             list
             )
         self.assertEqual(len(captions), 16)
@@ -425,15 +596,15 @@
                     00:00:00.500 --> 00:00:07.000
                     Caption test line 1
                     Caption test line 2
 
                     00:00:08.000 --> 00:00:15.000
                     Caption test line 3
                     Caption test line 4
-                    """).strip()
+                    """).strip() + '\n'
             )
 
     def test_repr(self):
         test_file = PATH_TO_SAMPLES / 'sample.vtt'
         self.assertEqual(
             repr(webvtt.read(test_file)),
             f"<WebVTT file='{test_file}' encoding='utf-8'>"
@@ -832,14 +1003,69 @@
     def test_can_parse_youtube_dl_files(self):
         vtt = webvtt.read(PATH_TO_SAMPLES / 'youtube_dl.vtt')
         self.assertEqual(
             "this will happen is I'm telling\n ",
             vtt.captions[2].text
             )
 
+    def test_parse_voice_spans(self):
+        vtt = webvtt.from_string(textwrap.dedent("""
+            WEBVTT
+
+            00:00:00.000 --> 00:00:00.800
+            <v.quiet.slow Lisa Simpson>Knock knock</v>
+
+            00:00:02.100 --> 00:00:06.500
+            <v Homer Simpson>Who's there?</v>
+
+            00:00:10.530 --> 00:00:11.090
+            <v.loud Lisa Simpson>Atish</v>
+            """).strip()
+            )
+        self.assertEqual(len(vtt), 3)
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.000 00:00:00.800 Knock knock'
+            )
+        self.assertEqual(
+            vtt[0].voice,
+            'Lisa Simpson'
+            )
+        self.assertEqual(
+            str(vtt[1]),
+            '00:00:02.100 00:00:06.500 Who\'s there?'
+            )
+        self.assertEqual(
+            vtt[1].voice,
+            'Homer Simpson'
+            )
+        self.assertEqual(
+            str(vtt[2]),
+            '00:00:10.530 00:00:11.090 Atish'
+            )
+        self.assertEqual(
+            vtt[2].voice,
+            'Lisa Simpson'
+            )
+
+    def test_parse_caption_not_a_voice_span(self):
+        vtt = webvtt.from_string(textwrap.dedent("""
+            WEBVTT
+
+            00:00:00.000 --> 00:00:00.800
+            <v Not an actual voice span here
+            """).strip()
+            )
+        self.assertEqual(len(vtt), 1)
+        self.assertEqual(
+            str(vtt[0]),
+            '00:00:00.000 00:00:00.800 <v Not an actual voice span here'
+            )
+        self.assertIsNone(vtt[0].voice)
+
 
 class TestParseSRT(unittest.TestCase):
 
     def test_parse_empty_file(self):
         self.assertRaises(
             webvtt.errors.MalformedFileError,
             webvtt.from_srt,
@@ -1005,15 +1231,15 @@
             self.assertEqual(
                 f.read(),
                 textwrap.dedent(f'''
                     {CODEC_BOMS['utf-8'].decode()}WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_file_with_bom_keeps_bom(self):
         with tempfile.NamedTemporaryFile('r', suffix='.vtt') as f:
             webvtt.read(
                 PATH_TO_SAMPLES / 'captions_with_bom.vtt'
             ).save(f.name)
@@ -1029,15 +1255,15 @@
                     Caption text #2
 
                     00:00:11.890 --> 00:00:16.320
                     Caption text #3
 
                     00:00:16.320 --> 00:00:21.580
                     Caption text #4
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_file_with_bom_removes_bom_if_requested(self):
         with tempfile.NamedTemporaryFile('r', suffix='.vtt') as f:
             webvtt.read(
                 PATH_TO_SAMPLES / 'captions_with_bom.vtt'
             ).save(f.name, add_bom=False)
@@ -1053,15 +1279,15 @@
                     Caption text #2
 
                     00:00:11.890 --> 00:00:16.320
                     Caption text #3
 
                     00:00:16.320 --> 00:00:21.580
                     Caption text #4
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_file_with_encoding(self):
         with tempfile.NamedTemporaryFile('rb', suffix='.vtt') as f:
             webvtt.read(
                 PATH_TO_SAMPLES / 'one_caption.vtt'
             ).save(f.name,
@@ -1070,15 +1296,15 @@
             self.assertEqual(
                 f.read().decode('utf-32-le'),
                 textwrap.dedent('''
                     WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_file_with_encoding_and_bom(self):
         with tempfile.NamedTemporaryFile('rb', suffix='.vtt') as f:
             webvtt.read(
                 PATH_TO_SAMPLES / 'one_caption.vtt'
             ).save(f.name,
@@ -1088,15 +1314,15 @@
             self.assertEqual(
                 f.read().decode('utf-32-le'),
                 textwrap.dedent(f'''
                     {CODEC_BOMS['utf-32-le'].decode('utf-32-le')}WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_new_file_utf_8_default_encoding_no_bom(self):
         with tempfile.NamedTemporaryFile('r', suffix='.vtt') as f:
             vtt = webvtt.WebVTT()
             vtt.captions.append(
                 Caption(start='00:00:00.500',
@@ -1109,15 +1335,15 @@
             self.assertEqual(
                 f.read(),
                 textwrap.dedent(f'''
                     WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_save_new_file_utf_8_default_encoding_with_bom(self):
         with tempfile.NamedTemporaryFile('r', suffix='.vtt') as f:
             vtt = webvtt.WebVTT()
             vtt.captions.append(
                 Caption(start='00:00:00.500',
@@ -1132,15 +1358,15 @@
             self.assertEqual(
                 f.read(),
                 textwrap.dedent(f'''
                     {CODEC_BOMS['utf-8'].decode()}WEBVTT
 
                     00:00:00.500 --> 00:00:07.000
                     Caption text #1
-                    ''').strip()
+                    ''').strip() + '\n'
                 )
 
     def test_iter_slice(self):
         vtt = webvtt.read(
                 PATH_TO_SAMPLES / 'sample.vtt'
                 )
         slice_of_captions = vtt.iter_slice(start='00:00:11.000',
```

### Comparing `webvtt-py-0.5.0/webvtt/cli.py` & `webvtt-py-0.5.1/webvtt/cli.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/webvtt/models.py` & `webvtt-py-0.5.1/webvtt/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
                 )
 
 
 class Caption:
     """Representation of a caption."""
 
     CUE_TEXT_TAGS = re.compile('<.*?>')
+    VOICE_SPAN_PATTERN = re.compile(r'<v(?:\.\w+)*\s+([^>]+)>')
 
     def __init__(self,
                  start: typing.Optional[str] = None,
                  end: typing.Optional[str] = None,
                  text: typing.Optional[typing.Union[str,
                                                     typing.Sequence[str]
                                                     ]] = None,
@@ -200,14 +201,24 @@
         if not isinstance(value, str):
             raise AttributeError(
                 f'String value expected but received {value}.'
                 )
 
         self.lines = value.splitlines()
 
+    @property
+    def voice(self) -> typing.Optional[str]:
+        """Return the voice span if present."""
+        if self.lines and self.lines[0].startswith('<v'):
+            match = re.match(self.VOICE_SPAN_PATTERN, self.lines[0])
+            if match:
+                return match.group(1)
+
+        return None
+
 
 class Style:
     """Representation of a style."""
 
     def __init__(self, text: typing.Union[str, typing.List[str]]):
         """Initialize.
```

### Comparing `webvtt-py-0.5.0/webvtt/sbv.py` & `webvtt-py-0.5.1/webvtt/sbv.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/webvtt/segmenter.py` & `webvtt-py-0.5.1/webvtt/segmenter.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/webvtt/srt.py` & `webvtt-py-0.5.1/webvtt/srt.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,11 +138,11 @@
     output = []
     for index, caption in enumerate(captions, start=1):
         output.extend([
             f'{index}',
             '{} --> {}'.format(*map(lambda x: x.replace('.', ','),
                                     (caption.start, caption.end))
                                ),
-            *caption.lines,
+            *caption.text.splitlines(),
             ''
             ])
     f.write('\n'.join(output).rstrip())
```

### Comparing `webvtt-py-0.5.0/webvtt/utils.py` & `webvtt-py-0.5.1/webvtt/utils.py`

 * *Files identical despite different names*

### Comparing `webvtt-py-0.5.0/webvtt/vtt.py` & `webvtt-py-0.5.1/webvtt/vtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,14 +387,17 @@
         for comment in caption.comments:
             output.extend([
                 '',
                 *WebVTTCommentBlock.format_lines(comment)
             ])
         output.extend(WebVTTCueBlock.format_lines(caption))
 
+    if not footer_comments:
+        output.append('')
+
     for comment in footer_comments:
         output.extend([
             '',
             *WebVTTCommentBlock.format_lines(comment)
         ])
 
     return '\n'.join(output)
```

### Comparing `webvtt-py-0.5.0/webvtt/webvtt.py` & `webvtt-py-0.5.1/webvtt/webvtt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """WebVTT module."""
 
 import os
+import io
 import typing
 import warnings
+from functools import partial
 
 from . import vtt, utils
 from . import srt
 from . import sbv
 from .models import Caption, Style, Timestamp
 from .errors import MissingFilenameError
 
@@ -111,34 +113,53 @@
             DeprecationWarning
             )
         return cls.from_buffer(buffer)
 
     @classmethod
     def from_buffer(
             cls,
-            buffer: typing.Iterator[str]
+            buffer: typing.Union[typing.Iterable[str], io.BytesIO],
+            format: str = 'vtt'
             ) -> 'WebVTT':
         """
         Read WebVTT captions from a file-like object.
 
         Such file-like object may be the return of an io.open call,
         io.StringIO object, tempfile.TemporaryFile object, etc.
 
         :param buffer: the file-like object to read captions from
+        :param format: the format of the data (vtt, srt or sbv)
         :returns: a `WebVTT` instance
         """
-        output = vtt.parse(cls._get_lines(buffer))
+        if isinstance(buffer, io.BytesIO):
+            buffer = (line.decode('utf-8') for line in buffer)
 
-        return cls(
-            file=getattr(buffer, 'name', None),
-            captions=output.captions,
-            styles=output.styles,
-            header_comments=output.header_comments,
-            footer_comments=output.footer_comments
-            )
+        _cls = partial(cls, file=getattr(buffer, 'name', None))
+
+        if format == 'vtt':
+            output = vtt.parse(cls._get_lines(buffer))
+
+            return _cls(
+                captions=output.captions,
+                styles=output.styles,
+                header_comments=output.header_comments,
+                footer_comments=output.footer_comments
+                )
+
+        if format == 'srt':
+            return _cls(
+                captions=srt.parse(cls._get_lines(buffer))
+                )
+
+        if format == 'sbv':
+            return _cls(
+                captions=sbv.parse(cls._get_lines(buffer))
+                )
+
+        raise ValueError(f'Format {format} is not supported.')
 
     @classmethod
     def from_srt(
             cls,
             file: str,
             encoding: typing.Optional[str] = None
             ) -> 'WebVTT':
```

### Comparing `webvtt-py-0.5.0/webvtt_py.egg-info/PKG-INFO` & `webvtt-py-0.5.1/webvtt_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webvtt-py
-Version: 0.5.0
+Version: 0.5.1
 Summary: WebVTT reader, writer and segmenter
 Home-page: https://github.com/glut23/webvtt-py
 Author: Alejandro Mendez
 Author-email: amendez23@gmail.com
 License: MIT
 Description: webvtt-py
         =========
```

### Comparing `webvtt-py-0.5.0/webvtt_py.egg-info/SOURCES.txt` & `webvtt-py-0.5.1/webvtt_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

