# Comparing `tmp/smasunnyisland-0.44.tar.gz` & `tmp/smasunnyisland-0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smasunnyisland-0.44.tar", last modified: Thu May 30 08:00:50 2024, max compression
+gzip compressed data, was "smasunnyisland-0.45.tar", last modified: Thu May 30 08:05:15 2024, max compression
```

## Comparing `smasunnyisland-0.44.tar` & `smasunnyisland-0.45.tar`

### file list

```diff
@@ -1,214 +1,16 @@
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.577142 smasunnyisland-0.44/
--rw-r--r--   0 ton        (501) staff       (20)     1075 2024-05-30 05:57:21.000000 smasunnyisland-0.44/LICENSE
--rw-r--r--   0 ton        (501) staff       (20)       63 2024-05-30 07:46:56.000000 smasunnyisland-0.44/MANIFEST.in
--rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 08:00:50.576897 smasunnyisland-0.44/PKG-INFO
--rw-r--r--   0 ton        (501) staff       (20)     1549 2024-05-30 06:55:14.000000 smasunnyisland-0.44/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.576587 smasunnyisland-0.44/SMASunnyIsland.egg-info/
--rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/PKG-INFO
--rw-r--r--   0 ton        (501) staff       (20)     9245 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/SOURCES.txt
--rw-r--r--   0 ton        (501) staff       (20)        1 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/dependency_links.txt
--rw-r--r--   0 ton        (501) staff       (20)       25 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/requires.txt
--rw-r--r--   0 ton        (501) staff       (20)       15 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/top_level.txt
--rw-r--r--   0 ton        (501) staff       (20)      726 2024-05-30 08:00:46.000000 smasunnyisland-0.44/pyproject.toml
--rw-r--r--   0 ton        (501) staff       (20)       38 2024-05-30 08:00:50.577182 smasunnyisland-0.44/setup.cfg
--rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:35:47.000000 smasunnyisland-0.44/setup.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.542448 smasunnyisland-0.44/smasunnyisland/
--rw-r--r--   0 ton        (501) staff       (20)       48 2024-05-30 06:53:20.000000 smasunnyisland-0.44/smasunnyisland/__init__.py
--rw-r--r--   0 ton        (501) staff       (20)     6757 2024-05-30 08:00:38.000000 smasunnyisland-0.44/smasunnyisland/sma_controller.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.539110 smasunnyisland-0.44/vendor/
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.544277 smasunnyisland-0.44/vendor/pysunspec/
--rw-r--r--   0 ton        (501) staff       (20)       44 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.git
--rw-r--r--   0 ton        (501) staff       (20)      969 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.gitignore
--rw-r--r--   0 ton        (501) staff       (20)       97 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.gitmodules
--rw-r--r--   0 ton        (501) staff       (20)      247 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.travis.yml
--rw-r--r--   0 ton        (501) staff       (20)     3050 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/CHANGES.txt
--rw-r--r--   0 ton        (501) staff       (20)     1062 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/LICENSE
--rw-r--r--   0 ton        (501) staff       (20)     6627 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.545646 smasunnyisland-0.44/vendor/pysunspec/doc/
--rw-r--r--   0 ton        (501) staff       (20)     6774 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/Makefile
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549088 smasunnyisland-0.44/vendor/pysunspec/doc/_static/
--rw-r--r--   0 ton        (501) staff       (20)      673 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/ajax-loader.gif
--rw-r--r--   0 ton        (501) staff       (20)     8463 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/basic.css
--rw-r--r--   0 ton        (501) staff       (20)     3500 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-bright.png
--rw-r--r--   0 ton        (501) staff       (20)     3578 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-close.png
--rw-r--r--   0 ton        (501) staff       (20)     3445 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment.png
--rw-r--r--   0 ton        (501) staff       (20)     4040 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/default.css
--rw-r--r--   0 ton        (501) staff       (20)     6620 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/doctools.js
--rw-r--r--   0 ton        (501) staff       (20)      368 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/down-pressed.png
--rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/down.png
--rw-r--r--   0 ton        (501) staff       (20)      392 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/file.png
--rw-r--r--   0 ton        (501) staff       (20)    93636 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/jquery.js
--rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/minus.png
--rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/plus.png
--rw-r--r--   0 ton        (501) staff       (20)     3932 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/pygments.css
--rw-r--r--   0 ton        (501) staff       (20)    17844 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/searchtools.js
--rw-r--r--   0 ton        (501) staff       (20)     4803 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/sidebar.js
--rw-r--r--   0 ton        (501) staff       (20)    12140 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/underscore.js
--rw-r--r--   0 ton        (501) staff       (20)      372 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/up-pressed.png
--rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/up.png
--rw-r--r--   0 ton        (501) staff       (20)    25246 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/websupport.js
--rw-r--r--   0 ton        (501) staff       (20)     8295 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/conf.py
--rw-r--r--   0 ton        (501) staff       (20)      463 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/index.rst
--rw-r--r--   0 ton        (501) staff       (20)     6465 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/make.bat
--rw-r--r--   0 ton        (501) staff       (20)    13217 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec.rst
--rw-r--r--   0 ton        (501) staff       (20)     8858 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec_api.rst
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549416 smasunnyisland-0.44/vendor/pysunspec/scripts/
--rw-r--r--   0 ton        (501) staff       (20)      725 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/scripts/pysunspec_coverage_report.py
--rw-r--r--   0 ton        (501) staff       (20)     4872 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/scripts/suns.py
--rw-r--r--   0 ton        (501) staff       (20)     1300 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/setup.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549563 smasunnyisland-0.44/vendor/pysunspec/sunspec/
--rw-r--r--   0 ton        (501) staff       (20)       41 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549721 smasunnyisland-0.44/vendor/pysunspec/sunspec/__pycache__/
--rw-r--r--   0 ton        (501) staff       (20)      223 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.551140 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.551581 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/
--rw-r--r--   0 ton        (501) staff       (20)      210 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ton        (501) staff       (20)    37799 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/client.cpython-311.pyc
--rwxr-xr-x   0 ton        (501) staff       (20)    30669 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/client.py
--rw-r--r--   0 ton        (501) staff       (20)     9525 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/data.py
--rw-r--r--   0 ton        (501) staff       (20)    50822 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/device.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.552302 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/__init__.py
--rwxr-xr-x   0 ton        (501) staff       (20)    34177 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/client.py
--rw-r--r--   0 ton        (501) staff       (20)    20936 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/mbmap.py
--rw-r--r--   0 ton        (501) staff       (20)     2189 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/pics.py
--rw-r--r--   0 ton        (501) staff       (20)     4125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/smdx.py
--rw-r--r--   0 ton        (501) staff       (20)     6808 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/suns.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.553856 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556276 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/
--rw-r--r--   0 ton        (501) staff       (20)    16406 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1.xml
--rw-r--r--   0 ton        (501) staff       (20)    16290 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_a.xml
--rw-r--r--   0 ton        (501) staff       (20)    15978 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_b.xml
--rw-r--r--   0 ton        (501) staff       (20)    12196 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_c.xml
--rw-r--r--   0 ton        (501) staff       (20)    12203 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_d.xml
--rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_processed.xml
--rw-r--r--   0 ton        (501) staff       (20)      647 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_2.xml
--rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_3.xml
--rw-r--r--   0 ton        (501) staff       (20)     5432 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     9354 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_2.xml
--rw-r--r--   0 ton        (501) staff       (20)    17198 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_3.xml
--rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_2.xml
--rw-r--r--   0 ton        (501) staff       (20)     3159 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     1422 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_2.xml
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556701 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/__init__.py
--rw-r--r--   0 ton        (501) staff       (20)     2485 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/serial.py
--rw-r--r--   0 ton        (501) staff       (20)     2049 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/socket.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556858 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/models/
--rw-r--r--   0 ton        (501) staff       (20)      479 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/models/smdx_65000.xml
--rw-r--r--   0 ton        (501) staff       (20)     2674 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_all.py
--rw-r--r--   0 ton        (501) staff       (20)     7939 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_client.py
--rw-r--r--   0 ton        (501) staff       (20)     2117 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_data.py
--rw-r--r--   0 ton        (501) staff       (20)    21372 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_device.py
--rw-r--r--   0 ton        (501) staff       (20)     3834 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_client.py
--rw-r--r--   0 ton        (501) staff       (20)     4479 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_mbmap.py
--rw-r--r--   0 ton        (501) staff       (20)     6189 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_util.py
--rw-r--r--   0 ton        (501) staff       (20)     7558 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/util.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.557887 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/
--rw-r--r--   0 ton        (501) staff       (20)       73 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.git
--rw-r--r--   0 ton        (501) staff       (20)      483 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.gitattributes
--rw-r--r--   0 ton        (501) staff       (20)     2643 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.gitignore
--rw-r--r--   0 ton        (501) staff       (20)      141 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.travis.yml
--rw-r--r--   0 ton        (501) staff       (20)      112 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.576284 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/
--rw-r--r--   0 ton        (501) staff       (20)     5099 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/CHANGELOG
--rw-r--r--   0 ton        (501) staff       (20)     1958 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/Makefile
--rw-r--r--   0 ton        (501) staff       (20)     5679 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.py
--rw-r--r--   0 ton        (501) staff       (20)     6780 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.xml
--rw-r--r--   0 ton        (501) staff       (20)       32 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.xml.md5
--rw-r--r--   0 ton        (501) staff       (20)     7076 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx.xsd
--rw-r--r--   0 ton        (501) staff       (20)     1914 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00001.xml
--rw-r--r--   0 ton        (501) staff       (20)     4107 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00002.xml
--rw-r--r--   0 ton        (501) staff       (20)     7457 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00003.xml
--rw-r--r--   0 ton        (501) staff       (20)     9120 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00004.xml
--rw-r--r--   0 ton        (501) staff       (20)    10097 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00005.xml
--rw-r--r--   0 ton        (501) staff       (20)    10295 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00006.xml
--rw-r--r--   0 ton        (501) staff       (20)     4994 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00007.xml
--rw-r--r--   0 ton        (501) staff       (20)     1319 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00008.xml
--rw-r--r--   0 ton        (501) staff       (20)    11522 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00009.xml
--rw-r--r--   0 ton        (501) staff       (20)     2628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00010.xml
--rw-r--r--   0 ton        (501) staff       (20)     4729 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00011.xml
--rw-r--r--   0 ton        (501) staff       (20)     7692 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00012.xml
--rw-r--r--   0 ton        (501) staff       (20)     7716 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00013.xml
--rw-r--r--   0 ton        (501) staff       (20)     2781 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00014.xml
--rw-r--r--   0 ton        (501) staff       (20)     3151 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00015.xml
--rw-r--r--   0 ton        (501) staff       (20)     4476 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00016.xml
--rw-r--r--   0 ton        (501) staff       (20)     4776 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00017.xml
--rw-r--r--   0 ton        (501) staff       (20)     1468 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00018.xml
--rw-r--r--   0 ton        (501) staff       (20)     4418 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00019.xml
--rw-r--r--   0 ton        (501) staff       (20)    12770 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00101.xml
--rw-r--r--   0 ton        (501) staff       (20)    12834 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00102.xml
--rw-r--r--   0 ton        (501) staff       (20)    12883 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00103.xml
--rw-r--r--   0 ton        (501) staff       (20)    11866 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00111.xml
--rw-r--r--   0 ton        (501) staff       (20)    11895 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00112.xml
--rw-r--r--   0 ton        (501) staff       (20)    11964 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00113.xml
--rw-r--r--   0 ton        (501) staff       (20)     7816 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00120.xml
--rw-r--r--   0 ton        (501) staff       (20)     9437 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00121.xml
--rw-r--r--   0 ton        (501) staff       (20)     7499 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00122.xml
--rw-r--r--   0 ton        (501) staff       (20)     8208 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00123.xml
--rw-r--r--   0 ton        (501) staff       (20)     7583 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00124.xml
--rw-r--r--   0 ton        (501) staff       (20)     3496 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00125.xml
--rw-r--r--   0 ton        (501) staff       (20)    14940 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00126.xml
--rw-r--r--   0 ton        (501) staff       (20)     3450 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00127.xml
--rw-r--r--   0 ton        (501) staff       (20)     4848 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00128.xml
--rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00129.xml
--rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00130.xml
--rw-r--r--   0 ton        (501) staff       (20)    14955 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00131.xml
--rw-r--r--   0 ton        (501) staff       (20)    15233 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00132.xml
--rw-r--r--   0 ton        (501) staff       (20)    11710 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00133.xml
--rw-r--r--   0 ton        (501) staff       (20)    16249 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00134.xml
--rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00135.xml
--rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00136.xml
--rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00137.xml
--rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00138.xml
--rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00139.xml
--rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00140.xml
--rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00141.xml
--rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00142.xml
--rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00143.xml
--rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00144.xml
--rw-r--r--   0 ton        (501) staff       (20)     2810 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00145.xml
--rw-r--r--   0 ton        (501) staff       (20)    13998 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00160.xml
--rw-r--r--   0 ton        (501) staff       (20)    20615 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00201.xml
--rw-r--r--   0 ton        (501) staff       (20)    21089 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00202.xml
--rw-r--r--   0 ton        (501) staff       (20)    21145 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00203.xml
--rw-r--r--   0 ton        (501) staff       (20)    21095 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00204.xml
--rw-r--r--   0 ton        (501) staff       (20)    18870 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00211.xml
--rw-r--r--   0 ton        (501) staff       (20)    18973 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00212.xml
--rw-r--r--   0 ton        (501) staff       (20)    19047 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00213.xml
--rw-r--r--   0 ton        (501) staff       (20)    18980 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00214.xml
--rw-r--r--   0 ton        (501) staff       (20)    12093 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00220.xml
--rw-r--r--   0 ton        (501) staff       (20)     1483 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00302.xml
--rw-r--r--   0 ton        (501) staff       (20)      709 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00303.xml
--rw-r--r--   0 ton        (501) staff       (20)     1078 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00304.xml
--rw-r--r--   0 ton        (501) staff       (20)     1823 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00305.xml
--rw-r--r--   0 ton        (501) staff       (20)     1313 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00306.xml
--rw-r--r--   0 ton        (501) staff       (20)     2521 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00307.xml
--rw-r--r--   0 ton        (501) staff       (20)     1260 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00308.xml
--rw-r--r--   0 ton        (501) staff       (20)     5426 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00401.xml
--rw-r--r--   0 ton        (501) staff       (20)     7223 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00402.xml
--rw-r--r--   0 ton        (501) staff       (20)     5727 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00403.xml
--rw-r--r--   0 ton        (501) staff       (20)     8177 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00404.xml
--rw-r--r--   0 ton        (501) staff       (20)    10768 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00501.xml
--rw-r--r--   0 ton        (501) staff       (20)    11574 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00502.xml
--rw-r--r--   0 ton        (501) staff       (20)     9121 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00601.xml
--rw-r--r--   0 ton        (501) staff       (20)      638 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00801.xml
--rw-r--r--   0 ton        (501) staff       (20)    31467 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00802.xml
--rw-r--r--   0 ton        (501) staff       (20)    32797 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00803.xml
--rw-r--r--   0 ton        (501) staff       (20)    31777 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00804.xml
--rw-r--r--   0 ton        (501) staff       (20)     7846 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00805.xml
--rw-r--r--   0 ton        (501) staff       (20)      850 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00806.xml
--rw-r--r--   0 ton        (501) staff       (20)    42745 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00807.xml
--rw-r--r--   0 ton        (501) staff       (20)      858 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00808.xml
--rw-r--r--   0 ton        (501) staff       (20)      848 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00809.xml
--rw-r--r--   0 ton        (501) staff       (20)     5185 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63001.xml
--rw-r--r--   0 ton        (501) staff       (20)      559 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63002.xml
--rw-r--r--   0 ton        (501) staff       (20)     6862 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64001.xml
--rw-r--r--   0 ton        (501) staff       (20)     7909 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64020.xml
--rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64101.xml
--rw-r--r--   0 ton        (501) staff       (20)    12153 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64110.xml
--rw-r--r--   0 ton        (501) staff       (20)     5688 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64111.xml
--rw-r--r--   0 ton        (501) staff       (20)    21312 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64112.xml
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:05:15.162580 smasunnyisland-0.45/
+-rw-r--r--   0 ton        (501) staff       (20)     1075 2024-05-30 05:57:21.000000 smasunnyisland-0.45/LICENSE
+-rw-r--r--   0 ton        (501) staff       (20)     2333 2024-05-30 08:05:15.162354 smasunnyisland-0.45/PKG-INFO
+-rw-r--r--   0 ton        (501) staff       (20)     1549 2024-05-30 06:55:14.000000 smasunnyisland-0.45/README.md
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:05:15.162094 smasunnyisland-0.45/SMASunnyIsland.egg-info/
+-rw-r--r--   0 ton        (501) staff       (20)     2333 2024-05-30 08:05:15.000000 smasunnyisland-0.45/SMASunnyIsland.egg-info/PKG-INFO
+-rw-r--r--   0 ton        (501) staff       (20)      290 2024-05-30 08:05:15.000000 smasunnyisland-0.45/SMASunnyIsland.egg-info/SOURCES.txt
+-rw-r--r--   0 ton        (501) staff       (20)        1 2024-05-30 08:05:15.000000 smasunnyisland-0.45/SMASunnyIsland.egg-info/dependency_links.txt
+-rw-r--r--   0 ton        (501) staff       (20)       42 2024-05-30 08:05:15.000000 smasunnyisland-0.45/SMASunnyIsland.egg-info/requires.txt
+-rw-r--r--   0 ton        (501) staff       (20)       15 2024-05-30 08:05:15.000000 smasunnyisland-0.45/SMASunnyIsland.egg-info/top_level.txt
+-rw-r--r--   0 ton        (501) staff       (20)      748 2024-05-30 08:04:59.000000 smasunnyisland-0.45/pyproject.toml
+-rw-r--r--   0 ton        (501) staff       (20)       38 2024-05-30 08:05:15.162622 smasunnyisland-0.45/setup.cfg
+-rw-r--r--   0 ton        (501) staff       (20)      623 2024-05-30 08:03:49.000000 smasunnyisland-0.45/setup.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:05:15.161732 smasunnyisland-0.45/smasunnyisland/
+-rw-r--r--   0 ton        (501) staff       (20)       48 2024-05-30 06:53:20.000000 smasunnyisland-0.45/smasunnyisland/__init__.py
+-rw-r--r--   0 ton        (501) staff       (20)     6739 2024-05-30 08:04:37.000000 smasunnyisland-0.45/smasunnyisland/sma_controller.py
```

### Comparing `smasunnyisland-0.44/LICENSE` & `smasunnyisland-0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.44/PKG-INFO` & `smasunnyisland-0.45/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: SMASunnyIsland
-Version: 0.44
+Version: 0.45
 Summary: A Python library for controlling SMA Sunny Island inverters
 Home-page: https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Author: Harm van den Brink
 Author-email: Harm van den Brink <harmvandenbrink@gmail.com>
 Project-URL: Homepage, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Project-URL: Issues, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: pymodbus==2.5.3
