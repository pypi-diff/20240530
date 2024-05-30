# Comparing `tmp/tikhub-1.0.5.tar.gz` & `tmp/tikhub-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.0.5.tar", last modified: Thu May 30 12:04:54 2024, max compression
+gzip compressed data, was "tikhub-1.0.6.tar", last modified: Thu May 30 12:10:50 2024, max compression
```

## Comparing `tikhub-1.0.5.tar` & `tikhub-1.0.6.tar`

### file list

```diff
@@ -1,66 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.481435 tikhub-1.0.5/
--rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.5/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:04:54.480442 tikhub-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.5/README.md
--rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 12:04:54.481435 tikhub-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-05-30 12:04:34.000000 tikhub-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.458077 tikhub-1.0.5/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.5/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.462072 tikhub-1.0.5/tikhub/api/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.463072 tikhub-1.0.5/tikhub/api/v1/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.463665 tikhub-1.0.5/tikhub/api/v1/endpoints/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.464750 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/captcha_solver.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.464750 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.467748 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/__init__.py
--rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
--rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
--rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.468751 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/__init__.py
--rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.468751 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.469741 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/__init__.py
--rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.471747 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/__init__.py
--rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.471747 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.474366 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/__init__.py
--rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
--rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.475365 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/__init__.py
--rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.476435 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.477440 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/__init__.py
--rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.477440 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.478436 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.480442 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
--rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.5/tikhub/sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.462072 tikhub-1.0.5/tikhub.egg-info/
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1691 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.695263 tikhub-1.0.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:10:50.694263 tikhub-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.6/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:10:50.695263 tikhub-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-30 12:10:47.000000 tikhub-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.659288 tikhub-1.0.6/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.6/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.664430 tikhub-1.0.6/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.665430 tikhub-1.0.6/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.665430 tikhub-1.0.6/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.667430 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.668018 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.671023 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.672056 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.673560 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.674565 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.676569 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.677571 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.679570 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.680569 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.681581 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.682570 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.683569 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.685753 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.686753 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.688753 tikhub-1.0.6/tikhub/api/v1/models/
+-rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.0.6/tikhub/api/v1/models/APIResponseModel.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.6/tikhub/api/v1/models/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.0.6/tikhub/api/v1/models/douyin_web_models.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.693258 tikhub-1.0.6/tikhub/client/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/client/__init__.py
+-rw-rw-rw-   0        0        0    11300 2024-05-25 02:04:46.000000 tikhub-1.0.6/tikhub/client/api_client.py
+-rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.0.6/tikhub/client/api_exceptions.py
+-rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.0.6/tikhub/client/api_logger.py
+-rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.0.6/tikhub/client/deprecated.py
+-rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.6/tikhub/sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.663287 tikhub-1.0.6/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1949 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.0.5/LICENSE` & `tikhub-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/PKG-INFO` & `tikhub-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.5/README.md` & `tikhub-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/setup.py` & `tikhub-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name="tikhub",
-    version="1.0.5",
+    version="1.0.6",
     author="TikHub.io",
     author_email="tikhub.io@proton.me",
     description="A Python SDK for TikHub RESTful API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TikHubIO/TikHub-API-SDK-Python",
     packages=find_packages(),
```

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/douyin_web.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/douyin_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/instagram_web.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/instagram_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/tikhub_user.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/tikhub_user.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/weibo_web.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/weibo_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py` & `tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub/sdk.py` & `tikhub-1.0.6/tikhub/sdk.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.5/tikhub.egg-info/PKG-INFO` & `tikhub-1.0.6/tikhub.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.5
+Version: 1.0.6
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.5/tikhub.egg-info/SOURCES.txt` & `tikhub-1.0.6/tikhub.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -36,8 +36,16 @@
 tikhub/api/v1/endpoints/weibo/__init__.py
 tikhub/api/v1/endpoints/weibo/web/__init__.py
 tikhub/api/v1/endpoints/weibo/web/weibo_web.py
 tikhub/api/v1/endpoints/xiaohongshu/__init__.py
 tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
 tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
 tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
-tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+tikhub/api/v1/models/APIResponseModel.py
+tikhub/api/v1/models/__init__.py
+tikhub/api/v1/models/douyin_web_models.py
+tikhub/client/__init__.py
+tikhub/client/api_client.py
+tikhub/client/api_exceptions.py
+tikhub/client/api_logger.py
+tikhub/client/deprecated.py
```

