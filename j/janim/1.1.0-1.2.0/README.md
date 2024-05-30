# Comparing `tmp/janim-1.1.0.tar.gz` & `tmp/janim-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janim-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "janim-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `janim-1.1.0.tar` & `janim-1.2.0.tar`

### file list

```diff
@@ -1,101 +1,102 @@
--rw-r--r--   0        0        0      491 2024-05-27 02:44:21.173265 janim-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      153 2024-05-27 02:44:21.173265 janim-1.1.0/.gitignore
--rw-r--r--   0        0        0       27 2024-05-27 02:44:21.173265 janim-1.1.0/.pypirc
--rw-r--r--   0        0        0     1011 2024-05-27 02:44:21.173265 janim-1.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0     1085 2024-05-27 02:44:21.173265 janim-1.1.0/LICENSE
--rw-r--r--   0        0        0     1208 2024-05-27 02:44:21.173265 janim-1.1.0/README.md
--rw-r--r--   0        0        0       68 2024-05-27 02:44:21.217265 janim-1.1.0/janim/__init__.py
--rw-r--r--   0        0        0     3025 2024-05-27 02:44:21.217265 janim-1.1.0/janim/__main__.py
--rw-r--r--   0        0        0     4108 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/animation.py
--rw-r--r--   0        0        0     6203 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/composition.py
--rw-r--r--   0        0        0     5842 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/creation.py
--rw-r--r--   0        0        0      784 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/display.py
--rw-r--r--   0        0        0     3329 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/fading.py
--rw-r--r--   0        0        0     3799 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/growing.py
--rw-r--r--   0        0        0    12480 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/indication.py
--rw-r--r--   0        0        0     2375 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/movement.py
--rw-r--r--   0        0        0     1501 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/rotation.py
--rw-r--r--   0        0        0    27706 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/timeline.py
--rw-r--r--   0        0        0     8961 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/transform.py
--rw-r--r--   0        0        0     9662 2024-05-27 02:44:21.217265 janim-1.1.0/janim/anims/updater.py
--rw-r--r--   0        0        0     4360 2024-05-27 02:44:21.217265 janim-1.1.0/janim/camera/camera.py
--rw-r--r--   0        0        0     2665 2024-05-27 02:44:21.217265 janim-1.1.0/janim/camera/camera_info.py
--rw-r--r--   0        0        0     6647 2024-05-27 02:44:21.217265 janim-1.1.0/janim/cli.py
--rw-r--r--   0        0        0     8927 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/component.py
--rw-r--r--   0        0        0     2331 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/data.py
--rw-r--r--   0        0        0     2518 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/depth.py
--rw-r--r--   0        0        0     1239 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/image.py
--rw-r--r--   0        0        0    30089 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/points.py
--rw-r--r--   0        0        0     2733 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/radius.py
--rw-r--r--   0        0        0     7677 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/rgbas.py
--rw-r--r--   0        0        0    21993 2024-05-27 02:44:21.217265 janim-1.1.0/janim/components/vpoints.py
--rw-r--r--   0        0        0      236 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/__init__.py
--rw-r--r--   0        0        0      162 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/alignment.py
--rw-r--r--   0        0        0     1469 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/colors.py
--rw-r--r--   0        0        0      614 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/coord.py
--rw-r--r--   0        0        0      171 2024-05-27 02:44:21.217265 janim-1.1.0/janim/constants/degrees.py
--rw-r--r--   0        0        0     5265 2024-05-27 02:44:21.217265 janim-1.1.0/janim/examples.py
--rw-r--r--   0        0        0     1654 2024-05-27 02:44:21.217265 janim-1.1.0/janim/exception.py
--rw-r--r--   0        0        0    41845 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/anim_viewer.py
--rw-r--r--   0        0        0      319 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/application.py
--rw-r--r--   0        0        0      766 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/audio_player.py
--rw-r--r--   0        0        0     3181 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/export.png
--rw-r--r--   0        0        0    16958 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/favicon.ico
--rw-r--r--   0        0        0     1491 2024-05-27 02:44:21.217265 janim-1.1.0/janim/gui/fixed_ratio_widget.py
--rw-r--r--   0        0        0     1419 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/glwidget.py
--rw-r--r--   0        0        0      869 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/precise_timer.py
--rw-r--r--   0        0        0     5115 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/richtext_editor.py
--rw-r--r--   0        0        0     8115 2024-05-27 02:44:21.221265 janim-1.1.0/janim/gui/selector.py
--rw-r--r--   0        0        0     1699 2024-05-27 02:44:21.221265 janim-1.1.0/janim/imports.py
--rw-r--r--   0        0        0     7886 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/audio.py
--rw-r--r--   0        0        0     5190 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/boolean_ops.py
--rw-r--r--   0        0        0     8569 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/coordinate_systems.py
--rw-r--r--   0        0        0     2093 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/functions.py
--rw-r--r--   0        0        0     8078 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/coordinate/number_line.py
--rw-r--r--   0        0        0     8471 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/arc.py
--rw-r--r--   0        0        0     6679 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/arrow.py
--rw-r--r--   0        0        0     7653 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/line.py
--rw-r--r--   0        0        0     5077 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/geometry/polygon.py
--rw-r--r--   0        0        0     5071 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/image_item.py
--rw-r--r--   0        0        0    18487 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/item.py
--rw-r--r--   0        0        0     3150 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/points.py
--rw-r--r--   0        0        0     7446 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/relation.py
--rw-r--r--   0        0        0     2012 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/shape_matchers.py
--rw-r--r--   0        0        0     5764 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/brace.py
--rw-r--r--   0        0        0     1719 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/brace.svg
--rw-r--r--   0        0        0     4298 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/svg_item.py
--rw-r--r--   0        0        0     2979 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/typst.py
--rw-r--r--   0        0        0       37 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/svg/typst_template.typ
--rw-r--r--   0        0        0    15793 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/text/text.py
--rw-r--r--   0        0        0     1053 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/value_tracker.py
--rw-r--r--   0        0        0     5204 2024-05-27 02:44:21.221265 janim-1.1.0/janim/items/vitem.py
--rw-r--r--   0        0        0      258 2024-05-27 02:44:21.221265 janim-1.1.0/janim/logger.py
--rw-r--r--   0        0        0     2951 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/base.py
--rw-r--r--   0        0        0     8622 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/impl.py
--rw-r--r--   0        0        0      427 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.frag.glsl
--rw-r--r--   0        0        0     1200 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.geom.glsl
--rw-r--r--   0        0        0      306 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/dotcloud.vert.glsl
--rw-r--r--   0        0        0      167 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/image.frag.glsl
--rw-r--r--   0        0        0      332 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/image.vert.glsl
--rw-r--r--   0        0        0     6752 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/vitem.frag.glsl
--rw-r--r--   0        0        0      190 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/shaders/vitem.vert.glsl
--rw-r--r--   0        0        0     1069 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/texture.py
--rw-r--r--   0        0        0     6771 2024-05-27 02:44:21.221265 janim-1.1.0/janim/render/writer.py
--rw-r--r--   0        0        0      931 2024-05-27 02:44:21.221265 janim-1.1.0/janim/typing.py
--rw-r--r--   0        0        0    16826 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/bezier.py
--rw-r--r--   0        0        0     5297 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/config.py
--rw-r--r--   0        0        0     5590 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/data.py
--rw-r--r--   0        0        0      618 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/dict_ops.py
--rw-r--r--   0        0        0     2400 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/file_ops.py
--rw-r--r--   0        0        0     2896 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/font.py
--rw-r--r--   0        0        0     6192 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/font_manager.py
--rw-r--r--   0        0        0     5767 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/iterables.py
--rw-r--r--   0        0        0     1810 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/paths.py
--rw-r--r--   0        0        0     2601 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/rate_functions.py
--rw-r--r--   0        0        0     2566 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/refresh.py
--rw-r--r--   0        0        0     8074 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/signal.py
--rw-r--r--   0        0        0     1919 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/simple_functions.py
--rw-r--r--   0        0        0     9707 2024-05-27 02:44:21.221265 janim-1.1.0/janim/utils/space_ops.py
--rw-r--r--   0        0        0    18504 2024-05-27 02:44:21.221265 janim-1.1.0/logo.png
--rw-r--r--   0        0        0      985 2024-05-27 02:44:21.221265 janim-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 janim-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2024-05-30 01:22:23.686382 janim-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1011 2024-05-30 01:22:23.686382 janim-1.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1085 2024-05-30 01:22:23.686382 janim-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1208 2024-05-30 01:22:23.686382 janim-1.2.0/README.md
+-rw-r--r--   0        0        0       68 2024-05-30 01:22:23.726382 janim-1.2.0/janim/__init__.py
+-rw-r--r--   0        0        0     3412 2024-05-30 01:22:23.726382 janim-1.2.0/janim/__main__.py
+-rw-r--r--   0        0        0     4108 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/animation.py
+-rw-r--r--   0        0        0     6203 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/composition.py
+-rw-r--r--   0        0        0     5842 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/creation.py
+-rw-r--r--   0        0        0      784 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/display.py
+-rw-r--r--   0        0        0     3339 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/fading.py
+-rw-r--r--   0        0        0     3799 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/growing.py
+-rw-r--r--   0        0        0    12480 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/indication.py
+-rw-r--r--   0        0        0     2375 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/movement.py
+-rw-r--r--   0        0        0     1501 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/rotation.py
+-rw-r--r--   0        0        0    28675 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/timeline.py
+-rw-r--r--   0        0        0     8961 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/transform.py
+-rw-r--r--   0        0        0     9907 2024-05-30 01:22:23.726382 janim-1.2.0/janim/anims/updater.py
+-rw-r--r--   0        0        0     4360 2024-05-30 01:22:23.726382 janim-1.2.0/janim/camera/camera.py
+-rw-r--r--   0        0        0     2768 2024-05-30 01:22:23.726382 janim-1.2.0/janim/camera/camera_info.py
+-rw-r--r--   0        0        0     7387 2024-05-30 01:22:23.726382 janim-1.2.0/janim/cli.py
+-rw-r--r--   0        0        0     8927 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/component.py
+-rw-r--r--   0        0        0     2331 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/data.py
+-rw-r--r--   0        0        0     2518 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/depth.py
+-rw-r--r--   0        0        0     1239 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/image.py
+-rw-r--r--   0        0        0    30723 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/points.py
+-rw-r--r--   0        0        0     2733 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/radius.py
+-rw-r--r--   0        0        0     7677 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/rgbas.py
+-rw-r--r--   0        0        0    21993 2024-05-30 01:22:23.726382 janim-1.2.0/janim/components/vpoints.py
+-rw-r--r--   0        0        0      236 2024-05-30 01:22:23.726382 janim-1.2.0/janim/constants/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-30 01:22:23.726382 janim-1.2.0/janim/constants/alignment.py
+-rw-r--r--   0        0        0     1469 2024-05-30 01:22:23.726382 janim-1.2.0/janim/constants/colors.py
+-rw-r--r--   0        0        0      614 2024-05-30 01:22:23.726382 janim-1.2.0/janim/constants/coord.py
+-rw-r--r--   0        0        0      171 2024-05-30 01:22:23.726382 janim-1.2.0/janim/constants/degrees.py
+-rw-r--r--   0        0        0     5265 2024-05-30 01:22:23.726382 janim-1.2.0/janim/examples.py
+-rw-r--r--   0        0        0     1654 2024-05-30 01:22:23.726382 janim-1.2.0/janim/exception.py
+-rw-r--r--   0        0        0    21738 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/anim_viewer.py
+-rw-r--r--   0        0        0      319 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/application.py
+-rw-r--r--   0        0        0      766 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/audio_player.py
+-rw-r--r--   0        0        0     3181 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/export.png
+-rw-r--r--   0        0        0    16958 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/favicon.ico
+-rw-r--r--   0        0        0     1458 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/fixed_ratio_widget.py
+-rw-r--r--   0        0        0     3722 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/font_table.py
+-rw-r--r--   0        0        0     1508 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/glwidget.py
+-rw-r--r--   0        0        0     1011 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/precise_timer.py
+-rw-r--r--   0        0        0     5162 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/richtext_editor.py
+-rw-r--r--   0        0        0     1764 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/search.png
+-rw-r--r--   0        0        0     8115 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/selector.py
+-rw-r--r--   0        0        0    24412 2024-05-30 01:22:23.726382 janim-1.2.0/janim/gui/timeline_view.py
+-rw-r--r--   0        0        0     1699 2024-05-30 01:22:23.726382 janim-1.2.0/janim/imports.py
+-rw-r--r--   0        0        0     7886 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/audio.py
+-rw-r--r--   0        0        0     5190 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/boolean_ops.py
+-rw-r--r--   0        0        0     8569 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/coordinate/coordinate_systems.py
+-rw-r--r--   0        0        0     2093 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/coordinate/functions.py
+-rw-r--r--   0        0        0     8078 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/coordinate/number_line.py
+-rw-r--r--   0        0        0     8471 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/geometry/arc.py
+-rw-r--r--   0        0        0     6679 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/geometry/arrow.py
+-rw-r--r--   0        0        0     7653 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/geometry/line.py
+-rw-r--r--   0        0        0     5077 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/geometry/polygon.py
+-rw-r--r--   0        0        0     5071 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/image_item.py
+-rw-r--r--   0        0        0    18849 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/item.py
+-rw-r--r--   0        0        0     3149 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/points.py
+-rw-r--r--   0        0        0     7446 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/relation.py
+-rw-r--r--   0        0        0     2012 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/shape_matchers.py
+-rw-r--r--   0        0        0     5764 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/svg/brace.py
+-rw-r--r--   0        0        0     1719 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/svg/brace.svg
+-rw-r--r--   0        0        0     4298 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/svg/svg_item.py
+-rw-r--r--   0        0        0     2979 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/svg/typst.py
+-rw-r--r--   0        0        0       37 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/svg/typst_template.typ
+-rw-r--r--   0        0        0    15877 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/text/text.py
+-rw-r--r--   0        0        0     1053 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/value_tracker.py
+-rw-r--r--   0        0        0     5204 2024-05-30 01:22:23.730382 janim-1.2.0/janim/items/vitem.py
+-rw-r--r--   0        0        0      258 2024-05-30 01:22:23.730382 janim-1.2.0/janim/logger.py
+-rw-r--r--   0        0        0     3242 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/base.py
+-rw-r--r--   0        0        0     9282 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/impl.py
+-rw-r--r--   0        0        0      427 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/dotcloud.frag.glsl
+-rw-r--r--   0        0        0     1200 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/dotcloud.geom.glsl
+-rw-r--r--   0        0        0      502 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/dotcloud.vert.glsl
+-rw-r--r--   0        0        0      167 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/image.frag.glsl
+-rw-r--r--   0        0        0      533 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/image.vert.glsl
+-rw-r--r--   0        0        0     6752 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/vitem.frag.glsl
+-rw-r--r--   0        0        0      190 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/shaders/vitem.vert.glsl
+-rw-r--r--   0        0        0     1083 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/texture.py
+-rw-r--r--   0        0        0     6771 2024-05-30 01:22:23.730382 janim-1.2.0/janim/render/writer.py
+-rw-r--r--   0        0        0      931 2024-05-30 01:22:23.730382 janim-1.2.0/janim/typing.py
+-rw-r--r--   0        0        0    16826 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/bezier.py
+-rw-r--r--   0        0        0     5365 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/config.py
+-rw-r--r--   0        0        0     5590 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/data.py
+-rw-r--r--   0        0        0      618 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/dict_ops.py
+-rw-r--r--   0        0        0     2400 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/file_ops.py
+-rw-r--r--   0        0        0     4519 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/font.py
+-rw-r--r--   0        0        0     6192 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/font_manager.py
+-rw-r--r--   0        0        0     5767 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/iterables.py
+-rw-r--r--   0        0        0     1810 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/paths.py
+-rw-r--r--   0        0        0     2601 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/rate_functions.py
+-rw-r--r--   0        0        0     2566 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/refresh.py
+-rw-r--r--   0        0        0     8074 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/signal.py
+-rw-r--r--   0        0        0     1919 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/simple_functions.py
+-rw-r--r--   0        0        0     9707 2024-05-30 01:22:23.730382 janim-1.2.0/janim/utils/space_ops.py
+-rw-r--r--   0        0        0    18504 2024-05-30 01:22:23.730382 janim-1.2.0/logo.png
+-rw-r--r--   0        0        0     1018 2024-05-30 01:22:23.730382 janim-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2226 1970-01-01 00:00:00.000000 janim-1.2.0/PKG-INFO
```

