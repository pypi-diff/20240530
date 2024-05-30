# Comparing `tmp/tikhub-1.0.6.tar.gz` & `tmp/tikhub-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.0.6.tar", last modified: Thu May 30 12:10:50 2024, max compression
+gzip compressed data, was "tikhub-1.0.7.tar", last modified: Thu May 30 12:19:41 2024, max compression
```

## Comparing `tikhub-1.0.6.tar` & `tikhub-1.0.7.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.695263 tikhub-1.0.6/
--rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:10:50.694263 tikhub-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.6/README.md
--rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 12:10:50.695263 tikhub-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-05-30 12:10:47.000000 tikhub-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.659288 tikhub-1.0.6/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.6/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.664430 tikhub-1.0.6/tikhub/api/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.665430 tikhub-1.0.6/tikhub/api/v1/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.665430 tikhub-1.0.6/tikhub/api/v1/endpoints/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.667430 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/captcha/captcha_solver.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.668018 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.671023 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/__init__.py
--rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
--rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
--rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.672056 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/__init__.py
--rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.673560 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.674565 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/__init__.py
--rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.676569 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/__init__.py
--rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.677571 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.679570 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/__init__.py
--rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
--rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.680569 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/__init__.py
--rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.681581 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.682570 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/__init__.py
--rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.683569 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.685753 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.686753 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.688753 tikhub-1.0.6/tikhub/api/v1/models/
--rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.0.6/tikhub/api/v1/models/APIResponseModel.py
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.6/tikhub/api/v1/models/__init__.py
--rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.0.6/tikhub/api/v1/models/douyin_web_models.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.693258 tikhub-1.0.6/tikhub/client/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.6/tikhub/client/__init__.py
--rw-rw-rw-   0        0        0    11300 2024-05-25 02:04:46.000000 tikhub-1.0.6/tikhub/client/api_client.py
--rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.0.6/tikhub/client/api_exceptions.py
--rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.0.6/tikhub/client/api_logger.py
--rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.0.6/tikhub/client/deprecated.py
--rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.6/tikhub/sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-30 12:10:50.663287 tikhub-1.0.6/tikhub.egg-info/
--rw-rw-rw-   0        0        0     3234 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1949 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 12:10:50.000000 tikhub-1.0.6/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.958255 tikhub-1.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:19:41.958255 tikhub-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.7/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:19:41.958255 tikhub-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-30 12:19:09.000000 tikhub-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.929602 tikhub-1.0.7/tikhub/
+-rw-rw-rw-   0        0        0       67 2024-05-30 12:16:42.000000 tikhub-1.0.7/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.932603 tikhub-1.0.7/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.7/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.933602 tikhub-1.0.7/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.7/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.934602 tikhub-1.0.7/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.935602 tikhub-1.0.7/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      478 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.935602 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.939113 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14139 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15959 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12565 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.940618 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31217 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.941624 tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.942625 tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      961 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.943624 tikhub-1.0.7/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3246 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.944623 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.945622 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13951 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22972 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.946622 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    13858 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.948125 tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.949129 tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1834 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.949129 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.950128 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.952128 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.954128 tikhub-1.0.7/tikhub/api/v1/models/
+-rw-rw-rw-   0        0        0     2508 2024-05-20 09:37:37.000000 tikhub-1.0.7/tikhub/api/v1/models/APIResponseModel.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.7/tikhub/api/v1/models/__init__.py
+-rw-rw-rw-   0        0        0     1930 2024-04-04 10:53:44.000000 tikhub-1.0.7/tikhub/api/v1/models/douyin_web_models.py
+-rw-rw-rw-   0        0        0     2428 2024-05-30 12:19:09.000000 tikhub-1.0.7/tikhub/client.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.957248 tikhub-1.0.7/tikhub/http_client/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.7/tikhub/http_client/__init__.py
+-rw-rw-rw-   0        0        0    11320 2024-05-30 12:14:39.000000 tikhub-1.0.7/tikhub/http_client/api_client.py
+-rw-rw-rw-   0        0        0     2819 2024-05-21 09:17:26.000000 tikhub-1.0.7/tikhub/http_client/api_exceptions.py
+-rw-rw-rw-   0        0        0     2978 2024-05-30 11:44:11.000000 tikhub-1.0.7/tikhub/http_client/api_logger.py
+-rw-rw-rw-   0        0        0      438 2024-05-21 13:15:30.000000 tikhub-1.0.7/tikhub/http_client/deprecated.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:19:41.932603 tikhub-1.0.7/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:19:41.000000 tikhub-1.0.7/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1977 2024-05-30 12:19:41.000000 tikhub-1.0.7/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:19:41.000000 tikhub-1.0.7/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 12:19:41.000000 tikhub-1.0.7/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:19:41.000000 tikhub-1.0.7/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.0.6/LICENSE` & `tikhub-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/PKG-INFO` & `tikhub-1.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.6/README.md` & `tikhub-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/setup.py` & `tikhub-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name="tikhub",
-    version="1.0.6",
+    version="1.0.7",
     author="TikHub.io",
     author_email="tikhub.io@proton.me",
     description="A Python SDK for TikHub RESTful API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TikHubIO/TikHub-API-SDK-Python",
     packages=find_packages(),
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # 导入API SDK Client类
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class DouyinAppV1:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 导入API SDK Client类
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 # 标记已废弃的方法
-from tikhub.client.deprecated import deprecated
+from tikhub.http_client.deprecated import deprecated
 
 
 class DouyinAppV2:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # 导入API SDK Client类
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 # 标记已废弃的方法
-from tikhub.client.deprecated import deprecated
+from tikhub.http_client.deprecated import deprecated
 
 
 class DouyinAppV3:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/douyin/web/douyin_web.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/douyin/web/douyin_web.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class DouyinWeb:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/instagram/web/instagram_web.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/instagram/web/instagram_web.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class InstagramWeb:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/tikhub/tikhub_user.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/tikhub/tikhub_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class TikHubUser:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class TikTokAppV2:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class TikTokAppV3:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 
 class TikTokWeb:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/weibo/web/weibo_web.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/weibo/web/weibo_web.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # 导入API SDK Client类
 import json
 
