# Comparing `tmp/pygerber-2.3.1.tar.gz` & `tmp/pygerber-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygerber-2.3.1.tar", max compression
+gzip compressed data, was "pygerber-2.3.2.tar", max compression
```

## Comparing `pygerber-2.3.1.tar` & `pygerber-2.3.2.tar`

### file list

```diff
@@ -1,232 +1,232 @@
--rw-r--r--   0        0        0     1069 2024-04-18 23:23:58.575230 pygerber-2.3.1/LICENSE.md
--rw-r--r--   0        0        0    12132 2024-04-18 23:23:58.575230 pygerber-2.3.1/README.md
--rw-r--r--   0        0        0    12976 2024-04-18 23:23:58.707229 pygerber-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      103 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/__init__.py
--rw-r--r--   0        0        0      149 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/__main__.py
--rw-r--r--   0        0        0      858 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/__init__.py
--rw-r--r--   0        0        0       61 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/__init__.py
--rw-r--r--   0        0        0     4205 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/aperture_handle.py
--rw-r--r--   0        0        0     6118 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/backend_cls.py
--rw-r--r--   0        0        0       50 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/__init__.py
--rw-r--r--   0        0        0     3958 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1165 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1214 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     1007 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_command.py
--rw-r--r--   0        0        0     1226 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     1527 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1323 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1395 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1707 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      793 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands_handle.py
--rw-r--r--   0        0        0     1101 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/drawing_target.py
--rw-r--r--   0        0        0      280 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/errors.py
--rw-r--r--   0        0        0      663 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/abstract/result_handle.py
--rw-r--r--   0        0        0       65 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/__init__.py
--rw-r--r--   0        0        0     2435 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/aperture_handle.py
--rw-r--r--   0        0        0     8530 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/backend_cls.py
--rw-r--r--   0        0        0     8452 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/color_scheme.py
--rw-r--r--   0        0        0       81 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
--rw-r--r--   0        0        0     1371 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
--rw-r--r--   0        0        0     1583 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
--rw-r--r--   0        0        0     1702 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
--rw-r--r--   0        0        0     2072 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
--rw-r--r--   0        0        0     2139 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
--rw-r--r--   0        0        0     1634 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
--rw-r--r--   0        0        0     1616 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
--rw-r--r--   0        0        0     1389 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
--rw-r--r--   0        0        0      317 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
--rw-r--r--   0        0        0     4122 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/drawing_target.py
--rw-r--r--   0        0        0      520 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/errors.py
--rw-r--r--   0        0        0      801 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/image_tools.py
--rw-r--r--   0        0        0     1589 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/backend/rasterized_2d/result_handle.py
--rw-r--r--   0        0        0       53 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/__init__.py
--rw-r--r--   0        0        0      202 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/error.py
--rw-r--r--   0        0        0      369 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/frozen_general_model.py
--rw-r--r--   0        0        0      364 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/general_model.py
--rw-r--r--   0        0        0     2179 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/immutable_map_model.py
--rw-r--r--   0        0        0     2860 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/position.py
--rw-r--r--   0        0        0     4913 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/common/rgba.py
--rw-r--r--   0        0        0       37 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/__init__.py
--rw-r--r--   0        0        0     3410 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/commands.py
--rw-r--r--   0        0        0     2950 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/console/raster_2d_style.py
--rw-r--r--   0        0        0      925 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/__init__.py
--rw-r--r--   0        0        0     1176 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/shape_flashes.grb
--rw-r--r--   0        0        0    49675 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Cu.gbr
--rw-r--r--   0        0        0     3742 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Mask.gbr
--rw-r--r--   0        0        0     2486 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Paste.gbr
--rw-r--r--   0        0        0     9518 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr
--rw-r--r--   0        0        0    10101 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/examples/ucamco_ex_2_shapes.grb
--rw-r--r--   0        0        0       50 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/__init__.py
--rw-r--r--   0        0        0     1130 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_errors.py
--rw-r--r--   0        0        0    12011 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_layers.py
--rw-r--r--   0        0        0    13437 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/_v2.py
--rw-r--r--   0        0        0      981 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/api/v2.py
--rw-r--r--   0        0        0      248 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/__init__.py
--rw-r--r--   0        0        0     1248 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/__main__.py
--rw-r--r--   0        0        0      489 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/__init__.py
--rw-r--r--   0        0        0     4711 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/document.py
--rw-r--r--   0        0        0      167 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/error.py
--rw-r--r--   0        0        0      273 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/errors.py
--rw-r--r--   0        0        0     3891 2024-04-18 23:23:58.707229 pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/server.py
--rw-r--r--   0        0        0       29 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/linter/__init__.py
--rw-r--r--   0        0        0     6540 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/linter/diagnostic.py
--rw-r--r--   0        0        0       40 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/__init__.py
--rw-r--r--   0        0        0     6193 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/bounding_box.py
--rw-r--r--   0        0        0     5071 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/offset.py
--rw-r--r--   0        0        0      711 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/rotate_point.py
--rw-r--r--   0        0        0     8028 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/math/vector_2d.py
--rw-r--r--   0        0        0       29 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/optimizer/__init__.py
--rw-r--r--   0        0        0       38 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
--rw-r--r--   0        0        0       23 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/errors.py
--rw-r--r--   0        0        0     5942 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/parser.py
--rw-r--r--   0        0        0     6100 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser/state.py
--rw-r--r--   0        0        0       36 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/__init__.py
--rw-r--r--   0        0        0       82 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/__init__.py
--rw-r--r--   0        0        0     1844 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
--rw-r--r--   0        0        0     2122 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/block2.py
--rw-r--r--   0        0        0     1942 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py
--rw-r--r--   0        0        0     2056 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/macro2.py
--rw-r--r--   0        0        0      789 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/obround2.py
--rw-r--r--   0        0        0     1635 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
--rw-r--r--   0        0        0     2007 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
--rw-r--r--   0        0        0     8944 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/attributes2.py
--rw-r--r--   0        0        0     3922 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/command_buffer2.py
--rw-r--r--   0        0        0       88 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/__init__.py
--rw-r--r--   0        0        0      975 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
--rw-r--r--   0        0        0     4375 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/arc2.py
--rw-r--r--   0        0        0     2952 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
--rw-r--r--   0        0        0     2258 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/command2.py
--rw-r--r--   0        0        0     2477 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/flash2.py
--rw-r--r--   0        0        0     2688 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/line2.py
--rw-r--r--   0        0        0     1733 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/region2.py
--rw-r--r--   0        0        0    24876 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/context2.py
--rw-r--r--   0        0        0     4052 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/errors2.py
--rw-r--r--   0        0        0       66 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/__init__.py
--rw-r--r--   0        0        0      729 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py
--rw-r--r--   0        0        0      238 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/element2.py
--rw-r--r--   0        0        0      242 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/enums.py
--rw-r--r--   0        0        0       61 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
--rw-r--r--   0        0        0     1785 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
--rw-r--r--   0        0        0      674 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
--rw-r--r--   0        0        0     1207 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
--rw-r--r--   0        0        0      957 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
--rw-r--r--   0        0        0      663 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
--rw-r--r--   0        0        0      757 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/macro2.py
--rw-r--r--   0        0        0      392 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/point2.py
--rw-r--r--   0        0        0       56 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
--rw-r--r--   0        0        0      749 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
--rw-r--r--   0        0        0      811 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
--rw-r--r--   0        0        0      791 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
--rw-r--r--   0        0        0      588 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
--rw-r--r--   0        0        0      555 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
--rw-r--r--   0        0        0      849 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
--rw-r--r--   0        0        0      875 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
--rw-r--r--   0        0        0      532 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
--rw-r--r--   0        0        0      786 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
--rw-r--r--   0        0        0      207 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
--rw-r--r--   0        0        0      891 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement2.py
--rw-r--r--   0        0        0     1294 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
--rw-r--r--   0        0        0     5052 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2.py
--rw-r--r--   0        0        0    84867 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks.py
--rw-r--r--   0        0        0    29008 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py
--rw-r--r--   0        0        0    29444 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/parser2/state2.py
--rw-r--r--   0        0        0      135 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/__init__.py
--rw-r--r--   0        0        0     4767 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/abstract.py
--rw-r--r--   0        0        0      497 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/errors2.py
--rw-r--r--   0        0        0    30444 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/raster.py
--rw-r--r--   0        0        0    29602 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/renderer2/svg.py
--rw-r--r--   0        0        0    14537 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/revisions.py
--rw-r--r--   0        0        0     5321 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/state_enums.py
--rw-r--r--   0        0        0       27 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/__init__.py
--rw-r--r--   0        0        0      936 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/aperture_id.py
--rw-r--r--   0        0        0     1075 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/decorators.py
--rw-r--r--   0        0        0      162 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/errors.py
--rw-r--r--   0        0        0     4459 2024-04-18 23:23:58.711229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf
--rw-r--r--   0        0        0    38460 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.py
--rw-r--r--   0        0        0       22 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
--rw-r--r--   0        0        0      509 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
--rw-r--r--   0        0        0     2355 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokenizer.py
--rw-r--r--   0        0        0       32 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
--rw-r--r--   0        0        0     6972 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
--rw-r--r--   0        0        0    31743 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
--rw-r--r--   0        0        0     4355 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
--rw-r--r--   0        0        0     3984 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
--rw-r--r--   0        0        0       43 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
--rw-r--r--   0        0        0     2369 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
--rw-r--r--   0        0        0     2388 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
--rw-r--r--   0        0        0      907 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
--rw-r--r--   0        0        0     4049 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
--rw-r--r--   0        0        0     4775 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
--rw-r--r--   0        0        0      633 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
--rw-r--r--   0        0        0     2823 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
--rw-r--r--   0        0        0    10302 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
--rw-r--r--   0        0        0     4122 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
--rw-r--r--   0        0        0     4219 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
--rw-r--r--   0        0        0     3199 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
--rw-r--r--   0        0        0     1486 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
--rw-r--r--   0        0        0     7836 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
--rw-r--r--   0        0        0     1933 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
--rw-r--r--   0        0        0     2039 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
--rw-r--r--   0        0        0     2154 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
--rw-r--r--   0        0        0     2170 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
--rw-r--r--   0        0        0     1914 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
--rw-r--r--   0        0        0     2158 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
--rw-r--r--   0        0        0     1939 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
--rw-r--r--   0        0        0     2554 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
--rw-r--r--   0        0        0     2343 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
--rw-r--r--   0        0        0     2272 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
--rw-r--r--   0        0        0     2705 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
--rw-r--r--   0        0        0     2325 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
--rw-r--r--   0        0        0     2383 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
--rw-r--r--   0        0        0       20 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
--rw-r--r--   0        0        0      206 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
--rw-r--r--   0        0        0     2057 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
--rw-r--r--   0        0        0     3263 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
--rw-r--r--   0        0        0     2052 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
--rw-r--r--   0        0        0     2904 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
--rw-r--r--   0        0        0     2491 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
--rw-r--r--   0        0        0     3384 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
--rw-r--r--   0        0        0     2471 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
--rw-r--r--   0        0        0     3189 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
--rw-r--r--   0        0        0     3184 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
--rw-r--r--   0        0        0     1615 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
--rw-r--r--   0        0        0     1621 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
--rw-r--r--   0        0        0     1607 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
--rw-r--r--   0        0        0     1164 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
--rw-r--r--   0        0        0     7925 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
--rw-r--r--   0        0        0       62 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
--rw-r--r--   0        0        0     5585 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
--rw-r--r--   0        0        0      274 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
--rw-r--r--   0        0        0     1776 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
--rw-r--r--   0        0        0     2135 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
--rw-r--r--   0        0        0     3647 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
--rw-r--r--   0        0        0     2431 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
--rw-r--r--   0        0        0     3660 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
--rw-r--r--   0        0        0      360 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
--rw-r--r--   0        0        0     1935 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
--rw-r--r--   0        0        0       60 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
--rw-r--r--   0        0        0     4874 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
--rw-r--r--   0        0        0     4264 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
--rw-r--r--   0        0        0     4006 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
--rw-r--r--   0        0        0      944 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
--rw-r--r--   0        0        0      898 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
--rw-r--r--   0        0        0     5065 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
--rw-r--r--   0        0        0     4182 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
--rw-r--r--   0        0        0      866 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
--rw-r--r--   0        0        0     3980 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
--rw-r--r--   0        0        0     2204 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
--rw-r--r--   0        0        0      370 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
--rw-r--r--   0        0        0      953 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
--rw-r--r--   0        0        0     4388 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
--rw-r--r--   0        0        0     2711 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
--rw-r--r--   0        0        0     3801 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
--rw-r--r--   0        0        0     3090 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
--rw-r--r--   0        0        0     1892 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
--rw-r--r--   0        0        0     2122 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
--rw-r--r--   0        0        0     1477 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
--rw-r--r--   0        0        0     1724 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
--rw-r--r--   0        0        0      899 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/sequence_tools.py
--rw-r--r--   0        0        0      491 2024-04-18 23:23:58.715229 pygerber-2.3.1/src/pygerber/warnings.py
--rw-r--r--   0        0        0    14868 1970-01-01 00:00:00.000000 pygerber-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 10:01:43.663665 pygerber-2.3.2/LICENSE.md
+-rw-r--r--   0        0        0    12132 2024-05-30 10:01:43.663665 pygerber-2.3.2/README.md
+-rw-r--r--   0        0        0    12976 2024-05-30 10:01:43.795667 pygerber-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/__init__.py
+-rw-r--r--   0        0        0      149 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/__main__.py
+-rw-r--r--   0        0        0      858 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/__init__.py
+-rw-r--r--   0        0        0     4205 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/aperture_handle.py
+-rw-r--r--   0        0        0     6118 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/backend_cls.py
+-rw-r--r--   0        0        0       50 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/__init__.py
+-rw-r--r--   0        0        0     3958 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1165 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1214 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     1007 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_command.py
+-rw-r--r--   0        0        0     1226 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     1527 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1323 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1395 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1707 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      793 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands_handle.py
+-rw-r--r--   0        0        0     1101 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/drawing_target.py
+-rw-r--r--   0        0        0      280 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/errors.py
+-rw-r--r--   0        0        0      663 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/abstract/result_handle.py
+-rw-r--r--   0        0        0       65 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/__init__.py
+-rw-r--r--   0        0        0     2435 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/aperture_handle.py
+-rw-r--r--   0        0        0     8530 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/backend_cls.py
+-rw-r--r--   0        0        0     8452 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/color_scheme.py
+-rw-r--r--   0        0        0       81 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/__init__.py
+-rw-r--r--   0        0        0     1371 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py
+-rw-r--r--   0        0        0     1583 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py
+-rw-r--r--   0        0        0     1702 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py
+-rw-r--r--   0        0        0     2072 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py
+-rw-r--r--   0        0        0     2139 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py
+-rw-r--r--   0        0        0     1634 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py
+-rw-r--r--   0        0        0     1616 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py
+-rw-r--r--   0        0        0     1389 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py
+-rw-r--r--   0        0        0      317 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands_handle.py
+-rw-r--r--   0        0        0     4122 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/drawing_target.py
+-rw-r--r--   0        0        0      520 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/errors.py
+-rw-r--r--   0        0        0      801 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/image_tools.py
+-rw-r--r--   0        0        0     1589 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/backend/rasterized_2d/result_handle.py
+-rw-r--r--   0        0        0       53 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/error.py
+-rw-r--r--   0        0        0      369 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/frozen_general_model.py
+-rw-r--r--   0        0        0      364 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/general_model.py
+-rw-r--r--   0        0        0     2179 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/immutable_map_model.py
+-rw-r--r--   0        0        0     2860 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/position.py
+-rw-r--r--   0        0        0     4913 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/common/rgba.py
+-rw-r--r--   0        0        0       37 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/console/__init__.py
+-rw-r--r--   0        0        0     3410 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/console/commands.py
+-rw-r--r--   0        0        0     2950 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/console/raster_2d_style.py
+-rw-r--r--   0        0        0      925 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/__init__.py
+-rw-r--r--   0        0        0     1176 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/shape_flashes.grb
+-rw-r--r--   0        0        0    49675 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Cu.gbr
+-rw-r--r--   0        0        0     3742 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Mask.gbr
+-rw-r--r--   0        0        0     2486 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Paste.gbr
+-rw-r--r--   0        0        0     9518 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr
+-rw-r--r--   0        0        0    10101 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/examples/ucamco_ex_2_shapes.grb
+-rw-r--r--   0        0        0       50 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/__init__.py
+-rw-r--r--   0        0        0     1727 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/api/__init__.py
+-rw-r--r--   0        0        0     1130 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/api/_errors.py
+-rw-r--r--   0        0        0    12011 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/api/_layers.py
+-rw-r--r--   0        0        0    13437 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/api/_v2.py
+-rw-r--r--   0        0        0      981 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/api/v2.py
+-rw-r--r--   0        0        0      248 2024-05-30 10:01:43.795667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/__init__.py
+-rw-r--r--   0        0        0     1248 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/__main__.py
+-rw-r--r--   0        0        0      489 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/__init__.py
+-rw-r--r--   0        0        0     4711 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/document.py
+-rw-r--r--   0        0        0      167 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/error.py
+-rw-r--r--   0        0        0      273 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/errors.py
+-rw-r--r--   0        0        0     3891 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/server.py
+-rw-r--r--   0        0        0       29 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/linter/__init__.py
+-rw-r--r--   0        0        0     6540 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/linter/diagnostic.py
+-rw-r--r--   0        0        0       40 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/math/__init__.py
+-rw-r--r--   0        0        0     6193 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/math/bounding_box.py
+-rw-r--r--   0        0        0     5071 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/math/offset.py
+-rw-r--r--   0        0        0      711 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/math/rotate_point.py
+-rw-r--r--   0        0        0     8028 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/math/vector_2d.py
+-rw-r--r--   0        0        0       29 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/optimizer/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/optimizer/optimizer_pass/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser/__init__.py
+-rw-r--r--   0        0        0     2282 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser/errors.py
+-rw-r--r--   0        0        0     5942 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser/parser.py
+-rw-r--r--   0        0        0     6100 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser/state.py
+-rw-r--r--   0        0        0       36 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/__init__.py
+-rw-r--r--   0        0        0     1844 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/aperture2.py
+-rw-r--r--   0        0        0     2122 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/block2.py
+-rw-r--r--   0        0        0     1942 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/circle2.py
+-rw-r--r--   0        0        0     2056 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/macro2.py
+-rw-r--r--   0        0        0      789 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/obround2.py
+-rw-r--r--   0        0        0     1635 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/polygon2.py
+-rw-r--r--   0        0        0     2007 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py
+-rw-r--r--   0        0        0     8944 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/attributes2.py
+-rw-r--r--   0        0        0     3922 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/command_buffer2.py
+-rw-r--r--   0        0        0       88 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/__init__.py
+-rw-r--r--   0        0        0      975 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py
+-rw-r--r--   0        0        0     4375 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/arc2.py
+-rw-r--r--   0        0        0     2952 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py
+-rw-r--r--   0        0        0     2258 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/command2.py
+-rw-r--r--   0        0        0     2477 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/flash2.py
+-rw-r--r--   0        0        0     2688 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/line2.py
+-rw-r--r--   0        0        0     1733 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/region2.py
+-rw-r--r--   0        0        0    24876 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/context2.py
+-rw-r--r--   0        0        0     4052 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/errors2.py
+-rw-r--r--   0        0        0       66 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/__init__.py
+-rw-r--r--   0        0        0      729 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/assignment2.py
+-rw-r--r--   0        0        0      238 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/element2.py
+-rw-r--r--   0        0        0      242 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/enums.py
+-rw-r--r--   0        0        0       61 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/__init__.py
+-rw-r--r--   0        0        0     1785 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py
+-rw-r--r--   0        0        0      674 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py
+-rw-r--r--   0        0        0     1207 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py
+-rw-r--r--   0        0        0      957 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py
+-rw-r--r--   0        0        0      663 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py
+-rw-r--r--   0        0        0      757 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/macro2.py
+-rw-r--r--   0        0        0      392 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/point2.py
+-rw-r--r--   0        0        0       56 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/__init__.py
+-rw-r--r--   0        0        0      749 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py
+-rw-r--r--   0        0        0      811 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py
+-rw-r--r--   0        0        0      791 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py
+-rw-r--r--   0        0        0      588 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py
+-rw-r--r--   0        0        0      555 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py
+-rw-r--r--   0        0        0      849 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py
+-rw-r--r--   0        0        0      875 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py
+-rw-r--r--   0        0        0      532 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py
+-rw-r--r--   0        0        0      786 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py
+-rw-r--r--   0        0        0      207 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/primitive2.py
+-rw-r--r--   0        0        0      891 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/statement2.py
+-rw-r--r--   0        0        0     1294 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py
+-rw-r--r--   0        0        0     5052 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2.py
+-rw-r--r--   0        0        0    84867 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2hooks.py
+-rw-r--r--   0        0        0    29008 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2hooks_base.py
+-rw-r--r--   0        0        0    29444 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/parser2/state2.py
+-rw-r--r--   0        0        0      135 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/renderer2/__init__.py
+-rw-r--r--   0        0        0     4767 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/renderer2/abstract.py
+-rw-r--r--   0        0        0      497 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/renderer2/errors2.py
+-rw-r--r--   0        0        0    31610 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/renderer2/raster.py
+-rw-r--r--   0        0        0    29602 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/renderer2/svg.py
+-rw-r--r--   0        0        0    14537 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/revisions.py
+-rw-r--r--   0        0        0     5321 2024-05-30 10:01:43.799667 pygerber-2.3.2/src/pygerber/gerberx3/state_enums.py
+-rw-r--r--   0        0        0       27 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/__init__.py
+-rw-r--r--   0        0        0      936 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/aperture_id.py
+-rw-r--r--   0        0        0     1075 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/decorators.py
+-rw-r--r--   0        0        0      162 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/errors.py
+-rw-r--r--   0        0        0     4459 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/grammar.ebnf
+-rw-r--r--   0        0        0    38477 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/grammar.py
+-rw-r--r--   0        0        0       22 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/helpers/__init__.py
+-rw-r--r--   0        0        0      509 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/helpers/gerber_code_enum.py
+-rw-r--r--   0        0        0     2355 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokenizer.py
+-rw-r--r--   0        0        0       32 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/__init__.py
+-rw-r--r--   0        0        0     6972 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py
+-rw-r--r--   0        0        0    31743 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py
+-rw-r--r--   0        0        0     4355 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py
+-rw-r--r--   0        0        0     3984 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py
+-rw-r--r--   0        0        0       43 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/__init__.py
+-rw-r--r--   0        0        0     2369 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py
+-rw-r--r--   0        0        0     2388 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py
+-rw-r--r--   0        0        0      907 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py
+-rw-r--r--   0        0        0     4049 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py
+-rw-r--r--   0        0        0     4775 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py
+-rw-r--r--   0        0        0      633 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py
+-rw-r--r--   0        0        0     2823 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py
+-rw-r--r--   0        0        0    10302 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py
+-rw-r--r--   0        0        0     4122 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py
+-rw-r--r--   0        0        0     4219 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py
+-rw-r--r--   0        0        0     3199 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py
+-rw-r--r--   0        0        0     1486 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py
+-rw-r--r--   0        0        0     7836 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py
+-rw-r--r--   0        0        0     1933 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py
+-rw-r--r--   0        0        0     2039 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py
+-rw-r--r--   0        0        0     2154 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py
+-rw-r--r--   0        0        0     2170 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py
+-rw-r--r--   0        0        0     1914 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py
+-rw-r--r--   0        0        0     2158 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py
+-rw-r--r--   0        0        0     1939 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py
+-rw-r--r--   0        0        0     2554 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py
+-rw-r--r--   0        0        0     2343 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py
+-rw-r--r--   0        0        0     2272 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py
+-rw-r--r--   0        0        0     2705 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py
+-rw-r--r--   0        0        0     2325 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py
+-rw-r--r--   0        0        0     2383 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py
+-rw-r--r--   0        0        0       20 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/groups/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/groups/ast.py
+-rw-r--r--   0        0        0     2057 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py
+-rw-r--r--   0        0        0     3263 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py
+-rw-r--r--   0        0        0     2052 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py
+-rw-r--r--   0        0        0     2904 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py
+-rw-r--r--   0        0        0     2491 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py
+-rw-r--r--   0        0        0     3384 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py
+-rw-r--r--   0        0        0     2471 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py
+-rw-r--r--   0        0        0     3189 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py
+-rw-r--r--   0        0        0     3184 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py
+-rw-r--r--   0        0        0     1615 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py
+-rw-r--r--   0        0        0     1621 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py
+-rw-r--r--   0        0        0     1607 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py
+-rw-r--r--   0        0        0     1164 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py
+-rw-r--r--   0        0        0     7925 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py
+-rw-r--r--   0        0        0       62 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/__init__.py
+-rw-r--r--   0        0        0     5585 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py
+-rw-r--r--   0        0        0      274 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/errors.py
+-rw-r--r--   0        0        0     1776 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py
+-rw-r--r--   0        0        0     2135 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py
+-rw-r--r--   0        0        0     3647 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py
+-rw-r--r--   0        0        0     2431 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py
+-rw-r--r--   0        0        0     3660 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py
+-rw-r--r--   0        0        0      360 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_context.py
+-rw-r--r--   0        0        0     1935 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py
+-rw-r--r--   0        0        0       60 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/__init__.py
+-rw-r--r--   0        0        0     4874 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py
+-rw-r--r--   0        0        0     4264 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py
+-rw-r--r--   0        0        0     4006 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py
+-rw-r--r--   0        0        0      944 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py
+-rw-r--r--   0        0        0      898 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py
+-rw-r--r--   0        0        0     5065 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py
+-rw-r--r--   0        0        0     4182 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py
+-rw-r--r--   0        0        0      866 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py
+-rw-r--r--   0        0        0     3980 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py
+-rw-r--r--   0        0        0     2204 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py
+-rw-r--r--   0        0        0      370 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/primitive.py
+-rw-r--r--   0        0        0      953 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py
+-rw-r--r--   0        0        0     4388 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py
+-rw-r--r--   0        0        0     2711 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py
+-rw-r--r--   0        0        0     3801 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py
+-rw-r--r--   0        0        0     3090 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py
+-rw-r--r--   0        0        0     1892 2024-05-30 10:01:43.803667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py
+-rw-r--r--   0        0        0     2122 2024-05-30 10:01:43.807667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py
+-rw-r--r--   0        0        0     1477 2024-05-30 10:01:43.807667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py
+-rw-r--r--   0        0        0     1724 2024-05-30 10:01:43.807667 pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py
+-rw-r--r--   0        0        0      899 2024-05-30 10:01:43.807667 pygerber-2.3.2/src/pygerber/sequence_tools.py
+-rw-r--r--   0        0        0      491 2024-05-30 10:01:43.807667 pygerber-2.3.2/src/pygerber/warnings.py
+-rw-r--r--   0        0        0    14868 1970-01-01 00:00:00.000000 pygerber-2.3.2/PKG-INFO
```

### Comparing `pygerber-2.3.1/LICENSE.md` & `pygerber-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/README.md` & `pygerber-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/pyproject.toml` & `pygerber-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pygerber"
-version = "2.3.1"
+version = "2.3.2"
 description = "Parsing, formatting and rendering toolkit for Gerber X3 file format"
 authors = ["Krzysztof Wisniewski <argmaster.world@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.facebook.com/pygerber"
 repository = "https://github.com/Argmaster/pygerber"
 documentation = "https://argmaster.github.io/pygerber/latest"
```

### Comparing `pygerber-2.3.1/src/pygerber/backend/__init__.py` & `pygerber-2.3.2/src/pygerber/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/aperture_handle.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/backend_cls.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_arc.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_circle.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_command.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_paste.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_polygon.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_region.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/draw_commands_handle.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/draw_commands_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/drawing_target.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/abstract/result_handle.py` & `pygerber-2.3.2/src/pygerber/backend/abstract/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/aperture_handle.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/aperture_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/backend_cls.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/backend_cls.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/color_scheme.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/color_scheme.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_arc.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_paste.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_rectangle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/draw_commands/draw_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/drawing_target.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/drawing_target.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/errors.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/image_tools.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/image_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/backend/rasterized_2d/result_handle.py` & `pygerber-2.3.2/src/pygerber/backend/rasterized_2d/result_handle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/common/immutable_map_model.py` & `pygerber-2.3.2/src/pygerber/common/immutable_map_model.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/common/position.py` & `pygerber-2.3.2/src/pygerber/common/position.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/common/rgba.py` & `pygerber-2.3.2/src/pygerber/common/rgba.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/console/commands.py` & `pygerber-2.3.2/src/pygerber/console/commands.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/console/raster_2d_style.py` & `pygerber-2.3.2/src/pygerber/console/raster_2d_style.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/__init__.py` & `pygerber-2.3.2/src/pygerber/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/shape_flashes.grb` & `pygerber-2.3.2/src/pygerber/examples/shape_flashes.grb`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Cu.gbr` & `pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Cu.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Mask.gbr` & `pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Mask.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Paste.gbr` & `pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Paste.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr` & `pygerber-2.3.2/src/pygerber/examples/simple_2layer-F_Silkscreen.gbr`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/examples/ucamco_ex_2_shapes.grb` & `pygerber-2.3.2/src/pygerber/examples/ucamco_ex_2_shapes.grb`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/api/__init__.py` & `pygerber-2.3.2/src/pygerber/gerberx3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/api/_errors.py` & `pygerber-2.3.2/src/pygerber/gerberx3/api/_errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/api/_layers.py` & `pygerber-2.3.2/src/pygerber/gerberx3/api/_layers.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/api/_v2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/api/_v2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/api/v2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/api/v2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/language_server/__main__.py` & `pygerber-2.3.2/src/pygerber/gerberx3/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/document.py` & `pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/document.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/language_server/_internals/server.py` & `pygerber-2.3.2/src/pygerber/gerberx3/language_server/_internals/server.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/linter/diagnostic.py` & `pygerber-2.3.2/src/pygerber/gerberx3/linter/diagnostic.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/math/bounding_box.py` & `pygerber-2.3.2/src/pygerber/gerberx3/math/bounding_box.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/math/offset.py` & `pygerber-2.3.2/src/pygerber/gerberx3/math/offset.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/math/rotate_point.py` & `pygerber-2.3.2/src/pygerber/gerberx3/math/rotate_point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/math/vector_2d.py` & `pygerber-2.3.2/src/pygerber/gerberx3/math/vector_2d.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser/errors.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser/errors.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser/parser.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser/state.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser/state.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/aperture2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/aperture2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/block2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/block2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/circle2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/circle2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/macro2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/macro2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/obround2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/obround2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/polygon2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/polygon2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/apertures2/rectangle2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/attributes2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/attributes2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/command_buffer2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/command_buffer2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/aperture_draw_command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/arc2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/arc2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/buffer_command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/command2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/command2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/flash2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/flash2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/line2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/commands2/region2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/commands2/region2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/context2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/context2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/errors2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/errors2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/assignment2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/assignment2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/binary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/constant2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/expression2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/unary2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/expressions2/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/macro2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/macro2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_1_circle2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_20_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_21_center_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_22_lower_left_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_2_vector_line2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_4_outline2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_5_polygon2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_6_moire2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/primitives2/code_7_thermal2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/statement2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/macro2/statement_buffer2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2hooks.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/parser2hooks_base.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/parser2hooks_base.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/parser2/state2.py` & `pygerber-2.3.2/src/pygerber/gerberx3/parser2/state2.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/abstract.py` & `pygerber-2.3.2/src/pygerber/gerberx3/renderer2/abstract.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/raster.py` & `pygerber-2.3.2/src/pygerber/gerberx3/renderer2/raster.py`

 * *Files 3% similar despite different names*

```diff
@@ -479,16 +479,16 @@
 
         if end_angle <= start_angle:
             end_angle += 360
 
         self.frame.arc(
             command.transform.polarity,
             bbox,
-            start_angle,
             end_angle,
+            start_angle,
             width=self.convert_size(command.aperture.get_stroke_width()),
         )
 
         command.aperture.render_flash(
             self.renderer,
             Flash2(
                 transform=command.transform,
@@ -496,20 +496,61 @@
                 aperture=command.aperture,
                 flash_point=command.end_point,
             ),
         )
 
     def render_cc_arc(self, command: CCArc2) -> None:
         """Render arc to target image."""
-        return self.render_arc(
-            command.model_copy(
-                update={
-                    "start_point": command.start_point,
-                    "end_point": command.end_point,
-                },
+        command.aperture.render_flash(
+            self.renderer,
+            Flash2(
+                transform=command.transform,
+                attributes=command.attributes,
+                aperture=command.aperture,
+                flash_point=command.start_point,
+            ),
+        )
+
+        start_angle = (
+            command.get_relative_start_point().angle_between(
+                Vector2D.UNIT_X,
+            )
+            % 360
+        )
+        end_angle = (
+            command.get_relative_end_point().angle_between(
+                Vector2D.UNIT_X,
+            )
+            % 360
+        )
+        bbox = self.convert_bbox(
+            BoundingBox.from_diameter(
+                (command.get_radius() * 2) + (command.aperture.get_stroke_width()),
+            )
+            + command.center_point,
+        )
+
+        if end_angle <= start_angle:
+            end_angle += 360
+
+        self.frame.arc(
+            command.transform.polarity,
+            bbox,
+            start_angle,
+            end_angle,
+            width=self.convert_size(command.aperture.get_stroke_width()),
+        )
+
+        command.aperture.render_flash(
+            self.renderer,
+            Flash2(
+                transform=command.transform,
+                attributes=command.attributes,
+                aperture=command.aperture,
+                flash_point=command.end_point,
             ),
         )
 
     def render_flash_circle(self, command: Flash2, aperture: Circle2) -> None:
         """Render flash circle to target image."""
         aperture_id = self.get_aperture_id(aperture, command.transform)
         raster_aperture = self.get_aperture(aperture_id)
```

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/renderer2/svg.py` & `pygerber-2.3.2/src/pygerber/gerberx3/renderer2/svg.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/revisions.py` & `pygerber-2.3.2/src/pygerber/gerberx3/revisions.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/state_enums.py` & `pygerber-2.3.2/src/pygerber/gerberx3/state_enums.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/aperture_id.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/aperture_id.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/decorators.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/decorators.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.ebnf` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/grammar.ebnf`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/grammar.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/grammar.py`

 * *Files 0% similar despite different names*

```diff
@@ -553,15 +553,15 @@
     def _build_comment_token(self) -> ParserElement:
         wrapper = self.wrapper
         eoex = self._build_eoex()
 
         # A human readable comment, does not affect the image.
         return wrapper(
             self.options.g04_comment_token_cls,
-            Regex("G0*4") + self._build_string() + eoex,
+            Regex("G0*4") + Opt(self._build_string(), default="") + eoex,
         )
 
     def _build_define_aperture(self) -> ParserElement:
         wrapper = self.wrapper
 
         ad = Literal("AD").set_name("AD code")
```

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokenizer.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ab_block_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ad_define_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/as_axis_select.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/attribute_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/extended_command.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/gerber_code.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/group.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/bases/token_accessor.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/coordinate.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d01_draw.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d02_move.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/d03_flash.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/dnn_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/end_of_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/fs_coordinate_format.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g01_set_linear.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g02_set_clockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g03_set_counterclockwise_circular.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g04_comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g36_begin_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g37_end_region.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g54_select_aperture.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g70_set_unit_inch.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g71_set_unit_mm.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g74_single_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g75_multi_quadrant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g90_set_coordinate_absolute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/g91_set_coordinate_incremental.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/groups/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/in_image_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/invalid_token.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ip_image_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lm_load_mirroring.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ln_load_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lp_load_polarity.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/lr_load_rotation.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ls_load_scaling.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m00_program_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m01_optional_stop.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/m02_end_of_file.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/__init__.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/am_macro.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/binary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/macro_expression.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/numeric_constant.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/unary.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/expressions/variable_name.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/macro_begin.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/point.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_1_circle.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_20_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_21_center_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_22_lower_left_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_2_vector_line.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_4_outline.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_5_polygon.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_6_moire.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/code_7_thermal.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/comment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/statement.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/macro/statements/variable_assignment.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/mo_unit_mode.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/of_image_offset.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/sr_step_repeat.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/ta_aperture_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/td_delete_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/tf_file_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py` & `pygerber-2.3.2/src/pygerber/gerberx3/tokenizer/tokens/to_object_attribute.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/src/pygerber/sequence_tools.py` & `pygerber-2.3.2/src/pygerber/sequence_tools.py`

 * *Files identical despite different names*

### Comparing `pygerber-2.3.1/PKG-INFO` & `pygerber-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygerber
-Version: 2.3.1
+Version: 2.3.2
 Summary: Parsing, formatting and rendering toolkit for Gerber X3 file format
 Home-page: https://www.facebook.com/pygerber
 License: MIT
 Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski
 Author-email: argmaster.world@gmail.com
 Requires-Python: >=3.8,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygerber Version: 2.3.1 Summary: Parsing,
+Metadata-Version: 2.1 Name: pygerber Version: 2.3.2 Summary: Parsing,
 formatting and rendering toolkit for Gerber X3 file format Home-page: https://
 www.facebook.com/pygerber License: MIT Keywords: gerber,pcb,embedded,images,x3
 Author: Krzysztof Wisniewski Author-email: argmaster.world@gmail.com Requires-
 Python: >=3.8,<3.13 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop Classifier: Intended
 Audience :: Information Technology Classifier: Intended Audience ::
```