### Comparing `janim-1.1.0/.readthedocs.yaml` & `janim-1.2.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/LICENSE` & `janim-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/README.md` & `janim-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/__main__.py` & `janim-1.2.0/janim/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
         action='store_true'
     )
 
     sp = parser.add_subparsers()
     run_parser(sp.add_parser('run', help='Run timeline(s) from specific namespace'))
     write_parser(sp.add_parser('write', help='Generate video file(s) of timeline(s) from specific namesapce'))
     examples_parser(sp.add_parser('examples', help='Show examples of janim'))
+    tool_parser(sp.add_parser('tool', help='Run useful tools'))
 
     args = parser.parse_args()
 
     if args.version:
         from janim import __version__
         print(f'JAnim {__version__}')
 
@@ -104,19 +105,34 @@
     )
     parser.set_defaults(all=None)
     parser.set_defaults(config=None)
     parser.set_defaults(func=run)
     parser.set_defaults(interact=False)
 
 
+def tool_parser(parser: ArgumentParser) -> None:
+    parser.add_argument(
+        'tool_name',
+        choices=['richtext', 'fonts'],
+        nargs='*',
+        help='Tool(s) that you want to use'
+    )
+    parser.set_defaults(func=tool)
+
+
 def run(args: Namespace) -> None:
     from janim.cli import run
     run(args)
 
 
 def write(args: Namespace) -> None:
     from janim.cli import write
     write(args)
 
 
