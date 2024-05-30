# Comparing `tmp/pyalsaaudio-0.9.1.tar.gz` & `tmp/pyalsaaudio-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyalsaaudio-0.9.1.tar", last modified: Tue May  3 19:14:37 2022, max compression
+gzip compressed data, was "pyalsaaudio-0.9.2.tar", last modified: Fri May  6 19:36:01 2022, max compression
```

## Comparing `pyalsaaudio-0.9.1.tar` & `pyalsaaudio-0.9.2.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.529240 pyalsaaudio-0.9.1/
--rw-r--r--   0 lars      (1000) lars      (1000)     2526 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.1/LICENSE
--rw-r--r--   0 lars      (1000) lars      (1000)      137 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.1/MANIFEST.in
--rw-r--r--   0 lars      (1000) lars      (1000)      956 2022-05-03 19:14:37.529240 pyalsaaudio-0.9.1/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     2335 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.1/README.md
--rw-r--r--   0 lars      (1000) lars      (1000)      104 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.1/TODO
--rw-r--r--   0 lars      (1000) lars      (1000)    86209 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/alsaaudio.c
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.485238 pyalsaaudio-0.9.1/doc/
--rw-r--r--   0 lars      (1000) lars      (1000)     2312 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.1/doc/Makefile
--rw-r--r--   0 lars      (1000) lars      (1000)     4972 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.1/doc/conf.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.489239 pyalsaaudio-0.9.1/doc/gh-pages/
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.505239 pyalsaaudio-0.9.1/doc/gh-pages/_static/
--rw-r--r--   0 lars      (1000) lars      (1000)      673 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/ajax-loader.gif
--rw-r--r--   0 lars      (1000) lars      (1000)    11185 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/alabaster.css
--rw-r--r--   0 lars      (1000) lars      (1000)    14692 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/basic.css
--rw-r--r--   0 lars      (1000) lars      (1000)      756 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/comment-bright.png
--rw-r--r--   0 lars      (1000) lars      (1000)      829 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/comment-close.png
--rw-r--r--   0 lars      (1000) lars      (1000)      641 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/comment.png
--rw-r--r--   0 lars      (1000) lars      (1000)       42 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/custom.css
--rw-r--r--   0 lars      (1000) lars      (1000)     4040 2017-07-09 11:44:11.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/default.css
--rw-r--r--   0 lars      (1000) lars      (1000)    10766 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/doctools.js
--rw-r--r--   0 lars      (1000) lars      (1000)      422 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/documentation_options.js
--rw-r--r--   0 lars      (1000) lars      (1000)      222 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/down-pressed.png
--rw-r--r--   0 lars      (1000) lars      (1000)      202 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/down.png
--rw-r--r--   0 lars      (1000) lars      (1000)      286 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/file.png
--rw-r--r--   0 lars      (1000) lars      (1000)   263767 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery-3.1.0.js
--rw-r--r--   0 lars      (1000) lars      (1000)   287630 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery-3.5.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    89476 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery.js
--rw-r--r--   0 lars      (1000) lars      (1000)    10854 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/language_data.js
--rw-r--r--   0 lars      (1000) lars      (1000)       90 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/minus.png
--rw-r--r--   0 lars      (1000) lars      (1000)       90 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/plus.png
--rw-r--r--   0 lars      (1000) lars      (1000)     4780 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/pygments.css
--rw-r--r--   0 lars      (1000) lars      (1000)    16634 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/searchtools.js
--rw-r--r--   0 lars      (1000) lars      (1000)     4803 2017-07-09 11:44:11.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/sidebar.js
--rw-r--r--   0 lars      (1000) lars      (1000)    68420 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore-1.13.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    35168 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore-1.3.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    19530 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore.js
--rw-r--r--   0 lars      (1000) lars      (1000)      214 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/up-pressed.png
--rw-r--r--   0 lars      (1000) lars      (1000)      203 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/up.png
--rw-r--r--   0 lars      (1000) lars      (1000)    25351 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/_static/websupport.js
--rw-r--r--   0 lars      (1000) lars      (1000)     9925 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/genindex.html
--rw-r--r--   0 lars      (1000) lars      (1000)     6191 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/index.html
--rw-r--r--   0 lars      (1000) lars      (1000)    65554 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/libalsaaudio.html
--rw-r--r--   0 lars      (1000) lars      (1000)     3762 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/py-modindex.html
--rw-r--r--   0 lars      (1000) lars      (1000)    10195 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/pyalsaaudio.html
--rw-r--r--   0 lars      (1000) lars      (1000)     3521 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/search.html
--rw-r--r--   0 lars      (1000) lars      (1000)     9587 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/searchindex.js
--rw-r--r--   0 lars      (1000) lars      (1000)     7462 2022-05-03 19:06:28.000000 pyalsaaudio-0.9.1/doc/gh-pages/terminology.html
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.509240 pyalsaaudio-0.9.1/doc/html/
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.525240 pyalsaaudio-0.9.1/doc/html/_static/
--rw-r--r--   0 lars      (1000) lars      (1000)      673 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/ajax-loader.gif
--rw-r--r--   0 lars      (1000) lars      (1000)    11185 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/_static/alabaster.css
--rw-r--r--   0 lars      (1000) lars      (1000)    14692 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/_static/basic.css
--rw-r--r--   0 lars      (1000) lars      (1000)      756 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/comment-bright.png
--rw-r--r--   0 lars      (1000) lars      (1000)      829 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/comment-close.png
--rw-r--r--   0 lars      (1000) lars      (1000)      641 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/comment.png
--rw-r--r--   0 lars      (1000) lars      (1000)       42 2017-03-30 21:24:11.000000 pyalsaaudio-0.9.1/doc/html/_static/custom.css
--rw-r--r--   0 lars      (1000) lars      (1000)    10766 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/doctools.js
--rw-r--r--   0 lars      (1000) lars      (1000)      422 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/_static/documentation_options.js
--rw-r--r--   0 lars      (1000) lars      (1000)      222 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/down-pressed.png
--rw-r--r--   0 lars      (1000) lars      (1000)      202 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/down.png
--rw-r--r--   0 lars      (1000) lars      (1000)      286 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/file.png
--rw-r--r--   0 lars      (1000) lars      (1000)   263767 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/jquery-3.1.0.js
--rw-r--r--   0 lars      (1000) lars      (1000)   287630 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/jquery-3.5.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    89476 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/jquery.js
--rw-r--r--   0 lars      (1000) lars      (1000)    10854 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/_static/language_data.js
--rw-r--r--   0 lars      (1000) lars      (1000)       90 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/minus.png
--rw-r--r--   0 lars      (1000) lars      (1000)       90 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/plus.png
--rw-r--r--   0 lars      (1000) lars      (1000)     4780 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/_static/pygments.css
--rw-r--r--   0 lars      (1000) lars      (1000)    16634 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/searchtools.js
--rw-r--r--   0 lars      (1000) lars      (1000)    68420 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/underscore-1.13.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    35168 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/underscore-1.3.1.js
--rw-r--r--   0 lars      (1000) lars      (1000)    19530 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.1/doc/html/_static/underscore.js
--rw-r--r--   0 lars      (1000) lars      (1000)      214 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/up-pressed.png
--rw-r--r--   0 lars      (1000) lars      (1000)      203 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/up.png
--rw-r--r--   0 lars      (1000) lars      (1000)    25351 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.1/doc/html/_static/websupport.js
--rw-r--r--   0 lars      (1000) lars      (1000)     9925 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/genindex.html
--rw-r--r--   0 lars      (1000) lars      (1000)     6191 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/index.html
--rw-r--r--   0 lars      (1000) lars      (1000)    65554 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/libalsaaudio.html
--rw-r--r--   0 lars      (1000) lars      (1000)     3762 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/py-modindex.html
--rw-r--r--   0 lars      (1000) lars      (1000)    10195 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/pyalsaaudio.html
--rw-r--r--   0 lars      (1000) lars      (1000)     3521 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/search.html
--rw-r--r--   0 lars      (1000) lars      (1000)     9587 2022-05-03 19:06:26.000000 pyalsaaudio-0.9.1/doc/html/searchindex.js
--rw-r--r--   0 lars      (1000) lars      (1000)     7462 2022-05-03 19:06:25.000000 pyalsaaudio-0.9.1/doc/html/terminology.html
--rw-r--r--   0 lars      (1000) lars      (1000)      756 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.1/doc/index.rst
--rw-r--r--   0 lars      (1000) lars      (1000)    25083 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/doc/libalsaaudio.rst
--rw-r--r--   0 lars      (1000) lars      (1000)     4533 2019-03-27 13:45:59.000000 pyalsaaudio-0.9.1/doc/pyalsaaudio.rst
--rw-r--r--   0 lars      (1000) lars      (1000)     3222 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.1/doc/terminology.rst
--rw-r--r--   0 lars      (1000) lars      (1000)     2712 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/isine.py
--rwxr-xr-x   0 lars      (1000) lars      (1000)     5270 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/mixertest.py
--rw-r--r--   0 lars      (1000) lars      (1000)      540 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.1/play_rusage.py
--rwxr-xr-x   0 lars      (1000) lars      (1000)     1412 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/playbacktest.py
--rwxr-xr-x   0 lars      (1000) lars      (1000)     1484 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/playwav.py
-drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-03 19:14:37.529240 pyalsaaudio-0.9.1/pyalsaaudio.egg-info/
--rw-r--r--   0 lars      (1000) lars      (1000)      956 2022-05-03 19:14:37.000000 pyalsaaudio-0.9.1/pyalsaaudio.egg-info/PKG-INFO
--rw-r--r--   0 lars      (1000) lars      (1000)     2590 2022-05-03 19:14:37.000000 pyalsaaudio-0.9.1/pyalsaaudio.egg-info/SOURCES.txt
--rw-r--r--   0 lars      (1000) lars      (1000)        1 2022-05-03 19:14:37.000000 pyalsaaudio-0.9.1/pyalsaaudio.egg-info/dependency_links.txt
--rw-r--r--   0 lars      (1000) lars      (1000)       10 2022-05-03 19:14:37.000000 pyalsaaudio-0.9.1/pyalsaaudio.egg-info/top_level.txt
--rwxr-xr-x   0 lars      (1000) lars      (1000)     1755 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/recordtest.py
--rw-r--r--   0 lars      (1000) lars      (1000)       38 2022-05-03 19:14:37.529240 pyalsaaudio-0.9.1/setup.cfg
--rwxr-xr-x   0 lars      (1000) lars      (1000)     1446 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/setup.py
--rwxr-xr-x   0 lars      (1000) lars      (1000)     4081 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.1/test.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.743096 pyalsaaudio-0.9.2/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2526 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.2/LICENSE
+-rw-r--r--   0 lars      (1000) lars      (1000)      137 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.2/MANIFEST.in
+-rw-r--r--   0 lars      (1000) lars      (1000)      951 2022-05-06 19:36:01.739096 pyalsaaudio-0.9.2/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     2335 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.2/README.md
+-rw-r--r--   0 lars      (1000) lars      (1000)      104 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.2/TODO
+-rw-r--r--   0 lars      (1000) lars      (1000)    86212 2022-05-06 19:28:47.000000 pyalsaaudio-0.9.2/alsaaudio.c
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.703095 pyalsaaudio-0.9.2/doc/
+-rw-r--r--   0 lars      (1000) lars      (1000)     2312 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.2/doc/Makefile
+-rw-r--r--   0 lars      (1000) lars      (1000)     4972 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.2/doc/conf.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.703095 pyalsaaudio-0.9.2/doc/gh-pages/
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.719095 pyalsaaudio-0.9.2/doc/gh-pages/_static/
+-rw-r--r--   0 lars      (1000) lars      (1000)      673 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/ajax-loader.gif
+-rw-r--r--   0 lars      (1000) lars      (1000)    11185 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/alabaster.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    14692 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/basic.css
+-rw-r--r--   0 lars      (1000) lars      (1000)      756 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/comment-bright.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      829 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/comment-close.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      641 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/comment.png
+-rw-r--r--   0 lars      (1000) lars      (1000)       42 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/custom.css
+-rw-r--r--   0 lars      (1000) lars      (1000)     4040 2017-07-09 11:44:11.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/default.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    10766 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/doctools.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      422 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/documentation_options.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      222 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/down-pressed.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      202 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/down.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      286 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/file.png
+-rw-r--r--   0 lars      (1000) lars      (1000)   263767 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery-3.1.0.js
+-rw-r--r--   0 lars      (1000) lars      (1000)   287630 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery-3.5.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    89476 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    10854 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/language_data.js
+-rw-r--r--   0 lars      (1000) lars      (1000)       90 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/minus.png
+-rw-r--r--   0 lars      (1000) lars      (1000)       90 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/plus.png
+-rw-r--r--   0 lars      (1000) lars      (1000)     4780 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/pygments.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    16634 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/searchtools.js
+-rw-r--r--   0 lars      (1000) lars      (1000)     4803 2017-07-09 11:44:11.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/sidebar.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    68420 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore-1.13.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    35168 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore-1.3.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    19530 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      214 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/up-pressed.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      203 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/up.png
+-rw-r--r--   0 lars      (1000) lars      (1000)    25351 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/_static/websupport.js
+-rw-r--r--   0 lars      (1000) lars      (1000)     9925 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/genindex.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     6191 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/index.html
+-rw-r--r--   0 lars      (1000) lars      (1000)    65554 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/libalsaaudio.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     3762 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/py-modindex.html
+-rw-r--r--   0 lars      (1000) lars      (1000)    10195 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/pyalsaaudio.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     3521 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/search.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     9587 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/searchindex.js
+-rw-r--r--   0 lars      (1000) lars      (1000)     7462 2022-05-06 19:34:15.000000 pyalsaaudio-0.9.2/doc/gh-pages/terminology.html
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.723096 pyalsaaudio-0.9.2/doc/html/
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.739096 pyalsaaudio-0.9.2/doc/html/_static/
+-rw-r--r--   0 lars      (1000) lars      (1000)      673 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/ajax-loader.gif
+-rw-r--r--   0 lars      (1000) lars      (1000)    11185 2022-05-06 19:34:14.000000 pyalsaaudio-0.9.2/doc/html/_static/alabaster.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    14692 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/_static/basic.css
+-rw-r--r--   0 lars      (1000) lars      (1000)      756 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/comment-bright.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      829 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/comment-close.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      641 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/comment.png
+-rw-r--r--   0 lars      (1000) lars      (1000)       42 2017-03-30 21:24:11.000000 pyalsaaudio-0.9.2/doc/html/_static/custom.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    10766 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/doctools.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      422 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/_static/documentation_options.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      222 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/down-pressed.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      202 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/down.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      286 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/file.png
+-rw-r--r--   0 lars      (1000) lars      (1000)   263767 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/jquery-3.1.0.js
+-rw-r--r--   0 lars      (1000) lars      (1000)   287630 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    89476 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/jquery.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    10854 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/_static/language_data.js
+-rw-r--r--   0 lars      (1000) lars      (1000)       90 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/minus.png
+-rw-r--r--   0 lars      (1000) lars      (1000)       90 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/plus.png
+-rw-r--r--   0 lars      (1000) lars      (1000)     4780 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/_static/pygments.css
+-rw-r--r--   0 lars      (1000) lars      (1000)    16634 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/searchtools.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    68420 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    35168 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 lars      (1000) lars      (1000)    19530 2022-05-03 19:06:16.000000 pyalsaaudio-0.9.2/doc/html/_static/underscore.js
+-rw-r--r--   0 lars      (1000) lars      (1000)      214 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/up-pressed.png
+-rw-r--r--   0 lars      (1000) lars      (1000)      203 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/up.png
+-rw-r--r--   0 lars      (1000) lars      (1000)    25351 2017-03-30 21:24:06.000000 pyalsaaudio-0.9.2/doc/html/_static/websupport.js
+-rw-r--r--   0 lars      (1000) lars      (1000)     9925 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/genindex.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     6191 2022-05-06 19:34:12.000000 pyalsaaudio-0.9.2/doc/html/index.html
+-rw-r--r--   0 lars      (1000) lars      (1000)    65554 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/libalsaaudio.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     3762 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/py-modindex.html
+-rw-r--r--   0 lars      (1000) lars      (1000)    10195 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/pyalsaaudio.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     3521 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/search.html
+-rw-r--r--   0 lars      (1000) lars      (1000)     9587 2022-05-06 19:34:14.000000 pyalsaaudio-0.9.2/doc/html/searchindex.js
+-rw-r--r--   0 lars      (1000) lars      (1000)     7462 2022-05-06 19:34:13.000000 pyalsaaudio-0.9.2/doc/html/terminology.html
+-rw-r--r--   0 lars      (1000) lars      (1000)      756 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.2/doc/index.rst
+-rw-r--r--   0 lars      (1000) lars      (1000)    25083 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/doc/libalsaaudio.rst
+-rw-r--r--   0 lars      (1000) lars      (1000)     4533 2019-03-27 13:45:59.000000 pyalsaaudio-0.9.2/doc/pyalsaaudio.rst
+-rw-r--r--   0 lars      (1000) lars      (1000)     3222 2017-07-09 11:44:22.000000 pyalsaaudio-0.9.2/doc/terminology.rst
+-rw-r--r--   0 lars      (1000) lars      (1000)     2712 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/isine.py
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     5270 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/mixertest.py
+-rw-r--r--   0 lars      (1000) lars      (1000)      540 2019-03-27 15:51:14.000000 pyalsaaudio-0.9.2/play_rusage.py
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     1412 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/playbacktest.py
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     1484 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/playwav.py
+drwxr-xr-x   0 lars      (1000) lars      (1000)        0 2022-05-06 19:36:01.739096 pyalsaaudio-0.9.2/pyalsaaudio.egg-info/
+-rw-r--r--   0 lars      (1000) lars      (1000)      951 2022-05-06 19:35:59.000000 pyalsaaudio-0.9.2/pyalsaaudio.egg-info/PKG-INFO
+-rw-r--r--   0 lars      (1000) lars      (1000)     2590 2022-05-06 19:36:01.000000 pyalsaaudio-0.9.2/pyalsaaudio.egg-info/SOURCES.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)        1 2022-05-06 19:35:59.000000 pyalsaaudio-0.9.2/pyalsaaudio.egg-info/dependency_links.txt
+-rw-r--r--   0 lars      (1000) lars      (1000)       10 2022-05-06 19:36:01.000000 pyalsaaudio-0.9.2/pyalsaaudio.egg-info/top_level.txt
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     1755 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/recordtest.py
+-rw-r--r--   0 lars      (1000) lars      (1000)       38 2022-05-06 19:36:01.743096 pyalsaaudio-0.9.2/setup.cfg
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     1446 2022-05-06 19:33:10.000000 pyalsaaudio-0.9.2/setup.py
+-rwxr-xr-x   0 lars      (1000) lars      (1000)     4081 2022-05-03 19:05:04.000000 pyalsaaudio-0.9.2/test.py
```

### Comparing `pyalsaaudio-0.9.1/LICENSE` & `pyalsaaudio-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/PKG-INFO` & `pyalsaaudio-0.9.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyalsaaudio
-Version: 0.9.1
+Version: 0.9.2
 Summary: ALSA bindings
 Home-page: http://larsimmisch.github.io/pyalsaaudio/
 Author: Casper Wilstrup
 Author-email: cwi@aves.dk
 Maintainer: Lars Immisch
 Maintainer-email: lars@ibp.de
 License: PSF
