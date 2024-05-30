# Comparing `tmp/smasunnyisland-0.43.tar.gz` & `tmp/smasunnyisland-0.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smasunnyisland-0.43.tar", last modified: Thu May 30 07:59:24 2024, max compression
+gzip compressed data, was "smasunnyisland-0.44.tar", last modified: Thu May 30 08:00:50 2024, max compression
```

## Comparing `smasunnyisland-0.43.tar` & `smasunnyisland-0.44.tar`

### file list

```diff
@@ -1,214 +1,214 @@
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.515323 smasunnyisland-0.43/
--rw-r--r--   0 ton        (501) staff       (20)     1075 2024-05-30 05:57:21.000000 smasunnyisland-0.43/LICENSE
--rw-r--r--   0 ton        (501) staff       (20)       63 2024-05-30 07:46:56.000000 smasunnyisland-0.43/MANIFEST.in
--rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 07:59:24.515108 smasunnyisland-0.43/PKG-INFO
--rw-r--r--   0 ton        (501) staff       (20)     1549 2024-05-30 06:55:14.000000 smasunnyisland-0.43/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.514854 smasunnyisland-0.43/SMASunnyIsland.egg-info/
--rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 07:59:24.000000 smasunnyisland-0.43/SMASunnyIsland.egg-info/PKG-INFO
--rw-r--r--   0 ton        (501) staff       (20)     9245 2024-05-30 07:59:24.000000 smasunnyisland-0.43/SMASunnyIsland.egg-info/SOURCES.txt
--rw-r--r--   0 ton        (501) staff       (20)        1 2024-05-30 07:59:24.000000 smasunnyisland-0.43/SMASunnyIsland.egg-info/dependency_links.txt
--rw-r--r--   0 ton        (501) staff       (20)       25 2024-05-30 07:59:24.000000 smasunnyisland-0.43/SMASunnyIsland.egg-info/requires.txt
--rw-r--r--   0 ton        (501) staff       (20)       15 2024-05-30 07:59:24.000000 smasunnyisland-0.43/SMASunnyIsland.egg-info/top_level.txt
--rw-r--r--   0 ton        (501) staff       (20)      726 2024-05-30 07:59:17.000000 smasunnyisland-0.43/pyproject.toml
--rw-r--r--   0 ton        (501) staff       (20)       38 2024-05-30 07:59:24.515359 smasunnyisland-0.43/setup.cfg
--rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:35:47.000000 smasunnyisland-0.43/setup.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.479885 smasunnyisland-0.43/smasunnyisland/
--rw-r--r--   0 ton        (501) staff       (20)       48 2024-05-30 06:53:20.000000 smasunnyisland-0.43/smasunnyisland/__init__.py
--rw-r--r--   0 ton        (501) staff       (20)     6758 2024-05-30 07:59:07.000000 smasunnyisland-0.43/smasunnyisland/sma_controller.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.475086 smasunnyisland-0.43/vendor/
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.482833 smasunnyisland-0.43/vendor/pysunspec/
--rw-r--r--   0 ton        (501) staff       (20)       44 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/.git
--rw-r--r--   0 ton        (501) staff       (20)      969 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/.gitignore
--rw-r--r--   0 ton        (501) staff       (20)       97 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/.gitmodules
--rw-r--r--   0 ton        (501) staff       (20)      247 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/.travis.yml
--rw-r--r--   0 ton        (501) staff       (20)     3050 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/CHANGES.txt
--rw-r--r--   0 ton        (501) staff       (20)     1062 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/LICENSE
--rw-r--r--   0 ton        (501) staff       (20)     6627 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.484141 smasunnyisland-0.43/vendor/pysunspec/doc/
--rw-r--r--   0 ton        (501) staff       (20)     6774 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/Makefile
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.487572 smasunnyisland-0.43/vendor/pysunspec/doc/_static/
--rw-r--r--   0 ton        (501) staff       (20)      673 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/ajax-loader.gif
--rw-r--r--   0 ton        (501) staff       (20)     8463 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/basic.css
--rw-r--r--   0 ton        (501) staff       (20)     3500 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment-bright.png
--rw-r--r--   0 ton        (501) staff       (20)     3578 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment-close.png
--rw-r--r--   0 ton        (501) staff       (20)     3445 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment.png
--rw-r--r--   0 ton        (501) staff       (20)     4040 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/default.css
--rw-r--r--   0 ton        (501) staff       (20)     6620 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/doctools.js
--rw-r--r--   0 ton        (501) staff       (20)      368 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/down-pressed.png
--rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/down.png
--rw-r--r--   0 ton        (501) staff       (20)      392 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/file.png
--rw-r--r--   0 ton        (501) staff       (20)    93636 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/jquery.js
--rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/minus.png
--rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/plus.png
--rw-r--r--   0 ton        (501) staff       (20)     3932 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/pygments.css
--rw-r--r--   0 ton        (501) staff       (20)    17844 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/searchtools.js
--rw-r--r--   0 ton        (501) staff       (20)     4803 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/sidebar.js
--rw-r--r--   0 ton        (501) staff       (20)    12140 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/underscore.js
--rw-r--r--   0 ton        (501) staff       (20)      372 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/up-pressed.png
--rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/up.png
--rw-r--r--   0 ton        (501) staff       (20)    25246 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/_static/websupport.js
--rw-r--r--   0 ton        (501) staff       (20)     8295 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/conf.py
--rw-r--r--   0 ton        (501) staff       (20)      463 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/index.rst
--rw-r--r--   0 ton        (501) staff       (20)     6465 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/make.bat
--rw-r--r--   0 ton        (501) staff       (20)    13217 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/pysunspec.rst
--rw-r--r--   0 ton        (501) staff       (20)     8858 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/doc/pysunspec_api.rst
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.487960 smasunnyisland-0.43/vendor/pysunspec/scripts/
--rw-r--r--   0 ton        (501) staff       (20)      725 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/scripts/pysunspec_coverage_report.py
--rw-r--r--   0 ton        (501) staff       (20)     4872 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/scripts/suns.py
--rw-r--r--   0 ton        (501) staff       (20)     1300 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/setup.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.488160 smasunnyisland-0.43/vendor/pysunspec/sunspec/
--rw-r--r--   0 ton        (501) staff       (20)       41 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.488355 smasunnyisland-0.43/vendor/pysunspec/sunspec/__pycache__/
--rw-r--r--   0 ton        (501) staff       (20)      223 2024-05-30 07:53:38.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.489920 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.490397 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/__pycache__/
--rw-r--r--   0 ton        (501) staff       (20)      210 2024-05-30 07:53:38.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 ton        (501) staff       (20)    37799 2024-05-30 07:53:38.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/__pycache__/client.cpython-311.pyc
--rwxr-xr-x   0 ton        (501) staff       (20)    30669 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/client.py
--rw-r--r--   0 ton        (501) staff       (20)     9525 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/data.py
--rw-r--r--   0 ton        (501) staff       (20)    50822 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/device.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.491190 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/__init__.py
--rwxr-xr-x   0 ton        (501) staff       (20)    34177 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/client.py
--rw-r--r--   0 ton        (501) staff       (20)    20936 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/mbmap.py
--rw-r--r--   0 ton        (501) staff       (20)     2189 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/pics.py
--rw-r--r--   0 ton        (501) staff       (20)     4125 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/smdx.py
--rw-r--r--   0 ton        (501) staff       (20)     6808 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/suns.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.492714 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/__init__.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.495539 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/
--rw-r--r--   0 ton        (501) staff       (20)    16406 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1.xml
--rw-r--r--   0 ton        (501) staff       (20)    16290 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_a.xml
--rw-r--r--   0 ton        (501) staff       (20)    15978 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_b.xml
--rw-r--r--   0 ton        (501) staff       (20)    12196 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_c.xml
--rw-r--r--   0 ton        (501) staff       (20)    12203 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_d.xml
--rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_processed.xml
--rw-r--r--   0 ton        (501) staff       (20)      647 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_2.xml
--rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_3.xml
--rw-r--r--   0 ton        (501) staff       (20)     5432 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     9354 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_2.xml
--rw-r--r--   0 ton        (501) staff       (20)    17198 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_3.xml
--rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_2.xml
--rw-r--r--   0 ton        (501) staff       (20)     3159 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_1.xml
--rw-r--r--   0 ton        (501) staff       (20)     1422 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_2.xml
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.495947 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/
--rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/__init__.py
--rw-r--r--   0 ton        (501) staff       (20)     2485 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/serial.py
--rw-r--r--   0 ton        (501) staff       (20)     2049 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/socket.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.496112 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/models/
--rw-r--r--   0 ton        (501) staff       (20)      479 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/models/smdx_65000.xml
--rw-r--r--   0 ton        (501) staff       (20)     2674 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_all.py
--rw-r--r--   0 ton        (501) staff       (20)     7939 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_client.py
--rw-r--r--   0 ton        (501) staff       (20)     2117 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_data.py
--rw-r--r--   0 ton        (501) staff       (20)    21372 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_device.py
--rw-r--r--   0 ton        (501) staff       (20)     3834 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_modbus_client.py
--rw-r--r--   0 ton        (501) staff       (20)     4479 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_modbus_mbmap.py
--rw-r--r--   0 ton        (501) staff       (20)     6189 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_util.py
--rw-r--r--   0 ton        (501) staff       (20)     7558 2024-05-30 07:09:54.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/core/util.py
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.497134 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/
--rw-r--r--   0 ton        (501) staff       (20)       73 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/.git
--rw-r--r--   0 ton        (501) staff       (20)      483 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/.gitattributes
--rw-r--r--   0 ton        (501) staff       (20)     2643 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/.gitignore
--rw-r--r--   0 ton        (501) staff       (20)      141 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/.travis.yml
--rw-r--r--   0 ton        (501) staff       (20)      112 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/README.md
-drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 07:59:24.514581 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/
--rw-r--r--   0 ton        (501) staff       (20)     5099 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/CHANGELOG
--rw-r--r--   0 ton        (501) staff       (20)     1958 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/Makefile
--rw-r--r--   0 ton        (501) staff       (20)     5679 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/manifest.py
--rw-r--r--   0 ton        (501) staff       (20)     6780 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/manifest.xml
--rw-r--r--   0 ton        (501) staff       (20)       32 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/manifest.xml.md5
--rw-r--r--   0 ton        (501) staff       (20)     7076 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx.xsd
--rw-r--r--   0 ton        (501) staff       (20)     1914 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00001.xml
--rw-r--r--   0 ton        (501) staff       (20)     4107 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00002.xml
--rw-r--r--   0 ton        (501) staff       (20)     7457 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00003.xml
--rw-r--r--   0 ton        (501) staff       (20)     9120 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00004.xml
--rw-r--r--   0 ton        (501) staff       (20)    10097 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00005.xml
--rw-r--r--   0 ton        (501) staff       (20)    10295 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00006.xml
--rw-r--r--   0 ton        (501) staff       (20)     4994 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00007.xml
--rw-r--r--   0 ton        (501) staff       (20)     1319 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00008.xml
--rw-r--r--   0 ton        (501) staff       (20)    11522 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00009.xml
--rw-r--r--   0 ton        (501) staff       (20)     2628 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00010.xml
--rw-r--r--   0 ton        (501) staff       (20)     4729 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00011.xml
--rw-r--r--   0 ton        (501) staff       (20)     7692 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00012.xml
--rw-r--r--   0 ton        (501) staff       (20)     7716 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00013.xml
--rw-r--r--   0 ton        (501) staff       (20)     2781 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00014.xml
--rw-r--r--   0 ton        (501) staff       (20)     3151 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00015.xml
--rw-r--r--   0 ton        (501) staff       (20)     4476 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00016.xml
--rw-r--r--   0 ton        (501) staff       (20)     4776 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00017.xml
--rw-r--r--   0 ton        (501) staff       (20)     1468 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00018.xml
--rw-r--r--   0 ton        (501) staff       (20)     4418 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00019.xml
--rw-r--r--   0 ton        (501) staff       (20)    12770 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00101.xml
--rw-r--r--   0 ton        (501) staff       (20)    12834 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00102.xml
--rw-r--r--   0 ton        (501) staff       (20)    12883 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00103.xml
--rw-r--r--   0 ton        (501) staff       (20)    11866 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00111.xml
--rw-r--r--   0 ton        (501) staff       (20)    11895 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00112.xml
--rw-r--r--   0 ton        (501) staff       (20)    11964 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00113.xml
--rw-r--r--   0 ton        (501) staff       (20)     7816 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00120.xml
--rw-r--r--   0 ton        (501) staff       (20)     9437 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00121.xml
--rw-r--r--   0 ton        (501) staff       (20)     7499 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00122.xml
--rw-r--r--   0 ton        (501) staff       (20)     8208 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00123.xml
--rw-r--r--   0 ton        (501) staff       (20)     7583 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00124.xml
--rw-r--r--   0 ton        (501) staff       (20)     3496 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00125.xml
--rw-r--r--   0 ton        (501) staff       (20)    14940 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00126.xml
--rw-r--r--   0 ton        (501) staff       (20)     3450 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00127.xml
--rw-r--r--   0 ton        (501) staff       (20)     4848 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00128.xml
--rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00129.xml
--rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00130.xml
--rw-r--r--   0 ton        (501) staff       (20)    14955 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00131.xml
--rw-r--r--   0 ton        (501) staff       (20)    15233 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00132.xml
--rw-r--r--   0 ton        (501) staff       (20)    11710 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00133.xml
--rw-r--r--   0 ton        (501) staff       (20)    16249 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00134.xml
--rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00135.xml
--rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00136.xml
--rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00137.xml
--rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00138.xml
--rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00139.xml
--rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00140.xml
--rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00141.xml
--rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00142.xml
--rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00143.xml
--rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00144.xml
--rw-r--r--   0 ton        (501) staff       (20)     2810 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00145.xml
--rw-r--r--   0 ton        (501) staff       (20)    13998 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00160.xml
--rw-r--r--   0 ton        (501) staff       (20)    20615 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00201.xml
--rw-r--r--   0 ton        (501) staff       (20)    21089 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00202.xml
--rw-r--r--   0 ton        (501) staff       (20)    21145 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00203.xml
--rw-r--r--   0 ton        (501) staff       (20)    21095 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00204.xml
--rw-r--r--   0 ton        (501) staff       (20)    18870 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00211.xml
--rw-r--r--   0 ton        (501) staff       (20)    18973 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00212.xml
--rw-r--r--   0 ton        (501) staff       (20)    19047 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00213.xml
--rw-r--r--   0 ton        (501) staff       (20)    18980 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00214.xml
--rw-r--r--   0 ton        (501) staff       (20)    12093 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00220.xml
--rw-r--r--   0 ton        (501) staff       (20)     1483 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00302.xml
--rw-r--r--   0 ton        (501) staff       (20)      709 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00303.xml
--rw-r--r--   0 ton        (501) staff       (20)     1078 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00304.xml
--rw-r--r--   0 ton        (501) staff       (20)     1823 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00305.xml
--rw-r--r--   0 ton        (501) staff       (20)     1313 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00306.xml
--rw-r--r--   0 ton        (501) staff       (20)     2521 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00307.xml
--rw-r--r--   0 ton        (501) staff       (20)     1260 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00308.xml
--rw-r--r--   0 ton        (501) staff       (20)     5426 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00401.xml
--rw-r--r--   0 ton        (501) staff       (20)     7223 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00402.xml
--rw-r--r--   0 ton        (501) staff       (20)     5727 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00403.xml
--rw-r--r--   0 ton        (501) staff       (20)     8177 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00404.xml
--rw-r--r--   0 ton        (501) staff       (20)    10768 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00501.xml
--rw-r--r--   0 ton        (501) staff       (20)    11574 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00502.xml
--rw-r--r--   0 ton        (501) staff       (20)     9121 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00601.xml
--rw-r--r--   0 ton        (501) staff       (20)      638 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00801.xml
--rw-r--r--   0 ton        (501) staff       (20)    31467 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00802.xml
--rw-r--r--   0 ton        (501) staff       (20)    32797 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00803.xml
--rw-r--r--   0 ton        (501) staff       (20)    31777 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00804.xml
--rw-r--r--   0 ton        (501) staff       (20)     7846 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00805.xml
--rw-r--r--   0 ton        (501) staff       (20)      850 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00806.xml
--rw-r--r--   0 ton        (501) staff       (20)    42745 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00807.xml
--rw-r--r--   0 ton        (501) staff       (20)      858 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00808.xml
--rw-r--r--   0 ton        (501) staff       (20)      848 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00809.xml
--rw-r--r--   0 ton        (501) staff       (20)     5185 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_63001.xml
--rw-r--r--   0 ton        (501) staff       (20)      559 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_63002.xml
--rw-r--r--   0 ton        (501) staff       (20)     6862 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64001.xml
--rw-r--r--   0 ton        (501) staff       (20)     7909 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64020.xml
--rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64101.xml
--rw-r--r--   0 ton        (501) staff       (20)    12153 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64110.xml
--rw-r--r--   0 ton        (501) staff       (20)     5688 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64111.xml
--rw-r--r--   0 ton        (501) staff       (20)    21312 2024-05-30 07:46:26.000000 smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64112.xml
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.577142 smasunnyisland-0.44/
+-rw-r--r--   0 ton        (501) staff       (20)     1075 2024-05-30 05:57:21.000000 smasunnyisland-0.44/LICENSE
+-rw-r--r--   0 ton        (501) staff       (20)       63 2024-05-30 07:46:56.000000 smasunnyisland-0.44/MANIFEST.in
+-rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 08:00:50.576897 smasunnyisland-0.44/PKG-INFO
+-rw-r--r--   0 ton        (501) staff       (20)     1549 2024-05-30 06:55:14.000000 smasunnyisland-0.44/README.md
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.576587 smasunnyisland-0.44/SMASunnyIsland.egg-info/
+-rw-r--r--   0 ton        (501) staff       (20)     2301 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/PKG-INFO
+-rw-r--r--   0 ton        (501) staff       (20)     9245 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/SOURCES.txt
+-rw-r--r--   0 ton        (501) staff       (20)        1 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/dependency_links.txt
+-rw-r--r--   0 ton        (501) staff       (20)       25 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/requires.txt
+-rw-r--r--   0 ton        (501) staff       (20)       15 2024-05-30 08:00:50.000000 smasunnyisland-0.44/SMASunnyIsland.egg-info/top_level.txt
+-rw-r--r--   0 ton        (501) staff       (20)      726 2024-05-30 08:00:46.000000 smasunnyisland-0.44/pyproject.toml
+-rw-r--r--   0 ton        (501) staff       (20)       38 2024-05-30 08:00:50.577182 smasunnyisland-0.44/setup.cfg
+-rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:35:47.000000 smasunnyisland-0.44/setup.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.542448 smasunnyisland-0.44/smasunnyisland/
+-rw-r--r--   0 ton        (501) staff       (20)       48 2024-05-30 06:53:20.000000 smasunnyisland-0.44/smasunnyisland/__init__.py
+-rw-r--r--   0 ton        (501) staff       (20)     6757 2024-05-30 08:00:38.000000 smasunnyisland-0.44/smasunnyisland/sma_controller.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.539110 smasunnyisland-0.44/vendor/
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.544277 smasunnyisland-0.44/vendor/pysunspec/
+-rw-r--r--   0 ton        (501) staff       (20)       44 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.git
+-rw-r--r--   0 ton        (501) staff       (20)      969 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.gitignore
+-rw-r--r--   0 ton        (501) staff       (20)       97 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.gitmodules
+-rw-r--r--   0 ton        (501) staff       (20)      247 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/.travis.yml
+-rw-r--r--   0 ton        (501) staff       (20)     3050 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/CHANGES.txt
+-rw-r--r--   0 ton        (501) staff       (20)     1062 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/LICENSE
+-rw-r--r--   0 ton        (501) staff       (20)     6627 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/README.md
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.545646 smasunnyisland-0.44/vendor/pysunspec/doc/
+-rw-r--r--   0 ton        (501) staff       (20)     6774 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/Makefile
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549088 smasunnyisland-0.44/vendor/pysunspec/doc/_static/
+-rw-r--r--   0 ton        (501) staff       (20)      673 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/ajax-loader.gif
+-rw-r--r--   0 ton        (501) staff       (20)     8463 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/basic.css
+-rw-r--r--   0 ton        (501) staff       (20)     3500 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-bright.png
+-rw-r--r--   0 ton        (501) staff       (20)     3578 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-close.png
+-rw-r--r--   0 ton        (501) staff       (20)     3445 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment.png
+-rw-r--r--   0 ton        (501) staff       (20)     4040 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/default.css
+-rw-r--r--   0 ton        (501) staff       (20)     6620 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/doctools.js
+-rw-r--r--   0 ton        (501) staff       (20)      368 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/down-pressed.png
+-rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/down.png
+-rw-r--r--   0 ton        (501) staff       (20)      392 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/file.png
+-rw-r--r--   0 ton        (501) staff       (20)    93636 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/jquery.js
+-rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/minus.png
+-rw-r--r--   0 ton        (501) staff       (20)      199 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/plus.png
+-rw-r--r--   0 ton        (501) staff       (20)     3932 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/pygments.css
+-rw-r--r--   0 ton        (501) staff       (20)    17844 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/searchtools.js
+-rw-r--r--   0 ton        (501) staff       (20)     4803 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/sidebar.js
+-rw-r--r--   0 ton        (501) staff       (20)    12140 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/underscore.js
+-rw-r--r--   0 ton        (501) staff       (20)      372 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/up-pressed.png
+-rw-r--r--   0 ton        (501) staff       (20)      363 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/up.png
+-rw-r--r--   0 ton        (501) staff       (20)    25246 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/_static/websupport.js
+-rw-r--r--   0 ton        (501) staff       (20)     8295 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/conf.py
+-rw-r--r--   0 ton        (501) staff       (20)      463 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/index.rst
+-rw-r--r--   0 ton        (501) staff       (20)     6465 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/make.bat
+-rw-r--r--   0 ton        (501) staff       (20)    13217 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec.rst
+-rw-r--r--   0 ton        (501) staff       (20)     8858 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec_api.rst
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549416 smasunnyisland-0.44/vendor/pysunspec/scripts/
+-rw-r--r--   0 ton        (501) staff       (20)      725 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/scripts/pysunspec_coverage_report.py
+-rw-r--r--   0 ton        (501) staff       (20)     4872 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/scripts/suns.py
+-rw-r--r--   0 ton        (501) staff       (20)     1300 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/setup.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549563 smasunnyisland-0.44/vendor/pysunspec/sunspec/
+-rw-r--r--   0 ton        (501) staff       (20)       41 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/__init__.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.549721 smasunnyisland-0.44/vendor/pysunspec/sunspec/__pycache__/
+-rw-r--r--   0 ton        (501) staff       (20)      223 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.551140 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/
+-rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__init__.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.551581 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/
+-rw-r--r--   0 ton        (501) staff       (20)      210 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 ton        (501) staff       (20)    37799 2024-05-30 07:53:38.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/client.cpython-311.pyc
+-rwxr-xr-x   0 ton        (501) staff       (20)    30669 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/client.py
+-rw-r--r--   0 ton        (501) staff       (20)     9525 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/data.py
+-rw-r--r--   0 ton        (501) staff       (20)    50822 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/device.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.552302 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/
+-rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/__init__.py
+-rwxr-xr-x   0 ton        (501) staff       (20)    34177 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/client.py
+-rw-r--r--   0 ton        (501) staff       (20)    20936 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/mbmap.py
+-rw-r--r--   0 ton        (501) staff       (20)     2189 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/pics.py
+-rw-r--r--   0 ton        (501) staff       (20)     4125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/smdx.py
+-rw-r--r--   0 ton        (501) staff       (20)     6808 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/suns.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.553856 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/
+-rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/__init__.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556276 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/
+-rw-r--r--   0 ton        (501) staff       (20)    16406 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1.xml
+-rw-r--r--   0 ton        (501) staff       (20)    16290 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_a.xml
+-rw-r--r--   0 ton        (501) staff       (20)    15978 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_b.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12196 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_c.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12203 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_d.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_processed.xml
+-rw-r--r--   0 ton        (501) staff       (20)      647 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_2.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1125 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_3.xml
+-rw-r--r--   0 ton        (501) staff       (20)     5432 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_1.xml
+-rw-r--r--   0 ton        (501) staff       (20)     9354 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_2.xml
+-rw-r--r--   0 ton        (501) staff       (20)    17198 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_3.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_1.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4665 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_2.xml
+-rw-r--r--   0 ton        (501) staff       (20)     3159 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_1.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1422 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_2.xml
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556701 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/
+-rw-r--r--   0 ton        (501) staff       (20)        0 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/__init__.py
+-rw-r--r--   0 ton        (501) staff       (20)     2485 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/serial.py
+-rw-r--r--   0 ton        (501) staff       (20)     2049 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/socket.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.556858 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/models/
+-rw-r--r--   0 ton        (501) staff       (20)      479 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/models/smdx_65000.xml
+-rw-r--r--   0 ton        (501) staff       (20)     2674 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_all.py
+-rw-r--r--   0 ton        (501) staff       (20)     7939 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_client.py
+-rw-r--r--   0 ton        (501) staff       (20)     2117 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_data.py
+-rw-r--r--   0 ton        (501) staff       (20)    21372 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_device.py
+-rw-r--r--   0 ton        (501) staff       (20)     3834 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_client.py
+-rw-r--r--   0 ton        (501) staff       (20)     4479 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_mbmap.py
+-rw-r--r--   0 ton        (501) staff       (20)     6189 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_util.py
+-rw-r--r--   0 ton        (501) staff       (20)     7558 2024-05-30 07:09:54.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/core/util.py
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.557887 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/
+-rw-r--r--   0 ton        (501) staff       (20)       73 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.git
+-rw-r--r--   0 ton        (501) staff       (20)      483 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.gitattributes
+-rw-r--r--   0 ton        (501) staff       (20)     2643 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.gitignore
+-rw-r--r--   0 ton        (501) staff       (20)      141 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.travis.yml
+-rw-r--r--   0 ton        (501) staff       (20)      112 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/README.md
+drwxr-xr-x   0 ton        (501) staff       (20)        0 2024-05-30 08:00:50.576284 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/
+-rw-r--r--   0 ton        (501) staff       (20)     5099 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/CHANGELOG
+-rw-r--r--   0 ton        (501) staff       (20)     1958 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/Makefile
+-rw-r--r--   0 ton        (501) staff       (20)     5679 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.py
+-rw-r--r--   0 ton        (501) staff       (20)     6780 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.xml
+-rw-r--r--   0 ton        (501) staff       (20)       32 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.xml.md5
+-rw-r--r--   0 ton        (501) staff       (20)     7076 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx.xsd
+-rw-r--r--   0 ton        (501) staff       (20)     1914 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00001.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4107 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00002.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7457 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00003.xml
+-rw-r--r--   0 ton        (501) staff       (20)     9120 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00004.xml
+-rw-r--r--   0 ton        (501) staff       (20)    10097 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00005.xml
+-rw-r--r--   0 ton        (501) staff       (20)    10295 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00006.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4994 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00007.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1319 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00008.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11522 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00009.xml
+-rw-r--r--   0 ton        (501) staff       (20)     2628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00010.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4729 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00011.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7692 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00012.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7716 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00013.xml
+-rw-r--r--   0 ton        (501) staff       (20)     2781 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00014.xml
+-rw-r--r--   0 ton        (501) staff       (20)     3151 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00015.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4476 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00016.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4776 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00017.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1468 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00018.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4418 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00019.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12770 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00101.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12834 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00102.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12883 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00103.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11866 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00111.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11895 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00112.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11964 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00113.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7816 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00120.xml
+-rw-r--r--   0 ton        (501) staff       (20)     9437 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00121.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7499 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00122.xml
+-rw-r--r--   0 ton        (501) staff       (20)     8208 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00123.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7583 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00124.xml
+-rw-r--r--   0 ton        (501) staff       (20)     3496 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00125.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14940 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00126.xml
+-rw-r--r--   0 ton        (501) staff       (20)     3450 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00127.xml
+-rw-r--r--   0 ton        (501) staff       (20)     4848 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00128.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00129.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14375 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00130.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14955 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00131.xml
+-rw-r--r--   0 ton        (501) staff       (20)    15233 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00132.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11710 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00133.xml
+-rw-r--r--   0 ton        (501) staff       (20)    16249 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00134.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00135.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14404 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00136.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00137.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14628 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00138.xml
+-rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00139.xml
+-rw-r--r--   0 ton        (501) staff       (20)    13818 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00140.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00141.xml
+-rw-r--r--   0 ton        (501) staff       (20)    14661 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00142.xml
+-rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00143.xml
+-rw-r--r--   0 ton        (501) staff       (20)    13857 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00144.xml
+-rw-r--r--   0 ton        (501) staff       (20)     2810 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00145.xml
+-rw-r--r--   0 ton        (501) staff       (20)    13998 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00160.xml
+-rw-r--r--   0 ton        (501) staff       (20)    20615 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00201.xml
+-rw-r--r--   0 ton        (501) staff       (20)    21089 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00202.xml
+-rw-r--r--   0 ton        (501) staff       (20)    21145 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00203.xml
+-rw-r--r--   0 ton        (501) staff       (20)    21095 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00204.xml
+-rw-r--r--   0 ton        (501) staff       (20)    18870 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00211.xml
+-rw-r--r--   0 ton        (501) staff       (20)    18973 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00212.xml
+-rw-r--r--   0 ton        (501) staff       (20)    19047 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00213.xml
+-rw-r--r--   0 ton        (501) staff       (20)    18980 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00214.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12093 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00220.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1483 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00302.xml
+-rw-r--r--   0 ton        (501) staff       (20)      709 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00303.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1078 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00304.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1823 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00305.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1313 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00306.xml
+-rw-r--r--   0 ton        (501) staff       (20)     2521 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00307.xml
+-rw-r--r--   0 ton        (501) staff       (20)     1260 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00308.xml
+-rw-r--r--   0 ton        (501) staff       (20)     5426 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00401.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7223 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00402.xml
+-rw-r--r--   0 ton        (501) staff       (20)     5727 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00403.xml
+-rw-r--r--   0 ton        (501) staff       (20)     8177 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00404.xml
+-rw-r--r--   0 ton        (501) staff       (20)    10768 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00501.xml
+-rw-r--r--   0 ton        (501) staff       (20)    11574 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00502.xml
+-rw-r--r--   0 ton        (501) staff       (20)     9121 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00601.xml
+-rw-r--r--   0 ton        (501) staff       (20)      638 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00801.xml
+-rw-r--r--   0 ton        (501) staff       (20)    31467 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00802.xml
+-rw-r--r--   0 ton        (501) staff       (20)    32797 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00803.xml
+-rw-r--r--   0 ton        (501) staff       (20)    31777 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00804.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7846 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00805.xml
+-rw-r--r--   0 ton        (501) staff       (20)      850 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00806.xml
+-rw-r--r--   0 ton        (501) staff       (20)    42745 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00807.xml
+-rw-r--r--   0 ton        (501) staff       (20)      858 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00808.xml
+-rw-r--r--   0 ton        (501) staff       (20)      848 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00809.xml
+-rw-r--r--   0 ton        (501) staff       (20)     5185 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63001.xml
+-rw-r--r--   0 ton        (501) staff       (20)      559 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63002.xml
+-rw-r--r--   0 ton        (501) staff       (20)     6862 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64001.xml
+-rw-r--r--   0 ton        (501) staff       (20)     7909 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64020.xml
+-rw-r--r--   0 ton        (501) staff       (20)      763 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64101.xml
+-rw-r--r--   0 ton        (501) staff       (20)    12153 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64110.xml
+-rw-r--r--   0 ton        (501) staff       (20)     5688 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64111.xml
+-rw-r--r--   0 ton        (501) staff       (20)    21312 2024-05-30 07:46:26.000000 smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64112.xml
```

### Comparing `smasunnyisland-0.43/LICENSE` & `smasunnyisland-0.44/LICENSE`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/PKG-INFO` & `smasunnyisland-0.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMASunnyIsland
-Version: 0.43
+Version: 0.44
 Summary: A Python library for controlling SMA Sunny Island inverters
 Home-page: https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Author: Harm van den Brink
 Author-email: Harm van den Brink <harmvandenbrink@gmail.com>
 Project-URL: Homepage, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Project-URL: Issues, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smasunnyisland-0.43/README.md` & `smasunnyisland-0.44/README.md`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/SMASunnyIsland.egg-info/PKG-INFO` & `smasunnyisland-0.44/SMASunnyIsland.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SMASunnyIsland