+def tool(args: Namespace) -> None:
+    from janim.cli import tool
+    tool(args)
+
+
 if __name__ == '__main__':
     main()
```

### Comparing `janim-1.1.0/janim/anims/animation.py` & `janim-1.2.0/janim/anims/animation.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/composition.py` & `janim-1.2.0/janim/anims/composition.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/creation.py` & `janim-1.2.0/janim/anims/creation.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/display.py` & `janim-1.2.0/janim/anims/display.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/fading.py` & `janim-1.2.0/janim/anims/fading.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         super().__init__(
             item,
             self.updater,
             become_at_end=become_at_end,
             root_only=root_only,
             **kwargs
         )
-        self.shift = shift
+        self.shift = np.array(shift)
         self.scale = scale
 
         if about_point is None and scale != 1.0:
             cmpt = item(Points).points
             box = cmpt.self_box if root_only else cmpt.box
             about_point = box.get(about_edge)
         self.about_point = about_point
```

### Comparing `janim-1.1.0/janim/anims/growing.py` & `janim-1.2.0/janim/anims/growing.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/indication.py` & `janim-1.2.0/janim/anims/indication.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/movement.py` & `janim-1.2.0/janim/anims/movement.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/rotation.py` & `janim-1.2.0/janim/anims/rotation.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/timeline.py` & `janim-1.2.0/janim/anims/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,19 @@
         调用 :meth:`~.Timeline.subtitle` 的参数信息
         '''
         text: str
         range: TimeRange
         kwargs: dict
         subtitle: Text
 
+    @dataclass
+    class PausePoint:
+        at: float
+        at_previous_frame: bool
+
     class ItemHistory:
         def __init__(self):
             self.history: History[Item | DynamicItem] = History()
             self.history_without_dynamic: History[Item] = History()
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -164,14 +169,16 @@
 
         self.scheduled_tasks: list[Timeline.ScheduledTask] = []
         self.anims: list[AnimGroup] = []
         self.display_anims: list[Display] = []
         self.audio_infos: list[Timeline.PlayAudioInfo] = []
         self.subtitle_infos: list[Timeline.SubtitleInfo] = []   # helpful for extracting subtitles
 
+        self.pause_points: list[Timeline.PausePoint] = []
+
         self.items_history: defaultdict[Item, Timeline.ItemHistory] = defaultdict(Timeline.ItemHistory)
         self.item_display_times: dict[Item, int] = {}
 
     @abstractmethod
     def construct(self) -> None:
         '''
         继承该方法以实现动画的构建逻辑
@@ -273,14 +280,28 @@
     def play(self, *anims: Animation, **kwargs) -> None:
         '''
         应用动画并推进到动画结束的时候
         '''
         t_range = self.prepare(*anims, **kwargs)
         self.forward_to(t_range.end, _detect_changes=False)
 