-Description: This package contains wrappers for accessing the ALSA API from Python.
-        It is fairly complete for PCM devices and Mixer access.
-        
 Platform: posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Mixers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+License-File: LICENSE
+
+This package contains wrappers for accessing the ALSA API from Python.
+It is fairly complete for PCM devices and Mixer access.
+
+
```

### Comparing `pyalsaaudio-0.9.1/README.md` & `pyalsaaudio-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/alsaaudio.c` & `pyalsaaudio-0.9.2/alsaaudio.c`

 * *Files 0% similar despite different names*

```diff
@@ -2411,17 +2411,17 @@
 
 	elem = alsamixer_find_elem(self->handle,self->controlname,self->controlid);
 
 	if (!pcmtypeobj || (pcmtypeobj == Py_None)) {
 		if (self->pchannels) {
 			pcmtype = SND_PCM_STREAM_PLAYBACK;
 		}
-	}
-	else {
-		pcmtype = SND_PCM_STREAM_CAPTURE;
+		else {
+			pcmtype = SND_PCM_STREAM_CAPTURE;
+		}
 	}
 
 	result = PyList_New(0);
 
 	for (channel = 0; channel <= SND_MIXER_SCHN_LAST; channel++) {
 		if (pcmtype == SND_PCM_STREAM_PLAYBACK &&
 			snd_mixer_selem_has_playback_channel(elem, channel))
```

### Comparing `pyalsaaudio-0.9.1/doc/Makefile` & `pyalsaaudio-0.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/conf.py` & `pyalsaaudio-0.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/ajax-loader.gif` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/alabaster.css` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/basic.css` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/comment-bright.png` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/comment-close.png` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/comment.png` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/comment.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/default.css` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/default.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/doctools.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery-3.1.0.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery-3.5.1.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/jquery.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/language_data.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/pygments.css` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/searchtools.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/sidebar.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore-1.13.1.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore-1.3.1.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/underscore.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/_static/websupport.js` & `pyalsaaudio-0.9.2/doc/gh-pages/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/genindex.html` & `pyalsaaudio-0.9.2/doc/gh-pages/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Index &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="#" />
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/index.html` & `pyalsaaudio-0.9.2/doc/gh-pages/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>alsaaudio documentation &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>alsaaudio documentation &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/libalsaaudio.html` & `pyalsaaudio-0.9.2/doc/gh-pages/libalsaaudio.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>alsaaudio &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>alsaaudio &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/py-modindex.html` & `pyalsaaudio-0.9.2/doc/gh-pages/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Python Module Index &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/pyalsaaudio.html` & `pyalsaaudio-0.9.2/doc/gh-pages/pyalsaaudio.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Introduction &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Introduction &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/search.html` & `pyalsaaudio-0.9.2/doc/gh-pages/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Search &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
```

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/searchindex.js` & `pyalsaaudio-0.9.2/doc/gh-pages/searchindex.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/gh-pages/terminology.html` & `pyalsaaudio-0.9.2/doc/gh-pages/terminology.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>PCM Terminology and Concepts &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>PCM Terminology and Concepts &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/ajax-loader.gif` & `pyalsaaudio-0.9.2/doc/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/alabaster.css` & `pyalsaaudio-0.9.2/doc/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/basic.css` & `pyalsaaudio-0.9.2/doc/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/comment-bright.png` & `pyalsaaudio-0.9.2/doc/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/comment-close.png` & `pyalsaaudio-0.9.2/doc/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/comment.png` & `pyalsaaudio-0.9.2/doc/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/doctools.js` & `pyalsaaudio-0.9.2/doc/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/jquery-3.1.0.js` & `pyalsaaudio-0.9.2/doc/html/_static/jquery-3.1.0.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/jquery-3.5.1.js` & `pyalsaaudio-0.9.2/doc/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/jquery.js` & `pyalsaaudio-0.9.2/doc/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/language_data.js` & `pyalsaaudio-0.9.2/doc/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/pygments.css` & `pyalsaaudio-0.9.2/doc/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/searchtools.js` & `pyalsaaudio-0.9.2/doc/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/underscore-1.13.1.js` & `pyalsaaudio-0.9.2/doc/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/underscore-1.3.1.js` & `pyalsaaudio-0.9.2/doc/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/underscore.js` & `pyalsaaudio-0.9.2/doc/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/_static/websupport.js` & `pyalsaaudio-0.9.2/doc/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/genindex.html` & `pyalsaaudio-0.9.2/doc/html/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Index &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="#" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/index.html` & `pyalsaaudio-0.9.2/doc/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>alsaaudio documentation &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>alsaaudio documentation &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/libalsaaudio.html` & `pyalsaaudio-0.9.2/doc/html/libalsaaudio.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>alsaaudio &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>alsaaudio &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/py-modindex.html` & `pyalsaaudio-0.9.2/doc/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Python Module Index &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/pyalsaaudio.html` & `pyalsaaudio-0.9.2/doc/html/pyalsaaudio.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>Introduction &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Introduction &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/html/search.html` & `pyalsaaudio-0.9.2/doc/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>Search &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
```

### Comparing `pyalsaaudio-0.9.1/doc/html/searchindex.js` & `pyalsaaudio-0.9.2/doc/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/html/terminology.html` & `pyalsaaudio-0.9.2/doc/html/terminology.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html>
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.17.1: http://docutils.sourceforge.net/" />
 
-    <title>PCM Terminology and Concepts &#8212; alsaaudio documentation 0.9.1 documentation</title>
+    <title>PCM Terminology and Concepts &#8212; alsaaudio documentation 0.9.2 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/alabaster.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/jquery.js"></script>
     <script src="_static/underscore.js"></script>
     <script src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
```

### Comparing `pyalsaaudio-0.9.1/doc/index.rst` & `pyalsaaudio-0.9.2/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/libalsaaudio.rst` & `pyalsaaudio-0.9.2/doc/libalsaaudio.rst`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/pyalsaaudio.rst` & `pyalsaaudio-0.9.2/doc/pyalsaaudio.rst`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/doc/terminology.rst` & `pyalsaaudio-0.9.2/doc/terminology.rst`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/isine.py` & `pyalsaaudio-0.9.2/isine.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/mixertest.py` & `pyalsaaudio-0.9.2/mixertest.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/play_rusage.py` & `pyalsaaudio-0.9.2/play_rusage.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/playbacktest.py` & `pyalsaaudio-0.9.2/playbacktest.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/playwav.py` & `pyalsaaudio-0.9.2/playwav.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/pyalsaaudio.egg-info/PKG-INFO` & `pyalsaaudio-0.9.2/pyalsaaudio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pyalsaaudio
-Version: 0.9.1
+Version: 0.9.2
 Summary: ALSA bindings
 Home-page: http://larsimmisch.github.io/pyalsaaudio/
 Author: Casper Wilstrup
 Author-email: cwi@aves.dk
 Maintainer: Lars Immisch
 Maintainer-email: lars@ibp.de
 License: PSF
-Description: This package contains wrappers for accessing the ALSA API from Python.
-        It is fairly complete for PCM devices and Mixer access.
-        
 Platform: posix
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Mixers
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: Topic :: Multimedia :: Sound/Audio :: Capture/Recording
+License-File: LICENSE
+
+This package contains wrappers for accessing the ALSA API from Python.
+It is fairly complete for PCM devices and Mixer access.
+
+
```

### Comparing `pyalsaaudio-0.9.1/pyalsaaudio.egg-info/SOURCES.txt` & `pyalsaaudio-0.9.2/pyalsaaudio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/recordtest.py` & `pyalsaaudio-0.9.2/recordtest.py`

 * *Files identical despite different names*

### Comparing `pyalsaaudio-0.9.1/setup.py` & `pyalsaaudio-0.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It is fairly complete for PCM devices and Mixer access.
 '''
 
 from setuptools import setup
 from setuptools.extension import Extension
 from sys import version
 
-pyalsa_version = '0.9.1'
+pyalsa_version = '0.9.2'
 
 if __name__ == '__main__':
     setup(
         name = 'pyalsaaudio',
         version = pyalsa_version,
         description = 'ALSA bindings',
         long_description = __doc__,
```

### Comparing `pyalsaaudio-0.9.1/test.py` & `pyalsaaudio-0.9.2/test.py`

 * *Files identical despite different names*