-Version: 0.43
+Version: 0.44
 Summary: A Python library for controlling SMA Sunny Island inverters
 Home-page: https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Author: Harm van den Brink
 Author-email: Harm van den Brink <harmvandenbrink@gmail.com>
 Project-URL: Homepage, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller
 Project-URL: Issues, https://github.com/HarmvandenBrink/SMA_Sunny_Island_Controller/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `smasunnyisland-0.43/SMASunnyIsland.egg-info/SOURCES.txt` & `smasunnyisland-0.44/SMASunnyIsland.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/pyproject.toml` & `smasunnyisland-0.44/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "SMASunnyIsland"
-version = "0.43"
+version = "0.44"
 authors = [
   { name="Harm van den Brink", email="harmvandenbrink@gmail.com" },
 ]
 description = "A Python library for controlling SMA Sunny Island inverters"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `smasunnyisland-0.43/setup.py` & `smasunnyisland-0.44/setup.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/smasunnyisland/sma_controller.py` & `smasunnyisland-0.44/smasunnyisland/sma_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 __author__ = "Harm van den Brink"
 __email__ = "harmvandenbrink@gmail.com"
 __license__ = "MIT License"
 
 __version__ = "1.42"
 __status__ = "Production"
 
-from ..vendor.pysunspec.sunspec.core import client as clientSunspec
+from .vendor.pysunspec.sunspec.core import client as clientSunspec
 from pymodbus.constants import Endian
 from pymodbus.payload import BinaryPayloadBuilder
 from pymodbus.client.sync import ModbusTcpClient as ModbusClient
 from collections import OrderedDict
 
 
 class SMASunnyIslandClient:
```