+    def pause_point(
+        self,
+        *,
+        offset: float = 0,
+        at_previous_frame: bool = True
+    ) -> None:
+        '''
+        标记在预览界面中，执行到当前时间点时会暂停
+
+        - ``at_previous_frame`` 控制是在前一帧暂停（默认）还是在当前帧暂停
+        - ``offset`` 表示偏移多少秒，例如 ``offset=2`` 则是当前位置 2s 后
+        '''
+        self.pause_points.append(Timeline.PausePoint(self.current_time + offset, at_previous_frame))
+
     # endregion
 
     # region display
 
     def is_displaying(self, item: Item) -> None:
         '''
         判断特定的物件是否正在显示中
@@ -293,18 +314,17 @@
         self.item_display_times.setdefault(item, self.current_time)
 
     def show(self, *roots: Item, root_only=False) -> None:
         '''
         显示物件
         '''
         for root in roots:
-            self._show(root)
-            if not root_only:
-                for item in root.descendants():
-                    self._show(item)
+            for item in root.walk_self_and_descendants(root_only):
+                self._show(item)
+                self.track(item)
 
     def _hide(self, item: Item) -> Display:
         time = self.item_display_times.pop(item, None)
         if time is None:
             return
 
         duration = self.current_time - time
@@ -316,18 +336,16 @@
         return anim
 
     def hide(self, *roots: Item, root_only=False) -> None:
         '''
         隐藏物件
         '''
         for root in roots:
-            self._hide(root)
-            if not root_only:
-                for item in root.descendants():
-                    self._hide(item)
+            for item in root.walk_self_and_descendants(root_only):
+                self._hide(item)
 
     def cleanup_display(self) -> None:
         '''
         对目前显示中的所有物件调用隐藏，使得正确产生 :class:`~.Display` 对象
         '''
         for item in list(self.item_display_times.keys()):
             self._hide(item)
@@ -487,14 +505,15 @@
         duration: float = 1,
         delay: float = 0,
         scale: float | Iterable[float] = 1,
         base_scale: float = 0.8,
         use_typst_text: bool | Iterable[bool] = False,
         surrounding_color: JAnimColor = BLACK,
         surrounding_alpha: float = 0.5,
+        font: str | Iterable[str] = [],
         **kwargs
     ) -> TimeRange:
         '''
         添加字幕
 
         - 文字可以传入一个列表，纵向排列显示
         - 可以指定在当前位置往后 ``delay`` 秒才显示
@@ -509,33 +528,45 @@
         use_typst_lst = [use_typst_text] if not isinstance(use_typst_text, Iterable) else use_typst_text
 
         if isinstance(duration, TimeRange):
             range = duration
         else:
             range = TimeRange(self.current_time + delay, duration)
 
+        cfg_font = Config.get.subtitle_font
+        if cfg_font:
+            if isinstance(font, str):
+                font = [font]
+            else:
+                font = list(font)
+
+            if isinstance(cfg_font, str):
+                font.append(cfg_font)
+            else:
+                font.extend(cfg_font)
+
         for text, scale, use_typst_text in zip(reversed(text_lst),
                                                reversed(resize_preserving_order(scale_lst, len(text_lst))),
                                                reversed(resize_preserving_order(use_typst_lst, len(text_lst)))):
-            subtitle = (TypstText if use_typst_text else Text)(text, **kwargs)
+            if use_typst_text:
+                subtitle = TypstText(text, **kwargs)
+            else:
+                subtitle = Text(text, font=font, **kwargs)
             subtitle.depth.set(-1e5)
             subtitle.points.scale(scale * base_scale)
             self.place_subtitle(subtitle, range)
-            self.subtitle_infos.append(Timeline.SubtitleInfo(text,
-                                                             range,
-                                                             kwargs,
-                                                             subtitle))
+            self.subtitle_infos.append(Timeline.SubtitleInfo(text, range, kwargs, subtitle))
 
             subtitle_group = Group(
                 SurroundingRect(subtitle,
                                 color=surrounding_color,
                                 stroke_alpha=0,
                                 fill_alpha=surrounding_alpha),
                 subtitle
-            )
+            ).fix_in_frame()
             subtitle_group.depth.arrange(subtitle.depth.get())
 
             self.schedule(range.at, subtitle_group.show)
             self.schedule(range.end, subtitle_group.hide)
 
         return range.copy()
 
@@ -548,15 +579,15 @@
         '''
         for other in reversed(self.subtitle_infos):
             # 根据 TimelineView 中排列显示标签的经验
             # 这里加了一个 np.isclose 的判断
             # 如果不加可能导致前一个字幕消失但是后一个字幕凭空出现在更上面
             # （但是我没有测试过是否会出现这个bug，只是根据写 TimelineView 时的经验加了 np.isclose）
             if other.range.at <= range.at < other.range.end and not np.isclose(range.at, other.range.end):
-                subtitle.points.next_to(other.subtitle, UP, buff=SMALL_BUFF)
+                subtitle.points.next_to(other.subtitle, UP, buff=2 * SMALL_BUFF)
                 return
         subtitle.points.to_border(DOWN)
 
     # endregion
 
     # endregion
 
@@ -711,15 +742,15 @@
         with ContextSetter(self.ctx_var, self):
             SourceDisplayer(self.__class__).show()
         return super().build(quiet=quiet)
 
 
 class TimelineAnim(AnimGroup):
     '''
