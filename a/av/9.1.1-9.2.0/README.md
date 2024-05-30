# Comparing `tmp/av-9.1.1.tar.gz` & `tmp/av-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/av-9.1.1.tar", last modified: Fri Apr  1 06:09:47 2022, max compression
+gzip compressed data, was "dist/av-9.2.0.tar", last modified: Wed Apr 20 06:46:11 2022, max compression
```

## Comparing `av-9.1.1.tar` & `av-9.2.0.tar`

### file list

```diff
@@ -1,287 +1,296 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-04-01 06:09:33.000000 av-9.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-01 06:09:33.000000 av-9.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-04-01 06:09:47.000000 av-9.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-04-01 06:09:33.000000 av-9.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-04-01 06:09:33.000000 av-9.1.1/av/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-01 06:09:33.000000 av-9.1.1/av/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-04-01 06:09:33.000000 av-9.1.1/av/_core.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-01 06:09:33.000000 av-9.1.1/av/about.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/audio/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/fifo.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/fifo.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      729 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/layout.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/layout.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/resampler.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/resampler.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-01 06:09:33.000000 av-9.1.1/av/audio/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-01 06:09:33.000000 av-9.1.1/av/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-04-01 06:09:33.000000 av-9.1.1/av/buffer.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-04-01 06:09:33.000000 av-9.1.1/av/bytesource.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-04-01 06:09:33.000000 av-9.1.1/av/bytesource.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/codec/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-01 06:09:33.000000 av-9.1.1/av/codec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-04-01 06:09:33.000000 av-9.1.1/av/codec/codec.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-04-01 06:09:33.000000 av-9.1.1/av/codec/codec.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-04-01 06:09:33.000000 av-9.1.1/av/codec/context.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    22024 2022-04-01 06:09:33.000000 av-9.1.1/av/codec/context.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/container/
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-04-01 06:09:33.000000 av-9.1.1/av/container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-04-01 06:09:33.000000 av-9.1.1/av/container/core.pxd
--rwxr-xr-x   0 runner    (1001) docker     (121)    11577 2022-04-01 06:09:33.000000 av-9.1.1/av/container/core.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-01 06:09:33.000000 av-9.1.1/av/container/input.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-04-01 06:09:33.000000 av-9.1.1/av/container/input.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-04-01 06:09:33.000000 av-9.1.1/av/container/output.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8327 2022-04-01 06:09:33.000000 av-9.1.1/av/container/output.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      587 2022-04-01 06:09:33.000000 av-9.1.1/av/container/pyio.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-04-01 06:09:33.000000 av-9.1.1/av/container/pyio.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-04-01 06:09:33.000000 av-9.1.1/av/container/streams.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-04-01 06:09:33.000000 av-9.1.1/av/container/streams.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:33.000000 av-9.1.1/av/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-04-01 06:09:33.000000 av-9.1.1/av/data/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-01 06:09:33.000000 av-9.1.1/av/data/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-01 06:09:33.000000 av-9.1.1/av/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-04-01 06:09:33.000000 av-9.1.1/av/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      527 2022-04-01 06:09:33.000000 av-9.1.1/av/descriptor.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-04-01 06:09:33.000000 av-9.1.1/av/descriptor.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-01 06:09:33.000000 av-9.1.1/av/dictionary.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-04-01 06:09:33.000000 av-9.1.1/av/dictionary.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-01 06:09:33.000000 av-9.1.1/av/enum.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10643 2022-04-01 06:09:33.000000 av-9.1.1/av/enum.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-01 06:09:33.000000 av-9.1.1/av/error.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-04-01 06:09:33.000000 av-9.1.1/av/error.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/filter/
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      394 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/context.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/context.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/filter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/filter.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/graph.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/graph.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      335 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/link.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/link.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/pad.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-04-01 06:09:33.000000 av-9.1.1/av/filter/pad.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-01 06:09:33.000000 av-9.1.1/av/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7055 2022-04-01 06:09:33.000000 av-9.1.1/av/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-04-01 06:09:33.000000 av-9.1.1/av/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-04-01 06:09:33.000000 av-9.1.1/av/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-01 06:09:33.000000 av-9.1.1/av/logging.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-04-01 06:09:33.000000 av-9.1.1/av/logging.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-01 06:09:33.000000 av-9.1.1/av/option.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-04-01 06:09:33.000000 av-9.1.1/av/option.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-04-01 06:09:33.000000 av-9.1.1/av/packet.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-01 06:09:33.000000 av-9.1.1/av/packet.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-01 06:09:33.000000 av-9.1.1/av/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-01 06:09:33.000000 av-9.1.1/av/plane.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:33.000000 av-9.1.1/av/sidedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-04-01 06:09:33.000000 av-9.1.1/av/sidedata/motionvectors.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-04-01 06:09:33.000000 av-9.1.1/av/sidedata/motionvectors.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      419 2022-04-01 06:09:33.000000 av-9.1.1/av/sidedata/sidedata.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-04-01 06:09:33.000000 av-9.1.1/av/sidedata/sidedata.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-04-01 06:09:33.000000 av-9.1.1/av/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-04-01 06:09:33.000000 av-9.1.1/av/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      101 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      624 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/stream.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/subtitle.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-04-01 06:09:33.000000 av-9.1.1/av/subtitles/subtitle.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-04-01 06:09:33.000000 av-9.1.1/av/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-04-01 06:09:33.000000 av-9.1.1/av/utils.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av/video/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-01 06:09:33.000000 av-9.1.1/av/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-01 06:09:33.000000 av-9.1.1/av/video/codeccontext.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-04-01 06:09:33.000000 av-9.1.1/av/video/codeccontext.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-01 06:09:33.000000 av-9.1.1/av/video/format.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-04-01 06:09:33.000000 av-9.1.1/av/video/format.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-01 06:09:33.000000 av-9.1.1/av/video/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    14336 2022-04-01 06:09:33.000000 av-9.1.1/av/video/frame.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-01 06:09:33.000000 av-9.1.1/av/video/plane.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-04-01 06:09:33.000000 av-9.1.1/av/video/plane.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-01 06:09:33.000000 av-9.1.1/av/video/reformatter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     7053 2022-04-01 06:09:33.000000 av-9.1.1/av/video/reformatter.pyx
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-01 06:09:33.000000 av-9.1.1/av/video/stream.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-04-01 06:09:33.000000 av-9.1.1/av/video/stream.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5419 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-04-01 06:09:47.000000 av-9.1.1/av.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/docs/api/
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/_globals.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/audio.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/buffer.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/codec.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/container.rst
--rw-r--r--   0 runner    (1001) docker     (121)      217 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/enum.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/error.rst
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/error_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/filter.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/frame.rst
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/packet.rst
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/plane.rst
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/sidedata.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/stream.rst
--rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/subtitles.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/time.rst
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-01 06:09:33.000000 av-9.1.1/docs/api/video.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13563 2022-04-01 06:09:33.000000 av-9.1.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/docs/cookbook/
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-04-01 06:09:33.000000 av-9.1.1/docs/cookbook/basics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-01 06:09:33.000000 av-9.1.1/docs/cookbook/numpy.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/docs/development/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/hacking.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11074 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/includes.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/includes.rst
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-01 06:09:33.000000 av-9.1.1/docs/development/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-04-01 06:09:33.000000 av-9.1.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/docs/overview/
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-04-01 06:09:33.000000 av-9.1.1/docs/overview/caveats.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-01 06:09:33.000000 av-9.1.1/docs/overview/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/examples/basics/
--rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-04-01 06:09:33.000000 av-9.1.1/examples/basics/parse.py
--rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-01 06:09:33.000000 av-9.1.1/examples/basics/remux.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-01 06:09:33.000000 av-9.1.1/examples/basics/save_keyframes.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-04-01 06:09:33.000000 av-9.1.1/examples/basics/thread_type.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/examples/numpy/
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-04-01 06:09:33.000000 av-9.1.1/examples/numpy/barcode.py
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-04-01 06:09:33.000000 av-9.1.1/examples/numpy/generate_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-04-01 06:09:33.000000 av-9.1.1/examples/numpy/generate_video_with_pts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-04-01 06:09:33.000000 av-9.1.1/flags.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-04-01 06:09:33.000000 av-9.1.1/include/libav.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libavcodec/
--rw-r--r--   0 runner    (1001) docker     (121)    11421 2022-04-01 06:09:33.000000 av-9.1.1/include/libavcodec/avcodec.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libavdevice/
--rw-r--r--   0 runner    (1001) docker     (121)      465 2022-04-01 06:09:33.000000 av-9.1.1/include/libavdevice/avdevice.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libavfilter/
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-04-01 06:09:33.000000 av-9.1.1/include/libavfilter/avfilter.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-04-01 06:09:33.000000 av-9.1.1/include/libavfilter/avfiltergraph.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-01 06:09:33.000000 av-9.1.1/include/libavfilter/buffersink.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-01 06:09:33.000000 av-9.1.1/include/libavfilter/buffersrc.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libavformat/
--rw-r--r--   0 runner    (1001) docker     (121)     7567 2022-04-01 06:09:33.000000 av-9.1.1/include/libavformat/avformat.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libavutil/
--rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/avutil.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/channel_layout.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/dict.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/error.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/frame.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/motion_vector.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-04-01 06:09:33.000000 av-9.1.1/include/libavutil/samplefmt.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libswresample/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-04-01 06:09:33.000000 av-9.1.1/include/libswresample/swresample.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/include/libswscale/
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-04-01 06:09:33.000000 av-9.1.1/include/libswscale/swscale.pxd
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-04-01 06:09:33.000000 av-9.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-04-01 06:09:47.000000 av-9.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6897 2022-04-01 06:09:33.000000 av-9.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/
--rw-r--r--   0 runner    (1001) docker     (121)   168273 2022-04-01 06:09:39.000000 av-9.1.1/src/av/_core.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/audio/
--rw-r--r--   0 runner    (1001) docker     (121)   266717 2022-04-01 06:09:41.000000 av-9.1.1/src/av/audio/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   293447 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/fifo.c
--rw-r--r--   0 runner    (1001) docker     (121)   214505 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/format.c
--rw-r--r--   0 runner    (1001) docker     (121)   351787 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   359762 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/layout.c
--rw-r--r--   0 runner    (1001) docker     (121)   193075 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/plane.c
--rw-r--r--   0 runner    (1001) docker     (121)   304646 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/resampler.c
--rw-r--r--   0 runner    (1001) docker     (121)   189581 2022-04-01 06:09:42.000000 av-9.1.1/src/av/audio/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   227068 2022-04-01 06:09:38.000000 av-9.1.1/src/av/buffer.c
--rw-r--r--   0 runner    (1001) docker     (121)   169363 2022-04-01 06:09:38.000000 av-9.1.1/src/av/bytesource.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/codec/
--rw-r--r--   0 runner    (1001) docker     (121)   425072 2022-04-01 06:09:41.000000 av-9.1.1/src/av/codec/codec.c
--rw-r--r--   0 runner    (1001) docker     (121)   659900 2022-04-01 06:09:41.000000 av-9.1.1/src/av/codec/context.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/container/
--rw-r--r--   0 runner    (1001) docker     (121)   503889 2022-04-01 06:09:47.000000 av-9.1.1/src/av/container/core.c
--rw-r--r--   0 runner    (1001) docker     (121)   423474 2022-04-01 06:09:46.000000 av-9.1.1/src/av/container/input.c
--rw-r--r--   0 runner    (1001) docker     (121)   367461 2022-04-01 06:09:46.000000 av-9.1.1/src/av/container/output.c
--rw-r--r--   0 runner    (1001) docker     (121)   262646 2022-04-01 06:09:46.000000 av-9.1.1/src/av/container/pyio.c
--rw-r--r--   0 runner    (1001) docker     (121)   334831 2022-04-01 06:09:47.000000 av-9.1.1/src/av/container/streams.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/data/
--rw-r--r--   0 runner    (1001) docker     (121)   207100 2022-04-01 06:09:46.000000 av-9.1.1/src/av/data/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   196054 2022-04-01 06:09:40.000000 av-9.1.1/src/av/descriptor.c
--rw-r--r--   0 runner    (1001) docker     (121)   264489 2022-04-01 06:09:38.000000 av-9.1.1/src/av/dictionary.c
--rw-r--r--   0 runner    (1001) docker     (121)   628354 2022-04-01 06:09:38.000000 av-9.1.1/src/av/enum.c
--rw-r--r--   0 runner    (1001) docker     (121)   491313 2022-04-01 06:09:39.000000 av-9.1.1/src/av/error.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/filter/
--rw-r--r--   0 runner    (1001) docker     (121)   324656 2022-04-01 06:09:43.000000 av-9.1.1/src/av/filter/context.c
--rw-r--r--   0 runner    (1001) docker     (121)   383993 2022-04-01 06:09:43.000000 av-9.1.1/src/av/filter/filter.c
--rw-r--r--   0 runner    (1001) docker     (121)   404942 2022-04-01 06:09:43.000000 av-9.1.1/src/av/filter/graph.c
--rw-r--r--   0 runner    (1001) docker     (121)   222055 2022-04-01 06:09:43.000000 av-9.1.1/src/av/filter/link.c
--rw-r--r--   0 runner    (1001) docker     (121)   235565 2022-04-01 06:09:43.000000 av-9.1.1/src/av/filter/pad.c
--rw-r--r--   0 runner    (1001) docker     (121)   304795 2022-04-01 06:09:40.000000 av-9.1.1/src/av/format.c
--rw-r--r--   0 runner    (1001) docker     (121)   253460 2022-04-01 06:09:38.000000 av-9.1.1/src/av/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   379960 2022-04-01 06:09:38.000000 av-9.1.1/src/av/logging.c
--rw-r--r--   0 runner    (1001) docker     (121)   306007 2022-04-01 06:09:39.000000 av-9.1.1/src/av/option.c
--rw-r--r--   0 runner    (1001) docker     (121)   305917 2022-04-01 06:09:39.000000 av-9.1.1/src/av/packet.c
--rw-r--r--   0 runner    (1001) docker     (121)   197939 2022-04-01 06:09:38.000000 av-9.1.1/src/av/plane.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/sidedata/
--rw-r--r--   0 runner    (1001) docker     (121)   328271 2022-04-01 06:09:45.000000 av-9.1.1/src/av/sidedata/motionvectors.c
--rw-r--r--   0 runner    (1001) docker     (121)   349772 2022-04-01 06:09:46.000000 av-9.1.1/src/av/sidedata/sidedata.c
--rw-r--r--   0 runner    (1001) docker     (121)   345153 2022-04-01 06:09:40.000000 av-9.1.1/src/av/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/subtitles/
--rw-r--r--   0 runner    (1001) docker     (121)   195320 2022-04-01 06:09:40.000000 av-9.1.1/src/av/subtitles/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   172188 2022-04-01 06:09:41.000000 av-9.1.1/src/av/subtitles/stream.c
--rw-r--r--   0 runner    (1001) docker     (121)   517901 2022-04-01 06:09:40.000000 av-9.1.1/src/av/subtitles/subtitle.c
--rw-r--r--   0 runner    (1001) docker     (121)   205321 2022-04-01 06:09:39.000000 av-9.1.1/src/av/utils.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/src/av/video/
--rw-r--r--   0 runner    (1001) docker     (121)   306976 2022-04-01 06:09:44.000000 av-9.1.1/src/av/video/codeccontext.c
--rw-r--r--   0 runner    (1001) docker     (121)   398253 2022-04-01 06:09:45.000000 av-9.1.1/src/av/video/format.c
--rw-r--r--   0 runner    (1001) docker     (121)  1204358 2022-04-01 06:09:45.000000 av-9.1.1/src/av/video/frame.c
--rw-r--r--   0 runner    (1001) docker     (121)   255436 2022-04-01 06:09:45.000000 av-9.1.1/src/av/video/plane.c
--rw-r--r--   0 runner    (1001) docker     (121)   278053 2022-04-01 06:09:45.000000 av-9.1.1/src/av/video/reformatter.c
--rw-r--r--   0 runner    (1001) docker     (121)   190546 2022-04-01 06:09:45.000000 av-9.1.1/src/av/video/stream.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:47.000000 av-9.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-01 06:09:33.000000 av-9.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-04-01 06:09:33.000000 av-9.1.1/tests/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_audiofifo.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_audioformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_audioframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_audiolayout.py
--rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_audioresampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (121)    11744 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_codec_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_containerformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_deprecation.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_doctests.py
--rw-r--r--   0 runner    (1001) docker     (121)     8294 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    14227 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_file_probing.py
--rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)      568 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (121)     5180 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_python_io.py
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_seek.py
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_subtitles.py
--rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_timeout.py
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_videoformat.py
--rw-r--r--   0 runner    (1001) docker     (121)    16390 2022-04-01 06:09:33.000000 av-9.1.1/tests/test_videoframe.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-04-20 06:45:49.000000 av-9.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-04-20 06:45:49.000000 av-9.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-04-20 06:46:11.000000 av-9.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3010 2022-04-20 06:45:49.000000 av-9.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-04-20 06:45:49.000000 av-9.2.0/av/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-20 06:45:49.000000 av-9.2.0/av/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1700 2022-04-20 06:45:49.000000 av-9.2.0/av/_core.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-04-20 06:45:49.000000 av-9.2.0/av/about.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3868 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/fifo.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     6236 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/fifo.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3836 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      729 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3986 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/layout.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      496 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/resampler.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4090 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/resampler.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      341 2022-04-20 06:45:49.000000 av-9.2.0/av/audio/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-20 06:45:49.000000 av-9.2.0/av/buffer.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2161 2022-04-20 06:45:49.000000 av-9.2.0/av/buffer.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-04-20 06:45:49.000000 av-9.2.0/av/bytesource.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-04-20 06:45:49.000000 av-9.2.0/av/bytesource.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      237 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/codec.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    14756 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/codec.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2328 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    22024 2022-04-20 06:45:49.000000 av-9.2.0/av/codec/context.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/container/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/container/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-04-20 06:45:49.000000 av-9.2.0/av/container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-04-20 06:45:49.000000 av-9.2.0/av/container/core.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (121)    15157 2022-04-20 06:45:49.000000 av-9.2.0/av/container/core.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-20 06:45:49.000000 av-9.2.0/av/container/input.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10045 2022-04-20 06:45:49.000000 av-9.2.0/av/container/input.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-04-20 06:45:49.000000 av-9.2.0/av/container/output.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     8427 2022-04-20 06:45:49.000000 av-9.2.0/av/container/output.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      712 2022-04-20 06:45:49.000000 av-9.2.0/av/container/pyio.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5253 2022-04-20 06:45:49.000000 av-9.2.0/av/container/pyio.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      319 2022-04-20 06:45:49.000000 av-9.2.0/av/container/streams.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-04-20 06:45:49.000000 av-9.2.0/av/container/streams.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/data/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-04-20 06:45:49.000000 av-9.2.0/av/data/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      653 2022-04-20 06:45:49.000000 av-9.2.0/av/data/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     3029 2022-04-20 06:45:49.000000 av-9.2.0/av/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2340 2022-04-20 06:45:49.000000 av-9.2.0/av/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      527 2022-04-20 06:45:49.000000 av-9.2.0/av/descriptor.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2412 2022-04-20 06:45:49.000000 av-9.2.0/av/descriptor.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-04-20 06:45:49.000000 av-9.2.0/av/dictionary.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1567 2022-04-20 06:45:49.000000 av-9.2.0/av/dictionary.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-04-20 06:45:49.000000 av-9.2.0/av/enum.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10754 2022-04-20 06:45:49.000000 av-9.2.0/av/enum.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2022-04-20 06:45:49.000000 av-9.2.0/av/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    10449 2022-04-20 06:45:49.000000 av-9.2.0/av/error.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      394 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/context.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4178 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/context.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/filter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2998 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/filter.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/graph.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     8066 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/graph.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/link.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/link.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      526 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/pad.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2777 2022-04-20 06:45:49.000000 av-9.2.0/av/filter/pad.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-20 06:45:49.000000 av-9.2.0/av/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7055 2022-04-20 06:45:49.000000 av-9.2.0/av/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-04-20 06:45:49.000000 av-9.2.0/av/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3980 2022-04-20 06:45:49.000000 av-9.2.0/av/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-20 06:45:49.000000 av-9.2.0/av/logging.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-04-20 06:45:49.000000 av-9.2.0/av/logging.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      374 2022-04-20 06:45:49.000000 av-9.2.0/av/option.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5760 2022-04-20 06:45:49.000000 av-9.2.0/av/option.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      447 2022-04-20 06:45:49.000000 av-9.2.0/av/packet.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-20 06:45:49.000000 av-9.2.0/av/packet.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-04-20 06:45:49.000000 av-9.2.0/av/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-20 06:45:49.000000 av-9.2.0/av/plane.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/motionvectors.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2644 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/motionvectors.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/sidedata.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-04-20 06:45:49.000000 av-9.2.0/av/sidedata/sidedata.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      733 2022-04-20 06:45:49.000000 av-9.2.0/av/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     9941 2022-04-20 06:45:49.000000 av-9.2.0/av/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      101 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       76 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/stream.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/subtitle.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5067 2022-04-20 06:45:49.000000 av-9.2.0/av/subtitles/subtitle.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      523 2022-04-20 06:45:49.000000 av-9.2.0/av/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2495 2022-04-20 06:45:49.000000 av-9.2.0/av/utils.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av/video/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/av/video/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       62 2022-04-20 06:45:49.000000 av-9.2.0/av/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      483 2022-04-20 06:45:49.000000 av-9.2.0/av/video/codeccontext.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     4789 2022-04-20 06:45:49.000000 av-9.2.0/av/video/codeccontext.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-20 06:45:49.000000 av-9.2.0/av/video/format.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     5988 2022-04-20 06:45:49.000000 av-9.2.0/av/video/format.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      634 2022-04-20 06:45:49.000000 av-9.2.0/av/video/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    14336 2022-04-20 06:45:49.000000 av-9.2.0/av/video/frame.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-04-20 06:45:49.000000 av-9.2.0/av/video/plane.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1316 2022-04-20 06:45:49.000000 av-9.2.0/av/video/plane.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-04-20 06:45:49.000000 av-9.2.0/av/video/reformatter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     7053 2022-04-20 06:45:49.000000 av-9.2.0/av/video/reformatter.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-20 06:45:49.000000 av-9.2.0/av/video/stream.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-04-20 06:45:49.000000 av-9.2.0/av/video/stream.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5052 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5622 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        3 2022-04-20 06:46:11.000000 av-9.2.0/av.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/_globals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/audio.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/buffer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/codec.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/container.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      217 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/enum.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/error.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      749 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/error_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      478 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/filter.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/frame.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/packet.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       85 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/plane.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/sidedata.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/subtitles.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/time.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-20 06:45:49.000000 av-9.2.0/docs/api/video.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13563 2022-04-20 06:45:49.000000 av-9.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/docs/cookbook/
+-rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-04-20 06:45:49.000000 av-9.2.0/docs/cookbook/basics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-20 06:45:49.000000 av-9.2.0/docs/cookbook/numpy.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/docs/development/
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/hacking.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11074 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/includes.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/includes.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-20 06:45:49.000000 av-9.2.0/docs/development/license.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2122 2022-04-20 06:45:49.000000 av-9.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/docs/overview/
+-rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-04-20 06:45:49.000000 av-9.2.0/docs/overview/caveats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2976 2022-04-20 06:45:49.000000 av-9.2.0/docs/overview/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/examples/basics/
+-rw-r--r--   0 runner    (1001) docker     (121)     1097 2022-04-20 06:45:49.000000 av-9.2.0/examples/basics/parse.py
+-rw-r--r--   0 runner    (1001) docker     (121)      668 2022-04-20 06:45:49.000000 av-9.2.0/examples/basics/remux.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-04-20 06:45:49.000000 av-9.2.0/examples/basics/save_keyframes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-04-20 06:45:49.000000 av-9.2.0/examples/basics/thread_type.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/examples/numpy/
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-04-20 06:45:49.000000 av-9.2.0/examples/numpy/barcode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-04-20 06:45:49.000000 av-9.2.0/examples/numpy/generate_video.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2957 2022-04-20 06:45:49.000000 av-9.2.0/examples/numpy/generate_video_with_pts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-04-20 06:45:49.000000 av-9.2.0/flags.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/
+-rw-r--r--   0 runner    (1001) docker     (121)      739 2022-04-20 06:45:49.000000 av-9.2.0/include/libav.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libavcodec/
+-rw-r--r--   0 runner    (1001) docker     (121)    11766 2022-04-20 06:45:49.000000 av-9.2.0/include/libavcodec/avcodec.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libavdevice/
+-rw-r--r--   0 runner    (1001) docker     (121)      465 2022-04-20 06:45:49.000000 av-9.2.0/include/libavdevice/avdevice.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libavfilter/
+-rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-04-20 06:45:49.000000 av-9.2.0/include/libavfilter/avfilter.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1279 2022-04-20 06:45:49.000000 av-9.2.0/include/libavfilter/avfiltergraph.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      144 2022-04-20 06:45:49.000000 av-9.2.0/include/libavfilter/buffersink.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-20 06:45:49.000000 av-9.2.0/include/libavfilter/buffersrc.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libavformat/
+-rw-r--r--   0 runner    (1001) docker     (121)     7931 2022-04-20 06:45:49.000000 av-9.2.0/include/libavformat/avformat.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libavutil/
+-rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/avutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/channel_layout.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      832 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/dict.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/error.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      718 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/frame.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/motion_vector.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     1647 2022-04-20 06:45:49.000000 av-9.2.0/include/libavutil/samplefmt.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libswresample/
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-04-20 06:45:49.000000 av-9.2.0/include/libswresample/swresample.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/include/libswscale/
+-rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-04-20 06:45:49.000000 av-9.2.0/include/libswscale/swscale.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2022-04-20 06:45:49.000000 av-9.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-04-20 06:46:11.000000 av-9.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7070 2022-04-20 06:45:49.000000 av-9.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/
+-rw-r--r--   0 runner    (1001) docker     (121)   168569 2022-04-20 06:46:00.000000 av-9.2.0/src/av/_core.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/audio/
+-rw-r--r--   0 runner    (1001) docker     (121)   267027 2022-04-20 06:46:07.000000 av-9.2.0/src/av/audio/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   293757 2022-04-20 06:46:07.000000 av-9.2.0/src/av/audio/fifo.c
+-rw-r--r--   0 runner    (1001) docker     (121)   214801 2022-04-20 06:46:06.000000 av-9.2.0/src/av/audio/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)   352097 2022-04-20 06:46:06.000000 av-9.2.0/src/av/audio/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   360058 2022-04-20 06:46:07.000000 av-9.2.0/src/av/audio/layout.c
+-rw-r--r--   0 runner    (1001) docker     (121)   193385 2022-04-20 06:46:07.000000 av-9.2.0/src/av/audio/plane.c
+-rw-r--r--   0 runner    (1001) docker     (121)   304956 2022-04-20 06:46:06.000000 av-9.2.0/src/av/audio/resampler.c
+-rw-r--r--   0 runner    (1001) docker     (121)   189891 2022-04-20 06:46:06.000000 av-9.2.0/src/av/audio/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   227068 2022-04-20 06:46:00.000000 av-9.2.0/src/av/buffer.c
+-rw-r--r--   0 runner    (1001) docker     (121)   169363 2022-04-20 06:45:59.000000 av-9.2.0/src/av/bytesource.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/codec/
+-rw-r--r--   0 runner    (1001) docker     (121)   425368 2022-04-20 06:46:03.000000 av-9.2.0/src/av/codec/codec.c
+-rw-r--r--   0 runner    (1001) docker     (121)   660210 2022-04-20 06:46:04.000000 av-9.2.0/src/av/codec/context.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/container/
+-rw-r--r--   0 runner    (1001) docker     (121)   550169 2022-04-20 06:46:05.000000 av-9.2.0/src/av/container/core.c
+-rw-r--r--   0 runner    (1001) docker     (121)   423784 2022-04-20 06:46:05.000000 av-9.2.0/src/av/container/input.c
+-rw-r--r--   0 runner    (1001) docker     (121)   369851 2022-04-20 06:46:06.000000 av-9.2.0/src/av/container/output.c
+-rw-r--r--   0 runner    (1001) docker     (121)   271972 2022-04-20 06:46:05.000000 av-9.2.0/src/av/container/pyio.c
+-rw-r--r--   0 runner    (1001) docker     (121)   335141 2022-04-20 06:46:05.000000 av-9.2.0/src/av/container/streams.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/data/
+-rw-r--r--   0 runner    (1001) docker     (121)   207410 2022-04-20 06:46:03.000000 av-9.2.0/src/av/data/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   196350 2022-04-20 06:46:02.000000 av-9.2.0/src/av/descriptor.c
+-rw-r--r--   0 runner    (1001) docker     (121)   264785 2022-04-20 06:46:02.000000 av-9.2.0/src/av/dictionary.c
+-rw-r--r--   0 runner    (1001) docker     (121)   631630 2022-04-20 06:46:00.000000 av-9.2.0/src/av/enum.c
+-rw-r--r--   0 runner    (1001) docker     (121)   491609 2022-04-20 06:46:02.000000 av-9.2.0/src/av/error.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/filter/
+-rw-r--r--   0 runner    (1001) docker     (121)   324966 2022-04-20 06:46:08.000000 av-9.2.0/src/av/filter/context.c
+-rw-r--r--   0 runner    (1001) docker     (121)   384289 2022-04-20 06:46:08.000000 av-9.2.0/src/av/filter/filter.c
+-rw-r--r--   0 runner    (1001) docker     (121)   405252 2022-04-20 06:46:09.000000 av-9.2.0/src/av/filter/graph.c
+-rw-r--r--   0 runner    (1001) docker     (121)   222351 2022-04-20 06:46:08.000000 av-9.2.0/src/av/filter/link.c
+-rw-r--r--   0 runner    (1001) docker     (121)   235861 2022-04-20 06:46:08.000000 av-9.2.0/src/av/filter/pad.c
+-rw-r--r--   0 runner    (1001) docker     (121)   305091 2022-04-20 06:46:01.000000 av-9.2.0/src/av/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)   253770 2022-04-20 06:46:00.000000 av-9.2.0/src/av/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   380256 2022-04-20 06:46:02.000000 av-9.2.0/src/av/logging.c
+-rw-r--r--   0 runner    (1001) docker     (121)   306303 2022-04-20 06:46:01.000000 av-9.2.0/src/av/option.c
+-rw-r--r--   0 runner    (1001) docker     (121)   306227 2022-04-20 06:45:59.000000 av-9.2.0/src/av/packet.c
+-rw-r--r--   0 runner    (1001) docker     (121)   198249 2022-04-20 06:46:01.000000 av-9.2.0/src/av/plane.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/sidedata/
+-rw-r--r--   0 runner    (1001) docker     (121)   328581 2022-04-20 06:46:03.000000 av-9.2.0/src/av/sidedata/motionvectors.c
+-rw-r--r--   0 runner    (1001) docker     (121)   351899 2022-04-20 06:46:03.000000 av-9.2.0/src/av/sidedata/sidedata.c
+-rw-r--r--   0 runner    (1001) docker     (121)   345463 2022-04-20 06:46:01.000000 av-9.2.0/src/av/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/subtitles/
+-rw-r--r--   0 runner    (1001) docker     (121)   195630 2022-04-20 06:46:04.000000 av-9.2.0/src/av/subtitles/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   172498 2022-04-20 06:46:04.000000 av-9.2.0/src/av/subtitles/stream.c
+-rw-r--r--   0 runner    (1001) docker     (121)   518211 2022-04-20 06:46:04.000000 av-9.2.0/src/av/subtitles/subtitle.c
+-rw-r--r--   0 runner    (1001) docker     (121)   205617 2022-04-20 06:46:00.000000 av-9.2.0/src/av/utils.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/src/av/video/
+-rw-r--r--   0 runner    (1001) docker     (121)   307286 2022-04-20 06:46:10.000000 av-9.2.0/src/av/video/codeccontext.c
+-rw-r--r--   0 runner    (1001) docker     (121)   398549 2022-04-20 06:46:10.000000 av-9.2.0/src/av/video/format.c
+-rw-r--r--   0 runner    (1001) docker     (121)  1204668 2022-04-20 06:46:10.000000 av-9.2.0/src/av/video/frame.c
+-rw-r--r--   0 runner    (1001) docker     (121)   255746 2022-04-20 06:46:11.000000 av-9.2.0/src/av/video/plane.c
+-rw-r--r--   0 runner    (1001) docker     (121)   278363 2022-04-20 06:46:11.000000 av-9.2.0/src/av/video/reformatter.c
+-rw-r--r--   0 runner    (1001) docker     (121)   190856 2022-04-20 06:46:10.000000 av-9.2.0/src/av/video/stream.c
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 06:46:11.000000 av-9.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 06:45:49.000000 av-9.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-04-20 06:45:49.000000 av-9.2.0/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3085 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_audiofifo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_audioformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_audioframe.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_audiolayout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5828 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_audioresampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3256 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11744 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_codec_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_containerformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (121)      472 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_encode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6256 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14227 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_file_probing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9047 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)      568 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9830 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_python_io.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_seek.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1649 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_subtitles.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2070 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_videoformat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16390 2022-04-20 06:45:49.000000 av-9.2.0/tests/test_videoframe.py
```

### Comparing `av-9.1.1/LICENSE.txt` & `av-9.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `av-9.1.1/PKG-INFO` & `av-9.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: av
-Version: 9.1.1
+Version: 9.2.0
 Summary: Pythonic bindings for FFmpeg's libraries.
 Home-page: https://github.com/PyAV-Org/PyAV
 Author: Mike Boers
 Author-email: pyav@mikeboers.com
 License: BSD
 Project-URL: Bug Reports, https://github.com/PyAV-Org/PyAV/issues
 Project-URL: Documentation, https://pyav.org/docs
```

### Comparing `av-9.1.1/README.md` & `av-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/__init__.py` & `av-9.2.0/av/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,22 @@
-# Add the native FFMPEG and MinGW libraries to executable path, so that the
-# AV pyd files can find them.
 import os
+import sys
 
-if os.name == "nt":
+# Some Python versions distributed by Conda have a buggy `os.add_dll_directory`
+# which prevents binary wheels from finding the FFmpeg DLLs in the `av.libs`
+# directory. We work around this by adding `av.libs` to the PATH.
+if (
+    os.name == "nt"
+    and sys.version_info[:2] in ((3, 8), (3, 9))
+    and os.path.exists(os.path.join(sys.base_prefix, "conda-meta"))
+):
     os.environ["PATH"] = (
-        os.path.abspath(os.path.dirname(__file__)) + os.pathsep + os.environ["PATH"]
+        os.path.abspath(os.path.join(os.path.dirname(__file__), os.pardir, "av.libs"))
+        + os.pathsep
+        + os.environ["PATH"]
     )
 
 # MUST import the core before anything else in order to initalize the underlying
 # library that is being wrapped.
 from av._core import time_base, library_versions
 
 # Capture logging (by importing it).
```

### Comparing `av-9.1.1/av/__main__.py` & `av-9.2.0/av/__main__.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/_core.pyx` & `av-9.2.0/av/_core.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/codeccontext.pyx` & `av-9.2.0/av/audio/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/fifo.pyx` & `av-9.2.0/av/audio/fifo.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/format.pyx` & `av-9.2.0/av/audio/format.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/frame.pxd` & `av-9.2.0/av/audio/frame.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/frame.pyx` & `av-9.2.0/av/audio/frame.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/layout.pyx` & `av-9.2.0/av/audio/layout.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/audio/resampler.pyx` & `av-9.2.0/av/audio/resampler.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/buffer.pyx` & `av-9.2.0/av/buffer.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/bytesource.pyx` & `av-9.2.0/av/bytesource.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/codec/codec.pyx` & `av-9.2.0/av/codec/codec.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/codec/context.pxd` & `av-9.2.0/av/codec/context.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/codec/context.pyx` & `av-9.2.0/av/codec/context.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/container/core.pxd` & `av-9.2.0/av/container/core.pxd`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,18 @@
     cdef lib.AVFormatContext *ptr
 
     cdef readonly object name
     cdef readonly str metadata_encoding
     cdef readonly str metadata_errors
 
     cdef readonly PyIOFile file
+    cdef int buffer_size
     cdef bint input_was_opened
+    cdef readonly object io_open
+    cdef readonly object open_files
 
     cdef readonly ContainerFormat format
 
     cdef readonly dict options
     cdef readonly dict container_options
     cdef readonly list stream_options
```

### Comparing `av-9.1.1/av/container/input.pyx` & `av-9.2.0/av/container/input.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/container/output.pyx` & `av-9.2.0/av/container/output.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,21 @@
 
 
 cdef class OutputContainer(Container):
 
     def __cinit__(self, *args, **kwargs):
         self.streams = StreamContainer()
         self.metadata = {}
+        with nogil:
+            self.packet_ptr = lib.av_packet_alloc()
 
     def __dealloc__(self):
         close_output(self)
+        with nogil:
+            lib.av_packet_free(&self.packet_ptr)
 
     def add_stream(self, codec_name=None, object rate=None, Stream template=None, options=None, **kwargs):
         """add_stream(codec_name, rate=None)
 
         Create a new stream, and return it.
 
         :param str codec_name: The name of a codec.
@@ -215,15 +219,14 @@
         # Assert the packet is in stream time.
         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:
             raise ValueError('Bad Packet stream_index.')
         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
         packet._rebase_time(stream.time_base)
 
         # Make another reference to the packet, as av_interleaved_write_frame
-        # takes ownership of it.
-        cdef lib.AVPacket *packet_ptr = lib.av_packet_alloc()
-        self.err_check(lib.av_packet_ref(packet_ptr, packet.ptr))
+        # takes ownership of the reference.
+        self.err_check(lib.av_packet_ref(self.packet_ptr, packet.ptr))
 
         cdef int ret
         with nogil:
-            ret = lib.av_interleaved_write_frame(self.ptr, packet_ptr)
+            ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)
         self.err_check(ret)
```

### Comparing `av-9.1.1/av/container/pyio.pyx` & `av-9.2.0/av/container/pyio.pyx`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
         readable = getattr(self.file, 'readable', None)
         writable = getattr(self.file, 'writable', None)
         seekable = getattr(self.file, 'seekable', None)
         self.fread = getattr(self.file, 'read', None)
         self.fwrite = getattr(self.file, 'write', None)
         self.fseek = getattr(self.file, 'seek', None)
         self.ftell = getattr(self.file, 'tell', None)
+        self.fclose = getattr(self.file, 'close', None)
 
         # To be seekable the file object must have `seek` and `tell` methods.
         # If it also has a `seekable` method, it must return True.
         if (
             self.fseek is not None
             and self.ftell is not None
             and (seekable is None or seekable())
@@ -139,7 +140,30 @@
             if self.pos_is_valid:
                 res = self.pos
             else:
                 res = self.ftell()
         return res
     except Exception as e:
         return stash_exception()
+
+
+cdef void pyio_close_gil(lib.AVIOContext *pb):
+    try:
+        lib.avio_close(pb)
+
+    except Exception as e:
+        stash_exception()
+
+
+cdef void pyio_close_custom_gil(lib.AVIOContext *pb):
+    cdef PyIOFile self
+    try:
+        self = <PyIOFile>pb.opaque
+
+        # Flush bytes in the AVIOContext buffers to the custom I/O
+        lib.avio_flush(pb)
+
+        if self.fclose is not None:
+            self.fclose()
+
+    except Exception as e:
+        stash_exception()
```

### Comparing `av-9.1.1/av/container/streams.pyx` & `av-9.2.0/av/container/streams.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/data/stream.pyx` & `av-9.2.0/av/data/stream.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/datasets.py` & `av-9.2.0/av/datasets.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/deprecation.py` & `av-9.2.0/av/deprecation.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/descriptor.pxd` & `av-9.2.0/av/descriptor.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/descriptor.pyx` & `av-9.2.0/av/descriptor.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/dictionary.pyx` & `av-9.2.0/av/dictionary.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/enum.pyx` & `av-9.2.0/av/enum.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -380,10 +380,11 @@
 cpdef define_enum(name, module, items, bint is_flags=False):
 
     if is_flags:
         base_cls = EnumFlag
     else:
         base_cls = EnumItem
 
-    cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+    # Some items may be None if they correspond to an unsupported FFmpeg feature
+    cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])
 
     return cls
```

### Comparing `av-9.1.1/av/error.pyx` & `av-9.2.0/av/error.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/context.pyx` & `av-9.2.0/av/filter/context.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/filter.pyx` & `av-9.2.0/av/filter/filter.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/graph.pyx` & `av-9.2.0/av/filter/graph.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/link.pyx` & `av-9.2.0/av/filter/link.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/pad.pxd` & `av-9.2.0/av/filter/pad.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/filter/pad.pyx` & `av-9.2.0/av/filter/pad.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/format.pyx` & `av-9.2.0/av/format.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/frame.pyx` & `av-9.2.0/av/frame.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/logging.pyx` & `av-9.2.0/av/logging.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/option.pyx` & `av-9.2.0/av/option.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/packet.pyx` & `av-9.2.0/av/packet.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/plane.pyx` & `av-9.2.0/av/plane.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/sidedata/motionvectors.pyx` & `av-9.2.0/av/sidedata/motionvectors.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/sidedata/sidedata.pyx` & `av-9.2.0/av/sidedata/sidedata.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     ('SKIP_SAMPLES', lib.AV_FRAME_DATA_SKIP_SAMPLES),
     ('AUDIO_SERVICE_TYPE', lib.AV_FRAME_DATA_AUDIO_SERVICE_TYPE),
     ('MASTERING_DISPLAY_METADATA', lib.AV_FRAME_DATA_MASTERING_DISPLAY_METADATA),
     ('GOP_TIMECODE', lib.AV_FRAME_DATA_GOP_TIMECODE),
     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),
     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
+    # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,
 
     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
     # ('QP_TABLE_PROPERTIES', lib.AV_FRAME_DATA_QP_TABLE_PROPERTIES),
     # ('QP_TABLE_DATA', lib.AV_FRAME_DATA_QP_TABLE_DATA),
 
 ))
```

### Comparing `av-9.1.1/av/stream.pxd` & `av-9.2.0/av/stream.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/stream.pyx` & `av-9.2.0/av/stream.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/subtitles/codeccontext.pyx` & `av-9.2.0/av/subtitles/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/subtitles/subtitle.pxd` & `av-9.2.0/av/subtitles/subtitle.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/subtitles/subtitle.pyx` & `av-9.2.0/av/subtitles/subtitle.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/utils.pxd` & `av-9.2.0/av/utils.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/utils.pyx` & `av-9.2.0/av/utils.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/codeccontext.pyx` & `av-9.2.0/av/video/codeccontext.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/format.pxd` & `av-9.2.0/av/video/format.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/format.pyx` & `av-9.2.0/av/video/format.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/frame.pxd` & `av-9.2.0/av/video/frame.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/frame.pyx` & `av-9.2.0/av/video/frame.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/plane.pyx` & `av-9.2.0/av/video/plane.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av/video/reformatter.pyx` & `av-9.2.0/av/video/reformatter.pyx`

 * *Files identical despite different names*

### Comparing `av-9.1.1/av.egg-info/PKG-INFO` & `av-9.2.0/av.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: av
-Version: 9.1.1
+Version: 9.2.0
 Summary: Pythonic bindings for FFmpeg's libraries.
 Home-page: https://github.com/PyAV-Org/PyAV
 Author: Mike Boers
 Author-email: pyav@mikeboers.com
 License: BSD
 Project-URL: Bug Reports, https://github.com/PyAV-Org/PyAV/issues
 Project-URL: Documentation, https://pyav.org/docs
```

### Comparing `av-9.1.1/av.egg-info/SOURCES.txt` & `av-9.2.0/av.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 flags.txt
 pyproject.toml
 setup.cfg
 setup.py
+av/__init__.pxd
 av/__init__.py
 av/__main__.py
 av/_core.pyx
 av/about.py
 av/buffer.pxd
 av/buffer.pyx
 av/bytesource.pxd
@@ -41,14 +42,15 @@
 av/utils.pyx
 av.egg-info/PKG-INFO
 av.egg-info/SOURCES.txt
 av.egg-info/dependency_links.txt
 av.egg-info/entry_points.txt
 av.egg-info/not-zip-safe
 av.egg-info/top_level.txt
+av/audio/__init__.pxd
 av/audio/__init__.py
 av/audio/codeccontext.pxd
 av/audio/codeccontext.pyx
 av/audio/fifo.pxd
 av/audio/fifo.pyx
 av/audio/format.pxd
 av/audio/format.pyx
@@ -58,56 +60,63 @@
 av/audio/layout.pyx
 av/audio/plane.pxd
 av/audio/plane.pyx
 av/audio/resampler.pxd
 av/audio/resampler.pyx
 av/audio/stream.pxd
 av/audio/stream.pyx
+av/codec/__init__.pxd
 av/codec/__init__.py
 av/codec/codec.pxd
 av/codec/codec.pyx
 av/codec/context.pxd
 av/codec/context.pyx
+av/container/__init__.pxd
 av/container/__init__.py
 av/container/core.pxd
 av/container/core.pyx
 av/container/input.pxd
 av/container/input.pyx
 av/container/output.pxd
 av/container/output.pyx
 av/container/pyio.pxd
 av/container/pyio.pyx
 av/container/streams.pxd
 av/container/streams.pyx
+av/data/__init__.pxd
 av/data/__init__.py
 av/data/stream.pxd
 av/data/stream.pyx
+av/filter/__init__.pxd
 av/filter/__init__.py
 av/filter/context.pxd
 av/filter/context.pyx
 av/filter/filter.pxd
 av/filter/filter.pyx
 av/filter/graph.pxd
 av/filter/graph.pyx
 av/filter/link.pxd
 av/filter/link.pyx
 av/filter/pad.pxd
 av/filter/pad.pyx
+av/sidedata/__init__.pxd
 av/sidedata/__init__.py
 av/sidedata/motionvectors.pxd
 av/sidedata/motionvectors.pyx
 av/sidedata/sidedata.pxd
 av/sidedata/sidedata.pyx
+av/subtitles/__init__.pxd
 av/subtitles/__init__.py
 av/subtitles/codeccontext.pxd
 av/subtitles/codeccontext.pyx
 av/subtitles/stream.pxd
 av/subtitles/stream.pyx
 av/subtitles/subtitle.pxd
 av/subtitles/subtitle.pyx
+av/video/__init__.pxd
 av/video/__init__.py
 av/video/codeccontext.pxd
 av/video/codeccontext.pyx
 av/video/format.pxd
 av/video/format.pyx
 av/video/frame.pxd
 av/video/frame.pyx
```

### Comparing `av-9.1.1/docs/api/audio.rst` & `av-9.2.0/docs/api/audio.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/codec.rst` & `av-9.2.0/docs/api/codec.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/container.rst` & `av-9.2.0/docs/api/container.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/error.rst` & `av-9.2.0/docs/api/error.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/error_table.py` & `av-9.2.0/docs/api/error_table.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/stream.rst` & `av-9.2.0/docs/api/stream.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/time.rst` & `av-9.2.0/docs/api/time.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/api/video.rst` & `av-9.2.0/docs/api/video.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/conf.py` & `av-9.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/cookbook/basics.rst` & `av-9.2.0/docs/cookbook/basics.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/cookbook/numpy.rst` & `av-9.2.0/docs/cookbook/numpy.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/development/includes.py` & `av-9.2.0/docs/development/includes.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/index.rst` & `av-9.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/overview/caveats.rst` & `av-9.2.0/docs/overview/caveats.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/docs/overview/installation.rst` & `av-9.2.0/docs/overview/installation.rst`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/basics/parse.py` & `av-9.2.0/examples/basics/parse.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/basics/remux.py` & `av-9.2.0/examples/basics/remux.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/basics/save_keyframes.py` & `av-9.2.0/examples/basics/save_keyframes.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/basics/thread_type.py` & `av-9.2.0/examples/basics/thread_type.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/numpy/barcode.py` & `av-9.2.0/examples/numpy/barcode.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/numpy/generate_video.py` & `av-9.2.0/examples/numpy/generate_video.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/examples/numpy/generate_video_with_pts.py` & `av-9.2.0/examples/numpy/generate_video_with_pts.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/flags.txt` & `av-9.2.0/flags.txt`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libav.pxd` & `av-9.2.0/include/libav.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavcodec/avcodec.pxd` & `av-9.2.0/include/libavcodec/avcodec.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,22 @@
     uint16_t, int16_t,
     uint32_t, int32_t,
     uint64_t, int64_t
 )
 
 
 cdef extern from "libavcodec/avcodec.h" nogil:
+    """
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    """
 
     # custom
     cdef set pyav_get_available_codecs()
 
     cdef int   avcodec_version()
     cdef char* avcodec_configuration()
     cdef char* avcodec_license()
@@ -279,14 +287,15 @@
         AV_FRAME_DATA_MASTERING_DISPLAY_METADATA
         AV_FRAME_DATA_GOP_TIMECODE
         AV_FRAME_DATA_SPHERICAL
         AV_FRAME_DATA_CONTENT_LIGHT_LEVEL
         AV_FRAME_DATA_ICC_PROFILE
         AV_FRAME_DATA_QP_TABLE_PROPERTIES
         AV_FRAME_DATA_QP_TABLE_DATA
+        AV_FRAME_DATA_SEI_UNREGISTERED
 
     cdef struct AVFrameSideData:
         AVFrameSideDataType type
         uint8_t *data
         int size
         AVDictionary *metadata
```

### Comparing `av-9.1.1/include/libavfilter/avfilter.pxd` & `av-9.2.0/include/libavfilter/avfilter.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavfilter/avfiltergraph.pxd` & `av-9.2.0/include/libavfilter/avfiltergraph.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavformat/avformat.pxd` & `av-9.2.0/include/libavformat/avformat.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     cdef struct AVIOContext:
         unsigned char* buffer
         int buffer_size
         int write_flag
         int direct
         int seekable
         int max_packet_size
+        void *opaque
 
     # http://ffmpeg.org/doxygen/trunk/structAVIOInterruptCB.html
     cdef struct AVIOInterruptCB:
         int (*callback)(void*)
         void *opaque
 
     cdef int AVIO_FLAG_DIRECT
@@ -181,14 +182,27 @@
         int64_t start_time
         int64_t duration
         int bit_rate
 
         int flags
         int64_t max_analyze_duration
 
+        void *opaque
+
+        int (*io_open)(
+            AVFormatContext *s,
+            AVIOContext **pb,
+            const char *url,
+            int flags,
+            AVDictionary **options
+        )
+        void (*io_close)(
+            AVFormatContext *s,
+            AVIOContext *pb
+        )
 
     cdef AVFormatContext* avformat_alloc_context()
 
     # .. c:function:: avformat_open_input(...)
     #
     #       Options are passed via :func:`av.open`.
     #
@@ -245,14 +259,16 @@
 
     cdef int avformat_query_codec(
         AVOutputFormat *ofmt,
         AVCodecID codec_id,
         int std_compliance
     )
 
+    cdef void avio_flush(AVIOContext *s)
+
     cdef int avio_close(AVIOContext *s)
 
     cdef int avio_closep(AVIOContext **s)
 
     cdef int avformat_find_stream_info(
         AVFormatContext *ctx,
         AVDictionary **options, # Can be NULL.
```

### Comparing `av-9.1.1/include/libavutil/avutil.pxd` & `av-9.2.0/include/libavutil/avutil.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavutil/dict.pxd` & `av-9.2.0/include/libavutil/dict.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavutil/error.pxd` & `av-9.2.0/include/libavutil/error.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavutil/frame.pxd` & `av-9.2.0/include/libavutil/frame.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libavutil/samplefmt.pxd` & `av-9.2.0/include/libavutil/samplefmt.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libswresample/swresample.pxd` & `av-9.2.0/include/libswresample/swresample.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/include/libswscale/swscale.pxd` & `av-9.2.0/include/libswscale/swscale.pxd`

 * *Files identical despite different names*

### Comparing `av-9.1.1/setup.cfg` & `av-9.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `av-9.1.1/setup.py` & `av-9.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import argparse
 import os
+import pathlib
 import platform
 import re
 import shlex
 import subprocess
 import sys
 
 from Cython.Build import cythonize
@@ -174,23 +175,27 @@
 
 # Read package metadata
 about = {}
 about_file = os.path.join(os.path.dirname(__file__), "av", "about.py")
 with open(about_file, encoding="utf-8") as fp:
     exec(fp.read(), about)
 
+package_folders = pathlib.Path("av").glob("**/")
+package_data = {".".join(pckg.parts): ["*.pxd"] for pckg in package_folders}
+
 
 setup(
     name="av",
     version=about["__version__"],
     description="Pythonic bindings for FFmpeg's libraries.",
     author="Mike Boers",
     author_email="pyav@mikeboers.com",
     url="https://github.com/PyAV-Org/PyAV",
     packages=find_packages(exclude=["build*", "examples*", "scratchpad*", "tests*"]),
+    package_data=package_data,
     zip_safe=False,
     ext_modules=ext_modules,
     test_suite="tests",
     entry_points={
         "console_scripts": [
             "pyav = av.__main__:main",
         ],
```

### Comparing `av-9.1.1/src/av/_core.c` & `av-9.2.0/src/av/_core.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/audio/codeccontext.c` & `av-9.2.0/src/av/audio/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1275,28 +1283,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1360,15 +1369,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4129,18 +4141,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.codec"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_5codec_Codec = __Pyx_ImportType(__pyx_t_1, "av.codec.codec", "Codec", sizeof(struct __pyx_obj_2av_5codec_5codec_Codec), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_5codec_Codec) __PYX_ERR(6, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_5codec_Codec = (struct __pyx_vtabstruct_2av_5codec_5codec_Codec*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_5codec_Codec->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_5codec_Codec)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(8, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/audio/fifo.c` & `av-9.2.0/src/av/audio/fifo.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1277,28 +1285,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1362,15 +1371,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4851,18 +4863,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(8, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(8, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(9, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(9, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(10, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(10, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/audio/format.c` & `av-9.2.0/src/av/audio/format.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/audio/frame.c` & `av-9.2.0/src/av/audio/frame.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1253,28 +1261,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1338,15 +1347,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -5298,18 +5310,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(7, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(7, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(8, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(8, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(9, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(9, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/audio/layout.c` & `av-9.2.0/src/av/audio/layout.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/audio/plane.c` & `av-9.2.0/src/av/audio/plane.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1175,28 +1183,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1260,15 +1269,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2695,18 +2707,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(6, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(8, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/audio/resampler.c` & `av-9.2.0/src/av/audio/resampler.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1239,28 +1247,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1324,15 +1333,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4512,18 +4524,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(8, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(8, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(9, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(9, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(10, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(10, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/audio/stream.c` & `av-9.2.0/src/av/audio/stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1242,28 +1250,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1313,15 +1322,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2612,18 +2624,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/buffer.c` & `av-9.2.0/src/av/buffer.c`

 * *Files identical despite different names*

### Comparing `av-9.1.1/src/av/bytesource.c` & `av-9.2.0/src/av/bytesource.c`

 * *Files identical despite different names*

### Comparing `av-9.1.1/src/av/codec/codec.c` & `av-9.2.0/src/av/codec/codec.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/codec/context.c` & `av-9.2.0/src/av/codec/context.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1206,28 +1214,29 @@
  */
 struct __pyx_obj_2av_6buffer_Buffer {
   PyObject_HEAD
   struct __pyx_vtabstruct_2av_6buffer_Buffer *__pyx_vtab;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1291,15 +1300,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -10175,18 +10187,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.buffer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_6buffer_Buffer = __Pyx_ImportType(__pyx_t_1, "av.buffer", "Buffer", sizeof(struct __pyx_obj_2av_6buffer_Buffer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_6buffer_Buffer) __PYX_ERR(5, 2, __pyx_L1_error)
   __pyx_vtabptr_2av_6buffer_Buffer = (struct __pyx_vtabstruct_2av_6buffer_Buffer*)__Pyx_GetVtable(__pyx_ptype_2av_6buffer_Buffer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_6buffer_Buffer)) __PYX_ERR(5, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/container/core.c` & `av-9.2.0/src/av/container/core.c`

 * *Files 2% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1167,37 +1175,38 @@
  *     double timeout
  */
 struct __pyx_t_2av_9container_4core_timeout_info {
   double start_time;
   double timeout;
 };
 
-/* "av/container/core.pyx":22
+/* "av/container/core.pyx":23
  * 
  * 
  * ctypedef int64_t (*seek_func_t)(void *opaque, int64_t offset, int whence) nogil             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef int64_t (*__pyx_t_2av_9container_4core_seek_func_t)(void *, int64_t, int);
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1409,15 +1418,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -1445,31 +1457,32 @@
  * 
  *     cdef bint _started
  */
 struct __pyx_obj_2av_9container_6output_OutputContainer {
   struct __pyx_obj_2av_9container_4core_Container __pyx_base;
   int _started;
   int _done;
+  struct AVPacket *packet_ptr;
 };
 
 
-/* "av/container/core.pyx":207
+/* "av/container/core.pyx":294
  *         return err_check(value, filename=self.name)
  * 
  *     def dumps_format(self):             # <<<<<<<<<<<<<<
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  */
 struct __pyx_obj_2av_9container_4core___pyx_scope_struct__dumps_format {
   PyObject_HEAD
   PyObject *__pyx_v_logs;
 };
 
 
-/* "av/container/core.pyx":210
+/* "av/container/core.pyx":297
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)             # <<<<<<<<<<<<<<
  * 
  *     cdef set_timeout(self, timeout):
  */
 struct __pyx_obj_2av_9container_4core___pyx_scope_struct_1_genexpr {
@@ -1625,15 +1638,15 @@
 
 struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer {
   PyObject *(*add_stream)(struct __pyx_obj_2av_9container_7streams_StreamContainer *, struct __pyx_obj_2av_6stream_Stream *);
 };
 static struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer *__pyx_vtabptr_2av_9container_7streams_StreamContainer;
 
 
-/* "av/container/core.pyx":95
+/* "av/container/core.pyx":171
  * 
  * 
  * cdef class Container(object):             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, sentinel, file_, format_name, options,
  */
 
@@ -1839,14 +1852,72 @@
 #endif
 
 /* WriteUnraisableException.proto */
 static void __Pyx_WriteUnraisable(const char *name, int clineno,
                                   int lineno, const char *filename,
                                   int full_traceback, int nogil);
 
+/* SetItemInt.proto */
+#define __Pyx_SetItemInt(o, i, v, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_SetItemInt_Fast(o, (Py_ssize_t)i, v, is_list, wraparound, boundscheck) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
+               __Pyx_SetItemInt_Generic(o, to_py_func(i), v)))
+static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v);
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v,
+                                               int is_list, int wraparound, int boundscheck);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
+/* SaveResetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+#else
+#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
+#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
+#endif
+
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+#else
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#endif
+
+/* GetException.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
+#endif
+
+/* PySequenceContains.proto */
+static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
+    int result = PySequence_Contains(seq, item);
+    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
+}
+
+/* DelItemInt.proto */
+#define __Pyx_DelItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
+    (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
+    __Pyx_DelItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound) :\
+    (is_list ? (PyErr_SetString(PyExc_IndexError, "list assignment index out of range"), -1) :\
+               __Pyx_DelItem_Generic(o, to_py_func(i))))
+static int __Pyx_DelItem_Generic(PyObject *o, PyObject *j);
+static CYTHON_INLINE int __Pyx_DelItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                               int is_list, int wraparound);
+
 /* RaiseArgTupleInvalid.proto */
 static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
     Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
 
 /* RaiseDoubleKeywords.proto */
 static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
 
@@ -1854,22 +1925,14 @@
 static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
     PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
     const char* function_name);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
-#else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
-#endif
-
 /* GetAttr.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* ListCompAppend.proto */
@@ -2092,19 +2155,22 @@
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
@@ -2116,30 +2182,14 @@
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
-/* SaveResetException.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-#else
-#define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
-#define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
-#endif
-
 /* SwapException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSwap(type, value, tb)  __Pyx__ExceptionSwap(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static CYTHON_INLINE void __Pyx_ExceptionSwap(PyObject **type, PyObject **value, PyObject **tb);
 #endif
@@ -2241,14 +2291,16 @@
 
 /* Module declarations from 'libc.stdint' */
 
 /* Module declarations from 'libav' */
 
 /* Module declarations from 'av.container.pyio' */
 static PyTypeObject *__pyx_ptype_2av_9container_4pyio_PyIOFile = 0;
+static void (*__pyx_f_2av_9container_4pyio_pyio_close_gil)(struct AVIOContext *); /*proto*/
+static void (*__pyx_f_2av_9container_4pyio_pyio_close_custom_gil)(struct AVIOContext *); /*proto*/
 
 /* Module declarations from 'cpython.buffer' */
 
 /* Module declarations from 'av.bytesource' */
 static PyTypeObject *__pyx_ptype_2av_10bytesource_ByteSource = 0;
 
 /* Module declarations from 'av.codec.codec' */
@@ -2307,26 +2359,30 @@
 /* Module declarations from 'av.container.core' */
 static PyTypeObject *__pyx_ptype_2av_9container_4core_Container = 0;
 static PyTypeObject *__pyx_ptype_2av_9container_4core___pyx_scope_struct__dumps_format = 0;
 static PyTypeObject *__pyx_ptype_2av_9container_4core___pyx_scope_struct_1_genexpr = 0;
 static PyObject *__pyx_v_2av_9container_4core__cinit_sentinel = 0;
 static PyObject *__pyx_v_2av_9container_4core_clock = 0;
 static int __pyx_f_2av_9container_4core_interrupt_cb(void *); /*proto*/
+static int __pyx_f_2av_9container_4core_pyav_io_open(struct AVFormatContext *, struct AVIOContext **, char const *, int, AVDictionary **); /*proto*/
+static int __pyx_f_2av_9container_4core_pyav_io_open_gil(struct AVFormatContext *, struct AVIOContext **, char const *, int, AVDictionary **); /*proto*/
+static void __pyx_f_2av_9container_4core_pyav_io_close(struct AVFormatContext *, struct AVIOContext *); /*proto*/
+static void __pyx_f_2av_9container_4core_pyav_io_close_gil(struct AVFormatContext *, struct AVIOContext *); /*proto*/
 #define __Pyx_MODULE_NAME "av.container.core"
 extern int __pyx_module_is_main_av__container__core;
 int __pyx_module_is_main_av__container__core = 0;
 
 /* Implementation of 'av.container.core' */
 static PyObject *__pyx_builtin_object;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static const char __pyx_k_r[] = "r";
 static const char __pyx_k_w[] = "w";
-static const char __pyx_k__6[] = "";
+static const char __pyx_k__2[] = "";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_exit[] = "__exit__";
 static const char __pyx_k_file[] = "file_";
 static const char __pyx_k_join[] = "join";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_mode[] = "mode";
@@ -2358,14 +2414,15 @@
 static const char __pyx_k_Capture[] = "Capture";
 static const char __pyx_k_NOPARSE[] = "NOPARSE";
 static const char __pyx_k_exc_val[] = "exc_val";
 static const char __pyx_k_gen_pts[] = "gen_pts";
 static const char __pyx_k_genexpr[] = "genexpr";
 static const char __pyx_k_ign_dts[] = "ign_dts";
 static const char __pyx_k_ign_idx[] = "ign_idx";
+static const char __pyx_k_io_open[] = "io_open";
 static const char __pyx_k_options[] = "options";
 static const char __pyx_k_timeout[] = "timeout";
 static const char __pyx_k_AUTO_BSF[] = "AUTO_BSF";
 static const char __pyx_k_BITEXACT[] = "BITEXACT";
 static const char __pyx_k_NOBUFFER[] = "NOBUFFER";
 static const char __pyx_k_NOFILLIN[] = "NOFILLIN";
 static const char __pyx_k_NONBLOCK[] = "NONBLOCK";
@@ -2409,15 +2466,15 @@
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_open_timeout[] = "open_timeout";
 static const char __pyx_k_read_timeout[] = "read_timeout";
 static const char __pyx_k_FLUSH_PACKETS[] = "FLUSH_PACKETS";
 static const char __pyx_k_av_dictionary[] = "av.dictionary";
 static const char __pyx_k_flag_property[] = "flag_property";
 static const char __pyx_k_flush_packets[] = "flush_packets";
-static const char __pyx_k_open_line_251[] = "open (line 251)";
+static const char __pyx_k_open_line_338[] = "open (line 338)";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_stream_options[] = "stream_options";
 static const char __pyx_k_DISCARD_CORRUPT[] = "DISCARD_CORRUPT";
 static const char __pyx_k_discard_corrupt[] = "discard_corrupt";
 static const char __pyx_k_metadata_errors[] = "metadata_errors";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_av_container_core[] = "av.container.core";
@@ -2445,15 +2502,15 @@
 static const char __pyx_k_Ignore_DTS_on_frames_that_contai[] = "Ignore DTS on frames that contain both DTS & PTS.";
 static const char __pyx_k_Provide_stream_options_via_Conta[] = "Provide stream options via Container.add_stream(..., options={}).";
 static const char __pyx_k_Stop_muxing_when_the_shortest_st[] = "Stop muxing when the shortest stream stops.";
 static const char __pyx_k_The_caller_has_supplied_a_custom[] = "The caller has supplied a custom AVIOContext, don't avio_close() it.";
 static const char __pyx_k_Try_to_interleave_outputted_pack[] = "Try to interleave outputted packets by dts (using this flag can slow demuxing down).";
 static const char __pyx_k_When_muxing_try_to_avoid_writing[] = "When muxing, try to avoid writing any random/volatile data to the output.\n\n        This includes any random IDs, real-time timestamps/dates, muxer version, etc.\n        This flag is mainly intended for testing.";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static const char __pyx_k_open_file_mode_r_kwargs_Main_ent[] = "open(file, mode='r', **kwargs)\n\n    Main entrypoint to opening files/streams.\n\n    :param str file: The file to open, which can be either a string or a file-like object.\n    :param str mode: ``\"r\"`` for reading and ``\"w\"`` for writing.\n    :param str format: Specific format to use. Defaults to autodect.\n    :param dict options: Options to pass to the container and all streams.\n    :param dict container_options: Options to pass to the container.\n    :param list stream_options: Options to pass to each stream.\n    :param str metadata_encoding: Encoding to use when reading or writing file metadata.\n        Defaults to ``\"utf-8\"``.\n    :param str metadata_errors: Specifies how to handle encoding errors; behaves like\n        ``str.encode`` parameter. Defaults to ``\"strict\"``.\n    :param int buffer_size: Size of buffer for Python input/output operations in bytes.\n        Honored only when ``file`` is a file-like object. Defaults to 32768 (32k).\n    :param timeout: How many seconds to wait for data before giving up, as a float, or a\n        :ref:`(open timeout, read timeout) <timeouts>` tuple.\n    :type timeout: float or tuple\n\n    For devices (via ``libavdevice``), pass the name of the device to ``format``,\n    e.g.::\n\n        >>> # Open webcam on OS X.\n        >>> av.open(format='avfoundation', file='0') # doctest: +SKIP\n\n    .. seealso:: :ref:`garbage_collection`\n\n    More information on using input and output devices is available on the\n    `FFmpeg website <https://www.ffmpeg.org/ffmpeg-devices.html>`_.\n    ";
+static const char __pyx_k_open_file_mode_r_kwargs_Main_ent[] = "open(file, mode='r', **kwargs)\n\n    Main entrypoint to opening files/streams.\n\n    :param str file: The file to open, which can be either a string or a file-like object.\n    :param str mode: ``\"r\"`` for reading and ``\"w\"`` for writing.\n    :param str format: Specific format to use. Defaults to autodect.\n    :param dict options: Options to pass to the container and all streams.\n    :param dict container_options: Options to pass to the container.\n    :param list stream_options: Options to pass to each stream.\n    :param str metadata_encoding: Encoding to use when reading or writing file metadata.\n        Defaults to ``\"utf-8\"``.\n    :param str metadata_errors: Specifies how to handle encoding errors; behaves like\n        ``str.encode`` parameter. Defaults to ``\"strict\"``.\n    :param int buffer_size: Size of buffer for Python input/output operations in bytes.\n        Honored only when ``file`` is a file-like object. Defaults to 32768 (32k).\n    :param timeout: How many seconds to wait for data before giving up, as a float, or a\n        :ref:`(open timeout, read timeout) <timeouts>` tuple.\n    :type timeout: float or tuple\n    :param callable io_open: Custom I/O callable for opening files/streams.\n        This option is intended for formats that need to open additional\n        file-like objects to ``file`` using custom I/O.\n        The callable signature is ``io_open(url: str, flags: int, options: dict)``, where\n        ``url`` is the url to open, ``flags`` is a combination of AVIO_FLAG_* and\n        ``options`` is a dictionary of additional options. The callable should return a\n        file-like object.\n\n    For devices (via ``libavdevice``), pass the name of the device to ``format``,\n    e.g.::\n\n        >>> # Open webcam on OS X.\n        >>> av.open(format='avfoundation', file='0') # doctest: +SKIP\n\n    For DASH and custom I/O using ``io_open``, add a protocol prefix to the ``file`` to\n    prevent the DASH encoder defaulting t""o the file protocol and using temporary files.\n    The custom I/O callable can be used to remove the protocol prefix to reveal the actual\n    name for creating the file-like object. E.g.::\n\n        >>> av.open(\"customprotocol://manifest.mpd\", \"w\", io_open=custom_io) # doctest: +SKIP\n\n    .. seealso:: :ref:`garbage_collection`\n\n    More information on using input and output devices is available on the\n    `FFmpeg website <https://www.ffmpeg.org/ffmpeg-devices.html>`_.\n    ";
 static PyObject *__pyx_n_s_AUTO_BSF;
 static PyObject *__pyx_kp_s_Add_bitstream_filters_as_request;
 static PyObject *__pyx_n_s_BITEXACT;
 static PyObject *__pyx_n_s_CUSTOM_IO;
 static PyObject *__pyx_n_s_Capture;
 static PyObject *__pyx_kp_s_Clock_has_been_changed_to_before;
 static PyObject *__pyx_n_s_Container;
@@ -2491,15 +2548,15 @@
 static PyObject *__pyx_n_s_SORT_DTS;
 static PyObject *__pyx_kp_s_Stop_muxing_when_the_shortest_st;
 static PyObject *__pyx_kp_s_The_caller_has_supplied_a_custom;
 static PyObject *__pyx_kp_s_Try_to_interleave_outputted_pack;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_kp_s_When_muxing_try_to_avoid_writing;
-static PyObject *__pyx_kp_s__6;
+static PyObject *__pyx_kp_s__2;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_auto_bsf;
 static PyObject *__pyx_n_s_av_container_core;
 static PyObject *__pyx_kp_s_av_container_core_pyx;
 static PyObject *__pyx_n_s_av_dictionary;
 static PyObject *__pyx_n_s_av_logging;
 static PyObject *__pyx_kp_s_av_s_r;
@@ -2530,14 +2587,15 @@
 static PyObject *__pyx_n_s_gen_pts;
 static PyObject *__pyx_n_s_genexpr;
 static PyObject *__pyx_n_s_get_flags;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_ign_dts;
 static PyObject *__pyx_n_s_ign_idx;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_io_open;
 static PyObject *__pyx_n_s_join;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_metadata_encoding;
 static PyObject *__pyx_n_s_metadata_errors;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_kp_s_mode_must_be_r_or_w_got_r;
 static PyObject *__pyx_n_s_monotonic;
@@ -2548,15 +2606,15 @@
 static PyObject *__pyx_n_s_no_fill_in;
 static PyObject *__pyx_n_s_no_parse;
 static PyObject *__pyx_n_s_non_block;
 static PyObject *__pyx_kp_s_none;
 static PyObject *__pyx_n_s_object;
 static PyObject *__pyx_n_s_open;
 static PyObject *__pyx_kp_u_open_file_mode_r_kwargs_Main_ent;
-static PyObject *__pyx_kp_u_open_line_251;
+static PyObject *__pyx_kp_u_open_line_338;
 static PyObject *__pyx_n_s_open_timeout;
 static PyObject *__pyx_n_s_options;
 static PyObject *__pyx_n_s_os;
 static PyObject *__pyx_n_s_priv_opt;
 static PyObject *__pyx_n_s_property;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_r;
@@ -2576,56 +2634,58 @@
 static PyObject *__pyx_n_s_strict;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_throw;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_timeout;
 static PyObject *__pyx_kp_s_utf_8;
 static PyObject *__pyx_n_s_w;
-static int __pyx_pf_2av_9container_4core_9Container___cinit__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, PyObject *__pyx_v_sentinel, PyObject *__pyx_v_file_, PyObject *__pyx_v_format_name, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_open_timeout, PyObject *__pyx_v_read_timeout); /* proto */
+static int __pyx_pf_2av_9container_4core_9Container___cinit__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, PyObject *__pyx_v_sentinel, PyObject *__pyx_v_file_, PyObject *__pyx_v_format_name, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_open_timeout, PyObject *__pyx_v_read_timeout, PyObject *__pyx_v_io_open); /* proto */
 static void __pyx_pf_2av_9container_4core_9Container_2__dealloc__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_4__enter__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_6__exit__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_type, CYTHON_UNUSED PyObject *__pyx_v_exc_val, CYTHON_UNUSED PyObject *__pyx_v_exc_tb); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_8__repr__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_12dumps_format_genexpr(PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_10dumps_format(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_12_get_flags(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_14_set_flags(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_9writeable___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_4name___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_17metadata_encoding___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_15metadata_errors___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_4file___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_2av_9container_4core_9Container_7io_open___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_2av_9container_4core_9Container_10open_files___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_6format___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_7options___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_17container_options___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_14stream_options___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_7streams___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_8metadata___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_12open_timeout___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_12read_timeout___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_16__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2av_9container_4core_9Container_18__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_2av_9container_4core_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file, PyObject *__pyx_v_mode, PyObject *__pyx_v_format, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_timeout); /* proto */
+static PyObject *__pyx_pf_2av_9container_4core_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file, PyObject *__pyx_v_mode, PyObject *__pyx_v_format, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_timeout, PyObject *__pyx_v_io_open); /* proto */
 static PyObject *__pyx_tp_new_2av_9container_4core_Container(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_2av_9container_4core___pyx_scope_struct__dumps_format(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_2av_9container_4core___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_32768;
 static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_codeobj__11;
 /* Late includes */
 
-/* "av/container/core.pyx":31
+/* "av/container/core.pyx":32
  * cdef object clock = getattr(time, 'monotonic', time.time)
  * 
  * cdef int interrupt_cb (void *p) nogil:             # <<<<<<<<<<<<<<
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)
  */
 
@@ -2644,67 +2704,67 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_RefNannySetupContext("interrupt_cb", 1);
 
-  /* "av/container/core.pyx":33
+  /* "av/container/core.pyx":34
  * cdef int interrupt_cb (void *p) nogil:
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)             # <<<<<<<<<<<<<<
  *     if info.timeout < 0:  # timeout < 0 means no timeout
  *         return 0
  */
   /*try:*/ {
     __pyx_v_info = (*((__pyx_t_2av_9container_4core_timeout_info *)__pyx_v_p));
 
-    /* "av/container/core.pyx":34
+    /* "av/container/core.pyx":35
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)
  *     if info.timeout < 0:  # timeout < 0 means no timeout             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     __pyx_t_1 = ((__pyx_v_info.timeout < 0.0) != 0);
     if (__pyx_t_1) {
 
-      /* "av/container/core.pyx":35
+      /* "av/container/core.pyx":36
  *     cdef timeout_info info = dereference(<timeout_info*> p)
  *     if info.timeout < 0:  # timeout < 0 means no timeout
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     cdef double current_time
  */
       __pyx_r = 0;
       goto __pyx_L3_return;
 
-      /* "av/container/core.pyx":34
+      /* "av/container/core.pyx":35
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)
  *     if info.timeout < 0:  # timeout < 0 means no timeout             # <<<<<<<<<<<<<<
  *         return 0
  * 
  */
     }
 
-    /* "av/container/core.pyx":38
+    /* "av/container/core.pyx":39
  * 
  *     cdef double current_time
  *     with gil:             # <<<<<<<<<<<<<<
  * 
  *         current_time = clock()
  */
     {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         /*try:*/ {
 
-          /* "av/container/core.pyx":40
+          /* "av/container/core.pyx":41
  *     with gil:
  * 
  *         current_time = clock()             # <<<<<<<<<<<<<<
  * 
  *         # Check if the clock has been changed.
  */
           __Pyx_INCREF(__pyx_v_2av_9container_4core_clock);
@@ -2716,41 +2776,41 @@
               __Pyx_INCREF(__pyx_t_4);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_3, function);
             }
           }
           __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L8_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 41, __pyx_L8_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-          __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L8_error)
+          __pyx_t_5 = __pyx_PyFloat_AsDouble(__pyx_t_2); if (unlikely((__pyx_t_5 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 41, __pyx_L8_error)
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_v_current_time = __pyx_t_5;
 
-          /* "av/container/core.pyx":43
+          /* "av/container/core.pyx":44
  * 
  *         # Check if the clock has been changed.
  *         if current_time < info.start_time:             # <<<<<<<<<<<<<<
  *             # Raise this when we get back to Python.
  *             stash_exception((RuntimeError, RuntimeError("Clock has been changed to before timeout start"), None))
  */
           __pyx_t_1 = ((__pyx_v_current_time < __pyx_v_info.start_time) != 0);
           if (__pyx_t_1) {
 
-            /* "av/container/core.pyx":45
+            /* "av/container/core.pyx":46
  *         if current_time < info.start_time:
  *             # Raise this when we get back to Python.
  *             stash_exception((RuntimeError, RuntimeError("Clock has been changed to before timeout start"), None))             # <<<<<<<<<<<<<<
  *             return 1
  * 
  */
-            __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L8_error)
+            __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_2);
-            __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 45, __pyx_L8_error)
+            __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 46, __pyx_L8_error)
             __Pyx_GOTREF(__pyx_t_3);
             __Pyx_INCREF(__pyx_builtin_RuntimeError);
             __Pyx_GIVEREF(__pyx_builtin_RuntimeError);
             PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_builtin_RuntimeError);
             __Pyx_GIVEREF(__pyx_t_2);
             PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
             __Pyx_INCREF(Py_None);
@@ -2758,35 +2818,35 @@
             PyTuple_SET_ITEM(__pyx_t_3, 2, Py_None);
             __pyx_t_2 = 0;
             __pyx_t_6.__pyx_n = 1;
             __pyx_t_6.exc_info = __pyx_t_3;
             __pyx_f_2av_5error_stash_exception(&__pyx_t_6); 
             __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-            /* "av/container/core.pyx":46
+            /* "av/container/core.pyx":47
  *             # Raise this when we get back to Python.
  *             stash_exception((RuntimeError, RuntimeError("Clock has been changed to before timeout start"), None))
  *             return 1             # <<<<<<<<<<<<<<
  * 
  *     if current_time > info.start_time + info.timeout:
  */
             __pyx_r = 1;
             goto __pyx_L7_return;
 
-            /* "av/container/core.pyx":43
+            /* "av/container/core.pyx":44
  * 
  *         # Check if the clock has been changed.
  *         if current_time < info.start_time:             # <<<<<<<<<<<<<<
  *             # Raise this when we get back to Python.
  *             stash_exception((RuntimeError, RuntimeError("Clock has been changed to before timeout start"), None))
  */
           }
         }
 
-        /* "av/container/core.pyx":38
+        /* "av/container/core.pyx":39
  * 
  *     cdef double current_time
  *     with gil:             # <<<<<<<<<<<<<<
  * 
  *         current_time = clock()
  */
         /*finally:*/ {
@@ -2808,55 +2868,55 @@
             #endif
             goto __pyx_L4_error;
           }
           __pyx_L9:;
         }
     }
 
-    /* "av/container/core.pyx":48
+    /* "av/container/core.pyx":49
  *             return 1
  * 
  *     if current_time > info.start_time + info.timeout:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
     __pyx_t_1 = ((__pyx_v_current_time > (__pyx_v_info.start_time + __pyx_v_info.timeout)) != 0);
     if (__pyx_t_1) {
 
-      /* "av/container/core.pyx":49
+      /* "av/container/core.pyx":50
  * 
  *     if current_time > info.start_time + info.timeout:
  *         return 1             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
       __pyx_r = 1;
       goto __pyx_L3_return;
 
-      /* "av/container/core.pyx":48
+      /* "av/container/core.pyx":49
  *             return 1
  * 
  *     if current_time > info.start_time + info.timeout:             # <<<<<<<<<<<<<<
  *         return 1
  * 
  */
     }
 
-    /* "av/container/core.pyx":51
+    /* "av/container/core.pyx":52
  *         return 1
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_r = 0;
     goto __pyx_L3_return;
   }
 
-  /* "av/container/core.pyx":33
+  /* "av/container/core.pyx":34
  * cdef int interrupt_cb (void *p) nogil:
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)             # <<<<<<<<<<<<<<
  *     if info.timeout < 0:  # timeout < 0 means no timeout
  *         return 0
  */
   /*finally:*/ {
@@ -2870,15 +2930,15 @@
       #ifdef WITH_THREAD
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L1_error;
     }
   }
 
-  /* "av/container/core.pyx":31
+  /* "av/container/core.pyx":32
  * cdef object clock = getattr(time, 'monotonic', time.time)
  * 
  * cdef int interrupt_cb (void *p) nogil:             # <<<<<<<<<<<<<<
  * 
  *     cdef timeout_info info = dereference(<timeout_info*> p)
  */
 
@@ -2894,15 +2954,788 @@
   __pyx_L0:;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":97
+/* "av/container/core.pyx":55
+ * 
+ * 
+ * cdef int pyav_io_open(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                       lib.AVIOContext **pb,
+ *                       const char *url,
+ */
+
+static int __pyx_f_2av_9container_4core_pyav_io_open(struct AVFormatContext *__pyx_v_s, struct AVIOContext **__pyx_v_pb, char const *__pyx_v_url, int __pyx_v_flags, AVDictionary **__pyx_v_options) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+  __Pyx_RefNannySetupContext("pyav_io_open", 1);
+
+  /* "av/container/core.pyx":60
+ *                       int flags,
+ *                       lib.AVDictionary **options) nogil:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         return pyav_io_open_gil(s, pb, url, flags, options)
+ * 
+ */
+  /*try:*/ {
+    {
+        #ifdef WITH_THREAD
+        PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+        #endif
+        /*try:*/ {
+
+          /* "av/container/core.pyx":61
+ *                       lib.AVDictionary **options) nogil:
+ *     with gil:
+ *         return pyav_io_open_gil(s, pb, url, flags, options)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+          __pyx_r = __pyx_f_2av_9container_4core_pyav_io_open_gil(__pyx_v_s, __pyx_v_pb, __pyx_v_url, __pyx_v_flags, __pyx_v_options);
+          goto __pyx_L6_return;
+        }
+
+        /* "av/container/core.pyx":60
+ *                       int flags,
+ *                       lib.AVDictionary **options) nogil:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         return pyav_io_open_gil(s, pb, url, flags, options)
+ * 
+ */
+        /*finally:*/ {
+          __pyx_L6_return: {
+            #ifdef WITH_THREAD
+            __Pyx_PyGILState_Release(__pyx_gilstate_save);
+            #endif
+            goto __pyx_L3_return;
+          }
+        }
+    }
+  }
+  /*finally:*/ {
+    __pyx_L3_return: {
+      #ifdef WITH_THREAD
+      __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      goto __pyx_L0;
+    }
+  }
+
+  /* "av/container/core.pyx":55
+ * 
+ * 
+ * cdef int pyav_io_open(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                       lib.AVIOContext **pb,
+ *                       const char *url,
+ */
+
+  /* function exit code */
+  __pyx_r = 0;
+  __pyx_L0:;
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  return __pyx_r;
+}
+
+/* "av/container/core.pyx":64
+ * 
+ * 
+ * cdef int pyav_io_open_gil(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                           lib.AVIOContext **pb,
+ *                           const char *url,
+ */
+
+static int __pyx_f_2av_9container_4core_pyav_io_open_gil(struct AVFormatContext *__pyx_v_s, struct AVIOContext **__pyx_v_pb, char const *__pyx_v_url, int __pyx_v_flags, AVDictionary **__pyx_v_options) {
+  struct __pyx_obj_2av_9container_4core_Container *__pyx_v_container = 0;
+  PyObject *__pyx_v_file = 0;
+  struct __pyx_obj_2av_9container_4pyio_PyIOFile *__pyx_v_pyio_file = 0;
+  PyObject *__pyx_v_options_dict = NULL;
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  void *__pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_9 = NULL;
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_t_11;
+  PyObject *__pyx_t_12 = NULL;
+  struct AVIOContext *__pyx_t_13;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("pyav_io_open_gil", 0);
+
+  /* "av/container/core.pyx":72
+ *     cdef object file
+ *     cdef PyIOFile pyio_file
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "av/container/core.pyx":73
+ *     cdef PyIOFile pyio_file
+ *     try:
+ *         container = <Container>dereference(s).opaque             # <<<<<<<<<<<<<<
+ * 
+ *         if options is not NULL:
+ */
+      __pyx_t_4 = (*__pyx_v_s).opaque;
+      __pyx_t_5 = ((PyObject *)__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __pyx_v_container = ((struct __pyx_obj_2av_9container_4core_Container *)__pyx_t_5);
+      __pyx_t_5 = 0;
+
+      /* "av/container/core.pyx":75
+ *         container = <Container>dereference(s).opaque
+ * 
+ *         if options is not NULL:             # <<<<<<<<<<<<<<
+ *             options_dict = avdict_to_dict(
+ *                 dereference(<lib.AVDictionary**>options),
+ */
+      __pyx_t_6 = ((__pyx_v_options != NULL) != 0);
+      if (__pyx_t_6) {
+
+        /* "av/container/core.pyx":78
+ *             options_dict = avdict_to_dict(
+ *                 dereference(<lib.AVDictionary**>options),
+ *                 encoding=container.metadata_encoding,             # <<<<<<<<<<<<<<
+ *                 errors=container.metadata_errors
+ *             )
+ */
+        __pyx_t_5 = __pyx_v_container->metadata_encoding;
+        __Pyx_INCREF(__pyx_t_5);
+
+        /* "av/container/core.pyx":79
+ *                 dereference(<lib.AVDictionary**>options),
+ *                 encoding=container.metadata_encoding,
+ *                 errors=container.metadata_errors             # <<<<<<<<<<<<<<
+ *             )
+ *         else:
+ */
+        __pyx_t_7 = __pyx_v_container->metadata_errors;
+        __Pyx_INCREF(__pyx_t_7);
+
+        /* "av/container/core.pyx":76
+ * 
+ *         if options is not NULL:
+ *             options_dict = avdict_to_dict(             # <<<<<<<<<<<<<<
+ *                 dereference(<lib.AVDictionary**>options),
+ *                 encoding=container.metadata_encoding,
+ */
+        __pyx_t_8 = __pyx_f_2av_5utils_avdict_to_dict((*((AVDictionary **)__pyx_v_options)), ((PyObject*)__pyx_t_5), ((PyObject*)__pyx_t_7)); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 76, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __pyx_v_options_dict = ((PyObject*)__pyx_t_8);
+        __pyx_t_8 = 0;
+
+        /* "av/container/core.pyx":75
+ *         container = <Container>dereference(s).opaque
+ * 
+ *         if options is not NULL:             # <<<<<<<<<<<<<<
+ *             options_dict = avdict_to_dict(
+ *                 dereference(<lib.AVDictionary**>options),
+ */
+        goto __pyx_L9;
+      }
+
+      /* "av/container/core.pyx":82
+ *             )
+ *         else:
+ *             options_dict = {}             # <<<<<<<<<<<<<<
+ * 
+ *         file = container.io_open(
+ */
+      /*else*/ {
+        __pyx_t_8 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 82, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __pyx_v_options_dict = ((PyObject*)__pyx_t_8);
+        __pyx_t_8 = 0;
+      }
+      __pyx_L9:;
+
+      /* "av/container/core.pyx":85
+ * 
+ *         file = container.io_open(
+ *             <str>url if url is not NULL else "",             # <<<<<<<<<<<<<<
+ *             flags,
+ *             options_dict
+ */
+      if (((__pyx_v_url != NULL) != 0)) {
+        __pyx_t_5 = __Pyx_PyStr_FromString(__pyx_v_url); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 85, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_5);
+        __Pyx_INCREF(((PyObject*)__pyx_t_5));
+        __pyx_t_7 = __pyx_t_5;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      } else {
+        __Pyx_INCREF(__pyx_kp_s__2);
+        __pyx_t_7 = __pyx_kp_s__2;
+      }
+
+      /* "av/container/core.pyx":86
+ *         file = container.io_open(
+ *             <str>url if url is not NULL else "",
+ *             flags,             # <<<<<<<<<<<<<<
+ *             options_dict
+ *         )
+ */
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 86, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+
+      /* "av/container/core.pyx":87
+ *             <str>url if url is not NULL else "",
+ *             flags,
+ *             options_dict             # <<<<<<<<<<<<<<
+ *         )
+ * 
+ */
+      __Pyx_INCREF(__pyx_v_container->io_open);
+      __pyx_t_9 = __pyx_v_container->io_open; __pyx_t_10 = NULL;
+      __pyx_t_11 = 0;
+      if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_9))) {
+        __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
+        if (likely(__pyx_t_10)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_9);
+          __Pyx_INCREF(__pyx_t_10);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_9, function);
+          __pyx_t_11 = 1;
+        }
+      }
+      #if CYTHON_FAST_PYCALL
+      if (PyFunction_Check(__pyx_t_9)) {
+        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_t_7, __pyx_t_5, __pyx_v_options_dict};
+        __pyx_t_8 = __Pyx_PyFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L3_error)
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      } else
+      #endif
+      #if CYTHON_FAST_PYCCALL
+      if (__Pyx_PyFastCFunction_Check(__pyx_t_9)) {
+        PyObject *__pyx_temp[4] = {__pyx_t_10, __pyx_t_7, __pyx_t_5, __pyx_v_options_dict};
+        __pyx_t_8 = __Pyx_PyCFunction_FastCall(__pyx_t_9, __pyx_temp+1-__pyx_t_11, 3+__pyx_t_11); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L3_error)
+        __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      } else
+      #endif
+      {
+        __pyx_t_12 = PyTuple_New(3+__pyx_t_11); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 84, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_12);
+        if (__pyx_t_10) {
+          __Pyx_GIVEREF(__pyx_t_10); PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_t_10); __pyx_t_10 = NULL;
+        }
+        __Pyx_GIVEREF(__pyx_t_7);
+        PyTuple_SET_ITEM(__pyx_t_12, 0+__pyx_t_11, __pyx_t_7);
+        __Pyx_GIVEREF(__pyx_t_5);
+        PyTuple_SET_ITEM(__pyx_t_12, 1+__pyx_t_11, __pyx_t_5);
+        __Pyx_INCREF(__pyx_v_options_dict);
+        __Pyx_GIVEREF(__pyx_v_options_dict);
+        PyTuple_SET_ITEM(__pyx_t_12, 2+__pyx_t_11, __pyx_v_options_dict);
+        __pyx_t_7 = 0;
+        __pyx_t_5 = 0;
+        __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_9, __pyx_t_12, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 84, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_8);
+        __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      }
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __pyx_v_file = __pyx_t_8;
+      __pyx_t_8 = 0;
+
+      /* "av/container/core.pyx":92
+ *         pyio_file = PyIOFile(
+ *             file,
+ *             container.buffer_size,             # <<<<<<<<<<<<<<
+ *             (flags & lib.AVIO_FLAG_WRITE) != 0
+ *         )
+ */
+      __pyx_t_8 = __Pyx_PyInt_From_int(__pyx_v_container->buffer_size); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 92, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_8);
+
+      /* "av/container/core.pyx":93
+ *             file,
+ *             container.buffer_size,
+ *             (flags & lib.AVIO_FLAG_WRITE) != 0             # <<<<<<<<<<<<<<
+ *         )
+ * 
+ */
+      __pyx_t_9 = __Pyx_PyBool_FromLong(((__pyx_v_flags & AVIO_FLAG_WRITE) != 0)); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 93, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_9);
+
+      /* "av/container/core.pyx":90
+ *         )
+ * 
+ *         pyio_file = PyIOFile(             # <<<<<<<<<<<<<<
+ *             file,
+ *             container.buffer_size,
+ */
+      __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 90, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_12);
+      __Pyx_INCREF(__pyx_v_file);
+      __Pyx_GIVEREF(__pyx_v_file);
+      PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_v_file);
+      __Pyx_GIVEREF(__pyx_t_8);
+      PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_8);
+      __Pyx_GIVEREF(__pyx_t_9);
+      PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_t_9);
+      __pyx_t_8 = 0;
+      __pyx_t_9 = 0;
+      __pyx_t_9 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_4pyio_PyIOFile), __pyx_t_12, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 90, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      __pyx_v_pyio_file = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_9);
+      __pyx_t_9 = 0;
+
+      /* "av/container/core.pyx":97
+ * 
+ *         # Add it to the container to avoid it being deallocated
+ *         container.open_files[<int64_t>pyio_file.iocontext.opaque] = pyio_file             # <<<<<<<<<<<<<<
+ * 
+ *         pb[0] = pyio_file.iocontext
+ */
+      if (unlikely(__Pyx_SetItemInt(__pyx_v_container->open_files, ((int64_t)__pyx_v_pyio_file->iocontext->opaque), ((PyObject *)__pyx_v_pyio_file), int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 1, 1) < 0)) __PYX_ERR(0, 97, __pyx_L3_error)
+
+      /* "av/container/core.pyx":99
+ *         container.open_files[<int64_t>pyio_file.iocontext.opaque] = pyio_file
+ * 
+ *         pb[0] = pyio_file.iocontext             # <<<<<<<<<<<<<<
+ *         return 0
+ * 
+ */
+      __pyx_t_13 = __pyx_v_pyio_file->iocontext;
+      (__pyx_v_pb[0]) = __pyx_t_13;
+
+      /* "av/container/core.pyx":100
+ * 
+ *         pb[0] = pyio_file.iocontext
+ *         return 0             # <<<<<<<<<<<<<<
+ * 
+ *     except Exception as e:
+ */
+      __pyx_r = 0;
+      goto __pyx_L7_try_return;
+
+      /* "av/container/core.pyx":72
+ *     cdef object file
+ *     cdef PyIOFile pyio_file
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+    }
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+    __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+
+    /* "av/container/core.pyx":102
+ *         return 0
+ * 
+ *     except Exception as e:             # <<<<<<<<<<<<<<
+ *         return stash_exception()
+ * 
+ */
+    __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_11) {
+      __Pyx_AddTraceback("av.container.core.pyav_io_open_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_12, &__pyx_t_8) < 0) __PYX_ERR(0, 102, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_9);
+      __Pyx_GOTREF(__pyx_t_12);
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_12);
+      __pyx_v_e = __pyx_t_12;
+
+      /* "av/container/core.pyx":103
+ * 
+ *     except Exception as e:
+ *         return stash_exception()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      __pyx_r = __pyx_f_2av_5error_stash_exception(NULL);
+      __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+      __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
+      __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
+      goto __pyx_L6_except_return;
+    }
+    goto __pyx_L5_except_error;
+    __pyx_L5_except_error:;
+
+    /* "av/container/core.pyx":72
+ *     cdef object file
+ *     cdef PyIOFile pyio_file
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L7_try_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+    __pyx_L6_except_return:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L0;
+  }
+
+  /* "av/container/core.pyx":64
+ * 
+ * 
+ * cdef int pyav_io_open_gil(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                           lib.AVIOContext **pb,
+ *                           const char *url,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_12);
+  __Pyx_WriteUnraisable("av.container.core.pyav_io_open_gil", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_container);
+  __Pyx_XDECREF(__pyx_v_file);
+  __Pyx_XDECREF((PyObject *)__pyx_v_pyio_file);
+  __Pyx_XDECREF(__pyx_v_options_dict);
+  __Pyx_XDECREF(__pyx_v_e);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "av/container/core.pyx":106
+ * 
+ * 
+ * cdef void pyav_io_close(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                         lib.AVIOContext *pb) nogil:
+ *     with gil:
+ */
+
+static void __pyx_f_2av_9container_4core_pyav_io_close(struct AVFormatContext *__pyx_v_s, struct AVIOContext *__pyx_v_pb) {
+  __Pyx_RefNannyDeclarations
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+  __Pyx_RefNannySetupContext("pyav_io_close", 1);
+
+  /* "av/container/core.pyx":108
+ * cdef void pyav_io_close(lib.AVFormatContext *s,
+ *                         lib.AVIOContext *pb) nogil:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         pyav_io_close_gil(s, pb)
+ * 
+ */
+  /*try:*/ {
+    {
+        #ifdef WITH_THREAD
+        PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+        #endif
+        /*try:*/ {
+
+          /* "av/container/core.pyx":109
+ *                         lib.AVIOContext *pb) nogil:
+ *     with gil:
+ *         pyav_io_close_gil(s, pb)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+          __pyx_f_2av_9container_4core_pyav_io_close_gil(__pyx_v_s, __pyx_v_pb);
+        }
+
+        /* "av/container/core.pyx":108
+ * cdef void pyav_io_close(lib.AVFormatContext *s,
+ *                         lib.AVIOContext *pb) nogil:
+ *     with gil:             # <<<<<<<<<<<<<<
+ *         pyav_io_close_gil(s, pb)
+ * 
+ */
+        /*finally:*/ {
+          /*normal exit:*/{
+            #ifdef WITH_THREAD
+            __Pyx_PyGILState_Release(__pyx_gilstate_save);
+            #endif
+            goto __pyx_L8;
+          }
+          __pyx_L8:;
+        }
+    }
+  }
+  /*finally:*/ {
+    /*normal exit:*/{
+      #ifdef WITH_THREAD
+      __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+      #endif
+      goto __pyx_L5;
+    }
+    __pyx_L5:;
+  }
+
+  /* "av/container/core.pyx":106
+ * 
+ * 
+ * cdef void pyav_io_close(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                         lib.AVIOContext *pb) nogil:
+ *     with gil:
+ */
+
+  /* function exit code */
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+}
+
+/* "av/container/core.pyx":112
+ * 
+ * 
+ * cdef void pyav_io_close_gil(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                             lib.AVIOContext *pb):
+ *     cdef Container container
+ */
+
+static void __pyx_f_2av_9container_4core_pyav_io_close_gil(struct AVFormatContext *__pyx_v_s, struct AVIOContext *__pyx_v_pb) {
+  struct __pyx_obj_2av_9container_4core_Container *__pyx_v_container = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  void *__pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_t_9;
+  PyObject *__pyx_t_10 = NULL;
+  PyObject *__pyx_t_11 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("pyav_io_close_gil", 0);
+
+  /* "av/container/core.pyx":115
+ *                             lib.AVIOContext *pb):
+ *     cdef Container container
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "av/container/core.pyx":116
+ *     cdef Container container
+ *     try:
+ *         container = <Container>dereference(s).opaque             # <<<<<<<<<<<<<<
+ * 
+ *         if container.open_files is not None and <int64_t>pb.opaque in container.open_files:
+ */
+      __pyx_t_4 = (*__pyx_v_s).opaque;
+      __pyx_t_5 = ((PyObject *)__pyx_t_4);
+      __Pyx_INCREF(__pyx_t_5);
+      __pyx_v_container = ((struct __pyx_obj_2av_9container_4core_Container *)__pyx_t_5);
+      __pyx_t_5 = 0;
+
+      /* "av/container/core.pyx":118
+ *         container = <Container>dereference(s).opaque
+ * 
+ *         if container.open_files is not None and <int64_t>pb.opaque in container.open_files:             # <<<<<<<<<<<<<<
+ *             pyio_close_custom_gil(pb)
+ * 
+ */
+      __pyx_t_7 = (__pyx_v_container->open_files != Py_None);
+      __pyx_t_8 = (__pyx_t_7 != 0);
+      if (__pyx_t_8) {
+      } else {
+        __pyx_t_6 = __pyx_t_8;
+        goto __pyx_L10_bool_binop_done;
+      }
+      __pyx_t_5 = __Pyx_PyInt_From_int64_t(((int64_t)__pyx_v_pb->opaque)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 118, __pyx_L3_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __pyx_t_8 = (__Pyx_PySequence_ContainsTF(__pyx_t_5, __pyx_v_container->open_files, Py_EQ)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 118, __pyx_L3_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_7 = (__pyx_t_8 != 0);
+      __pyx_t_6 = __pyx_t_7;
+      __pyx_L10_bool_binop_done:;
+      if (__pyx_t_6) {
+
+        /* "av/container/core.pyx":119
+ * 
+ *         if container.open_files is not None and <int64_t>pb.opaque in container.open_files:
+ *             pyio_close_custom_gil(pb)             # <<<<<<<<<<<<<<
+ * 
+ *             # Remove it from the container so that it can be deallocated
+ */
+        __pyx_f_2av_9container_4pyio_pyio_close_custom_gil(__pyx_v_pb);
+
+        /* "av/container/core.pyx":122
+ * 
+ *             # Remove it from the container so that it can be deallocated
+ *             del container.open_files[<int64_t>pb.opaque]             # <<<<<<<<<<<<<<
+ *         else:
+ *             pyio_close_gil(pb)
+ */
+        if (unlikely(__Pyx_DelItemInt(__pyx_v_container->open_files, ((int64_t)__pyx_v_pb->opaque), int64_t, 1, __Pyx_PyInt_From_int64_t, 0, 1, 1) < 0)) __PYX_ERR(0, 122, __pyx_L3_error)
+
+        /* "av/container/core.pyx":118
+ *         container = <Container>dereference(s).opaque
+ * 
+ *         if container.open_files is not None and <int64_t>pb.opaque in container.open_files:             # <<<<<<<<<<<<<<
+ *             pyio_close_custom_gil(pb)
+ * 
+ */
+        goto __pyx_L9;
+      }
+
+      /* "av/container/core.pyx":124
+ *             del container.open_files[<int64_t>pb.opaque]
+ *         else:
+ *             pyio_close_gil(pb)             # <<<<<<<<<<<<<<
+ * 
+ *     except Exception as e:
+ */
+      /*else*/ {
+        __pyx_f_2av_9container_4pyio_pyio_close_gil(__pyx_v_pb);
+      }
+      __pyx_L9:;
+
+      /* "av/container/core.pyx":115
+ *                             lib.AVIOContext *pb):
+ *     cdef Container container
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+
+    /* "av/container/core.pyx":126
+ *             pyio_close_gil(pb)
+ * 
+ *     except Exception as e:             # <<<<<<<<<<<<<<
+ *         stash_exception()
+ * 
+ */
+    __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_9) {
+      __Pyx_AddTraceback("av.container.core.pyav_io_close_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_10, &__pyx_t_11) < 0) __PYX_ERR(0, 126, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_GOTREF(__pyx_t_10);
+      __Pyx_GOTREF(__pyx_t_11);
+      __Pyx_INCREF(__pyx_t_10);
+      __pyx_v_e = __pyx_t_10;
+
+      /* "av/container/core.pyx":127
+ * 
+ *     except Exception as e:
+ *         stash_exception()             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+      (void)(__pyx_f_2av_5error_stash_exception(NULL));
+      __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
+      __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
+      goto __pyx_L4_exception_handled;
+    }
+    goto __pyx_L5_except_error;
+    __pyx_L5_except_error:;
+
+    /* "av/container/core.pyx":115
+ *                             lib.AVIOContext *pb):
+ *     cdef Container container
+ *     try:             # <<<<<<<<<<<<<<
+ *         container = <Container>dereference(s).opaque
+ * 
+ */
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L4_exception_handled:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    __pyx_L8_try_end:;
+  }
+
+  /* "av/container/core.pyx":112
+ * 
+ * 
+ * cdef void pyav_io_close_gil(lib.AVFormatContext *s,             # <<<<<<<<<<<<<<
+ *                             lib.AVIOContext *pb):
+ *     cdef Container container
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_10);
+  __Pyx_XDECREF(__pyx_t_11);
+  __Pyx_WriteUnraisable("av.container.core.pyav_io_close_gil", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_container);
+  __Pyx_XDECREF(__pyx_v_e);
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "av/container/core.pyx":173
  * cdef class Container(object):
  * 
  *     def __cinit__(self, sentinel, file_, format_name, options,             # <<<<<<<<<<<<<<
  *                   container_options, stream_options,
  *                   metadata_encoding, metadata_errors,
  */
 
@@ -2916,27 +3749,30 @@
   PyObject *__pyx_v_container_options = 0;
   PyObject *__pyx_v_stream_options = 0;
   PyObject *__pyx_v_metadata_encoding = 0;
   PyObject *__pyx_v_metadata_errors = 0;
   PyObject *__pyx_v_buffer_size = 0;
   PyObject *__pyx_v_open_timeout = 0;
   PyObject *__pyx_v_read_timeout = 0;
+  PyObject *__pyx_v_io_open = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_sentinel,&__pyx_n_s_file,&__pyx_n_s_format_name,&__pyx_n_s_options,&__pyx_n_s_container_options,&__pyx_n_s_stream_options,&__pyx_n_s_metadata_encoding,&__pyx_n_s_metadata_errors,&__pyx_n_s_buffer_size,&__pyx_n_s_open_timeout,&__pyx_n_s_read_timeout,0};
-    PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_sentinel,&__pyx_n_s_file,&__pyx_n_s_format_name,&__pyx_n_s_options,&__pyx_n_s_container_options,&__pyx_n_s_stream_options,&__pyx_n_s_metadata_encoding,&__pyx_n_s_metadata_errors,&__pyx_n_s_buffer_size,&__pyx_n_s_open_timeout,&__pyx_n_s_read_timeout,&__pyx_n_s_io_open,0};
+    PyObject* values[12] = {0,0,0,0,0,0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case 12: values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
+        CYTHON_FALLTHROUGH;
         case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
         CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
@@ -2963,117 +3799,125 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sentinel)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_file)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 1); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 1); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format_name)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 2); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 2); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 3); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 3); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container_options)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 4); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 4); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_stream_options)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 5); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 5); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  6:
         if (likely((values[6] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_metadata_encoding)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 6); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 6); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  7:
         if (likely((values[7] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_metadata_errors)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 7); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 7); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  8:
         if (likely((values[8] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_buffer_size)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 8); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 8); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (likely((values[9] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_open_timeout)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 9); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 9); __PYX_ERR(0, 173, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case 10:
         if (likely((values[10] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_read_timeout)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, 10); __PYX_ERR(0, 97, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 10); __PYX_ERR(0, 173, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case 11:
+        if (likely((values[11] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_io_open)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, 11); __PYX_ERR(0, 173, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 97, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 173, __pyx_L3_error)
       }
-    } else if (PyTuple_GET_SIZE(__pyx_args) != 11) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 12) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
       values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
       values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
       values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
       values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
       values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
       values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
       values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+      values[11] = PyTuple_GET_ITEM(__pyx_args, 11);
     }
     __pyx_v_sentinel = values[0];
     __pyx_v_file_ = values[1];
     __pyx_v_format_name = values[2];
     __pyx_v_options = values[3];
     __pyx_v_container_options = values[4];
     __pyx_v_stream_options = values[5];
     __pyx_v_metadata_encoding = values[6];
     __pyx_v_metadata_errors = values[7];
     __pyx_v_buffer_size = values[8];
     __pyx_v_open_timeout = values[9];
     __pyx_v_read_timeout = values[10];
+    __pyx_v_io_open = values[11];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 11, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 97, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 1, 12, 12, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 173, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.container.core.Container.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2av_9container_4core_9Container___cinit__(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_sentinel, __pyx_v_file_, __pyx_v_format_name, __pyx_v_options, __pyx_v_container_options, __pyx_v_stream_options, __pyx_v_metadata_encoding, __pyx_v_metadata_errors, __pyx_v_buffer_size, __pyx_v_open_timeout, __pyx_v_read_timeout);
+  __pyx_r = __pyx_pf_2av_9container_4core_9Container___cinit__(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_sentinel, __pyx_v_file_, __pyx_v_format_name, __pyx_v_options, __pyx_v_container_options, __pyx_v_stream_options, __pyx_v_metadata_encoding, __pyx_v_metadata_errors, __pyx_v_buffer_size, __pyx_v_open_timeout, __pyx_v_read_timeout, __pyx_v_io_open);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_2av_9container_4core_9Container___cinit__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, PyObject *__pyx_v_sentinel, PyObject *__pyx_v_file_, PyObject *__pyx_v_format_name, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_open_timeout, PyObject *__pyx_v_read_timeout) {
+static int __pyx_pf_2av_9container_4core_9Container___cinit__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self, PyObject *__pyx_v_sentinel, PyObject *__pyx_v_file_, PyObject *__pyx_v_format_name, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_open_timeout, PyObject *__pyx_v_read_timeout, PyObject *__pyx_v_io_open) {
   int __pyx_v_res;
   PyObject *__pyx_v_name_obj = 0;
   char *__pyx_v_name;
   CYTHON_UNUSED __pyx_t_2av_9container_4core_seek_func_t __pyx_v_seek_func;
   struct AVOutputFormat *__pyx_v_ofmt;
   struct AVInputFormat *__pyx_v_ifmt;
   struct __pyx_obj_2av_10dictionary__Dictionary *__pyx_v_c_options = 0;
@@ -3084,69 +3928,69 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   Py_ssize_t __pyx_t_7;
   PyObject *(*__pyx_t_8)(PyObject *);
-  char *__pyx_t_9;
-  struct AVOutputFormat *__pyx_t_10;
-  int __pyx_t_11;
+  int __pyx_t_9;
+  char *__pyx_t_10;
+  struct AVOutputFormat *__pyx_t_11;
   struct AVIOContext *__pyx_t_12;
   struct AVInputFormat *__pyx_t_13;
   PyObject *__pyx_t_14 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "av/container/core.pyx":102
- *                   buffer_size, open_timeout, read_timeout):
+  /* "av/container/core.pyx":179
+ *                   io_open):
  * 
  *         if sentinel is not _cinit_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot construct base Container')
  * 
  */
   __pyx_t_1 = (__pyx_v_sentinel != __pyx_v_2av_9container_4core__cinit_sentinel);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/container/core.pyx":103
+    /* "av/container/core.pyx":180
  * 
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('cannot construct base Container')             # <<<<<<<<<<<<<<
  * 
  *         self.writeable = isinstance(self, OutputContainer)
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 103, __pyx_L1_error)
+    __PYX_ERR(0, 180, __pyx_L1_error)
 
-    /* "av/container/core.pyx":102
- *                   buffer_size, open_timeout, read_timeout):
+    /* "av/container/core.pyx":179
+ *                   io_open):
  * 
  *         if sentinel is not _cinit_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot construct base Container')
  * 
  */
   }
 
-  /* "av/container/core.pyx":105
+  /* "av/container/core.pyx":182
  *             raise RuntimeError('cannot construct base Container')
  * 
  *         self.writeable = isinstance(self, OutputContainer)             # <<<<<<<<<<<<<<
  *         if not self.writeable and not isinstance(self, InputContainer):
  *             raise RuntimeError('Container cannot be directly extended.')
  */
   __pyx_t_2 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_2av_9container_6output_OutputContainer); 
   __pyx_v_self->writeable = __pyx_t_2;
 
-  /* "av/container/core.pyx":106
+  /* "av/container/core.pyx":183
  * 
  *         self.writeable = isinstance(self, OutputContainer)
  *         if not self.writeable and not isinstance(self, InputContainer):             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Container cannot be directly extended.')
  * 
  */
   __pyx_t_1 = ((!(__pyx_v_self->writeable != 0)) != 0);
@@ -3157,455 +4001,478 @@
   }
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_2av_9container_5input_InputContainer); 
   __pyx_t_4 = ((!(__pyx_t_1 != 0)) != 0);
   __pyx_t_2 = __pyx_t_4;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/container/core.pyx":107
+    /* "av/container/core.pyx":184
  *         self.writeable = isinstance(self, OutputContainer)
  *         if not self.writeable and not isinstance(self, InputContainer):
  *             raise RuntimeError('Container cannot be directly extended.')             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(file_, str):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 107, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 107, __pyx_L1_error)
+    __PYX_ERR(0, 184, __pyx_L1_error)
 
-    /* "av/container/core.pyx":106
+    /* "av/container/core.pyx":183
  * 
  *         self.writeable = isinstance(self, OutputContainer)
  *         if not self.writeable and not isinstance(self, InputContainer):             # <<<<<<<<<<<<<<
  *             raise RuntimeError('Container cannot be directly extended.')
  * 
  */
   }
 
-  /* "av/container/core.pyx":109
+  /* "av/container/core.pyx":186
  *             raise RuntimeError('Container cannot be directly extended.')
  * 
  *         if isinstance(file_, str):             # <<<<<<<<<<<<<<
  *             self.name = file_
  *         else:
  */
   __pyx_t_2 = PyString_Check(__pyx_v_file_); 
   __pyx_t_4 = (__pyx_t_2 != 0);
   if (__pyx_t_4) {
 
-    /* "av/container/core.pyx":110
+    /* "av/container/core.pyx":187
  * 
  *         if isinstance(file_, str):
  *             self.name = file_             # <<<<<<<<<<<<<<
  *         else:
  *             self.name = str(getattr(file_, 'name', '<none>'))
  */
     __Pyx_INCREF(__pyx_v_file_);
     __Pyx_GIVEREF(__pyx_v_file_);
     __Pyx_GOTREF(__pyx_v_self->name);
     __Pyx_DECREF(__pyx_v_self->name);
     __pyx_v_self->name = __pyx_v_file_;
 
-    /* "av/container/core.pyx":109
+    /* "av/container/core.pyx":186
  *             raise RuntimeError('Container cannot be directly extended.')
  * 
  *         if isinstance(file_, str):             # <<<<<<<<<<<<<<
  *             self.name = file_
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "av/container/core.pyx":112
+  /* "av/container/core.pyx":189
  *             self.name = file_
  *         else:
  *             self.name = str(getattr(file_, 'name', '<none>'))             # <<<<<<<<<<<<<<
  * 
  *         self.options = dict(options or ())
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_file_, __pyx_n_s_name, __pyx_kp_s_none); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_file_, __pyx_n_s_name, __pyx_kp_s_none); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyString_Type)), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_v_self->name);
     __Pyx_DECREF(__pyx_v_self->name);
     __pyx_v_self->name = __pyx_t_5;
     __pyx_t_5 = 0;
   }
   __pyx_L7:;
 
-  /* "av/container/core.pyx":114
+  /* "av/container/core.pyx":191
  *             self.name = str(getattr(file_, 'name', '<none>'))
  * 
  *         self.options = dict(options or ())             # <<<<<<<<<<<<<<
  *         self.container_options = dict(container_options or ())
  *         self.stream_options = [dict(x) for x in stream_options or ()]
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_options);
     __pyx_t_5 = __pyx_v_options;
     goto __pyx_L8_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_empty_tuple);
   __pyx_t_5 = __pyx_empty_tuple;
   __pyx_L8_bool_binop_done:;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 114, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->options);
   __Pyx_DECREF(__pyx_v_self->options);
   __pyx_v_self->options = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":115
+  /* "av/container/core.pyx":192
  * 
  *         self.options = dict(options or ())
  *         self.container_options = dict(container_options or ())             # <<<<<<<<<<<<<<
  *         self.stream_options = [dict(x) for x in stream_options or ()]
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_container_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_container_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_container_options);
     __pyx_t_3 = __pyx_v_container_options;
     goto __pyx_L10_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_empty_tuple);
   __pyx_t_3 = __pyx_empty_tuple;
   __pyx_L10_bool_binop_done:;
-  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->container_options);
   __Pyx_DECREF(__pyx_v_self->container_options);
   __pyx_v_self->container_options = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "av/container/core.pyx":116
+  /* "av/container/core.pyx":193
  *         self.options = dict(options or ())
  *         self.container_options = dict(container_options or ())
  *         self.stream_options = [dict(x) for x in stream_options or ()]             # <<<<<<<<<<<<<<
  * 
  *         self.metadata_encoding = metadata_encoding
  */
-  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 193, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_stream_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_stream_options); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
   if (!__pyx_t_4) {
   } else {
     __Pyx_INCREF(__pyx_v_stream_options);
     __pyx_t_3 = __pyx_v_stream_options;
     goto __pyx_L14_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_empty_tuple);
   __pyx_t_3 = __pyx_empty_tuple;
   __pyx_L14_bool_binop_done:;
   if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
     __pyx_t_6 = __pyx_t_3; __Pyx_INCREF(__pyx_t_6); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_6)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 193, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_6))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_6)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_7); __Pyx_INCREF(__pyx_t_3); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_6, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_8(__pyx_t_6);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 116, __pyx_L1_error)
+          else __PYX_ERR(0, 193, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_x, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_x); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 116, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 193, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->stream_options);
   __Pyx_DECREF(__pyx_v_self->stream_options);
   __pyx_v_self->stream_options = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "av/container/core.pyx":118
+  /* "av/container/core.pyx":195
  *         self.stream_options = [dict(x) for x in stream_options or ()]
  * 
  *         self.metadata_encoding = metadata_encoding             # <<<<<<<<<<<<<<
  *         self.metadata_errors = metadata_errors
  * 
  */
-  if (!(likely(PyString_CheckExact(__pyx_v_metadata_encoding))||((__pyx_v_metadata_encoding) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_v_metadata_encoding)->tp_name), 0))) __PYX_ERR(0, 118, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_v_metadata_encoding))||((__pyx_v_metadata_encoding) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_v_metadata_encoding)->tp_name), 0))) __PYX_ERR(0, 195, __pyx_L1_error)
   __pyx_t_5 = __pyx_v_metadata_encoding;
   __Pyx_INCREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->metadata_encoding);
   __Pyx_DECREF(__pyx_v_self->metadata_encoding);
   __pyx_v_self->metadata_encoding = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "av/container/core.pyx":119
+  /* "av/container/core.pyx":196
  * 
  *         self.metadata_encoding = metadata_encoding
  *         self.metadata_errors = metadata_errors             # <<<<<<<<<<<<<<
  * 
  *         self.open_timeout = open_timeout
  */
-  if (!(likely(PyString_CheckExact(__pyx_v_metadata_errors))||((__pyx_v_metadata_errors) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_v_metadata_errors)->tp_name), 0))) __PYX_ERR(0, 119, __pyx_L1_error)
+  if (!(likely(PyString_CheckExact(__pyx_v_metadata_errors))||((__pyx_v_metadata_errors) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "str", Py_TYPE(__pyx_v_metadata_errors)->tp_name), 0))) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_t_5 = __pyx_v_metadata_errors;
   __Pyx_INCREF(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   __Pyx_GOTREF(__pyx_v_self->metadata_errors);
   __Pyx_DECREF(__pyx_v_self->metadata_errors);
   __pyx_v_self->metadata_errors = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "av/container/core.pyx":121
+  /* "av/container/core.pyx":198
  *         self.metadata_errors = metadata_errors
  * 
  *         self.open_timeout = open_timeout             # <<<<<<<<<<<<<<
  *         self.read_timeout = read_timeout
  * 
  */
   __Pyx_INCREF(__pyx_v_open_timeout);
   __Pyx_GIVEREF(__pyx_v_open_timeout);
   __Pyx_GOTREF(__pyx_v_self->open_timeout);
   __Pyx_DECREF(__pyx_v_self->open_timeout);
   __pyx_v_self->open_timeout = __pyx_v_open_timeout;
 
-  /* "av/container/core.pyx":122
+  /* "av/container/core.pyx":199
  * 
  *         self.open_timeout = open_timeout
  *         self.read_timeout = read_timeout             # <<<<<<<<<<<<<<
  * 
- *         if format_name is not None:
+ *         self.buffer_size = buffer_size
  */
   __Pyx_INCREF(__pyx_v_read_timeout);
   __Pyx_GIVEREF(__pyx_v_read_timeout);
   __Pyx_GOTREF(__pyx_v_self->read_timeout);
   __Pyx_DECREF(__pyx_v_self->read_timeout);
   __pyx_v_self->read_timeout = __pyx_v_read_timeout;
 
-  /* "av/container/core.pyx":124
+  /* "av/container/core.pyx":201
  *         self.read_timeout = read_timeout
  * 
+ *         self.buffer_size = buffer_size             # <<<<<<<<<<<<<<
+ *         self.io_open = io_open
+ * 
+ */
+  __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_buffer_size); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L1_error)
+  __pyx_v_self->buffer_size = __pyx_t_9;
+
+  /* "av/container/core.pyx":202
+ * 
+ *         self.buffer_size = buffer_size
+ *         self.io_open = io_open             # <<<<<<<<<<<<<<
+ * 
+ *         if format_name is not None:
+ */
+  __Pyx_INCREF(__pyx_v_io_open);
+  __Pyx_GIVEREF(__pyx_v_io_open);
+  __Pyx_GOTREF(__pyx_v_self->io_open);
+  __Pyx_DECREF(__pyx_v_self->io_open);
+  __pyx_v_self->io_open = __pyx_v_io_open;
+
+  /* "av/container/core.pyx":204
+ *         self.io_open = io_open
+ * 
  *         if format_name is not None:             # <<<<<<<<<<<<<<
  *             self.format = ContainerFormat(format_name)
  * 
  */
   __pyx_t_4 = (__pyx_v_format_name != Py_None);
   __pyx_t_2 = (__pyx_t_4 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":125
+    /* "av/container/core.pyx":205
  * 
  *         if format_name is not None:
  *             self.format = ContainerFormat(format_name)             # <<<<<<<<<<<<<<
  * 
  *         self.input_was_opened = False
  */
-    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_6format_ContainerFormat), __pyx_v_format_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2av_6format_ContainerFormat), __pyx_v_format_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 205, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_v_self->format);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->format));
     __pyx_v_self->format = ((struct __pyx_obj_2av_6format_ContainerFormat *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "av/container/core.pyx":124
- *         self.read_timeout = read_timeout
+    /* "av/container/core.pyx":204
+ *         self.io_open = io_open
  * 
  *         if format_name is not None:             # <<<<<<<<<<<<<<
  *             self.format = ContainerFormat(format_name)
  * 
  */
   }
 
-  /* "av/container/core.pyx":127
+  /* "av/container/core.pyx":207
  *             self.format = ContainerFormat(format_name)
  * 
  *         self.input_was_opened = False             # <<<<<<<<<<<<<<
  *         cdef int res
  * 
  */
   __pyx_v_self->input_was_opened = 0;
 
-  /* "av/container/core.pyx":130
+  /* "av/container/core.pyx":210
  *         cdef int res
  * 
  *         cdef bytes name_obj = os.fsencode(self.name)             # <<<<<<<<<<<<<<
  *         cdef char *name = name_obj
  *         cdef seek_func_t seek_func = NULL
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_os); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_fsencode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 130, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_fsencode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_6 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_6)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_5 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_6, __pyx_v_self->name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_self->name);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 130, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_5))||((__pyx_t_5) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_5)->tp_name), 0))) __PYX_ERR(0, 210, __pyx_L1_error)
   __pyx_v_name_obj = ((PyObject*)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "av/container/core.pyx":131
+  /* "av/container/core.pyx":211
  * 
  *         cdef bytes name_obj = os.fsencode(self.name)
  *         cdef char *name = name_obj             # <<<<<<<<<<<<<<
  *         cdef seek_func_t seek_func = NULL
  * 
  */
   if (unlikely(__pyx_v_name_obj == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 131, __pyx_L1_error)
+    __PYX_ERR(0, 211, __pyx_L1_error)
   }
-  __pyx_t_9 = __Pyx_PyBytes_AsWritableString(__pyx_v_name_obj); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 131, __pyx_L1_error)
-  __pyx_v_name = __pyx_t_9;
+  __pyx_t_10 = __Pyx_PyBytes_AsWritableString(__pyx_v_name_obj); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_v_name = __pyx_t_10;
 
-  /* "av/container/core.pyx":132
+  /* "av/container/core.pyx":212
  *         cdef bytes name_obj = os.fsencode(self.name)
  *         cdef char *name = name_obj
  *         cdef seek_func_t seek_func = NULL             # <<<<<<<<<<<<<<
  * 
  *         cdef lib.AVOutputFormat *ofmt
  */
   __pyx_v_seek_func = NULL;
 
-  /* "av/container/core.pyx":135
+  /* "av/container/core.pyx":215
  * 
  *         cdef lib.AVOutputFormat *ofmt
  *         if self.writeable:             # <<<<<<<<<<<<<<
  * 
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  */
   __pyx_t_2 = (__pyx_v_self->writeable != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":137
+    /* "av/container/core.pyx":217
  *         if self.writeable:
  * 
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)             # <<<<<<<<<<<<<<
  *             if ofmt == NULL:
  *                 raise ValueError("Could not determine output format")
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->format)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->format)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 217, __pyx_L1_error)
     if (__pyx_t_2) {
-      __pyx_t_10 = __pyx_v_self->format->optr;
+      __pyx_t_11 = __pyx_v_self->format->optr;
     } else {
-      __pyx_t_10 = av_guess_format(NULL, __pyx_v_name, NULL);
+      __pyx_t_11 = av_guess_format(NULL, __pyx_v_name, NULL);
     }
-    __pyx_v_ofmt = __pyx_t_10;
+    __pyx_v_ofmt = __pyx_t_11;
 
-    /* "av/container/core.pyx":138
+    /* "av/container/core.pyx":218
  * 
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  *             if ofmt == NULL:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Could not determine output format")
  * 
  */
     __pyx_t_2 = ((__pyx_v_ofmt == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "av/container/core.pyx":139
+      /* "av/container/core.pyx":219
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  *             if ofmt == NULL:
  *                 raise ValueError("Could not determine output format")             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 139, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 139, __pyx_L1_error)
+      __PYX_ERR(0, 219, __pyx_L1_error)
 
-      /* "av/container/core.pyx":138
+      /* "av/container/core.pyx":218
  * 
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  *             if ofmt == NULL:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Could not determine output format")
  * 
  */
     }
 
-    /* "av/container/core.pyx":141
+    /* "av/container/core.pyx":221
  *                 raise ValueError("Could not determine output format")
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 # This does not actually open the file.
  *                 res = lib.avformat_alloc_output_context2(
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "av/container/core.pyx":143
+          /* "av/container/core.pyx":223
  *             with nogil:
  *                 # This does not actually open the file.
  *                 res = lib.avformat_alloc_output_context2(             # <<<<<<<<<<<<<<
  *                     &self.ptr,
  *                     ofmt,
  */
           __pyx_v_res = avformat_alloc_output_context2((&__pyx_v_self->ptr), __pyx_v_ofmt, NULL, __pyx_v_name);
         }
 
-        /* "av/container/core.pyx":141
+        /* "av/container/core.pyx":221
  *                 raise ValueError("Could not determine output format")
  * 
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 # This does not actually open the file.
  *                 res = lib.avformat_alloc_output_context2(
  */
         /*finally:*/ {
@@ -3616,44 +4483,44 @@
             #endif
             goto __pyx_L21;
           }
           __pyx_L21:;
         }
     }
 
-    /* "av/container/core.pyx":149
+    /* "av/container/core.pyx":229
  *                     name,
  *                 )
  *             self.err_check(res)             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->err_check(__pyx_v_self, __pyx_v_res); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 149, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->err_check(__pyx_v_self, __pyx_v_res); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
 
-    /* "av/container/core.pyx":135
+    /* "av/container/core.pyx":215
  * 
  *         cdef lib.AVOutputFormat *ofmt
  *         if self.writeable:             # <<<<<<<<<<<<<<
  * 
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  */
     goto __pyx_L17;
   }
 
-  /* "av/container/core.pyx":153
+  /* "av/container/core.pyx":233
  *         else:
  *             # We need the context before we open the input AND setup Python IO.
  *             self.ptr = lib.avformat_alloc_context()             # <<<<<<<<<<<<<<
  * 
  *             # Setup interrupt callback
  */
   /*else*/ {
     __pyx_v_self->ptr = avformat_alloc_context();
 
-    /* "av/container/core.pyx":156
+    /* "av/container/core.pyx":236
  * 
  *             # Setup interrupt callback
  *             if self.open_timeout is not None or self.read_timeout is not None:             # <<<<<<<<<<<<<<
  *                 self.ptr.interrupt_callback.callback = interrupt_cb
  *                 self.ptr.interrupt_callback.opaque = &self.interrupt_callback_info
  */
     __pyx_t_4 = (__pyx_v_self->open_timeout != Py_None);
@@ -3665,337 +4532,408 @@
     }
     __pyx_t_1 = (__pyx_v_self->read_timeout != Py_None);
     __pyx_t_4 = (__pyx_t_1 != 0);
     __pyx_t_2 = __pyx_t_4;
     __pyx_L23_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "av/container/core.pyx":157
+      /* "av/container/core.pyx":237
  *             # Setup interrupt callback
  *             if self.open_timeout is not None or self.read_timeout is not None:
  *                 self.ptr.interrupt_callback.callback = interrupt_cb             # <<<<<<<<<<<<<<
  *                 self.ptr.interrupt_callback.opaque = &self.interrupt_callback_info
  * 
  */
       __pyx_v_self->ptr->interrupt_callback.callback = __pyx_f_2av_9container_4core_interrupt_cb;
 
-      /* "av/container/core.pyx":158
+      /* "av/container/core.pyx":238
  *             if self.open_timeout is not None or self.read_timeout is not None:
  *                 self.ptr.interrupt_callback.callback = interrupt_cb
  *                 self.ptr.interrupt_callback.opaque = &self.interrupt_callback_info             # <<<<<<<<<<<<<<
  * 
  *         self.ptr.flags |= lib.AVFMT_FLAG_GENPTS
  */
       __pyx_v_self->ptr->interrupt_callback.opaque = (&__pyx_v_self->interrupt_callback_info);
 
-      /* "av/container/core.pyx":156
+      /* "av/container/core.pyx":236
  * 
  *             # Setup interrupt callback
  *             if self.open_timeout is not None or self.read_timeout is not None:             # <<<<<<<<<<<<<<
  *                 self.ptr.interrupt_callback.callback = interrupt_cb
  *                 self.ptr.interrupt_callback.opaque = &self.interrupt_callback_info
  */
     }
   }
   __pyx_L17:;
 
-  /* "av/container/core.pyx":160
+  /* "av/container/core.pyx":240
  *                 self.ptr.interrupt_callback.opaque = &self.interrupt_callback_info
  * 
  *         self.ptr.flags |= lib.AVFMT_FLAG_GENPTS             # <<<<<<<<<<<<<<
+ *         self.ptr.opaque = <void*>self
  * 
- *         # Setup Python IO.
  */
   __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags | AVFMT_FLAG_GENPTS);
 
-  /* "av/container/core.pyx":163
+  /* "av/container/core.pyx":241
+ * 
+ *         self.ptr.flags |= lib.AVFMT_FLAG_GENPTS
+ *         self.ptr.opaque = <void*>self             # <<<<<<<<<<<<<<
  * 
  *         # Setup Python IO.
+ */
+  __pyx_v_self->ptr->opaque = ((void *)__pyx_v_self);
+
+  /* "av/container/core.pyx":244
+ * 
+ *         # Setup Python IO.
+ *         self.open_files = {}             # <<<<<<<<<<<<<<
+ *         if not isinstance(file_, basestring):
+ *             self.file = PyIOFile(file_, buffer_size, self.writeable)
+ */
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_GIVEREF(__pyx_t_5);
+  __Pyx_GOTREF(__pyx_v_self->open_files);
+  __Pyx_DECREF(__pyx_v_self->open_files);
+  __pyx_v_self->open_files = __pyx_t_5;
+  __pyx_t_5 = 0;
+
+  /* "av/container/core.pyx":245
+ *         # Setup Python IO.
+ *         self.open_files = {}
  *         if not isinstance(file_, basestring):             # <<<<<<<<<<<<<<
  *             self.file = PyIOFile(file_, buffer_size, self.writeable)
  *             self.ptr.pb = self.file.iocontext
  */
   __pyx_t_2 = __Pyx_PyBaseString_Check(__pyx_v_file_); 
   __pyx_t_4 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "av/container/core.pyx":164
- *         # Setup Python IO.
+    /* "av/container/core.pyx":246
+ *         self.open_files = {}
  *         if not isinstance(file_, basestring):
  *             self.file = PyIOFile(file_, buffer_size, self.writeable)             # <<<<<<<<<<<<<<
  *             self.ptr.pb = self.file.iocontext
  * 
  */
-    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_self->writeable); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBool_FromLong(__pyx_v_self->writeable); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_file_);
     __Pyx_GIVEREF(__pyx_v_file_);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_file_);
     __Pyx_INCREF(__pyx_v_buffer_size);
     __Pyx_GIVEREF(__pyx_v_buffer_size);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_buffer_size);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_4pyio_PyIOFile), __pyx_t_3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_4pyio_PyIOFile), __pyx_t_3, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 246, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_GIVEREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_v_self->file);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->file));
     __pyx_v_self->file = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "av/container/core.pyx":165
+    /* "av/container/core.pyx":247
  *         if not isinstance(file_, basestring):
  *             self.file = PyIOFile(file_, buffer_size, self.writeable)
  *             self.ptr.pb = self.file.iocontext             # <<<<<<<<<<<<<<
  * 
- *         cdef lib.AVInputFormat *ifmt
+ *         if io_open is not None:
  */
     __pyx_t_12 = __pyx_v_self->file->iocontext;
     __pyx_v_self->ptr->pb = __pyx_t_12;
 
-    /* "av/container/core.pyx":163
- * 
+    /* "av/container/core.pyx":245
  *         # Setup Python IO.
+ *         self.open_files = {}
  *         if not isinstance(file_, basestring):             # <<<<<<<<<<<<<<
  *             self.file = PyIOFile(file_, buffer_size, self.writeable)
  *             self.ptr.pb = self.file.iocontext
  */
   }
 
-  /* "av/container/core.pyx":169
+  /* "av/container/core.pyx":249
+ *             self.ptr.pb = self.file.iocontext
+ * 
+ *         if io_open is not None:             # <<<<<<<<<<<<<<
+ *             self.ptr.io_open = pyav_io_open
+ *             self.ptr.io_close = pyav_io_close
+ */
+  __pyx_t_4 = (__pyx_v_io_open != Py_None);
+  __pyx_t_2 = (__pyx_t_4 != 0);
+  if (__pyx_t_2) {
+
+    /* "av/container/core.pyx":250
+ * 
+ *         if io_open is not None:
+ *             self.ptr.io_open = pyav_io_open             # <<<<<<<<<<<<<<
+ *             self.ptr.io_close = pyav_io_close
+ *             self.ptr.flags |= lib.AVFMT_FLAG_CUSTOM_IO
+ */
+    __pyx_v_self->ptr->io_open = __pyx_f_2av_9container_4core_pyav_io_open;
+
+    /* "av/container/core.pyx":251
+ *         if io_open is not None:
+ *             self.ptr.io_open = pyav_io_open
+ *             self.ptr.io_close = pyav_io_close             # <<<<<<<<<<<<<<
+ *             self.ptr.flags |= lib.AVFMT_FLAG_CUSTOM_IO
+ * 
+ */
+    __pyx_v_self->ptr->io_close = __pyx_f_2av_9container_4core_pyav_io_close;
+
+    /* "av/container/core.pyx":252
+ *             self.ptr.io_open = pyav_io_open
+ *             self.ptr.io_close = pyav_io_close
+ *             self.ptr.flags |= lib.AVFMT_FLAG_CUSTOM_IO             # <<<<<<<<<<<<<<
+ * 
+ *         cdef lib.AVInputFormat *ifmt
+ */
+    __pyx_v_self->ptr->flags = (__pyx_v_self->ptr->flags | AVFMT_FLAG_CUSTOM_IO);
+
+    /* "av/container/core.pyx":249
+ *             self.ptr.pb = self.file.iocontext
+ * 
+ *         if io_open is not None:             # <<<<<<<<<<<<<<
+ *             self.ptr.io_open = pyav_io_open
+ *             self.ptr.io_close = pyav_io_close
+ */
+  }
+
+  /* "av/container/core.pyx":256
  *         cdef lib.AVInputFormat *ifmt
  *         cdef _Dictionary c_options
  *         if not self.writeable:             # <<<<<<<<<<<<<<
  * 
  *             ifmt = self.format.iptr if self.format else NULL
  */
-  __pyx_t_4 = ((!(__pyx_v_self->writeable != 0)) != 0);
-  if (__pyx_t_4) {
+  __pyx_t_2 = ((!(__pyx_v_self->writeable != 0)) != 0);
+  if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":171
+    /* "av/container/core.pyx":258
  *         if not self.writeable:
  * 
  *             ifmt = self.format.iptr if self.format else NULL             # <<<<<<<<<<<<<<
  * 
  *             c_options = Dictionary(self.options, self.container_options)
  */
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->format)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
-    if (__pyx_t_4) {
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->format)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 258, __pyx_L1_error)
+    if (__pyx_t_2) {
       __pyx_t_13 = __pyx_v_self->format->iptr;
     } else {
       __pyx_t_13 = NULL;
     }
     __pyx_v_ifmt = __pyx_t_13;
 
-    /* "av/container/core.pyx":173
+    /* "av/container/core.pyx":260
  *             ifmt = self.format.iptr if self.format else NULL
  * 
  *             c_options = Dictionary(self.options, self.container_options)             # <<<<<<<<<<<<<<
  * 
  *             self.set_timeout(self.open_timeout)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 260, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_6 = NULL;
-    __pyx_t_11 = 0;
+    __pyx_t_9 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
-        __pyx_t_11 = 1;
+        __pyx_t_9 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_self->options, __pyx_v_self->container_options};
-      __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_5);
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
       PyObject *__pyx_temp[3] = {__pyx_t_6, __pyx_v_self->options, __pyx_v_self->container_options};
-      __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_11, 2+__pyx_t_11); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_5);
     } else
     #endif
     {
-      __pyx_t_14 = PyTuple_New(2+__pyx_t_11); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 173, __pyx_L1_error)
+      __pyx_t_14 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 260, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_14);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_INCREF(__pyx_v_self->options);
       __Pyx_GIVEREF(__pyx_v_self->options);
-      PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_11, __pyx_v_self->options);
+      PyTuple_SET_ITEM(__pyx_t_14, 0+__pyx_t_9, __pyx_v_self->options);
       __Pyx_INCREF(__pyx_v_self->container_options);
       __Pyx_GIVEREF(__pyx_v_self->container_options);
-      PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_11, __pyx_v_self->container_options);
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_14, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 173, __pyx_L1_error)
+      PyTuple_SET_ITEM(__pyx_t_14, 1+__pyx_t_9, __pyx_v_self->container_options);
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_14, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 260, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 173, __pyx_L1_error)
+    if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 260, __pyx_L1_error)
     __pyx_v_c_options = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "av/container/core.pyx":175
+    /* "av/container/core.pyx":262
  *             c_options = Dictionary(self.options, self.container_options)
  * 
  *             self.set_timeout(self.open_timeout)             # <<<<<<<<<<<<<<
  *             self.start_timeout()
  *             with nogil:
  */
     __pyx_t_5 = __pyx_v_self->open_timeout;
     __Pyx_INCREF(__pyx_t_5);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->set_timeout(__pyx_v_self, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->set_timeout(__pyx_v_self, __pyx_t_5); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 262, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":176
+    /* "av/container/core.pyx":263
  * 
  *             self.set_timeout(self.open_timeout)
  *             self.start_timeout()             # <<<<<<<<<<<<<<
  *             with nogil:
  *                 res = lib.avformat_open_input(
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->start_timeout(__pyx_v_self); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->start_timeout(__pyx_v_self); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":177
+    /* "av/container/core.pyx":264
  *             self.set_timeout(self.open_timeout)
  *             self.start_timeout()
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 res = lib.avformat_open_input(
  *                     &self.ptr,
  */
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
 
-          /* "av/container/core.pyx":178
+          /* "av/container/core.pyx":265
  *             self.start_timeout()
  *             with nogil:
  *                 res = lib.avformat_open_input(             # <<<<<<<<<<<<<<
  *                     &self.ptr,
  *                     name,
  */
           __pyx_v_res = avformat_open_input((&__pyx_v_self->ptr), __pyx_v_name, __pyx_v_ifmt, (&__pyx_v_c_options->ptr));
         }
 
-        /* "av/container/core.pyx":177
+        /* "av/container/core.pyx":264
  *             self.set_timeout(self.open_timeout)
  *             self.start_timeout()
  *             with nogil:             # <<<<<<<<<<<<<<
  *                 res = lib.avformat_open_input(
  *                     &self.ptr,
  */
         /*finally:*/ {
           /*normal exit:*/{
             #ifdef WITH_THREAD
             __Pyx_FastGIL_Forget();
             Py_BLOCK_THREADS
             #endif
-            goto __pyx_L29;
+            goto __pyx_L30;
           }
-          __pyx_L29:;
+          __pyx_L30:;
         }
     }
 
-    /* "av/container/core.pyx":184
+    /* "av/container/core.pyx":271
  *                     &c_options.ptr
  *                 )
  *             self.set_timeout(None)             # <<<<<<<<<<<<<<
  *             self.err_check(res)
  *             self.input_was_opened = True
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->set_timeout(__pyx_v_self, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->set_timeout(__pyx_v_self, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":185
+    /* "av/container/core.pyx":272
  *                 )
  *             self.set_timeout(None)
  *             self.err_check(res)             # <<<<<<<<<<<<<<
  *             self.input_was_opened = True
  * 
  */
-    __pyx_t_11 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->err_check(__pyx_v_self, __pyx_v_res); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_9 = ((struct __pyx_vtabstruct_2av_9container_4core_Container *)__pyx_v_self->__pyx_vtab)->err_check(__pyx_v_self, __pyx_v_res); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(0, 272, __pyx_L1_error)
 
-    /* "av/container/core.pyx":186
+    /* "av/container/core.pyx":273
  *             self.set_timeout(None)
  *             self.err_check(res)
  *             self.input_was_opened = True             # <<<<<<<<<<<<<<
  * 
  *         if format_name is None:
  */
     __pyx_v_self->input_was_opened = 1;
 
-    /* "av/container/core.pyx":169
+    /* "av/container/core.pyx":256
  *         cdef lib.AVInputFormat *ifmt
  *         cdef _Dictionary c_options
  *         if not self.writeable:             # <<<<<<<<<<<<<<
  * 
  *             ifmt = self.format.iptr if self.format else NULL
  */
   }
 
-  /* "av/container/core.pyx":188
+  /* "av/container/core.pyx":275
  *             self.input_was_opened = True
  * 
  *         if format_name is None:             # <<<<<<<<<<<<<<
  *             self.format = build_container_format(self.ptr.iformat, self.ptr.oformat)
  * 
  */
-  __pyx_t_4 = (__pyx_v_format_name == Py_None);
-  __pyx_t_2 = (__pyx_t_4 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_2 = (__pyx_v_format_name == Py_None);
+  __pyx_t_4 = (__pyx_t_2 != 0);
+  if (__pyx_t_4) {
 
-    /* "av/container/core.pyx":189
+    /* "av/container/core.pyx":276
  * 
  *         if format_name is None:
  *             self.format = build_container_format(self.ptr.iformat, self.ptr.oformat)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-    __pyx_t_3 = ((PyObject *)__pyx_f_2av_6format_build_container_format(__pyx_v_self->ptr->iformat, __pyx_v_self->ptr->oformat)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_f_2av_6format_build_container_format(__pyx_v_self->ptr->iformat, __pyx_v_self->ptr->oformat)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 276, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->format);
     __Pyx_DECREF(((PyObject *)__pyx_v_self->format));
     __pyx_v_self->format = ((struct __pyx_obj_2av_6format_ContainerFormat *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":188
+    /* "av/container/core.pyx":275
  *             self.input_was_opened = True
  * 
  *         if format_name is None:             # <<<<<<<<<<<<<<
  *             self.format = build_container_format(self.ptr.iformat, self.ptr.oformat)
  * 
  */
   }
 
-  /* "av/container/core.pyx":97
+  /* "av/container/core.pyx":173
  * cdef class Container(object):
  * 
  *     def __cinit__(self, sentinel, file_, format_name, options,             # <<<<<<<<<<<<<<
  *                   container_options, stream_options,
  *                   metadata_encoding, metadata_errors,
  */
 
@@ -4013,15 +4951,15 @@
   __Pyx_XDECREF(__pyx_v_name_obj);
   __Pyx_XDECREF((PyObject *)__pyx_v_c_options);
   __Pyx_XDECREF(__pyx_v_x);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":191
+/* "av/container/core.pyx":278
  *             self.format = build_container_format(self.ptr.iformat, self.ptr.oformat)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             lib.avformat_free_context(self.ptr)
  */
 
@@ -4036,40 +4974,40 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_pf_2av_9container_4core_9Container_2__dealloc__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "av/container/core.pyx":192
+  /* "av/container/core.pyx":279
  * 
  *     def __dealloc__(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             lib.avformat_free_context(self.ptr)
  * 
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/container/core.pyx":193
+        /* "av/container/core.pyx":280
  *     def __dealloc__(self):
  *         with nogil:
  *             lib.avformat_free_context(self.ptr)             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
         (void)(avformat_free_context(__pyx_v_self->ptr));
       }
 
-      /* "av/container/core.pyx":192
+      /* "av/container/core.pyx":279
  * 
  *     def __dealloc__(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             lib.avformat_free_context(self.ptr)
  * 
  */
       /*finally:*/ {
@@ -4080,27 +5018,27 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "av/container/core.pyx":191
+  /* "av/container/core.pyx":278
  *             self.format = build_container_format(self.ptr.iformat, self.ptr.oformat)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             lib.avformat_free_context(self.ptr)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "av/container/core.pyx":195
+/* "av/container/core.pyx":282
  *             lib.avformat_free_context(self.ptr)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -4119,42 +5057,42 @@
 }
 
 static PyObject *__pyx_pf_2av_9container_4core_9Container_4__enter__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "av/container/core.pyx":196
+  /* "av/container/core.pyx":283
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "av/container/core.pyx":195
+  /* "av/container/core.pyx":282
  *             lib.avformat_free_context(self.ptr)
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":198
+/* "av/container/core.pyx":285
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -4192,40 +5130,40 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_val)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 1); __PYX_ERR(0, 285, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_exc_tb)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 198, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, 2); __PYX_ERR(0, 285, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 198, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__exit__") < 0)) __PYX_ERR(0, 285, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_exc_type = values[0];
     __pyx_v_exc_val = values[1];
     __pyx_v_exc_tb = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 198, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__exit__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 285, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.container.core.Container.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_2av_9container_4core_9Container_6__exit__(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_exc_type, __pyx_v_exc_val, __pyx_v_exc_tb);
 
@@ -4241,41 +5179,41 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "av/container/core.pyx":199
+  /* "av/container/core.pyx":286
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/core.pyx":198
+  /* "av/container/core.pyx":285
  *         return self
  * 
  *     def __exit__(self, exc_type, exc_val, exc_tb):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -4290,15 +5228,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":201
+/* "av/container/core.pyx":288
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<av.%s %r>' % (self.__class__.__name__, self.file or self.name)
  * 
  */
 
@@ -4323,53 +5261,53 @@
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "av/container/core.pyx":202
+  /* "av/container/core.pyx":289
  * 
  *     def __repr__(self):
  *         return '<av.%s %r>' % (self.__class__.__name__, self.file or self.name)             # <<<<<<<<<<<<<<
  * 
  *     cdef int err_check(self, int value) except -1:
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->file)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(((PyObject *)__pyx_v_self->file)); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 289, __pyx_L1_error)
   if (!__pyx_t_3) {
   } else {
     __Pyx_INCREF(((PyObject *)__pyx_v_self->file));
     __pyx_t_1 = ((PyObject *)__pyx_v_self->file);
     goto __pyx_L3_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_t_1 = __pyx_v_self->name;
   __pyx_L3_bool_binop_done:;
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_av_s_r, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_av_s_r, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/container/core.pyx":201
+  /* "av/container/core.pyx":288
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return '<av.%s %r>' % (self.__class__.__name__, self.file or self.name)
  * 
  */
 
@@ -4382,15 +5320,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":204
+/* "av/container/core.pyx":291
  *         return '<av.%s %r>' % (self.__class__.__name__, self.file or self.name)
  * 
  *     cdef int err_check(self, int value) except -1:             # <<<<<<<<<<<<<<
  *         return err_check(value, filename=self.name)
  * 
  */
 
@@ -4401,31 +5339,31 @@
   int __pyx_t_2;
   struct __pyx_opt_args_2av_5error_err_check __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("err_check", 0);
 
-  /* "av/container/core.pyx":205
+  /* "av/container/core.pyx":292
  * 
  *     cdef int err_check(self, int value) except -1:
  *         return err_check(value, filename=self.name)             # <<<<<<<<<<<<<<
  * 
  *     def dumps_format(self):
  */
   __pyx_t_1 = __pyx_v_self->name;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_3.__pyx_n = 1;
   __pyx_t_3.filename = __pyx_t_1;
-  __pyx_t_2 = __pyx_f_2av_5error_err_check(__pyx_v_value, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 205, __pyx_L1_error)
+  __pyx_t_2 = __pyx_f_2av_5error_err_check(__pyx_v_value, 0, &__pyx_t_3); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 292, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "av/container/core.pyx":204
+  /* "av/container/core.pyx":291
  *         return '<av.%s %r>' % (self.__class__.__name__, self.file or self.name)
  * 
  *     cdef int err_check(self, int value) except -1:             # <<<<<<<<<<<<<<
  *         return err_check(value, filename=self.name)
  * 
  */
 
@@ -4435,15 +5373,15 @@
   __Pyx_AddTraceback("av.container.core.Container.err_check", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":207
+/* "av/container/core.pyx":294
  *         return err_check(value, filename=self.name)
  * 
  *     def dumps_format(self):             # <<<<<<<<<<<<<<
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  */
 
@@ -4458,15 +5396,15 @@
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2av_9container_4core_9Container_12dumps_format_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "av/container/core.pyx":210
+/* "av/container/core.pyx":297
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)             # <<<<<<<<<<<<<<
  * 
  *     cdef set_timeout(self, timeout):
  */
 
@@ -4478,23 +5416,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2av_9container_4core___pyx_scope_struct_1_genexpr *)__pyx_tp_new_2av_9container_4core___pyx_scope_struct_1_genexpr(__pyx_ptype_2av_9container_4core___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2av_9container_4core___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 210, __pyx_L1_error)
+    __PYX_ERR(0, 297, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_2av_9container_4core___pyx_scope_struct__dumps_format *) __pyx_self;
   __Pyx_INCREF(((PyObject *)__pyx_cur_scope->__pyx_outer_scope));
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_outer_scope);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2av_9container_4core_9Container_12dumps_format_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_dumps_format_locals_genexpr, __pyx_n_s_av_container_core); if (unlikely(!gen)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2av_9container_4core_9Container_12dumps_format_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_dumps_format_locals_genexpr, __pyx_n_s_av_container_core); if (unlikely(!gen)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4523,60 +5461,60 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L6_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 210, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs)) { __Pyx_RaiseClosureNameError("logs"); __PYX_ERR(0, 210, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 297, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs)) { __Pyx_RaiseClosureNameError("logs"); __PYX_ERR(0, 297, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs; __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_logs); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 210, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 297, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 210, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 297, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 210, __pyx_L1_error)
+          else __PYX_ERR(0, 297, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_log);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_log, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_log, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_log, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 297, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     __Pyx_XGIVEREF(__pyx_t_1);
     __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
     __pyx_cur_scope->__pyx_t_1 = __pyx_t_2;
     __pyx_cur_scope->__pyx_t_2 = __pyx_t_3;
@@ -4588,15 +5526,15 @@
     return __pyx_r;
     __pyx_L6_resume_from_yield:;
     __pyx_t_1 = __pyx_cur_scope->__pyx_t_0;
     __pyx_cur_scope->__pyx_t_0 = 0;
     __Pyx_XGOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
     __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
-    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 210, __pyx_L1_error)
+    if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 297, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   PyErr_SetNone(PyExc_StopIteration);
   goto __pyx_L0;
@@ -4611,15 +5549,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":207
+/* "av/container/core.pyx":294
  *         return err_check(value, filename=self.name)
  * 
  *     def dumps_format(self):             # <<<<<<<<<<<<<<
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  */
 
@@ -4641,132 +5579,132 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dumps_format", 0);
   __pyx_cur_scope = (struct __pyx_obj_2av_9container_4core___pyx_scope_struct__dumps_format *)__pyx_tp_new_2av_9container_4core___pyx_scope_struct__dumps_format(__pyx_ptype_2av_9container_4core___pyx_scope_struct__dumps_format, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2av_9container_4core___pyx_scope_struct__dumps_format *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 207, __pyx_L1_error)
+    __PYX_ERR(0, 294, __pyx_L1_error)
   } else {
     __Pyx_GOTREF(__pyx_cur_scope);
   }
 
-  /* "av/container/core.pyx":208
+  /* "av/container/core.pyx":295
  * 
  *     def dumps_format(self):
  *         with LogCapture() as logs:             # <<<<<<<<<<<<<<
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)
  */
   /*with:*/ {
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogCapture); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_LogCapture); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_exit); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 295, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 208, __pyx_L3_error)
+    __pyx_t_3 = __Pyx_PyObject_LookupSpecial(__pyx_t_1, __pyx_n_s_enter); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 295, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_5) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L3_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L3_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = __pyx_t_2;
     __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     /*try:*/ {
       {
         (void)__pyx_t_6; (void)__pyx_t_7; (void)__pyx_t_8; /* mark used */
         /*try:*/ {
           __Pyx_GIVEREF(__pyx_t_3);
           __pyx_cur_scope->__pyx_v_logs = __pyx_t_3;
           __pyx_t_3 = 0;
 
-          /* "av/container/core.pyx":209
+          /* "av/container/core.pyx":296
  *     def dumps_format(self):
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))             # <<<<<<<<<<<<<<
  *         return ''.join(log[2] for log in logs)
  * 
  */
           __pyx_t_9 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_2av_9container_6output_OutputContainer); 
           av_dump_format(__pyx_v_self->ptr, 0, ((char *)""), __pyx_t_9);
 
-          /* "av/container/core.pyx":208
+          /* "av/container/core.pyx":295
  * 
  *     def dumps_format(self):
  *         with LogCapture() as logs:             # <<<<<<<<<<<<<<
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)
  */
         }
       }
     }
     /*finally:*/ {
       /*normal exit:*/{
         if (__pyx_t_4) {
-          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__5, NULL);
+          __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_tuple__6, NULL);
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 208, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 295, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         goto __pyx_L6;
       }
       __pyx_L6:;
     }
     goto __pyx_L13;
     __pyx_L3_error:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L1_error;
     __pyx_L13:;
   }
 
-  /* "av/container/core.pyx":210
+  /* "av/container/core.pyx":297
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)             # <<<<<<<<<<<<<<
  * 
  *     cdef set_timeout(self, timeout):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = __pyx_pf_2av_9container_4core_9Container_12dumps_format_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_3 = __pyx_pf_2av_9container_4core_9Container_12dumps_format_genexpr(((PyObject*)__pyx_cur_scope)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__6, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Join(__pyx_kp_s__2, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 297, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/container/core.pyx":207
+  /* "av/container/core.pyx":294
  *         return err_check(value, filename=self.name)
  * 
  *     def dumps_format(self):             # <<<<<<<<<<<<<<
  *         with LogCapture() as logs:
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  */
 
@@ -4782,15 +5720,15 @@
   __Pyx_XDECREF(__pyx_gb_2av_9container_4core_9Container_12dumps_format_2generator);
   __Pyx_DECREF(((PyObject *)__pyx_cur_scope));
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":212
+/* "av/container/core.pyx":299
  *         return ''.join(log[2] for log in logs)
  * 
  *     cdef set_timeout(self, timeout):             # <<<<<<<<<<<<<<
  *         if timeout is None:
  *             self.interrupt_callback_info.timeout = -1.0
  */
 
@@ -4801,58 +5739,58 @@
   int __pyx_t_2;
   double __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_timeout", 0);
 
-  /* "av/container/core.pyx":213
+  /* "av/container/core.pyx":300
  * 
  *     cdef set_timeout(self, timeout):
  *         if timeout is None:             # <<<<<<<<<<<<<<
  *             self.interrupt_callback_info.timeout = -1.0
  *         else:
  */
   __pyx_t_1 = (__pyx_v_timeout == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":214
+    /* "av/container/core.pyx":301
  *     cdef set_timeout(self, timeout):
  *         if timeout is None:
  *             self.interrupt_callback_info.timeout = -1.0             # <<<<<<<<<<<<<<
  *         else:
  *             self.interrupt_callback_info.timeout = timeout
  */
     __pyx_v_self->interrupt_callback_info.timeout = -1.0;
 
-    /* "av/container/core.pyx":213
+    /* "av/container/core.pyx":300
  * 
  *     cdef set_timeout(self, timeout):
  *         if timeout is None:             # <<<<<<<<<<<<<<
  *             self.interrupt_callback_info.timeout = -1.0
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "av/container/core.pyx":216
+  /* "av/container/core.pyx":303
  *             self.interrupt_callback_info.timeout = -1.0
  *         else:
  *             self.interrupt_callback_info.timeout = timeout             # <<<<<<<<<<<<<<
  * 
  *     cdef start_timeout(self):
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_timeout); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 216, __pyx_L1_error)
+    __pyx_t_3 = __pyx_PyFloat_AsDouble(__pyx_v_timeout); if (unlikely((__pyx_t_3 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 303, __pyx_L1_error)
     __pyx_v_self->interrupt_callback_info.timeout = __pyx_t_3;
   }
   __pyx_L3:;
 
-  /* "av/container/core.pyx":212
+  /* "av/container/core.pyx":299
  *         return ''.join(log[2] for log in logs)
  * 
  *     cdef set_timeout(self, timeout):             # <<<<<<<<<<<<<<
  *         if timeout is None:
  *             self.interrupt_callback_info.timeout = -1.0
  */
 
@@ -4864,15 +5802,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":218
+/* "av/container/core.pyx":305
  *             self.interrupt_callback_info.timeout = timeout
  * 
  *     cdef start_timeout(self):             # <<<<<<<<<<<<<<
  *         self.interrupt_callback_info.start_time = clock()
  * 
  */
 
@@ -4884,15 +5822,15 @@
   PyObject *__pyx_t_3 = NULL;
   double __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("start_timeout", 0);
 
-  /* "av/container/core.pyx":219
+  /* "av/container/core.pyx":306
  * 
  *     cdef start_timeout(self):
  *         self.interrupt_callback_info.start_time = clock()             # <<<<<<<<<<<<<<
  * 
  *     def _get_flags(self):
  */
   __Pyx_INCREF(__pyx_v_2av_9container_4core_clock);
@@ -4904,22 +5842,22 @@
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_4 = __pyx_PyFloat_AsDouble(__pyx_t_1); if (unlikely((__pyx_t_4 == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 306, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->interrupt_callback_info.start_time = __pyx_t_4;
 
-  /* "av/container/core.pyx":218
+  /* "av/container/core.pyx":305
  *             self.interrupt_callback_info.timeout = timeout
  * 
  *     cdef start_timeout(self):             # <<<<<<<<<<<<<<
  *         self.interrupt_callback_info.start_time = clock()
  * 
  */
 
@@ -4934,15 +5872,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":221
+/* "av/container/core.pyx":308
  *         self.interrupt_callback_info.start_time = clock()
  * 
  *     def _get_flags(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags
  * 
  */
 
@@ -4965,29 +5903,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_get_flags", 0);
 
-  /* "av/container/core.pyx":222
+  /* "av/container/core.pyx":309
  * 
  *     def _get_flags(self):
  *         return self.ptr.flags             # <<<<<<<<<<<<<<
  * 
  *     def _set_flags(self, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->ptr->flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/container/core.pyx":221
+  /* "av/container/core.pyx":308
  *         self.interrupt_callback_info.start_time = clock()
  * 
  *     def _get_flags(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.flags
  * 
  */
 
@@ -4998,15 +5936,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":224
+/* "av/container/core.pyx":311
  *         return self.ptr.flags
  * 
  *     def _set_flags(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags = value
  * 
  */
 
@@ -5029,25 +5967,25 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_set_flags", 0);
 
-  /* "av/container/core.pyx":225
+  /* "av/container/core.pyx":312
  * 
  *     def _set_flags(self, value):
  *         self.ptr.flags = value             # <<<<<<<<<<<<<<
  * 
  *     flags = Flags.property(
  */
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 225, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 312, __pyx_L1_error)
   __pyx_v_self->ptr->flags = __pyx_t_1;
 
-  /* "av/container/core.pyx":224
+  /* "av/container/core.pyx":311
  *         return self.ptr.flags
  * 
  *     def _set_flags(self, value):             # <<<<<<<<<<<<<<
  *         self.ptr.flags = value
  * 
  */
 
@@ -5221,16 +6159,16 @@
   return __pyx_r;
 }
 
 /* "av/container/core.pxd":25
  *     cdef readonly str metadata_errors
  * 
  *     cdef readonly PyIOFile file             # <<<<<<<<<<<<<<
+ *     cdef int buffer_size
  *     cdef bint input_was_opened
- * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9container_4core_9Container_4file_1__get__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_2av_9container_4core_9Container_4file_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5255,15 +6193,89 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "av/container/core.pxd":28
+ *     cdef int buffer_size
  *     cdef bint input_was_opened
+ *     cdef readonly object io_open             # <<<<<<<<<<<<<<
+ *     cdef readonly object open_files
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_2av_9container_4core_9Container_7io_open_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_2av_9container_4core_9Container_7io_open_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_2av_9container_4core_9Container_7io_open___get__(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_2av_9container_4core_9Container_7io_open___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->io_open);
+  __pyx_r = __pyx_v_self->io_open;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "av/container/core.pxd":29
+ *     cdef bint input_was_opened
+ *     cdef readonly object io_open
+ *     cdef readonly object open_files             # <<<<<<<<<<<<<<
+ * 
+ *     cdef readonly ContainerFormat format
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_2av_9container_4core_9Container_10open_files_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_2av_9container_4core_9Container_10open_files_1__get__(PyObject *__pyx_v_self) {
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
+  __pyx_r = __pyx_pf_2av_9container_4core_9Container_10open_files___get__(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self));
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_2av_9container_4core_9Container_10open_files___get__(struct __pyx_obj_2av_9container_4core_Container *__pyx_v_self) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("__get__", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_self->open_files);
+  __pyx_r = __pyx_v_self->open_files;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "av/container/core.pxd":31
+ *     cdef readonly object open_files
  * 
  *     cdef readonly ContainerFormat format             # <<<<<<<<<<<<<<
  * 
  *     cdef readonly dict options
  */
 
 /* Python wrapper */
@@ -5291,15 +6303,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":30
+/* "av/container/core.pxd":33
  *     cdef readonly ContainerFormat format
  * 
  *     cdef readonly dict options             # <<<<<<<<<<<<<<
  *     cdef readonly dict container_options
  *     cdef readonly list stream_options
  */
 
@@ -5328,15 +6340,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":31
+/* "av/container/core.pxd":34
  * 
  *     cdef readonly dict options
  *     cdef readonly dict container_options             # <<<<<<<<<<<<<<
  *     cdef readonly list stream_options
  * 
  */
 
@@ -5365,15 +6377,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":32
+/* "av/container/core.pxd":35
  *     cdef readonly dict options
  *     cdef readonly dict container_options
  *     cdef readonly list stream_options             # <<<<<<<<<<<<<<
  * 
  *     cdef readonly StreamContainer streams
  */
 
@@ -5402,15 +6414,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":34
+/* "av/container/core.pxd":37
  *     cdef readonly list stream_options
  * 
  *     cdef readonly StreamContainer streams             # <<<<<<<<<<<<<<
  *     cdef readonly dict metadata
  * 
  */
 
@@ -5439,15 +6451,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":35
+/* "av/container/core.pxd":38
  * 
  *     cdef readonly StreamContainer streams
  *     cdef readonly dict metadata             # <<<<<<<<<<<<<<
  * 
  *     cdef int err_check(self, int value) except -1
  */
 
@@ -5476,15 +6488,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":40
+/* "av/container/core.pxd":43
  * 
  *     # Timeouts
  *     cdef readonly object open_timeout             # <<<<<<<<<<<<<<
  *     cdef readonly object read_timeout
  *     cdef timeout_info interrupt_callback_info
  */
 
@@ -5513,15 +6525,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pxd":41
+/* "av/container/core.pxd":44
  *     # Timeouts
  *     cdef readonly object open_timeout
  *     cdef readonly object read_timeout             # <<<<<<<<<<<<<<
  *     cdef timeout_info interrupt_callback_info
  *     cdef set_timeout(self, object)
  */
 
@@ -5665,75 +6677,79 @@
   __Pyx_AddTraceback("av.container.core.Container.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/core.pyx":251
+/* "av/container/core.pyx":338
  * 
  * 
  * def open(file, mode=None, format=None, options=None,             # <<<<<<<<<<<<<<
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_9container_4core_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_2av_9container_4core_open[] = "open(file, mode='r', **kwargs)\n\n    Main entrypoint to opening files/streams.\n\n    :param str file: The file to open, which can be either a string or a file-like object.\n    :param str mode: ``\"r\"`` for reading and ``\"w\"`` for writing.\n    :param str format: Specific format to use. Defaults to autodect.\n    :param dict options: Options to pass to the container and all streams.\n    :param dict container_options: Options to pass to the container.\n    :param list stream_options: Options to pass to each stream.\n    :param str metadata_encoding: Encoding to use when reading or writing file metadata.\n        Defaults to ``\"utf-8\"``.\n    :param str metadata_errors: Specifies how to handle encoding errors; behaves like\n        ``str.encode`` parameter. Defaults to ``\"strict\"``.\n    :param int buffer_size: Size of buffer for Python input/output operations in bytes.\n        Honored only when ``file`` is a file-like object. Defaults to 32768 (32k).\n    :param timeout: How many seconds to wait for data before giving up, as a float, or a\n        :ref:`(open timeout, read timeout) <timeouts>` tuple.\n    :type timeout: float or tuple\n\n    For devices (via ``libavdevice``), pass the name of the device to ``format``,\n    e.g.::\n\n        >>> # Open webcam on OS X.\n        >>> av.open(format='avfoundation', file='0') # doctest: +SKIP\n\n    .. seealso:: :ref:`garbage_collection`\n\n    More information on using input and output devices is available on the\n    `FFmpeg website <https://www.ffmpeg.org/ffmpeg-devices.html>`_.\n    ";
+static char __pyx_doc_2av_9container_4core_open[] = "open(file, mode='r', **kwargs)\n\n    Main entrypoint to opening files/streams.\n\n    :param str file: The file to open, which can be either a string or a file-like object.\n    :param str mode: ``\"r\"`` for reading and ``\"w\"`` for writing.\n    :param str format: Specific format to use. Defaults to autodect.\n    :param dict options: Options to pass to the container and all streams.\n    :param dict container_options: Options to pass to the container.\n    :param list stream_options: Options to pass to each stream.\n    :param str metadata_encoding: Encoding to use when reading or writing file metadata.\n        Defaults to ``\"utf-8\"``.\n    :param str metadata_errors: Specifies how to handle encoding errors; behaves like\n        ``str.encode`` parameter. Defaults to ``\"strict\"``.\n    :param int buffer_size: Size of buffer for Python input/output operations in bytes.\n        Honored only when ``file`` is a file-like object. Defaults to 32768 (32k).\n    :param timeout: How many seconds to wait for data before giving up, as a float, or a\n        :ref:`(open timeout, read timeout) <timeouts>` tuple.\n    :type timeout: float or tuple\n    :param callable io_open: Custom I/O callable for opening files/streams.\n        This option is intended for formats that need to open additional\n        file-like objects to ``file`` using custom I/O.\n        The callable signature is ``io_open(url: str, flags: int, options: dict)``, where\n        ``url`` is the url to open, ``flags`` is a combination of AVIO_FLAG_* and\n        ``options`` is a dictionary of additional options. The callable should return a\n        file-like object.\n\n    For devices (via ``libavdevice``), pass the name of the device to ``format``,\n    e.g.::\n\n        >>> # Open webcam on OS X.\n        >>> av.open(format='avfoundation', file='0') # doctest: +SKIP\n\n    For DASH and custom I/O using ``io_open``, add a protocol prefix to the ``file`` to\n    prevent the DASH encoder defaulting t""o the file protocol and using temporary files.\n    The custom I/O callable can be used to remove the protocol prefix to reveal the actual\n    name for creating the file-like object. E.g.::\n\n        >>> av.open(\"customprotocol://manifest.mpd\", \"w\", io_open=custom_io) # doctest: +SKIP\n\n    .. seealso:: :ref:`garbage_collection`\n\n    More information on using input and output devices is available on the\n    `FFmpeg website <https://www.ffmpeg.org/ffmpeg-devices.html>`_.\n    ";
 static PyMethodDef __pyx_mdef_2av_9container_4core_1open = {"open", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_2av_9container_4core_1open, METH_VARARGS|METH_KEYWORDS, __pyx_doc_2av_9container_4core_open};
 static PyObject *__pyx_pw_2av_9container_4core_1open(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_file = 0;
   PyObject *__pyx_v_mode = 0;
   PyObject *__pyx_v_format = 0;
   PyObject *__pyx_v_options = 0;
   PyObject *__pyx_v_container_options = 0;
   PyObject *__pyx_v_stream_options = 0;
   PyObject *__pyx_v_metadata_encoding = 0;
   PyObject *__pyx_v_metadata_errors = 0;
   PyObject *__pyx_v_buffer_size = 0;
   PyObject *__pyx_v_timeout = 0;
+  PyObject *__pyx_v_io_open = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("open (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file_2,&__pyx_n_s_mode,&__pyx_n_s_format,&__pyx_n_s_options,&__pyx_n_s_container_options,&__pyx_n_s_stream_options,&__pyx_n_s_metadata_encoding,&__pyx_n_s_metadata_errors,&__pyx_n_s_buffer_size,&__pyx_n_s_timeout,0};
-    PyObject* values[10] = {0,0,0,0,0,0,0,0,0,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_file_2,&__pyx_n_s_mode,&__pyx_n_s_format,&__pyx_n_s_options,&__pyx_n_s_container_options,&__pyx_n_s_stream_options,&__pyx_n_s_metadata_encoding,&__pyx_n_s_metadata_errors,&__pyx_n_s_buffer_size,&__pyx_n_s_timeout,&__pyx_n_s_io_open,0};
+    PyObject* values[11] = {0,0,0,0,0,0,0,0,0,0,0};
     values[1] = ((PyObject *)Py_None);
     values[2] = ((PyObject *)Py_None);
     values[3] = ((PyObject *)Py_None);
 
-    /* "av/container/core.pyx":252
+    /* "av/container/core.pyx":339
  * 
  * def open(file, mode=None, format=None, options=None,
  *          container_options=None, stream_options=None,             # <<<<<<<<<<<<<<
  *          metadata_encoding='utf-8', metadata_errors='strict',
- *          buffer_size=32768, timeout=None):
+ *          buffer_size=32768, timeout=None, io_open=None):
  */
     values[4] = ((PyObject *)Py_None);
     values[5] = ((PyObject *)Py_None);
     values[6] = ((PyObject *)__pyx_kp_s_utf_8);
     values[7] = ((PyObject *)__pyx_n_s_strict);
     values[8] = ((PyObject *)__pyx_int_32768);
 
-    /* "av/container/core.pyx":254
+    /* "av/container/core.pyx":341
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
- *          buffer_size=32768, timeout=None):             # <<<<<<<<<<<<<<
+ *          buffer_size=32768, timeout=None, io_open=None):             # <<<<<<<<<<<<<<
  *     """open(file, mode='r', **kwargs)
  * 
  */
     values[9] = ((PyObject *)Py_None);
+    values[10] = ((PyObject *)Py_None);
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -5808,20 +6824,28 @@
         }
         CYTHON_FALLTHROUGH;
         case  9:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_timeout);
           if (value) { values[9] = value; kw_args--; }
         }
+        CYTHON_FALLTHROUGH;
+        case 10:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_io_open);
+          if (value) { values[10] = value; kw_args--; }
+        }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 251, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open") < 0)) __PYX_ERR(0, 338, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case 11: values[10] = PyTuple_GET_ITEM(__pyx_args, 10);
+        CYTHON_FALLTHROUGH;
         case 10: values[9] = PyTuple_GET_ITEM(__pyx_args, 9);
         CYTHON_FALLTHROUGH;
         case  9: values[8] = PyTuple_GET_ITEM(__pyx_args, 8);
         CYTHON_FALLTHROUGH;
         case  8: values[7] = PyTuple_GET_ITEM(__pyx_args, 7);
         CYTHON_FALLTHROUGH;
         case  7: values[6] = PyTuple_GET_ITEM(__pyx_args, 6);
@@ -5847,39 +6871,40 @@
     __pyx_v_options = values[3];
     __pyx_v_container_options = values[4];
     __pyx_v_stream_options = values[5];
     __pyx_v_metadata_encoding = values[6];
     __pyx_v_metadata_errors = values[7];
     __pyx_v_buffer_size = values[8];
     __pyx_v_timeout = values[9];
+    __pyx_v_io_open = values[10];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 10, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 251, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open", 0, 1, 11, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 338, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.container.core.open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_2av_9container_4core_open(__pyx_self, __pyx_v_file, __pyx_v_mode, __pyx_v_format, __pyx_v_options, __pyx_v_container_options, __pyx_v_stream_options, __pyx_v_metadata_encoding, __pyx_v_metadata_errors, __pyx_v_buffer_size, __pyx_v_timeout);
+  __pyx_r = __pyx_pf_2av_9container_4core_open(__pyx_self, __pyx_v_file, __pyx_v_mode, __pyx_v_format, __pyx_v_options, __pyx_v_container_options, __pyx_v_stream_options, __pyx_v_metadata_encoding, __pyx_v_metadata_errors, __pyx_v_buffer_size, __pyx_v_timeout, __pyx_v_io_open);
 
-  /* "av/container/core.pyx":251
+  /* "av/container/core.pyx":338
  * 
  * 
  * def open(file, mode=None, format=None, options=None,             # <<<<<<<<<<<<<<
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2av_9container_4core_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file, PyObject *__pyx_v_mode, PyObject *__pyx_v_format, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_timeout) {
+static PyObject *__pyx_pf_2av_9container_4core_open(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_file, PyObject *__pyx_v_mode, PyObject *__pyx_v_format, PyObject *__pyx_v_options, PyObject *__pyx_v_container_options, PyObject *__pyx_v_stream_options, PyObject *__pyx_v_metadata_encoding, PyObject *__pyx_v_metadata_errors, PyObject *__pyx_v_buffer_size, PyObject *__pyx_v_timeout, PyObject *__pyx_v_io_open) {
   PyObject *__pyx_v_open_timeout = NULL;
   PyObject *__pyx_v_read_timeout = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -5887,189 +6912,189 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open", 0);
   __Pyx_INCREF(__pyx_v_mode);
 
-  /* "av/container/core.pyx":287
+  /* "av/container/core.pyx":388
  *     """
  * 
  *     if mode is None:             # <<<<<<<<<<<<<<
  *         mode = getattr(file, 'mode', None)
  *     if mode is None:
  */
   __pyx_t_1 = (__pyx_v_mode == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":288
+    /* "av/container/core.pyx":389
  * 
  *     if mode is None:
  *         mode = getattr(file, 'mode', None)             # <<<<<<<<<<<<<<
  *     if mode is None:
  *         mode = 'r'
  */
-    __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_file, __pyx_n_s_mode, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 288, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetAttr3(__pyx_v_file, __pyx_n_s_mode, Py_None); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 389, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF_SET(__pyx_v_mode, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":287
+    /* "av/container/core.pyx":388
  *     """
  * 
  *     if mode is None:             # <<<<<<<<<<<<<<
  *         mode = getattr(file, 'mode', None)
  *     if mode is None:
  */
   }
 
-  /* "av/container/core.pyx":289
+  /* "av/container/core.pyx":390
  *     if mode is None:
  *         mode = getattr(file, 'mode', None)
  *     if mode is None:             # <<<<<<<<<<<<<<
  *         mode = 'r'
  * 
  */
   __pyx_t_2 = (__pyx_v_mode == Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "av/container/core.pyx":290
+    /* "av/container/core.pyx":391
  *         mode = getattr(file, 'mode', None)
  *     if mode is None:
  *         mode = 'r'             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(timeout, tuple):
  */
     __Pyx_INCREF(__pyx_n_s_r);
     __Pyx_DECREF_SET(__pyx_v_mode, __pyx_n_s_r);
 
-    /* "av/container/core.pyx":289
+    /* "av/container/core.pyx":390
  *     if mode is None:
  *         mode = getattr(file, 'mode', None)
  *     if mode is None:             # <<<<<<<<<<<<<<
  *         mode = 'r'
  * 
  */
   }
 
-  /* "av/container/core.pyx":292
+  /* "av/container/core.pyx":393
  *         mode = 'r'
  * 
  *     if isinstance(timeout, tuple):             # <<<<<<<<<<<<<<
  *         open_timeout = timeout[0]
  *         read_timeout = timeout[1]
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_timeout); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":293
+    /* "av/container/core.pyx":394
  * 
  *     if isinstance(timeout, tuple):
  *         open_timeout = timeout[0]             # <<<<<<<<<<<<<<
  *         read_timeout = timeout[1]
  *     else:
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_timeout, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 293, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_timeout, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 394, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_open_timeout = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":294
+    /* "av/container/core.pyx":395
  *     if isinstance(timeout, tuple):
  *         open_timeout = timeout[0]
  *         read_timeout = timeout[1]             # <<<<<<<<<<<<<<
  *     else:
  *         open_timeout = timeout
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_timeout, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 294, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_timeout, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_v_read_timeout = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "av/container/core.pyx":292
+    /* "av/container/core.pyx":393
  *         mode = 'r'
  * 
  *     if isinstance(timeout, tuple):             # <<<<<<<<<<<<<<
  *         open_timeout = timeout[0]
  *         read_timeout = timeout[1]
  */
     goto __pyx_L5;
   }
 
-  /* "av/container/core.pyx":296
+  /* "av/container/core.pyx":397
  *         read_timeout = timeout[1]
  *     else:
  *         open_timeout = timeout             # <<<<<<<<<<<<<<
  *         read_timeout = timeout
  * 
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_timeout);
     __pyx_v_open_timeout = __pyx_v_timeout;
 
-    /* "av/container/core.pyx":297
+    /* "av/container/core.pyx":398
  *     else:
  *         open_timeout = timeout
  *         read_timeout = timeout             # <<<<<<<<<<<<<<
  * 
  *     if mode.startswith('r'):
  */
     __Pyx_INCREF(__pyx_v_timeout);
     __pyx_v_read_timeout = __pyx_v_timeout;
   }
   __pyx_L5:;
 
-  /* "av/container/core.pyx":299
+  /* "av/container/core.pyx":400
  *         read_timeout = timeout
  * 
  *     if mode.startswith('r'):             # <<<<<<<<<<<<<<
  *         return InputContainer(
  *             _cinit_sentinel, file, format, options,
  */
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_startswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_startswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_n_s_r) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_n_s_r);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 299, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 400, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":300
+    /* "av/container/core.pyx":401
  * 
  *     if mode.startswith('r'):
  *         return InputContainer(             # <<<<<<<<<<<<<<
  *             _cinit_sentinel, file, format, options,
  *             container_options, stream_options,
  */
     __Pyx_XDECREF(__pyx_r);
 
-    /* "av/container/core.pyx":304
- *             container_options, stream_options,
+    /* "av/container/core.pyx":406
  *             metadata_encoding, metadata_errors,
- *             buffer_size, open_timeout, read_timeout             # <<<<<<<<<<<<<<
+ *             buffer_size, open_timeout, read_timeout,
+ *             io_open             # <<<<<<<<<<<<<<
  *         )
  *     if mode.startswith('w'):
  */
-    __pyx_t_3 = PyTuple_New(11); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(12); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_2av_9container_4core__cinit_sentinel);
     __Pyx_GIVEREF(__pyx_v_2av_9container_4core__cinit_sentinel);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_2av_9container_4core__cinit_sentinel);
     __Pyx_INCREF(__pyx_v_file);
     __Pyx_GIVEREF(__pyx_v_file);
     PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_file);
@@ -6096,115 +7121,118 @@
     PyTuple_SET_ITEM(__pyx_t_3, 8, __pyx_v_buffer_size);
     __Pyx_INCREF(__pyx_v_open_timeout);
     __Pyx_GIVEREF(__pyx_v_open_timeout);
     PyTuple_SET_ITEM(__pyx_t_3, 9, __pyx_v_open_timeout);
     __Pyx_INCREF(__pyx_v_read_timeout);
     __Pyx_GIVEREF(__pyx_v_read_timeout);
     PyTuple_SET_ITEM(__pyx_t_3, 10, __pyx_v_read_timeout);
+    __Pyx_INCREF(__pyx_v_io_open);
+    __Pyx_GIVEREF(__pyx_v_io_open);
+    PyTuple_SET_ITEM(__pyx_t_3, 11, __pyx_v_io_open);
 
-    /* "av/container/core.pyx":300
+    /* "av/container/core.pyx":401
  * 
  *     if mode.startswith('r'):
  *         return InputContainer(             # <<<<<<<<<<<<<<
  *             _cinit_sentinel, file, format, options,
  *             container_options, stream_options,
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_5input_InputContainer), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_5input_InputContainer), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "av/container/core.pyx":299
+    /* "av/container/core.pyx":400
  *         read_timeout = timeout
  * 
  *     if mode.startswith('r'):             # <<<<<<<<<<<<<<
  *         return InputContainer(
  *             _cinit_sentinel, file, format, options,
  */
   }
 
-  /* "av/container/core.pyx":306
- *             buffer_size, open_timeout, read_timeout
+  /* "av/container/core.pyx":408
+ *             io_open
  *         )
  *     if mode.startswith('w'):             # <<<<<<<<<<<<<<
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_mode, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_5, __pyx_n_s_w) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_s_w);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 306, __pyx_L1_error)
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_2) {
 
-    /* "av/container/core.pyx":307
+    /* "av/container/core.pyx":409
  *         )
  *     if mode.startswith('w'):
  *         if stream_options:             # <<<<<<<<<<<<<<
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  *         return OutputContainer(
  */
-    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_stream_options); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 307, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_stream_options); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
     if (unlikely(__pyx_t_2)) {
 
-      /* "av/container/core.pyx":308
+      /* "av/container/core.pyx":410
  *     if mode.startswith('w'):
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")             # <<<<<<<<<<<<<<
  *         return OutputContainer(
  *             _cinit_sentinel, file, format, options,
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 308, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
 
-      /* "av/container/core.pyx":307
+      /* "av/container/core.pyx":409
  *         )
  *     if mode.startswith('w'):
  *         if stream_options:             # <<<<<<<<<<<<<<
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  *         return OutputContainer(
  */
     }
 
-    /* "av/container/core.pyx":309
+    /* "av/container/core.pyx":411
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  *         return OutputContainer(             # <<<<<<<<<<<<<<
  *             _cinit_sentinel, file, format, options,
  *             container_options, stream_options,
  */
     __Pyx_XDECREF(__pyx_r);
 
-    /* "av/container/core.pyx":313
- *             container_options, stream_options,
+    /* "av/container/core.pyx":416
  *             metadata_encoding, metadata_errors,
- *             buffer_size, open_timeout, read_timeout             # <<<<<<<<<<<<<<
+ *             buffer_size, open_timeout, read_timeout,
+ *             io_open             # <<<<<<<<<<<<<<
  *         )
  *     raise ValueError("mode must be 'r' or 'w'; got %r" % mode)
  */
-    __pyx_t_4 = PyTuple_New(11); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 309, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(12); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_2av_9container_4core__cinit_sentinel);
     __Pyx_GIVEREF(__pyx_v_2av_9container_4core__cinit_sentinel);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_2av_9container_4core__cinit_sentinel);
     __Pyx_INCREF(__pyx_v_file);
     __Pyx_GIVEREF(__pyx_v_file);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_file);
@@ -6231,53 +7259,56 @@
     PyTuple_SET_ITEM(__pyx_t_4, 8, __pyx_v_buffer_size);
     __Pyx_INCREF(__pyx_v_open_timeout);
     __Pyx_GIVEREF(__pyx_v_open_timeout);
     PyTuple_SET_ITEM(__pyx_t_4, 9, __pyx_v_open_timeout);
     __Pyx_INCREF(__pyx_v_read_timeout);
     __Pyx_GIVEREF(__pyx_v_read_timeout);
     PyTuple_SET_ITEM(__pyx_t_4, 10, __pyx_v_read_timeout);
+    __Pyx_INCREF(__pyx_v_io_open);
+    __Pyx_GIVEREF(__pyx_v_io_open);
+    PyTuple_SET_ITEM(__pyx_t_4, 11, __pyx_v_io_open);
 
-    /* "av/container/core.pyx":309
+    /* "av/container/core.pyx":411
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  *         return OutputContainer(             # <<<<<<<<<<<<<<
  *             _cinit_sentinel, file, format, options,
  *             container_options, stream_options,
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_6output_OutputContainer), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 309, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_9container_6output_OutputContainer), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/container/core.pyx":306
- *             buffer_size, open_timeout, read_timeout
+    /* "av/container/core.pyx":408
+ *             io_open
  *         )
  *     if mode.startswith('w'):             # <<<<<<<<<<<<<<
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")
  */
   }
 
-  /* "av/container/core.pyx":315
- *             buffer_size, open_timeout, read_timeout
+  /* "av/container/core.pyx":418
+ *             io_open
  *         )
  *     raise ValueError("mode must be 'r' or 'w'; got %r" % mode)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_mode_must_be_r_or_w_got_r, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_mode_must_be_r_or_w_got_r, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 315, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(0, 315, __pyx_L1_error)
+  __PYX_ERR(0, 418, __pyx_L1_error)
 
-  /* "av/container/core.pyx":251
+  /* "av/container/core.pyx":338
  * 
  * 
  * def open(file, mode=None, format=None, options=None,             # <<<<<<<<<<<<<<
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
  */
 
@@ -6309,14 +7340,16 @@
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_2av_9container_4core_Container *)o);
   p->__pyx_vtab = __pyx_vtabptr_2av_9container_4core_Container;
   p->name = Py_None; Py_INCREF(Py_None);
   p->metadata_encoding = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->metadata_errors = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->file = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)Py_None); Py_INCREF(Py_None);
+  p->io_open = Py_None; Py_INCREF(Py_None);
+  p->open_files = Py_None; Py_INCREF(Py_None);
   p->format = ((struct __pyx_obj_2av_6format_ContainerFormat *)Py_None); Py_INCREF(Py_None);
   p->options = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->container_options = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->stream_options = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->streams = ((struct __pyx_obj_2av_9container_7streams_StreamContainer *)Py_None); Py_INCREF(Py_None);
   p->metadata = ((PyObject*)Py_None); Py_INCREF(Py_None);
   p->open_timeout = Py_None; Py_INCREF(Py_None);
@@ -6344,14 +7377,16 @@
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->name);
   Py_CLEAR(p->metadata_encoding);
   Py_CLEAR(p->metadata_errors);
   Py_CLEAR(p->file);
+  Py_CLEAR(p->io_open);
+  Py_CLEAR(p->open_files);
   Py_CLEAR(p->format);
   Py_CLEAR(p->options);
   Py_CLEAR(p->container_options);
   Py_CLEAR(p->stream_options);
   Py_CLEAR(p->streams);
   Py_CLEAR(p->metadata);
   Py_CLEAR(p->open_timeout);
@@ -6364,14 +7399,20 @@
   struct __pyx_obj_2av_9container_4core_Container *p = (struct __pyx_obj_2av_9container_4core_Container *)o;
   if (p->name) {
     e = (*v)(p->name, a); if (e) return e;
   }
   if (p->file) {
     e = (*v)(((PyObject *)p->file), a); if (e) return e;
   }
+  if (p->io_open) {
+    e = (*v)(p->io_open, a); if (e) return e;
+  }
+  if (p->open_files) {
+    e = (*v)(p->open_files, a); if (e) return e;
+  }
   if (p->format) {
     e = (*v)(((PyObject *)p->format), a); if (e) return e;
   }
   if (p->options) {
     e = (*v)(p->options, a); if (e) return e;
   }
   if (p->container_options) {
@@ -6400,14 +7441,20 @@
   struct __pyx_obj_2av_9container_4core_Container *p = (struct __pyx_obj_2av_9container_4core_Container *)o;
   tmp = ((PyObject*)p->name);
   p->name = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->file);
   p->file = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->io_open);
+  p->io_open = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->open_files);
+  p->open_files = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
   tmp = ((PyObject*)p->format);
   p->format = ((struct __pyx_obj_2av_6format_ContainerFormat *)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->options);
   p->options = ((PyObject*)Py_None); Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->container_options);
@@ -6447,14 +7494,22 @@
   return __pyx_pw_2av_9container_4core_9Container_15metadata_errors_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_2av_9container_4core_9Container_file(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_9container_4core_9Container_4file_1__get__(o);
 }
 
+static PyObject *__pyx_getprop_2av_9container_4core_9Container_io_open(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_2av_9container_4core_9Container_7io_open_1__get__(o);
+}
+
+static PyObject *__pyx_getprop_2av_9container_4core_9Container_open_files(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_2av_9container_4core_9Container_10open_files_1__get__(o);
+}
+
 static PyObject *__pyx_getprop_2av_9container_4core_9Container_format(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_9container_4core_9Container_6format_1__get__(o);
 }
 
 static PyObject *__pyx_getprop_2av_9container_4core_9Container_options(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_9container_4core_9Container_7options_1__get__(o);
 }
@@ -6496,14 +7551,16 @@
 
 static struct PyGetSetDef __pyx_getsets_2av_9container_4core_Container[] = {
   {(char *)"writeable", __pyx_getprop_2av_9container_4core_9Container_writeable, 0, (char *)0, 0},
   {(char *)"name", __pyx_getprop_2av_9container_4core_9Container_name, 0, (char *)0, 0},
   {(char *)"metadata_encoding", __pyx_getprop_2av_9container_4core_9Container_metadata_encoding, 0, (char *)0, 0},
   {(char *)"metadata_errors", __pyx_getprop_2av_9container_4core_9Container_metadata_errors, 0, (char *)0, 0},
   {(char *)"file", __pyx_getprop_2av_9container_4core_9Container_file, 0, (char *)0, 0},
+  {(char *)"io_open", __pyx_getprop_2av_9container_4core_9Container_io_open, 0, (char *)0, 0},
+  {(char *)"open_files", __pyx_getprop_2av_9container_4core_9Container_open_files, 0, (char *)0, 0},
   {(char *)"format", __pyx_getprop_2av_9container_4core_9Container_format, 0, (char *)0, 0},
   {(char *)"options", __pyx_getprop_2av_9container_4core_9Container_options, 0, (char *)0, 0},
   {(char *)"container_options", __pyx_getprop_2av_9container_4core_9Container_container_options, 0, (char *)0, 0},
   {(char *)"stream_options", __pyx_getprop_2av_9container_4core_9Container_stream_options, 0, (char *)0, 0},
   {(char *)"streams", __pyx_getprop_2av_9container_4core_9Container_streams, 0, (char *)0, 0},
   {(char *)"metadata", __pyx_getprop_2av_9container_4core_9Container_metadata, 0, (char *)0, 0},
   {(char *)"open_timeout", __pyx_getprop_2av_9container_4core_9Container_open_timeout, 0, (char *)0, 0},
@@ -6905,15 +7962,15 @@
   {&__pyx_n_s_SORT_DTS, __pyx_k_SORT_DTS, sizeof(__pyx_k_SORT_DTS), 0, 0, 1, 1},
   {&__pyx_kp_s_Stop_muxing_when_the_shortest_st, __pyx_k_Stop_muxing_when_the_shortest_st, sizeof(__pyx_k_Stop_muxing_when_the_shortest_st), 0, 0, 1, 0},
   {&__pyx_kp_s_The_caller_has_supplied_a_custom, __pyx_k_The_caller_has_supplied_a_custom, sizeof(__pyx_k_The_caller_has_supplied_a_custom), 0, 0, 1, 0},
   {&__pyx_kp_s_Try_to_interleave_outputted_pack, __pyx_k_Try_to_interleave_outputted_pack, sizeof(__pyx_k_Try_to_interleave_outputted_pack), 0, 0, 1, 0},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_kp_s_When_muxing_try_to_avoid_writing, __pyx_k_When_muxing_try_to_avoid_writing, sizeof(__pyx_k_When_muxing_try_to_avoid_writing), 0, 0, 1, 0},
-  {&__pyx_kp_s__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 0, 1, 0},
+  {&__pyx_kp_s__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 0, 1, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_auto_bsf, __pyx_k_auto_bsf, sizeof(__pyx_k_auto_bsf), 0, 0, 1, 1},
   {&__pyx_n_s_av_container_core, __pyx_k_av_container_core, sizeof(__pyx_k_av_container_core), 0, 0, 1, 1},
   {&__pyx_kp_s_av_container_core_pyx, __pyx_k_av_container_core_pyx, sizeof(__pyx_k_av_container_core_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_av_dictionary, __pyx_k_av_dictionary, sizeof(__pyx_k_av_dictionary), 0, 0, 1, 1},
   {&__pyx_n_s_av_logging, __pyx_k_av_logging, sizeof(__pyx_k_av_logging), 0, 0, 1, 1},
   {&__pyx_kp_s_av_s_r, __pyx_k_av_s_r, sizeof(__pyx_k_av_s_r), 0, 0, 1, 0},
@@ -6944,14 +8001,15 @@
   {&__pyx_n_s_gen_pts, __pyx_k_gen_pts, sizeof(__pyx_k_gen_pts), 0, 0, 1, 1},
   {&__pyx_n_s_genexpr, __pyx_k_genexpr, sizeof(__pyx_k_genexpr), 0, 0, 1, 1},
   {&__pyx_n_s_get_flags, __pyx_k_get_flags, sizeof(__pyx_k_get_flags), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_ign_dts, __pyx_k_ign_dts, sizeof(__pyx_k_ign_dts), 0, 0, 1, 1},
   {&__pyx_n_s_ign_idx, __pyx_k_ign_idx, sizeof(__pyx_k_ign_idx), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_io_open, __pyx_k_io_open, sizeof(__pyx_k_io_open), 0, 0, 1, 1},
   {&__pyx_n_s_join, __pyx_k_join, sizeof(__pyx_k_join), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_metadata_encoding, __pyx_k_metadata_encoding, sizeof(__pyx_k_metadata_encoding), 0, 0, 1, 1},
   {&__pyx_n_s_metadata_errors, __pyx_k_metadata_errors, sizeof(__pyx_k_metadata_errors), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_kp_s_mode_must_be_r_or_w_got_r, __pyx_k_mode_must_be_r_or_w_got_r, sizeof(__pyx_k_mode_must_be_r_or_w_got_r), 0, 0, 1, 0},
   {&__pyx_n_s_monotonic, __pyx_k_monotonic, sizeof(__pyx_k_monotonic), 0, 0, 1, 1},
@@ -6962,15 +8020,15 @@
   {&__pyx_n_s_no_fill_in, __pyx_k_no_fill_in, sizeof(__pyx_k_no_fill_in), 0, 0, 1, 1},
   {&__pyx_n_s_no_parse, __pyx_k_no_parse, sizeof(__pyx_k_no_parse), 0, 0, 1, 1},
   {&__pyx_n_s_non_block, __pyx_k_non_block, sizeof(__pyx_k_non_block), 0, 0, 1, 1},
   {&__pyx_kp_s_none, __pyx_k_none, sizeof(__pyx_k_none), 0, 0, 1, 0},
   {&__pyx_n_s_object, __pyx_k_object, sizeof(__pyx_k_object), 0, 0, 1, 1},
   {&__pyx_n_s_open, __pyx_k_open, sizeof(__pyx_k_open), 0, 0, 1, 1},
   {&__pyx_kp_u_open_file_mode_r_kwargs_Main_ent, __pyx_k_open_file_mode_r_kwargs_Main_ent, sizeof(__pyx_k_open_file_mode_r_kwargs_Main_ent), 0, 1, 0, 0},
-  {&__pyx_kp_u_open_line_251, __pyx_k_open_line_251, sizeof(__pyx_k_open_line_251), 0, 1, 0, 0},
+  {&__pyx_kp_u_open_line_338, __pyx_k_open_line_338, sizeof(__pyx_k_open_line_338), 0, 1, 0, 0},
   {&__pyx_n_s_open_timeout, __pyx_k_open_timeout, sizeof(__pyx_k_open_timeout), 0, 0, 1, 1},
   {&__pyx_n_s_options, __pyx_k_options, sizeof(__pyx_k_options), 0, 0, 1, 1},
   {&__pyx_n_s_os, __pyx_k_os, sizeof(__pyx_k_os), 0, 0, 1, 1},
   {&__pyx_n_s_priv_opt, __pyx_k_priv_opt, sizeof(__pyx_k_priv_opt), 0, 0, 1, 1},
   {&__pyx_n_s_property, __pyx_k_property, sizeof(__pyx_k_property), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_r, __pyx_k_r, sizeof(__pyx_k_r), 0, 0, 1, 1},
@@ -6993,81 +8051,81 @@
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_timeout, __pyx_k_timeout, sizeof(__pyx_k_timeout), 0, 0, 1, 1},
   {&__pyx_kp_s_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 0, 1, 0},
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 25, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 45, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 139, __pyx_L1_error)
+  __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 26, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 46, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 219, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/container/core.pyx":45
+  /* "av/container/core.pyx":46
  *         if current_time < info.start_time:
  *             # Raise this when we get back to Python.
  *             stash_exception((RuntimeError, RuntimeError("Clock has been changed to before timeout start"), None))             # <<<<<<<<<<<<<<
  *             return 1
  * 
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Clock_has_been_changed_to_before); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_Clock_has_been_changed_to_before); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "av/container/core.pyx":103
+  /* "av/container/core.pyx":180
  * 
  *         if sentinel is not _cinit_sentinel:
  *             raise RuntimeError('cannot construct base Container')             # <<<<<<<<<<<<<<
  * 
  *         self.writeable = isinstance(self, OutputContainer)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_cannot_construct_base_Container); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 103, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_cannot_construct_base_Container); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 180, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "av/container/core.pyx":107
+  /* "av/container/core.pyx":184
  *         self.writeable = isinstance(self, OutputContainer)
  *         if not self.writeable and not isinstance(self, InputContainer):
  *             raise RuntimeError('Container cannot be directly extended.')             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(file_, str):
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Container_cannot_be_directly_ext); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 107, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Container_cannot_be_directly_ext); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 184, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "av/container/core.pyx":139
+  /* "av/container/core.pyx":219
  *             ofmt = self.format.optr if self.format else lib.av_guess_format(NULL, name, NULL)
  *             if ofmt == NULL:
  *                 raise ValueError("Could not determine output format")             # <<<<<<<<<<<<<<
  * 
  *             with nogil:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_Could_not_determine_output_forma); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 139, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Could_not_determine_output_forma); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "av/container/core.pyx":208
+  /* "av/container/core.pyx":295
  * 
  *     def dumps_format(self):
  *         with LogCapture() as logs:             # <<<<<<<<<<<<<<
  *             lib.av_dump_format(self.ptr, 0, "", isinstance(self, OutputContainer))
  *         return ''.join(log[2] for log in logs)
  */
-  __pyx_tuple__5 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 208, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_tuple__6 = PyTuple_Pack(3, Py_None, Py_None, Py_None); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 295, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__6);
+  __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
@@ -7080,36 +8138,36 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "av/container/core.pyx":308
+  /* "av/container/core.pyx":410
  *     if mode.startswith('w'):
  *         if stream_options:
  *             raise ValueError("Provide stream options via Container.add_stream(..., options={}).")             # <<<<<<<<<<<<<<
  *         return OutputContainer(
  *             _cinit_sentinel, file, format, options,
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Provide_stream_options_via_Conta); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_Provide_stream_options_via_Conta); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 410, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "av/container/core.pyx":251
+  /* "av/container/core.pyx":338
  * 
  * 
  * def open(file, mode=None, format=None, options=None,             # <<<<<<<<<<<<<<
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
  */
-  __pyx_tuple__10 = PyTuple_Pack(12, __pyx_n_s_file_2, __pyx_n_s_mode, __pyx_n_s_format, __pyx_n_s_options, __pyx_n_s_container_options, __pyx_n_s_stream_options, __pyx_n_s_metadata_encoding, __pyx_n_s_metadata_errors, __pyx_n_s_buffer_size, __pyx_n_s_timeout, __pyx_n_s_open_timeout, __pyx_n_s_read_timeout); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(13, __pyx_n_s_file_2, __pyx_n_s_mode, __pyx_n_s_format, __pyx_n_s_options, __pyx_n_s_container_options, __pyx_n_s_stream_options, __pyx_n_s_metadata_encoding, __pyx_n_s_metadata_errors, __pyx_n_s_buffer_size, __pyx_n_s_timeout, __pyx_n_s_io_open, __pyx_n_s_open_timeout, __pyx_n_s_read_timeout); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(10, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_av_container_core_pyx, __pyx_n_s_open, 251, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(11, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_av_container_core_pyx, __pyx_n_s_open, 338, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -7162,34 +8220,34 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_2av_9container_4core_Container = &__pyx_vtable_2av_9container_4core_Container;
   __pyx_vtable_2av_9container_4core_Container.err_check = (int (*)(struct __pyx_obj_2av_9container_4core_Container *, int))__pyx_f_2av_9container_4core_9Container_err_check;
   __pyx_vtable_2av_9container_4core_Container.set_timeout = (PyObject *(*)(struct __pyx_obj_2av_9container_4core_Container *, PyObject *))__pyx_f_2av_9container_4core_9Container_set_timeout;
   __pyx_vtable_2av_9container_4core_Container.start_timeout = (PyObject *(*)(struct __pyx_obj_2av_9container_4core_Container *))__pyx_f_2av_9container_4core_9Container_start_timeout;
-  if (PyType_Ready(&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_9container_4core_Container.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_9container_4core_Container.tp_dictoffset && __pyx_type_2av_9container_4core_Container.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_9container_4core_Container.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2av_9container_4core_Container.tp_dict, __pyx_vtabptr_2av_9container_4core_Container) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Container, (PyObject *)&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 95, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2av_9container_4core_Container.tp_dict, __pyx_vtabptr_2av_9container_4core_Container) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Container, (PyObject *)&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_9container_4core_Container) < 0) __PYX_ERR(0, 171, __pyx_L1_error)
   __pyx_ptype_2av_9container_4core_Container = &__pyx_type_2av_9container_4core_Container;
-  if (PyType_Ready(&__pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format) < 0) __PYX_ERR(0, 207, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format) < 0) __PYX_ERR(0, 294, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format.tp_dictoffset && __pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2av_9container_4core___pyx_scope_struct__dumps_format = &__pyx_type_2av_9container_4core___pyx_scope_struct__dumps_format;
-  if (PyType_Ready(&__pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr.tp_dictoffset && __pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   __pyx_ptype_2av_9container_4core___pyx_scope_struct_1_genexpr = &__pyx_type_2av_9container_4core___pyx_scope_struct_1_genexpr;
@@ -7204,18 +8262,18 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(3, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(3, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.bytesource"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_10bytesource_ByteSource = __Pyx_ImportType(__pyx_t_1, "av.bytesource", "ByteSource", sizeof(struct __pyx_obj_2av_10bytesource_ByteSource), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_10bytesource_ByteSource) __PYX_ERR(4, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.codec"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 4, __pyx_L1_error)
@@ -7311,14 +8369,19 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_ImportFunction(__pyx_t_1, "pyio_close_gil", (void (**)(void))&__pyx_f_2av_9container_4pyio_pyio_close_gil, "void (struct AVIOContext *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ImportFunction(__pyx_t_1, "pyio_close_custom_gil", (void (**)(void))&__pyx_f_2av_9container_4pyio_pyio_close_custom_gil, "void (struct AVIOContext *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.dictionary"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "wrap_dictionary", (void (**)(void))&__pyx_f_2av_10dictionary_wrap_dictionary, "struct __pyx_obj_2av_10dictionary__Dictionary *(AVDictionary *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.format"); if (!__pyx_t_1) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (__Pyx_ImportFunction(__pyx_t_1, "build_container_format", (void (**)(void))&__pyx_f_2av_6format_build_container_format, "struct __pyx_obj_2av_6format_ContainerFormat *(struct AVInputFormat *, struct AVOutputFormat *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7583,447 +8646,447 @@
  * cimport libav as lib
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_time, 0, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_time, __pyx_t_1) < 0) __PYX_ERR(0, 6, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/core.pyx":18
+  /* "av/container/core.pyx":19
  * from av.utils cimport avdict_to_dict
  * 
  * from av.dictionary import Dictionary             # <<<<<<<<<<<<<<
  * from av.logging import Capture as LogCapture
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_Dictionary);
   __Pyx_GIVEREF(__pyx_n_s_Dictionary);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_Dictionary);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_dictionary, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_av_dictionary, __pyx_t_1, -1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dictionary, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Dictionary, __pyx_t_1) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "av/container/core.pyx":19
+  /* "av/container/core.pyx":20
  * 
  * from av.dictionary import Dictionary
  * from av.logging import Capture as LogCapture             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Capture);
   __Pyx_GIVEREF(__pyx_n_s_Capture);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Capture);
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_av_logging, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_av_logging, __pyx_t_2, -1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Capture); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_1, __pyx_n_s_Capture); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LogCapture, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_LogCapture, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/core.pyx":25
+  /* "av/container/core.pyx":26
  * 
  * 
  * cdef object _cinit_sentinel = object()             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallNoArg(__pyx_builtin_object); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(__pyx_v_2av_9container_4core__cinit_sentinel);
   __Pyx_DECREF_SET(__pyx_v_2av_9container_4core__cinit_sentinel, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/container/core.pyx":29
+  /* "av/container/core.pyx":30
  * 
  * # We want to use the monotonic clock if it is available.
  * cdef object clock = getattr(time, 'monotonic', time.time)             # <<<<<<<<<<<<<<
  * 
  * cdef int interrupt_cb (void *p) nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_time); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_GetAttr3(__pyx_t_1, __pyx_n_s_monotonic, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetAttr3(__pyx_t_1, __pyx_n_s_monotonic, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_XGOTREF(__pyx_v_2av_9container_4core_clock);
   __Pyx_DECREF_SET(__pyx_v_2av_9container_4core_clock, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "av/container/core.pyx":54
+  /* "av/container/core.pyx":130
  * 
  * 
  * Flags = define_enum('Flags', __name__, (             # <<<<<<<<<<<<<<
  *     ('GENPTS', lib.AVFMT_FLAG_GENPTS,
  *         "Generate missing pts even if it requires parsing future frames."),
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "av/container/core.pyx":55
+  /* "av/container/core.pyx":131
  * 
  * Flags = define_enum('Flags', __name__, (
  *     ('GENPTS', lib.AVFMT_FLAG_GENPTS,             # <<<<<<<<<<<<<<
  *         "Generate missing pts even if it requires parsing future frames."),
  *     ('IGNIDX', lib.AVFMT_FLAG_IGNIDX,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_GENPTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_GENPTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_GENPTS);
   __Pyx_GIVEREF(__pyx_n_s_GENPTS);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_GENPTS);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Generate_missing_pts_even_if_it);
   __Pyx_GIVEREF(__pyx_kp_s_Generate_missing_pts_even_if_it);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_s_Generate_missing_pts_even_if_it);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":57
+  /* "av/container/core.pyx":133
  *     ('GENPTS', lib.AVFMT_FLAG_GENPTS,
  *         "Generate missing pts even if it requires parsing future frames."),
  *     ('IGNIDX', lib.AVFMT_FLAG_IGNIDX,             # <<<<<<<<<<<<<<
  *         "Ignore index."),
  *     ('NONBLOCK', lib.AVFMT_FLAG_NONBLOCK,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_IGNIDX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_IGNIDX); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 57, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(__pyx_n_s_IGNIDX);
   __Pyx_GIVEREF(__pyx_n_s_IGNIDX);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_n_s_IGNIDX);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Ignore_index);
   __Pyx_GIVEREF(__pyx_kp_s_Ignore_index);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_kp_s_Ignore_index);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":59
+  /* "av/container/core.pyx":135
  *     ('IGNIDX', lib.AVFMT_FLAG_IGNIDX,
  *         "Ignore index."),
  *     ('NONBLOCK', lib.AVFMT_FLAG_NONBLOCK,             # <<<<<<<<<<<<<<
  *         "Do not block when reading packets from input."),
  *     ('IGNDTS', lib.AVFMT_FLAG_IGNDTS,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NONBLOCK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NONBLOCK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 59, __pyx_L1_error)
+  __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_INCREF(__pyx_n_s_NONBLOCK);
   __Pyx_GIVEREF(__pyx_n_s_NONBLOCK);
   PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_n_s_NONBLOCK);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Do_not_block_when_reading_packet);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_block_when_reading_packet);
   PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_kp_s_Do_not_block_when_reading_packet);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":61
+  /* "av/container/core.pyx":137
  *     ('NONBLOCK', lib.AVFMT_FLAG_NONBLOCK,
  *         "Do not block when reading packets from input."),
  *     ('IGNDTS', lib.AVFMT_FLAG_IGNDTS,             # <<<<<<<<<<<<<<
  *         "Ignore DTS on frames that contain both DTS & PTS."),
  *     ('NOFILLIN', lib.AVFMT_FLAG_NOFILLIN,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_IGNDTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_IGNDTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 61, __pyx_L1_error)
+  __pyx_t_6 = PyTuple_New(3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 137, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_INCREF(__pyx_n_s_IGNDTS);
   __Pyx_GIVEREF(__pyx_n_s_IGNDTS);
   PyTuple_SET_ITEM(__pyx_t_6, 0, __pyx_n_s_IGNDTS);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_6, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Ignore_DTS_on_frames_that_contai);
   __Pyx_GIVEREF(__pyx_kp_s_Ignore_DTS_on_frames_that_contai);
   PyTuple_SET_ITEM(__pyx_t_6, 2, __pyx_kp_s_Ignore_DTS_on_frames_that_contai);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":63
+  /* "av/container/core.pyx":139
  *     ('IGNDTS', lib.AVFMT_FLAG_IGNDTS,
  *         "Ignore DTS on frames that contain both DTS & PTS."),
  *     ('NOFILLIN', lib.AVFMT_FLAG_NOFILLIN,             # <<<<<<<<<<<<<<
  *         "Do not infer any values from other values, just return what is stored in the container."),
  *     ('NOPARSE', lib.AVFMT_FLAG_NOPARSE,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOFILLIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOFILLIN); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 139, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_n_s_NOFILLIN);
   __Pyx_GIVEREF(__pyx_n_s_NOFILLIN);
   PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_n_s_NOFILLIN);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Do_not_infer_any_values_from_oth);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_infer_any_values_from_oth);
   PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_kp_s_Do_not_infer_any_values_from_oth);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":65
+  /* "av/container/core.pyx":141
  *     ('NOFILLIN', lib.AVFMT_FLAG_NOFILLIN,
  *         "Do not infer any values from other values, just return what is stored in the container."),
  *     ('NOPARSE', lib.AVFMT_FLAG_NOPARSE,             # <<<<<<<<<<<<<<
  *         """Do not use AVParsers, you also must set AVFMT_FLAG_NOFILLIN as the fillin code works on frames and no parsing -> no frames.
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOPARSE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOPARSE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_INCREF(__pyx_n_s_NOPARSE);
   __Pyx_GIVEREF(__pyx_n_s_NOPARSE);
   PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_n_s_NOPARSE);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Do_not_use_AVParsers_you_also_mu);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_use_AVParsers_you_also_mu);
   PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_kp_s_Do_not_use_AVParsers_you_also_mu);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":69
+  /* "av/container/core.pyx":145
  * 
  *         Also seeking to frames can not work if parsing to find frame boundaries has been disabled."""),
  *     ('NOBUFFER', lib.AVFMT_FLAG_NOBUFFER,             # <<<<<<<<<<<<<<
  *         "Do not buffer frames when possible."),
  *     ('CUSTOM_IO', lib.AVFMT_FLAG_CUSTOM_IO,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOBUFFER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_NOBUFFER); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_t_9 = PyTuple_New(3); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 145, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_INCREF(__pyx_n_s_NOBUFFER);
   __Pyx_GIVEREF(__pyx_n_s_NOBUFFER);
   PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_n_s_NOBUFFER);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_9, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Do_not_buffer_frames_when_possib);
   __Pyx_GIVEREF(__pyx_kp_s_Do_not_buffer_frames_when_possib);
   PyTuple_SET_ITEM(__pyx_t_9, 2, __pyx_kp_s_Do_not_buffer_frames_when_possib);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":71
+  /* "av/container/core.pyx":147
  *     ('NOBUFFER', lib.AVFMT_FLAG_NOBUFFER,
  *         "Do not buffer frames when possible."),
  *     ('CUSTOM_IO', lib.AVFMT_FLAG_CUSTOM_IO,             # <<<<<<<<<<<<<<
  *         "The caller has supplied a custom AVIOContext, don't avio_close() it."),
  *     ('DISCARD_CORRUPT', lib.AVFMT_FLAG_DISCARD_CORRUPT,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_CUSTOM_IO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_CUSTOM_IO); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 71, __pyx_L1_error)
+  __pyx_t_10 = PyTuple_New(3); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 147, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_10);
   __Pyx_INCREF(__pyx_n_s_CUSTOM_IO);
   __Pyx_GIVEREF(__pyx_n_s_CUSTOM_IO);
   PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_n_s_CUSTOM_IO);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_The_caller_has_supplied_a_custom);
   __Pyx_GIVEREF(__pyx_kp_s_The_caller_has_supplied_a_custom);
   PyTuple_SET_ITEM(__pyx_t_10, 2, __pyx_kp_s_The_caller_has_supplied_a_custom);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":73
+  /* "av/container/core.pyx":149
  *     ('CUSTOM_IO', lib.AVFMT_FLAG_CUSTOM_IO,
  *         "The caller has supplied a custom AVIOContext, don't avio_close() it."),
  *     ('DISCARD_CORRUPT', lib.AVFMT_FLAG_DISCARD_CORRUPT,             # <<<<<<<<<<<<<<
  *         "Discard frames marked corrupted."),
  *     ('FLUSH_PACKETS', lib.AVFMT_FLAG_FLUSH_PACKETS,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_DISCARD_CORRUPT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_DISCARD_CORRUPT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 73, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(3); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 149, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_INCREF(__pyx_n_s_DISCARD_CORRUPT);
   __Pyx_GIVEREF(__pyx_n_s_DISCARD_CORRUPT);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_n_s_DISCARD_CORRUPT);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Discard_frames_marked_corrupted);
   __Pyx_GIVEREF(__pyx_kp_s_Discard_frames_marked_corrupted);
   PyTuple_SET_ITEM(__pyx_t_11, 2, __pyx_kp_s_Discard_frames_marked_corrupted);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":75
+  /* "av/container/core.pyx":151
  *     ('DISCARD_CORRUPT', lib.AVFMT_FLAG_DISCARD_CORRUPT,
  *         "Discard frames marked corrupted."),
  *     ('FLUSH_PACKETS', lib.AVFMT_FLAG_FLUSH_PACKETS,             # <<<<<<<<<<<<<<
  *         "Flush the AVIOContext every packet."),
  *     ('BITEXACT', lib.AVFMT_FLAG_BITEXACT,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_FLUSH_PACKETS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_FLUSH_PACKETS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_12 = PyTuple_New(3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 151, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_12);
   __Pyx_INCREF(__pyx_n_s_FLUSH_PACKETS);
   __Pyx_GIVEREF(__pyx_n_s_FLUSH_PACKETS);
   PyTuple_SET_ITEM(__pyx_t_12, 0, __pyx_n_s_FLUSH_PACKETS);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_12, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Flush_the_AVIOContext_every_pack);
   __Pyx_GIVEREF(__pyx_kp_s_Flush_the_AVIOContext_every_pack);
   PyTuple_SET_ITEM(__pyx_t_12, 2, __pyx_kp_s_Flush_the_AVIOContext_every_pack);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":77
+  /* "av/container/core.pyx":153
  *     ('FLUSH_PACKETS', lib.AVFMT_FLAG_FLUSH_PACKETS,
  *         "Flush the AVIOContext every packet."),
  *     ('BITEXACT', lib.AVFMT_FLAG_BITEXACT,             # <<<<<<<<<<<<<<
  *         """When muxing, try to avoid writing any random/volatile data to the output.
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_BITEXACT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_BITEXACT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_13 = PyTuple_New(3); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 153, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
   __Pyx_INCREF(__pyx_n_s_BITEXACT);
   __Pyx_GIVEREF(__pyx_n_s_BITEXACT);
   PyTuple_SET_ITEM(__pyx_t_13, 0, __pyx_n_s_BITEXACT);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_13, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_When_muxing_try_to_avoid_writing);
   __Pyx_GIVEREF(__pyx_kp_s_When_muxing_try_to_avoid_writing);
   PyTuple_SET_ITEM(__pyx_t_13, 2, __pyx_kp_s_When_muxing_try_to_avoid_writing);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":82
+  /* "av/container/core.pyx":158
  *         This includes any random IDs, real-time timestamps/dates, muxer version, etc.
  *         This flag is mainly intended for testing."""),
  *     ('SORT_DTS', lib.AVFMT_FLAG_SORT_DTS,             # <<<<<<<<<<<<<<
  *         "Try to interleave outputted packets by dts (using this flag can slow demuxing down)."),
  *     ('PRIV_OPT', lib.AVFMT_FLAG_PRIV_OPT,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_SORT_DTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_SORT_DTS); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_14 = PyTuple_New(3); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 158, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_14);
   __Pyx_INCREF(__pyx_n_s_SORT_DTS);
   __Pyx_GIVEREF(__pyx_n_s_SORT_DTS);
   PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_n_s_SORT_DTS);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_14, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Try_to_interleave_outputted_pack);
   __Pyx_GIVEREF(__pyx_kp_s_Try_to_interleave_outputted_pack);
   PyTuple_SET_ITEM(__pyx_t_14, 2, __pyx_kp_s_Try_to_interleave_outputted_pack);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":84
+  /* "av/container/core.pyx":160
  *     ('SORT_DTS', lib.AVFMT_FLAG_SORT_DTS,
  *         "Try to interleave outputted packets by dts (using this flag can slow demuxing down)."),
  *     ('PRIV_OPT', lib.AVFMT_FLAG_PRIV_OPT,             # <<<<<<<<<<<<<<
  *         "Enable use of private options by delaying codec open (this could be made default once all code is converted)."),
  *     ('FAST_SEEK', lib.AVFMT_FLAG_FAST_SEEK,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_PRIV_OPT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_PRIV_OPT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 84, __pyx_L1_error)
+  __pyx_t_15 = PyTuple_New(3); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 160, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_INCREF(__pyx_n_s_PRIV_OPT);
   __Pyx_GIVEREF(__pyx_n_s_PRIV_OPT);
   PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_n_s_PRIV_OPT);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_15, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Enable_use_of_private_options_by);
   __Pyx_GIVEREF(__pyx_kp_s_Enable_use_of_private_options_by);
   PyTuple_SET_ITEM(__pyx_t_15, 2, __pyx_kp_s_Enable_use_of_private_options_by);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":86
+  /* "av/container/core.pyx":162
  *     ('PRIV_OPT', lib.AVFMT_FLAG_PRIV_OPT,
  *         "Enable use of private options by delaying codec open (this could be made default once all code is converted)."),
  *     ('FAST_SEEK', lib.AVFMT_FLAG_FAST_SEEK,             # <<<<<<<<<<<<<<
  *         "Enable fast, but inaccurate seeks for some formats."),
  *     ('SHORTEST', lib.AVFMT_FLAG_SHORTEST,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_FAST_SEEK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_FAST_SEEK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 86, __pyx_L1_error)
+  __pyx_t_16 = PyTuple_New(3); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 162, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_16);
   __Pyx_INCREF(__pyx_n_s_FAST_SEEK);
   __Pyx_GIVEREF(__pyx_n_s_FAST_SEEK);
   PyTuple_SET_ITEM(__pyx_t_16, 0, __pyx_n_s_FAST_SEEK);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_16, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Enable_fast_but_inaccurate_seeks);
   __Pyx_GIVEREF(__pyx_kp_s_Enable_fast_but_inaccurate_seeks);
   PyTuple_SET_ITEM(__pyx_t_16, 2, __pyx_kp_s_Enable_fast_but_inaccurate_seeks);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":88
+  /* "av/container/core.pyx":164
  *     ('FAST_SEEK', lib.AVFMT_FLAG_FAST_SEEK,
  *         "Enable fast, but inaccurate seeks for some formats."),
  *     ('SHORTEST', lib.AVFMT_FLAG_SHORTEST,             # <<<<<<<<<<<<<<
  *         "Stop muxing when the shortest stream stops."),
  *     ('AUTO_BSF', lib.AVFMT_FLAG_AUTO_BSF,
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_SHORTEST); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_SHORTEST); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 88, __pyx_L1_error)
+  __pyx_t_17 = PyTuple_New(3); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 164, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_INCREF(__pyx_n_s_SHORTEST);
   __Pyx_GIVEREF(__pyx_n_s_SHORTEST);
   PyTuple_SET_ITEM(__pyx_t_17, 0, __pyx_n_s_SHORTEST);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Stop_muxing_when_the_shortest_st);
   __Pyx_GIVEREF(__pyx_kp_s_Stop_muxing_when_the_shortest_st);
   PyTuple_SET_ITEM(__pyx_t_17, 2, __pyx_kp_s_Stop_muxing_when_the_shortest_st);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":90
+  /* "av/container/core.pyx":166
  *     ('SHORTEST', lib.AVFMT_FLAG_SHORTEST,
  *         "Stop muxing when the shortest stream stops."),
  *     ('AUTO_BSF', lib.AVFMT_FLAG_AUTO_BSF,             # <<<<<<<<<<<<<<
  *         "Add bitstream filters as requested by the muxer."),
  * ), is_flags=True)
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_AUTO_BSF); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(AVFMT_FLAG_AUTO_BSF); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_18 = PyTuple_New(3); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 166, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_n_s_AUTO_BSF);
   __Pyx_GIVEREF(__pyx_n_s_AUTO_BSF);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_n_s_AUTO_BSF);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_3);
   __Pyx_INCREF(__pyx_kp_s_Add_bitstream_filters_as_request);
   __Pyx_GIVEREF(__pyx_kp_s_Add_bitstream_filters_as_request);
   PyTuple_SET_ITEM(__pyx_t_18, 2, __pyx_kp_s_Add_bitstream_filters_as_request);
   __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":55
+  /* "av/container/core.pyx":131
  * 
  * Flags = define_enum('Flags', __name__, (
  *     ('GENPTS', lib.AVFMT_FLAG_GENPTS,             # <<<<<<<<<<<<<<
  *         "Generate missing pts even if it requires parsing future frames."),
  *     ('IGNIDX', lib.AVFMT_FLAG_IGNIDX,
  */
-  __pyx_t_3 = PyTuple_New(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 55, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(16); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 131, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_5);
@@ -8066,61 +9129,61 @@
   __pyx_t_13 = 0;
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
   __pyx_t_16 = 0;
   __pyx_t_17 = 0;
   __pyx_t_18 = 0;
 
-  /* "av/container/core.pyx":54
+  /* "av/container/core.pyx":130
  * 
  * 
  * Flags = define_enum('Flags', __name__, (             # <<<<<<<<<<<<<<
  *     ('GENPTS', lib.AVFMT_FLAG_GENPTS,
  *         "Generate missing pts even if it requires parsing future frames."),
  */
   __pyx_t_19.__pyx_n = 1;
   __pyx_t_19.is_flags = 1;
-  __pyx_t_18 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags, __pyx_t_2, __pyx_t_3, 0, &__pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 54, __pyx_L1_error)
+  __pyx_t_18 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Flags, __pyx_t_2, __pyx_t_3, 0, &__pyx_t_19); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags, __pyx_t_18) < 0) __PYX_ERR(0, 54, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Flags, __pyx_t_18) < 0) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
-  /* "av/container/core.pyx":227
+  /* "av/container/core.pyx":314
  *         self.ptr.flags = value
  * 
  *     flags = Flags.property(             # <<<<<<<<<<<<<<
  *         _get_flags,
  *         _set_flags,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "av/container/core.pyx":228
+  /* "av/container/core.pyx":315
  * 
  *     flags = Flags.property(
  *         _get_flags,             # <<<<<<<<<<<<<<
  *         _set_flags,
  *         """Flags property of :class:`.Flags`"""
  */
-  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_get_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 228, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_3, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_get_flags); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 315, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
 
-  /* "av/container/core.pyx":229
+  /* "av/container/core.pyx":316
  *     flags = Flags.property(
  *         _get_flags,
  *         _set_flags,             # <<<<<<<<<<<<<<
  *         """Flags property of :class:`.Flags`"""
  *     )
  */
-  __Pyx_GetNameInClass(__pyx_t_17, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_set_flags); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 229, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_17, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_set_flags); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 316, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __pyx_t_16 = NULL;
   __pyx_t_20 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_16 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_16)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
@@ -8129,571 +9192,571 @@
       __Pyx_DECREF_SET(__pyx_t_2, function);
       __pyx_t_20 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_16, __pyx_t_3, __pyx_t_17, __pyx_kp_s_Flags_property_of_class_Flags};
-    __pyx_t_18 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_20, 3+__pyx_t_20); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_20, 3+__pyx_t_20); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_2)) {
     PyObject *__pyx_temp[4] = {__pyx_t_16, __pyx_t_3, __pyx_t_17, __pyx_kp_s_Flags_property_of_class_Flags};
-    __pyx_t_18 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_20, 3+__pyx_t_20); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyCFunction_FastCall(__pyx_t_2, __pyx_temp+1-__pyx_t_20, 3+__pyx_t_20); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_16); __pyx_t_16 = 0;
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
   } else
   #endif
   {
-    __pyx_t_15 = PyTuple_New(3+__pyx_t_20); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_15 = PyTuple_New(3+__pyx_t_20); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_15);
     if (__pyx_t_16) {
       __Pyx_GIVEREF(__pyx_t_16); PyTuple_SET_ITEM(__pyx_t_15, 0, __pyx_t_16); __pyx_t_16 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_15, 0+__pyx_t_20, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_17);
     PyTuple_SET_ITEM(__pyx_t_15, 1+__pyx_t_20, __pyx_t_17);
     __Pyx_INCREF(__pyx_kp_s_Flags_property_of_class_Flags);
     __Pyx_GIVEREF(__pyx_kp_s_Flags_property_of_class_Flags);
     PyTuple_SET_ITEM(__pyx_t_15, 2+__pyx_t_20, __pyx_kp_s_Flags_property_of_class_Flags);
     __pyx_t_3 = 0;
     __pyx_t_17 = 0;
-    __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_15, NULL); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __pyx_t_18 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_15, NULL); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 314, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_18);
     __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_flags, __pyx_t_18) < 0) __PYX_ERR(0, 227, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_flags, __pyx_t_18) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":233
+  /* "av/container/core.pyx":320
  *     )
  * 
  *     gen_pts = flags.flag_property('GENPTS')             # <<<<<<<<<<<<<<
  *     ign_idx = flags.flag_property('IGNIDX')
  *     non_block = flags.flag_property('NONBLOCK')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_GENPTS) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_GENPTS);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_gen_pts, __pyx_t_18) < 0) __PYX_ERR(0, 233, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_gen_pts, __pyx_t_18) < 0) __PYX_ERR(0, 320, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":234
+  /* "av/container/core.pyx":321
  * 
  *     gen_pts = flags.flag_property('GENPTS')
  *     ign_idx = flags.flag_property('IGNIDX')             # <<<<<<<<<<<<<<
  *     non_block = flags.flag_property('NONBLOCK')
  *     ign_dts = flags.flag_property('IGNDTS')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_IGNIDX) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_IGNIDX);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_ign_idx, __pyx_t_18) < 0) __PYX_ERR(0, 234, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_ign_idx, __pyx_t_18) < 0) __PYX_ERR(0, 321, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":235
+  /* "av/container/core.pyx":322
  *     gen_pts = flags.flag_property('GENPTS')
  *     ign_idx = flags.flag_property('IGNIDX')
  *     non_block = flags.flag_property('NONBLOCK')             # <<<<<<<<<<<<<<
  *     ign_dts = flags.flag_property('IGNDTS')
  *     no_fill_in = flags.flag_property('NOFILLIN')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 235, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_NONBLOCK) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_NONBLOCK);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_non_block, __pyx_t_18) < 0) __PYX_ERR(0, 235, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_non_block, __pyx_t_18) < 0) __PYX_ERR(0, 322, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":236
+  /* "av/container/core.pyx":323
  *     ign_idx = flags.flag_property('IGNIDX')
  *     non_block = flags.flag_property('NONBLOCK')
  *     ign_dts = flags.flag_property('IGNDTS')             # <<<<<<<<<<<<<<
  *     no_fill_in = flags.flag_property('NOFILLIN')
  *     no_parse = flags.flag_property('NOPARSE')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_IGNDTS) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_IGNDTS);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_ign_dts, __pyx_t_18) < 0) __PYX_ERR(0, 236, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_ign_dts, __pyx_t_18) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":237
+  /* "av/container/core.pyx":324
  *     non_block = flags.flag_property('NONBLOCK')
  *     ign_dts = flags.flag_property('IGNDTS')
  *     no_fill_in = flags.flag_property('NOFILLIN')             # <<<<<<<<<<<<<<
  *     no_parse = flags.flag_property('NOPARSE')
  *     no_buffer = flags.flag_property('NOBUFFER')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_NOFILLIN) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_NOFILLIN);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_fill_in, __pyx_t_18) < 0) __PYX_ERR(0, 237, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_fill_in, __pyx_t_18) < 0) __PYX_ERR(0, 324, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":238
+  /* "av/container/core.pyx":325
  *     ign_dts = flags.flag_property('IGNDTS')
  *     no_fill_in = flags.flag_property('NOFILLIN')
  *     no_parse = flags.flag_property('NOPARSE')             # <<<<<<<<<<<<<<
  *     no_buffer = flags.flag_property('NOBUFFER')
  *     custom_io = flags.flag_property('CUSTOM_IO')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_NOPARSE) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_NOPARSE);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_parse, __pyx_t_18) < 0) __PYX_ERR(0, 238, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_parse, __pyx_t_18) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":239
+  /* "av/container/core.pyx":326
  *     no_fill_in = flags.flag_property('NOFILLIN')
  *     no_parse = flags.flag_property('NOPARSE')
  *     no_buffer = flags.flag_property('NOBUFFER')             # <<<<<<<<<<<<<<
  *     custom_io = flags.flag_property('CUSTOM_IO')
  *     discard_corrupt = flags.flag_property('DISCARD_CORRUPT')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 239, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_NOBUFFER) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_NOBUFFER);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_buffer, __pyx_t_18) < 0) __PYX_ERR(0, 239, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_no_buffer, __pyx_t_18) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":240
+  /* "av/container/core.pyx":327
  *     no_parse = flags.flag_property('NOPARSE')
  *     no_buffer = flags.flag_property('NOBUFFER')
  *     custom_io = flags.flag_property('CUSTOM_IO')             # <<<<<<<<<<<<<<
  *     discard_corrupt = flags.flag_property('DISCARD_CORRUPT')
  *     flush_packets = flags.flag_property('FLUSH_PACKETS')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_CUSTOM_IO) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_CUSTOM_IO);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 240, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_custom_io, __pyx_t_18) < 0) __PYX_ERR(0, 240, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_custom_io, __pyx_t_18) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":241
+  /* "av/container/core.pyx":328
  *     no_buffer = flags.flag_property('NOBUFFER')
  *     custom_io = flags.flag_property('CUSTOM_IO')
  *     discard_corrupt = flags.flag_property('DISCARD_CORRUPT')             # <<<<<<<<<<<<<<
  *     flush_packets = flags.flag_property('FLUSH_PACKETS')
  *     bit_exact = flags.flag_property('BITEXACT')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 241, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_DISCARD_CORRUPT) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_DISCARD_CORRUPT);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_discard_corrupt, __pyx_t_18) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_discard_corrupt, __pyx_t_18) < 0) __PYX_ERR(0, 328, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":242
+  /* "av/container/core.pyx":329
  *     custom_io = flags.flag_property('CUSTOM_IO')
  *     discard_corrupt = flags.flag_property('DISCARD_CORRUPT')
  *     flush_packets = flags.flag_property('FLUSH_PACKETS')             # <<<<<<<<<<<<<<
  *     bit_exact = flags.flag_property('BITEXACT')
  *     sort_dts = flags.flag_property('SORT_DTS')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_FLUSH_PACKETS) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_FLUSH_PACKETS);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_flush_packets, __pyx_t_18) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_flush_packets, __pyx_t_18) < 0) __PYX_ERR(0, 329, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":243
+  /* "av/container/core.pyx":330
  *     discard_corrupt = flags.flag_property('DISCARD_CORRUPT')
  *     flush_packets = flags.flag_property('FLUSH_PACKETS')
  *     bit_exact = flags.flag_property('BITEXACT')             # <<<<<<<<<<<<<<
  *     sort_dts = flags.flag_property('SORT_DTS')
  *     priv_opt = flags.flag_property('PRIV_OPT')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_BITEXACT) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_BITEXACT);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_bit_exact, __pyx_t_18) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_bit_exact, __pyx_t_18) < 0) __PYX_ERR(0, 330, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":244
+  /* "av/container/core.pyx":331
  *     flush_packets = flags.flag_property('FLUSH_PACKETS')
  *     bit_exact = flags.flag_property('BITEXACT')
  *     sort_dts = flags.flag_property('SORT_DTS')             # <<<<<<<<<<<<<<
  *     priv_opt = flags.flag_property('PRIV_OPT')
  *     fast_seek = flags.flag_property('FAST_SEEK')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_SORT_DTS) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_SORT_DTS);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_sort_dts, __pyx_t_18) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_sort_dts, __pyx_t_18) < 0) __PYX_ERR(0, 331, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":245
+  /* "av/container/core.pyx":332
  *     bit_exact = flags.flag_property('BITEXACT')
  *     sort_dts = flags.flag_property('SORT_DTS')
  *     priv_opt = flags.flag_property('PRIV_OPT')             # <<<<<<<<<<<<<<
  *     fast_seek = flags.flag_property('FAST_SEEK')
  *     shortest = flags.flag_property('SHORTEST')
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_PRIV_OPT) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_PRIV_OPT);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_priv_opt, __pyx_t_18) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_priv_opt, __pyx_t_18) < 0) __PYX_ERR(0, 332, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":246
+  /* "av/container/core.pyx":333
  *     sort_dts = flags.flag_property('SORT_DTS')
  *     priv_opt = flags.flag_property('PRIV_OPT')
  *     fast_seek = flags.flag_property('FAST_SEEK')             # <<<<<<<<<<<<<<
  *     shortest = flags.flag_property('SHORTEST')
  *     auto_bsf = flags.flag_property('AUTO_BSF')
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_FAST_SEEK) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_FAST_SEEK);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_fast_seek, __pyx_t_18) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_fast_seek, __pyx_t_18) < 0) __PYX_ERR(0, 333, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":247
+  /* "av/container/core.pyx":334
  *     priv_opt = flags.flag_property('PRIV_OPT')
  *     fast_seek = flags.flag_property('FAST_SEEK')
  *     shortest = flags.flag_property('SHORTEST')             # <<<<<<<<<<<<<<
  *     auto_bsf = flags.flag_property('AUTO_BSF')
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_2, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_15 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_15))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_15);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_15);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_15, function);
     }
   }
   __pyx_t_18 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_15, __pyx_t_2, __pyx_n_s_SHORTEST) : __Pyx_PyObject_CallOneArg(__pyx_t_15, __pyx_n_s_SHORTEST);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 247, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_shortest, __pyx_t_18) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_shortest, __pyx_t_18) < 0) __PYX_ERR(0, 334, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":248
+  /* "av/container/core.pyx":335
  *     fast_seek = flags.flag_property('FAST_SEEK')
  *     shortest = flags.flag_property('SHORTEST')
  *     auto_bsf = flags.flag_property('AUTO_BSF')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_15, (PyObject *)__pyx_ptype_2av_9container_4core_Container, __pyx_n_s_flags); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_15);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_15, __pyx_n_s_flag_property); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_18 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_15, __pyx_n_s_AUTO_BSF) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_n_s_AUTO_BSF);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
-  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 248, __pyx_L1_error)
+  if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_auto_bsf, __pyx_t_18) < 0) __PYX_ERR(0, 248, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_2av_9container_4core_Container->tp_dict, __pyx_n_s_auto_bsf, __pyx_t_18) < 0) __PYX_ERR(0, 335, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
   PyType_Modified(__pyx_ptype_2av_9container_4core_Container);
 
-  /* "av/container/core.pyx":251
+  /* "av/container/core.pyx":338
  * 
  * 
  * def open(file, mode=None, format=None, options=None,             # <<<<<<<<<<<<<<
  *          container_options=None, stream_options=None,
  *          metadata_encoding='utf-8', metadata_errors='strict',
  */
-  __pyx_t_18 = PyCFunction_NewEx(&__pyx_mdef_2av_9container_4core_1open, NULL, __pyx_n_s_av_container_core); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_18 = PyCFunction_NewEx(&__pyx_mdef_2av_9container_4core_1open, NULL, __pyx_n_s_av_container_core); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_18) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_open, __pyx_t_18) < 0) __PYX_ERR(0, 338, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
   /* "av/container/core.pyx":1
  * from cython.operator cimport dereference             # <<<<<<<<<<<<<<
  * from libc.stdint cimport int64_t
  * from libc.stdlib cimport free, malloc
  */
   __pyx_t_18 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
-  if (PyDict_SetItem(__pyx_t_18, __pyx_kp_u_open_line_251, __pyx_kp_u_open_file_mode_r_kwargs_Main_ent) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_18, __pyx_kp_u_open_line_338, __pyx_kp_u_open_file_mode_r_kwargs_Main_ent) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_18) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
@@ -9086,14 +10149,251 @@
     }
 #ifdef WITH_THREAD
     if (nogil)
         PyGILState_Release(state);
 #endif
 }
 
+/* SetItemInt */
+static int __Pyx_SetItemInt_Generic(PyObject *o, PyObject *j, PyObject *v) {
+    int r;
+    if (!j) return -1;
+    r = PyObject_SetItem(o, j, v);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE int __Pyx_SetItemInt_Fast(PyObject *o, Py_ssize_t i, PyObject *v, int is_list,
+                                               CYTHON_NCP_UNUSED int wraparound, CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = (!wraparound) ? i : ((likely(i >= 0)) ? i : i + PyList_GET_SIZE(o));
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o)))) {
+            PyObject* old = PyList_GET_ITEM(o, n);
+            Py_INCREF(v);
+            PyList_SET_ITEM(o, n, v);
+            Py_DECREF(old);
+            return 1;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_ass_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return -1;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_ass_item(o, i, v);
+        }
+    }
+#else
+#if CYTHON_COMPILING_IN_PYPY
+    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
+#else
+    if (is_list || PySequence_Check(o))
+#endif
+    {
+        return PySequence_SetItem(o, i, v);
+    }
+#endif
+    return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
+}
+
+/* GetTopmostException */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem *
+__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
+{
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
+           exc_info->previous_item != NULL)
+    {
+        exc_info = exc_info->previous_item;
+    }
+    return exc_info;
+}
+#endif
+
+/* SaveResetException */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
+    *type = exc_info->exc_type;
+    *value = exc_info->exc_value;
+    *tb = exc_info->exc_traceback;
+    #else
+    *type = tstate->exc_type;
+    *value = tstate->exc_value;
+    *tb = tstate->exc_traceback;
+    #endif
+    Py_XINCREF(*type);
+    Py_XINCREF(*value);
+    Py_XINCREF(*tb);
+}
+static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    #if CYTHON_USE_EXC_INFO_STACK
+    _PyErr_StackItem *exc_info = tstate->exc_info;
+    tmp_type = exc_info->exc_type;
+    tmp_value = exc_info->exc_value;
+    tmp_tb = exc_info->exc_traceback;
+    exc_info->exc_type = type;
+    exc_info->exc_value = value;
+    exc_info->exc_traceback = tb;
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = type;
+    tstate->exc_value = value;
+    tstate->exc_traceback = tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+#endif
+
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
+    return 0;
+}
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* GetException */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb)
+#else
+static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb)
+#endif
+{
+    PyObject *local_type, *local_value, *local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    local_type = tstate->curexc_type;
+    local_value = tstate->curexc_value;
+    local_tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+#else
+    PyErr_Fetch(&local_type, &local_value, &local_tb);
+#endif
+    PyErr_NormalizeException(&local_type, &local_value, &local_tb);
+#if CYTHON_FAST_THREAD_STATE
+    if (unlikely(tstate->curexc_type))
+#else
+    if (unlikely(PyErr_Occurred()))
+#endif
+        goto bad;
+    #if PY_MAJOR_VERSION >= 3
+    if (local_tb) {
+        if (unlikely(PyException_SetTraceback(local_value, local_tb) < 0))
+            goto bad;
+    }
+    #endif
+    Py_XINCREF(local_tb);
+    Py_XINCREF(local_type);
+    Py_XINCREF(local_value);
+    *type = local_type;
+    *value = local_value;
+    *tb = local_tb;
+#if CYTHON_FAST_THREAD_STATE
+    #if CYTHON_USE_EXC_INFO_STACK
+    {
+        _PyErr_StackItem *exc_info = tstate->exc_info;
+        tmp_type = exc_info->exc_type;
+        tmp_value = exc_info->exc_value;
+        tmp_tb = exc_info->exc_traceback;
+        exc_info->exc_type = local_type;
+        exc_info->exc_value = local_value;
+        exc_info->exc_traceback = local_tb;
+    }
+    #else
+    tmp_type = tstate->exc_type;
+    tmp_value = tstate->exc_value;
+    tmp_tb = tstate->exc_traceback;
+    tstate->exc_type = local_type;
+    tstate->exc_value = local_value;
+    tstate->exc_traceback = local_tb;
+    #endif
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+#else
+    PyErr_SetExcInfo(local_type, local_value, local_tb);
+#endif
+    return 0;
+bad:
+    *type = 0;
+    *value = 0;
+    *tb = 0;
+    Py_XDECREF(local_type);
+    Py_XDECREF(local_value);
+    Py_XDECREF(local_tb);
+    return -1;
+}
+
+/* DelItemInt */
+static int __Pyx_DelItem_Generic(PyObject *o, PyObject *j) {
+    int r;
+    if (!j) return -1;
+    r = PyObject_DelItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE int __Pyx_DelItemInt_Fast(PyObject *o, Py_ssize_t i,
+                                               CYTHON_UNUSED int is_list, CYTHON_NCP_UNUSED int wraparound) {
+#if !CYTHON_USE_TYPE_SLOTS
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_DelItem(o, i);
+    }
+#else
+    PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+    if (likely(m && m->sq_ass_item)) {
+        if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+            Py_ssize_t l = m->sq_length(o);
+            if (likely(l >= 0)) {
+                i += l;
+            } else {
+                if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                    return -1;
+                PyErr_Clear();
+            }
+        }
+        return m->sq_ass_item(o, i, (PyObject *)NULL);
+    }
+#endif
+    return __Pyx_DelItem_Generic(o, PyInt_FromSsize_t(i));
+}
+
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -9387,39 +10687,14 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    PyObject *exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-    if (unlikely(PyTuple_Check(err)))
-        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-}
-#endif
-
 /* GetAttr */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
 #if CYTHON_USE_TYPE_SLOTS
 #if PY_MAJOR_VERSION >= 3
     if (likely(PyUnicode_Check(n)))
 #else
     if (likely(PyString_Check(n)))
@@ -10270,47 +11545,47 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int64_t(int64_t value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
+    const int64_t neg_one = (int64_t) -1, const_zero = (int64_t) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
 #endif
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
+        if (sizeof(int64_t) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
+        } else if (sizeof(int64_t) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(int64_t) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(long) <= sizeof(long)) {
+        if (sizeof(int64_t) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(int64_t) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
+        return _PyLong_FromByteArray(bytes, sizeof(int64_t),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -10503,14 +11778,52 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const long neg_one = (long) -1, const_zero = (long) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -10838,70 +12151,14 @@
     return cached_type;
 bad:
     Py_XDECREF(cached_type);
     cached_type = NULL;
     goto done;
 }
 
-/* GetTopmostException */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem *
-__Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
-{
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
-           exc_info->previous_item != NULL)
-    {
-        exc_info = exc_info->previous_item;
-    }
-    return exc_info;
-}
-#endif
-
-/* SaveResetException */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = __Pyx_PyErr_GetTopmostException(tstate);
-    *type = exc_info->exc_type;
-    *value = exc_info->exc_value;
-    *tb = exc_info->exc_traceback;
-    #else
-    *type = tstate->exc_type;
-    *value = tstate->exc_value;
-    *tb = tstate->exc_traceback;
-    #endif
-    Py_XINCREF(*type);
-    Py_XINCREF(*value);
-    Py_XINCREF(*tb);
-}
-static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    #if CYTHON_USE_EXC_INFO_STACK
-    _PyErr_StackItem *exc_info = tstate->exc_info;
-    tmp_type = exc_info->exc_type;
-    tmp_value = exc_info->exc_value;
-    tmp_tb = exc_info->exc_traceback;
-    exc_info->exc_type = type;
-    exc_info->exc_value = value;
-    exc_info->exc_traceback = tb;
-    #else
-    tmp_type = tstate->exc_type;
-    tmp_value = tstate->exc_value;
-    tmp_tb = tstate->exc_traceback;
-    tstate->exc_type = type;
-    tstate->exc_value = value;
-    tstate->exc_traceback = tb;
-    #endif
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-#endif
-
 /* SwapException */
 #if CYTHON_FAST_THREAD_STATE
 static CYTHON_INLINE void __Pyx__ExceptionSwap(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
     PyObject *tmp_type, *tmp_value, *tmp_tb;
     #if CYTHON_USE_EXC_INFO_STACK
     _PyErr_StackItem *exc_info = tstate->exc_info;
     tmp_type = exc_info->exc_type;
```

### Comparing `av-9.1.1/src/av/container/input.c` & `av-9.2.0/src/av/container/input.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1151,28 +1159,29 @@
  */
 struct __pyx_opt_args_2av_5error_make_error {
   int __pyx_n;
   PyObject *filename;
   PyObject *log;
 };
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1384,15 +1393,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -5858,18 +5870,18 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(2, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.bytesource"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_10bytesource_ByteSource = __Pyx_ImportType(__pyx_t_1, "av.bytesource", "ByteSource", sizeof(struct __pyx_obj_2av_10bytesource_ByteSource), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_10bytesource_ByteSource) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.codec"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 4, __pyx_L1_error)
```

### Comparing `av-9.1.1/src/av/container/output.c` & `av-9.2.0/src/av/container/output.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1147,28 +1155,29 @@
  */
 struct __pyx_opt_args_2av_5error_make_error {
   int __pyx_n;
   PyObject *filename;
   PyObject *log;
 };
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1380,15 +1389,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -1404,14 +1416,15 @@
  * 
  *     cdef bint _started
  */
 struct __pyx_obj_2av_9container_6output_OutputContainer {
   struct __pyx_obj_2av_9container_4core_Container __pyx_base;
   int _started;
   int _done;
+  struct AVPacket *packet_ptr;
 };
 
 
 
 /* "av/codec/codec.pxd":4
  * 
  * 
@@ -2535,39 +2548,83 @@
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "av/container/output.pyx":35
  * 
  *     def __cinit__(self, *args, **kwargs):
  *         self.streams = StreamContainer()             # <<<<<<<<<<<<<<
  *         self.metadata = {}
- * 
+ *         with nogil:
  */
   __pyx_t_1 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2av_9container_7streams_StreamContainer)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 35, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base.streams);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->__pyx_base.streams));
   __pyx_v_self->__pyx_base.streams = ((struct __pyx_obj_2av_9container_7streams_StreamContainer *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "av/container/output.pyx":36
  *     def __cinit__(self, *args, **kwargs):
  *         self.streams = StreamContainer()
  *         self.metadata = {}             # <<<<<<<<<<<<<<
- * 
- *     def __dealloc__(self):
+ *         with nogil:
+ *             self.packet_ptr = lib.av_packet_alloc()
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base.metadata);
   __Pyx_DECREF(__pyx_v_self->__pyx_base.metadata);
   __pyx_v_self->__pyx_base.metadata = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
+  /* "av/container/output.pyx":37
+ *         self.streams = StreamContainer()
+ *         self.metadata = {}
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             self.packet_ptr = lib.av_packet_alloc()
+ * 
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "av/container/output.pyx":38
+ *         self.metadata = {}
+ *         with nogil:
+ *             self.packet_ptr = lib.av_packet_alloc()             # <<<<<<<<<<<<<<
+ * 
+ *     def __dealloc__(self):
+ */
+        __pyx_v_self->packet_ptr = av_packet_alloc();
+      }
+
+      /* "av/container/output.pyx":37
+ *         self.streams = StreamContainer()
+ *         self.metadata = {}
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             self.packet_ptr = lib.av_packet_alloc()
+ * 
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
   /* "av/container/output.pyx":34
  * cdef class OutputContainer(Container):
  * 
  *     def __cinit__(self, *args, **kwargs):             # <<<<<<<<<<<<<<
  *         self.streams = StreamContainer()
  *         self.metadata = {}
  */
@@ -2580,20 +2637,20 @@
   __Pyx_AddTraceback("av.container.output.OutputContainer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/output.pyx":38
- *         self.metadata = {}
+/* "av/container/output.pyx":40
+ *             self.packet_ptr = lib.av_packet_alloc()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         close_output(self)
- * 
+ *         with nogil:
  */
 
 /* Python wrapper */
 static void __pyx_pw_2av_9container_6output_15OutputContainer_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
 static void __pyx_pw_2av_9container_6output_15OutputContainer_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
@@ -2607,44 +2664,88 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "av/container/output.pyx":39
+  /* "av/container/output.pyx":41
  * 
  *     def __dealloc__(self):
  *         close_output(self)             # <<<<<<<<<<<<<<
- * 
- *     def add_stream(self, codec_name=None, object rate=None, Stream template=None, options=None, **kwargs):
+ *         with nogil:
+ *             lib.av_packet_free(&self.packet_ptr)
  */
-  __pyx_t_1 = __pyx_f_2av_9container_6output_close_output(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 39, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2av_9container_6output_close_output(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":38
- *         self.metadata = {}
+  /* "av/container/output.pyx":42
+ *     def __dealloc__(self):
+ *         close_output(self)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             lib.av_packet_free(&self.packet_ptr)
  * 
- *     def __dealloc__(self):             # <<<<<<<<<<<<<<
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "av/container/output.pyx":43
  *         close_output(self)
+ *         with nogil:
+ *             lib.av_packet_free(&self.packet_ptr)             # <<<<<<<<<<<<<<
  * 
+ *     def add_stream(self, codec_name=None, object rate=None, Stream template=None, options=None, **kwargs):
+ */
+        av_packet_free((&__pyx_v_self->packet_ptr));
+      }
+
+      /* "av/container/output.pyx":42
+ *     def __dealloc__(self):
+ *         close_output(self)
+ *         with nogil:             # <<<<<<<<<<<<<<
+ *             lib.av_packet_free(&self.packet_ptr)
+ * 
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L5;
+        }
+        __pyx_L5:;
+      }
+  }
+
+  /* "av/container/output.pyx":40
+ *             self.packet_ptr = lib.av_packet_alloc()
+ * 
+ *     def __dealloc__(self):             # <<<<<<<<<<<<<<
+ *         close_output(self)
+ *         with nogil:
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_WriteUnraisable("av.container.output.OutputContainer.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "av/container/output.pyx":41
- *         close_output(self)
+/* "av/container/output.pyx":45
+ *             lib.av_packet_free(&self.packet_ptr)
  * 
  *     def add_stream(self, codec_name=None, object rate=None, Stream template=None, options=None, **kwargs):             # <<<<<<<<<<<<<<
  *         """add_stream(codec_name, rate=None)
  * 
  */
 
 /* Python wrapper */
@@ -2709,15 +2810,15 @@
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_options);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "add_stream") < 0)) __PYX_ERR(0, 41, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, __pyx_v_kwargs, values, pos_args, "add_stream") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -2732,22 +2833,22 @@
     __pyx_v_codec_name = values[0];
     __pyx_v_rate = values[1];
     __pyx_v_template = ((struct __pyx_obj_2av_6stream_Stream *)values[2]);
     __pyx_v_options = values[3];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("add_stream", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 41, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("add_stream", 0, 0, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 45, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwargs); __pyx_v_kwargs = 0;
   __Pyx_AddTraceback("av.container.output.OutputContainer.add_stream", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_template), __pyx_ptype_2av_6stream_Stream, 1, "template", 0))) __PYX_ERR(0, 41, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_template), __pyx_ptype_2av_6stream_Stream, 1, "template", 0))) __PYX_ERR(0, 45, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_9container_6output_15OutputContainer_4add_stream(((struct __pyx_obj_2av_9container_6output_OutputContainer *)__pyx_v_self), __pyx_v_codec_name, __pyx_v_rate, __pyx_v_template, __pyx_v_options, __pyx_v_kwargs);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -2786,15 +2887,15 @@
   int __pyx_t_18;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("add_stream", 0);
   __Pyx_INCREF(__pyx_v_rate);
 
-  /* "av/container/output.pyx":55
+  /* "av/container/output.pyx":59
  *         """
  * 
  *         if (codec_name is None and template is None) or (codec_name is not None and template is not None):             # <<<<<<<<<<<<<<
  *             raise ValueError('needs one of codec_name or template')
  * 
  */
   __pyx_t_2 = (__pyx_v_codec_name == Py_None);
@@ -2820,366 +2921,366 @@
   }
   __pyx_t_3 = (((PyObject *)__pyx_v_template) != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "av/container/output.pyx":56
+    /* "av/container/output.pyx":60
  * 
  *         if (codec_name is None and template is None) or (codec_name is not None and template is not None):
  *             raise ValueError('needs one of codec_name or template')             # <<<<<<<<<<<<<<
  * 
  *         cdef const lib.AVCodec *codec
  */
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 56, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 60, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 56, __pyx_L1_error)
+    __PYX_ERR(0, 60, __pyx_L1_error)
 
-    /* "av/container/output.pyx":55
+    /* "av/container/output.pyx":59
  *         """
  * 
  *         if (codec_name is None and template is None) or (codec_name is not None and template is not None):             # <<<<<<<<<<<<<<
  *             raise ValueError('needs one of codec_name or template')
  * 
  */
   }
 
-  /* "av/container/output.pyx":61
+  /* "av/container/output.pyx":65
  *         cdef Codec codec_obj
  * 
  *         if codec_name is not None:             # <<<<<<<<<<<<<<
  *             codec_obj = codec_name if isinstance(codec_name, Codec) else Codec(codec_name, 'w')
  *             codec = codec_obj.ptr
  */
   __pyx_t_1 = (__pyx_v_codec_name != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/output.pyx":62
+    /* "av/container/output.pyx":66
  * 
  *         if codec_name is not None:
  *             codec_obj = codec_name if isinstance(codec_name, Codec) else Codec(codec_name, 'w')             # <<<<<<<<<<<<<<
  *             codec = codec_obj.ptr
  * 
  */
     __pyx_t_2 = __Pyx_TypeCheck(__pyx_v_codec_name, __pyx_ptype_2av_5codec_5codec_Codec); 
     if ((__pyx_t_2 != 0)) {
-      if (!(likely(((__pyx_v_codec_name) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_codec_name, __pyx_ptype_2av_5codec_5codec_Codec))))) __PYX_ERR(0, 62, __pyx_L1_error)
+      if (!(likely(((__pyx_v_codec_name) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_codec_name, __pyx_ptype_2av_5codec_5codec_Codec))))) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_INCREF(__pyx_v_codec_name);
       __pyx_t_4 = __pyx_v_codec_name;
     } else {
-      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 62, __pyx_L1_error)
+      __pyx_t_5 = PyTuple_New(2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_v_codec_name);
       __Pyx_GIVEREF(__pyx_v_codec_name);
       PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_codec_name);
       __Pyx_INCREF(__pyx_n_s_w);
       __Pyx_GIVEREF(__pyx_n_s_w);
       PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_n_s_w);
-      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_5codec_5codec_Codec), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 62, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_5codec_5codec_Codec), __pyx_t_5, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 66, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_t_4 = __pyx_t_6;
       __pyx_t_6 = 0;
     }
     __pyx_v_codec_obj = ((struct __pyx_obj_2av_5codec_5codec_Codec *)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "av/container/output.pyx":63
+    /* "av/container/output.pyx":67
  *         if codec_name is not None:
  *             codec_obj = codec_name if isinstance(codec_name, Codec) else Codec(codec_name, 'w')
  *             codec = codec_obj.ptr             # <<<<<<<<<<<<<<
  * 
  *         else:
  */
     __pyx_t_7 = __pyx_v_codec_obj->ptr;
     __pyx_v_codec = __pyx_t_7;
 
-    /* "av/container/output.pyx":61
+    /* "av/container/output.pyx":65
  *         cdef Codec codec_obj
  * 
  *         if codec_name is not None:             # <<<<<<<<<<<<<<
  *             codec_obj = codec_name if isinstance(codec_name, Codec) else Codec(codec_name, 'w')
  *             codec = codec_obj.ptr
  */
     goto __pyx_L8;
   }
 
-  /* "av/container/output.pyx":66
+  /* "av/container/output.pyx":70
  * 
  *         else:
  *             if not template._codec:             # <<<<<<<<<<<<<<
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:
  */
   /*else*/ {
     __pyx_t_2 = ((!(__pyx_v_template->_codec != 0)) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "av/container/output.pyx":67
+      /* "av/container/output.pyx":71
  *         else:
  *             if not template._codec:
  *                 raise ValueError("template has no codec")             # <<<<<<<<<<<<<<
  *             if not template._codec_context:
  *                 raise ValueError("template has no codec context")
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 71, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 67, __pyx_L1_error)
+      __PYX_ERR(0, 71, __pyx_L1_error)
 
-      /* "av/container/output.pyx":66
+      /* "av/container/output.pyx":70
  * 
  *         else:
  *             if not template._codec:             # <<<<<<<<<<<<<<
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:
  */
     }
 
-    /* "av/container/output.pyx":68
+    /* "av/container/output.pyx":72
  *             if not template._codec:
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:             # <<<<<<<<<<<<<<
  *                 raise ValueError("template has no codec context")
  *             codec = template._codec
  */
     __pyx_t_2 = ((!(__pyx_v_template->_codec_context != 0)) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "av/container/output.pyx":69
+      /* "av/container/output.pyx":73
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:
  *                 raise ValueError("template has no codec context")             # <<<<<<<<<<<<<<
  *             codec = template._codec
  * 
  */
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 69, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 73, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_Raise(__pyx_t_4, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __PYX_ERR(0, 69, __pyx_L1_error)
+      __PYX_ERR(0, 73, __pyx_L1_error)
 
-      /* "av/container/output.pyx":68
+      /* "av/container/output.pyx":72
  *             if not template._codec:
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:             # <<<<<<<<<<<<<<
  *                 raise ValueError("template has no codec context")
  *             codec = template._codec
  */
     }
 
-    /* "av/container/output.pyx":70
+    /* "av/container/output.pyx":74
  *             if not template._codec_context:
  *                 raise ValueError("template has no codec context")
  *             codec = template._codec             # <<<<<<<<<<<<<<
  * 
  *         # Assert that this format supports the requested codec.
  */
     __pyx_t_8 = __pyx_v_template->_codec;
     __pyx_v_codec = __pyx_t_8;
   }
   __pyx_L8:;
 
-  /* "av/container/output.pyx":73
+  /* "av/container/output.pyx":77
  * 
  *         # Assert that this format supports the requested codec.
  *         if not lib.avformat_query_codec(             # <<<<<<<<<<<<<<
  *             self.ptr.oformat,
  *             codec.id,
  */
   __pyx_t_2 = ((!(avformat_query_codec(__pyx_v_self->__pyx_base.ptr->oformat, __pyx_v_codec->id, FF_COMPLIANCE_NORMAL) != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/container/output.pyx":78
+    /* "av/container/output.pyx":82
  *             lib.FF_COMPLIANCE_NORMAL,
  *         ):
  *             raise ValueError("%r format does not support %r codec" % (self.format.name, codec_name))             # <<<<<<<<<<<<<<
  * 
  *         # Create new stream in the AVFormatContext, set AVCodecContext values.
  */
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_self->__pyx_base.format->name);
     __Pyx_GIVEREF(__pyx_v_self->__pyx_base.format->name);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_self->__pyx_base.format->name);
     __Pyx_INCREF(__pyx_v_codec_name);
     __Pyx_GIVEREF(__pyx_v_codec_name);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_v_codec_name);
-    __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_r_format_does_not_support_r_cod, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_r_format_does_not_support_r_cod, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 78, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __PYX_ERR(0, 78, __pyx_L1_error)
+    __PYX_ERR(0, 82, __pyx_L1_error)
 
-    /* "av/container/output.pyx":73
+    /* "av/container/output.pyx":77
  * 
  *         # Assert that this format supports the requested codec.
  *         if not lib.avformat_query_codec(             # <<<<<<<<<<<<<<
  *             self.ptr.oformat,
  *             codec.id,
  */
   }
 
-  /* "av/container/output.pyx":84
+  /* "av/container/output.pyx":88
  *         # the context, but doesn't modify it in any other way. Ergo, we can allow CodecContext
  *         # to finish initializing it.
  *         lib.avformat_new_stream(self.ptr, codec)             # <<<<<<<<<<<<<<
  *         cdef lib.AVStream *stream = self.ptr.streams[self.ptr.nb_streams - 1]
  *         cdef lib.AVCodecContext *codec_context = stream.codec  # For readability.
  */
   (void)(avformat_new_stream(__pyx_v_self->__pyx_base.ptr, __pyx_v_codec));
 
-  /* "av/container/output.pyx":85
+  /* "av/container/output.pyx":89
  *         # to finish initializing it.
  *         lib.avformat_new_stream(self.ptr, codec)
  *         cdef lib.AVStream *stream = self.ptr.streams[self.ptr.nb_streams - 1]             # <<<<<<<<<<<<<<
  *         cdef lib.AVCodecContext *codec_context = stream.codec  # For readability.
  * 
  */
   __pyx_v_stream = (__pyx_v_self->__pyx_base.ptr->streams[(__pyx_v_self->__pyx_base.ptr->nb_streams - 1)]);
 
-  /* "av/container/output.pyx":86
+  /* "av/container/output.pyx":90
  *         lib.avformat_new_stream(self.ptr, codec)
  *         cdef lib.AVStream *stream = self.ptr.streams[self.ptr.nb_streams - 1]
  *         cdef lib.AVCodecContext *codec_context = stream.codec  # For readability.             # <<<<<<<<<<<<<<
  * 
  *         # Copy from the template.
  */
   __pyx_t_9 = __pyx_v_stream->codec;
   __pyx_v_codec_context = __pyx_t_9;
 
-  /* "av/container/output.pyx":89
+  /* "av/container/output.pyx":93
  * 
  *         # Copy from the template.
  *         if template is not None:             # <<<<<<<<<<<<<<
  *             lib.avcodec_copy_context(codec_context, template._codec_context)
  *             # Reset the codec tag assuming we are remuxing.
  */
   __pyx_t_2 = (((PyObject *)__pyx_v_template) != Py_None);
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "av/container/output.pyx":90
+    /* "av/container/output.pyx":94
  *         # Copy from the template.
  *         if template is not None:
  *             lib.avcodec_copy_context(codec_context, template._codec_context)             # <<<<<<<<<<<<<<
  *             # Reset the codec tag assuming we are remuxing.
  *             codec_context.codec_tag = 0
  */
     (void)(avcodec_copy_context(__pyx_v_codec_context, __pyx_v_template->_codec_context));
 
-    /* "av/container/output.pyx":92
+    /* "av/container/output.pyx":96
  *             lib.avcodec_copy_context(codec_context, template._codec_context)
  *             # Reset the codec tag assuming we are remuxing.
  *             codec_context.codec_tag = 0             # <<<<<<<<<<<<<<
  * 
  *         # Now lets set some more sane video defaults
  */
     __pyx_v_codec_context->codec_tag = 0;
 
-    /* "av/container/output.pyx":89
+    /* "av/container/output.pyx":93
  * 
  *         # Copy from the template.
  *         if template is not None:             # <<<<<<<<<<<<<<
  *             lib.avcodec_copy_context(codec_context, template._codec_context)
  *             # Reset the codec tag assuming we are remuxing.
  */
     goto __pyx_L12;
   }
 
-  /* "av/container/output.pyx":95
+  /* "av/container/output.pyx":99
  * 
  *         # Now lets set some more sane video defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_VIDEO:             # <<<<<<<<<<<<<<
  *             codec_context.pix_fmt = lib.AV_PIX_FMT_YUV420P
  *             codec_context.width = 640
  */
   __pyx_t_1 = ((__pyx_v_codec->type == AVMEDIA_TYPE_VIDEO) != 0);
   if (__pyx_t_1) {
 
-    /* "av/container/output.pyx":96
+    /* "av/container/output.pyx":100
  *         # Now lets set some more sane video defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_VIDEO:
  *             codec_context.pix_fmt = lib.AV_PIX_FMT_YUV420P             # <<<<<<<<<<<<<<
  *             codec_context.width = 640
  *             codec_context.height = 480
  */
     __pyx_v_codec_context->pix_fmt = AV_PIX_FMT_YUV420P;
 
-    /* "av/container/output.pyx":97
+    /* "av/container/output.pyx":101
  *         elif codec.type == lib.AVMEDIA_TYPE_VIDEO:
  *             codec_context.pix_fmt = lib.AV_PIX_FMT_YUV420P
  *             codec_context.width = 640             # <<<<<<<<<<<<<<
  *             codec_context.height = 480
  *             codec_context.bit_rate = 1024000
  */
     __pyx_v_codec_context->width = 0x280;
 
-    /* "av/container/output.pyx":98
+    /* "av/container/output.pyx":102
  *             codec_context.pix_fmt = lib.AV_PIX_FMT_YUV420P
  *             codec_context.width = 640
  *             codec_context.height = 480             # <<<<<<<<<<<<<<
  *             codec_context.bit_rate = 1024000
  *             codec_context.bit_rate_tolerance = 128000
  */
     __pyx_v_codec_context->height = 0x1E0;
 
-    /* "av/container/output.pyx":99
+    /* "av/container/output.pyx":103
  *             codec_context.width = 640
  *             codec_context.height = 480
  *             codec_context.bit_rate = 1024000             # <<<<<<<<<<<<<<
  *             codec_context.bit_rate_tolerance = 128000
  *             codec_context.ticks_per_frame = 1
  */
     __pyx_v_codec_context->bit_rate = 0xFA000;
 
-    /* "av/container/output.pyx":100
+    /* "av/container/output.pyx":104
  *             codec_context.height = 480
  *             codec_context.bit_rate = 1024000
  *             codec_context.bit_rate_tolerance = 128000             # <<<<<<<<<<<<<<
  *             codec_context.ticks_per_frame = 1
  * 
  */
     __pyx_v_codec_context->bit_rate_tolerance = 0x1F400;
 
-    /* "av/container/output.pyx":101
+    /* "av/container/output.pyx":105
  *             codec_context.bit_rate = 1024000
  *             codec_context.bit_rate_tolerance = 128000
  *             codec_context.ticks_per_frame = 1             # <<<<<<<<<<<<<<
  * 
  *             rate = Fraction(rate or 24)
  */
     __pyx_v_codec_context->ticks_per_frame = 1;
 
-    /* "av/container/output.pyx":103
+    /* "av/container/output.pyx":107
  *             codec_context.ticks_per_frame = 1
  * 
  *             rate = Fraction(rate or 24)             # <<<<<<<<<<<<<<
  * 
  *             codec_context.framerate.num = rate.numerator
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Fraction); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_Fraction); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rate); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rate); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 107, __pyx_L1_error)
     if (!__pyx_t_1) {
     } else {
       __Pyx_INCREF(__pyx_v_rate);
       __pyx_t_5 = __pyx_v_rate;
       goto __pyx_L13_bool_binop_done;
     }
-    __pyx_t_10 = __Pyx_PyInt_From_long(24); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 103, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyInt_From_long(24); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __pyx_t_5 = __pyx_t_10;
     __pyx_t_10 = 0;
     __pyx_L13_bool_binop_done:;
     __pyx_t_10 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_6);
@@ -3189,391 +3290,391 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_6, function);
       }
     }
     __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_10, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 103, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF_SET(__pyx_v_rate, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "av/container/output.pyx":105
+    /* "av/container/output.pyx":109
  *             rate = Fraction(rate or 24)
  * 
  *             codec_context.framerate.num = rate.numerator             # <<<<<<<<<<<<<<
  *             codec_context.framerate.den = rate.denominator
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rate, __pyx_n_s_numerator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rate, __pyx_n_s_numerator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 105, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_codec_context->framerate.num = __pyx_t_11;
 
-    /* "av/container/output.pyx":106
+    /* "av/container/output.pyx":110
  * 
  *             codec_context.framerate.num = rate.numerator
  *             codec_context.framerate.den = rate.denominator             # <<<<<<<<<<<<<<
  * 
  *             stream.avg_frame_rate = codec_context.framerate
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rate, __pyx_n_s_denominator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_rate, __pyx_n_s_denominator); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 106, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_11 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_v_codec_context->framerate.den = __pyx_t_11;
 
-    /* "av/container/output.pyx":108
+    /* "av/container/output.pyx":112
  *             codec_context.framerate.den = rate.denominator
  * 
  *             stream.avg_frame_rate = codec_context.framerate             # <<<<<<<<<<<<<<
  *             stream.time_base = codec_context.time_base
  * 
  */
     __pyx_t_12 = __pyx_v_codec_context->framerate;
     __pyx_v_stream->avg_frame_rate = __pyx_t_12;
 
-    /* "av/container/output.pyx":109
+    /* "av/container/output.pyx":113
  * 
  *             stream.avg_frame_rate = codec_context.framerate
  *             stream.time_base = codec_context.time_base             # <<<<<<<<<<<<<<
  * 
  *         # Some sane audio defaults
  */
     __pyx_t_12 = __pyx_v_codec_context->time_base;
     __pyx_v_stream->time_base = __pyx_t_12;
 
-    /* "av/container/output.pyx":95
+    /* "av/container/output.pyx":99
  * 
  *         # Now lets set some more sane video defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_VIDEO:             # <<<<<<<<<<<<<<
  *             codec_context.pix_fmt = lib.AV_PIX_FMT_YUV420P
  *             codec_context.width = 640
  */
     goto __pyx_L12;
   }
 
-  /* "av/container/output.pyx":112
+  /* "av/container/output.pyx":116
  * 
  *         # Some sane audio defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_AUDIO:             # <<<<<<<<<<<<<<
  *             codec_context.sample_fmt = codec.sample_fmts[0]
  *             codec_context.bit_rate = 128000
  */
   __pyx_t_1 = ((__pyx_v_codec->type == AVMEDIA_TYPE_AUDIO) != 0);
   if (__pyx_t_1) {
 
-    /* "av/container/output.pyx":113
+    /* "av/container/output.pyx":117
  *         # Some sane audio defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_AUDIO:
  *             codec_context.sample_fmt = codec.sample_fmts[0]             # <<<<<<<<<<<<<<
  *             codec_context.bit_rate = 128000
  *             codec_context.bit_rate_tolerance = 32000
  */
     __pyx_v_codec_context->sample_fmt = (__pyx_v_codec->sample_fmts[0]);
 
-    /* "av/container/output.pyx":114
+    /* "av/container/output.pyx":118
  *         elif codec.type == lib.AVMEDIA_TYPE_AUDIO:
  *             codec_context.sample_fmt = codec.sample_fmts[0]
  *             codec_context.bit_rate = 128000             # <<<<<<<<<<<<<<
  *             codec_context.bit_rate_tolerance = 32000
  *             codec_context.sample_rate = rate or 48000
  */
     __pyx_v_codec_context->bit_rate = 0x1F400;
 
-    /* "av/container/output.pyx":115
+    /* "av/container/output.pyx":119
  *             codec_context.sample_fmt = codec.sample_fmts[0]
  *             codec_context.bit_rate = 128000
  *             codec_context.bit_rate_tolerance = 32000             # <<<<<<<<<<<<<<
  *             codec_context.sample_rate = rate or 48000
  *             codec_context.channels = 2
  */
     __pyx_v_codec_context->bit_rate_tolerance = 0x7D00;
 
-    /* "av/container/output.pyx":116
+    /* "av/container/output.pyx":120
  *             codec_context.bit_rate = 128000
  *             codec_context.bit_rate_tolerance = 32000
  *             codec_context.sample_rate = rate or 48000             # <<<<<<<<<<<<<<
  *             codec_context.channels = 2
  *             codec_context.channel_layout = lib.AV_CH_LAYOUT_STEREO
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rate); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_rate); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
     if (!__pyx_t_1) {
     } else {
-      __pyx_t_13 = __Pyx_PyInt_As_int(__pyx_v_rate); if (unlikely((__pyx_t_13 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 116, __pyx_L1_error)
+      __pyx_t_13 = __Pyx_PyInt_As_int(__pyx_v_rate); if (unlikely((__pyx_t_13 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 120, __pyx_L1_error)
       __pyx_t_11 = __pyx_t_13;
       goto __pyx_L15_bool_binop_done;
     }
     __pyx_t_11 = 0xBB80;
     __pyx_L15_bool_binop_done:;
     __pyx_v_codec_context->sample_rate = __pyx_t_11;
 
-    /* "av/container/output.pyx":117
+    /* "av/container/output.pyx":121
  *             codec_context.bit_rate_tolerance = 32000
  *             codec_context.sample_rate = rate or 48000
  *             codec_context.channels = 2             # <<<<<<<<<<<<<<
  *             codec_context.channel_layout = lib.AV_CH_LAYOUT_STEREO
  * 
  */
     __pyx_v_codec_context->channels = 2;
 
-    /* "av/container/output.pyx":118
+    /* "av/container/output.pyx":122
  *             codec_context.sample_rate = rate or 48000
  *             codec_context.channels = 2
  *             codec_context.channel_layout = lib.AV_CH_LAYOUT_STEREO             # <<<<<<<<<<<<<<
  * 
  *         # Some formats want stream headers to be separate
  */
     __pyx_v_codec_context->channel_layout = AV_CH_LAYOUT_STEREO;
 
-    /* "av/container/output.pyx":112
+    /* "av/container/output.pyx":116
  * 
  *         # Some sane audio defaults
  *         elif codec.type == lib.AVMEDIA_TYPE_AUDIO:             # <<<<<<<<<<<<<<
  *             codec_context.sample_fmt = codec.sample_fmts[0]
  *             codec_context.bit_rate = 128000
  */
   }
   __pyx_L12:;
 
-  /* "av/container/output.pyx":121
+  /* "av/container/output.pyx":125
  * 
  *         # Some formats want stream headers to be separate
  *         if self.ptr.oformat.flags & lib.AVFMT_GLOBALHEADER:             # <<<<<<<<<<<<<<
  *             codec_context.flags |= lib.AV_CODEC_FLAG_GLOBAL_HEADER
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->__pyx_base.ptr->oformat->flags & AVFMT_GLOBALHEADER) != 0);
   if (__pyx_t_1) {
 
-    /* "av/container/output.pyx":122
+    /* "av/container/output.pyx":126
  *         # Some formats want stream headers to be separate
  *         if self.ptr.oformat.flags & lib.AVFMT_GLOBALHEADER:
  *             codec_context.flags |= lib.AV_CODEC_FLAG_GLOBAL_HEADER             # <<<<<<<<<<<<<<
  * 
  *         # Construct the user-land stream
  */
     __pyx_v_codec_context->flags = (__pyx_v_codec_context->flags | AV_CODEC_FLAG_GLOBAL_HEADER);
 
-    /* "av/container/output.pyx":121
+    /* "av/container/output.pyx":125
  * 
  *         # Some formats want stream headers to be separate
  *         if self.ptr.oformat.flags & lib.AVFMT_GLOBALHEADER:             # <<<<<<<<<<<<<<
  *             codec_context.flags |= lib.AV_CODEC_FLAG_GLOBAL_HEADER
  * 
  */
   }
 
-  /* "av/container/output.pyx":125
+  /* "av/container/output.pyx":129
  * 
  *         # Construct the user-land stream
  *         cdef Stream py_stream = wrap_stream(self, stream)             # <<<<<<<<<<<<<<
  *         self.streams.add_stream(py_stream)
  * 
  */
-  __pyx_t_4 = ((PyObject *)__pyx_f_2av_6stream_wrap_stream(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_stream)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+  __pyx_t_4 = ((PyObject *)__pyx_f_2av_6stream_wrap_stream(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_stream)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_v_py_stream = ((struct __pyx_obj_2av_6stream_Stream *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "av/container/output.pyx":126
+  /* "av/container/output.pyx":130
  *         # Construct the user-land stream
  *         cdef Stream py_stream = wrap_stream(self, stream)
  *         self.streams.add_stream(py_stream)             # <<<<<<<<<<<<<<
  * 
  *         if options:
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer *)__pyx_v_self->__pyx_base.streams->__pyx_vtab)->add_stream(__pyx_v_self->__pyx_base.streams, __pyx_v_py_stream); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer *)__pyx_v_self->__pyx_base.streams->__pyx_vtab)->add_stream(__pyx_v_self->__pyx_base.streams, __pyx_v_py_stream); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "av/container/output.pyx":128
+  /* "av/container/output.pyx":132
  *         self.streams.add_stream(py_stream)
  * 
  *         if options:             # <<<<<<<<<<<<<<
  *             py_stream.options.update(options)
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_options); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 128, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_options); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "av/container/output.pyx":129
+    /* "av/container/output.pyx":133
  * 
  *         if options:
  *             py_stream.options.update(options)             # <<<<<<<<<<<<<<
  * 
  *         for k, v in kwargs.items():
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_py_stream), __pyx_n_s_options); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_py_stream), __pyx_n_s_options); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_options) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_options);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "av/container/output.pyx":128
+    /* "av/container/output.pyx":132
  *         self.streams.add_stream(py_stream)
  * 
  *         if options:             # <<<<<<<<<<<<<<
  *             py_stream.options.update(options)
  * 
  */
   }
 
-  /* "av/container/output.pyx":131
+  /* "av/container/output.pyx":135
  *             py_stream.options.update(options)
  * 
  *         for k, v in kwargs.items():             # <<<<<<<<<<<<<<
  *             setattr(py_stream, k, v)
  * 
  */
-  __pyx_t_4 = __Pyx_PyDict_Items(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_Items(__pyx_v_kwargs); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (likely(PyList_CheckExact(__pyx_t_4)) || PyTuple_CheckExact(__pyx_t_4)) {
     __pyx_t_5 = __pyx_t_4; __Pyx_INCREF(__pyx_t_5); __pyx_t_14 = 0;
     __pyx_t_15 = NULL;
   } else {
-    __pyx_t_14 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_14 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 135, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_15 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __pyx_t_15 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 135, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   for (;;) {
     if (likely(!__pyx_t_15)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_14 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_4); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_4); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_14 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_4); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_14); __Pyx_INCREF(__pyx_t_4); __pyx_t_14++; if (unlikely(0 < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_5, __pyx_t_14); __pyx_t_14++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_15(__pyx_t_5);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 131, __pyx_L1_error)
+          else __PYX_ERR(0, 135, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     if ((likely(PyTuple_CheckExact(__pyx_t_4))) || (PyList_CheckExact(__pyx_t_4))) {
       PyObject* sequence = __pyx_t_4;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 131, __pyx_L1_error)
+        __PYX_ERR(0, 135, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_6 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_10 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_6 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_10 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_10);
       #else
-      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_6 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_10 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       #endif
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_16 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 131, __pyx_L1_error)
+      __pyx_t_16 = PyObject_GetIter(__pyx_t_4); if (unlikely(!__pyx_t_16)) __PYX_ERR(0, 135, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_16);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_17 = Py_TYPE(__pyx_t_16)->tp_iternext;
       index = 0; __pyx_t_6 = __pyx_t_17(__pyx_t_16); if (unlikely(!__pyx_t_6)) goto __pyx_L21_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_6);
       index = 1; __pyx_t_10 = __pyx_t_17(__pyx_t_16); if (unlikely(!__pyx_t_10)) goto __pyx_L21_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_10);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_17(__pyx_t_16), 2) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_17(__pyx_t_16), 2) < 0) __PYX_ERR(0, 135, __pyx_L1_error)
       __pyx_t_17 = NULL;
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       goto __pyx_L22_unpacking_done;
       __pyx_L21_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_16); __pyx_t_16 = 0;
       __pyx_t_17 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 131, __pyx_L1_error)
+      __PYX_ERR(0, 135, __pyx_L1_error)
       __pyx_L22_unpacking_done:;
     }
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_6);
     __pyx_t_6 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_10);
     __pyx_t_10 = 0;
 
-    /* "av/container/output.pyx":132
+    /* "av/container/output.pyx":136
  * 
  *         for k, v in kwargs.items():
  *             setattr(py_stream, k, v)             # <<<<<<<<<<<<<<
  * 
  *         return py_stream
  */
-    __pyx_t_18 = PyObject_SetAttr(((PyObject *)__pyx_v_py_stream), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 132, __pyx_L1_error)
+    __pyx_t_18 = PyObject_SetAttr(((PyObject *)__pyx_v_py_stream), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_18 == ((int)-1))) __PYX_ERR(0, 136, __pyx_L1_error)
 
-    /* "av/container/output.pyx":131
+    /* "av/container/output.pyx":135
  *             py_stream.options.update(options)
  * 
  *         for k, v in kwargs.items():             # <<<<<<<<<<<<<<
  *             setattr(py_stream, k, v)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "av/container/output.pyx":134
+  /* "av/container/output.pyx":138
  *             setattr(py_stream, k, v)
  * 
  *         return py_stream             # <<<<<<<<<<<<<<
  * 
  *     cpdef start_encoding(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_py_stream));
   __pyx_r = ((PyObject *)__pyx_v_py_stream);
   goto __pyx_L0;
 
-  /* "av/container/output.pyx":41
- *         close_output(self)
+  /* "av/container/output.pyx":45
+ *             lib.av_packet_free(&self.packet_ptr)
  * 
  *     def add_stream(self, codec_name=None, object rate=None, Stream template=None, options=None, **kwargs):             # <<<<<<<<<<<<<<
  *         """add_stream(codec_name, rate=None)
  * 
  */
 
   /* function exit code */
@@ -3592,15 +3693,15 @@
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XDECREF(__pyx_v_rate);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/output.pyx":136
+/* "av/container/output.pyx":140
  *         return py_stream
  * 
  *     cpdef start_encoding(self):             # <<<<<<<<<<<<<<
  *         """Write the file header! Called automatically."""
  * 
  */
 
@@ -3647,15 +3748,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || (Py_TYPE(((PyObject *)__pyx_v_self))->tp_flags & (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_type_dict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start_encoding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_start_encoding); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!PyCFunction_Check(__pyx_t_1) || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_2av_9container_6output_15OutputContainer_7start_encoding)) {
         __Pyx_XDECREF(__pyx_r);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_3 = __pyx_t_1; __pyx_t_4 = NULL;
         if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
           __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
@@ -3664,15 +3765,15 @@
             __Pyx_INCREF(__pyx_t_4);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_3, function);
           }
         }
         __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
         __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_r = __pyx_t_2;
         __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -3685,372 +3786,372 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "av/container/output.pyx":139
+  /* "av/container/output.pyx":143
  *         """Write the file header! Called automatically."""
  * 
  *         if self._started:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   __pyx_t_5 = (__pyx_v_self->_started != 0);
   if (__pyx_t_5) {
 
-    /* "av/container/output.pyx":140
+    /* "av/container/output.pyx":144
  * 
  *         if self._started:
  *             return             # <<<<<<<<<<<<<<
  * 
  *         # TODO: This does NOT handle options coming from 3 sources.
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "av/container/output.pyx":139
+    /* "av/container/output.pyx":143
  *         """Write the file header! Called automatically."""
  * 
  *         if self._started:             # <<<<<<<<<<<<<<
  *             return
  * 
  */
   }
 
-  /* "av/container/output.pyx":144
+  /* "av/container/output.pyx":148
  *         # TODO: This does NOT handle options coming from 3 sources.
  *         # This is only a rough approximation of what would be cool to do.
  *         used_options = set()             # <<<<<<<<<<<<<<
  * 
  *         # Finalize and open all streams.
  */
-  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+  __pyx_t_1 = PySet_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_used_options = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":148
+  /* "av/container/output.pyx":152
  *         # Finalize and open all streams.
  *         cdef Stream stream
  *         for stream in self.streams:             # <<<<<<<<<<<<<<
  * 
  *             ctx = stream.codec_context
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self->__pyx_base.streams))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self->__pyx_base.streams))) {
     __pyx_t_1 = ((PyObject *)__pyx_v_self->__pyx_base.streams); __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self->__pyx_base.streams)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self->__pyx_base.streams)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 152, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 152, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_2); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 152, __pyx_L1_error)
         #else
-        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+        __pyx_t_2 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_7(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 148, __pyx_L1_error)
+          else __PYX_ERR(0, 152, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_6stream_Stream))))) __PYX_ERR(0, 148, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2av_6stream_Stream))))) __PYX_ERR(0, 152, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_stream, ((struct __pyx_obj_2av_6stream_Stream *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "av/container/output.pyx":150
+    /* "av/container/output.pyx":154
  *         for stream in self.streams:
  * 
  *             ctx = stream.codec_context             # <<<<<<<<<<<<<<
  *             if not ctx.is_open:
  * 
  */
     __pyx_t_2 = ((PyObject *)__pyx_v_stream->codec_context);
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_ctx, ((struct __pyx_obj_2av_5codec_7context_CodecContext *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "av/container/output.pyx":151
+    /* "av/container/output.pyx":155
  * 
  *             ctx = stream.codec_context
  *             if not ctx.is_open:             # <<<<<<<<<<<<<<
  * 
  *                 for k, v in self.options.items():
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ctx), __pyx_n_s_is_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_ctx), __pyx_n_s_is_open); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 155, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_t_8 = ((!__pyx_t_5) != 0);
     if (__pyx_t_8) {
 
-      /* "av/container/output.pyx":153
+      /* "av/container/output.pyx":157
  *             if not ctx.is_open:
  * 
  *                 for k, v in self.options.items():             # <<<<<<<<<<<<<<
  *                     ctx.options.setdefault(k, v)
  *                 ctx.open()
  */
       if (unlikely(__pyx_v_self->__pyx_base.options == Py_None)) {
         PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-        __PYX_ERR(0, 153, __pyx_L1_error)
+        __PYX_ERR(0, 157, __pyx_L1_error)
       }
-      __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_self->__pyx_base.options); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_Items(__pyx_v_self->__pyx_base.options); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
         __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3); __pyx_t_9 = 0;
         __pyx_t_10 = NULL;
       } else {
-        __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __pyx_t_9 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 157, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 153, __pyx_L1_error)
+        __pyx_t_10 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 157, __pyx_L1_error)
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       for (;;) {
         if (likely(!__pyx_t_10)) {
           if (likely(PyList_CheckExact(__pyx_t_3))) {
             if (__pyx_t_9 >= PyList_GET_SIZE(__pyx_t_3)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 153, __pyx_L1_error)
+            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
             #else
-            __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           } else {
             if (__pyx_t_9 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 153, __pyx_L1_error)
+            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely(0 < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
             #else
-            __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+            __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           }
         } else {
           __pyx_t_2 = __pyx_t_10(__pyx_t_3);
           if (unlikely(!__pyx_t_2)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 153, __pyx_L1_error)
+              else __PYX_ERR(0, 157, __pyx_L1_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_2);
         }
         if ((likely(PyTuple_CheckExact(__pyx_t_2))) || (PyList_CheckExact(__pyx_t_2))) {
           PyObject* sequence = __pyx_t_2;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 153, __pyx_L1_error)
+            __PYX_ERR(0, 157, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
             __pyx_t_11 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
             __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
             __pyx_t_11 = PyList_GET_ITEM(sequence, 1); 
           }
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(__pyx_t_11);
           #else
-          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
-          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 153, __pyx_L1_error)
+          __pyx_t_11 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 157, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_11);
           #endif
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_12 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 153, __pyx_L1_error)
+          __pyx_t_12 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 157, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __pyx_t_13 = Py_TYPE(__pyx_t_12)->tp_iternext;
           index = 0; __pyx_t_4 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_4)) goto __pyx_L9_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_4);
           index = 1; __pyx_t_11 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_11)) goto __pyx_L9_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_11);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 153, __pyx_L1_error)
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 157, __pyx_L1_error)
           __pyx_t_13 = NULL;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           goto __pyx_L10_unpacking_done;
           __pyx_L9_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
           __pyx_t_13 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 153, __pyx_L1_error)
+          __PYX_ERR(0, 157, __pyx_L1_error)
           __pyx_L10_unpacking_done:;
         }
         __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_4);
         __pyx_t_4 = 0;
         __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_11);
         __pyx_t_11 = 0;
 
-        /* "av/container/output.pyx":154
+        /* "av/container/output.pyx":158
  * 
  *                 for k, v in self.options.items():
  *                     ctx.options.setdefault(k, v)             # <<<<<<<<<<<<<<
  *                 ctx.open()
  * 
  */
         if (unlikely(__pyx_v_ctx->options == Py_None)) {
           PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "setdefault");
-          __PYX_ERR(0, 154, __pyx_L1_error)
+          __PYX_ERR(0, 158, __pyx_L1_error)
         }
-        __pyx_t_2 = __Pyx_PyDict_SetDefault(__pyx_v_ctx->options, __pyx_v_k, __pyx_v_v, -1L); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyDict_SetDefault(__pyx_v_ctx->options, __pyx_v_k, __pyx_v_v, -1L); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-        /* "av/container/output.pyx":153
+        /* "av/container/output.pyx":157
  *             if not ctx.is_open:
  * 
  *                 for k, v in self.options.items():             # <<<<<<<<<<<<<<
  *                     ctx.options.setdefault(k, v)
  *                 ctx.open()
  */
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "av/container/output.pyx":155
+      /* "av/container/output.pyx":159
  *                 for k, v in self.options.items():
  *                     ctx.options.setdefault(k, v)
  *                 ctx.open()             # <<<<<<<<<<<<<<
  * 
  *                 # Track option consumption.
  */
-      __pyx_t_3 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_ctx->__pyx_vtab)->open(__pyx_v_ctx, 0, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 155, __pyx_L1_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_2av_5codec_7context_CodecContext *)__pyx_v_ctx->__pyx_vtab)->open(__pyx_v_ctx, 0, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 159, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "av/container/output.pyx":158
+      /* "av/container/output.pyx":162
  * 
  *                 # Track option consumption.
  *                 for k in self.options:             # <<<<<<<<<<<<<<
  *                     if k not in ctx.options:
  *                         used_options.add(k)
  */
       __pyx_t_9 = 0;
       if (unlikely(__pyx_v_self->__pyx_base.options == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-        __PYX_ERR(0, 158, __pyx_L1_error)
+        __PYX_ERR(0, 162, __pyx_L1_error)
       }
-      __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->__pyx_base.options, 1, ((PyObject *)NULL), (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_dict_iterator(__pyx_v_self->__pyx_base.options, 1, ((PyObject *)NULL), (&__pyx_t_14), (&__pyx_t_15)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_XDECREF(__pyx_t_3);
       __pyx_t_3 = __pyx_t_2;
       __pyx_t_2 = 0;
       while (1) {
         __pyx_t_16 = __Pyx_dict_iter_next(__pyx_t_3, __pyx_t_14, &__pyx_t_9, &__pyx_t_2, NULL, NULL, __pyx_t_15);
         if (unlikely(__pyx_t_16 == 0)) break;
-        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 158, __pyx_L1_error)
+        if (unlikely(__pyx_t_16 == -1)) __PYX_ERR(0, 162, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "av/container/output.pyx":159
+        /* "av/container/output.pyx":163
  *                 # Track option consumption.
  *                 for k in self.options:
  *                     if k not in ctx.options:             # <<<<<<<<<<<<<<
  *                         used_options.add(k)
  * 
  */
         if (unlikely(__pyx_v_ctx->options == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-          __PYX_ERR(0, 159, __pyx_L1_error)
+          __PYX_ERR(0, 163, __pyx_L1_error)
         }
-        __pyx_t_8 = (__Pyx_PyDict_ContainsTF(__pyx_v_k, __pyx_v_ctx->options, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 159, __pyx_L1_error)
+        __pyx_t_8 = (__Pyx_PyDict_ContainsTF(__pyx_v_k, __pyx_v_ctx->options, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 163, __pyx_L1_error)
         __pyx_t_5 = (__pyx_t_8 != 0);
         if (__pyx_t_5) {
 
-          /* "av/container/output.pyx":160
+          /* "av/container/output.pyx":164
  *                 for k in self.options:
  *                     if k not in ctx.options:
  *                         used_options.add(k)             # <<<<<<<<<<<<<<
  * 
  *             stream._finalize_for_output()
  */
-          __pyx_t_17 = PySet_Add(__pyx_v_used_options, __pyx_v_k); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 160, __pyx_L1_error)
+          __pyx_t_17 = PySet_Add(__pyx_v_used_options, __pyx_v_k); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 164, __pyx_L1_error)
 
-          /* "av/container/output.pyx":159
+          /* "av/container/output.pyx":163
  *                 # Track option consumption.
  *                 for k in self.options:
  *                     if k not in ctx.options:             # <<<<<<<<<<<<<<
  *                         used_options.add(k)
  * 
  */
         }
       }
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "av/container/output.pyx":151
+      /* "av/container/output.pyx":155
  * 
  *             ctx = stream.codec_context
  *             if not ctx.is_open:             # <<<<<<<<<<<<<<
  * 
  *                 for k, v in self.options.items():
  */
     }
 
-    /* "av/container/output.pyx":162
+    /* "av/container/output.pyx":166
  *                         used_options.add(k)
  * 
  *             stream._finalize_for_output()             # <<<<<<<<<<<<<<
  * 
  *         # Open the output file, if needed.
  */
-    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_6stream_Stream *)__pyx_v_stream->__pyx_vtab)->_finalize_for_output(__pyx_v_stream); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_2av_6stream_Stream *)__pyx_v_stream->__pyx_vtab)->_finalize_for_output(__pyx_v_stream); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 166, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/container/output.pyx":148
+    /* "av/container/output.pyx":152
  *         # Finalize and open all streams.
  *         cdef Stream stream
  *         for stream in self.streams:             # <<<<<<<<<<<<<<
  * 
  *             ctx = stream.codec_context
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":165
+  /* "av/container/output.pyx":169
  * 
  *         # Open the output file, if needed.
  *         cdef bytes name_obj = os.fsencode(self.name if self.file is None else "")             # <<<<<<<<<<<<<<
  *         cdef char *name = name_obj
  *         if self.ptr.pb == NULL and not self.ptr.oformat.flags & lib.AVFMT_NOFILE:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_os); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fsencode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_fsencode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_5 = (((PyObject *)__pyx_v_self->__pyx_base.file) == Py_None);
   if ((__pyx_t_5 != 0)) {
     __Pyx_INCREF(__pyx_v_self->__pyx_base.name);
     __pyx_t_3 = __pyx_v_self->__pyx_base.name;
   } else {
@@ -4066,36 +4167,36 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_11) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_11, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 165, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 169, __pyx_L1_error)
   __pyx_v_name_obj = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":166
+  /* "av/container/output.pyx":170
  *         # Open the output file, if needed.
  *         cdef bytes name_obj = os.fsencode(self.name if self.file is None else "")
  *         cdef char *name = name_obj             # <<<<<<<<<<<<<<
  *         if self.ptr.pb == NULL and not self.ptr.oformat.flags & lib.AVFMT_NOFILE:
  *             err_check(lib.avio_open(&self.ptr.pb, name, lib.AVIO_FLAG_WRITE))
  */
   if (unlikely(__pyx_v_name_obj == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 166, __pyx_L1_error)
+    __PYX_ERR(0, 170, __pyx_L1_error)
   }
-  __pyx_t_18 = __Pyx_PyBytes_AsWritableString(__pyx_v_name_obj); if (unlikely((!__pyx_t_18) && PyErr_Occurred())) __PYX_ERR(0, 166, __pyx_L1_error)
+  __pyx_t_18 = __Pyx_PyBytes_AsWritableString(__pyx_v_name_obj); if (unlikely((!__pyx_t_18) && PyErr_Occurred())) __PYX_ERR(0, 170, __pyx_L1_error)
   __pyx_v_name = __pyx_t_18;
 
-  /* "av/container/output.pyx":167
+  /* "av/container/output.pyx":171
  *         cdef bytes name_obj = os.fsencode(self.name if self.file is None else "")
  *         cdef char *name = name_obj
  *         if self.ptr.pb == NULL and not self.ptr.oformat.flags & lib.AVFMT_NOFILE:             # <<<<<<<<<<<<<<
  *             err_check(lib.avio_open(&self.ptr.pb, name, lib.AVIO_FLAG_WRITE))
  * 
  */
   __pyx_t_8 = ((__pyx_v_self->__pyx_base.ptr->pb == NULL) != 0);
@@ -4105,84 +4206,84 @@
     goto __pyx_L15_bool_binop_done;
   }
   __pyx_t_8 = ((!((__pyx_v_self->__pyx_base.ptr->oformat->flags & AVFMT_NOFILE) != 0)) != 0);
   __pyx_t_5 = __pyx_t_8;
   __pyx_L15_bool_binop_done:;
   if (__pyx_t_5) {
 
-    /* "av/container/output.pyx":168
+    /* "av/container/output.pyx":172
  *         cdef char *name = name_obj
  *         if self.ptr.pb == NULL and not self.ptr.oformat.flags & lib.AVFMT_NOFILE:
  *             err_check(lib.avio_open(&self.ptr.pb, name, lib.AVIO_FLAG_WRITE))             # <<<<<<<<<<<<<<
  * 
  *         # Copy the metadata dict.
  */
-    __pyx_t_15 = __pyx_f_2av_5error_err_check(avio_open((&__pyx_v_self->__pyx_base.ptr->pb), __pyx_v_name, AVIO_FLAG_WRITE), 0, NULL); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 168, __pyx_L1_error)
+    __pyx_t_15 = __pyx_f_2av_5error_err_check(avio_open((&__pyx_v_self->__pyx_base.ptr->pb), __pyx_v_name, AVIO_FLAG_WRITE), 0, NULL); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 172, __pyx_L1_error)
 
-    /* "av/container/output.pyx":167
+    /* "av/container/output.pyx":171
  *         cdef bytes name_obj = os.fsencode(self.name if self.file is None else "")
  *         cdef char *name = name_obj
  *         if self.ptr.pb == NULL and not self.ptr.oformat.flags & lib.AVFMT_NOFILE:             # <<<<<<<<<<<<<<
  *             err_check(lib.avio_open(&self.ptr.pb, name, lib.AVIO_FLAG_WRITE))
  * 
  */
   }
 
-  /* "av/container/output.pyx":172
+  /* "av/container/output.pyx":176
  *         # Copy the metadata dict.
  *         dict_to_avdict(
  *             &self.ptr.metadata, self.metadata,             # <<<<<<<<<<<<<<
  *             encoding=self.metadata_encoding,
  *             errors=self.metadata_errors
  */
   __pyx_t_1 = __pyx_v_self->__pyx_base.metadata;
   __Pyx_INCREF(__pyx_t_1);
 
-  /* "av/container/output.pyx":173
+  /* "av/container/output.pyx":177
  *         dict_to_avdict(
  *             &self.ptr.metadata, self.metadata,
  *             encoding=self.metadata_encoding,             # <<<<<<<<<<<<<<
  *             errors=self.metadata_errors
  *         )
  */
   __pyx_t_2 = __pyx_v_self->__pyx_base.metadata_encoding;
   __Pyx_INCREF(__pyx_t_2);
 
-  /* "av/container/output.pyx":174
+  /* "av/container/output.pyx":178
  *             &self.ptr.metadata, self.metadata,
  *             encoding=self.metadata_encoding,
  *             errors=self.metadata_errors             # <<<<<<<<<<<<<<
  *         )
  * 
  */
   __pyx_t_3 = __pyx_v_self->__pyx_base.metadata_errors;
   __Pyx_INCREF(__pyx_t_3);
 
-  /* "av/container/output.pyx":171
+  /* "av/container/output.pyx":175
  * 
  *         # Copy the metadata dict.
  *         dict_to_avdict(             # <<<<<<<<<<<<<<
  *             &self.ptr.metadata, self.metadata,
  *             encoding=self.metadata_encoding,
  */
-  __pyx_t_11 = __pyx_f_2av_5utils_dict_to_avdict((&__pyx_v_self->__pyx_base.ptr->metadata), ((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), ((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 171, __pyx_L1_error)
+  __pyx_t_11 = __pyx_f_2av_5utils_dict_to_avdict((&__pyx_v_self->__pyx_base.ptr->metadata), ((PyObject*)__pyx_t_1), ((PyObject*)__pyx_t_2), ((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 175, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-  /* "av/container/output.pyx":177
+  /* "av/container/output.pyx":181
  *         )
  * 
  *         cdef _Dictionary all_options = Dictionary(self.options, self.container_options)             # <<<<<<<<<<<<<<
  *         cdef _Dictionary options = all_options.copy()
  *         self.err_check(lib.avformat_write_header(
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 177, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Dictionary); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   __pyx_t_15 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4191,267 +4292,267 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_15 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_self->__pyx_base.options, __pyx_v_self->__pyx_base.container_options};
-    __pyx_t_11 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_11);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_self->__pyx_base.options, __pyx_v_self->__pyx_base.container_options};
-    __pyx_t_11 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_15, 2+__pyx_t_15); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_11);
   } else
   #endif
   {
-    __pyx_t_1 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2+__pyx_t_15); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_self->__pyx_base.options);
     __Pyx_GIVEREF(__pyx_v_self->__pyx_base.options);
     PyTuple_SET_ITEM(__pyx_t_1, 0+__pyx_t_15, __pyx_v_self->__pyx_base.options);
     __Pyx_INCREF(__pyx_v_self->__pyx_base.container_options);
     __Pyx_GIVEREF(__pyx_v_self->__pyx_base.container_options);
     PyTuple_SET_ITEM(__pyx_t_1, 1+__pyx_t_15, __pyx_v_self->__pyx_base.container_options);
-    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_1, NULL); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 181, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 177, __pyx_L1_error)
+  if (!(likely(((__pyx_t_11) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_11, __pyx_ptype_2av_10dictionary__Dictionary))))) __PYX_ERR(0, 181, __pyx_L1_error)
   __pyx_v_all_options = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "av/container/output.pyx":178
+  /* "av/container/output.pyx":182
  * 
  *         cdef _Dictionary all_options = Dictionary(self.options, self.container_options)
  *         cdef _Dictionary options = all_options.copy()             # <<<<<<<<<<<<<<
  *         self.err_check(lib.avformat_write_header(
  *             self.ptr,
  */
-  __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_2av_10dictionary__Dictionary *)__pyx_v_all_options->__pyx_vtab)->copy(__pyx_v_all_options, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 178, __pyx_L1_error)
+  __pyx_t_11 = ((PyObject *)((struct __pyx_vtabstruct_2av_10dictionary__Dictionary *)__pyx_v_all_options->__pyx_vtab)->copy(__pyx_v_all_options, 0)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __pyx_v_options = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "av/container/output.pyx":179
+  /* "av/container/output.pyx":183
  *         cdef _Dictionary all_options = Dictionary(self.options, self.container_options)
  *         cdef _Dictionary options = all_options.copy()
  *         self.err_check(lib.avformat_write_header(             # <<<<<<<<<<<<<<
  *             self.ptr,
  *             &options.ptr
  */
-  __pyx_t_15 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), avformat_write_header(__pyx_v_self->__pyx_base.ptr, (&__pyx_v_options->ptr))); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 179, __pyx_L1_error)
+  __pyx_t_15 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), avformat_write_header(__pyx_v_self->__pyx_base.ptr, (&__pyx_v_options->ptr))); if (unlikely(__pyx_t_15 == ((int)-1))) __PYX_ERR(0, 183, __pyx_L1_error)
 
-  /* "av/container/output.pyx":185
+  /* "av/container/output.pyx":189
  * 
  *         # Track option usage...
  *         for k in all_options:             # <<<<<<<<<<<<<<
  *             if k not in options:
  *                 used_options.add(k)
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_all_options))) || PyTuple_CheckExact(((PyObject *)__pyx_v_all_options))) {
     __pyx_t_11 = ((PyObject *)__pyx_v_all_options); __Pyx_INCREF(__pyx_t_11); __pyx_t_6 = 0;
     __pyx_t_7 = NULL;
   } else {
-    __pyx_t_6 = -1; __pyx_t_11 = PyObject_GetIter(((PyObject *)__pyx_v_all_options)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_6 = -1; __pyx_t_11 = PyObject_GetIter(((PyObject *)__pyx_v_all_options)); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
-    __pyx_t_7 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_7 = Py_TYPE(__pyx_t_11)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 189, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_7)) {
       if (likely(PyList_CheckExact(__pyx_t_11))) {
         if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_11)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_11, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_11, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_11, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_11)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_11, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_11, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 185, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_11, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_7(__pyx_t_11);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 185, __pyx_L1_error)
+          else __PYX_ERR(0, 189, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "av/container/output.pyx":186
+    /* "av/container/output.pyx":190
  *         # Track option usage...
  *         for k in all_options:
  *             if k not in options:             # <<<<<<<<<<<<<<
  *                 used_options.add(k)
  *         # ... and warn if any weren't used.
  */
-    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_k, ((PyObject *)__pyx_v_options), Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_v_k, ((PyObject *)__pyx_v_options), Py_NE)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
     __pyx_t_8 = (__pyx_t_5 != 0);
     if (__pyx_t_8) {
 
-      /* "av/container/output.pyx":187
+      /* "av/container/output.pyx":191
  *         for k in all_options:
  *             if k not in options:
  *                 used_options.add(k)             # <<<<<<<<<<<<<<
  *         # ... and warn if any weren't used.
  *         unused_options = {k: v for k, v in self.options.items() if k not in used_options}
  */
-      __pyx_t_17 = PySet_Add(__pyx_v_used_options, __pyx_v_k); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 187, __pyx_L1_error)
+      __pyx_t_17 = PySet_Add(__pyx_v_used_options, __pyx_v_k); if (unlikely(__pyx_t_17 == ((int)-1))) __PYX_ERR(0, 191, __pyx_L1_error)
 
-      /* "av/container/output.pyx":186
+      /* "av/container/output.pyx":190
  *         # Track option usage...
  *         for k in all_options:
  *             if k not in options:             # <<<<<<<<<<<<<<
  *                 used_options.add(k)
  *         # ... and warn if any weren't used.
  */
     }
 
-    /* "av/container/output.pyx":185
+    /* "av/container/output.pyx":189
  * 
  *         # Track option usage...
  *         for k in all_options:             # <<<<<<<<<<<<<<
  *             if k not in options:
  *                 used_options.add(k)
  */
   }
   __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-  /* "av/container/output.pyx":189
+  /* "av/container/output.pyx":193
  *                 used_options.add(k)
  *         # ... and warn if any weren't used.
  *         unused_options = {k: v for k, v in self.options.items() if k not in used_options}             # <<<<<<<<<<<<<<
  *         if unused_options:
  *             log.warning('Some options were not used: %s' % unused_options)
  */
   { /* enter inner scope */
-    __pyx_t_11 = PyDict_New(); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 189, __pyx_L22_error)
+    __pyx_t_11 = PyDict_New(); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 193, __pyx_L22_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (unlikely(__pyx_v_self->__pyx_base.options == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "items");
-      __PYX_ERR(0, 189, __pyx_L22_error)
+      __PYX_ERR(0, 193, __pyx_L22_error)
     }
-    __pyx_t_3 = __Pyx_PyDict_Items(__pyx_v_self->__pyx_base.options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L22_error)
+    __pyx_t_3 = __Pyx_PyDict_Items(__pyx_v_self->__pyx_base.options); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L22_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_1 = __pyx_t_3; __Pyx_INCREF(__pyx_t_1); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L22_error)
+      __pyx_t_6 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L22_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 189, __pyx_L22_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 193, __pyx_L22_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_1))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 189, __pyx_L22_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 193, __pyx_L22_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L22_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L22_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 189, __pyx_L22_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_6); __Pyx_INCREF(__pyx_t_3); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 193, __pyx_L22_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 189, __pyx_L22_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_1, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 193, __pyx_L22_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_7(__pyx_t_1);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 189, __pyx_L22_error)
+            else __PYX_ERR(0, 193, __pyx_L22_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
         PyObject* sequence = __pyx_t_3;
         Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
         if (unlikely(size != 2)) {
           if (size > 2) __Pyx_RaiseTooManyValuesError(2);
           else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-          __PYX_ERR(0, 189, __pyx_L22_error)
+          __PYX_ERR(0, 193, __pyx_L22_error)
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
         if (likely(PyTuple_CheckExact(sequence))) {
           __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
         } else {
           __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
           __pyx_t_4 = PyList_GET_ITEM(sequence, 1); 
         }
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         #else
-        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L22_error)
+        __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L22_error)
+        __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       } else {
         Py_ssize_t index = -1;
-        __pyx_t_12 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 189, __pyx_L22_error)
+        __pyx_t_12 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 193, __pyx_L22_error)
         __Pyx_GOTREF(__pyx_t_12);
         __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         __pyx_t_13 = Py_TYPE(__pyx_t_12)->tp_iternext;
         index = 0; __pyx_t_2 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_2)) goto __pyx_L25_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_2);
         index = 1; __pyx_t_4 = __pyx_t_13(__pyx_t_12); if (unlikely(!__pyx_t_4)) goto __pyx_L25_unpacking_failed;
         __Pyx_GOTREF(__pyx_t_4);
-        if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 189, __pyx_L22_error)
+        if (__Pyx_IternextUnpackEndCheck(__pyx_t_13(__pyx_t_12), 2) < 0) __PYX_ERR(0, 193, __pyx_L22_error)
         __pyx_t_13 = NULL;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         goto __pyx_L26_unpacking_done;
         __pyx_L25_unpacking_failed:;
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __pyx_t_13 = NULL;
         if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-        __PYX_ERR(0, 189, __pyx_L22_error)
+        __PYX_ERR(0, 193, __pyx_L22_error)
         __pyx_L26_unpacking_done:;
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_k, __pyx_t_2);
       __pyx_t_2 = 0;
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_v, __pyx_t_4);
       __pyx_t_4 = 0;
-      __pyx_t_8 = (__Pyx_PySet_ContainsTF(__pyx_7genexpr__pyx_v_k, __pyx_v_used_options, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 189, __pyx_L22_error)
+      __pyx_t_8 = (__Pyx_PySet_ContainsTF(__pyx_7genexpr__pyx_v_k, __pyx_v_used_options, Py_NE)); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 193, __pyx_L22_error)
       __pyx_t_5 = (__pyx_t_8 != 0);
       if (__pyx_t_5) {
-        if (unlikely(PyDict_SetItem(__pyx_t_11, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 189, __pyx_L22_error)
+        if (unlikely(PyDict_SetItem(__pyx_t_11, (PyObject*)__pyx_7genexpr__pyx_v_k, (PyObject*)__pyx_7genexpr__pyx_v_v))) __PYX_ERR(0, 193, __pyx_L22_error)
       }
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_k); __pyx_7genexpr__pyx_v_k = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L28_exit_scope;
     __pyx_L22_error:;
@@ -4459,75 +4560,75 @@
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_v); __pyx_7genexpr__pyx_v_v = 0;
     goto __pyx_L1_error;
     __pyx_L28_exit_scope:;
   } /* exit inner scope */
   __pyx_v_unused_options = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
 
-  /* "av/container/output.pyx":190
+  /* "av/container/output.pyx":194
  *         # ... and warn if any weren't used.
  *         unused_options = {k: v for k, v in self.options.items() if k not in used_options}
  *         if unused_options:             # <<<<<<<<<<<<<<
  *             log.warning('Some options were not used: %s' % unused_options)
  * 
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_unused_options); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_unused_options); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 194, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "av/container/output.pyx":191
+    /* "av/container/output.pyx":195
  *         unused_options = {k: v for k, v in self.options.items() if k not in used_options}
  *         if unused_options:
  *             log.warning('Some options were not used: %s' % unused_options)             # <<<<<<<<<<<<<<
  * 
  *         self._started = True
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_log); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_warning); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Some_options_were_not_used_s, __pyx_v_unused_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Some_options_were_not_used_s, __pyx_v_unused_options); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_11 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_1);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 191, __pyx_L1_error)
+    if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 195, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
 
-    /* "av/container/output.pyx":190
+    /* "av/container/output.pyx":194
  *         # ... and warn if any weren't used.
  *         unused_options = {k: v for k, v in self.options.items() if k not in used_options}
  *         if unused_options:             # <<<<<<<<<<<<<<
  *             log.warning('Some options were not used: %s' % unused_options)
  * 
  */
   }
 
-  /* "av/container/output.pyx":193
+  /* "av/container/output.pyx":197
  *             log.warning('Some options were not used: %s' % unused_options)
  * 
  *         self._started = True             # <<<<<<<<<<<<<<
  * 
  *     def close(self):
  */
   __pyx_v_self->_started = 1;
 
-  /* "av/container/output.pyx":136
+  /* "av/container/output.pyx":140
  *         return py_stream
  * 
  *     cpdef start_encoding(self):             # <<<<<<<<<<<<<<
  *         """Write the file header! Called automatically."""
  * 
  */
 
@@ -4579,15 +4680,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("start_encoding", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_2av_9container_6output_15OutputContainer_start_encoding(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2av_9container_6output_15OutputContainer_start_encoding(__pyx_v_self, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4596,15 +4697,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/output.pyx":195
+/* "av/container/output.pyx":199
  *         self._started = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         for stream in self.streams:
  *             if stream.codec_context:
  */
 
@@ -4634,128 +4735,128 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
 
-  /* "av/container/output.pyx":196
+  /* "av/container/output.pyx":200
  * 
  *     def close(self):
  *         for stream in self.streams:             # <<<<<<<<<<<<<<
  *             if stream.codec_context:
  *                 stream.codec_context.close(strict=False)
  */
   if (likely(PyList_CheckExact(((PyObject *)__pyx_v_self->__pyx_base.streams))) || PyTuple_CheckExact(((PyObject *)__pyx_v_self->__pyx_base.streams))) {
     __pyx_t_1 = ((PyObject *)__pyx_v_self->__pyx_base.streams); __Pyx_INCREF(__pyx_t_1); __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self->__pyx_base.streams)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(((PyObject *)__pyx_v_self->__pyx_base.streams)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_1)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 200, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         if (__pyx_t_2 >= PyList_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 196, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 200, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_2 >= PyTuple_GET_SIZE(__pyx_t_1)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 196, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely(0 < 0)) __PYX_ERR(0, 200, __pyx_L1_error)
         #else
-        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+        __pyx_t_4 = PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 196, __pyx_L1_error)
+          else __PYX_ERR(0, 200, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_stream, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "av/container/output.pyx":197
+    /* "av/container/output.pyx":201
  *     def close(self):
  *         for stream in self.streams:
  *             if stream.codec_context:             # <<<<<<<<<<<<<<
  *                 stream.codec_context.close(strict=False)
  * 
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_stream, __pyx_n_s_codec_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_stream, __pyx_n_s_codec_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
 
-      /* "av/container/output.pyx":198
+      /* "av/container/output.pyx":202
  *         for stream in self.streams:
  *             if stream.codec_context:
  *                 stream.codec_context.close(strict=False)             # <<<<<<<<<<<<<<
  * 
  *         close_output(self)
  */
-      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_stream, __pyx_n_s_codec_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_stream, __pyx_n_s_codec_context); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_close); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_close); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 202, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_strict, Py_False) < 0) __PYX_ERR(0, 198, __pyx_L1_error)
-      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 198, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_strict, Py_False) < 0) __PYX_ERR(0, 202, __pyx_L1_error)
+      __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_4); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 202, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "av/container/output.pyx":197
+      /* "av/container/output.pyx":201
  *     def close(self):
  *         for stream in self.streams:
  *             if stream.codec_context:             # <<<<<<<<<<<<<<
  *                 stream.codec_context.close(strict=False)
  * 
  */
     }
 
-    /* "av/container/output.pyx":196
+    /* "av/container/output.pyx":200
  * 
  *     def close(self):
  *         for stream in self.streams:             # <<<<<<<<<<<<<<
  *             if stream.codec_context:
  *                 stream.codec_context.close(strict=False)
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":200
+  /* "av/container/output.pyx":204
  *                 stream.codec_context.close(strict=False)
  * 
  *         close_output(self)             # <<<<<<<<<<<<<<
  * 
  *     def mux(self, packets):
  */
-  __pyx_t_1 = __pyx_f_2av_9container_6output_close_output(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2av_9container_6output_close_output(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":195
+  /* "av/container/output.pyx":199
  *         self._started = True
  * 
  *     def close(self):             # <<<<<<<<<<<<<<
  *         for stream in self.streams:
  *             if stream.codec_context:
  */
 
@@ -4772,15 +4873,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_stream);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/output.pyx":202
+/* "av/container/output.pyx":206
  *         close_output(self)
  * 
  *     def mux(self, packets):             # <<<<<<<<<<<<<<
  *         # We accept either a Packet, or a sequence of packets. This should
  *         # smooth out the transition to the new encode API which returns a
  */
 
@@ -4811,150 +4912,150 @@
   PyObject *(*__pyx_t_7)(PyObject *);
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mux", 0);
 
-  /* "av/container/output.pyx":206
+  /* "av/container/output.pyx":210
  *         # smooth out the transition to the new encode API which returns a
  *         # sequence of packets.
  *         if isinstance(packets, Packet):             # <<<<<<<<<<<<<<
  *             self.mux_one(packets)
  *         else:
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_packets, __pyx_ptype_2av_6packet_Packet); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/container/output.pyx":207
+    /* "av/container/output.pyx":211
  *         # sequence of packets.
  *         if isinstance(packets, Packet):
  *             self.mux_one(packets)             # <<<<<<<<<<<<<<
  *         else:
  *             for packet in packets:
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mux_one); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mux_one); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_v_packets) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_v_packets);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 207, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "av/container/output.pyx":206
+    /* "av/container/output.pyx":210
  *         # smooth out the transition to the new encode API which returns a
  *         # sequence of packets.
  *         if isinstance(packets, Packet):             # <<<<<<<<<<<<<<
  *             self.mux_one(packets)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "av/container/output.pyx":209
+  /* "av/container/output.pyx":213
  *             self.mux_one(packets)
  *         else:
  *             for packet in packets:             # <<<<<<<<<<<<<<
  *                 self.mux_one(packet)
  * 
  */
   /*else*/ {
     if (likely(PyList_CheckExact(__pyx_v_packets)) || PyTuple_CheckExact(__pyx_v_packets)) {
       __pyx_t_3 = __pyx_v_packets; __Pyx_INCREF(__pyx_t_3); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
     } else {
-      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_packets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 209, __pyx_L1_error)
+      __pyx_t_6 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_packets); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 209, __pyx_L1_error)
+      __pyx_t_7 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 213, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_7)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_6 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
+          __pyx_t_4 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 213, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         } else {
           if (__pyx_t_6 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
+          __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_6); __Pyx_INCREF(__pyx_t_4); __pyx_t_6++; if (unlikely(0 < 0)) __PYX_ERR(0, 213, __pyx_L1_error)
           #else
-          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+          __pyx_t_4 = PySequence_ITEM(__pyx_t_3, __pyx_t_6); __pyx_t_6++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_4);
           #endif
         }
       } else {
         __pyx_t_4 = __pyx_t_7(__pyx_t_3);
         if (unlikely(!__pyx_t_4)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 209, __pyx_L1_error)
+            else __PYX_ERR(0, 213, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_4);
       }
       __Pyx_XDECREF_SET(__pyx_v_packet, __pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/output.pyx":210
+      /* "av/container/output.pyx":214
  *         else:
  *             for packet in packets:
  *                 self.mux_one(packet)             # <<<<<<<<<<<<<<
  * 
  *     def mux_one(self, Packet packet not None):
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mux_one); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 210, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_mux_one); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 214, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_8, __pyx_v_packet) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_packet);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "av/container/output.pyx":209
+      /* "av/container/output.pyx":213
  *             self.mux_one(packets)
  *         else:
  *             for packet in packets:             # <<<<<<<<<<<<<<
  *                 self.mux_one(packet)
  * 
  */
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "av/container/output.pyx":202
+  /* "av/container/output.pyx":206
  *         close_output(self)
  * 
  *     def mux(self, packets):             # <<<<<<<<<<<<<<
  *         # We accept either a Packet, or a sequence of packets. This should
  *         # smooth out the transition to the new encode API which returns a
  */
 
@@ -4971,15 +5072,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_packet);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/output.pyx":212
+/* "av/container/output.pyx":216
  *                 self.mux_one(packet)
  * 
  *     def mux_one(self, Packet packet not None):             # <<<<<<<<<<<<<<
  *         self.start_encoding()
  * 
  */
 
@@ -4989,53 +5090,52 @@
 static PyObject *__pyx_pw_2av_9container_6output_15OutputContainer_13mux_one(PyObject *__pyx_v_self, PyObject *__pyx_v_packet) {
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("mux_one (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_packet), __pyx_ptype_2av_6packet_Packet, 0, "packet", 0))) __PYX_ERR(0, 212, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_packet), __pyx_ptype_2av_6packet_Packet, 0, "packet", 0))) __PYX_ERR(0, 216, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_9container_6output_15OutputContainer_12mux_one(((struct __pyx_obj_2av_9container_6output_OutputContainer *)__pyx_v_self), ((struct __pyx_obj_2av_6packet_Packet *)__pyx_v_packet));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_2av_9container_6output_15OutputContainer_12mux_one(struct __pyx_obj_2av_9container_6output_OutputContainer *__pyx_v_self, struct __pyx_obj_2av_6packet_Packet *__pyx_v_packet) {
   struct AVStream *__pyx_v_stream;
-  struct AVPacket *__pyx_v_packet_ptr;
   int __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("mux_one", 0);
 
-  /* "av/container/output.pyx":213
+  /* "av/container/output.pyx":217
  * 
  *     def mux_one(self, Packet packet not None):
  *         self.start_encoding()             # <<<<<<<<<<<<<<
  * 
  *         # Assert the packet is in stream time.
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->start_encoding(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->start_encoding(__pyx_v_self, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":216
+  /* "av/container/output.pyx":220
  * 
  *         # Assert the packet is in stream time.
  *         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:             # <<<<<<<<<<<<<<
  *             raise ValueError('Bad Packet stream_index.')
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
  */
   __pyx_t_3 = ((__pyx_v_packet->ptr->stream_index < 0) != 0);
@@ -5045,125 +5145,116 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_3 = ((((unsigned int)__pyx_v_packet->ptr->stream_index) >= __pyx_v_self->__pyx_base.ptr->nb_streams) != 0);
   __pyx_t_2 = __pyx_t_3;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/container/output.pyx":217
+    /* "av/container/output.pyx":221
  *         # Assert the packet is in stream time.
  *         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:
  *             raise ValueError('Bad Packet stream_index.')             # <<<<<<<<<<<<<<
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
  *         packet._rebase_time(stream.time_base)
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 217, __pyx_L1_error)
+    __PYX_ERR(0, 221, __pyx_L1_error)
 
-    /* "av/container/output.pyx":216
+    /* "av/container/output.pyx":220
  * 
  *         # Assert the packet is in stream time.
  *         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:             # <<<<<<<<<<<<<<
  *             raise ValueError('Bad Packet stream_index.')
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
  */
   }
 
-  /* "av/container/output.pyx":218
+  /* "av/container/output.pyx":222
  *         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:
  *             raise ValueError('Bad Packet stream_index.')
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]             # <<<<<<<<<<<<<<
  *         packet._rebase_time(stream.time_base)
  * 
  */
   __pyx_v_stream = (__pyx_v_self->__pyx_base.ptr->streams[__pyx_v_packet->ptr->stream_index]);
 
-  /* "av/container/output.pyx":219
+  /* "av/container/output.pyx":223
  *             raise ValueError('Bad Packet stream_index.')
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
  *         packet._rebase_time(stream.time_base)             # <<<<<<<<<<<<<<
  * 
  *         # Make another reference to the packet, as av_interleaved_write_frame
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_6packet_Packet *)__pyx_v_packet->__pyx_base.__pyx_vtab)->_rebase_time(__pyx_v_packet, __pyx_v_stream->time_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_2av_6packet_Packet *)__pyx_v_packet->__pyx_base.__pyx_vtab)->_rebase_time(__pyx_v_packet, __pyx_v_stream->time_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "av/container/output.pyx":223
+  /* "av/container/output.pyx":227
  *         # Make another reference to the packet, as av_interleaved_write_frame
- *         # takes ownership of it.
- *         cdef lib.AVPacket *packet_ptr = lib.av_packet_alloc()             # <<<<<<<<<<<<<<
- *         self.err_check(lib.av_packet_ref(packet_ptr, packet.ptr))
- * 
- */
-  __pyx_v_packet_ptr = av_packet_alloc();
-
-  /* "av/container/output.pyx":224
- *         # takes ownership of it.
- *         cdef lib.AVPacket *packet_ptr = lib.av_packet_alloc()
- *         self.err_check(lib.av_packet_ref(packet_ptr, packet.ptr))             # <<<<<<<<<<<<<<
+ *         # takes ownership of the reference.
+ *         self.err_check(lib.av_packet_ref(self.packet_ptr, packet.ptr))             # <<<<<<<<<<<<<<
  * 
  *         cdef int ret
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), av_packet_ref(__pyx_v_packet_ptr, __pyx_v_packet->ptr)); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 224, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), av_packet_ref(__pyx_v_self->packet_ptr, __pyx_v_packet->ptr)); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 227, __pyx_L1_error)
 
-  /* "av/container/output.pyx":227
+  /* "av/container/output.pyx":230
  * 
  *         cdef int ret
  *         with nogil:             # <<<<<<<<<<<<<<
- *             ret = lib.av_interleaved_write_frame(self.ptr, packet_ptr)
+ *             ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)
  *         self.err_check(ret)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/container/output.pyx":228
+        /* "av/container/output.pyx":231
  *         cdef int ret
  *         with nogil:
- *             ret = lib.av_interleaved_write_frame(self.ptr, packet_ptr)             # <<<<<<<<<<<<<<
+ *             ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)             # <<<<<<<<<<<<<<
  *         self.err_check(ret)
  */
-        __pyx_v_ret = av_interleaved_write_frame(__pyx_v_self->__pyx_base.ptr, __pyx_v_packet_ptr);
+        __pyx_v_ret = av_interleaved_write_frame(__pyx_v_self->__pyx_base.ptr, __pyx_v_self->packet_ptr);
       }
 
-      /* "av/container/output.pyx":227
+      /* "av/container/output.pyx":230
  * 
  *         cdef int ret
  *         with nogil:             # <<<<<<<<<<<<<<
- *             ret = lib.av_interleaved_write_frame(self.ptr, packet_ptr)
+ *             ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)
  *         self.err_check(ret)
  */
       /*finally:*/ {
         /*normal exit:*/{
           #ifdef WITH_THREAD
           __Pyx_FastGIL_Forget();
           Py_BLOCK_THREADS
           #endif
           goto __pyx_L8;
         }
         __pyx_L8:;
       }
   }
 
-  /* "av/container/output.pyx":229
+  /* "av/container/output.pyx":232
  *         with nogil:
- *             ret = lib.av_interleaved_write_frame(self.ptr, packet_ptr)
+ *             ret = lib.av_interleaved_write_frame(self.ptr, self.packet_ptr)
  *         self.err_check(ret)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_ret); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 229, __pyx_L1_error)
+  __pyx_t_4 = ((struct __pyx_vtabstruct_2av_9container_6output_OutputContainer *)__pyx_v_self->__pyx_base.__pyx_vtab)->__pyx_base.err_check(((struct __pyx_obj_2av_9container_4core_Container *)__pyx_v_self), __pyx_v_ret); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 232, __pyx_L1_error)
 
-  /* "av/container/output.pyx":212
+  /* "av/container/output.pyx":216
  *                 self.mux_one(packet)
  * 
  *     def mux_one(self, Packet packet not None):             # <<<<<<<<<<<<<<
  *         self.start_encoding()
  * 
  */
 
@@ -5516,66 +5607,66 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
   {&__pyx_n_s_warning, __pyx_k_warning, sizeof(__pyx_k_warning), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/container/output.pyx":56
+  /* "av/container/output.pyx":60
  * 
  *         if (codec_name is None and template is None) or (codec_name is not None and template is not None):
  *             raise ValueError('needs one of codec_name or template')             # <<<<<<<<<<<<<<
  * 
  *         cdef const lib.AVCodec *codec
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_needs_one_of_codec_name_or_templ); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 56, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_needs_one_of_codec_name_or_templ); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 60, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "av/container/output.pyx":67
+  /* "av/container/output.pyx":71
  *         else:
  *             if not template._codec:
  *                 raise ValueError("template has no codec")             # <<<<<<<<<<<<<<
  *             if not template._codec_context:
  *                 raise ValueError("template has no codec context")
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_template_has_no_codec); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_template_has_no_codec); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 71, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "av/container/output.pyx":69
+  /* "av/container/output.pyx":73
  *                 raise ValueError("template has no codec")
  *             if not template._codec_context:
  *                 raise ValueError("template has no codec context")             # <<<<<<<<<<<<<<
  *             codec = template._codec
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_template_has_no_codec_context); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 69, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_template_has_no_codec_context); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 73, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "av/container/output.pyx":217
+  /* "av/container/output.pyx":221
  *         # Assert the packet is in stream time.
  *         if packet.ptr.stream_index < 0 or <unsigned int>packet.ptr.stream_index >= self.ptr.nb_streams:
  *             raise ValueError('Bad Packet stream_index.')             # <<<<<<<<<<<<<<
  *         cdef lib.AVStream *stream = self.ptr.streams[packet.ptr.stream_index]
  *         packet._rebase_time(stream.time_base)
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Bad_Packet_stream_index); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 217, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_Bad_Packet_stream_index); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 221, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -5682,18 +5773,18 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(2, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(2, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.bytesource"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_10bytesource_ByteSource = __Pyx_ImportType(__pyx_t_1, "av.bytesource", "ByteSource", sizeof(struct __pyx_obj_2av_10bytesource_ByteSource), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_10bytesource_ByteSource) __PYX_ERR(3, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.codec"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 4, __pyx_L1_error)
```

### Comparing `av-9.1.1/src/av/container/pyio.c` & `av-9.2.0/src/av/container/pyio.c`

 * *Files 2% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1028,28 +1036,29 @@
  * 
  * ctypedef int64_t (*seek_func_t)(void *opaque, int64_t offset, int whence) nogil             # <<<<<<<<<<<<<<
  * 
  * 
  */
 typedef int64_t (*__pyx_t_2av_9container_4pyio_seek_func_t)(void *, int64_t, int);
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1429,14 +1438,15 @@
 static const char __pyx_k_file[] = "file";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_read[] = "read";
 static const char __pyx_k_seek[] = "seek";
 static const char __pyx_k_tell[] = "tell";
 static const char __pyx_k_test[] = "__test__";
+static const char __pyx_k_close[] = "close";
 static const char __pyx_k_write[] = "write";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_PyIOFile[] = "PyIOFile";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_readable[] = "readable";
 static const char __pyx_k_seekable[] = "seekable";
 static const char __pyx_k_setstate[] = "__setstate__";
@@ -1455,14 +1465,15 @@
 static PyObject *__pyx_kp_s_File_object_has_no_read_method_o;
 static PyObject *__pyx_kp_s_File_object_has_no_write_method;
 static PyObject *__pyx_n_s_PyIOFile;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_buffer_size;
 static PyObject *__pyx_n_s_cline_in_traceback;
+static PyObject *__pyx_n_s_close;
 static PyObject *__pyx_n_s_file;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_read;
 static PyObject *__pyx_n_s_readable;
@@ -1703,15 +1714,15 @@
   __pyx_t_2 = 0;
 
   /* "av/container/pyio.pyx":23
  *         self.fread = getattr(self.file, 'read', None)
  *         self.fwrite = getattr(self.file, 'write', None)
  *         self.fseek = getattr(self.file, 'seek', None)             # <<<<<<<<<<<<<<
  *         self.ftell = getattr(self.file, 'tell', None)
- * 
+ *         self.fclose = getattr(self.file, 'close', None)
  */
   __pyx_t_2 = __pyx_v_self->file;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_GetAttr3(__pyx_t_2, __pyx_n_s_seek, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
@@ -1720,164 +1731,182 @@
   __pyx_v_self->fseek = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "av/container/pyio.pyx":24
  *         self.fwrite = getattr(self.file, 'write', None)
  *         self.fseek = getattr(self.file, 'seek', None)
  *         self.ftell = getattr(self.file, 'tell', None)             # <<<<<<<<<<<<<<
+ *         self.fclose = getattr(self.file, 'close', None)
  * 
- *         # To be seekable the file object must have `seek` and `tell` methods.
  */
   __pyx_t_1 = __pyx_v_self->file;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_GetAttr3(__pyx_t_1, __pyx_n_s_tell, Py_None); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->ftell);
   __Pyx_DECREF(__pyx_v_self->ftell);
   __pyx_v_self->ftell = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "av/container/pyio.pyx":29
+  /* "av/container/pyio.pyx":25
+ *         self.fseek = getattr(self.file, 'seek', None)
+ *         self.ftell = getattr(self.file, 'tell', None)
+ *         self.fclose = getattr(self.file, 'close', None)             # <<<<<<<<<<<<<<
+ * 
+ *         # To be seekable the file object must have `seek` and `tell` methods.
+ */
+  __pyx_t_2 = __pyx_v_self->file;
+  __Pyx_INCREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_GetAttr3(__pyx_t_2, __pyx_n_s_close, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_GIVEREF(__pyx_t_1);
+  __Pyx_GOTREF(__pyx_v_self->fclose);
+  __Pyx_DECREF(__pyx_v_self->fclose);
+  __pyx_v_self->fclose = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "av/container/pyio.pyx":30
  *         # If it also has a `seekable` method, it must return True.
  *         if (
  *             self.fseek is not None             # <<<<<<<<<<<<<<
  *             and self.ftell is not None
  *             and (seekable is None or seekable())
  */
   __pyx_t_4 = (__pyx_v_self->fseek != Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "av/container/pyio.pyx":30
+  /* "av/container/pyio.pyx":31
  *         if (
  *             self.fseek is not None
  *             and self.ftell is not None             # <<<<<<<<<<<<<<
  *             and (seekable is None or seekable())
  *         ):
  */
   __pyx_t_5 = (__pyx_v_self->ftell != Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (__pyx_t_4) {
   } else {
     __pyx_t_3 = __pyx_t_4;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "av/container/pyio.pyx":31
+  /* "av/container/pyio.pyx":32
  *             self.fseek is not None
  *             and self.ftell is not None
  *             and (seekable is None or seekable())             # <<<<<<<<<<<<<<
  *         ):
  *             seek_func = pyio_seek
  */
   __pyx_t_4 = (__pyx_v_seekable == Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (!__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
   __Pyx_INCREF(__pyx_v_seekable);
-  __pyx_t_1 = __pyx_v_seekable; __pyx_t_6 = NULL;
-  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+  __pyx_t_2 = __pyx_v_seekable; __pyx_t_6 = NULL;
+  if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_6)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_6);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+  __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 31, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 32, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
 
-  /* "av/container/pyio.pyx":28
+  /* "av/container/pyio.pyx":29
  *         # To be seekable the file object must have `seek` and `tell` methods.
  *         # If it also has a `seekable` method, it must return True.
  *         if (             # <<<<<<<<<<<<<<
  *             self.fseek is not None
  *             and self.ftell is not None
  */
   if (__pyx_t_3) {
 
-    /* "av/container/pyio.pyx":33
+    /* "av/container/pyio.pyx":34
  *             and (seekable is None or seekable())
  *         ):
  *             seek_func = pyio_seek             # <<<<<<<<<<<<<<
  * 
  *         if writeable is None:
  */
     __pyx_v_seek_func = __pyx_f_2av_9container_4pyio_pyio_seek;
 
-    /* "av/container/pyio.pyx":28
+    /* "av/container/pyio.pyx":29
  *         # To be seekable the file object must have `seek` and `tell` methods.
  *         # If it also has a `seekable` method, it must return True.
  *         if (             # <<<<<<<<<<<<<<
  *             self.fseek is not None
  *             and self.ftell is not None
  */
   }
 
-  /* "av/container/pyio.pyx":35
+  /* "av/container/pyio.pyx":36
  *             seek_func = pyio_seek
  * 
  *         if writeable is None:             # <<<<<<<<<<<<<<
  *             writeable = self.fwrite is not None
  * 
  */
   __pyx_t_3 = (__pyx_v_writeable == Py_None);
   __pyx_t_5 = (__pyx_t_3 != 0);
   if (__pyx_t_5) {
 
-    /* "av/container/pyio.pyx":36
+    /* "av/container/pyio.pyx":37
  * 
  *         if writeable is None:
  *             writeable = self.fwrite is not None             # <<<<<<<<<<<<<<
  * 
  *         if writeable:
  */
     __pyx_t_5 = (__pyx_v_self->fwrite != Py_None);
-    __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_5); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF_SET(__pyx_v_writeable, __pyx_t_2);
-    __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF_SET(__pyx_v_writeable, __pyx_t_1);
+    __pyx_t_1 = 0;
 
-    /* "av/container/pyio.pyx":35
+    /* "av/container/pyio.pyx":36
  *             seek_func = pyio_seek
  * 
  *         if writeable is None:             # <<<<<<<<<<<<<<
  *             writeable = self.fwrite is not None
  * 
  */
   }
 
-  /* "av/container/pyio.pyx":38
+  /* "av/container/pyio.pyx":39
  *             writeable = self.fwrite is not None
  * 
  *         if writeable:             # <<<<<<<<<<<<<<
  *             if self.fwrite is None or (writable is not None and not writable()):
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  */
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_writeable); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 38, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_v_writeable); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
   if (__pyx_t_5) {
 
-    /* "av/container/pyio.pyx":39
+    /* "av/container/pyio.pyx":40
  * 
  *         if writeable:
  *             if self.fwrite is None or (writable is not None and not writable()):             # <<<<<<<<<<<<<<
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  *         else:
  */
     __pyx_t_3 = (__pyx_v_self->fwrite == Py_None);
@@ -1891,69 +1920,69 @@
     __pyx_t_3 = (__pyx_t_4 != 0);
     if (__pyx_t_3) {
     } else {
       __pyx_t_5 = __pyx_t_3;
       goto __pyx_L11_bool_binop_done;
     }
     __Pyx_INCREF(__pyx_v_writable);
-    __pyx_t_1 = __pyx_v_writable; __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+    __pyx_t_2 = __pyx_v_writable; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+    __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 39, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 39, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_4 = ((!__pyx_t_3) != 0);
     __pyx_t_5 = __pyx_t_4;
     __pyx_L11_bool_binop_done:;
     if (unlikely(__pyx_t_5)) {
 
-      /* "av/container/pyio.pyx":40
+      /* "av/container/pyio.pyx":41
  *         if writeable:
  *             if self.fwrite is None or (writable is not None and not writable()):
  *                 raise ValueError("File object has no write() method, or writable() returned False.")             # <<<<<<<<<<<<<<
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 40, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __PYX_ERR(0, 41, __pyx_L1_error)
 
-      /* "av/container/pyio.pyx":39
+      /* "av/container/pyio.pyx":40
  * 
  *         if writeable:
  *             if self.fwrite is None or (writable is not None and not writable()):             # <<<<<<<<<<<<<<
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  *         else:
  */
     }
 
-    /* "av/container/pyio.pyx":38
+    /* "av/container/pyio.pyx":39
  *             writeable = self.fwrite is not None
  * 
  *         if writeable:             # <<<<<<<<<<<<<<
  *             if self.fwrite is None or (writable is not None and not writable()):
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  */
     goto __pyx_L9;
   }
 
-  /* "av/container/pyio.pyx":42
+  /* "av/container/pyio.pyx":43
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):             # <<<<<<<<<<<<<<
  *                 raise ValueError("File object has no read() method, or readable() returned False.")
  * 
  */
   /*else*/ {
@@ -1968,151 +1997,151 @@
     __pyx_t_4 = (__pyx_t_3 != 0);
     if (__pyx_t_4) {
     } else {
       __pyx_t_5 = __pyx_t_4;
       goto __pyx_L15_bool_binop_done;
     }
     __Pyx_INCREF(__pyx_v_readable);
-    __pyx_t_1 = __pyx_v_readable; __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+    __pyx_t_2 = __pyx_v_readable; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_2 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_1);
+    __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_6) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 42, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 43, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_3 = ((!__pyx_t_4) != 0);
     __pyx_t_5 = __pyx_t_3;
     __pyx_L15_bool_binop_done:;
     if (unlikely(__pyx_t_5)) {
 
-      /* "av/container/pyio.pyx":43
+      /* "av/container/pyio.pyx":44
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):
  *                 raise ValueError("File object has no read() method, or readable() returned False.")             # <<<<<<<<<<<<<<
  * 
  *         self.pos = 0
  */
-      __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 43, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_2);
-      __Pyx_Raise(__pyx_t_2, 0, 0, 0);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 43, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 44, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      __PYX_ERR(0, 44, __pyx_L1_error)
 
-      /* "av/container/pyio.pyx":42
+      /* "av/container/pyio.pyx":43
  *                 raise ValueError("File object has no write() method, or writable() returned False.")
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):             # <<<<<<<<<<<<<<
  *                 raise ValueError("File object has no read() method, or readable() returned False.")
  * 
  */
     }
   }
   __pyx_L9:;
 
-  /* "av/container/pyio.pyx":45
+  /* "av/container/pyio.pyx":46
  *                 raise ValueError("File object has no read() method, or readable() returned False.")
  * 
  *         self.pos = 0             # <<<<<<<<<<<<<<
  *         self.pos_is_valid = True
  * 
  */
   __pyx_v_self->pos = 0;
 
-  /* "av/container/pyio.pyx":46
+  /* "av/container/pyio.pyx":47
  * 
  *         self.pos = 0
  *         self.pos_is_valid = True             # <<<<<<<<<<<<<<
  * 
  *         # This is effectively the maximum size of reads.
  */
   __pyx_v_self->pos_is_valid = 1;
 
-  /* "av/container/pyio.pyx":49
+  /* "av/container/pyio.pyx":50
  * 
  *         # This is effectively the maximum size of reads.
  *         self.buffer = <unsigned char*>lib.av_malloc(buffer_size)             # <<<<<<<<<<<<<<
  * 
  *         self.iocontext = lib.avio_alloc_context(
  */
-  __pyx_t_7 = __Pyx_PyInt_As_size_t(__pyx_v_buffer_size); if (unlikely((__pyx_t_7 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_As_size_t(__pyx_v_buffer_size); if (unlikely((__pyx_t_7 == (size_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 50, __pyx_L1_error)
   __pyx_v_self->buffer = ((unsigned char *)av_malloc(__pyx_t_7));
 
-  /* "av/container/pyio.pyx":52
+  /* "av/container/pyio.pyx":53
  * 
  *         self.iocontext = lib.avio_alloc_context(
  *             self.buffer, buffer_size,             # <<<<<<<<<<<<<<
  *             writeable,
  *             <void*>self,  # User data.
  */
-  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_buffer_size); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyInt_As_int(__pyx_v_buffer_size); if (unlikely((__pyx_t_8 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
 
-  /* "av/container/pyio.pyx":53
+  /* "av/container/pyio.pyx":54
  *         self.iocontext = lib.avio_alloc_context(
  *             self.buffer, buffer_size,
  *             writeable,             # <<<<<<<<<<<<<<
  *             <void*>self,  # User data.
  *             pyio_read,
  */
-  __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_writeable); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 53, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_writeable); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 54, __pyx_L1_error)
 
-  /* "av/container/pyio.pyx":51
+  /* "av/container/pyio.pyx":52
  *         self.buffer = <unsigned char*>lib.av_malloc(buffer_size)
  * 
  *         self.iocontext = lib.avio_alloc_context(             # <<<<<<<<<<<<<<
  *             self.buffer, buffer_size,
  *             writeable,
  */
   __pyx_v_self->iocontext = avio_alloc_context(__pyx_v_self->buffer, __pyx_t_8, __pyx_t_9, ((void *)__pyx_v_self), __pyx_f_2av_9container_4pyio_pyio_read, __pyx_f_2av_9container_4pyio_pyio_write, __pyx_v_seek_func);
 
-  /* "av/container/pyio.pyx":60
+  /* "av/container/pyio.pyx":61
  *         )
  * 
  *         if seek_func:             # <<<<<<<<<<<<<<
  *             self.iocontext.seekable = lib.AVIO_SEEKABLE_NORMAL
  *         self.iocontext.max_packet_size = buffer_size
  */
   __pyx_t_5 = (__pyx_v_seek_func != 0);
   if (__pyx_t_5) {
 
-    /* "av/container/pyio.pyx":61
+    /* "av/container/pyio.pyx":62
  * 
  *         if seek_func:
  *             self.iocontext.seekable = lib.AVIO_SEEKABLE_NORMAL             # <<<<<<<<<<<<<<
  *         self.iocontext.max_packet_size = buffer_size
  * 
  */
     __pyx_v_self->iocontext->seekable = AVIO_SEEKABLE_NORMAL;
 
-    /* "av/container/pyio.pyx":60
+    /* "av/container/pyio.pyx":61
  *         )
  * 
  *         if seek_func:             # <<<<<<<<<<<<<<
  *             self.iocontext.seekable = lib.AVIO_SEEKABLE_NORMAL
  *         self.iocontext.max_packet_size = buffer_size
  */
   }
 
-  /* "av/container/pyio.pyx":62
+  /* "av/container/pyio.pyx":63
  *         if seek_func:
  *             self.iocontext.seekable = lib.AVIO_SEEKABLE_NORMAL
  *         self.iocontext.max_packet_size = buffer_size             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_buffer_size); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_buffer_size); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 63, __pyx_L1_error)
   __pyx_v_self->iocontext->max_packet_size = __pyx_t_9;
 
   /* "av/container/pyio.pyx":12
  * cdef class PyIOFile(object):
  * 
  *     def __cinit__(self, file, buffer_size, writeable=None):             # <<<<<<<<<<<<<<
  * 
@@ -2133,15 +2162,15 @@
   __Pyx_XDECREF(__pyx_v_writable);
   __Pyx_XDECREF(__pyx_v_seekable);
   __Pyx_XDECREF(__pyx_v_writeable);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":64
+/* "av/container/pyio.pyx":65
  *         self.iocontext.max_packet_size = buffer_size
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  */
 
@@ -2157,81 +2186,81 @@
 }
 
 static void __pyx_pf_2av_9container_4pyio_8PyIOFile_2__dealloc__(struct __pyx_obj_2av_9container_4pyio_PyIOFile *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "av/container/pyio.pyx":65
+  /* "av/container/pyio.pyx":66
  * 
  *     def __dealloc__(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  *             # Do not touch our original buffer as it may have been freed and replaced.
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "av/container/pyio.pyx":68
+        /* "av/container/pyio.pyx":69
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  *             # Do not touch our original buffer as it may have been freed and replaced.
  *             if self.iocontext:             # <<<<<<<<<<<<<<
  *                 lib.av_freep(&self.iocontext.buffer)
  *                 lib.av_freep(&self.iocontext)
  */
         __pyx_t_1 = (__pyx_v_self->iocontext != 0);
         if (__pyx_t_1) {
 
-          /* "av/container/pyio.pyx":69
+          /* "av/container/pyio.pyx":70
  *             # Do not touch our original buffer as it may have been freed and replaced.
  *             if self.iocontext:
  *                 lib.av_freep(&self.iocontext.buffer)             # <<<<<<<<<<<<<<
  *                 lib.av_freep(&self.iocontext)
  * 
  */
           av_freep((&__pyx_v_self->iocontext->buffer));
 
-          /* "av/container/pyio.pyx":70
+          /* "av/container/pyio.pyx":71
  *             if self.iocontext:
  *                 lib.av_freep(&self.iocontext.buffer)
  *                 lib.av_freep(&self.iocontext)             # <<<<<<<<<<<<<<
  * 
  *             # We likely errored badly if we got here, and so are still
  */
           av_freep((&__pyx_v_self->iocontext));
 
-          /* "av/container/pyio.pyx":68
+          /* "av/container/pyio.pyx":69
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  *             # Do not touch our original buffer as it may have been freed and replaced.
  *             if self.iocontext:             # <<<<<<<<<<<<<<
  *                 lib.av_freep(&self.iocontext.buffer)
  *                 lib.av_freep(&self.iocontext)
  */
           goto __pyx_L6;
         }
 
-        /* "av/container/pyio.pyx":75
+        /* "av/container/pyio.pyx":76
  *             # responsible for our buffer.
  *             else:
  *                 lib.av_freep(&self.buffer)             # <<<<<<<<<<<<<<
  * 
  * 
  */
         /*else*/ {
           av_freep((&__pyx_v_self->buffer));
         }
         __pyx_L6:;
       }
 
-      /* "av/container/pyio.pyx":65
+      /* "av/container/pyio.pyx":66
  * 
  *     def __dealloc__(self):
  *         with nogil:             # <<<<<<<<<<<<<<
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  *             # Do not touch our original buffer as it may have been freed and replaced.
  */
       /*finally:*/ {
@@ -2242,27 +2271,27 @@
           #endif
           goto __pyx_L5;
         }
         __pyx_L5:;
       }
   }
 
-  /* "av/container/pyio.pyx":64
+  /* "av/container/pyio.pyx":65
  *         self.iocontext.max_packet_size = buffer_size
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         with nogil:
  *             # FFmpeg will not release custom input, so it's up to us to free it.
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "av/container/pyio.pxd":14
+/* "av/container/pyio.pxd":19
  * 
  *     # File-like source.
  *     cdef readonly object file             # <<<<<<<<<<<<<<
  *     cdef object fread
  *     cdef object fwrite
  */
 
@@ -2406,15 +2435,15 @@
   __Pyx_AddTraceback("av.container.pyio.PyIOFile.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":78
+/* "av/container/pyio.pyx":79
  * 
  * 
  * cdef int pyio_read(void *opaque, uint8_t *buf, int buf_size) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         return pyio_read_gil(opaque, buf, buf_size)
  */
 
@@ -2422,40 +2451,40 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_RefNannySetupContext("pyio_read", 1);
 
-  /* "av/container/pyio.pyx":79
+  /* "av/container/pyio.pyx":80
  * 
  * cdef int pyio_read(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_read_gil(opaque, buf, buf_size)
  * 
  */
   /*try:*/ {
     {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         /*try:*/ {
 
-          /* "av/container/pyio.pyx":80
+          /* "av/container/pyio.pyx":81
  * cdef int pyio_read(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:
  *         return pyio_read_gil(opaque, buf, buf_size)             # <<<<<<<<<<<<<<
  * 
  * cdef int pyio_read_gil(void *opaque, uint8_t *buf, int buf_size):
  */
           __pyx_r = __pyx_f_2av_9container_4pyio_pyio_read_gil(__pyx_v_opaque, __pyx_v_buf, __pyx_v_buf_size);
           goto __pyx_L6_return;
         }
 
-        /* "av/container/pyio.pyx":79
+        /* "av/container/pyio.pyx":80
  * 
  * cdef int pyio_read(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_read_gil(opaque, buf, buf_size)
  * 
  */
         /*finally:*/ {
@@ -2473,15 +2502,15 @@
       #ifdef WITH_THREAD
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L0;
     }
   }
 
-  /* "av/container/pyio.pyx":78
+  /* "av/container/pyio.pyx":79
  * 
  * 
  * cdef int pyio_read(void *opaque, uint8_t *buf, int buf_size) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         return pyio_read_gil(opaque, buf, buf_size)
  */
 
@@ -2490,15 +2519,15 @@
   __pyx_L0:;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":82
+/* "av/container/pyio.pyx":83
  *         return pyio_read_gil(opaque, buf, buf_size)
  * 
  * cdef int pyio_read_gil(void *opaque, uint8_t *buf, int buf_size):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     cdef bytes res
  */
 
@@ -2521,15 +2550,15 @@
   int __pyx_t_11;
   int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyio_read_gil", 0);
 
-  /* "av/container/pyio.pyx":85
+  /* "av/container/pyio.pyx":86
  *     cdef PyIOFile self
  *     cdef bytes res
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fread(buf_size)
  */
   {
@@ -2537,34 +2566,34 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "av/container/pyio.pyx":86
+      /* "av/container/pyio.pyx":87
  *     cdef bytes res
  *     try:
  *         self = <PyIOFile>opaque             # <<<<<<<<<<<<<<
  *         res = self.fread(buf_size)
  *         memcpy(buf, <void*><char*>res, len(res))
  */
       __pyx_t_4 = ((PyObject *)__pyx_v_opaque);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_self = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":87
+      /* "av/container/pyio.pyx":88
  *     try:
  *         self = <PyIOFile>opaque
  *         res = self.fread(buf_size)             # <<<<<<<<<<<<<<
  *         memcpy(buf, <void*><char*>res, len(res))
  *         self.pos += len(res)
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_buf_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 87, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_buf_size); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 88, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_v_self->fread);
       __pyx_t_6 = __pyx_v_self->fread; __pyx_t_7 = NULL;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -2572,131 +2601,131 @@
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_6, function);
         }
       }
       __pyx_t_4 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_t_5);
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 87, __pyx_L3_error)
+      if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(0, 88, __pyx_L3_error)
       __pyx_v_res = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":88
+      /* "av/container/pyio.pyx":89
  *         self = <PyIOFile>opaque
  *         res = self.fread(buf_size)
  *         memcpy(buf, <void*><char*>res, len(res))             # <<<<<<<<<<<<<<
  *         self.pos += len(res)
  *         if not res:
  */
       if (unlikely(__pyx_v_res == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-        __PYX_ERR(0, 88, __pyx_L3_error)
+        __PYX_ERR(0, 89, __pyx_L3_error)
       }
-      __pyx_t_8 = __Pyx_PyBytes_AsWritableString(__pyx_v_res); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 88, __pyx_L3_error)
+      __pyx_t_8 = __Pyx_PyBytes_AsWritableString(__pyx_v_res); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 89, __pyx_L3_error)
       if (unlikely(__pyx_v_res == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 88, __pyx_L3_error)
+        __PYX_ERR(0, 89, __pyx_L3_error)
       }
-      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 88, __pyx_L3_error)
+      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 89, __pyx_L3_error)
       (void)(memcpy(__pyx_v_buf, ((void *)((char *)__pyx_t_8)), __pyx_t_9));
 
-      /* "av/container/pyio.pyx":89
+      /* "av/container/pyio.pyx":90
  *         res = self.fread(buf_size)
  *         memcpy(buf, <void*><char*>res, len(res))
  *         self.pos += len(res)             # <<<<<<<<<<<<<<
  *         if not res:
  *             return lib.AVERROR_EOF
  */
       if (unlikely(__pyx_v_res == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 89, __pyx_L3_error)
+        __PYX_ERR(0, 90, __pyx_L3_error)
       }
-      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 89, __pyx_L3_error)
+      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 90, __pyx_L3_error)
       __pyx_v_self->pos = (__pyx_v_self->pos + __pyx_t_9);
 
-      /* "av/container/pyio.pyx":90
+      /* "av/container/pyio.pyx":91
  *         memcpy(buf, <void*><char*>res, len(res))
  *         self.pos += len(res)
  *         if not res:             # <<<<<<<<<<<<<<
  *             return lib.AVERROR_EOF
  *         return len(res)
  */
       __pyx_t_10 = (__pyx_v_res != Py_None)&&(PyBytes_GET_SIZE(__pyx_v_res) != 0);
       __pyx_t_11 = ((!__pyx_t_10) != 0);
       if (__pyx_t_11) {
 
-        /* "av/container/pyio.pyx":91
+        /* "av/container/pyio.pyx":92
  *         self.pos += len(res)
  *         if not res:
  *             return lib.AVERROR_EOF             # <<<<<<<<<<<<<<
  *         return len(res)
  *     except Exception as e:
  */
         __pyx_r = AVERROR_EOF;
         goto __pyx_L7_try_return;
 
-        /* "av/container/pyio.pyx":90
+        /* "av/container/pyio.pyx":91
  *         memcpy(buf, <void*><char*>res, len(res))
  *         self.pos += len(res)
  *         if not res:             # <<<<<<<<<<<<<<
  *             return lib.AVERROR_EOF
  *         return len(res)
  */
       }
 
-      /* "av/container/pyio.pyx":92
+      /* "av/container/pyio.pyx":93
  *         if not res:
  *             return lib.AVERROR_EOF
  *         return len(res)             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         return stash_exception()
  */
       if (unlikely(__pyx_v_res == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 92, __pyx_L3_error)
+        __PYX_ERR(0, 93, __pyx_L3_error)
       }
-      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 92, __pyx_L3_error)
+      __pyx_t_9 = PyBytes_GET_SIZE(__pyx_v_res); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 93, __pyx_L3_error)
       __pyx_r = __pyx_t_9;
       goto __pyx_L7_try_return;
 
-      /* "av/container/pyio.pyx":85
+      /* "av/container/pyio.pyx":86
  *     cdef PyIOFile self
  *     cdef bytes res
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fread(buf_size)
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "av/container/pyio.pyx":93
+    /* "av/container/pyio.pyx":94
  *             return lib.AVERROR_EOF
  *         return len(res)
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         return stash_exception()
  * 
  */
     __pyx_t_12 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_12) {
       __Pyx_AddTraceback("av.container.pyio.pyio_read_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 93, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_6, &__pyx_t_5) < 0) __PYX_ERR(0, 94, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_6);
       __pyx_v_e = __pyx_t_6;
 
-      /* "av/container/pyio.pyx":94
+      /* "av/container/pyio.pyx":95
  *         return len(res)
  *     except Exception as e:
  *         return stash_exception()             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_r = __pyx_f_2av_5error_stash_exception(NULL);
@@ -2704,15 +2733,15 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "av/container/pyio.pyx":85
+    /* "av/container/pyio.pyx":86
  *     cdef PyIOFile self
  *     cdef bytes res
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fread(buf_size)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -2730,15 +2759,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "av/container/pyio.pyx":82
+  /* "av/container/pyio.pyx":83
  *         return pyio_read_gil(opaque, buf, buf_size)
  * 
  * cdef int pyio_read_gil(void *opaque, uint8_t *buf, int buf_size):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     cdef bytes res
  */
 
@@ -2754,15 +2783,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":97
+/* "av/container/pyio.pyx":98
  * 
  * 
  * cdef int pyio_write(void *opaque, uint8_t *buf, int buf_size) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         return pyio_write_gil(opaque, buf, buf_size)
  */
 
@@ -2770,40 +2799,40 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_RefNannySetupContext("pyio_write", 1);
 
-  /* "av/container/pyio.pyx":98
+  /* "av/container/pyio.pyx":99
  * 
  * cdef int pyio_write(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_write_gil(opaque, buf, buf_size)
  * 
  */
   /*try:*/ {
     {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         /*try:*/ {
 
-          /* "av/container/pyio.pyx":99
+          /* "av/container/pyio.pyx":100
  * cdef int pyio_write(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:
  *         return pyio_write_gil(opaque, buf, buf_size)             # <<<<<<<<<<<<<<
  * 
  * cdef int pyio_write_gil(void *opaque, uint8_t *buf, int buf_size):
  */
           __pyx_r = __pyx_f_2av_9container_4pyio_pyio_write_gil(__pyx_v_opaque, __pyx_v_buf, __pyx_v_buf_size);
           goto __pyx_L6_return;
         }
 
-        /* "av/container/pyio.pyx":98
+        /* "av/container/pyio.pyx":99
  * 
  * cdef int pyio_write(void *opaque, uint8_t *buf, int buf_size) nogil:
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_write_gil(opaque, buf, buf_size)
  * 
  */
         /*finally:*/ {
@@ -2821,15 +2850,15 @@
       #ifdef WITH_THREAD
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L0;
     }
   }
 
-  /* "av/container/pyio.pyx":97
+  /* "av/container/pyio.pyx":98
  * 
  * 
  * cdef int pyio_write(void *opaque, uint8_t *buf, int buf_size) nogil:             # <<<<<<<<<<<<<<
  *     with gil:
  *         return pyio_write_gil(opaque, buf, buf_size)
  */
 
@@ -2838,15 +2867,15 @@
   __pyx_L0:;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":101
+/* "av/container/pyio.pyx":102
  *         return pyio_write_gil(opaque, buf, buf_size)
  * 
  * cdef int pyio_write_gil(void *opaque, uint8_t *buf, int buf_size):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     cdef bytes bytes_to_write
  */
 
@@ -2868,15 +2897,15 @@
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyio_write_gil", 0);
 
-  /* "av/container/pyio.pyx":105
+  /* "av/container/pyio.pyx":106
  *     cdef bytes bytes_to_write
  *     cdef int bytes_written
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         bytes_to_write = buf[:buf_size]
  */
   {
@@ -2884,39 +2913,39 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "av/container/pyio.pyx":106
+      /* "av/container/pyio.pyx":107
  *     cdef int bytes_written
  *     try:
  *         self = <PyIOFile>opaque             # <<<<<<<<<<<<<<
  *         bytes_to_write = buf[:buf_size]
  *         ret_value = self.fwrite(bytes_to_write)
  */
       __pyx_t_4 = ((PyObject *)__pyx_v_opaque);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_self = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":107
+      /* "av/container/pyio.pyx":108
  *     try:
  *         self = <PyIOFile>opaque
  *         bytes_to_write = buf[:buf_size]             # <<<<<<<<<<<<<<
  *         ret_value = self.fwrite(bytes_to_write)
  *         bytes_written = ret_value if isinstance(ret_value, int) else buf_size
  */
-      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_buf) + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 107, __pyx_L3_error)
+      __pyx_t_4 = __Pyx_PyBytes_FromStringAndSize(((const char*)__pyx_v_buf) + 0, __pyx_v_buf_size - 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __pyx_v_bytes_to_write = ((PyObject*)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":108
+      /* "av/container/pyio.pyx":109
  *         self = <PyIOFile>opaque
  *         bytes_to_write = buf[:buf_size]
  *         ret_value = self.fwrite(bytes_to_write)             # <<<<<<<<<<<<<<
  *         bytes_written = ret_value if isinstance(ret_value, int) else buf_size
  *         self.pos += bytes_written
  */
       __Pyx_INCREF(__pyx_v_self->fwrite);
@@ -2928,86 +2957,86 @@
           __Pyx_INCREF(__pyx_t_6);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_5, function);
         }
       }
       __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_v_bytes_to_write) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_bytes_to_write);
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 108, __pyx_L3_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 109, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_ret_value = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":109
+      /* "av/container/pyio.pyx":110
  *         bytes_to_write = buf[:buf_size]
  *         ret_value = self.fwrite(bytes_to_write)
  *         bytes_written = ret_value if isinstance(ret_value, int) else buf_size             # <<<<<<<<<<<<<<
  *         self.pos += bytes_written
  *         return bytes_written
  */
       __pyx_t_8 = PyInt_Check(__pyx_v_ret_value); 
       if ((__pyx_t_8 != 0)) {
-        __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_ret_value); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 109, __pyx_L3_error)
+        __pyx_t_9 = __Pyx_PyInt_As_int(__pyx_v_ret_value); if (unlikely((__pyx_t_9 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 110, __pyx_L3_error)
         __pyx_t_7 = __pyx_t_9;
       } else {
         __pyx_t_7 = __pyx_v_buf_size;
       }
       __pyx_v_bytes_written = __pyx_t_7;
 
-      /* "av/container/pyio.pyx":110
+      /* "av/container/pyio.pyx":111
  *         ret_value = self.fwrite(bytes_to_write)
  *         bytes_written = ret_value if isinstance(ret_value, int) else buf_size
  *         self.pos += bytes_written             # <<<<<<<<<<<<<<
  *         return bytes_written
  *     except Exception as e:
  */
       __pyx_v_self->pos = (__pyx_v_self->pos + __pyx_v_bytes_written);
 
-      /* "av/container/pyio.pyx":111
+      /* "av/container/pyio.pyx":112
  *         bytes_written = ret_value if isinstance(ret_value, int) else buf_size
  *         self.pos += bytes_written
  *         return bytes_written             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         return stash_exception()
  */
       __pyx_r = __pyx_v_bytes_written;
       goto __pyx_L7_try_return;
 
-      /* "av/container/pyio.pyx":105
+      /* "av/container/pyio.pyx":106
  *     cdef bytes bytes_to_write
  *     cdef int bytes_written
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         bytes_to_write = buf[:buf_size]
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "av/container/pyio.pyx":112
+    /* "av/container/pyio.pyx":113
  *         self.pos += bytes_written
  *         return bytes_written
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         return stash_exception()
  * 
  */
     __pyx_t_7 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_7) {
       __Pyx_AddTraceback("av.container.pyio.pyio_write_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 112, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6) < 0) __PYX_ERR(0, 113, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_5);
       __pyx_v_e = __pyx_t_5;
 
-      /* "av/container/pyio.pyx":113
+      /* "av/container/pyio.pyx":114
  *         return bytes_written
  *     except Exception as e:
  *         return stash_exception()             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_r = __pyx_f_2av_5error_stash_exception(NULL);
@@ -3015,15 +3044,15 @@
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "av/container/pyio.pyx":105
+    /* "av/container/pyio.pyx":106
  *     cdef bytes bytes_to_write
  *     cdef int bytes_written
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         bytes_to_write = buf[:buf_size]
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -3041,15 +3070,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "av/container/pyio.pyx":101
+  /* "av/container/pyio.pyx":102
  *         return pyio_write_gil(opaque, buf, buf_size)
  * 
  * cdef int pyio_write_gil(void *opaque, uint8_t *buf, int buf_size):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     cdef bytes bytes_to_write
  */
 
@@ -3065,15 +3094,15 @@
   __Pyx_XDECREF(__pyx_v_bytes_to_write);
   __Pyx_XDECREF(__pyx_v_ret_value);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":116
+/* "av/container/pyio.pyx":117
  * 
  * 
  * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil:             # <<<<<<<<<<<<<<
  *     # Seek takes the standard flags, but also a ad-hoc one which means that
  *     # the library wants to know how large the file is. We are generally
  */
 
@@ -3082,69 +3111,69 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
   __Pyx_RefNannySetupContext("pyio_seek", 1);
 
-  /* "av/container/pyio.pyx":120
+  /* "av/container/pyio.pyx":121
  *     # the library wants to know how large the file is. We are generally
  *     # allowed to ignore this.
  *     if whence == lib.AVSEEK_SIZE:             # <<<<<<<<<<<<<<
  *         return -1
  *     with gil:
  */
   /*try:*/ {
     __pyx_t_1 = ((__pyx_v_whence == AVSEEK_SIZE) != 0);
     if (__pyx_t_1) {
 
-      /* "av/container/pyio.pyx":121
+      /* "av/container/pyio.pyx":122
  *     # allowed to ignore this.
  *     if whence == lib.AVSEEK_SIZE:
  *         return -1             # <<<<<<<<<<<<<<
  *     with gil:
  *         return pyio_seek_gil(opaque, offset, whence)
  */
       __pyx_r = -1L;
       goto __pyx_L3_return;
 
-      /* "av/container/pyio.pyx":120
+      /* "av/container/pyio.pyx":121
  *     # the library wants to know how large the file is. We are generally
  *     # allowed to ignore this.
  *     if whence == lib.AVSEEK_SIZE:             # <<<<<<<<<<<<<<
  *         return -1
  *     with gil:
  */
     }
 
-    /* "av/container/pyio.pyx":122
+    /* "av/container/pyio.pyx":123
  *     if whence == lib.AVSEEK_SIZE:
  *         return -1
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_seek_gil(opaque, offset, whence)
  * 
  */
     {
         #ifdef WITH_THREAD
         PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
         #endif
         /*try:*/ {
 
-          /* "av/container/pyio.pyx":123
+          /* "av/container/pyio.pyx":124
  *         return -1
  *     with gil:
  *         return pyio_seek_gil(opaque, offset, whence)             # <<<<<<<<<<<<<<
  * 
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):
  */
           __pyx_r = __pyx_f_2av_9container_4pyio_pyio_seek_gil(__pyx_v_opaque, __pyx_v_offset, __pyx_v_whence);
           goto __pyx_L7_return;
         }
 
-        /* "av/container/pyio.pyx":122
+        /* "av/container/pyio.pyx":123
  *     if whence == lib.AVSEEK_SIZE:
  *         return -1
  *     with gil:             # <<<<<<<<<<<<<<
  *         return pyio_seek_gil(opaque, offset, whence)
  * 
  */
         /*finally:*/ {
@@ -3154,15 +3183,15 @@
             #endif
             goto __pyx_L3_return;
           }
         }
     }
   }
 
-  /* "av/container/pyio.pyx":120
+  /* "av/container/pyio.pyx":121
  *     # the library wants to know how large the file is. We are generally
  *     # allowed to ignore this.
  *     if whence == lib.AVSEEK_SIZE:             # <<<<<<<<<<<<<<
  *         return -1
  *     with gil:
  */
   /*finally:*/ {
@@ -3170,15 +3199,15 @@
       #ifdef WITH_THREAD
       __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
       #endif
       goto __pyx_L0;
     }
   }
 
-  /* "av/container/pyio.pyx":116
+  /* "av/container/pyio.pyx":117
  * 
  * 
  * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil:             # <<<<<<<<<<<<<<
  *     # Seek takes the standard flags, but also a ad-hoc one which means that
  *     # the library wants to know how large the file is. We are generally
  */
 
@@ -3187,15 +3216,15 @@
   __pyx_L0:;
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "av/container/pyio.pyx":125
+/* "av/container/pyio.pyx":126
  *         return pyio_seek_gil(opaque, offset, whence)
  * 
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     try:
  */
 
@@ -3219,15 +3248,15 @@
   int __pyx_t_12;
   int64_t __pyx_t_13;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pyio_seek_gil", 0);
 
-  /* "av/container/pyio.pyx":127
+  /* "av/container/pyio.pyx":128
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):
  *     cdef PyIOFile self
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fseek(offset, whence)
  */
   {
@@ -3235,36 +3264,36 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "av/container/pyio.pyx":128
+      /* "av/container/pyio.pyx":129
  *     cdef PyIOFile self
  *     try:
  *         self = <PyIOFile>opaque             # <<<<<<<<<<<<<<
  *         res = self.fseek(offset, whence)
  * 
  */
       __pyx_t_4 = ((PyObject *)__pyx_v_opaque);
       __Pyx_INCREF(__pyx_t_4);
       __pyx_v_self = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_4);
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":129
+      /* "av/container/pyio.pyx":130
  *     try:
  *         self = <PyIOFile>opaque
  *         res = self.fseek(offset, whence)             # <<<<<<<<<<<<<<
  * 
  *         # Track the position for the user.
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 129, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int64_t(__pyx_v_offset); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 130, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_whence); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 129, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyInt_From_int(__pyx_v_whence); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 130, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_INCREF(__pyx_v_self->fseek);
       __pyx_t_7 = __pyx_v_self->fseek; __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
@@ -3274,154 +3303,154 @@
           __Pyx_DECREF_SET(__pyx_t_7, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_7)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_7)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_5, __pyx_t_6};
-        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_7, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 129, __pyx_L3_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 130, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_5);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_5);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_t_6);
         __pyx_t_5 = 0;
         __pyx_t_6 = 0;
-        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L3_error)
+        __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_10, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __pyx_v_res = __pyx_t_4;
       __pyx_t_4 = 0;
 
-      /* "av/container/pyio.pyx":132
+      /* "av/container/pyio.pyx":133
  * 
  *         # Track the position for the user.
  *         if whence == 0:             # <<<<<<<<<<<<<<
  *             self.pos = offset
  *         elif whence == 1:
  */
       switch (__pyx_v_whence) {
         case 0:
 
-        /* "av/container/pyio.pyx":133
+        /* "av/container/pyio.pyx":134
  *         # Track the position for the user.
  *         if whence == 0:
  *             self.pos = offset             # <<<<<<<<<<<<<<
  *         elif whence == 1:
  *             self.pos += offset
  */
         __pyx_v_self->pos = __pyx_v_offset;
 
-        /* "av/container/pyio.pyx":132
+        /* "av/container/pyio.pyx":133
  * 
  *         # Track the position for the user.
  *         if whence == 0:             # <<<<<<<<<<<<<<
  *             self.pos = offset
  *         elif whence == 1:
  */
         break;
         case 1:
 
-        /* "av/container/pyio.pyx":135
+        /* "av/container/pyio.pyx":136
  *             self.pos = offset
  *         elif whence == 1:
  *             self.pos += offset             # <<<<<<<<<<<<<<
  *         else:
  *             self.pos_is_valid = False
  */
         __pyx_v_self->pos = (__pyx_v_self->pos + __pyx_v_offset);
 
-        /* "av/container/pyio.pyx":134
+        /* "av/container/pyio.pyx":135
  *         if whence == 0:
  *             self.pos = offset
  *         elif whence == 1:             # <<<<<<<<<<<<<<
  *             self.pos += offset
  *         else:
  */
         break;
         default:
 
-        /* "av/container/pyio.pyx":137
+        /* "av/container/pyio.pyx":138
  *             self.pos += offset
  *         else:
  *             self.pos_is_valid = False             # <<<<<<<<<<<<<<
  *         if res is None:
  *             if self.pos_is_valid:
  */
         __pyx_v_self->pos_is_valid = 0;
         break;
       }
 
-      /* "av/container/pyio.pyx":138
+      /* "av/container/pyio.pyx":139
  *         else:
  *             self.pos_is_valid = False
  *         if res is None:             # <<<<<<<<<<<<<<
  *             if self.pos_is_valid:
  *                 res = self.pos
  */
       __pyx_t_11 = (__pyx_v_res == Py_None);
       __pyx_t_12 = (__pyx_t_11 != 0);
       if (__pyx_t_12) {
 
-        /* "av/container/pyio.pyx":139
+        /* "av/container/pyio.pyx":140
  *             self.pos_is_valid = False
  *         if res is None:
  *             if self.pos_is_valid:             # <<<<<<<<<<<<<<
  *                 res = self.pos
  *             else:
  */
         __pyx_t_12 = (__pyx_v_self->pos_is_valid != 0);
         if (__pyx_t_12) {
 
-          /* "av/container/pyio.pyx":140
+          /* "av/container/pyio.pyx":141
  *         if res is None:
  *             if self.pos_is_valid:
  *                 res = self.pos             # <<<<<<<<<<<<<<
  *             else:
  *                 res = self.ftell()
  */
-          __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_self->pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L3_error)
+          __pyx_t_4 = __Pyx_PyInt_From_long(__pyx_v_self->pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF_SET(__pyx_v_res, __pyx_t_4);
           __pyx_t_4 = 0;
 
-          /* "av/container/pyio.pyx":139
+          /* "av/container/pyio.pyx":140
  *             self.pos_is_valid = False
  *         if res is None:
  *             if self.pos_is_valid:             # <<<<<<<<<<<<<<
  *                 res = self.pos
  *             else:
  */
           goto __pyx_L10;
         }
 
-        /* "av/container/pyio.pyx":142
+        /* "av/container/pyio.pyx":143
  *                 res = self.pos
  *             else:
  *                 res = self.ftell()             # <<<<<<<<<<<<<<
  *         return res
  *     except Exception as e:
  */
         /*else*/ {
@@ -3434,43 +3463,43 @@
               __Pyx_INCREF(__pyx_t_10);
               __Pyx_INCREF(function);
               __Pyx_DECREF_SET(__pyx_t_7, function);
             }
           }
           __pyx_t_4 = (__pyx_t_10) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_10) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
-          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L3_error)
+          if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L3_error)
           __Pyx_GOTREF(__pyx_t_4);
           __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
           __Pyx_DECREF_SET(__pyx_v_res, __pyx_t_4);
           __pyx_t_4 = 0;
         }
         __pyx_L10:;
 
-        /* "av/container/pyio.pyx":138
+        /* "av/container/pyio.pyx":139
  *         else:
  *             self.pos_is_valid = False
  *         if res is None:             # <<<<<<<<<<<<<<
  *             if self.pos_is_valid:
  *                 res = self.pos
  */
       }
 
-      /* "av/container/pyio.pyx":143
+      /* "av/container/pyio.pyx":144
  *             else:
  *                 res = self.ftell()
  *         return res             # <<<<<<<<<<<<<<
  *     except Exception as e:
  *         return stash_exception()
  */
-      __pyx_t_13 = __Pyx_PyInt_As_int64_t(__pyx_v_res); if (unlikely((__pyx_t_13 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 143, __pyx_L3_error)
+      __pyx_t_13 = __Pyx_PyInt_As_int64_t(__pyx_v_res); if (unlikely((__pyx_t_13 == ((int64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 144, __pyx_L3_error)
       __pyx_r = __pyx_t_13;
       goto __pyx_L7_try_return;
 
-      /* "av/container/pyio.pyx":127
+      /* "av/container/pyio.pyx":128
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):
  *     cdef PyIOFile self
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fseek(offset, whence)
  */
     }
@@ -3478,45 +3507,48 @@
     __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "av/container/pyio.pyx":144
+    /* "av/container/pyio.pyx":145
  *                 res = self.ftell()
  *         return res
  *     except Exception as e:             # <<<<<<<<<<<<<<
  *         return stash_exception()
+ * 
  */
     __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_9) {
       __Pyx_AddTraceback("av.container.pyio.pyio_seek_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 144, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_10) < 0) __PYX_ERR(0, 145, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_e = __pyx_t_7;
 
-      /* "av/container/pyio.pyx":145
+      /* "av/container/pyio.pyx":146
  *         return res
  *     except Exception as e:
  *         return stash_exception()             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
       __pyx_r = __pyx_f_2av_5error_stash_exception(NULL);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       goto __pyx_L6_except_return;
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "av/container/pyio.pyx":127
+    /* "av/container/pyio.pyx":128
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):
  *     cdef PyIOFile self
  *     try:             # <<<<<<<<<<<<<<
  *         self = <PyIOFile>opaque
  *         res = self.fseek(offset, whence)
  */
     __Pyx_XGIVEREF(__pyx_t_1);
@@ -3534,15 +3566,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "av/container/pyio.pyx":125
+  /* "av/container/pyio.pyx":126
  *         return pyio_seek_gil(opaque, offset, whence)
  * 
  * cdef int64_t pyio_seek_gil(void *opaque, int64_t offset, int whence):             # <<<<<<<<<<<<<<
  *     cdef PyIOFile self
  *     try:
  */
 
@@ -3560,14 +3592,269 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_self);
   __Pyx_XDECREF(__pyx_v_res);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "av/container/pyio.pyx":149
+ * 
+ * 
+ * cdef void pyio_close_gil(lib.AVIOContext *pb):             # <<<<<<<<<<<<<<
+ *     try:
+ *         lib.avio_close(pb)
+ */
+
+static void __pyx_f_2av_9container_4pyio_pyio_close_gil(struct AVIOContext *__pyx_v_pb) {
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  __Pyx_RefNannySetupContext("pyio_close_gil", 0);
+
+  /* "av/container/pyio.pyx":150
+ * 
+ * cdef void pyio_close_gil(lib.AVIOContext *pb):
+ *     try:             # <<<<<<<<<<<<<<
+ *         lib.avio_close(pb)
+ * 
+ */
+  {
+    (void)__pyx_t_1; (void)__pyx_t_2; (void)__pyx_t_3; /* mark used */
+    /*try:*/ {
+
+      /* "av/container/pyio.pyx":151
+ * cdef void pyio_close_gil(lib.AVIOContext *pb):
+ *     try:
+ *         lib.avio_close(pb)             # <<<<<<<<<<<<<<
+ * 
+ *     except Exception as e:
+ */
+      (void)(avio_close(__pyx_v_pb));
+
+      /* "av/container/pyio.pyx":150
+ * 
+ * cdef void pyio_close_gil(lib.AVIOContext *pb):
+ *     try:             # <<<<<<<<<<<<<<
+ *         lib.avio_close(pb)
+ * 
+ */
+    }
+  }
+
+  /* "av/container/pyio.pyx":149
+ * 
+ * 
+ * cdef void pyio_close_gil(lib.AVIOContext *pb):             # <<<<<<<<<<<<<<
+ *     try:
+ *         lib.avio_close(pb)
+ */
+
+  /* function exit code */
+  __Pyx_XDECREF(__pyx_v_e);
+  __Pyx_RefNannyFinishContext();
+}
+
+/* "av/container/pyio.pyx":157
+ * 
+ * 
+ * cdef void pyio_close_custom_gil(lib.AVIOContext *pb):             # <<<<<<<<<<<<<<
+ *     cdef PyIOFile self
+ *     try:
+ */
+
+static void __pyx_f_2av_9container_4pyio_pyio_close_custom_gil(struct AVIOContext *__pyx_v_pb) {
+  struct __pyx_obj_2av_9container_4pyio_PyIOFile *__pyx_v_self = 0;
+  CYTHON_UNUSED PyObject *__pyx_v_e = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  PyObject *__pyx_t_8 = NULL;
+  int __pyx_t_9;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("pyio_close_custom_gil", 0);
+
+  /* "av/container/pyio.pyx":159
+ * cdef void pyio_close_custom_gil(lib.AVIOContext *pb):
+ *     cdef PyIOFile self
+ *     try:             # <<<<<<<<<<<<<<
+ *         self = <PyIOFile>pb.opaque
+ * 
+ */
+  {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
+    __Pyx_XGOTREF(__pyx_t_1);
+    __Pyx_XGOTREF(__pyx_t_2);
+    __Pyx_XGOTREF(__pyx_t_3);
+    /*try:*/ {
+
+      /* "av/container/pyio.pyx":160
+ *     cdef PyIOFile self
+ *     try:
+ *         self = <PyIOFile>pb.opaque             # <<<<<<<<<<<<<<
+ * 
+ *         # Flush bytes in the AVIOContext buffers to the custom I/O
+ */
+      __pyx_t_4 = ((PyObject *)__pyx_v_pb->opaque);
+      __Pyx_INCREF(__pyx_t_4);
+      __pyx_v_self = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)__pyx_t_4);
+      __pyx_t_4 = 0;
+
+      /* "av/container/pyio.pyx":163
+ * 
+ *         # Flush bytes in the AVIOContext buffers to the custom I/O
+ *         lib.avio_flush(pb)             # <<<<<<<<<<<<<<
+ * 
+ *         if self.fclose is not None:
+ */
+      avio_flush(__pyx_v_pb);
+
+      /* "av/container/pyio.pyx":165
+ *         lib.avio_flush(pb)
+ * 
+ *         if self.fclose is not None:             # <<<<<<<<<<<<<<
+ *             self.fclose()
+ * 
+ */
+      __pyx_t_5 = (__pyx_v_self->fclose != Py_None);
+      __pyx_t_6 = (__pyx_t_5 != 0);
+      if (__pyx_t_6) {
+
+        /* "av/container/pyio.pyx":166
+ * 
+ *         if self.fclose is not None:
+ *             self.fclose()             # <<<<<<<<<<<<<<
+ * 
+ *     except Exception as e:
+ */
+        __Pyx_INCREF(__pyx_v_self->fclose);
+        __pyx_t_7 = __pyx_v_self->fclose; __pyx_t_8 = NULL;
+        if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
+          __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
+          if (likely(__pyx_t_8)) {
+            PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
+            __Pyx_INCREF(__pyx_t_8);
+            __Pyx_INCREF(function);
+            __Pyx_DECREF_SET(__pyx_t_7, function);
+          }
+        }
+        __pyx_t_4 = (__pyx_t_8) ? __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_8) : __Pyx_PyObject_CallNoArg(__pyx_t_7);
+        __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L3_error)
+        __Pyx_GOTREF(__pyx_t_4);
+        __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+        __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
+        /* "av/container/pyio.pyx":165
+ *         lib.avio_flush(pb)
+ * 
+ *         if self.fclose is not None:             # <<<<<<<<<<<<<<
+ *             self.fclose()
+ * 
+ */
+      }
+
+      /* "av/container/pyio.pyx":159
+ * cdef void pyio_close_custom_gil(lib.AVIOContext *pb):
+ *     cdef PyIOFile self
+ *     try:             # <<<<<<<<<<<<<<
+ *         self = <PyIOFile>pb.opaque
+ * 
+ */
+    }
+    __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
+    goto __pyx_L8_try_end;
+    __pyx_L3_error:;
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+
+    /* "av/container/pyio.pyx":168
+ *             self.fclose()
+ * 
+ *     except Exception as e:             # <<<<<<<<<<<<<<
+ *         stash_exception()
+ */
+    __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
+    if (__pyx_t_9) {
+      __Pyx_AddTraceback("av.container.pyio.pyio_close_custom_gil", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 168, __pyx_L5_except_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_GOTREF(__pyx_t_7);
+      __Pyx_GOTREF(__pyx_t_8);
+      __Pyx_INCREF(__pyx_t_7);
+      __pyx_v_e = __pyx_t_7;
+
+      /* "av/container/pyio.pyx":169
+ * 
+ *     except Exception as e:
+ *         stash_exception()             # <<<<<<<<<<<<<<
+ */
+      (void)(__pyx_f_2av_5error_stash_exception(NULL));
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
+      goto __pyx_L4_exception_handled;
+    }
+    goto __pyx_L5_except_error;
+    __pyx_L5_except_error:;
+
+    /* "av/container/pyio.pyx":159
+ * cdef void pyio_close_custom_gil(lib.AVIOContext *pb):
+ *     cdef PyIOFile self
+ *     try:             # <<<<<<<<<<<<<<
+ *         self = <PyIOFile>pb.opaque
+ * 
+ */
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    goto __pyx_L1_error;
+    __pyx_L4_exception_handled:;
+    __Pyx_XGIVEREF(__pyx_t_1);
+    __Pyx_XGIVEREF(__pyx_t_2);
+    __Pyx_XGIVEREF(__pyx_t_3);
+    __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
+    __pyx_L8_try_end:;
+  }
+
+  /* "av/container/pyio.pyx":157
+ * 
+ * 
+ * cdef void pyio_close_custom_gil(lib.AVIOContext *pb):             # <<<<<<<<<<<<<<
+ *     cdef PyIOFile self
+ *     try:
+ */
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_WriteUnraisable("av.container.pyio.pyio_close_custom_gil", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_self);
+  __Pyx_XDECREF(__pyx_v_e);
+  __Pyx_RefNannyFinishContext();
+}
+
 static PyObject *__pyx_tp_new_2av_9container_4pyio_PyIOFile(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
@@ -3575,14 +3862,15 @@
   if (unlikely(!o)) return 0;
   p = ((struct __pyx_obj_2av_9container_4pyio_PyIOFile *)o);
   p->file = Py_None; Py_INCREF(Py_None);
   p->fread = Py_None; Py_INCREF(Py_None);
   p->fwrite = Py_None; Py_INCREF(Py_None);
   p->fseek = Py_None; Py_INCREF(Py_None);
   p->ftell = Py_None; Py_INCREF(Py_None);
+  p->fclose = Py_None; Py_INCREF(Py_None);
   if (unlikely(__pyx_pw_2av_9container_4pyio_8PyIOFile_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
@@ -3603,14 +3891,15 @@
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->file);
   Py_CLEAR(p->fread);
   Py_CLEAR(p->fwrite);
   Py_CLEAR(p->fseek);
   Py_CLEAR(p->ftell);
+  Py_CLEAR(p->fclose);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
 static int __pyx_tp_traverse_2av_9container_4pyio_PyIOFile(PyObject *o, visitproc v, void *a) {
   int e;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *p = (struct __pyx_obj_2av_9container_4pyio_PyIOFile *)o;
   if (p->file) {
@@ -3624,14 +3913,17 @@
   }
   if (p->fseek) {
     e = (*v)(p->fseek, a); if (e) return e;
   }
   if (p->ftell) {
     e = (*v)(p->ftell, a); if (e) return e;
   }
+  if (p->fclose) {
+    e = (*v)(p->fclose, a); if (e) return e;
+  }
   return 0;
 }
 
 static int __pyx_tp_clear_2av_9container_4pyio_PyIOFile(PyObject *o) {
   PyObject* tmp;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *p = (struct __pyx_obj_2av_9container_4pyio_PyIOFile *)o;
   tmp = ((PyObject*)p->file);
@@ -3645,14 +3937,17 @@
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->fseek);
   p->fseek = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->ftell);
   p->ftell = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
+  tmp = ((PyObject*)p->fclose);
+  p->fclose = Py_None; Py_INCREF(Py_None);
+  Py_XDECREF(tmp);
   return 0;
 }
 
 static PyObject *__pyx_getprop_2av_9container_4pyio_8PyIOFile_file(PyObject *o, CYTHON_UNUSED void *x) {
   return __pyx_pw_2av_9container_4pyio_8PyIOFile_4file_1__get__(o);
 }
 
@@ -3788,14 +4083,15 @@
   {&__pyx_kp_s_File_object_has_no_read_method_o, __pyx_k_File_object_has_no_read_method_o, sizeof(__pyx_k_File_object_has_no_read_method_o), 0, 0, 1, 0},
   {&__pyx_kp_s_File_object_has_no_write_method, __pyx_k_File_object_has_no_write_method, sizeof(__pyx_k_File_object_has_no_write_method), 0, 0, 1, 0},
   {&__pyx_n_s_PyIOFile, __pyx_k_PyIOFile, sizeof(__pyx_k_PyIOFile), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_buffer_size, __pyx_k_buffer_size, sizeof(__pyx_k_buffer_size), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+  {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
   {&__pyx_n_s_file, __pyx_k_file, sizeof(__pyx_k_file), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_read, __pyx_k_read, sizeof(__pyx_k_read), 0, 0, 1, 1},
   {&__pyx_n_s_readable, __pyx_k_readable, sizeof(__pyx_k_readable), 0, 0, 1, 1},
@@ -3810,44 +4106,44 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_writable, __pyx_k_writable, sizeof(__pyx_k_writable), 0, 0, 1, 1},
   {&__pyx_n_s_write, __pyx_k_write, sizeof(__pyx_k_write), 0, 0, 1, 1},
   {&__pyx_n_s_writeable, __pyx_k_writeable, sizeof(__pyx_k_writeable), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 41, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/container/pyio.pyx":40
+  /* "av/container/pyio.pyx":41
  *         if writeable:
  *             if self.fwrite is None or (writable is not None and not writable()):
  *                 raise ValueError("File object has no write() method, or writable() returned False.")             # <<<<<<<<<<<<<<
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_File_object_has_no_write_method); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_File_object_has_no_write_method); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 41, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "av/container/pyio.pyx":43
+  /* "av/container/pyio.pyx":44
  *         else:
  *             if self.fread is None or (readable is not None and not readable()):
  *                 raise ValueError("File object has no read() method, or readable() returned False.")             # <<<<<<<<<<<<<<
  * 
  *         self.pos = 0
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_File_object_has_no_read_method_o); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_File_object_has_no_read_method_o); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 44, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -3909,14 +4205,16 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("pyio_read", (void (*)(void))__pyx_f_2av_9container_4pyio_pyio_read, "int (void *, uint8_t *, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("pyio_write", (void (*)(void))__pyx_f_2av_9container_4pyio_pyio_write, "int (void *, uint8_t *, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("pyio_seek", (void (*)(void))__pyx_f_2av_9container_4pyio_pyio_seek, "int64_t (void *, int64_t, int)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("pyio_close_gil", (void (*)(void))__pyx_f_2av_9container_4pyio_pyio_close_gil, "void (struct AVIOContext *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("pyio_close_custom_gil", (void (*)(void))__pyx_f_2av_9container_4pyio_pyio_close_custom_gil, "void (struct AVIOContext *)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
```

### Comparing `av-9.1.1/src/av/container/streams.c` & `av-9.2.0/src/av/container/streams.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1242,28 +1250,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1294,15 +1303,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4720,18 +4732,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.format"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_6format_ContainerFormat = __Pyx_ImportType(__pyx_t_1, "av.format", "ContainerFormat", sizeof(struct __pyx_obj_2av_6format_ContainerFormat), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_6format_ContainerFormat) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.core"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 16, __pyx_L1_error)
```

### Comparing `av-9.1.1/src/av/data/stream.c` & `av-9.2.0/src/av/data/stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1242,28 +1250,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1313,15 +1322,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2963,18 +2975,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/descriptor.c` & `av-9.2.0/src/av/descriptor.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/dictionary.c` & `av-9.2.0/src/av/dictionary.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/enum.c` & `av-9.2.0/src/av/enum.c`

 * *Files 1% similar despite different names*

```diff
@@ -1480,14 +1480,31 @@
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
+/* ListCompAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len)) {
+        Py_INCREF(x);
+        PyList_SET_ITEM(list, len, x);
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+#endif
+
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
@@ -8950,24 +8967,29 @@
  */
 
 static PyObject *__pyx_pw_2av_4enum_3define_enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyObject *__pyx_f_2av_4enum_define_enum(PyObject *__pyx_v_name, PyObject *__pyx_v_module, PyObject *__pyx_v_items, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_2av_4enum_define_enum *__pyx_optional_args) {
   int __pyx_v_is_flags = ((int)0);
   PyTypeObject *__pyx_v_base_cls = NULL;
   PyObject *__pyx_v_cls = NULL;
+  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_t_7;
-  PyObject *__pyx_t_8 = NULL;
+  PyObject *__pyx_t_7 = NULL;
+  Py_ssize_t __pyx_t_8;
+  PyObject *(*__pyx_t_9)(PyObject *);
+  PyObject *__pyx_t_10 = NULL;
+  int __pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("define_enum", 0);
   if (__pyx_optional_args) {
     if (__pyx_optional_args->__pyx_n > 0) {
       __pyx_v_is_flags = __pyx_optional_args->is_flags;
@@ -9005,99 +9027,151 @@
   }
 
   /* "av/enum.pyx":385
  *         base_cls = EnumFlag
  *     else:
  *         base_cls = EnumItem             # <<<<<<<<<<<<<<
  * 
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+ *     # Some items may be None if they correspond to an unsupported FFmpeg feature
  */
   /*else*/ {
     __Pyx_INCREF(((PyObject *)__pyx_ptype_2av_4enum_EnumItem));
     __pyx_v_base_cls = __pyx_ptype_2av_4enum_EnumItem;
   }
   __pyx_L3:;
 
-  /* "av/enum.pyx":387
- *         base_cls = EnumItem
+  /* "av/enum.pyx":388
  * 
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)             # <<<<<<<<<<<<<<
+ *     # Some items may be None if they correspond to an unsupported FFmpeg feature
+ *     cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])             # <<<<<<<<<<<<<<
  * 
  *     return cls
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_EnumType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_EnumType); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_INCREF(((PyObject *)__pyx_v_base_cls));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_base_cls));
   PyTuple_SET_ITEM(__pyx_t_4, 0, ((PyObject *)__pyx_v_base_cls));
-  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 387, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_module, __pyx_v_module) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
-  __pyx_t_6 = NULL;
-  __pyx_t_7 = 0;
+  if (PyDict_SetItem(__pyx_t_5, __pyx_n_s_module, __pyx_v_module) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_6);
+  if (likely(PyList_CheckExact(__pyx_v_items)) || PyTuple_CheckExact(__pyx_v_items)) {
+    __pyx_t_7 = __pyx_v_items; __Pyx_INCREF(__pyx_t_7); __pyx_t_8 = 0;
+    __pyx_t_9 = NULL;
+  } else {
+    __pyx_t_8 = -1; __pyx_t_7 = PyObject_GetIter(__pyx_v_items); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = Py_TYPE(__pyx_t_7)->tp_iternext; if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 388, __pyx_L1_error)
+  }
+  for (;;) {
+    if (likely(!__pyx_t_9)) {
+      if (likely(PyList_CheckExact(__pyx_t_7))) {
+        if (__pyx_t_8 >= PyList_GET_SIZE(__pyx_t_7)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_10 = PyList_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_10); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 388, __pyx_L1_error)
+        #else
+        __pyx_t_10 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        #endif
+      } else {
+        if (__pyx_t_8 >= PyTuple_GET_SIZE(__pyx_t_7)) break;
+        #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+        __pyx_t_10 = PyTuple_GET_ITEM(__pyx_t_7, __pyx_t_8); __Pyx_INCREF(__pyx_t_10); __pyx_t_8++; if (unlikely(0 < 0)) __PYX_ERR(0, 388, __pyx_L1_error)
+        #else
+        __pyx_t_10 = PySequence_ITEM(__pyx_t_7, __pyx_t_8); __pyx_t_8++; if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_10);
+        #endif
+      }
+    } else {
+      __pyx_t_10 = __pyx_t_9(__pyx_t_7);
+      if (unlikely(!__pyx_t_10)) {
+        PyObject* exc_type = PyErr_Occurred();
+        if (exc_type) {
+          if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
+          else __PYX_ERR(0, 388, __pyx_L1_error)
+        }
+        break;
+      }
+      __Pyx_GOTREF(__pyx_t_10);
+    }
+    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_10);
+    __pyx_t_10 = 0;
+    __pyx_t_1 = (__pyx_v_i != Py_None);
+    __pyx_t_11 = (__pyx_t_1 != 0);
+    if (__pyx_t_11) {
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_6, (PyObject*)__pyx_v_i))) __PYX_ERR(0, 388, __pyx_L1_error)
+    }
+  }
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_7 = NULL;
+  __pyx_t_12 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_3);
-    if (likely(__pyx_t_6)) {
+    __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
+    if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
-      __Pyx_INCREF(__pyx_t_6);
+      __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_7 = 1;
+      __pyx_t_12 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_v_items};
-    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_t_6};
+    __pyx_t_2 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 4+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
-    PyObject *__pyx_temp[5] = {__pyx_t_6, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_v_items};
-    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_7, 4+__pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    PyObject *__pyx_temp[5] = {__pyx_t_7, __pyx_v_name, __pyx_t_4, __pyx_t_5, __pyx_t_6};
+    __pyx_t_2 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_12, 4+__pyx_t_12); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   } else
   #endif
   {
-    __pyx_t_8 = PyTuple_New(4+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 387, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_8);
-    if (__pyx_t_6) {
-      __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
+    __pyx_t_10 = PyTuple_New(4+__pyx_t_12); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 388, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_10);
+    if (__pyx_t_7) {
+      __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_7); __pyx_t_7 = NULL;
     }
     __Pyx_INCREF(__pyx_v_name);
     __Pyx_GIVEREF(__pyx_v_name);
-    PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_name);
+    PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_12, __pyx_v_name);
     __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_12, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
-    PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_t_5);
-    __Pyx_INCREF(__pyx_v_items);
-    __Pyx_GIVEREF(__pyx_v_items);
-    PyTuple_SET_ITEM(__pyx_t_8, 3+__pyx_t_7, __pyx_v_items);
+    PyTuple_SET_ITEM(__pyx_t_10, 2+__pyx_t_12, __pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_10, 3+__pyx_t_12, __pyx_t_6);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_8, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
+    __pyx_t_6 = 0;
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_cls = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "av/enum.pyx":389
- *     cls = EnumType(name, (base_cls, ), {'__module__': module}, items)
+  /* "av/enum.pyx":390
+ *     cls = EnumType(name, (base_cls, ), {'__module__': module}, [i for i in items if i is not None])
  * 
  *     return cls             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_cls);
   __pyx_r = __pyx_v_cls;
   goto __pyx_L0;
@@ -9113,20 +9187,22 @@
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_XDECREF(__pyx_t_7);
+  __Pyx_XDECREF(__pyx_t_10);
   __Pyx_AddTraceback("av.enum.define_enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_base_cls);
   __Pyx_XDECREF(__pyx_v_cls);
+  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
 static PyObject *__pyx_pw_2av_4enum_3define_enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
```

### Comparing `av-9.1.1/src/av/error.c` & `av-9.2.0/src/av/error.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/filter/context.c` & `av-9.2.0/src/av/filter/context.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1384,28 +1392,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1469,15 +1478,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -5243,18 +5255,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(10, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(10, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(11, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(11, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(12, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(12, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/filter/filter.c` & `av-9.2.0/src/av/filter/filter.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/filter/graph.c` & `av-9.2.0/src/av/filter/graph.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1354,28 +1362,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1439,15 +1448,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -6460,18 +6472,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(11, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(11, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(12, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(12, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(12, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(13, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(13, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(13, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/filter/link.c` & `av-9.2.0/src/av/filter/link.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/filter/pad.c` & `av-9.2.0/src/av/filter/pad.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/format.c` & `av-9.2.0/src/av/format.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/frame.c` & `av-9.2.0/src/av/frame.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1177,28 +1185,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1262,15 +1271,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -3931,18 +3943,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(6, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(8, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/logging.c` & `av-9.2.0/src/av/logging.c`

 * *Files 0% similar despite different names*

```diff
@@ -749,14 +749,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/option.c` & `av-9.2.0/src/av/option.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/packet.c` & `av-9.2.0/src/av/packet.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1272,28 +1280,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1343,15 +1352,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4828,18 +4840,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(7, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(7, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(8, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(8, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(9, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(9, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/plane.c` & `av-9.2.0/src/av/plane.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1165,28 +1173,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1250,15 +1259,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2710,18 +2722,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(4, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(4, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(5, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(5, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(6, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/sidedata/motionvectors.c` & `av-9.2.0/src/av/sidedata/motionvectors.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1167,28 +1175,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1252,15 +1261,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4901,18 +4913,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/sidedata/sidedata.c` & `av-9.2.0/src/av/sidedata/sidedata.c`

 * *Files 2% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1189,28 +1197,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1260,15 +1269,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -1504,15 +1516,15 @@
   PyObject *(*_rebase_time)(struct __pyx_obj_2av_5frame_Frame *, AVRational);
   PyObject *(*_copy_internal_attributes)(struct __pyx_obj_2av_5frame_Frame *, struct __pyx_obj_2av_5frame_Frame *, struct __pyx_opt_args_2av_5frame_5Frame__copy_internal_attributes *__pyx_optional_args);
   PyObject *(*_init_user_attributes)(struct __pyx_obj_2av_5frame_Frame *);
 };
 static struct __pyx_vtabstruct_2av_5frame_Frame *__pyx_vtabptr_2av_5frame_Frame;
 
 
-/* "av/sidedata/sidedata.pyx":45
+/* "av/sidedata/sidedata.pyx":47
  * 
  * 
  * cdef class SideData(Buffer):             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  */
 
@@ -2133,14 +2145,15 @@
 static const char __pyx_k_MotionVectors[] = "MotionVectors";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_MATRIXENCODING[] = "MATRIXENCODING";
 static const char __pyx_k_MOTION_VECTORS[] = "MOTION_VECTORS";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
+static const char __pyx_k_SEI_UNREGISTERED[] = "SEI_UNREGISTERED";
 static const char __pyx_k_SideDataContainer[] = "_SideDataContainer";
 static const char __pyx_k_AUDIO_SERVICE_TYPE[] = "AUDIO_SERVICE_TYPE";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_CONTENT_LIGHT_LEVEL[] = "CONTENT_LIGHT_LEVEL";
 static const char __pyx_k_SideDataContainer_2[] = "SideDataContainer";
 static const char __pyx_k_av_sidedata_sidedata[] = "av.sidedata.sidedata";
 static const char __pyx_k_av_sidedata_motionvectors[] = "av.sidedata.motionvectors";
@@ -2164,14 +2177,15 @@
 static PyObject *__pyx_n_s_MOTION_VECTORS;
 static PyObject *__pyx_n_s_Mapping;
 static PyObject *__pyx_n_s_MotionVectors;
 static PyObject *__pyx_n_s_PANSCAN;
 static PyObject *__pyx_n_s_PickleError;
 static PyObject *__pyx_n_s_REPLAYGAIN;
 static PyObject *__pyx_n_s_RuntimeError;
+static PyObject *__pyx_n_s_SEI_UNREGISTERED;
 static PyObject *__pyx_n_s_SKIP_SAMPLES;
 static PyObject *__pyx_n_s_SPHERICAL;
 static PyObject *__pyx_n_s_STEREO3D;
 static PyObject *__pyx_n_s_SideData;
 static PyObject *__pyx_n_s_SideDataContainer;
 static PyObject *__pyx_n_s_SideDataContainer_2;
 static PyObject *__pyx_n_s_Type;
@@ -2240,15 +2254,15 @@
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_codeobj__7;
 /* Late includes */
 
-/* "av/sidedata/sidedata.pyx":36
+/* "av/sidedata/sidedata.pyx":38
  * 
  * 
  * cdef SideData wrap_side_data(Frame frame, int index):             # <<<<<<<<<<<<<<
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  */
 
@@ -2265,45 +2279,45 @@
   int __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("wrap_side_data", 0);
 
-  /* "av/sidedata/sidedata.pyx":38
+  /* "av/sidedata/sidedata.pyx":40
  * cdef SideData wrap_side_data(Frame frame, int index):
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type             # <<<<<<<<<<<<<<
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  */
   __pyx_t_1 = (__pyx_v_frame->ptr->side_data[__pyx_v_index])->type;
   __pyx_v_type_ = __pyx_t_1;
 
-  /* "av/sidedata/sidedata.pyx":39
+  /* "av/sidedata/sidedata.pyx":41
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:             # <<<<<<<<<<<<<<
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  */
   __pyx_t_2 = ((__pyx_v_type_ == AV_FRAME_DATA_MOTION_VECTORS) != 0);
   if (__pyx_t_2) {
 
-    /* "av/sidedata/sidedata.pyx":40
+    /* "av/sidedata/sidedata.pyx":42
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)             # <<<<<<<<<<<<<<
  *     else:
  *         return SideData(_cinit_bypass_sentinel, frame, index)
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MotionVectors); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_MotionVectors); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 40, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 42, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -2312,94 +2326,94 @@
         __Pyx_DECREF_SET(__pyx_t_4, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel, ((PyObject *)__pyx_v_frame), __pyx_t_5};
-      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
       PyObject *__pyx_temp[4] = {__pyx_t_6, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel, ((PyObject *)__pyx_v_frame), __pyx_t_5};
-      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_7, 3+__pyx_t_7); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(3+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_6) {
         __Pyx_GIVEREF(__pyx_t_6); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_6); __pyx_t_6 = NULL;
       }
       __Pyx_INCREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       __Pyx_GIVEREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
       __Pyx_INCREF(((PyObject *)__pyx_v_frame));
       __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, ((PyObject *)__pyx_v_frame));
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_8, 2+__pyx_t_7, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 40, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2av_8sidedata_8sidedata_SideData))))) __PYX_ERR(0, 40, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_2av_8sidedata_8sidedata_SideData))))) __PYX_ERR(0, 42, __pyx_L1_error)
     __pyx_r = ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/sidedata/sidedata.pyx":39
+    /* "av/sidedata/sidedata.pyx":41
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  *     if type_ == lib.AV_FRAME_DATA_MOTION_VECTORS:             # <<<<<<<<<<<<<<
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":42
+  /* "av/sidedata/sidedata.pyx":44
  *         return MotionVectors(_cinit_bypass_sentinel, frame, index)
  *     else:
  *         return SideData(_cinit_bypass_sentinel, frame, index)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
-    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_index); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     __Pyx_GIVEREF(__pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
     __Pyx_INCREF(((PyObject *)__pyx_v_frame));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
     PyTuple_SET_ITEM(__pyx_t_4, 1, ((PyObject *)__pyx_v_frame));
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata_SideData), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata_SideData), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 44, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "av/sidedata/sidedata.pyx":36
+  /* "av/sidedata/sidedata.pyx":38
  * 
  * 
  * cdef SideData wrap_side_data(Frame frame, int index):             # <<<<<<<<<<<<<<
  * 
  *     cdef lib.AVFrameSideDataType type_ = frame.ptr.side_data[index].type
  */
 
@@ -2414,15 +2428,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":47
+/* "av/sidedata/sidedata.pyx":49
  * cdef class SideData(Buffer):
  * 
  *     def __init__(self, sentinel, Frame frame, int index):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  */
 
@@ -2459,46 +2473,46 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_sentinel)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 47, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 1); __PYX_ERR(0, 49, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_index)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 47, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, 2); __PYX_ERR(0, 49, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 47, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 49, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_sentinel = values[0];
     __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)values[1]);
-    __pyx_v_index = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_index == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 47, __pyx_L3_error)
+    __pyx_v_index = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_index == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 49, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 47, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 49, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 49, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_8sidedata_8sidedata_8SideData___init__(((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_v_self), __pyx_v_sentinel, __pyx_v_frame, __pyx_v_index);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -2513,85 +2527,85 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "av/sidedata/sidedata.pyx":48
+  /* "av/sidedata/sidedata.pyx":50
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  */
   __pyx_t_1 = (__pyx_v_sentinel != __pyx_v_2av_8sidedata_8sidedata__cinit_bypass_sentinel);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "av/sidedata/sidedata.pyx":49
+    /* "av/sidedata/sidedata.pyx":51
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')             # <<<<<<<<<<<<<<
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 49, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_RuntimeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 51, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 49, __pyx_L1_error)
+    __PYX_ERR(0, 51, __pyx_L1_error)
 
-    /* "av/sidedata/sidedata.pyx":48
+    /* "av/sidedata/sidedata.pyx":50
  * 
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:             # <<<<<<<<<<<<<<
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":50
+  /* "av/sidedata/sidedata.pyx":52
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame             # <<<<<<<<<<<<<<
  *         self.ptr = frame.ptr.side_data[index]
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_frame));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
   __Pyx_GOTREF(__pyx_v_self->frame);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->frame));
   __pyx_v_self->frame = __pyx_v_frame;
 
-  /* "av/sidedata/sidedata.pyx":51
+  /* "av/sidedata/sidedata.pyx":53
  *             raise RuntimeError('cannot manually instatiate SideData')
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]             # <<<<<<<<<<<<<<
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  */
   __pyx_v_self->ptr = (__pyx_v_frame->ptr->side_data[__pyx_v_index]);
 
-  /* "av/sidedata/sidedata.pyx":52
+  /* "av/sidedata/sidedata.pyx":54
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  *         self.metadata = wrap_dictionary(self.ptr.metadata)             # <<<<<<<<<<<<<<
  * 
  *     cdef size_t _buffer_size(self):
  */
-  __pyx_t_3 = ((PyObject *)__pyx_f_2av_10dictionary_wrap_dictionary(__pyx_v_self->ptr->metadata)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_3 = ((PyObject *)__pyx_f_2av_10dictionary_wrap_dictionary(__pyx_v_self->ptr->metadata)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 54, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->metadata);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->metadata));
   __pyx_v_self->metadata = ((struct __pyx_obj_2av_10dictionary__Dictionary *)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "av/sidedata/sidedata.pyx":47
+  /* "av/sidedata/sidedata.pyx":49
  * cdef class SideData(Buffer):
  * 
  *     def __init__(self, sentinel, Frame frame, int index):             # <<<<<<<<<<<<<<
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')
  */
 
@@ -2603,126 +2617,126 @@
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":54
+/* "av/sidedata/sidedata.pyx":56
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  *     cdef size_t _buffer_size(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.size
  * 
  */
 
 static size_t __pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_size(struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   size_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_size", 0);
 
-  /* "av/sidedata/sidedata.pyx":55
+  /* "av/sidedata/sidedata.pyx":57
  * 
  *     cdef size_t _buffer_size(self):
  *         return self.ptr.size             # <<<<<<<<<<<<<<
  * 
  *     cdef void* _buffer_ptr(self):
  */
   __pyx_r = __pyx_v_self->ptr->size;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":54
+  /* "av/sidedata/sidedata.pyx":56
  *         self.metadata = wrap_dictionary(self.ptr.metadata)
  * 
  *     cdef size_t _buffer_size(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.size
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":57
+/* "av/sidedata/sidedata.pyx":59
  *         return self.ptr.size
  * 
  *     cdef void* _buffer_ptr(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.data
  * 
  */
 
 static void *__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_ptr(struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   void *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_ptr", 0);
 
-  /* "av/sidedata/sidedata.pyx":58
+  /* "av/sidedata/sidedata.pyx":60
  * 
  *     cdef void* _buffer_ptr(self):
  *         return self.ptr.data             # <<<<<<<<<<<<<<
  * 
  *     cdef bint _buffer_writable(self):
  */
   __pyx_r = __pyx_v_self->ptr->data;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":57
+  /* "av/sidedata/sidedata.pyx":59
  *         return self.ptr.size
  * 
  *     cdef void* _buffer_ptr(self):             # <<<<<<<<<<<<<<
  *         return self.ptr.data
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":60
+/* "av/sidedata/sidedata.pyx":62
  *         return self.ptr.data
  * 
  *     cdef bint _buffer_writable(self):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
 
 static int __pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_writable(CYTHON_UNUSED struct __pyx_obj_2av_8sidedata_8sidedata_SideData *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_buffer_writable", 0);
 
-  /* "av/sidedata/sidedata.pyx":61
+  /* "av/sidedata/sidedata.pyx":63
  * 
  *     cdef bint _buffer_writable(self):
  *         return False             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":60
+  /* "av/sidedata/sidedata.pyx":62
  *         return self.ptr.data
  * 
  *     cdef bint _buffer_writable(self):             # <<<<<<<<<<<<<<
  *         return False
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":63
+/* "av/sidedata/sidedata.pyx":65
  *         return False
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'
  * 
  */
 
@@ -2748,93 +2762,93 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "av/sidedata/sidedata.pyx":64
+  /* "av/sidedata/sidedata.pyx":66
  * 
  *     def __repr__(self):
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(9); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = 0;
   __pyx_t_3 = 127;
   __Pyx_INCREF(__pyx_kp_u_av_sidedata);
   __pyx_t_2 += 13;
   __Pyx_GIVEREF(__pyx_kp_u_av_sidedata);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_av_sidedata);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_class); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_FormatSimple(__pyx_t_5, __pyx_empty_unicode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__2);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__2);
   PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u__2);
-  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->ptr->size, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_From_int(__pyx_v_self->ptr->size, 0, ' ', 'd'); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 3, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u_bytes_of);
   __pyx_t_2 += 10;
   __Pyx_GIVEREF(__pyx_kp_u_bytes_of);
   PyTuple_SET_ITEM(__pyx_t_1, 4, __pyx_kp_u_bytes_of);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_FormatSimple(__pyx_t_4, __pyx_empty_unicode); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_5) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_5);
   PyTuple_SET_ITEM(__pyx_t_1, 5, __pyx_t_5);
   __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_kp_u_at_0x);
   __pyx_t_2 += 6;
   __Pyx_GIVEREF(__pyx_kp_u_at_0x);
   PyTuple_SET_ITEM(__pyx_t_1, 6, __pyx_kp_u_at_0x);
-  __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(((unsigned int)__pyx_v_self->ptr->data)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_unsigned_int(((unsigned int)__pyx_v_self->ptr->data)); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_kp_u_0x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Format(__pyx_t_5, __pyx_kp_u_0x); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_3 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) > __pyx_t_3) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_4) : __pyx_t_3;
   __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 7, __pyx_t_4);
   __pyx_t_4 = 0;
   __Pyx_INCREF(__pyx_kp_u__3);
   __pyx_t_2 += 1;
   __Pyx_GIVEREF(__pyx_kp_u__3);
   PyTuple_SET_ITEM(__pyx_t_1, 8, __pyx_kp_u__3);
-  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 64, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyUnicode_Join(__pyx_t_1, 9, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":63
+  /* "av/sidedata/sidedata.pyx":65
  *         return False
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return f'<av.sidedata.{self.__class__.__name__} {self.ptr.size} bytes of {self.type} at 0x{<unsigned int>self.ptr.data:0x}>'
  * 
  */
 
@@ -2847,15 +2861,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":67
+/* "av/sidedata/sidedata.pyx":69
  * 
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         return Type.get(self.ptr.type) or self.ptr.type
  * 
  */
 
@@ -2882,64 +2896,64 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "av/sidedata/sidedata.pyx":68
+  /* "av/sidedata/sidedata.pyx":70
  *     @property
  *     def type(self):
  *         return Type.get(self.ptr.type) or self.ptr.type             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_get); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_5)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_4, function);
     }
   }
   __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_6 < 0)) __PYX_ERR(0, 70, __pyx_L1_error)
   if (!__pyx_t_6) {
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
     __Pyx_INCREF(__pyx_t_2);
     __pyx_t_1 = __pyx_t_2;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(__pyx_v_self->ptr->type); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 70, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":67
+  /* "av/sidedata/sidedata.pyx":69
  * 
  *     @property
  *     def type(self):             # <<<<<<<<<<<<<<
  *         return Type.get(self.ptr.type) or self.ptr.type
  * 
  */
 
@@ -3069,15 +3083,15 @@
   __Pyx_AddTraceback("av.sidedata.sidedata.SideData.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":73
+/* "av/sidedata/sidedata.pyx":75
  * cdef class _SideDataContainer(object):
  * 
  *     def __init__(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         self.frame = frame
  */
 
@@ -3106,32 +3120,32 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frame)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 73, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_frame = ((struct __pyx_obj_2av_5frame_Frame *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 73, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("av.sidedata.sidedata._SideDataContainer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_frame), __pyx_ptype_2av_5frame_Frame, 1, "frame", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
   __pyx_r = __pyx_pf_2av_8sidedata_8sidedata_18_SideDataContainer___init__(((struct __pyx_obj_2av_8sidedata_8sidedata__SideDataContainer *)__pyx_v_self), __pyx_v_frame);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -3150,112 +3164,112 @@
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "av/sidedata/sidedata.pyx":75
+  /* "av/sidedata/sidedata.pyx":77
  *     def __init__(self, Frame frame):
  * 
  *         self.frame = frame             # <<<<<<<<<<<<<<
  *         self._by_index = []
  *         self._by_type = {}
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_frame));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_frame));
   __Pyx_GOTREF(__pyx_v_self->frame);
   __Pyx_DECREF(((PyObject *)__pyx_v_self->frame));
   __pyx_v_self->frame = __pyx_v_frame;
 
-  /* "av/sidedata/sidedata.pyx":76
+  /* "av/sidedata/sidedata.pyx":78
  * 
  *         self.frame = frame
  *         self._by_index = []             # <<<<<<<<<<<<<<
  *         self._by_type = {}
  * 
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_by_index);
   __Pyx_DECREF(__pyx_v_self->_by_index);
   __pyx_v_self->_by_index = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/sidedata/sidedata.pyx":77
+  /* "av/sidedata/sidedata.pyx":79
  *         self.frame = frame
  *         self._by_index = []
  *         self._by_type = {}             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 77, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_by_type);
   __Pyx_DECREF(__pyx_v_self->_by_type);
   __pyx_v_self->_by_type = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "av/sidedata/sidedata.pyx":81
+  /* "av/sidedata/sidedata.pyx":83
  *         cdef int i
  *         cdef SideData data
  *         for i in range(self.frame.ptr.nb_side_data):             # <<<<<<<<<<<<<<
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)
  */
   __pyx_t_2 = __pyx_v_self->frame->ptr->nb_side_data;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "av/sidedata/sidedata.pyx":82
+    /* "av/sidedata/sidedata.pyx":84
  *         cdef SideData data
  *         for i in range(self.frame.ptr.nb_side_data):
  *             data = wrap_side_data(frame, i)             # <<<<<<<<<<<<<<
  *             self._by_index.append(data)
  *             self._by_type[data.type] = data
  */
-    __pyx_t_1 = ((PyObject *)__pyx_f_2av_8sidedata_8sidedata_wrap_side_data(__pyx_v_frame, __pyx_v_i)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
+    __pyx_t_1 = ((PyObject *)__pyx_f_2av_8sidedata_8sidedata_wrap_side_data(__pyx_v_frame, __pyx_v_i)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_data, ((struct __pyx_obj_2av_8sidedata_8sidedata_SideData *)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "av/sidedata/sidedata.pyx":83
+    /* "av/sidedata/sidedata.pyx":85
  *         for i in range(self.frame.ptr.nb_side_data):
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)             # <<<<<<<<<<<<<<
  *             self._by_type[data.type] = data
  * 
  */
     if (unlikely(__pyx_v_self->_by_index == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "append");
-      __PYX_ERR(0, 83, __pyx_L1_error)
+      __PYX_ERR(0, 85, __pyx_L1_error)
     }
-    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_self->_by_index, ((PyObject *)__pyx_v_data)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 83, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyList_Append(__pyx_v_self->_by_index, ((PyObject *)__pyx_v_data)); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(0, 85, __pyx_L1_error)
 
-    /* "av/sidedata/sidedata.pyx":84
+    /* "av/sidedata/sidedata.pyx":86
  *             data = wrap_side_data(frame, i)
  *             self._by_index.append(data)
  *             self._by_type[data.type] = data             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
     if (unlikely(__pyx_v_self->_by_type == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 84, __pyx_L1_error)
+      __PYX_ERR(0, 86, __pyx_L1_error)
     }
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 84, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_data), __pyx_n_s_type); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    if (unlikely(PyDict_SetItem(__pyx_v_self->_by_type, __pyx_t_1, ((PyObject *)__pyx_v_data)) < 0)) __PYX_ERR(0, 84, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_self->_by_type, __pyx_t_1, ((PyObject *)__pyx_v_data)) < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "av/sidedata/sidedata.pyx":73
+  /* "av/sidedata/sidedata.pyx":75
  * cdef class _SideDataContainer(object):
  * 
  *     def __init__(self, Frame frame):             # <<<<<<<<<<<<<<
  * 
  *         self.frame = frame
  */
 
@@ -3268,15 +3282,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_data);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":86
+/* "av/sidedata/sidedata.pyx":88
  *             self._by_type[data.type] = data
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self._by_index)
  * 
  */
 
@@ -3299,33 +3313,33 @@
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "av/sidedata/sidedata.pyx":87
+  /* "av/sidedata/sidedata.pyx":89
  * 
  *     def __len__(self):
  *         return len(self._by_index)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __pyx_t_1 = __pyx_v_self->_by_index;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 87, __pyx_L1_error)
+    __PYX_ERR(0, 89, __pyx_L1_error)
   }
-  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 87, __pyx_L1_error)
+  __pyx_t_2 = PyList_GET_SIZE(__pyx_t_1); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 89, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":86
+  /* "av/sidedata/sidedata.pyx":88
  *             self._by_type[data.type] = data
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return len(self._by_index)
  * 
  */
 
@@ -3335,15 +3349,15 @@
   __Pyx_AddTraceback("av.sidedata.sidedata._SideDataContainer.__len__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":89
+/* "av/sidedata/sidedata.pyx":91
  *         return len(self._by_index)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self._by_index)
  * 
  */
 
@@ -3366,32 +3380,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "av/sidedata/sidedata.pyx":90
+  /* "av/sidedata/sidedata.pyx":92
  * 
  *     def __iter__(self):
  *         return iter(self._by_index)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, key):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->_by_index;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+  __pyx_t_2 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":89
+  /* "av/sidedata/sidedata.pyx":91
  *         return len(self._by_index)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return iter(self._by_index)
  * 
  */
 
@@ -3403,15 +3417,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "av/sidedata/sidedata.pyx":92
+/* "av/sidedata/sidedata.pyx":94
  *         return iter(self._by_index)
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(key, int):
  */
 
@@ -3438,101 +3452,101 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "av/sidedata/sidedata.pyx":94
+  /* "av/sidedata/sidedata.pyx":96
  *     def __getitem__(self, key):
  * 
  *         if isinstance(key, int):             # <<<<<<<<<<<<<<
  *             return self._by_index[key]
  * 
  */
   __pyx_t_1 = PyInt_Check(__pyx_v_key); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "av/sidedata/sidedata.pyx":95
+    /* "av/sidedata/sidedata.pyx":97
  * 
  *         if isinstance(key, int):
  *             return self._by_index[key]             # <<<<<<<<<<<<<<
  * 
  *         type_ = Type.get(key)
  */
     __Pyx_XDECREF(__pyx_r);
     if (unlikely(__pyx_v_self->_by_index == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 95, __pyx_L1_error)
+      __PYX_ERR(0, 97, __pyx_L1_error)
     }
-    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_by_index, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 95, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetItem(__pyx_v_self->_by_index, __pyx_v_key); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "av/sidedata/sidedata.pyx":94
+    /* "av/sidedata/sidedata.pyx":96
  *     def __getitem__(self, key):
  * 
  *         if isinstance(key, int):             # <<<<<<<<<<<<<<
  *             return self._by_index[key]
  * 
  */
   }
 
-  /* "av/sidedata/sidedata.pyx":97
+  /* "av/sidedata/sidedata.pyx":99
  *             return self._by_index[key]
  * 
  *         type_ = Type.get(key)             # <<<<<<<<<<<<<<
  *         return self._by_type[type_]
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Type); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 97, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_get); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_v_key) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_v_key);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 97, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_v_type_ = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "av/sidedata/sidedata.pyx":98
+  /* "av/sidedata/sidedata.pyx":100
  * 
  *         type_ = Type.get(key)
  *         return self._by_type[type_]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   if (unlikely(__pyx_v_self->_by_type == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 98, __pyx_L1_error)
+    __PYX_ERR(0, 100, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->_by_type, __pyx_v_type_); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 98, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_GetItem(__pyx_v_self->_by_type, __pyx_v_type_); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "av/sidedata/sidedata.pyx":92
+  /* "av/sidedata/sidedata.pyx":94
  *         return iter(self._by_index)
  * 
  *     def __getitem__(self, key):             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(key, int):
  */
 
@@ -4659,14 +4673,15 @@
   {&__pyx_n_s_MOTION_VECTORS, __pyx_k_MOTION_VECTORS, sizeof(__pyx_k_MOTION_VECTORS), 0, 0, 1, 1},
   {&__pyx_n_s_Mapping, __pyx_k_Mapping, sizeof(__pyx_k_Mapping), 0, 0, 1, 1},
   {&__pyx_n_s_MotionVectors, __pyx_k_MotionVectors, sizeof(__pyx_k_MotionVectors), 0, 0, 1, 1},
   {&__pyx_n_s_PANSCAN, __pyx_k_PANSCAN, sizeof(__pyx_k_PANSCAN), 0, 0, 1, 1},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_REPLAYGAIN, __pyx_k_REPLAYGAIN, sizeof(__pyx_k_REPLAYGAIN), 0, 0, 1, 1},
   {&__pyx_n_s_RuntimeError, __pyx_k_RuntimeError, sizeof(__pyx_k_RuntimeError), 0, 0, 1, 1},
+  {&__pyx_n_s_SEI_UNREGISTERED, __pyx_k_SEI_UNREGISTERED, sizeof(__pyx_k_SEI_UNREGISTERED), 0, 0, 1, 1},
   {&__pyx_n_s_SKIP_SAMPLES, __pyx_k_SKIP_SAMPLES, sizeof(__pyx_k_SKIP_SAMPLES), 0, 0, 1, 1},
   {&__pyx_n_s_SPHERICAL, __pyx_k_SPHERICAL, sizeof(__pyx_k_SPHERICAL), 0, 0, 1, 1},
   {&__pyx_n_s_STEREO3D, __pyx_k_STEREO3D, sizeof(__pyx_k_STEREO3D), 0, 0, 1, 1},
   {&__pyx_n_s_SideData, __pyx_k_SideData, sizeof(__pyx_k_SideData), 0, 0, 1, 1},
   {&__pyx_n_s_SideDataContainer, __pyx_k_SideDataContainer, sizeof(__pyx_k_SideDataContainer), 0, 0, 1, 1},
   {&__pyx_n_s_SideDataContainer_2, __pyx_k_SideDataContainer_2, sizeof(__pyx_k_SideDataContainer_2), 0, 0, 1, 1},
   {&__pyx_n_s_Type, __pyx_k_Type, sizeof(__pyx_k_Type), 0, 0, 1, 1},
@@ -4717,34 +4732,34 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_type, __pyx_k_type, sizeof(__pyx_k_type), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_object = __Pyx_GetBuiltinName(__pyx_n_s_object); if (!__pyx_builtin_object) __PYX_ERR(0, 8, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 51, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(1, 2, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 83, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "av/sidedata/sidedata.pyx":49
+  /* "av/sidedata/sidedata.pyx":51
  *     def __init__(self, sentinel, Frame frame, int index):
  *         if sentinel is not _cinit_bypass_sentinel:
  *             raise RuntimeError('cannot manually instatiate SideData')             # <<<<<<<<<<<<<<
  *         self.frame = frame
  *         self.ptr = frame.ptr.side_data[index]
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_cannot_manually_instatiate_SideD); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_cannot_manually_instatiate_SideD); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 51, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("self.ptr cannot be converted to a Python object for pickling")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -4842,34 +4857,34 @@
   __pyx_vtabptr_2av_6buffer_Buffer = (struct __pyx_vtabstruct_2av_6buffer_Buffer*)__Pyx_GetVtable(__pyx_ptype_2av_6buffer_Buffer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_6buffer_Buffer)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_vtabptr_2av_8sidedata_8sidedata_SideData = &__pyx_vtable_2av_8sidedata_8sidedata_SideData;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base = *__pyx_vtabptr_2av_6buffer_Buffer;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_size = (size_t (*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_size;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_ptr = (void *(*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_ptr;
   __pyx_vtable_2av_8sidedata_8sidedata_SideData.__pyx_base._buffer_writable = (int (*)(struct __pyx_obj_2av_6buffer_Buffer *))__pyx_f_2av_8sidedata_8sidedata_8SideData__buffer_writable;
   __pyx_type_2av_8sidedata_8sidedata_SideData.tp_base = __pyx_ptype_2av_6buffer_Buffer;
-  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_8sidedata_8sidedata_SideData.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dictoffset && __pyx_type_2av_8sidedata_8sidedata_SideData.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_8sidedata_8sidedata_SideData.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dict, __pyx_vtabptr_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideData, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_2av_8sidedata_8sidedata_SideData.tp_dict, __pyx_vtabptr_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideData, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata_SideData) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
   __pyx_ptype_2av_8sidedata_8sidedata_SideData = &__pyx_type_2av_8sidedata_8sidedata_SideData;
-  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_dictoffset && __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type_2av_8sidedata_8sidedata__SideDataContainer.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideDataContainer, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 71, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_SideDataContainer, (PyObject *)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_2av_8sidedata_8sidedata__SideDataContainer) < 0) __PYX_ERR(0, 73, __pyx_L1_error)
   __pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer = &__pyx_type_2av_8sidedata_8sidedata__SideDataContainer;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -4903,18 +4918,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -5095,14 +5110,16 @@
   PyObject *__pyx_t_12 = NULL;
   PyObject *__pyx_t_13 = NULL;
   PyObject *__pyx_t_14 = NULL;
   PyObject *__pyx_t_15 = NULL;
   PyObject *__pyx_t_16 = NULL;
   PyObject *__pyx_t_17 = NULL;
   PyObject *__pyx_t_18 = NULL;
+  PyObject *__pyx_t_19 = NULL;
+  PyObject *__pyx_t_20 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -5523,15 +5540,15 @@
   __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":26
  *     ('GOP_TIMECODE', lib.AV_FRAME_DATA_GOP_TIMECODE),
  *     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
  *     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),             # <<<<<<<<<<<<<<
  *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
- * 
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
  */
   __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_CONTENT_LIGHT_LEVEL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_17 = PyTuple_New(2); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_17);
   __Pyx_INCREF(__pyx_n_s_CONTENT_LIGHT_LEVEL);
   __Pyx_GIVEREF(__pyx_n_s_CONTENT_LIGHT_LEVEL);
@@ -5540,69 +5557,96 @@
   PyTuple_SET_ITEM(__pyx_t_17, 1, __pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":27
  *     ('SPHERICAL', lib.AV_FRAME_DATA_SPHERICAL),
  *     ('CONTENT_LIGHT_LEVEL', lib.AV_FRAME_DATA_CONTENT_LIGHT_LEVEL),
  *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),             # <<<<<<<<<<<<<<
- * 
- *     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+ *     ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,
  */
   __pyx_t_2 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_ICC_PROFILE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_18 = PyTuple_New(2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_18);
   __Pyx_INCREF(__pyx_n_s_ICC_PROFILE);
   __Pyx_GIVEREF(__pyx_n_s_ICC_PROFILE);
   PyTuple_SET_ITEM(__pyx_t_18, 0, __pyx_n_s_ICC_PROFILE);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_18, 1, __pyx_t_2);
   __pyx_t_2 = 0;
 
+  /* "av/sidedata/sidedata.pyx":29
+ *     ('ICC_PROFILE', lib.AV_FRAME_DATA_ICC_PROFILE),
+ *     # SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+ *     ('SEI_UNREGISTERED', lib.AV_FRAME_DATA_SEI_UNREGISTERED) if lib.AV_FRAME_DATA_SEI_UNREGISTERED != -1 else None,             # <<<<<<<<<<<<<<
+ * 
+ *     # These are deprecated. See https://github.com/PyAV-Org/PyAV/issues/607
+ */
+  if (((AV_FRAME_DATA_SEI_UNREGISTERED != -1L) != 0)) {
+    __pyx_t_19 = __Pyx_PyInt_From_enum__AVFrameSideDataType(AV_FRAME_DATA_SEI_UNREGISTERED); if (unlikely(!__pyx_t_19)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_19);
+    __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_20);
+    __Pyx_INCREF(__pyx_n_s_SEI_UNREGISTERED);
+    __Pyx_GIVEREF(__pyx_n_s_SEI_UNREGISTERED);
+    PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_n_s_SEI_UNREGISTERED);
+    __Pyx_GIVEREF(__pyx_t_19);
+    PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_19);
+    __pyx_t_19 = 0;
+    __pyx_t_2 = __pyx_t_20;
+    __pyx_t_20 = 0;
+  } else {
+    __Pyx_INCREF(Py_None);
+    __pyx_t_2 = Py_None;
+  }
+
   /* "av/sidedata/sidedata.pyx":12
  * 
  * Type = define_enum('Type', __name__, (
  *     ('PANSCAN', lib.AV_FRAME_DATA_PANSCAN),             # <<<<<<<<<<<<<<
  *     ('A53_CC', lib.AV_FRAME_DATA_A53_CC),
  *     ('STEREO3D', lib.AV_FRAME_DATA_STEREO3D),
  */
-  __pyx_t_2 = PyTuple_New(16); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 12, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(17); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 12, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
   __Pyx_GIVEREF(__pyx_t_3);
-  PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_20, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_5);
-  PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
+  PyTuple_SET_ITEM(__pyx_t_20, 2, __pyx_t_5);
   __Pyx_GIVEREF(__pyx_t_6);
-  PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_6);
+  PyTuple_SET_ITEM(__pyx_t_20, 3, __pyx_t_6);
   __Pyx_GIVEREF(__pyx_t_7);
-  PyTuple_SET_ITEM(__pyx_t_2, 4, __pyx_t_7);
+  PyTuple_SET_ITEM(__pyx_t_20, 4, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_8);
-  PyTuple_SET_ITEM(__pyx_t_2, 5, __pyx_t_8);
+  PyTuple_SET_ITEM(__pyx_t_20, 5, __pyx_t_8);
   __Pyx_GIVEREF(__pyx_t_9);
-  PyTuple_SET_ITEM(__pyx_t_2, 6, __pyx_t_9);
+  PyTuple_SET_ITEM(__pyx_t_20, 6, __pyx_t_9);
   __Pyx_GIVEREF(__pyx_t_10);
-  PyTuple_SET_ITEM(__pyx_t_2, 7, __pyx_t_10);
+  PyTuple_SET_ITEM(__pyx_t_20, 7, __pyx_t_10);
   __Pyx_GIVEREF(__pyx_t_11);
-  PyTuple_SET_ITEM(__pyx_t_2, 8, __pyx_t_11);
+  PyTuple_SET_ITEM(__pyx_t_20, 8, __pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_12);
-  PyTuple_SET_ITEM(__pyx_t_2, 9, __pyx_t_12);
+  PyTuple_SET_ITEM(__pyx_t_20, 9, __pyx_t_12);
   __Pyx_GIVEREF(__pyx_t_13);
-  PyTuple_SET_ITEM(__pyx_t_2, 10, __pyx_t_13);
+  PyTuple_SET_ITEM(__pyx_t_20, 10, __pyx_t_13);
   __Pyx_GIVEREF(__pyx_t_14);
-  PyTuple_SET_ITEM(__pyx_t_2, 11, __pyx_t_14);
+  PyTuple_SET_ITEM(__pyx_t_20, 11, __pyx_t_14);
   __Pyx_GIVEREF(__pyx_t_15);
-  PyTuple_SET_ITEM(__pyx_t_2, 12, __pyx_t_15);
+  PyTuple_SET_ITEM(__pyx_t_20, 12, __pyx_t_15);
   __Pyx_GIVEREF(__pyx_t_16);
-  PyTuple_SET_ITEM(__pyx_t_2, 13, __pyx_t_16);
+  PyTuple_SET_ITEM(__pyx_t_20, 13, __pyx_t_16);
   __Pyx_GIVEREF(__pyx_t_17);
-  PyTuple_SET_ITEM(__pyx_t_2, 14, __pyx_t_17);
+  PyTuple_SET_ITEM(__pyx_t_20, 14, __pyx_t_17);
   __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_2, 15, __pyx_t_18);
+  PyTuple_SET_ITEM(__pyx_t_20, 15, __pyx_t_18);
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 16, __pyx_t_2);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_t_5 = 0;
   __pyx_t_6 = 0;
   __pyx_t_7 = 0;
   __pyx_t_8 = 0;
   __pyx_t_9 = 0;
@@ -5611,76 +5655,77 @@
   __pyx_t_12 = 0;
   __pyx_t_13 = 0;
   __pyx_t_14 = 0;
   __pyx_t_15 = 0;
   __pyx_t_16 = 0;
   __pyx_t_17 = 0;
   __pyx_t_18 = 0;
+  __pyx_t_2 = 0;
 
   /* "av/sidedata/sidedata.pyx":11
  * 
  * 
  * Type = define_enum('Type', __name__, (             # <<<<<<<<<<<<<<
  *     ('PANSCAN', lib.AV_FRAME_DATA_PANSCAN),
  *     ('A53_CC', lib.AV_FRAME_DATA_A53_CC),
  */
-  __pyx_t_18 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Type, __pyx_t_1, __pyx_t_2, 0, NULL); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
+  __pyx_t_2 = __pyx_f_2av_4enum_define_enum(__pyx_n_s_Type, __pyx_t_1, __pyx_t_20, 0, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 11, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_2) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_Type, __pyx_t_18) < 0) __PYX_ERR(0, 11, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
 
-  /* "av/sidedata/sidedata.pyx":101
+  /* "av/sidedata/sidedata.pyx":103
  * 
  * 
  * class SideDataContainer(_SideDataContainer, Mapping):             # <<<<<<<<<<<<<<
  *     pass
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_18, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 101, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Mapping); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_20 = PyTuple_New(2); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
   __Pyx_INCREF(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
   __Pyx_GIVEREF(((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
-  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
-  __Pyx_GIVEREF(__pyx_t_18);
-  PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_18);
-  __pyx_t_18 = 0;
-  __pyx_t_18 = __Pyx_CalculateMetaclass(NULL, __pyx_t_2); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_18);
-  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_18, __pyx_t_2, __pyx_n_s_SideDataContainer_2, __pyx_n_s_SideDataContainer_2, (PyObject *) NULL, __pyx_n_s_av_sidedata_sidedata, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 101, __pyx_L1_error)
+  PyTuple_SET_ITEM(__pyx_t_20, 0, ((PyObject *)__pyx_ptype_2av_8sidedata_8sidedata__SideDataContainer));
+  __Pyx_GIVEREF(__pyx_t_2);
+  PyTuple_SET_ITEM(__pyx_t_20, 1, __pyx_t_2);
+  __pyx_t_2 = 0;
+  __pyx_t_2 = __Pyx_CalculateMetaclass(NULL, __pyx_t_20); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_Py3MetaclassPrepare(__pyx_t_2, __pyx_t_20, __pyx_n_s_SideDataContainer_2, __pyx_n_s_SideDataContainer_2, (PyObject *) NULL, __pyx_n_s_av_sidedata_sidedata, (PyObject *) NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_17 = __Pyx_Py3ClassCreate(__pyx_t_18, __pyx_n_s_SideDataContainer_2, __pyx_t_2, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_17)) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_17);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SideDataContainer_2, __pyx_t_17) < 0) __PYX_ERR(0, 101, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_17); __pyx_t_17 = 0;
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_18 = __Pyx_Py3ClassCreate(__pyx_t_2, __pyx_n_s_SideDataContainer_2, __pyx_t_20, __pyx_t_1, NULL, 0, 1); if (unlikely(!__pyx_t_18)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_18);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SideDataContainer_2, __pyx_t_18) < 0) __PYX_ERR(0, 103, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_18); __pyx_t_18 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle__SideDataContainer(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_2av_8sidedata_8sidedata_1__pyx_unpickle__SideDataContainer, NULL, __pyx_n_s_av_sidedata_sidedata); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle__SideDataContaine, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_20 = PyCFunction_NewEx(&__pyx_mdef_2av_8sidedata_8sidedata_1__pyx_unpickle__SideDataContainer, NULL, __pyx_n_s_av_sidedata_sidedata); if (unlikely(!__pyx_t_20)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle__SideDataContaine, __pyx_t_20) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /* "av/sidedata/sidedata.pyx":1
  * from av.enum cimport define_enum             # <<<<<<<<<<<<<<
  * 
  * from collections.abc import Mapping
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_20 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_20)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_20);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_20) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_20); __pyx_t_20 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -5696,14 +5741,16 @@
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
   __Pyx_XDECREF(__pyx_t_16);
   __Pyx_XDECREF(__pyx_t_17);
   __Pyx_XDECREF(__pyx_t_18);
+  __Pyx_XDECREF(__pyx_t_19);
+  __Pyx_XDECREF(__pyx_t_20);
   if (__pyx_m) {
     if (__pyx_d) {
       __Pyx_AddTraceback("init av.sidedata.sidedata", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
     PyErr_SetString(PyExc_ImportError, "init av.sidedata.sidedata");
```

### Comparing `av-9.1.1/src/av/stream.c` & `av-9.2.0/src/av/stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1283,28 +1291,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1354,15 +1363,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -5937,18 +5949,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/subtitles/codeccontext.c` & `av-9.2.0/src/av/subtitles/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1188,28 +1196,29 @@
  */
 struct __pyx_obj_2av_6buffer_Buffer {
   PyObject_HEAD
   struct __pyx_vtabstruct_2av_6buffer_Buffer *__pyx_vtab;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1273,15 +1282,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2649,18 +2661,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.buffer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_6buffer_Buffer = __Pyx_ImportType(__pyx_t_1, "av.buffer", "Buffer", sizeof(struct __pyx_obj_2av_6buffer_Buffer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_6buffer_Buffer) __PYX_ERR(4, 2, __pyx_L1_error)
   __pyx_vtabptr_2av_6buffer_Buffer = (struct __pyx_vtabstruct_2av_6buffer_Buffer*)__Pyx_GetVtable(__pyx_ptype_2av_6buffer_Buffer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_6buffer_Buffer)) __PYX_ERR(4, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(5, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(5, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(6, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(6, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/subtitles/stream.c` & `av-9.2.0/src/av/subtitles/stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1242,28 +1250,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1313,15 +1322,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2338,18 +2350,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/subtitles/subtitle.c` & `av-9.2.0/src/av/subtitles/subtitle.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1245,28 +1253,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1316,15 +1325,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -8748,18 +8760,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/utils.c` & `av-9.2.0/src/av/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/video/codeccontext.c` & `av-9.2.0/src/av/video/codeccontext.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1214,28 +1222,29 @@
  */
 struct __pyx_obj_2av_6buffer_Buffer {
   PyObject_HEAD
   struct __pyx_vtabstruct_2av_6buffer_Buffer *__pyx_vtab;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1299,15 +1308,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -4983,18 +4995,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.buffer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_6buffer_Buffer = __Pyx_ImportType(__pyx_t_1, "av.buffer", "Buffer", sizeof(struct __pyx_obj_2av_6buffer_Buffer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_6buffer_Buffer) __PYX_ERR(5, 2, __pyx_L1_error)
   __pyx_vtabptr_2av_6buffer_Buffer = (struct __pyx_vtabstruct_2av_6buffer_Buffer*)__Pyx_GetVtable(__pyx_ptype_2av_6buffer_Buffer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_6buffer_Buffer)) __PYX_ERR(5, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/video/format.c` & `av-9.2.0/src/av/video/format.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
```

### Comparing `av-9.1.1/src/av/video/frame.c` & `av-9.2.0/src/av/video/frame.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1379,28 +1387,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1464,15 +1473,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -23988,18 +24000,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/video/plane.c` & `av-9.2.0/src/av/video/plane.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1201,28 +1209,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1286,15 +1295,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -3213,18 +3225,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(6, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(6, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(7, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(8, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(8, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/video/reformatter.c` & `av-9.2.0/src/av/video/reformatter.c`

 * *Files 1% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1257,28 +1265,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1342,15 +1351,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -3705,18 +3717,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(5, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(5, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(6, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(7, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(7, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/src/av/video/stream.c` & `av-9.2.0/src/av/video/stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,22 @@
 #include "libavutil/log.h"
 #include "libavutil/dict.h"
 #include "libavutil/error.h"
 #include "libavutil/frame.h"
 #include "libavutil/samplefmt.h"
 #include "libavutil/motion_vector.h"
 #include "libavcodec/avcodec.h"
+
+    // AV_FRAME_DATA_SEI_UNREGISTERED available since version 56.54.100 of libavutil (FFmpeg >= 4.4)
+    #define HAS_AV_FRAME_DATA_SEI_UNREGISTERED  (LIBAVUTIL_VERSION_INT >= 3683940)
+
+    #if !HAS_AV_FRAME_DATA_SEI_UNREGISTERED
+        #define AV_FRAME_DATA_SEI_UNREGISTERED -1
+    #endif
+    
 #include "libavdevice/avdevice.h"
 #include "libavformat/avformat.h"
 #include "libswresample/swresample.h"
 #include "libswscale/swscale.h"
 #include "libavfilter/avfilter.h"
 #include "libavfilter/buffersink.h"
 #include "libavfilter/buffersrc.h"
@@ -1242,28 +1250,29 @@
   struct AVCodecParserContext *parser;
   struct __pyx_obj_2av_5codec_5codec_Codec *codec;
   PyObject *options;
   struct __pyx_obj_2av_5frame_Frame *_next_frame;
 };
 
 
-/* "av/container/pyio.pxd":11
- * cdef int64_t pyio_seek(void *opaque, int64_t offset, int whence) nogil
+/* "av/container/pyio.pxd":16
+ * 
  * 
  * cdef class PyIOFile(object):             # <<<<<<<<<<<<<<
  * 
  *     # File-like source.
  */
 struct __pyx_obj_2av_9container_4pyio_PyIOFile {
   PyObject_HEAD
   PyObject *file;
   PyObject *fread;
   PyObject *fwrite;
   PyObject *fseek;
   PyObject *ftell;
+  PyObject *fclose;
   struct AVIOContext *iocontext;
   unsigned char *buffer;
   long pos;
   int pos_is_valid;
 };
 
 
@@ -1313,15 +1322,18 @@
   struct __pyx_vtabstruct_2av_9container_4core_Container *__pyx_vtab;
   int writeable;
   struct AVFormatContext *ptr;
   PyObject *name;
   PyObject *metadata_encoding;
   PyObject *metadata_errors;
   struct __pyx_obj_2av_9container_4pyio_PyIOFile *file;
+  int buffer_size;
   int input_was_opened;
+  PyObject *io_open;
+  PyObject *open_files;
   struct __pyx_obj_2av_6format_ContainerFormat *format;
   PyObject *options;
   PyObject *container_options;
   PyObject *stream_options;
   struct __pyx_obj_2av_9container_7streams_StreamContainer *streams;
   PyObject *metadata;
   PyObject *open_timeout;
@@ -2606,18 +2618,18 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.codec.context"); if (unlikely(!__pyx_t_1)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_5codec_7context_CodecContext = __Pyx_ImportType(__pyx_t_1, "av.codec.context", "CodecContext", sizeof(struct __pyx_obj_2av_5codec_7context_CodecContext), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_5codec_7context_CodecContext) __PYX_ERR(9, 10, __pyx_L1_error)
   __pyx_vtabptr_2av_5codec_7context_CodecContext = (struct __pyx_vtabstruct_2av_5codec_7context_CodecContext*)__Pyx_GetVtable(__pyx_ptype_2av_5codec_7context_CodecContext->tp_dict); if (unlikely(!__pyx_vtabptr_2av_5codec_7context_CodecContext)) __PYX_ERR(9, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 11, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("av.container.pyio"); if (unlikely(!__pyx_t_1)) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_4pyio_PyIOFile = __Pyx_ImportType(__pyx_t_1, "av.container.pyio", "PyIOFile", sizeof(struct __pyx_obj_2av_9container_4pyio_PyIOFile), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 11, __pyx_L1_error)
+   if (!__pyx_ptype_2av_9container_4pyio_PyIOFile) __PYX_ERR(10, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("av.container.streams"); if (unlikely(!__pyx_t_1)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2av_9container_7streams_StreamContainer = __Pyx_ImportType(__pyx_t_1, "av.container.streams", "StreamContainer", sizeof(struct __pyx_obj_2av_9container_7streams_StreamContainer), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_2av_9container_7streams_StreamContainer) __PYX_ERR(11, 4, __pyx_L1_error)
   __pyx_vtabptr_2av_9container_7streams_StreamContainer = (struct __pyx_vtabstruct_2av_9container_7streams_StreamContainer*)__Pyx_GetVtable(__pyx_ptype_2av_9container_7streams_StreamContainer->tp_dict); if (unlikely(!__pyx_vtabptr_2av_9container_7streams_StreamContainer)) __PYX_ERR(11, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
```

### Comparing `av-9.1.1/tests/common.py` & `av-9.2.0/tests/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,27 @@
         raise TypeError("extra kwargs: %s" % ", ".join(sorted(kwargs)))
     path = os.path.join(_sandbox(timed=timed) if base is None else base, *args)
     if do_makedirs:
         makedirs(os.path.dirname(path))
     return path
 
 
+# Decorator for running a test in the sandbox directory
+def run_in_sandbox(func):
+    @functools.wraps(func)
+    def _inner(self, *args, **kwargs):
+        current_dir = os.getcwd()
+        try:
+            os.chdir(self.sandbox)
+            return func(self, *args, **kwargs)
+        finally:
+            os.chdir(current_dir)
+    return _inner
+
+
 class MethodLogger(object):
     def __init__(self, obj):
         self._obj = obj
         self._log = []
 
     def __getattr__(self, name):
         value = getattr(self._obj, name)
```

### Comparing `av-9.1.1/tests/test_audiofifo.py` & `av-9.2.0/tests/test_audiofifo.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_audioformat.py` & `av-9.2.0/tests/test_audioformat.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_audioframe.py` & `av-9.2.0/tests/test_audioframe.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_audiolayout.py` & `av-9.2.0/tests/test_audiolayout.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_audioresampler.py` & `av-9.2.0/tests/test_audioresampler.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_codec.py` & `av-9.2.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_codec_context.py` & `av-9.2.0/tests/test_codec_context.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_containerformat.py` & `av-9.2.0/tests/test_containerformat.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_decode.py` & `av-9.2.0/tests/test_decode.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_deprecation.py` & `av-9.2.0/tests/test_deprecation.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_doctests.py` & `av-9.2.0/tests/test_doctests.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_encode.py` & `av-9.2.0/tests/test_encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,29 +59,39 @@
         for packet in stream.encode(frame):
             output.mux(packet)
 
     for packet in stream.encode(None):
         output.mux(packet)
 
 
-def assert_rgb_rotate(self, input_):
+def assert_rgb_rotate(self, input_, is_dash=False):
 
     # Now inspect it a little.
     self.assertEqual(len(input_.streams), 1)
-    self.assertEqual(input_.metadata.get("title"), "container", input_.metadata)
+    if is_dash:
+        # FFmpeg 4.2 added parsing of the programme information and it is named "Title"
+        if av.library_versions["libavformat"] >= (58, 28):
+            self.assertTrue(input_.metadata.get("Title") == "container", input_.metadata)
+    else:
+        self.assertEqual(input_.metadata.get("title"), "container", input_.metadata)
     self.assertEqual(input_.metadata.get("key"), None)
     stream = input_.streams[0]
     self.assertIsInstance(stream, VideoStream)
     self.assertEqual(stream.type, "video")
     self.assertEqual(stream.name, "mpeg4")
     self.assertEqual(
         stream.average_rate, 24
     )  # Only because we constructed is precisely.
     self.assertEqual(stream.rate, Fraction(24, 1))
-    self.assertEqual(stream.time_base * stream.duration, 2)
+    if is_dash:
+        # The DASH format doesn't provide a duration for the stream
+        # and so the container duration (micro seconds) is checked instead
+        self.assertEqual(input_.duration, 2000000)
+    else:
+        self.assertEqual(stream.time_base * stream.duration, 2)
     self.assertEqual(stream.format.name, "yuv420p")
     self.assertEqual(stream.format.width, WIDTH)
     self.assertEqual(stream.format.height, HEIGHT)
 
 
 class TestBasicVideoEncoding(TestCase):
     def test_default_options(self):
```

### Comparing `av-9.1.1/tests/test_enums.py` & `av-9.2.0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_errors.py` & `av-9.2.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_file_probing.py` & `av-9.2.0/tests/test_file_probing.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_filters.py` & `av-9.2.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_logging.py` & `av-9.2.0/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_options.py` & `av-9.2.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_seek.py` & `av-9.2.0/tests/test_seek.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_streams.py` & `av-9.2.0/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_subtitles.py` & `av-9.2.0/tests/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_timeout.py` & `av-9.2.0/tests/test_timeout.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_videoformat.py` & `av-9.2.0/tests/test_videoformat.py`

 * *Files identical despite different names*

### Comparing `av-9.1.1/tests/test_videoframe.py` & `av-9.2.0/tests/test_videoframe.py`

 * *Files identical despite different names*

