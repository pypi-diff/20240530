# Comparing `tmp/tikhub-1.0.4.tar.gz` & `tmp/tikhub-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.0.4.tar", last modified: Thu May 30 11:51:03 2024, max compression
+gzip compressed data, was "tikhub-1.0.5.tar", last modified: Thu May 30 12:04:54 2024, max compression
```

## Comparing `tikhub-1.0.4.tar` & `tikhub-1.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.533458 tikhub-1.0.4/
--rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3234 2024-05-30 11:51:03.532459 tikhub-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.4/README.md
--rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-30 11:51:03.533458 tikhub-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      975 2024-05-30 11:50:33.000000 tikhub-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.506625 tikhub-1.0.4/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.4/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.510625 tikhub-1.0.4/tikhub/api/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.511626 tikhub-1.0.4/tikhub/api/v1/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.512624 tikhub-1.0.4/tikhub/api/v1/endpoints/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.512624 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/__init__.py
--rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/captcha_solver.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.515132 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.518131 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/__init__.py
--rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
--rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
--rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.519132 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/__init__.py
--rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.520132 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.521132 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/__init__.py
--rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.522132 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/__init__.py
--rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.523132 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.525457 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/__init__.py
--rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
--rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.526457 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/__init__.py
--rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.527457 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.528457 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/__init__.py
--rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.528457 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.530458 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
--rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.531459 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/
--rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
--rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
--rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.4/tikhub/sdk.py
-drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.510625 tikhub-1.0.4/tikhub.egg-info/
--rw-rw-rw-   0        0        0     3234 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1691 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.481435 tikhub-1.0.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:04:54.480442 tikhub-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.5/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 12:04:54.481435 tikhub-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-30 12:04:34.000000 tikhub-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.458077 tikhub-1.0.5/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.5/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.462072 tikhub-1.0.5/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.463072 tikhub-1.0.5/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.463665 tikhub-1.0.5/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.464750 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.464750 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.467748 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.468751 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.468751 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.469741 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.471747 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.471747 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.474366 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.475365 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.476435 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.477440 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.477440 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.478436 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.480442 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+-rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.5/tikhub/sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-30 12:04:54.462072 tikhub-1.0.5/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     3234 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1691 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 12:04:54.000000 tikhub-1.0.5/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.0.4/LICENSE` & `tikhub-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/PKG-INFO` & `tikhub-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx>=0.27.1
+Requires-Dist: httpx>=0.27.0
 Requires-Dist: rich~=13.7.1
 
 # 更新 - 2023年6月15日
 
 <div align="center">
 <h1><a href="https://pypi.org/project/tikhub">TikHub_API</a></h1>
 <a href="https://github.com/TikHubIO/TikHub-API-Python-SDK/blob/main/README.en.md">English</a> | <a href="https://github.com/TikHubIO/TikHub-API-Python-SDK/blob/main/README.md">简体中文</a>
```

### Comparing `tikhub-1.0.4/README.md` & `tikhub-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/setup.py` & `tikhub-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name="tikhub",
-    version="1.0.4",
+    version="1.0.5",
     author="TikHub.io",
     author_email="tikhub.io@proton.me",
     description="A Python SDK for TikHub RESTful API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TikHubIO/TikHub-API-SDK-Python",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
     install_requires=[
-        "httpx>=0.27.1",
+        "httpx>=0.27.0",
         "rich~=13.7.1",
     ],
 )
```

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/douyin_web.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/douyin/web/douyin_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/instagram_web.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/instagram/web/instagram_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/tikhub_user.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/tikhub/tikhub_user.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/weibo_web.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/weibo/web/weibo_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py` & `tikhub-1.0.5/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub/sdk.py` & `tikhub-1.0.5/tikhub/sdk.py`

 * *Files identical despite different names*

### Comparing `tikhub-1.0.4/tikhub.egg-info/PKG-INFO` & `tikhub-1.0.5/tikhub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tikhub
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python SDK for TikHub RESTful API
 Home-page: https://github.com/TikHubIO/TikHub-API-SDK-Python
 Author: TikHub.io
 Author-email: tikhub.io@proton.me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx>=0.27.1
+Requires-Dist: httpx>=0.27.0
 Requires-Dist: rich~=13.7.1
 
 # 更新 - 2023年6月15日
 
 <div align="center">
 <h1><a href="https://pypi.org/project/tikhub">TikHub_API</a></h1>
 <a href="https://github.com/TikHubIO/TikHub-API-Python-SDK/blob/main/README.en.md">English</a> | <a href="https://github.com/TikHubIO/TikHub-API-Python-SDK/blob/main/README.md">简体中文</a>
```

### Comparing `tikhub-1.0.4/tikhub.egg-info/SOURCES.txt` & `tikhub-1.0.5/tikhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