-from tikhub.client.api_client import APIClient
+from tikhub.http_client.api_client import APIClient
 
 class WeiboWeb:
 
     # 初始化 | Initialize
     def __init__(self, client: APIClient):
         self.client = client
```

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py` & `tikhub-1.0.7/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/api/v1/models/APIResponseModel.py` & `tikhub-1.0.7/tikhub/api/v1/models/APIResponseModel.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/api/v1/models/douyin_web_models.py` & `tikhub-1.0.7/tikhub/api/v1/models/douyin_web_models.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/client/api_client.py` & `tikhub-1.0.7/tikhub/http_client/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import asyncio
 from typing import Union, List, Any
 
 import httpx
 from httpx import Response
 
-from tikhub.client.api_exceptions import (
+from tikhub.http_client.api_exceptions import (
     APIError,
     APIConnectionError,
     APIResponseError,
     APITimeoutError,
     APIUnavailableError,
     APIUnauthorizedError,
     APINotFoundError,
     APIRateLimitError,
     APIRetryExhaustedError,
 )
-from tikhub.client.api_logger import logger
+from tikhub.http_client.api_logger import logger
 
 
 class APIClient:
     """
-    基础API客户端 (Base API client)
+    基础API客户端 (Base API http_client)
     """
 
     def __init__(
             self,
             base_url: str,
             client_headers: dict,
             proxies: dict = None,
@@ -56,15 +56,15 @@
         self._max_retries = max_retries
         # 底层连接重试次数 / Underlying connection retry count
         self.atransport = httpx.AsyncHTTPTransport(retries=max_retries)
 
         # 超时等待时间 / Timeout waiting time
         self._timeout = timeout
         self.timeout = httpx.Timeout(timeout)
-        # 异步客户端 / Asynchronous client
+        # 异步客户端 / Asynchronous http_client
         self.aclient = httpx.AsyncClient(
             headers=self.client_headers,
             proxies=self.proxies,
             timeout=self.timeout,
             limits=self.limits,
             transport=self.atransport,
         )
```