-    运行 :meth:`Timeline.run` 后返回的动画组
+    运行 :meth:`Timeline.build` 后返回的动画组
 
     - ``self.display_anim`` 是由 :meth:`Timeline.construct` 中执行
       :meth:`Timeline.show` 和 :meth:`Timeline.hide` 而产生的
     - ``self.user_anim`` 是显式使用了 :meth:`Timeline.prepare` 或 :meth:`Timeline.play` 而产生的
     '''
     def __init__(self, timeline: Timeline, **kwargs):
         self.timeline = timeline
@@ -761,14 +792,15 @@
                 timeline = self.timeline
                 camera_info = timeline.camera.current().points.info
                 anti_alias_radius = self.cfg.anti_alias_width / 2 * camera_info.scaled_factor
 
                 set_global_uniforms(
                     ctx,
                     ('JA_VIEW_MATRIX', camera_info.view_matrix.T.flatten()),
+                    ('JA_DISTANCE_FROM_PLANE', camera_info.distance_from_plane),
                     ('JA_PROJ_MATRIX', camera_info.proj_matrix.T.flatten()),
                     ('JA_FRAME_RADIUS', camera_info.frame_radius),
                     ('JA_ANTI_ALIAS_RADIUS', anti_alias_radius)
                 )
 
                 with ContextSetter(Renderer.data_ctx, RenderData(ctx=ctx,
                                                                  camera_info=camera_info,
```

### Comparing `janim-1.1.0/janim/anims/transform.py` & `janim-1.2.0/janim/anims/transform.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/anims/updater.py` & `janim-1.2.0/janim/anims/updater.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     label_color = C_LABEL_ANIM_ABSTRACT
 
     @dataclass
     class DataGroup:
         orig_data: Item
         data: Item
         extra_data: Any | None
+        alpha_on: float | None = None
 
     def __init__(
         self,
         item: T,
         func: DataUpdaterFn[T],
         *,
         lag_ratio: float = 0,
@@ -171,14 +172,20 @@
         if self.show_at_end:
             self.timeline.schedule(self.global_range.end, self.item.show, root_only=self.root_only)
 
     def anim_on_alpha(self, alpha: float) -> None:
         global_t = self.global_t_ctx.get()
         for i, updater_data in enumerate(self.datas.values()):
             sub_alpha = self.get_sub_alpha(alpha, i)
+
+            # 如果此时将要插值的 sub_alpha 与上次的相同，则跳过
+            if sub_alpha == updater_data.alpha_on:
+                continue
+
+            updater_data.alpha_on = sub_alpha
             updater_data.data.restore(updater_data.orig_data)
 
             with UpdaterParams(self,
                                global_t,
                                sub_alpha,
                                self.global_range,
                                updater_data.extra_data) as params:
```

### Comparing `janim-1.1.0/janim/camera/camera.py` & `janim-1.2.0/janim/camera/camera.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/camera/camera_info.py` & `janim-1.2.0/janim/camera/camera_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,20 +45,24 @@
         aligned = np.hstack([
             points,
             np.full((len(points), 1), 1)
         ])
         mapped = np.dot(aligned, self.proj_view_matrix.T)
         return mapped[:, :2] / mapped[:, 3].reshape((len(mapped), 1))
 
+    @property
+    def distance_from_plane(self) -> float:
+        up = self.vertical_vect
+        return get_norm(up) / 2 / math.tan(math.radians(self.fov / 2))
+
     def _compute_camera_location(self) -> np.ndarray:
         right = self.horizontal_vect
         up = self.vertical_vect
         normal = get_unit_normal(right, up)
-        distance = get_norm(up) / 2 / math.tan(math.radians(self.fov / 2))
-        return self.center + normal * distance
+        return self.center + normal * self.distance_from_plane
 
     def _compute_view_matrix(self) -> np.ndarray:
         rot_matrix = np.eye(4)
         rot_matrix[0, :3] = normalize(self.horizontal_vect)
         rot_matrix[1, :3] = normalize(self.vertical_vect)
         rot_matrix[2, :3] = normalize(self.camera_location - self.center)
```

### Comparing `janim-1.1.0/janim/cli.py` & `janim-1.2.0/janim/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -115,14 +115,45 @@
                 os.path.join(output_dir,
                              f'{name}.{args.audio_format}')
             )
 
     log.info('======')
 
 
+def tool(args: Namespace) -> None:
+    # 不直接从对应的 module 导入，是为了经过 anim_viewer 中对 pyside6 安装的检查
+    from janim.gui.anim_viewer import FontTable, QWidget, RichTextEditor
+
+    log.info('======')
+    log.info('Constructing window')
+
+    t = time.time()
+
+    from janim.gui.application import Application
+
+    app = Application()
+
+    tool_map: dict[str, type[QWidget]] = {
+        'richtext': RichTextEditor,
+        'fonts': FontTable
+    }
+
+    widgets: list[QWidget] = []
+
+    for key in args.tool_name:
+        widget = tool_map[key]()
+        widgets.append(widget)
+        widget.show()
+
+    log.info(f'Finished constructing in {time.time() - t:.2f} s')
+    log.info('======')
+
+    app.exec()
+
+
 def modify_default_config(args: Namespace) -> None:
     if args.config:
         for key, value in args.config:
             dtype = type(getattr(default_config, key))
             setattr(default_config, key, dtype(value))
```

### Comparing `janim-1.1.0/janim/components/component.py` & `janim-1.2.0/janim/components/component.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/data.py` & `janim-1.2.0/janim/components/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/depth.py` & `janim-1.2.0/janim/components/depth.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/image.py` & `janim-1.2.0/janim/components/image.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/points.py` & `janim-1.2.0/janim/components/points.py`

 * *Files 2% similar despite different names*

```diff
@@ -910,14 +910,39 @@
                 x, y = index // n_rows, index % n_rows
             cmpt.move_to(ORIGIN, aligned_edge=aligned_edge)
             cmpt.shift(x * x_unit * RIGHT + y * y_unit * DOWN)
 
         self.to_center()
         return self
 
+    def arrange_by_offset(
+        self,
+        offset: Vect,
+        *,
+        aligned_edge: Vect = ORIGIN,
+        center: bool = True
+    ) -> Self:
+        if self.bind is None or not self.bind.at_item.children:
+            return self
+
+        cmpts = [
+            self.get_same_cmpt(item)
+            for item in self.bind.at_item.children
+        ]
+        offset = np.array(offset)
+
+        for cmpt1, cmpt2 in zip(cmpts, cmpts[1:]):
+            delta = cmpt2.box.get(aligned_edge) - cmpt1.box.get(aligned_edge)
+            cmpt2.shift(offset - delta)
+
+        if center:
+            self.to_center()
+
+        return self
+
     def to_center(self, root_only=False) -> Self:
         '''
         移动到原点 ``(0, 0, 0)``
         '''
         self.shift(-self.box.center, root_only=root_only)
         return self
```

### Comparing `janim-1.1.0/janim/components/radius.py` & `janim-1.2.0/janim/components/radius.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/rgbas.py` & `janim-1.2.0/janim/components/rgbas.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/components/vpoints.py` & `janim-1.2.0/janim/components/vpoints.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/constants/colors.py` & `janim-1.2.0/janim/constants/colors.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/constants/coord.py` & `janim-1.2.0/janim/constants/coord.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/examples.py` & `janim-1.2.0/janim/examples.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/exception.py` & `janim-1.2.0/janim/exception.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/gui/audio_player.py` & `janim-1.2.0/janim/gui/audio_player.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/gui/export.png` & `janim-1.2.0/janim/gui/export.png`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/gui/favicon.ico` & `janim-1.2.0/janim/gui/favicon.ico`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/gui/fixed_ratio_widget.py` & `janim-1.2.0/janim/gui/fixed_ratio_widget.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from PySide6.QtWidgets import QWidget
 
 
 class FixedRatioWidget(QWidget):
     '''
     使得传入的 ``inside`` 控件可以以固定比例塞在该控件中
     '''
-    def __init__(self, inside: QWidget, src_size: tuple[float, float], parent: QWidget | None = None) -> None:
+    def __init__(self, inside: QWidget, parent: QWidget | None = None) -> None:
         super().__init__(parent)
         self.inside = inside
         self.inside.setParent(self)
-        self.src_size = src_size
+        self.src_size = (1, 1)
 
     def set_src_size(self, size: tuple[float, float]) -> None:
         self.src_size = size
         self.update_inner_size(self.size())
 
     def update_inner_size(self, wnd_size: QSize) -> None:
         wnd_width, wnd_height = wnd_size.toTuple()
```

### Comparing `janim-1.1.0/janim/gui/glwidget.py` & `janim-1.2.0/janim/gui/glwidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 
 class GLWidget(QOpenGLWidget):
     '''
     窗口中央的渲染界面
     '''
     rendered = Signal()
 
-    def __init__(self, anim: TimelineAnim, parent: QWidget | None = None) -> None:
+    def __init__(self, parent: QWidget | None = None) -> None:
         super().__init__(parent)
-        self.anim = anim
         self.needs_update_clear_color = False
 
+    def set_anim(self, anim: TimelineAnim) -> None:
+        self.anim = anim
+        self.update_clear_color()
+        self.update()
+
     def set_time(self, time: float) -> None:
         self.anim.anim_on(time)
         self.update()
 
     def initializeGL(self) -> None:
         self.ctx = mgl.create_context()
         self.ctx.enable(mgl.BLEND)
```

### Comparing `janim-1.1.0/janim/gui/precise_timer.py` & `janim-1.2.0/janim/gui/precise_timer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 
 import time
 
 from PySide6.QtCore import QTimer, QObject, Qt
 
 
 class PreciseTimer(QTimer):
-    def __init__(self, duration: float, parent: QObject | None = None):
+    def __init__(self, duration: float | None = None, parent: QObject | None = None):
         super().__init__(parent)
 
         self.duration = duration
 
         self.setTimerType(Qt.TimerType.PreciseTimer)
         self.timeout.connect(self.on_timeout)
 
+    def set_duration(self, duration: float) -> None:
+        self.duration = duration
+
     def start_precise_timer(self) -> None:
+        assert self.duration is not None
         self.scheduled = 0
         self.start_time = time.time()
         self.start(int(self.duration * 1000))
 
     def on_timeout(self) -> None:
         if not self.isActive():
             return
```

### Comparing `janim-1.1.0/janim/gui/richtext_editor.py` & `janim-1.2.0/janim/gui/richtext_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 class RichTextEditor(QWidget):
     def __init__(self, parent: QWidget | None = None) -> None:
         super().__init__(parent)
 
         self.setup_ui()
+        self.setWindowTitle('富文本编辑')
         self.resize(600, 400)
         self.check_box_wordwrap.setChecked(True)
 
     def setup_ui(self):
         self.check_box_wordwrap = QCheckBox('自动换行')
         self.check_box_wordwrap.stateChanged.connect(
             lambda state: self.editor.setLineWrapMode(RichTextEdit.LineWrapMode.WidgetWidth
```

### Comparing `janim-1.1.0/janim/gui/selector.py` & `janim-1.2.0/janim/gui/selector.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/imports.py` & `janim-1.2.0/janim/imports.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/audio.py` & `janim-1.2.0/janim/items/audio.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/boolean_ops.py` & `janim-1.2.0/janim/items/boolean_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/coordinate/coordinate_systems.py` & `janim-1.2.0/janim/items/coordinate/coordinate_systems.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/coordinate/functions.py` & `janim-1.2.0/janim/items/coordinate/functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/coordinate/number_line.py` & `janim-1.2.0/janim/items/coordinate/number_line.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/geometry/arc.py` & `janim-1.2.0/janim/items/geometry/arc.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/geometry/arrow.py` & `janim-1.2.0/janim/items/geometry/arrow.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/geometry/line.py` & `janim-1.2.0/janim/items/geometry/line.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/geometry/polygon.py` & `janim-1.2.0/janim/items/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/image_item.py` & `janim-1.2.0/janim/items/image_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/item.py` & `janim-1.2.0/janim/items/item.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         self.timeline = Timeline.get_context(raise_exc=False)
 
         self._init_components()
 
         self._astype: type[Item] | None = None
         self._astype_mock_cmpt: dict[str, Component] = {}
 
+        self._fix_in_frame = False
         self.renderer: Renderer | None = None
 
         if children is not None:
             self.add(*children)
         self.digest_styles(**kwargs)
 
     @dataclass
@@ -539,14 +540,22 @@
             cmpt.interpolate(cmpt1, cmpt2, alpha, path_func=path_func)
 
     def apart_alpha(self, n: int) -> None:
         for cmpt in self.components.values():
             if isinstance(cmpt, SupportsApartAlpha):
                 cmpt.apart_alpha(n)
 
+    def fix_in_frame(self, on: bool = True, *, root_only: bool = False) -> Self:
+        '''
+        固定在屏幕上，也就是即使摄像头移动位置也不会改变在屏幕上的位置
+        '''
+        for item in self.walk_self_and_descendants(root_only):
+            item._fix_in_frame = on
+        return self
+
     @classmethod
     def get_global_renderer(cls) -> None:
         if cls.global_renderer is None:
             cls.global_renderer = cls.renderer_cls()
         return cls.global_renderer
 
     def create_renderer(self) -> None:
```

### Comparing `janim-1.1.0/janim/items/points.py` & `janim-1.2.0/janim/items/points.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
     radius = CmptInfo(Cmpt_Radius[Self], 0.05)
 
     renderer_cls = DotCloudRenderer
 
     def __init__(
         self,
         *args,
-
         **kwargs
     ):
         super().__init__(*args, **kwargs)
 
         Cmpt_Points.reverse.connect(self.points, lambda: self.radius.reverse())
 
         self.points.resize_func = resize_preserving_order
```

### Comparing `janim-1.1.0/janim/items/relation.py` & `janim-1.2.0/janim/items/relation.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/shape_matchers.py` & `janim-1.2.0/janim/items/shape_matchers.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/svg/brace.py` & `janim-1.2.0/janim/items/svg/brace.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/svg/brace.svg` & `janim-1.2.0/janim/items/svg/brace.svg`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/svg/svg_item.py` & `janim-1.2.0/janim/items/svg/svg_item.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/svg/typst.py` & `janim-1.2.0/janim/items/svg/typst.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/text/text.py` & `janim-1.2.0/janim/items/text/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from janim.exception import ColorNotFoundError
 from janim.items.geometry.line import Line
 from janim.items.points import Group, Points
 from janim.items.vitem import VItem
 from janim.logger import log
 from janim.typing import JAnimColor
 from janim.utils.config import Config
-from janim.utils.font import Font, get_fontpath_by_name
+from janim.utils.font import Font, get_font_info_by_name
 from janim.utils.simple_functions import decode_utf8
 from janim.utils.space_ops import get_norm, normalize
 
 DEFAULT_FONT_SIZE = 24
 ORIG_FONT_SIZE = 48
 
 
@@ -279,25 +279,27 @@
         line_kwargs: dict = {},
         stroke_alpha: float = 0,
         fill_alpha: float = 1,
         **kwargs
     ) -> None:
         # 获取字体
         if isinstance(font, str):
-            font = [font]
+            font_names = [font]
+        else:
+            font_names = list(font)
 
         cfg_font = Config.get.font
         if isinstance(cfg_font, str):
-            font.append(cfg_font)
+            font_names.append(cfg_font)
         else:
-            font.extend(cfg_font)
+            font_names.extend(cfg_font)
 
         fonts = [
-            Font.get(get_fontpath_by_name(name))
-            for name in font
+            Font.get_by_info(get_font_info_by_name(name))
+            for name in font_names
         ]
 
         if format is not Text.Format.RichText:
             self.text = text
         else:
             # 如果是 RichText，获取属性列表
             self.text = ''
```

### Comparing `janim-1.1.0/janim/items/value_tracker.py` & `janim-1.2.0/janim/items/value_tracker.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/items/vitem.py` & `janim-1.2.0/janim/items/vitem.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/render/base.py` & `janim-1.2.0/janim/render/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 from __future__ import annotations
 
 import os
 from contextvars import ContextVar
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 import moderngl as mgl
 
 from janim.camera.camera_info import CameraInfo
 from janim.utils.file_ops import get_janim_dir, readall
 
+if TYPE_CHECKING:
+    from janim.items.item import Item
+
+FIX_IN_FRAME_KEY = 'JA_FIX_IN_FRAME'
+
 
 class Renderer:
     '''渲染器的基类
 
     重写 :meth:`init` 和 :meth:`render` 以实现具体功能
     '''
     data_ctx: ContextVar[RenderData] = ContextVar('Renderer.data_ctx')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.initialized = False
 
     def init(self) -> None: ...
 
-    def render(self, data) -> None: ...
+    def render(self, item) -> None: ...
+
+    @staticmethod
+    def update_fix_in_frame(item: Item, prog: mgl.Program):
+        if FIX_IN_FRAME_KEY in prog._members:
+            prog[FIX_IN_FRAME_KEY] = item._fix_in_frame
 
 
 @dataclass(kw_only=True)
 class RenderData:
     '''在渲染过程中需要配置的属性
 
     通过 :py:obj:`Renderer.data_ctx` 进行设置和获取
