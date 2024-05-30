# Comparing `tmp/types-reportlab-4.2.0.20240525.tar.gz` & `tmp/types-reportlab-4.2.0.20240530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-reportlab-4.2.0.20240525.tar", last modified: Sat May 25 02:20:25 2024, max compression
+gzip compressed data, was "types-reportlab-4.2.0.20240530.tar", last modified: Thu May 30 02:24:28 2024, max compression
```

## Comparing `types-reportlab-4.2.0.20240525.tar` & `types-reportlab-4.2.0.20240530.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.108190 types-reportlab-4.2.0.20240525/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-25 02:20:23.000000 types-reportlab-4.2.0.20240525/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-25 02:20:23.000000 types-reportlab-4.2.0.20240525/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-25 02:20:25.108190 types-reportlab-4.2.0.20240525/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.088190 types-reportlab-4.2.0.20240525/reportlab-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-25 02:20:23.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.088190 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.092190 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code128.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code39.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code93.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/common.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/dmtx.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/eanbc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/ecc200datamatrix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/fourstate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/lto.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/qr.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/qrencoder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/usps.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/usps4s.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/widgets.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.092190 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/areas.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/axes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/barcharts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/dotbox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/doughnut.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/legends.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/linecharts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/lineplots.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/piecharts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/slidebox.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/spider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/textlabels.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/utils3d.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPDF.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPM.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPS.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4945 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderSVG.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderbase.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.096190 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/bubble.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/clustered_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/clustered_column.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/excelcolors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/exploded_pie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/filled_radar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/line_chart.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/linechart_with_markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/radar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/runall.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/scatter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/scatter_lines.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/scatter_lines_markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/simple_pie.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/stacked_bar.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/stacked_column.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/shapes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/svgpath.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/transform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgetbase.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.096190 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/adjustableArrow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/eventcal.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/flags.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/grids.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/markers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/signsandsymbols.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/table.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.100190 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/PyFontify.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/abag.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/arciv.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/attrmap.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/boxstuff.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/codecharts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/colors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/corp.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/enums.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/extformat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/fontfinder.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/fonts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/formatters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/geomutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/normalDate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/pagesizes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/pdfencrypt.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/pygments2xpre.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/randomtext.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rl_accel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rl_safe_eval.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rltempfile.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rparsexml.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/sequencer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/styles.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/testutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/textsplit.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/units.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/validators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/lib/yaml.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.104190 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/acroform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/cidfonts.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfdoc.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfform.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfmetrics.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfpattern.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfutils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/rl_codecs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/ttfonts.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.104190 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/canvas.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/pathobject.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/pdfgeom.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/pdfimages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/textobject.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.104190 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/doctemplate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/figures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/flowables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/frames.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/multicol.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/para.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/paragraph.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/paraparser.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/tableofcontents.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/tables.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/xpreformatted.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:23.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/rl_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-25 02:20:09.000000 types-reportlab-4.2.0.20240525/reportlab-stubs/rl_settings.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 02:20:25.108190 types-reportlab-4.2.0.20240525/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-25 02:20:23.000000 types-reportlab-4.2.0.20240525/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 02:20:25.108190 types-reportlab-4.2.0.20240525/types_reportlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-25 02:20:25.000000 types-reportlab-4.2.0.20240525/types_reportlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-25 02:20:25.000000 types-reportlab-4.2.0.20240525/types_reportlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 02:20:25.000000 types-reportlab-4.2.0.20240525/types_reportlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-25 02:20:25.000000 types-reportlab-4.2.0.20240525/types_reportlab.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.380992 types-reportlab-4.2.0.20240530/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 02:24:27.000000 types-reportlab-4.2.0.20240530/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 02:24:27.000000 types-reportlab-4.2.0.20240530/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 02:24:28.380992 types-reportlab-4.2.0.20240530/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.364992 types-reportlab-4.2.0.20240530/reportlab-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 02:24:27.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.364992 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.368991 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code128.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code39.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code93.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/common.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/dmtx.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/eanbc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/ecc200datamatrix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/fourstate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/lto.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/qr.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/qrencoder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/usps.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/usps4s.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/widgets.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.368991 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/areas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5941 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/axes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/barcharts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/dotbox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/doughnut.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/legends.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/linecharts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/lineplots.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/piecharts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/slidebox.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/spider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/textlabels.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/utils3d.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPDF.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPM.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3696 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPS.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderSVG.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderbase.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.372992 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/bubble.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/clustered_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/clustered_column.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/excelcolors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/exploded_pie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/filled_radar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/line_chart.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/linechart_with_markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/radar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/runall.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/scatter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/scatter_lines.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/scatter_lines_markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/simple_pie.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/stacked_bar.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/stacked_column.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/shapes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/svgpath.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/transform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgetbase.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.372992 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/adjustableArrow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/eventcal.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/flags.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/grids.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/markers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/signsandsymbols.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/table.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.376992 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/PyFontify.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/abag.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/arciv.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/attrmap.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/boxstuff.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/codecharts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/colors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/corp.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/enums.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/extformat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/fontfinder.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/fonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/formatters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/geomutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/normalDate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/pagesizes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/pdfencrypt.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/pygments2xpre.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/randomtext.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rl_accel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rl_safe_eval.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rltempfile.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rparsexml.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/sequencer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/styles.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/testutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/textsplit.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/units.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/validators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/lib/yaml.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.376992 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/acroform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/cidfonts.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfdoc.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfform.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfmetrics.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfpattern.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfutils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/rl_codecs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/ttfonts.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.376992 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11790 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/canvas.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/pathobject.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/pdfgeom.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/pdfimages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/textobject.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.380992 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/doctemplate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/figures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    15039 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/flowables.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/frames.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/multicol.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/para.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/paragraph.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/paraparser.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/tableofcontents.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/tables.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/xpreformatted.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:27.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/rl_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-30 02:24:11.000000 types-reportlab-4.2.0.20240530/reportlab-stubs/rl_settings.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 02:24:28.380992 types-reportlab-4.2.0.20240530/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-30 02:24:27.000000 types-reportlab-4.2.0.20240530/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 02:24:28.380992 types-reportlab-4.2.0.20240530/types_reportlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 02:24:28.000000 types-reportlab-4.2.0.20240530/types_reportlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-30 02:24:28.000000 types-reportlab-4.2.0.20240530/types_reportlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 02:24:28.000000 types-reportlab-4.2.0.20240530/types_reportlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 02:24:28.000000 types-reportlab-4.2.0.20240530/types_reportlab.egg-info/top_level.txt
```

### Comparing `types-reportlab-4.2.0.20240525/PKG-INFO` & `types-reportlab-4.2.0.20240530/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-reportlab
-Version: 4.2.0.20240525
+Version: 4.2.0.20240530
 Summary: Typing stubs for reportlab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/reportlab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-reportlab` aims to provide accurate annotations
 for `reportlab==4.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/reportlab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc33ba67ba25545e0decb5897b3d56b40c88b0b5` and was tested
+This package was generated from typeshed commit `c82d29fc7614a9ecd33bd416386062ba2915850d` and was tested
 with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code128.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code128.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code39.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code39.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/code93.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/code93.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/common.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/common.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/dmtx.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/dmtx.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/eanbc.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/eanbc.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/ecc200datamatrix.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/ecc200datamatrix.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/lto.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/lto.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/qr.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/qr.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/qrencoder.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/qrencoder.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/usps.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/usps.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/usps4s.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/usps4s.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/barcode/widgets.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/barcode/widgets.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/axes.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/axes.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/barcharts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/barcharts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/dotbox.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/dotbox.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/doughnut.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/doughnut.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/legends.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/legends.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/linecharts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/linecharts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/lineplots.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/lineplots.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/piecharts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/piecharts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/slidebox.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/slidebox.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/spider.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/spider.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/textlabels.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/textlabels.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/utils.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/charts/utils3d.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/charts/utils3d.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPDF.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPDF.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from _typeshed import Incomplete
-from typing import Final
+from typing import IO, Final
 
 from reportlab.graphics.renderbase import Renderer
+from reportlab.graphics.shapes import Drawing
+from reportlab.pdfgen.canvas import Canvas
 from reportlab.platypus import Flowable
 
 __version__: Final[str]
 
-def draw(drawing, canvas, x, y, showBoundary=...) -> None: ...
+def draw(drawing: Drawing, canvas: Canvas, x: float, y: float, showBoundary=...) -> None: ...
 
 class _PDFRenderer(Renderer):
     def __init__(self) -> None: ...
     def drawNode(self, node) -> None: ...
     def drawRect(self, rect) -> None: ...
     def drawImage(self, image) -> None: ...
     def drawLine(self, line) -> None: ...
@@ -28,10 +30,10 @@
 class GraphicsFlowable(Flowable):
     drawing: Incomplete
     width: Incomplete
     height: Incomplete
     def __init__(self, drawing) -> None: ...
     def draw(self) -> None: ...
 
-def drawToFile(d, fn, msg: str = "", showBoundary=..., autoSize: int = 1, canvasKwds={}) -> None: ...
-def drawToString(d, msg: str = "", showBoundary=..., autoSize: int = 1, canvasKwds={}): ...
+def drawToFile(d: Drawing, fn: str | IO[bytes], msg: str = "", showBoundary=..., autoSize: int = 1, canvasKwds={}) -> None: ...
+def drawToString(d: Drawing, msg: str = "", showBoundary=..., autoSize: int = 1, canvasKwds={}) -> str: ...
 def test(outDir: str = "pdfout", shout: bool = False) -> None: ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPM.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPM.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from _typeshed import Incomplete
-from typing import Final
+from typing import IO, Final
 
 from reportlab.graphics.renderbase import Renderer
+from reportlab.graphics.shapes import Drawing
+from reportlab.pdfgen.canvas import Canvas
 
 __version__: Final[str]
 
 def Color2Hex(c): ...
 def CairoColor(c): ...
-def draw(drawing, canvas, x, y, showBoundary=...) -> None: ...
+def draw(drawing: Drawing, canvas: Canvas, x: float, y: float, showBoundary=...) -> None: ...
 
 class _PMRenderer(Renderer):
     def pop(self) -> None: ...
     def push(self, node) -> None: ...
     def applyState(self) -> None: ...
     def initState(self, x, y) -> None: ...
     def drawNode(self, node) -> None: ...
@@ -68,58 +70,58 @@
     def setLineCap(self, cap) -> None: ...
     lineJoin: Incomplete
     def setLineJoin(self, join) -> None: ...
     strokeWidth: Incomplete
     def setLineWidth(self, width) -> None: ...
 
 def drawToPMCanvas(
-    d,
-    dpi: int = 72,
-    bg: int = 16777215,
+    d: Drawing,
+    dpi: float = 72,
+    bg: int = 0xFFFFFF,
     configPIL: Incomplete | None = None,
     showBoundary=...,
     backend="rlPyCairo",
     backendFmt: str = "RGB",
 ): ...
 def drawToPIL(
-    d,
-    dpi: int = 72,
-    bg: int = 16777215,
+    d: Drawing,
+    dpi: float = 72,
+    bg: int = 0xFFFFFF,
     configPIL: Incomplete | None = None,
     showBoundary=...,
     backend="rlPyCairo",
     backendFmt: str = "RGB",
 ): ...
 def drawToPILP(
-    d,
-    dpi: int = 72,
-    bg: int = 16777215,
+    d: Drawing,
+    dpi: float = 72,
+    bg: int = 0xFFFFFF,
     configPIL: Incomplete | None = None,
     showBoundary=...,
     backend="rlPyCairo",
     backendFmt: str = "RGB",
 ): ...
 def drawToFile(
-    d,
-    fn,
+    d: Drawing,
+    fn: str | IO[bytes],
     fmt: str = "GIF",
-    dpi: int = 72,
-    bg: int = 16777215,
+    dpi: float = 72,
+    bg: int = 0xFFFFFF,
     configPIL: Incomplete | None = None,
     showBoundary=...,
     backend="rlPyCairo",
     backendFmt: str = "RGB",
 ) -> None: ...
 def drawToString(
-    d,
+    d: Drawing,
     fmt: str = "GIF",
-    dpi: int = 72,
-    bg: int = 16777215,
+    dpi: float = 72,
+    bg: int = 0xFFFFFF,
     configPIL: Incomplete | None = None,
     showBoundary=...,
     backend="rlPyCairo",
     backendFmt: str = "RGB",
-): ...
+) -> str: ...
 
 save = drawToFile
 
 def test(outDir: str = "pmout", shout: bool = False): ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderPS.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderPS.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from _typeshed import Incomplete
-from typing import Final
+from typing import IO, Final
 
 from reportlab.graphics.renderbase import Renderer
+from reportlab.graphics.shapes import Drawing
+from reportlab.pdfgen.canvas import Canvas
 
 __version__: Final[str]
 PS_WinAnsiEncoding: Final[str]
 
 class PSCanvas:
     comments: int
     code: Incomplete
@@ -46,15 +48,15 @@
     def closePath(self) -> None: ...
     def polyLine(self, p) -> None: ...
     def drawFigure(self, partList, closed: int = 0) -> None: ...
     def translate(self, x, y) -> None: ...
     def scale(self, x, y) -> None: ...
     def transform(self, a, b, c, d, e, f) -> None: ...
 
-def draw(drawing, canvas, x: int = 0, y: int = 0, showBoundary=0) -> None: ...
+def draw(drawing: Drawing, canvas: Canvas, x: float = 0, y: float = 0, showBoundary=0) -> None: ...
 
 class _PSRenderer(Renderer):
     def drawNode(self, node) -> None: ...
     def drawRect(self, rect) -> None: ...
     def drawLine(self, line) -> None: ...
     def drawCircle(self, circle) -> None: ...
     def drawWedge(self, wedge) -> None: ...
@@ -62,10 +64,10 @@
     def drawEllipse(self, ellipse) -> None: ...
     def drawPolygon(self, p) -> None: ...
     def drawString(self, stringObj) -> None: ...
     def drawPath(self, path, fillMode: Incomplete | None = None): ...
     def applyStateChanges(self, delta, newState) -> None: ...
     def drawImage(self, image) -> None: ...
 
-def drawToFile(d, fn, showBoundary=0, **kwd) -> None: ...
-def drawToString(d, showBoundary=0): ...
+def drawToFile(d: Drawing, fn: IO[bytes], showBoundary=0, **kwd) -> None: ...
+def drawToString(d: Drawing, showBoundary=0) -> str: ...
 def test(outDir: str = "epsout", shout: bool = False) -> None: ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderSVG.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderSVG.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from _typeshed import Incomplete
 from collections.abc import Sequence
 from math import cos as cos, pi as pi, sin as sin
-from typing import Final
+from typing import IO, Final
 
 from reportlab.graphics.renderbase import Renderer
+from reportlab.graphics.shapes import Drawing
+from reportlab.pdfgen.canvas import Canvas
 
 AREA_STYLES: Final[Sequence[str]]
 LINE_STYLES: Final[Sequence[str]]
 TEXT_STYLES: Final[Sequence[str]]
 EXTRA_STROKE_STYLES: Final[Sequence[str]]
 EXTRA_FILL_STYLES: Final[Sequence[str]]
 
-def drawToString(d, showBoundary=0, **kwds): ...
-def drawToFile(d, fn, showBoundary=0, **kwds) -> None: ...
-def draw(drawing, canvas, x: int = 0, y: int = 0, showBoundary=0) -> None: ...
+def drawToString(d: Drawing, showBoundary=0, **kwds) -> str: ...
+def drawToFile(d: Drawing, fn: str | IO[str], showBoundary=0, **kwds) -> None: ...
+def draw(drawing: Drawing, canvas: Canvas, x: float = 0, y: float = 0, showBoundary=0) -> None: ...
 def transformNode(doc, newTag, node: Incomplete | None = None, **attrDict): ...
 
 class EncodedWriter(list[Incomplete]):
     BOMS: Incomplete
     encoding: Incomplete
     def __init__(self, encoding, bom: bool = False) -> None: ...
     def write(self, u) -> None: ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/renderbase.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/renderbase.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/samples/excelcolors.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/samples/excelcolors.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/utils.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgetbase.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgetbase.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,19 @@
     def verify(self) -> None: ...
     def __setattr__(self, name, value) -> None: ...
     def getProperties(self, recur: int = 1): ...
     def setProperties(self, propDict) -> None: ...
     def dumpProperties(self, prefix: str = "") -> None: ...
 
 class Widget(PropHolder, shapes.UserNode):
+    # TODO: draw should probably be marked abstract
     def draw(self) -> None: ...
     def demo(self) -> None: ...
-    def provideNode(self): ...
-    def getBounds(self): ...
+    def provideNode(self) -> shapes.Shape: ...
+    def getBounds(self) -> tuple[float, float, float, float]: ...
 
 class ScaleWidget(Widget):
     x: Incomplete
     y: Incomplete
     contents: Incomplete
     scale: Incomplete
     def __init__(self, x: int = 0, y: int = 0, scale: float = 1.0, contents: Incomplete | None = None) -> None: ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/eventcal.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/eventcal.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/flags.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/flags.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/grids.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/grids.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from _typeshed import Incomplete
-from typing import Final
+from typing import Final, NoReturn
 
 from reportlab.graphics.shapes import LineShape
 from reportlab.graphics.widgetbase import Widget
 
 __version__: Final[str]
 
 def frange(start, end: Incomplete | None = None, inc: Incomplete | None = None): ...
@@ -68,7 +68,9 @@
     fillColorStart: Incomplete
     fillColorEnd: Incomplete
     cylinderMode: int
     numShades: int
     points: Incomplete
     def __init__(self, **kw) -> None: ...
     def draw(self): ...
+    # NOTE: widgets don't implement this, only actual shapes
+    def copy(self) -> NoReturn: ...
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/signsandsymbols.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/signsandsymbols.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/graphics/widgets/table.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/graphics/widgets/table.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/attrmap.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/attrmap.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/codecharts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/codecharts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/colors.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/colors.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/corp.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/corp.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/fontfinder.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/fontfinder.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/formatters.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/formatters.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/logger.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/logger.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/normalDate.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/normalDate.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/pagesizes.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/pagesizes.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/pdfencrypt.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/pdfencrypt.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/randomtext.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/randomtext.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rl_safe_eval.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rl_safe_eval.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/rparsexml.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/rparsexml.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/sequencer.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/sequencer.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/styles.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/styles.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/testutils.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/testutils.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/textsplit.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/textsplit.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/utils.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/validators.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/validators.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/lib/yaml.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/lib/yaml.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/acroform.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/acroform.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/cidfonts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/cidfonts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfdoc.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfdoc.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfform.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfform.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfmetrics.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfmetrics.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfpattern.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfpattern.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/pdfutils.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/pdfutils.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/rl_codecs.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/rl_codecs.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfbase/ttfonts.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfbase/ttfonts.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/canvas.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/canvas.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/pathobject.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/pathobject.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/pdfimages.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/pdfimages.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/pdfgen/textobject.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/pdfgen/textobject.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/doctemplate.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/doctemplate.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/figures.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/figures.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/flowables.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/flowables.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/frames.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/frames.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/multicol.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/multicol.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/para.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/para.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/paragraph.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/paragraph.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/paraparser.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/paraparser.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/tableofcontents.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/tableofcontents.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/tables.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/tables.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,17 @@
     repeatCols: int
     splitByRow: int
     splitInRow: int
     spaceBefore: float
     spaceAfter: float
     def __init__(
         self,
-        data: list[list[Any]] | tuple[tuple[Any, ...], ...],
         # NOTE: Technically only list or tuple works but lack of covariance
         #       on list makes this too annoying
+        data: Sequence[list[Any] | tuple[Any, ...]],
         colWidths: Sequence[float | str | None] | float | str | None = None,
         rowHeights: Sequence[float | None] | float | None = None,
         style: TableStyle | Iterable[_TableCommand] | None = None,
         # docs say list/tuple, but the implementation allows any collection
         repeatRows: int | Collection[int] = 0,
         repeatCols: int | Collection[int] = 0,
         splitByRow: int = 1,
```

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/platypus/xpreformatted.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/platypus/xpreformatted.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/rl_config.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/rl_config.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/reportlab-stubs/rl_settings.pyi` & `types-reportlab-4.2.0.20240530/reportlab-stubs/rl_settings.pyi`

 * *Files identical despite different names*

### Comparing `types-reportlab-4.2.0.20240525/setup.py` & `types-reportlab-4.2.0.20240530/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-reportlab` aims to provide accurate annotations
 for `reportlab==4.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/reportlab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc33ba67ba25545e0decb5897b3d56b40c88b0b5` and was tested
+This package was generated from typeshed commit `c82d29fc7614a9ecd33bd416386062ba2915850d` and was tested
 with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="4.2.0.20240525",
+      version="4.2.0.20240530",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/reportlab.md",
```

### Comparing `types-reportlab-4.2.0.20240525/types_reportlab.egg-info/PKG-INFO` & `types-reportlab-4.2.0.20240530/types_reportlab.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-reportlab
-Version: 4.2.0.20240525
+Version: 4.2.0.20240530
 Summary: Typing stubs for reportlab
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/reportlab.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-reportlab` aims to provide accurate annotations
 for `reportlab==4.2.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/reportlab. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `fc33ba67ba25545e0decb5897b3d56b40c88b0b5` and was tested
+This package was generated from typeshed commit `c82d29fc7614a9ecd33bd416386062ba2915850d` and was tested
 with mypy 1.10.0, pyright 1.1.364, and
 pytype 2024.4.11.
```

### Comparing `types-reportlab-4.2.0.20240525/types_reportlab.egg-info/SOURCES.txt` & `types-reportlab-4.2.0.20240530/types_reportlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