+Requires-Dist: pysunspec==2.1.1
 
 # SMA Sunny Island Controller
 A controller to read out and send commands to a SMA Sunny Island battery inverter. SUNNY ISLAND 4.4M / 6.0H / 8.0H 
 
 This code was used in a home built Home Energy Management System (HEMS), to include a battery into a smart home. You can read more about it in my blog post: [How I built a HEMS with solar, a battery and a charge station (in Python)](https://medium.com/@harmvandenbrink/how-i-built-a-hems-with-solar-a-battery-and-a-charge-station-in-python-d5b51e60fd1c?source=friends_link&sk=f5e9302a02ea29065c3f677ecf1b8ed8)
 
 # How to use the code
```

### Comparing `smasunnyisland-0.44/README.md` & `smasunnyisland-0.45/README.md`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.44/SMASunnyIsland.egg-info/PKG-INFO` & `smasunnyisland-0.45/SMASunnyIsland.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: SMASunnyIsland
-Version: 0.44
+Version: 0.45
 Summary: A Python library for controlling SMA Sunny Island inverters
 Home-page: https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Author: Harm van den Brink
 Author-email: Harm van den Brink <harmvandenbrink@gmail.com>
 Project-URL: Homepage, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Project-URL: Issues, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pyserial
 Requires-Dist: pymodbus==2.5.3
+Requires-Dist: pysunspec==2.1.1
 
 # SMA Sunny Island Controller
 A controller to read out and send commands to a SMA Sunny Island battery inverter. SUNNY ISLAND 4.4M / 6.0H / 8.0H 
 
 This code was used in a home built Home Energy Management System (HEMS), to include a battery into a smart home. You can read more about it in my blog post: [How I built a HEMS with solar, a battery and a charge station (in Python)](https://medium.com/@harmvandenbrink/how-i-built-a-hems-with-solar-a-battery-and-a-charge-station-in-python-d5b51e60fd1c?source=friends_link&sk=f5e9302a02ea29065c3f677ecf1b8ed8)
 
 # How to use the code
```

### Comparing `smasunnyisland-0.44/pyproject.toml` & `smasunnyisland-0.45/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [project]
 name = "SMASunnyIsland"
-version = "0.44"
+version = "0.45"
 authors = [
   { name="Harm van den Brink", email="harmvandenbrink@gmail.com" },
 ]
 description = "A Python library for controlling SMA Sunny Island inverters"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'pyserial',
   'pymodbus==2.5.3',
+  'pysunspec==2.1.1',
 ]
 
 [project.urls]
 Homepage = "https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller"
 Issues = "https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller/issues"
 
 [build-system]
```

### Comparing `smasunnyisland-0.44/smasunnyisland/sma_controller.py` & `smasunnyisland-0.45/smasunnyisland/sma_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 __author__ = "Harm van den Brink"
 __email__ = "harmvandenbrink@gmail.com"
 __license__ = "MIT License"
 
 __version__ = "1.42"
 __status__ = "Production"
 
-from .vendor.pysunspec.sunspec.core import client as clientSunspec
+from sunspec.core import client as clientSunspec
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder
 from pymodbus.client.sync import ModbusTcpClient as ModbusClient
 from collections import OrderedDict
 
 
 class SMASunnyIslandClient:
```