```

### Comparing `janim-1.1.0/janim/render/impl.py` & `janim-1.2.0/janim/render/impl.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
             if len(bytes) != self.vbo_points.size:
                 self.vbo_points.orphan(len(bytes))
 
             self.vbo_points.write(bytes)
             self.prev_points = new_points
 
+        self.update_fix_in_frame(item, self.prog)
         self.vao.render(mgl.POINTS, vertices=len(self.prev_points))
 
 
 class VItemRenderer(Renderer):
     def init(self) -> None:
         self.prog = get_program('render/shaders/vitem')
 
@@ -81,36 +82,44 @@
         self.vbo_stroke_color = self.ctx.buffer(reserve=1)
         self.vbo_fill_color = self.ctx.buffer(reserve=1)
 
         self.vao = self.ctx.vertex_array(self.prog, self.vbo_coord, 'in_coord')
 
         self.prev_camera_info = None
 
+        self.prev_fix_in_frame = None
         self.prev_points = np.array([])
         self.prev_radius = np.array([])
         self.prev_stroke = np.array([])
         self.prev_fill = np.array([])
 
     def render(self, item: 'VItem') -> None:
         if item.points.curves_count() == 0:
             return
         render_data = self.data_ctx.get()
 
         new_camera_info = render_data.camera_info
 