### Comparing `tikhub-1.0.6/tikhub/client/api_exceptions.py` & `tikhub-1.0.7/tikhub/http_client/api_exceptions.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/client/api_logger.py` & `tikhub-1.0.7/tikhub/http_client/api_logger.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.6/tikhub/sdk.py` & `tikhub-1.0.7/tikhub/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# sdk.py
-from tikhub.client.api_client import APIClient
+# http_client
+from tikhub.http_client.api_client import APIClient
 
 # TikHub
 from tikhub.api.v1.endpoints.tikhub.tikhub_user import TikHubUser
 
-
 # Douyin
 from tikhub.api.v1.endpoints.douyin.web.douyin_web import DouyinWeb
 from tikhub.api.v1.endpoints.douyin.app.douyin_app_v1 import DouyinAppV1
 from tikhub.api.v1.endpoints.douyin.app.douyin_app_v2 import DouyinAppV2
 from tikhub.api.v1.endpoints.douyin.app.douyin_app_v3 import DouyinAppV3
 
 # TikTok
@@ -20,32 +19,40 @@
 from tikhub.api.v1.endpoints.instagram.web.instagram_web import InstagramWeb
 
 # Weibo
 from tikhub.api.v1.endpoints.weibo.web.weibo_web import WeiboWeb
 
 
 class Client:
-    def __init__(self, base_url: str = 'https://beta.tikhub.io', api_key: str = None):
+    def __init__(self,
+                 base_url: str = 'https://beta.tikhub.io',
+                 api_key: str = None,
+                 proxies: dict = None,
+                 max_retries: int = 3,
+                 max_connections: int = 50,
+                 timeout: int = 10,
+                 max_tasks: int = 50
+                 ):
         # Base URL
         self.base_url = base_url
 
         # API Key
         self.api_key = api_key
         if not self.api_key:
             raise RuntimeError("API Key is required to use the SDK. | 需要API Key才能使用SDK。")
 
         # API Client
         self.client = APIClient(
             base_url=self.base_url,
             client_headers={"Authorization": f"Bearer {self.api_key}"},
-            proxies=None,
-            max_retries=3,
-            max_connections=50,
-            timeout=10,
-            max_tasks=50,
+            proxies=proxies,
+            max_retries=max_retries,
+            max_connections=max_connections,
+            timeout=timeout,
+            max_tasks=max_tasks
         )
 
         # TikHub
         self.TikHubUser = TikHubUser(self.client)
 
         # Douyin
         self.DouyinWeb = DouyinWeb(self.client)
```

### Comparing `tikhub-1.0.6/tikhub.egg-info/PKG-INFO` & `tikhub-1.0.7/tikhub.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `tikhub-1.0.6/tikhub.egg-info/SOURCES.txt` & `tikhub-1.0.7/tikhub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tikhub/__init__.py
-tikhub/sdk.py
+tikhub/client.py
 tikhub.egg-info/PKG-INFO
 tikhub.egg-info/SOURCES.txt
 tikhub.egg-info/dependency_links.txt
 tikhub.egg-info/requires.txt
 tikhub.egg-info/top_level.txt
 tikhub/api/__init__.py
 tikhub/api/v1/__init__.py
@@ -40,12 +40,12 @@
 tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
 tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
 tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
 tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
 tikhub/api/v1/models/APIResponseModel.py
 tikhub/api/v1/models/__init__.py
 tikhub/api/v1/models/douyin_web_models.py
-tikhub/client/__init__.py
-tikhub/client/api_client.py
-tikhub/client/api_exceptions.py
-tikhub/client/api_logger.py
-tikhub/client/deprecated.py
+tikhub/http_client/__init__.py
+tikhub/http_client/api_client.py
+tikhub/http_client/api_exceptions.py
+tikhub/http_client/api_logger.py
+tikhub/http_client/deprecated.py
```

