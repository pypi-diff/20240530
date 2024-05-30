# Comparing `tmp/tikhub-1.0.9.tar.gz` & `tmp/tikhub-1.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.0.9.tar", last modified: Thu May 30 12:29:49 2024, max compression
+gzip compressed data, was "tikhub-1.10.0.tar", last modified: Thu May 30 12:34:50 2024, max compression
```

## Comparing `tikhub-1.0.9.tar` & `tikhub-1.10.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.791587 tikhub-1.0.9/
--rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.9/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:29:49.791587 tikhub-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.9/README.md
--rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 12:29:49.791587 tikhub-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-05-30 12:29:47.000000 tikhub-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.755823 tikhub-1.0.9/tikhub/
--rw-rw-rw-   0        0        0       67 2024-05-30 12:29:47.000000 tikhub-1.0.9/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.761823 tikhub-1.0.9/tikhub/api/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.9/tikhub/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.763327 tikhub-1.0.9/tikhub/api/v1/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.9/tikhub/api/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.764331 tikhub-1.0.9/tikhub/api/v1/endpoints/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.765335 tikhub-1.0.9/tikhub/api/v1/endpoints/captcha/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/captcha/__init__.py
--rw-rw-rw-   0        0        0      478 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/captcha/captcha_solver.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.766335 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.769334 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/__init__.py
--rw-rw-rw-   0        0        0    14139 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
--rw-rw-rw-   0        0        0    15959 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
--rw-rw-rw-   0        0        0    12565 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.770335 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/web/__init__.py
--rw-rw-rw-   0        0        0    31217 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.771335 tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.772335 tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/web/__init__.py
--rw-rw-rw-   0        0        0      961 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.773378 tikhub-1.0.9/tikhub/api/v1/endpoints/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tikhub/__init__.py
--rw-rw-rw-   0        0        0     3246 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.775064 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.777069 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/__init__.py
--rw-rw-rw-   0        0        0    13951 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
--rw-rw-rw-   0        0        0    22972 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.779068 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/web/__init__.py
--rw-rw-rw-   0        0        0    13858 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.780068 tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.781069 tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/web/__init__.py
--rw-rw-rw-   0        0        0     1834 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.781069 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.783067 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.783571 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.785576 tikhub-1.0.9/tikhub/api/v1/models/
--rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.0.9/tikhub/api/v1/models/APIResponseModel.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.9/tikhub/api/v1/models/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.0.9/tikhub/api/v1/models/douyin_web_models.py
--rw-rw-rw-   0        0        0     2428 2024-05-30 12:19:09.000000 tikhub-1.0.9/tikhub/client.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.789575 tikhub-1.0.9/tikhub/http_client/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.9/tikhub/http_client/__init__.py
--rw-rw-rw-   0        0        0    11320 2024-05-30 12:14:39.000000 tikhub-1.0.9/tikhub/http_client/api_client.py
--rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.0.9/tikhub/http_client/api_exceptions.py
--rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.0.9/tikhub/http_client/api_logger.py
--rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.0.9/tikhub/http_client/deprecated.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.790575 tikhub-1.0.9/tikhub/test/
--rw-rw-rw-   0        0        0        0 2024-05-30 12:29:47.000000 tikhub-1.0.9/tikhub/test/__init__.py
--rw-rw-rw-   0        0        0     1279 2024-05-30 12:16:42.000000 tikhub-1.0.9/tikhub/test/test.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:29:49.761823 tikhub-1.0.9/tikhub.egg-info/
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:29:49.000000 tikhub-1.0.9/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2021 2024-05-30 12:29:49.000000 tikhub-1.0.9/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:29:49.000000 tikhub-1.0.9/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 12:29:49.000000 tikhub-1.0.9/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 12:29:49.000000 tikhub-1.0.9/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.617829 tikhub-1.10.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.10.0/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.10.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3235 2024-05-30 12:34:50.616824 tikhub-1.10.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.10.0/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.10.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:34:50.617829 tikhub-1.10.0/setup.cfg
+-rw-rw-rw-   0        0        0      976 2024-05-30 12:34:35.000000 tikhub-1.10.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.584120 tikhub-1.10.0/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-30 12:34:35.000000 tikhub-1.10.0/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.588120 tikhub-1.10.0/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.0/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.589149 tikhub-1.10.0/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.0/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.589149 tikhub-1.10.0/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.591116 tikhub-1.10.0/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      478 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.591116 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.594486 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14139 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15959 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12565 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.595494 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31217 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.597487 tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.598502 tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.600494 tikhub-1.10.0/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3246 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.600494 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.603069 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13951 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22972 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.604164 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    13858 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.605152 tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.606151 tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1834 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.606151 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.607150 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.609149 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.610149 tikhub-1.10.0/tikhub/api/v1/models/
+-rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.10.0/tikhub/api/v1/models/APIResponseModel.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.10.0/tikhub/api/v1/models/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.10.0/tikhub/api/v1/models/douyin_web_models.py
+-rw-rw-rw-   0        0        0     2428 2024-05-30 12:19:09.000000 tikhub-1.10.0/tikhub/client.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.614818 tikhub-1.10.0/tikhub/http_client/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.10.0/tikhub/http_client/__init__.py
+-rw-rw-rw-   0        0        0    11320 2024-05-30 12:14:39.000000 tikhub-1.10.0/tikhub/http_client/api_client.py
+-rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.10.0/tikhub/http_client/api_exceptions.py
+-rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.10.0/tikhub/http_client/api_logger.py
+-rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.10.0/tikhub/http_client/deprecated.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.616824 tikhub-1.10.0/tikhub/test/
+-rw-rw-rw-   0        0        0        0 2024-05-30 12:29:47.000000 tikhub-1.10.0/tikhub/test/__init__.py
+-rw-rw-rw-   0        0        0     1279 2024-05-30 12:16:42.000000 tikhub-1.10.0/tikhub/test/test.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:34:50.587129 tikhub-1.10.0/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     3235 2024-05-30 12:34:50.000000 tikhub-1.10.0/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2021 2024-05-30 12:34:50.000000 tikhub-1.10.0/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:34:50.000000 tikhub-1.10.0/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 12:34:50.000000 tikhub-1.10.0/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:34:50.000000 tikhub-1.10.0/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.0.9/LICENSE` & `tikhub-1.10.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/PKG-INFO` & `tikhub-1.10.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.9
+Version: 1.10.0
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.9/README.md` & `tikhub-1.10.0/README.md`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/setup.py` & `tikhub-1.10.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name="tikhub",
-    version="1.0.9",
+    version="1.10.0",
     author="TikHub.io",
     author_email="tikhub.io@proton.me",
     description="A Python SDK for TikHub RESTful API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TikHubIO/TikHub-API-SDK-Python",
     packages=find_packages(),
```

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/douyin/web/douyin_web.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/douyin/web/douyin_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/instagram/web/instagram_web.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/instagram/web/instagram_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/tikhub/tikhub_user.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/tikhub/tikhub_user.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/weibo/web/weibo_web.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/weibo/web/weibo_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py` & `tikhub-1.10.0/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/models/APIResponseModel.py` & `tikhub-1.10.0/tikhub/api/v1/models/APIResponseModel.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/api/v1/models/douyin_web_models.py` & `tikhub-1.10.0/tikhub/api/v1/models/douyin_web_models.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/client.py` & `tikhub-1.10.0/tikhub/client.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/http_client/api_client.py` & `tikhub-1.10.0/tikhub/http_client/api_client.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/http_client/api_exceptions.py` & `tikhub-1.10.0/tikhub/http_client/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/http_client/api_logger.py` & `tikhub-1.10.0/tikhub/http_client/api_logger.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub/test/test.py` & `tikhub-1.10.0/tikhub/test/test.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.9/tikhub.egg-info/PKG-INFO` & `tikhub-1.10.0/tikhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.9
+Version: 1.10.0
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.9/tikhub.egg-info/SOURCES.txt` & `tikhub-1.10.0/tikhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