+        new_fix_in_frame = item._fix_in_frame
         new_points = item.points._points.data
         new_radius = item.radius._radii.data
         new_stroke = item.stroke._rgbas.data
         new_fill = item.fill._rgbas.data
 
         is_camera_changed = id(new_camera_info) != id(self.prev_camera_info)
 
-        if id(new_radius) != id(self.prev_radius) or id(new_points) != id(self.prev_points) or is_camera_changed:
-            clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
-            clip_box *= render_data.camera_info.frame_radius
+        if new_fix_in_frame != self.prev_fix_in_frame \
+                or id(new_radius) != id(self.prev_radius) \
+                or id(new_points) != id(self.prev_points) \
+                or is_camera_changed:
+            if new_fix_in_frame:
+                clip_box = np.array(item.points.self_box.get_corners())[:, :2]
+            else:
+                clip_box = render_data.camera_info.map_points(item.points.self_box.get_corners())
+                clip_box *= render_data.camera_info.frame_radius
 
             buff = new_radius.max() + render_data.anti_alias_radius
             clip_min = np.min(clip_box, axis=0) - buff
             clip_max = np.max(clip_box, axis=0) + buff
             clip_box = np.array([
                 clip_min,
                 [clip_min[0], clip_max[1]],
@@ -149,28 +158,34 @@
 
             if len(bytes) != self.vbo_fill_color.size:
                 self.vbo_fill_color.orphan(len(bytes))
 
             self.vbo_fill_color.write(bytes)
             self.prev_fill = new_fill
 
-        if id(new_points) != id(self.prev_points) or is_camera_changed:
-            mapped = render_data.camera_info.map_points(new_points)
-            mapped *= render_data.camera_info.frame_radius
+        if id(new_points) != id(self.prev_points) \
+                or new_fix_in_frame != self.prev_fix_in_frame \
+                or is_camera_changed:
+            if new_fix_in_frame:
+                mapped = new_points[:, :2]
+            else:
+                mapped = render_data.camera_info.map_points(new_points)
+                mapped *= render_data.camera_info.frame_radius
 
             bytes = np.hstack([
                 mapped,
                 item.points.get_closepath_flags()[:, np.newaxis],
                 np.zeros((len(mapped), 1))
             ]).astype('f4').tobytes()
 
             if len(bytes) != self.vbo_mapped_points.size:
                 self.vbo_mapped_points.orphan(len(bytes))
 
             self.vbo_mapped_points.write(bytes)
+            self.prev_fix_in_frame = new_fix_in_frame
             self.prev_camera_info = new_camera_info
             self.prev_points = new_points
 
         self.vbo_mapped_points.bind_to_storage_buffer(0)
         self.vbo_radius.bind_to_storage_buffer(1)
         self.vbo_stroke_color.bind_to_storage_buffer(2)
         self.vbo_fill_color.bind_to_storage_buffer(3)
@@ -228,8 +243,9 @@
             self.texture = get_texture_from_img(item.image.get())
             self.texture.build_mipmaps()
             self.prev_img = item.image.img
 
         self.prog['image'] = 0
         self.texture.filter = item.image.get_filter()
         self.texture.use(0)
+        self.update_fix_in_frame(item, self.prog)
         self.vao.render(mgl.TRIANGLE_STRIP)
```

### Comparing `janim-1.1.0/janim/render/shaders/dotcloud.geom.glsl` & `janim-1.2.0/janim/render/shaders/dotcloud.geom.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/render/shaders/vitem.frag.glsl` & `janim-1.2.0/janim/render/shaders/vitem.frag.glsl`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/render/texture.py` & `janim-1.2.0/janim/render/texture.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import moderngl as mgl
 from PIL import Image
 
 from janim.render.base import Renderer
 from janim.utils.file_ops import find_file
 
-filepath_to_img_map: dict[str, Image.Image] = {}
+filepath_to_img_map: dict[tuple[str, float], Image.Image] = {}
 
 
 def get_img_from_file(file_path: str) -> Image.Image:
     file_path = find_file(file_path)
     mtime = os.path.getmtime(file_path)
     key = (file_path, mtime)
```

### Comparing `janim-1.1.0/janim/render/writer.py` & `janim-1.2.0/janim/render/writer.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/typing.py` & `janim-1.2.0/janim/typing.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/bezier.py` & `janim-1.2.0/janim/utils/bezier.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/config.py` & `janim-1.2.0/janim/utils/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     frame_height: float = None
     frame_width: float = None
 
     pixel_height: int = None
     pixel_width: int = None
     background_color: Color = None
     font: str | Iterable[str] = None
+    subtitle_font: str | Iterable[str] = None
 
     audio_framerate: int = None
 
     wnd_pos: str = None
     wnd_monitor: int = None
 
     typst_bin: str = None
@@ -124,14 +125,15 @@
     frame_height=8.0,
     frame_width=16.0 / 9.0 * 8.0,   # aspect_ratio(16/9) * frame_height
 
     pixel_height=1080,
     pixel_width=1920,
     background_color=Color('#000000'),
     font='Consolas',
+    subtitle_font='',
 
     audio_framerate=44100,
 
     wnd_pos='OR',
     wnd_monitor=0,
 
     typst_bin='typst',
```

### Comparing `janim-1.1.0/janim/utils/data.py` & `janim-1.2.0/janim/utils/data.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/dict_ops.py` & `janim-1.2.0/janim/utils/dict_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/file_ops.py` & `janim-1.2.0/janim/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/font.py` & `janim-1.2.0/janim/utils/font.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,123 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import Callable
-from functools import lru_cache
+from typing import TYPE_CHECKING, Callable, Generator
 
 import freetype as FT
 import numpy as np
 from fontTools.ttLib import TTCollection, TTFont, TTLibError
 
 from janim.exception import FontNotFoundError
 from janim.utils.bezier import PathBuilder
+from janim.logger import log
 
-fontpaths: list[str] = None
+if TYPE_CHECKING:
+    from fontTools.ttLib.tables._n_a_m_e import table__n_a_m_e
 
 
-@lru_cache()
-def get_fontpath_by_name(font_name: str) -> str:
-    '''
-    通过字体名得到字体文件路径
+@dataclass
+class FontInfo:
+    filepath: str
+    index: int
+    name: str
+    table: table__n_a_m_e
 
-    例：通过 ``Consolas`` 得到 ``C:\\Windows\\Fonts\\consola.ttf``
-    '''
-    global fontpaths
 
-    if fontpaths is None:
-        from janim.utils.font_manager import findSystemFonts
-        fontpaths = findSystemFonts()
+_font_finder: Generator[FontInfo, None, None] | None = None
+_found_infos: dict[str, FontInfo] = {}
+
 
-    for filepath in fontpaths:
+def _font_finder_func() -> Generator[FontInfo, None, None]:
+    from janim.utils.font_manager import findSystemFonts
+    for filepath in findSystemFonts():
         try:
             fonts = TTCollection(filepath).fonts    \
-                if filepath[-3:].endswith('ttc')    \
+                if filepath.endswith('ttc')         \
                 else [TTFont(filepath)]
         except TTLibError:
+            log.debug(f'Skipped font "{filepath}"')
             continue
 
-        for font in fonts:
-            if font['name'].getDebugName(4) == font_name:
-                return filepath
+        for i, font in enumerate(fonts):
+            table: table__n_a_m_e = font['name']
+            name = table.getDebugName(4) or ''
+            info = FontInfo(filepath, i, name, table)
+            _found_infos[name] = info
+            yield info
+
+
+def _get_font_finder() -> Generator[FontInfo, None, None]:
+    global _font_finder
+    if _font_finder is None:
+        _font_finder = _font_finder_func()
+    return _font_finder
+
+
+def get_font_info_by_name(font_name: str) -> FontInfo:
+    '''
+    通过字体名得到字体文件信息
+
+    例：通过 ``Consolas`` 得到 ``FontInfo('C:\\Windows\\Fonts\\consola.ttf', 0, 'Consolas', <'name' table at ...>)``
+    '''
+    info = _found_infos.get(font_name, None)
+    if info is not None:
+        return info
+
+    finder = _get_font_finder()
+
+    try:
+        while True:
+            info = next(finder)
+            if info.name == font_name:
+                return info
+    except StopIteration:
+        raise FontNotFoundError(f'No font named "{font_name}"')
+
+
+def get_found_infos() -> dict[str, FontInfo]:
+    finder = _get_font_finder()
+    try:
+        while True:
+            next(finder)
+    except StopIteration:
+        pass
 
-    raise FontNotFoundError(f'No font named "{font_name}"')
+    return _found_infos
 
 
 class Font:
-    filepath_to_font_map: dict[str, Font] = {}
+    filepath_to_font_map: dict[tuple[str, int], Font] = {}
 
     @staticmethod
-    def get(filepath: str) -> FT.Face:
-        if filepath in Font.filepath_to_font_map:
-            return Font.filepath_to_font_map[filepath]
+    def get(filepath: str) -> Font:
+        key = (filepath, 0)
+        cache = Font.filepath_to_font_map.get(key)
+        if cache is not None:
+            return cache
 
         font = Font(filepath)
-        Font.filepath_to_font_map[filepath] = font
+        Font.filepath_to_font_map[key] = font
+        return font
+
+    @staticmethod
+    def get_by_info(info: FontInfo) -> Font:
+        key = (info.filepath, info.index)
+        cache = Font.filepath_to_font_map.get(key)
+        if cache is not None:
+            return cache
+
+        font = Font(info.filepath, info.index)
+        Font.filepath_to_font_map[key] = font
         return font
 
-    def __init__(self, filepath: str) -> None:
-        self.face = FT.Face(filepath)
+    def __init__(self, filepath: str | FontInfo, index: int = 0) -> None:
+        self.filepath = filepath
+        with open(filepath, 'rb') as file:
+            self.face = FT.Face(file, index=index)
         self.face.select_charmap(FT.FT_ENCODING_UNICODE)
         self.face.set_char_size(48 << 6)
         self.cached_glyph: dict[int, Font.GlyphData] = {}
 
     @dataclass
     class GlyphData:
         array: np.ndarray
```

### Comparing `janim-1.1.0/janim/utils/font_manager.py` & `janim-1.2.0/janim/utils/font_manager.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/iterables.py` & `janim-1.2.0/janim/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/paths.py` & `janim-1.2.0/janim/utils/paths.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/rate_functions.py` & `janim-1.2.0/janim/utils/rate_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/refresh.py` & `janim-1.2.0/janim/utils/refresh.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/signal.py` & `janim-1.2.0/janim/utils/signal.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/simple_functions.py` & `janim-1.2.0/janim/utils/simple_functions.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/janim/utils/space_ops.py` & `janim-1.2.0/janim/utils/space_ops.py`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/logo.png` & `janim-1.2.0/logo.png`

 * *Files identical despite different names*

### Comparing `janim-1.1.0/pyproject.toml` & `janim-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,18 @@
     "sphinx-copybutton",
     "furo",
     "jinja2",
     "docutils",
 ]
 
 [tool.flit.sdist]
-exclude = [".vscode/", "assets/", "doc/", "test/"]
+exclude = [
+    ".vscode/", ".github/", "assets/", "doc/", "test/",
+    ".pypirc"
+]
 
 [project.urls]
 Home = "https://github.com/jkjkil4/JAnim"
 Source = "https://github.com/jkjkil4/JAnim"
 Documentation = "https://janim.rtfd.io"
 
 [project.scripts]
```

### Comparing `janim-1.1.0/PKG-INFO` & `janim-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janim
-Version: 1.1.0
+Version: 1.2.0
 Summary: a library for simple animation effects
 Author: jkjkil4
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Requires-Dist: numpy
 Requires-Dist: scipy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: janim Version: 1.1.0 Summary: a library for simple
+Metadata-Version: 2.1 Name: janim Version: 1.2.0 Summary: a library for simple
 animation effects Author: jkjkil4 Requires-Python: >=3.12 Description-Content-
 Type: text/markdown Classifier: Programming Language :: Python Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: colour Requires-Dist: rich Requires-
 Dist: moderngl Requires-Dist: tqdm Requires-Dist: psutil Requires-Dist: skia-
 pathops Requires-Dist: fontTools Requires-Dist: freetype-py Requires-Dist:
 pillow Requires-Dist: svgelements Requires-Dist: sphinx ; extra == "doc"
 Requires-Dist: sphinx-copybutton ; extra == "doc" Requires-Dist: furo ; extra
```

