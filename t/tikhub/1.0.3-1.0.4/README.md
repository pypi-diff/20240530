# Comparing `tmp/tikhub-1.0.3.tar.gz` & `tmp/tikhub-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikhub-1.0.3.tar", last modified: Sat Apr 29 00:14:12 2023, max compression
+gzip compressed data, was "tikhub-1.0.4.tar", last modified: Thu May 30 11:51:03 2024, max compression
```

## Comparing `tikhub-1.0.3.tar` & `tikhub-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 00:14:12.352697 tikhub-1.0.3/
--rw-rw-rw-   0        0        0    11558 2023-04-19 07:18:56.000000 tikhub-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     6808 2023-04-29 00:14:12.351693 tikhub-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     6014 2023-04-29 00:09:46.000000 tikhub-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-29 00:14:12.353694 tikhub-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1324 2023-04-29 00:07:39.000000 tikhub-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:14:12.320695 tikhub-1.0.3/test/
--rw-rw-rw-   0        0        0     1817 2023-04-29 00:02:57.000000 tikhub-1.0.3/test/test.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:14:12.337694 tikhub-1.0.3/tikhub/
--rw-rw-rw-   0        0        0     3850 2023-04-20 09:51:13.000000 tikhub-1.0.3/tikhub/AiohttpClient.py
--rw-rw-rw-   0        0        0     2024 2023-04-29 00:06:53.000000 tikhub-1.0.3/tikhub/Auth.py
--rw-rw-rw-   0        0        0    18012 2023-04-28 22:28:38.000000 tikhub-1.0.3/tikhub/DouyinAPI.py
--rw-rw-rw-   0        0        0     9637 2023-04-27 00:36:56.000000 tikhub-1.0.3/tikhub/TikTokAPI.py
--rw-rw-rw-   0        0        0     4681 2023-04-29 00:06:53.000000 tikhub-1.0.3/tikhub/Utils.py
--rw-rw-rw-   0        0        0      365 2023-04-23 09:15:59.000000 tikhub-1.0.3/tikhub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 00:14:12.349694 tikhub-1.0.3/tikhub.egg-info/
--rw-rw-rw-   0        0        0     6808 2023-04-29 00:14:12.000000 tikhub-1.0.3/tikhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-04-29 00:14:12.000000 tikhub-1.0.3/tikhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 00:14:12.000000 tikhub-1.0.3/tikhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-29 00:14:12.000000 tikhub-1.0.3/tikhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-29 00:14:12.000000 tikhub-1.0.3/tikhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.533458 tikhub-1.0.4/
+-rw-rw-rw-   0        0        0    11558 2024-05-21 08:59:32.000000 tikhub-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       36 2024-05-30 11:25:11.000000 tikhub-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3234 2024-05-30 11:51:03.532459 tikhub-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2709 2024-05-30 11:39:24.000000 tikhub-1.0.4/README.md
+-rw-rw-rw-   0        0        0       93 2024-05-30 11:27:47.000000 tikhub-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-30 11:51:03.533458 tikhub-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      975 2024-05-30 11:50:33.000000 tikhub-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.506625 tikhub-1.0.4/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:00:16.000000 tikhub-1.0.4/tikhub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.510625 tikhub-1.0.4/tikhub/api/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.511626 tikhub-1.0.4/tikhub/api/v1/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.512624 tikhub-1.0.4/tikhub/api/v1/endpoints/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:06:51.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.512624 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:46.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/__init__.py
+-rw-rw-rw-   0        0        0      473 2024-05-21 09:24:45.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/captcha/captcha_solver.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.515132 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.518131 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:57:03.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/__init__.py
+-rw-rw-rw-   0        0        0    14134 2024-05-21 13:31:15.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v1.py
+-rw-rw-rw-   0        0        0    15949 2024-05-25 02:12:42.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v2.py
+-rw-rw-rw-   0        0        0    12555 2024-05-25 02:20:14.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/app/douyin_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.519132 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 09:29:11.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/__init__.py
+-rw-rw-rw-   0        0        0    31212 2024-05-25 04:06:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/douyin/web/douyin_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.520132 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.521132 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:14:52.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/__init__.py
+-rw-rw-rw-   0        0        0      956 2024-05-25 02:32:14.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/instagram/web/instagram_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.522132 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:07.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/__init__.py
+-rw-rw-rw-   0        0        0     3241 2024-05-25 03:58:17.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tikhub/tikhub_user.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.523132 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.525457 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:32.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/__init__.py
+-rw-rw-rw-   0        0        0    13946 2024-05-25 04:11:50.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v2.py
+-rw-rw-rw-   0        0        0    22967 2024-05-25 04:50:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/app/tiktok_app_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.526457 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:37.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/__init__.py
+-rw-rw-rw-   0        0        0    13853 2024-05-25 03:58:17.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/tiktok/web/tiktok_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.527457 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.528457 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:15:58.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/__init__.py
+-rw-rw-rw-   0        0        0     1829 2024-05-25 03:40:51.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/weibo/web/weibo_web.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.528457 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.530458 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:23.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/__init__.py
+-rw-rw-rw-   0        0        0      664 2024-05-04 23:05:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/app/xiaohongshu_app.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.531459 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/
+-rw-rw-rw-   0        0        0        0 2024-05-21 12:16:27.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/__init__.py
+-rw-rw-rw-   0        0        0      662 2024-05-04 23:05:56.000000 tikhub-1.0.4/tikhub/api/v1/endpoints/xiaohongshu/web/xiaohongshu_web.py
+-rw-rw-rw-   0        0        0     2127 2024-05-30 11:44:11.000000 tikhub-1.0.4/tikhub/sdk.py
+drwxrwxrwx   0        0        0        0 2024-05-30 11:51:03.510625 tikhub-1.0.4/tikhub.egg-info/
+-rw-rw-rw-   0        0        0     3234 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1691 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-30 11:51:03.000000 tikhub-1.0.4/tikhub.egg-info/top_level.txt
```

### Comparing `tikhub-1.0.3/LICENSE` & `tikhub-1.0.4/LICENSE`

 * *Files identical despite different names*

