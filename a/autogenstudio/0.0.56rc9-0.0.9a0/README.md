# Comparing `tmp/autogenstudio-0.0.56rc9.tar.gz` & `tmp/autogenstudio-0.0.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogenstudio-0.0.56rc9.tar", last modified: Wed May  8 18:35:06 2024, max compression
+gzip compressed data, was "autogenstudio-0.0.9a0.tar", last modified: Wed Dec  6 21:25:08 2023, max compression
```

## Comparing `autogenstudio-0.0.56rc9.tar` & `autogenstudio-0.0.9a0.tar`

### file list

```diff
@@ -1,114 +1,35 @@
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:06.181260 autogenstudio-0.0.56rc9/
--rw-r--r--   0 victordibia   (501) staff       (20)      361 2024-04-17 23:09:07.000000 autogenstudio-0.0.56rc9/.gitignore
--rw-r--r--   0 victordibia   (501) staff       (20)      421 2024-03-21 23:47:34.000000 autogenstudio-0.0.56rc9/Dockerfile
--rw-r--r--   0 victordibia   (501) staff       (20)      210 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc9/MANIFEST.in
--rw-r--r--   0 victordibia   (501) staff       (20)    12983 2024-05-08 18:35:06.175979 autogenstudio-0.0.56rc9/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)    12008 2024-04-23 18:30:57.000000 autogenstudio-0.0.56rc9/README.md
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.588108 autogenstudio-0.0.56rc9/autogenstudio/
--rw-r--r--   0 victordibia   (501) staff       (20)      116 2024-05-02 20:53:06.000000 autogenstudio-0.0.56rc9/autogenstudio/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     9639 2024-05-08 13:46:55.000000 autogenstudio-0.0.56rc9/autogenstudio/chatmanager.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1734 2024-04-17 23:18:50.000000 autogenstudio-0.0.56rc9/autogenstudio/cli.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.608375 autogenstudio-0.0.56rc9/autogenstudio/database/
--rw-r--r--   0 victordibia   (501) staff       (20)       73 2024-05-07 23:42:56.000000 autogenstudio-0.0.56rc9/autogenstudio/database/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     3610 2024-05-02 02:11:17.000000 autogenstudio-0.0.56rc9/autogenstudio/database/alembic.ini
--rw-r--r--   0 victordibia   (501) staff       (20)    20441 2024-05-08 17:30:14.000000 autogenstudio-0.0.56rc9/autogenstudio/database/dbmanager.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.624730 autogenstudio-0.0.56rc9/autogenstudio/database/migrations/
--rw-r--r--   0 victordibia   (501) staff       (20)       39 2024-05-04 23:23:37.000000 autogenstudio-0.0.56rc9/autogenstudio/database/migrations/README
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2024-05-04 23:23:37.000000 autogenstudio-0.0.56rc9/autogenstudio/database/migrations/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     2248 2024-05-04 23:23:39.000000 autogenstudio-0.0.56rc9/autogenstudio/database/migrations/env.py
--rw-r--r--   0 victordibia   (501) staff       (20)      651 2024-05-02 02:13:02.000000 autogenstudio-0.0.56rc9/autogenstudio/database/migrations/script.py.mako
--rw-r--r--   0 victordibia   (501) staff       (20)    15900 2024-05-08 03:02:38.000000 autogenstudio-0.0.56rc9/autogenstudio/database/utils.py
--rw-r--r--   0 victordibia   (501) staff       (20)     9517 2024-05-08 02:02:34.000000 autogenstudio-0.0.56rc9/autogenstudio/datamodel.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.640881 autogenstudio-0.0.56rc9/autogenstudio/utils/
--rw-r--r--   0 victordibia   (501) staff       (20)       21 2024-05-07 23:43:09.000000 autogenstudio-0.0.56rc9/autogenstudio/utils/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)    24868 2024-04-17 19:14:33.000000 autogenstudio-0.0.56rc9/autogenstudio/utils/dbdefaults.json
--rw-r--r--   0 victordibia   (501) staff       (20)    16029 2024-05-08 02:02:34.000000 autogenstudio-0.0.56rc9/autogenstudio/utils/utils.py
--rw-r--r--   0 victordibia   (501) staff       (20)       71 2024-05-08 18:34:48.000000 autogenstudio-0.0.56rc9/autogenstudio/version.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.646685 autogenstudio-0.0.56rc9/autogenstudio/web/
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)    14022 2024-05-08 18:34:28.000000 autogenstudio-0.0.56rc9/autogenstudio/web/app.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.819787 autogenstudio-0.0.56rc9/autogenstudio/web/ui/
--rw-r--r--   0 victordibia   (501) staff       (20)  1494879 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-70f9f4903a3352646019.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1173 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-70f9f4903a3352646019.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)  5012936 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/318ce576f236b79fd96f75904c13f6e55c3eee57-70f9f4903a3352646019.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.834120 autogenstudio-0.0.56rc9/autogenstudio/web/ui/404/
--rw-r--r--   0 victordibia   (501) staff       (20)    44335 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/404/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)    44339 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/404.html
--rw-r--r--   0 victordibia   (501) staff       (20)   232601 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/app-2b38170129588a9fab4b.js
--rw-r--r--   0 victordibia   (501) staff       (20)      512 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/app-2b38170129588a9fab4b.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)   952394 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/app-2b38170129588a9fab4b.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.845267 autogenstudio-0.0.56rc9/autogenstudio/web/ui/build/
--rw-r--r--   0 victordibia   (501) staff       (20)    54352 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/build/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)      432 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/chunk-map.json
--rw-r--r--   0 victordibia   (501) staff       (20)      807 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-404-tsx-9cfc00764f659a099247.js
--rw-r--r--   0 victordibia   (501) staff       (20)     2006 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-404-tsx-9cfc00764f659a099247.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)   177280 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-build-tsx-1fc19db57ad68d15f326.js
--rw-r--r--   0 victordibia   (501) staff       (20)   655909 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-build-tsx-1fc19db57ad68d15f326.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     4156 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-gallery-index-tsx-120f318117531bdd081d.js
--rw-r--r--   0 victordibia   (501) staff       (20)    12739 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-gallery-index-tsx-120f318117531bdd081d.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)    13892 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-index-tsx-df9ebcbeeaaabdd10426.js
--rw-r--r--   0 victordibia   (501) staff       (20)    41354 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/component---src-pages-index-tsx-df9ebcbeeaaabdd10426.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     1539 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/favicon-32x32.png
--rw-r--r--   0 victordibia   (501) staff       (20)   140385 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js
--rw-r--r--   0 victordibia   (501) staff       (20)      721 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js.LICENSE.txt
--rw-r--r--   0 victordibia   (501) staff       (20)   355268 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/framework-3b041e76ed3d1ab0eeef.js.map
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.855614 autogenstudio-0.0.56rc9/autogenstudio/web/ui/gallery/
--rw-r--r--   0 victordibia   (501) staff       (20)    47928 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/gallery/index.html
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.864772 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/
--rw-r--r--   0 victordibia   (501) staff       (20)     7211 2024-05-08 02:12:35.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-144x144.png
--rw-r--r--   0 victordibia   (501) staff       (20)    10299 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-192x192.png
--rw-r--r--   0 victordibia   (501) staff       (20)    15443 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-256x256.png
--rw-r--r--   0 victordibia   (501) staff       (20)    26979 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-384x384.png
--rw-r--r--   0 victordibia   (501) staff       (20)     2296 2024-05-08 02:12:35.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-48x48.png
--rw-r--r--   0 victordibia   (501) staff       (20)    39636 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-512x512.png
--rw-r--r--   0 victordibia   (501) staff       (20)     3358 2024-05-08 02:12:35.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-72x72.png
--rw-r--r--   0 victordibia   (501) staff       (20)     4475 2024-05-08 02:12:35.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/icons/icon-96x96.png
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.516545 autogenstudio-0.0.56rc9/autogenstudio/web/ui/images/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.865939 autogenstudio-0.0.56rc9/autogenstudio/web/ui/images/svgs/
--rw-r--r--   0 victordibia   (501) staff       (20)    10553 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/images/svgs/welcome.svg
--rw-r--r--   0 victordibia   (501) staff       (20)    51999 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/index.html
--rw-r--r--   0 victordibia   (501) staff       (20)      839 2024-05-08 02:12:36.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/manifest.webmanifest
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.867050 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.870033 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/404/
--rw-r--r--   0 victordibia   (501) staff       (20)      120 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/404/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.871837 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/404.html/
--rw-r--r--   0 victordibia   (501) staff       (20)      124 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/404.html/page-data.json
--rw-r--r--   0 victordibia   (501) staff       (20)       50 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/app-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.872330 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/build/
--rw-r--r--   0 victordibia   (501) staff       (20)      230 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/build/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.879717 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/gallery/
--rw-r--r--   0 victordibia   (501) staff       (20)      240 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/gallery/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.880585 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/index/
--rw-r--r--   0 victordibia   (501) staff       (20)      224 2024-05-08 02:13:29.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/page-data/index/page-data.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.928234 autogenstudio-0.0.56rc9/autogenstudio/web/ui/sitemap/
--rw-r--r--   0 victordibia   (501) staff       (20)      627 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/sitemap/sitemap-0.xml
--rw-r--r--   0 victordibia   (501) staff       (20)      187 2024-05-08 02:13:45.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/sitemap/sitemap-index.xml
--rw-r--r--   0 victordibia   (501) staff       (20)    39823 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/styles.7edf900ca1a9288e1661.css
--rw-r--r--   0 victordibia   (501) staff       (20)     3998 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/webpack-runtime-b8524354a2f9ef49478d.js
--rw-r--r--   0 victordibia   (501) staff       (20)    18697 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/webpack-runtime-b8524354a2f9ef49478d.js.map
--rw-r--r--   0 victordibia   (501) staff       (20)     2543 2024-05-08 02:13:12.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/webpack.stats.json
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:05.992220 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:06.170696 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/
--rw-r--r--   0 victordibia   (501) staff       (20)    28104 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)    17511 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-media.js
--rw-r--r--   0 victordibia   (501) staff       (20)    27197 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-sandbox-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1995 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)    82089 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-ww-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)    81649 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown-ww-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     3341 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/debug/partytown.js
--rw-r--r--   0 victordibia   (501) staff       (20)    28273 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/partytown-atomics.js
--rw-r--r--   0 victordibia   (501) staff       (20)     5689 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/partytown-media.js
--rw-r--r--   0 victordibia   (501) staff       (20)    29137 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/partytown-sw.js
--rw-r--r--   0 victordibia   (501) staff       (20)     1384 2024-05-08 02:12:32.000000 autogenstudio-0.0.56rc9/autogenstudio/web/ui/~partytown/partytown.js
--rw-r--r--   0 victordibia   (501) staff       (20)    10791 2024-04-18 18:15:41.000000 autogenstudio-0.0.56rc9/autogenstudio/workflowmanager.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2024-05-08 18:35:06.174498 autogenstudio-0.0.56rc9/autogenstudio.egg-info/
--rw-r--r--   0 victordibia   (501) staff       (20)    12983 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)     4098 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/SOURCES.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        1 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/dependency_links.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       56 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/entry_points.txt
--rw-r--r--   0 victordibia   (501) staff       (20)      174 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/requires.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       14 2024-05-08 18:35:05.000000 autogenstudio-0.0.56rc9/autogenstudio.egg-info/top_level.txt
--rw-r--r--   0 victordibia   (501) staff       (20)     1515 2024-05-04 23:23:53.000000 autogenstudio-0.0.56rc9/pyproject.toml
--rw-r--r--   0 victordibia   (501) staff       (20)        2 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc9/requirements.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2024-05-08 18:35:06.181385 autogenstudio-0.0.56rc9/setup.cfg
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2024-03-19 16:11:36.000000 autogenstudio-0.0.56rc9/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      342 2023-12-06 21:04:40.000000 autogenstudio-0.0.9a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      152 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7308 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     6592 2023-12-06 20:46:34.000000 autogenstudio-0.0.9a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       83 2023-12-06 20:49:20.000000 autogenstudio-0.0.9a0/autogenstudio/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2284 2023-12-06 20:43:55.000000 autogenstudio-0.0.9a0/autogenstudio/chatmanager.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      862 2023-12-06 20:49:48.000000 autogenstudio-0.0.9a0/autogenstudio/cli.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4036 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/utils/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       44 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)    12441 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/dbutils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)    15392 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/utils/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       43 2023-12-04 03:29:11.000000 autogenstudio-0.0.9a0/autogenstudio/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     9262 2023-12-06 20:44:10.000000 autogenstudio-0.0.9a0/autogenstudio/web/app.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/skills/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1329 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/fetch_profile.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2444 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/find_papers_arxiv.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1965 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/web/skills/global/generate_images.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4676 2023-12-01 20:04:02.000000 autogenstudio-0.0.9a0/autogenstudio/workflowmanager.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-12-06 21:25:08.862963 autogenstudio-0.0.9a0/autogenstudio.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     7308 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      758 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       56 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       77 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       14 2023-12-06 21:25:08.000000 autogenstudio-0.0.9a0/autogenstudio.egg-info/top_level.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1355 2023-12-06 20:48:09.000000 autogenstudio-0.0.9a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        2 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/requirements.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-12-06 21:25:08.866963 autogenstudio-0.0.9a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-11-20 19:33:35.000000 autogenstudio-0.0.9a0/setup.py
```

### Comparing `autogenstudio-0.0.56rc9/pyproject.toml` & `autogenstudio-0.0.9a0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "autogenstudio"
 authors = [
-  { name="AutoGen Team", email="autogen@microsoft.com" },
+  { name="Autogen Team", email="autogen@microsoft.com" },
 ]
-description = "AutoGen Studio"
+description = "Autogen Studio"
 readme = "README.md"
 license = { file="LICENSE" }
-requires-python = ">=3.9, <3.13"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 
 dependencies = [
     "pydantic",
     "fastapi",
     "typer",
     "uvicorn",
     "arxiv",
-    "pyautogen[gemini]>=0.2.0",
-    "python-dotenv",
-    "websockets",
-    "numpy < 2.0.0",
-    "sqlmodel",
-    "psycopg",
-    "alembic",
-    "loguru",
+    "pyautogen==0.2.0"
 ]
-optional-dependencies = {web = ["fastapi", "uvicorn"], database = ["psycopg"]}
+optional-dependencies = {web = ["fastapi", "uvicorn"]}
 
 dynamic = ["version"]
 
 [tool.setuptools]
 include-package-data = true
```