### Comparing `smasunnyisland-0.43/vendor/pysunspec/.gitignore` & `smasunnyisland-0.44/vendor/pysunspec/.gitignore`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/CHANGES.txt` & `smasunnyisland-0.44/vendor/pysunspec/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/LICENSE` & `smasunnyisland-0.44/vendor/pysunspec/LICENSE`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/README.md` & `smasunnyisland-0.44/vendor/pysunspec/README.md`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/Makefile` & `smasunnyisland-0.44/vendor/pysunspec/doc/Makefile`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/ajax-loader.gif` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/basic.css` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/basic.css`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment-bright.png` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment-close.png` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/comment.png` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/comment.png`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/default.css` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/default.css`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/doctools.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/jquery.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/pygments.css` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/searchtools.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/sidebar.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/sidebar.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/underscore.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/_static/websupport.js` & `smasunnyisland-0.44/vendor/pysunspec/doc/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/conf.py` & `smasunnyisland-0.44/vendor/pysunspec/doc/conf.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/make.bat` & `smasunnyisland-0.44/vendor/pysunspec/doc/make.bat`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/pysunspec.rst` & `smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec.rst`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/doc/pysunspec_api.rst` & `smasunnyisland-0.44/vendor/pysunspec/doc/pysunspec_api.rst`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/scripts/pysunspec_coverage_report.py` & `smasunnyisland-0.44/vendor/pysunspec/scripts/pysunspec_coverage_report.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/scripts/suns.py` & `smasunnyisland-0.44/vendor/pysunspec/scripts/suns.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/setup.py` & `smasunnyisland-0.44/vendor/pysunspec/setup.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/__pycache__/client.cpython-311.pyc` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/__pycache__/client.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/client.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/client.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/data.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/data.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/device.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/device.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/client.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/client.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/modbus/mbmap.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/modbus/mbmap.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/pics.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/pics.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/smdx.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/smdx.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/suns.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/suns.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_a.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_a.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_b.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_b.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_c.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_c.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_d.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_d.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_processed.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_1_processed.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_2.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_2.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_3.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_device_3.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_1.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_1.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_2.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_2.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_3.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/mbmap_test_inverter_3.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_1.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_1.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_2.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_device_2.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_1.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_1.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_2.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/devices/pics_test_inverter_2.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/serial.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/serial.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/fake/socket.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/fake/socket.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_all.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_all.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_client.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_client.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_data.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_data.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_device.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_device.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_modbus_client.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_client.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_modbus_mbmap.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_modbus_mbmap.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/test/test_util.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/test/test_util.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/core/util.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/core/util.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/.gitignore` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/.gitignore`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/CHANGELOG` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/CHANGELOG`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/Makefile` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/Makefile`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/manifest.py` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.py`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/manifest.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/manifest.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx.xsd` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx.xsd`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00001.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00001.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00002.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00002.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00003.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00003.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00004.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00004.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00005.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00005.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00006.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00006.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00007.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00007.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00008.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00008.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00009.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00009.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00010.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00010.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00011.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00011.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00012.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00012.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00013.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00013.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00014.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00014.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00015.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00015.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00016.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00016.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00017.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00017.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00018.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00018.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00019.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00019.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00101.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00101.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00102.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00102.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00103.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00103.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00111.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00111.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00112.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00112.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00113.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00113.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00120.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00120.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00121.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00121.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00122.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00122.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00123.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00123.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00124.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00124.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00125.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00125.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00126.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00126.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00127.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00127.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00128.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00128.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00129.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00129.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00130.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00130.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00131.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00131.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00132.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00132.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00133.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00133.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00134.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00134.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00135.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00135.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00136.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00136.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00137.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00137.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00138.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00138.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00139.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00139.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00140.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00140.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00141.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00141.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00142.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00142.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00143.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00143.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00144.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00144.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00145.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00145.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00160.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00160.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00201.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00201.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00202.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00202.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00203.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00203.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00204.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00204.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00211.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00211.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00212.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00212.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00213.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00213.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00214.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00214.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00220.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00220.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00302.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00302.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00303.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00303.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00304.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00304.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00305.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00305.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00306.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00306.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00307.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00307.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00308.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00308.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00401.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00401.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00402.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00402.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00403.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00403.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00404.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00404.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00501.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00501.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00502.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00502.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00601.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00601.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00801.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00801.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00802.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00802.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00803.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00803.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00804.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00804.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00805.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00805.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00806.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00806.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00807.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00807.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00808.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00808.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_00809.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_00809.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_63001.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63001.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_63002.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_63002.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64001.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64001.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64020.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64020.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64101.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64101.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64110.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64110.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64111.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64111.xml`

 * *Files identical despite different names*

### Comparing `smasunnyisland-0.43/vendor/pysunspec/sunspec/models/smdx/smdx_64112.xml` & `smasunnyisland-0.44/vendor/pysunspec/sunspec/models/smdx/smdx_64112.xml`

 * *Files identical despite different names*

