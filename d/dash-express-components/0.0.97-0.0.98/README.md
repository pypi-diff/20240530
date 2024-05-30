# Comparing `tmp/dash_express_components-0.0.97.tar.gz` & `tmp/dash_express_components-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_express_components-0.0.97.tar", last modified: Fri May 17 06:27:24 2024, max compression
+gzip compressed data, was "dash_express_components-0.0.98.tar", last modified: Thu May 30 13:10:53 2024, max compression
```

## Comparing `dash_express_components-0.0.97.tar` & `dash_express_components-0.0.98.tar`

### file list

```diff
@@ -1,114 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.888142 dash_express_components-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-17 06:27:24.888142 dash_express_components-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.880142 dash_express_components-0.0.97/dash_express_components/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/AggrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/AsType.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Bar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/BarCount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/BinTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Box.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/CategoryLookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/CombinecatTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/ConfigReceiver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/CoreGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/DropnaTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/EvalTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/FilterIqrTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components/Graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/GroupedSample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/HistogramLine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Localstore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/MeltTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/MetaCheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Parameterize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Plotter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/PlotterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/RenameTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/ScatterMatrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/StrSplitTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/SubComponentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/Violin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/WideToLong.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/ZerosToNanTransform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/_imports_.py
--rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-05-17 06:27:21.000000 dash_express_components-0.0.97/dash_express_components/async-excel.js
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-17 06:27:21.000000 dash_express_components-0.0.97/dash_express_components/async-excel.js.map
--rw-r--r--   0 runner    (1001) docker     (127)   711576 2024-05-17 06:27:21.000000 dash_express_components-0.0.97/dash_express_components/dash_express_components.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-17 06:27:21.000000 dash_express_components-0.0.97/dash_express_components/dash_express_components.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    91991 2024-05-17 06:27:23.000000 dash_express_components-0.0.97/dash_express_components/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/package-info.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.884142 dash_express_components-0.0.97/dash_express_components/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.884142 dash_express_components-0.0.97/dash_express_components/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-17 06:27:22.000000 dash_express_components-0.0.97/dash_express_components/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.880142 dash_express_components-0.0.97/dash_express_components.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-17 06:27:24.000000 dash_express_components-0.0.97/dash_express_components.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.884142 dash_express_components-0.0.97/dash_express_components_base/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.884142 dash_express_components-0.0.97/dash_express_components_base/plottypes/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_bar_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_box.py
--rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_histogram_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_imshow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/plottypes/_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 06:27:24.888142 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_aggr.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_asType.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_bin.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_catlookup.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_combinecat.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_dropna.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_groupby_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_iqrfilter.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_melt.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_strsplit.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_wide_to_long.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_zerostonan.py
--rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/dash_express_components_base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/package.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 06:27:24.888142 dash_express_components-0.0.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-17 06:26:17.000000 dash_express_components-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.310763 dash_express_components-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/AggrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/AsType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Bar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/BarCount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/BinTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CategoryLookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CombinecatTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ConfigReceiver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/CoreGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/DropnaTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/EvalTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/FilterIqrTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/GroupedSample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/HistogramLine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Localstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/MeltTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/MetaCheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Parameterize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Plotter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/PlotterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/RenameTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/RequestStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ScatterMatrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/StrSplitTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/SubComponentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/Violin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/WideToLong.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/ZerosToNanTransform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/_imports_.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1163624 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/async-excel.js
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/async-excel.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)   722247 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    95280 2024-05-30 13:10:51.000000 dash_express_components-0.0.98/dash_express_components/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/package-info.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.302763 dash_express_components-0.0.98/dash_express_components/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-30 13:10:50.000000 dash_express_components-0.0.98/dash_express_components/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.298763 dash_express_components-0.0.98/dash_express_components.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-30 13:10:53.000000 dash_express_components-0.0.98/dash_express_components.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 13:10:52.000000 dash_express_components-0.0.98/dash_express_components.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.302763 dash_express_components-0.0.98/dash_express_components_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/dash_express_components_base/plottypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_bar_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4121 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_histogram_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_imshow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/plottypes/_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 13:10:53.306763 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_aggr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_asType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_bin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_catlookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_combinecat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_dropna.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_groupby_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_iqrfilter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_melt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_strsplit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_wide_to_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_zerostonan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25545 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/dash_express_components_base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 13:10:53.310763 dash_express_components-0.0.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-30 13:09:34.000000 dash_express_components-0.0.98/setup.py
```

### Comparing `dash_express_components-0.0.97/PKG-INFO` & `dash_express_components-0.0.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash_express_components
-Version: 0.0.97
+Version: 0.0.98
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.97/README.md` & `dash_express_components-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/AggrTransform.py` & `dash_express_components-0.0.98/dash_express_components/AggrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/AsType.py` & `dash_express_components-0.0.98/dash_express_components/AsType.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Bar.py` & `dash_express_components-0.0.98/dash_express_components/Bar.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/BarCount.py` & `dash_express_components-0.0.98/dash_express_components/BarCount.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Base.py` & `dash_express_components-0.0.98/dash_express_components/Base.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/BinTransform.py` & `dash_express_components-0.0.98/dash_express_components/BinTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Box.py` & `dash_express_components-0.0.98/dash_express_components/Box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/CategoryLookup.py` & `dash_express_components-0.0.98/dash_express_components/CategoryLookup.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/CombinecatTransform.py` & `dash_express_components-0.0.98/dash_express_components/CombinecatTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/ConfigReceiver.py` & `dash_express_components-0.0.98/dash_express_components/ConfigReceiver.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Configurator.py` & `dash_express_components-0.0.98/dash_express_components/Configurator.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/CoreGraph.py` & `dash_express_components-0.0.98/dash_express_components/CoreGraph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/DropnaTransform.py` & `dash_express_components-0.0.98/dash_express_components/DropnaTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/EvalTransform.py` & `dash_express_components-0.0.98/dash_express_components/EvalTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Filter.py` & `dash_express_components-0.0.98/dash_express_components/Filter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/FilterIqrTransform.py` & `dash_express_components-0.0.98/dash_express_components/FilterIqrTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Graph.py` & `dash_express_components-0.0.98/dash_express_components/Graph.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/GroupedSample.py` & `dash_express_components-0.0.98/dash_express_components/GroupedSample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/HistogramLine.py` & `dash_express_components-0.0.98/dash_express_components/HistogramLine.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Imshow.py` & `dash_express_components-0.0.98/dash_express_components/Imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Localstore.py` & `dash_express_components-0.0.98/dash_express_components/Localstore.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/MeltTransform.py` & `dash_express_components-0.0.98/dash_express_components/MeltTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/MetaCheck.py` & `dash_express_components-0.0.98/dash_express_components/MetaCheck.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Parameterize.py` & `dash_express_components-0.0.98/dash_express_components/Parameterize.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Plotter.py` & `dash_express_components-0.0.98/dash_express_components/Plotter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/PlotterBase.py` & `dash_express_components-0.0.98/dash_express_components/PlotterBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Probability.py` & `dash_express_components-0.0.98/dash_express_components/Probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/RenameTransform.py` & `dash_express_components-0.0.98/dash_express_components/RenameTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Scatter.py` & `dash_express_components-0.0.98/dash_express_components/Scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/ScatterMatrix.py` & `dash_express_components-0.0.98/dash_express_components/ScatterMatrix.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/StrSplitTransform.py` & `dash_express_components-0.0.98/dash_express_components/StrSplitTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/SubComponentBase.py` & `dash_express_components-0.0.98/dash_express_components/SubComponentBase.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Table.py` & `dash_express_components-0.0.98/dash_express_components/Table.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Transform.py` & `dash_express_components-0.0.98/dash_express_components/Transform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/Violin.py` & `dash_express_components-0.0.98/dash_express_components/Violin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/WideToLong.py` & `dash_express_components-0.0.98/dash_express_components/WideToLong.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/ZerosToNanTransform.py` & `dash_express_components-0.0.98/dash_express_components/ZerosToNanTransform.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/__init__.py` & `dash_express_components-0.0.98/dash_express_components/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/_imports_.py` & `dash_express_components-0.0.98/dash_express_components/_imports_.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from .Configurator import Configurator
 from .Filter import Filter
 from .Graph import Graph
 from .Localstore import Localstore
 from .MetaCheck import MetaCheck
 from .Parameterize import Parameterize
 from .Plotter import Plotter
+from .RequestStore import RequestStore
 from .Transform import Transform
 from .CoreGraph import CoreGraph
 from .Bar import Bar
 from .BarCount import BarCount
 from .Box import Box
 from .HistogramLine import HistogramLine
 from .Imshow import Imshow
@@ -41,14 +42,15 @@
     "Configurator",
     "Filter",
     "Graph",
     "Localstore",
     "MetaCheck",
     "Parameterize",
     "Plotter",
+    "RequestStore",
     "Transform",
     "CoreGraph",
     "Bar",
     "BarCount",
     "Box",
     "HistogramLine",
     "Imshow",
```

### Comparing `dash_express_components-0.0.97/dash_express_components/async-excel.js` & `dash_express_components-0.0.98/dash_express_components/async-excel.js`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/dash_express_components.min.js` & `dash_express_components-0.0.98/dash_express_components/dash_express_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -113,15 +113,15 @@
             var t = function(e) {
                     return /\/_dash-component-suites\//.test(e.src)
                 }(l()),
                 n = c(e);
             if (!t) return n;
             var r = n.split("/"),
                 a = r.slice(-1)[0].split(".");
-            return a.splice(1, 0, "v0_0_97m1715927224"), r.splice(-1, 1, a.join(".")), r.join("/")
+            return a.splice(1, 0, "v0_0_98m1717074633"), r.splice(-1, 1, a.join(".")), r.join("/")
         }
     }
     var u = window.webpackJsonpdash_express_components = window.webpackJsonpdash_express_components || [],
         s = u.push.bind(u);
     u.push = t, u = u.slice();
     for (var f = 0; f < u.length; f++) t(u[f]);
     var p = s;
@@ -283,17 +283,17 @@
     })), n.d(t, "getYearRange", (function() {
         return z
     })), n.d(t, "getMonthStart", (function() {
         return T
     })), n.d(t, "getPreviousMonthStart", (function() {
         return N
     })), n.d(t, "getNextMonthStart", (function() {
-        return H
-    })), n.d(t, "getMonthEnd", (function() {
         return I
+    })), n.d(t, "getMonthEnd", (function() {
+        return H
     })), n.d(t, "getPreviousMonthEnd", (function() {
         return L
     })), n.d(t, "getNextMonthEnd", (function() {
         return B
     })), n.d(t, "getMonthRange", (function() {
         return q
     })), n.d(t, "getDayStart", (function() {
@@ -368,19 +368,19 @@
     function T(e) {
         var t = i(e),
             n = l(e),
             r = new Date;
         return r.setFullYear(t, n, 1), r.setHours(0, 0, 0, 0), r
     }
     var N = D(T, -1),
-        H = D(T, 1),
-        I = a(H),
-        L = D(I, -1),
-        B = D(I, 1),
-        q = o([T, I]);
+        I = D(T, 1),
+        H = a(I),
+        L = D(H, -1),
+        B = D(H, 1),
+        q = o([T, H]);
 
     function F(e, t) {
         return function(n) {
             var r = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : t,
                 a = i(n),
                 o = l(n),
                 c = u(n) + r,
@@ -400,15 +400,15 @@
         U = F(W, 1),
         K = a(U),
         Y = F(K, -1),
         Q = F(K, 1),
         G = o([W, K]);
 
     function J(e) {
-        return u(I(e))
+        return u(H(e))
     }
 
     function Z(e) {
         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 2,
             n = "".concat(e);
         return n.length >= t ? e : "0000".concat(n).slice(-t)
     }
@@ -994,15 +994,15 @@
             return a
         }.apply(t, [])) || (e.exports = r)
     }()
 }, function(e, t, n) {
     "use strict";
     var r = n(8),
         a = n(9);
-    var o = n(28);
+    var o = n(29);
 
     function i(e) {
         return (i = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -1090,21 +1090,21 @@
     n.d(t, "a", (function() {
         return R
     })), n.d(t, "b", (function() {
         return B
     })), n.d(t, "c", (function() {
         return L
     })), n.d(t, "d", (function() {
-        return I
+        return H
     })), n.d(t, "e", (function() {
         return w
     })), n.d(t, "f", (function() {
         return Ne
     })), n.d(t, "g", (function() {
-        return H
+        return I
     })), n.d(t, "h", (function() {
         return M
     })), n.d(t, "i", (function() {
         return E
     })), n.d(t, "j", (function() {
         return A
     })), n.d(t, "k", (function() {
@@ -1250,19 +1250,19 @@
                 return z = !0
             }
         },
         T = "undefined" != typeof window ? window : {};
     T.addEventListener && T.removeEventListener && (T.addEventListener("p", O, D), T.removeEventListener("p", O, !1));
     var N = z;
 
-    function H(e) {
+    function I(e) {
         return null != e
     }
 
-    function I(e, t, n) {
+    function H(e, t, n) {
         return e ? t : n
     }
 
     function L(e) {
         return e
     }
 
@@ -2394,15 +2394,15 @@
                 }
                 return o
             }
         }(e, t) || o(e, t) || function() {
             throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
         }()
     }
-    var l = n(28),
+    var l = n(29),
         c = n(0),
         u = n.n(c),
         s = ["defaultInputValue", "defaultMenuIsOpen", "defaultValue", "inputValue", "menuIsOpen", "onChange", "onInputChange", "onMenuClose", "onMenuOpen", "value"];
     var f = n(8),
         p = n(33),
         d = n(34),
         h = n(35);
@@ -2904,22 +2904,22 @@
                 opacity: 0,
                 position: "relative",
                 transform: "scale(.01)"
             }, "", "")
         }))
     }
     var N = ["boxSizing", "height", "overflow", "paddingRight", "position"],
-        H = {
+        I = {
             boxSizing: "border-box",
             overflow: "hidden",
             position: "relative",
             height: "100%"
         };
 
-    function I(e) {
+    function H(e) {
         e.preventDefault()
     }
 
     function L(e) {
         e.stopPropagation()
     }
 
@@ -3029,30 +3029,30 @@
                             if (r && N.forEach((function(e) {
                                     var t = n && n[e];
                                     a.current[e] = t
                                 })), r && W < 1) {
                                 var o = parseInt(a.current.paddingRight, 10) || 0,
                                     i = document.body ? document.body.clientWidth : 0,
                                     l = window.innerWidth - i + o || 0;
-                                Object.keys(H).forEach((function(e) {
-                                    var t = H[e];
+                                Object.keys(I).forEach((function(e) {
+                                    var t = I[e];
                                     n && (n[e] = t)
                                 })), n && (n.paddingRight = "".concat(l, "px"))
                             }
-                            t && q() && (t.addEventListener("touchmove", I, V), e && (e.addEventListener("touchstart", B, V), e.addEventListener("touchmove", L, V))), W += 1
+                            t && q() && (t.addEventListener("touchmove", H, V), e && (e.addEventListener("touchstart", B, V), e.addEventListener("touchmove", L, V))), W += 1
                         }
                     }), [r]),
                     l = Object(c.useCallback)((function(e) {
                         if (F) {
                             var t = document.body,
                                 n = t && t.style;
                             W = Math.max(W - 1, 0), r && W < 1 && N.forEach((function(e) {
                                 var t = a.current[e];
                                 n && (n[e] = t)
-                            })), t && q() && (t.removeEventListener("touchmove", I, V), e && (e.removeEventListener("touchstart", B, V), e.removeEventListener("touchmove", L, V)))
+                            })), t && q() && (t.removeEventListener("touchmove", H, V), e && (e.removeEventListener("touchstart", B, V), e.removeEventListener("touchmove", L, V)))
                         }
                     }), [r]);
                 return Object(c.useEffect)((function() {
                         if (t) {
                             var e = o.current;
                             return i(e),
                                 function() {
@@ -4302,26 +4302,26 @@
                 }
             }]), n
         }(c.Component);
     ue.defaultProps = Z;
     var se = n(18),
         fe = n(48),
         pe = (n(121), n(125), n(127), n(131), n(132), n(133), n(15), u.a.forwardRef((function(e, t) {
-            var n, a, o, p, d, h, m, b, v, y, g, O, _, w, E, j, M, k, P, x, S, A, C, R, z, D, T, N, H, I, L, B = (a = (n = e).defaultInputValue, o = void 0 === a ? "" : a, p = n.defaultMenuIsOpen, d = void 0 !== p && p, h = n.defaultValue, m = void 0 === h ? null : h, b = n.inputValue, v = n.menuIsOpen, y = n.onChange, g = n.onInputChange, O = n.onMenuClose, _ = n.onMenuOpen, w = n.value, E = Object(l.a)(n, s), j = i(Object(c.useState)(void 0 !== b ? b : o), 2), M = j[0], k = j[1], P = i(Object(c.useState)(void 0 !== v ? v : d), 2), x = P[0], S = P[1], A = i(Object(c.useState)(void 0 !== w ? w : m), 2), C = A[0], R = A[1], z = Object(c.useCallback)((function(e, t) {
+            var n, a, o, p, d, h, m, b, v, y, g, O, _, w, E, j, M, k, P, x, S, A, C, R, z, D, T, N, I, H, L, B = (a = (n = e).defaultInputValue, o = void 0 === a ? "" : a, p = n.defaultMenuIsOpen, d = void 0 !== p && p, h = n.defaultValue, m = void 0 === h ? null : h, b = n.inputValue, v = n.menuIsOpen, y = n.onChange, g = n.onInputChange, O = n.onMenuClose, _ = n.onMenuOpen, w = n.value, E = Object(l.a)(n, s), j = i(Object(c.useState)(void 0 !== b ? b : o), 2), M = j[0], k = j[1], P = i(Object(c.useState)(void 0 !== v ? v : d), 2), x = P[0], S = P[1], A = i(Object(c.useState)(void 0 !== w ? w : m), 2), C = A[0], R = A[1], z = Object(c.useCallback)((function(e, t) {
                 "function" == typeof y && y(e, t), R(e)
             }), [y]), D = Object(c.useCallback)((function(e, t) {
                 var n;
                 "function" == typeof g && (n = g(e, t)), k(void 0 !== n ? n : e)
             }), [g]), T = Object(c.useCallback)((function() {
                 "function" == typeof _ && _(), S(!0)
             }), [_]), N = Object(c.useCallback)((function() {
                 "function" == typeof O && O(), S(!1)
-            }), [O]), H = void 0 !== b ? b : M, I = void 0 !== v ? v : x, L = void 0 !== w ? w : C, Object(r.n)(Object(r.n)({}, E), {}, {
-                inputValue: H,
-                menuIsOpen: I,
+            }), [O]), I = void 0 !== b ? b : M, H = void 0 !== v ? v : x, L = void 0 !== w ? w : C, Object(r.n)(Object(r.n)({}, E), {}, {
+                inputValue: I,
+                menuIsOpen: H,
                 onChange: z,
                 onInputChange: D,
                 onMenuClose: N,
                 onMenuOpen: T,
                 value: L
             }));
             return u.a.createElement(ue, Object(f.a)({
@@ -4516,16 +4516,16 @@
             restoreFocus: M = !0,
             restoreFocusOptions: k,
             renderDialog: P,
             renderBackdrop: R = (e => Object(A.jsx)("div", Object.assign({}, e))),
             manager: D,
             container: T,
             onShow: N,
-            onHide: H = (() => {}),
-            onExit: I,
+            onHide: I = (() => {}),
+            onExit: H,
             onExited: L,
             onExiting: B,
             onEnter: q,
             onEntering: F,
             onEntered: W
         } = e, V = function(e, t) {
             if (null == e) return {};
@@ -4573,18 +4573,18 @@
         });
         const ee = Object(p.a)(() => {
                 if (!j || !Y() || !K.isTopModal()) return;
                 const e = v();
                 K.dialog && e && !y(K.dialog, e) && K.dialog.focus()
             }),
             te = Object(p.a)(e => {
-                e.target === e.currentTarget && (null == s || s(e), !0 === c && H())
+                e.target === e.currentTarget && (null == s || s(e), !0 === c && I())
             }),
             ne = Object(p.a)(e => {
-                u && 27 === e.keyCode && K.isTopModal() && (null == f || f(e), e.defaultPrevented || H())
+                u && 27 === e.keyCode && K.isTopModal() && (null == f || f(e), e.defaultPrevented || I())
             }),
             re = Object(h.useRef)(),
             ae = Object(h.useRef)(),
             oe = (...e) => {
                 J(!0), null == L || L(...e)
             },
             ie = d;
@@ -4603,15 +4603,15 @@
                 role: "document"
             })
         }));
         ie && (ce = Object(A.jsx)(ie, {
             appear: !0,
             unmountOnExit: !0,
             in: !!n,
-            onExit: I,
+            onExit: H,
             onExiting: B,
             onExited: oe,
             onEnter: q,
             onEntering: F,
             onEntered: W,
             children: ce
         }));
@@ -4635,19 +4635,19 @@
     });
     D.displayName = "Modal";
     var T = Object.assign(D, {
         Manager: k
     });
     var N = Function.prototype.bind.call(Function.prototype.call, [].slice);
 
-    function H(e, t) {
+    function I(e, t) {
         return N(e.querySelectorAll(t))
     }
 
-    function I(e, t) {
+    function H(e, t) {
         return e.replace(new RegExp("(^|\\s)" + t + "(?:\\s|$)", "g"), "$1").replace(/\s+/g, " ").replace(/^\s*|\s*$/g, "")
     }
     const L = ".fixed-top, .fixed-bottom, .is-fixed, .sticky-top",
         B = ".sticky-top",
         q = ".navbar-toggler";
     class F extends k {
         adjustAndStore(e, t, n) {
@@ -4667,24 +4667,24 @@
             const t = this.getElement();
             var n, r;
             if (r = "modal-open", (n = t).classList ? n.classList.add(r) : function(e, t) {
                     return e.classList ? !!t && e.classList.contains(t) : -1 !== (" " + (e.className.baseVal || e.className) + " ").indexOf(" " + t + " ")
                 }(n, r) || ("string" == typeof n.className ? n.className = n.className + " " + r : n.setAttribute("class", (n.className && n.className.baseVal || "") + " " + r)), !e.scrollBarWidth) return;
             const a = this.isRTL ? "paddingLeft" : "paddingRight",
                 o = this.isRTL ? "marginLeft" : "marginRight";
-            H(t, L).forEach(t => this.adjustAndStore(a, t, e.scrollBarWidth)), H(t, B).forEach(t => this.adjustAndStore(o, t, -e.scrollBarWidth)), H(t, q).forEach(t => this.adjustAndStore(o, t, e.scrollBarWidth))
+            I(t, L).forEach(t => this.adjustAndStore(a, t, e.scrollBarWidth)), I(t, B).forEach(t => this.adjustAndStore(o, t, -e.scrollBarWidth)), I(t, q).forEach(t => this.adjustAndStore(o, t, e.scrollBarWidth))
         }
         removeContainerStyle(e) {
             super.removeContainerStyle(e);
             const t = this.getElement();
             var n, r;
-            r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = I(n.className, r) : n.setAttribute("class", I(n.className && n.className.baseVal || "", r));
+            r = "modal-open", (n = t).classList ? n.classList.remove(r) : "string" == typeof n.className ? n.className = H(n.className, r) : n.setAttribute("class", H(n.className && n.className.baseVal || "", r));
             const a = this.isRTL ? "paddingLeft" : "paddingRight",
                 o = this.isRTL ? "marginLeft" : "marginRight";
-            H(t, L).forEach(e => this.restore(a, e)), H(t, B).forEach(e => this.restore(o, e)), H(t, q).forEach(e => this.restore(o, e))
+            I(t, L).forEach(e => this.restore(a, e)), I(t, B).forEach(e => this.restore(o, e)), I(t, q).forEach(e => this.restore(o, e))
         }
     }
     let W;
     var V = n(39),
         U = n(22),
         K = Object(U.a)("modal-body");
     var Y = h.createContext({
@@ -4808,16 +4808,16 @@
         autoFocus: x,
         enforceFocus: S,
         restoreFocus: C,
         restoreFocusOptions: R,
         onEntered: z,
         onExit: D,
         onExiting: N,
-        onEnter: H,
-        onEntering: I,
+        onEnter: I,
+        onEntering: H,
         onExited: L,
         backdropClassName: B,
         manager: q,
         ...V
     }, U) => {
         const [K, G] = Object(h.useState)({}), [J, Z] = Object(h.useState)(!1), X = Object(h.useRef)(!1), $ = Object(h.useRef)(!1), ee = Object(h.useRef)(null), [te, ne] = Object(f.a)(), re = Object(d.a)(U, ne), ae = Object(p.a)(k), oe = Object(Q.b)();
         e = Object(Q.a)(e, "modal");
@@ -4886,18 +4886,18 @@
                 restoreFocusOptions: R,
                 onEscapeKeyDown: e => {
                     E || "static" !== w ? E && j && j(e) : (e.preventDefault(), he())
                 },
                 onShow: M,
                 onHide: k,
                 onEnter: (e, t) => {
-                    e && (e.style.display = "block", se(e)), null == H || H(e, t)
+                    e && (e.style.display = "block", se(e)), null == I || I(e, t)
                 },
                 onEntering: (e, t) => {
-                    null == I || I(e, t), Object(i.a)(window, "resize", fe)
+                    null == H || H(e, t), Object(i.a)(window, "resize", fe)
                 },
                 onEntered: z,
                 onExit: e => {
                     null == ee.current || ee.current(), null == D || D(e)
                 },
                 onExiting: N,
                 onExited: e => {
@@ -5366,31 +5366,31 @@
         children: [n, Object(p.jsx)("label", {
             htmlFor: r,
             children: o
         })]
     })));
     T.displayName = "FloatingLabel";
     var N = T;
-    const H = {
+    const I = {
             _ref: i.a.any,
             validated: i.a.bool,
             as: i.a.elementType
         },
-        I = l.forwardRef(({
+        H = l.forwardRef(({
             className: e,
             validated: t,
             as: n = "form",
             ...r
         }, o) => Object(p.jsx)(n, {
             ...r,
             ref: o,
             className: a()(e, t && "was-validated")
         }));
-    I.displayName = "Form", I.propTypes = H;
-    t.a = Object.assign(I, {
+    H.displayName = "Form", H.propTypes = I;
+    t.a = Object.assign(H, {
         Group: _,
         Control: v.a,
         Floating: g,
         Check: b,
         Switch: D,
         Label: k,
         Text: R,
@@ -5745,15 +5745,15 @@
         onEntering: b,
         onEntered: b,
         onExit: b,
         onExiting: b,
         onExited: b
     }, m.UNMOUNTED = "unmounted", m.EXITED = f, m.ENTERING = p, m.ENTERED = d, m.EXITING = h;
     t.e = m
-}, function(e, t) {
+}, , function(e, t) {
     e.exports = function(e) {
         var t = {};
 
         function n(r) {
             if (t[r]) return t[r].exports;
             var a = t[r] = {
                 i: r,
@@ -6149,60 +6149,60 @@
             }(e.key) : t.toString(36)
         }
 
         function N(e, t) {
             e.func.call(e.context, t, e.count++)
         }
 
-        function H(e, t, n) {
+        function I(e, t, n) {
             var r = e.result,
                 a = e.keyPrefix;
-            e = e.func.call(e.context, t, e.count++), Array.isArray(e) ? I(e, r, n, (function(e) {
+            e = e.func.call(e.context, t, e.count++), Array.isArray(e) ? H(e, r, n, (function(e) {
                 return e
             })) : null != e && (S(e) && (e = function(e, t) {
                 return {
                     $$typeof: o,
                     type: e.type,
                     key: t,
                     ref: e.ref,
                     props: e.props,
                     _owner: e._owner
                 }
             }(e, a + (!e.key || t && t.key === e.key ? "" : ("" + e.key).replace(A, "$&/") + "/") + n)), r.push(e))
         }
 
-        function I(e, t, n, r, a) {
+        function H(e, t, n, r, a) {
             var o = "";
-            null != n && (o = ("" + n).replace(A, "$&/") + "/"), D(e, H, t = R(t, o, r, a)), z(t)
+            null != n && (o = ("" + n).replace(A, "$&/") + "/"), D(e, I, t = R(t, o, r, a)), z(t)
         }
 
         function L() {
             var e = j.current;
             if (null === e) throw Error(v(321));
             return e
         }
         var B = {
                 Children: {
                     map: function(e, t, n) {
                         if (null == e) return e;
                         var r = [];
-                        return I(e, r, null, t, n), r
+                        return H(e, r, null, t, n), r
                     },
                     forEach: function(e, t, n) {
                         if (null == e) return e;
                         D(e, N, t = R(null, null, t, n)), z(t)
                     },
                     count: function(e) {
                         return D(e, (function() {
                             return null
                         }), null)
                     },
                     toArray: function(e) {
                         var t = [];
-                        return I(e, t, null, (function(e) {
+                        return H(e, t, null, (function(e) {
                             return e
                         })), t
                     },
                     only: function(e) {
                         if (!S(e)) throw Error(v(143));
                         return e
                     }
@@ -6426,15 +6426,15 @@
         var n, a, o = Object(r.a)(e, t);
         if (Object.getOwnPropertySymbols) {
             var i = Object.getOwnPropertySymbols(e);
             for (a = 0; a < i.length; a++) n = i[a], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (o[n] = e[n])
         }
         return o
     }
-}, , function(e, t, n) {
+}, function(e, t, n) {
     "use strict";
 
     function r(e, t) {
         if (null == e) return {};
         var n, r, a = {},
             o = Object.keys(e);
         for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
@@ -6712,34 +6712,34 @@
                     u[0] = d + 1 / 3, u[1] = d, u[2] = d - 1 / 3;
                     for (var h = 0; h < 3; h++) u[h] < 0 && (u[h] += 1), u[h] > 1 && (u[h] -= 1), 6 * u[h] < 1 ? s[h] = p + 6 * (f - p) * u[h] : 2 * u[h] < 1 ? s[h] = f : 3 * u[h] < 2 ? s[h] = p + (f - p) * (2 / 3 - u[h]) * 6 : s[h] = p;
                     r = (e = [D(255 * s[0]), D(255 * s[1]), D(255 * s[2])])[0], a = e[1], o = e[2]
                 }
                 return t.length > 3 ? [r, a, o, t[3]] : [r, a, o, 1]
             },
             N = /^rgb\(\s*(-?\d+),\s*(-?\d+)\s*,\s*(-?\d+)\s*\)$/,
-            H = /^rgba\(\s*(-?\d+),\s*(-?\d+)\s*,\s*(-?\d+)\s*,\s*([01]|[01]?\.\d+)\)$/,
-            I = /^rgb\(\s*(-?\d+(?:\.\d+)?)%,\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*\)$/,
+            I = /^rgba\(\s*(-?\d+),\s*(-?\d+)\s*,\s*(-?\d+)\s*,\s*([01]|[01]?\.\d+)\)$/,
+            H = /^rgb\(\s*(-?\d+(?:\.\d+)?)%,\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*\)$/,
             L = /^rgba\(\s*(-?\d+(?:\.\d+)?)%,\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*,\s*([01]|[01]?\.\d+)\)$/,
             B = /^hsl\(\s*(-?\d+(?:\.\d+)?),\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*\)$/,
             q = /^hsla\(\s*(-?\d+(?:\.\d+)?),\s*(-?\d+(?:\.\d+)?)%\s*,\s*(-?\d+(?:\.\d+)?)%\s*,\s*([01]|[01]?\.\d+)\)$/,
             F = Math.round,
             W = function(e) {
                 var t;
                 if (e = e.toLowerCase().trim(), c.format.named) try {
                     return c.format.named(e)
                 } catch (e) {}
                 if (t = e.match(N)) {
                     for (var n = t.slice(1, 4), r = 0; r < 3; r++) n[r] = +n[r];
                     return n[3] = 1, n
                 }
-                if (t = e.match(H)) {
+                if (t = e.match(I)) {
                     for (var a = t.slice(1, 5), o = 0; o < 4; o++) a[o] = +a[o];
                     return a
                 }
-                if (t = e.match(I)) {
+                if (t = e.match(H)) {
                     for (var i = t.slice(1, 4), l = 0; l < 3; l++) i[l] = F(2.55 * i[l]);
                     return i[3] = 1, i
                 }
                 if (t = e.match(L)) {
                     for (var u = t.slice(1, 5), s = 0; s < 3; s++) u[s] = F(2.55 * u[s]);
                     return u[3] = +u[3], u
                 }
@@ -6753,15 +6753,15 @@
                     var d = t.slice(1, 4);
                     d[1] *= .01, d[2] *= .01;
                     var h = T(d);
                     return h[3] = +t[4], h
                 }
             };
         W.test = function(e) {
-            return N.test(e) || H.test(e) || I.test(e) || L.test(e) || B.test(e) || q.test(e)
+            return N.test(e) || I.test(e) || H.test(e) || L.test(e) || B.test(e) || q.test(e)
         };
         var V = W,
             U = l.type;
         d.prototype.css = function(e) {
             return R(this._rgb, e)
         }, m.css = function() {
             for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
@@ -7026,25 +7026,25 @@
                 if (e = Ce(e, "hsv"), "array" === Re(e) && 3 === e.length) return "hsv"
             }
         });
         var ze = 18,
             De = .95047,
             Te = 1,
             Ne = 1.08883,
-            He = .137931034,
-            Ie = .206896552,
+            Ie = .137931034,
+            He = .206896552,
             Le = .12841855,
             Be = .008856452,
             qe = l.unpack,
             Fe = Math.pow,
             We = function(e) {
                 return (e /= 255) <= .04045 ? e / 12.92 : Fe((e + .055) / 1.055, 2.4)
             },
             Ve = function(e) {
-                return e > Be ? Fe(e, 1 / 3) : e / Le + He
+                return e > Be ? Fe(e, 1 / 3) : e / Le + Ie
             },
             Ue = function(e, t, n) {
                 return e = We(e), t = We(t), n = We(n), [Ve((.4124564 * e + .3575761 * t + .1804375 * n) / De), Ve((.2126729 * e + .7151522 * t + .072175 * n) / Te), Ve((.0193339 * e + .119192 * t + .9503041 * n) / Ne)]
             },
             Ke = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n = qe(e, "rgb"),
@@ -7060,15 +7060,15 @@
             },
             Ye = l.unpack,
             Qe = Math.pow,
             Ge = function(e) {
                 return 255 * (e <= .00304 ? 12.92 * e : 1.055 * Qe(e, 1 / 2.4) - .055)
             },
             Je = function(e) {
-                return e > Ie ? e * e * e : Le * (e - He)
+                return e > He ? e * e * e : Le * (e - Ie)
             },
             Ze = function() {
                 for (var e = [], t = arguments.length; t--;) e[t] = arguments[t];
                 var n, r, a, o = (e = Ye(e, "lab"))[0],
                     i = e[1],
                     l = e[2];
                 return r = (o + 16) / 116, n = isNaN(i) ? r : r + i / 500, a = isNaN(l) ? r : r - l / 200, r = Te * Je(r), n = De * Je(n), a = Ne * Je(a), [Ge(3.2404542 * n - 1.5371385 * r - .4985314 * a), Ge(-.969266 * n + 1.8760108 * r + .041556 * a), Ge(.0556434 * n - .2040259 * r + 1.0572252 * a), e.length > 3 ? e[3] : 1]
@@ -7450,20 +7450,20 @@
                         var o = t.interpolate(a, .5, "rgb"),
                             i = o.luminance();
                         return Math.abs(e - i) < 1e-7 || !n-- ? o : i > e ? r(t, o) : r(o, a)
                     },
                     a = (t > e ? r(new d([0, 0, 0]), this) : r(this, new d([255, 255, 255]))).rgb();
                 return new d(a.concat([this._rgb[3]]))
             }
-            return Ht.apply(void 0, this._rgb.slice(0, 3))
+            return It.apply(void 0, this._rgb.slice(0, 3))
         };
-        var Ht = function(e, t, n) {
-                return .2126 * (e = It(e)) + .7152 * (t = It(t)) + .0722 * (n = It(n))
+        var It = function(e, t, n) {
+                return .2126 * (e = Ht(e)) + .7152 * (t = Ht(t)) + .0722 * (n = Ht(n))
             },
-            It = function(e) {
+            Ht = function(e) {
                 return (e /= 255) <= .03928 ? e / 12.92 : Nt((e + .055) / 1.055, 2.4)
             },
             Lt = {},
             Bt = l.type,
             qt = function(e, t, n) {
                 void 0 === n && (n = .5);
                 for (var r = [], a = arguments.length - 3; a-- > 0;) r[a] = arguments[a + 3];
@@ -7885,16 +7885,16 @@
                         O = !1;
                         for (var T = 0; T < n; T++)
                             if (C[T] !== w[T]) {
                                 O = !0;
                                 break
                             } w = C, ++_ > 200 && (O = !1)
                     }
-                    for (var N = {}, H = 0; H < n; H++) N[H] = [];
-                    for (var I = 0; I < v; I++) N[b = y[I]].push(i[I]);
+                    for (var N = {}, I = 0; I < n; I++) N[I] = [];
+                    for (var H = 0; H < v; H++) N[b = y[H]].push(i[H]);
                     for (var L = [], B = 0; B < n; B++) L.push(N[B][0]), L.push(N[B][N[B].length - 1]);
                     L = L.sort((function(e, t) {
                         return e - t
                     })), l.push(L[0]);
                     for (var q = 1; q < L.length; q += 2) {
                         var F = L[q];
                         isNaN(F) || -1 !== l.indexOf(F) || l.push(F)
@@ -8839,19 +8839,19 @@
             case 41:
             case 93:
                 return 1
         }
         return 0
     }
 
-    function H(e) {
+    function I(e) {
         return E = j = 1, M = g(x = e), k = 0, []
     }
 
-    function I(e) {
+    function H(e) {
         return x = "", e
     }
 
     function L(e) {
         return h(T(k - 1, function e(t) {
             for (; R();) switch (P) {
                 case t:
@@ -8888,15 +8888,15 @@
 
     function W(e) {
         for (; !N(z());) R();
         return T(e, k)
     }
 
     function V(e) {
-        return I(function e(t, n, r, a, o, i, l, c, u) {
+        return H(function e(t, n, r, a, o, i, l, c, u) {
             var s = 0,
                 f = 0,
                 d = l,
                 h = 0,
                 v = 0,
                 y = 0,
                 O = 1,
@@ -8984,15 +8984,15 @@
                             45 === z() && (S += L(R())), h = z(), f = d = g(M = S += W(D())), j++;
                             break;
                         case 45:
                             45 === y && 2 == g(S) && (O = 0)
                     }
             }
             return i
-        }("", null, null, null, [""], e = H(e), 0, [0], e))
+        }("", null, null, null, [""], e = I(e), 0, [0], e))
     }
 
     function U(e, t, n, r, a, o, i, l, u, s, p) {
         for (var d = a - 1, b = 0 === a ? o : [""], v = O(b), g = 0, _ = 0, w = 0; g < r; ++g)
             for (var E = 0, j = y(e, d + 1, d = f(_ = i[g])), M = e; E < v; ++E)(M = h(_ > 0 ? b[E] + " " + j : m(j, /&\f/g, b[E]))) && (u[w++] = M);
         return S(e, t, n, 0 === a ? c : l, u, s, p)
     }
@@ -9146,15 +9146,15 @@
     }
     n(47), n(73);
     var X = function(e, t, n) {
             for (var r = 0, a = 0; r = a, a = z(), 38 === r && 12 === a && (t[n] = 1), !N(a);) R();
             return T(e, k)
         },
         $ = function(e, t) {
-            return I(function(e, t) {
+            return H(function(e, t) {
                 var n = -1,
                     r = 44;
                 do {
                     switch (N(r)) {
                         case 0:
                             38 === r && 12 === z() && (t[n] = 1), e[n] += X(k - 1, t, n);
                             break;
@@ -9167,15 +9167,15 @@
                                 break
                             }
                         default:
                             e[n] += p(r)
                     }
                 } while (r = R());
                 return e
-            }(H(e), t))
+            }(I(e), t))
         },
         ee = new WeakMap,
         te = function(e) {
             if ("rule" === e.type && e.parent && !(e.length < 1)) {
                 for (var t = e.value, n = e.parent, r = e.column === n.column && e.line === n.line;
                     "rule" !== n.type;)
                     if (!(n = n.parent)) return;
@@ -9534,15 +9534,15 @@
         prop_types__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(1),
         prop_types__WEBPACK_IMPORTED_MODULE_2___default = __webpack_require__.n(prop_types__WEBPACK_IMPORTED_MODULE_2__),
         react_bootstrap_InputGroup__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(5),
         react_bootstrap_Button__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(14),
         react_bootstrap_Form__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(19),
         react_bootstrap_FormControl__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(13),
         react_bootstrap_Modal__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(12),
-        react_list_editable__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__(27),
+        react_list_editable__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__(28),
         react_list_editable__WEBPACK_IMPORTED_MODULE_8___default = __webpack_require__.n(react_list_editable__WEBPACK_IMPORTED_MODULE_8__),
         react_bootstrap_Alert__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__(24),
         react_select__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__(10);
 
     function _extends() {
         return (_extends = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
@@ -11795,16 +11795,16 @@
                         S = e.secondAriaLabel,
                         A = e.secondPlaceholder,
                         R = e.showLeadingZeros,
                         z = e.value,
                         D = e.yearAriaLabel,
                         T = e.yearPlaceholder,
                         N = this.state,
-                        H = N.isCalendarOpen,
-                        I = N.isClockOpen,
+                        I = N.isCalendarOpen,
+                        H = N.isClockOpen,
                         L = O([].concat(z), 1)[0],
                         B = {
                             amPmAriaLabel: t,
                             dayAriaLabel: c,
                             hourAriaLabel: h,
                             minuteAriaLabel: w,
                             monthAriaLabel: j,
@@ -11823,15 +11823,15 @@
                     return a.default.createElement("div", {
                         className: "".concat(C, "__wrapper")
                     }, a.default.createElement(f.default, g({}, B, q, {
                         autoFocus: n,
                         className: "".concat(C, "__inputGroup"),
                         disabled: p,
                         format: d,
-                        isWidgetOpen: H || I,
+                        isWidgetOpen: I || H,
                         locale: b,
                         maxDate: v,
                         maxDetail: y,
                         minDate: _,
                         name: k,
                         onChange: this.onChange,
                         placeholder: this.placeholder,
@@ -11964,15 +11964,15 @@
         clearIcon: N,
         closeWidgets: !0,
         isCalendarOpen: null,
         isClockOpen: null,
         maxDetail: "minute",
         openWidgetsOnFocus: !0
     };
-    var H = o.default.oneOfType([o.default.string, o.default.instanceOf(Date)]);
+    var I = o.default.oneOfType([o.default.string, o.default.instanceOf(Date)]);
     z.propTypes = {
         amPmAriaLabel: o.default.string,
         autoFocus: o.default.bool,
         calendarAriaLabel: o.default.string,
         calendarClassName: o.default.oneOfType([o.default.string, o.default.arrayOf(o.default.string)]),
         calendarIcon: o.default.node,
         className: o.default.oneOfType([o.default.string, o.default.arrayOf(o.default.string)]),
@@ -12007,15 +12007,15 @@
         onClockOpen: o.default.func,
         onFocus: o.default.func,
         openWidgetsOnFocus: o.default.bool,
         required: o.default.bool,
         secondAriaLabel: o.default.string,
         secondPlaceholder: o.default.string,
         showLeadingZeros: o.default.bool,
-        value: o.default.oneOfType([H, o.default.arrayOf(H)]),
+        value: o.default.oneOfType([I, o.default.arrayOf(I)]),
         yearAriaLabel: o.default.string,
         yearPlaceholder: o.default.string
     }
 }, function(e, t, n) {
     "use strict";
     n.r(t), n.d(t, "clipboardEvents", (function() {
         return r
@@ -12261,17 +12261,17 @@
     }
 
     function N(e, t) {
         (null == t || t > e.length) && (t = e.length);
         for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
         return r
     }
-    var H = new Date;
-    H.setFullYear(1, 0, 1), H.setHours(0, 0, 0, 0);
-    var I = new Date(864e13),
+    var I = new Date;
+    I.setFullYear(1, 0, 1), I.setHours(0, 0, 0, 0);
+    var H = new Date(864e13),
         L = ["hour", "minute", "second"];
 
     function B(e, t) {
         return e && !t || !e && t || e && t && e.getTime() !== t.getTime()
     }
 
     function q(e, t, n, r) {
@@ -12727,16 +12727,16 @@
                     r = e.isWidgetOpen,
                     a = e.maxDate,
                     o = e.minDate,
                     i = e.required;
                 return {
                     className: t,
                     disabled: n,
-                    maxDate: a || I,
-                    minDate: o || H,
+                    maxDate: a || H,
+                    minDate: o || I,
                     onChange: this.onChange,
                     onKeyDown: this.onKeyDown,
                     onKeyUp: this.onKeyUp,
                     placeholder: "--",
                     required: i || r
                 }
             }
@@ -12800,16 +12800,16 @@
                     i = e.nativeInputAriaLabel,
                     l = e.required,
                     c = this.state.value;
                 return a.default.createElement(v.default, {
                     key: "time",
                     ariaLabel: i,
                     disabled: t,
-                    maxDate: n || I,
-                    minDate: r || H,
+                    maxDate: n || H,
+                    minDate: r || I,
                     name: o,
                     onChange: this.onChangeNative,
                     required: l,
                     value: c,
                     valueType: this.valueType
                 })
             }
@@ -14305,15 +14305,15 @@
                 ...o,
                 className: i()(n, t)
             })
         })
     });
     T.displayName = "AccordionItem";
     var N = T;
-    const H = r.forwardRef((e, t) => {
+    const I = r.forwardRef((e, t) => {
         const {
             as: n = "div",
             activeKey: a,
             bsPrefix: o,
             className: u,
             onSelect: s,
             flush: f,
@@ -14329,16 +14329,16 @@
             children: Object(m.jsx)(n, {
                 ref: t,
                 ...p,
                 className: i()(u, d, f && d + "-flush")
             })
         })
     });
-    H.displayName = "Accordion";
-    var I = Object.assign(H, {
+    I.displayName = "Accordion";
+    var H = Object.assign(I, {
             Button: C,
             Collapse: M,
             Item: N,
             Header: D,
             Body: S
         }),
         L = n(12),
@@ -15392,18 +15392,18 @@
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
-    var He = n(87);
+    var Ie = n(87);
 
-    function Ie(e) {
-        return (Ie = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function He(e) {
+        return (He = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function Le(e, t) {
@@ -15469,15 +15469,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return Ue(this, n)
         }
     }
 
     function Ue(e, t) {
-        if (t && ("object" === Ie(t) || "function" == typeof t)) return t;
+        if (t && ("object" === He(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -15563,29 +15563,29 @@
                         log10: Math.log10,
                         log1p: Math.log1p,
                         expm1: Math.expm1,
                         sqrt: Math.sqrt
                     }, Object.keys(t).reduce((function(e, n) {
                         return "numerical" === t[n].type && (e[o.fix_variable_name(n)] = t[n].median), "bool" === t[n].type && (e[o.fix_variable_name(n)] = !0), "categorical" === t[n].type && (e[o.fix_variable_name(n)] = t[n].cat[0]), "temporal" === t[n].type && (e[o.fix_variable_name(n)] = new Date(t[n].median)), e
                     }), {}));
-                    a = Object(He.a)("return " + n.replaceAll("@", "at_").replaceAll("&", "&&"))(u)
+                    a = Object(Ie.a)("return " + n.replaceAll("@", "at_").replaceAll("&", "&&"))(u)
                 } catch (e) {
                     i = !0, l = e.message
                 }
                 if (!i) {
                     if (String(a).indexOf(":") >= 0) try {
                         var s = new Date(a);
                         s.getTime() == s.getTime() && (c = "temporal")
                     } catch (e) {}
                     "temporal" !== c && (c = {
                         number: "numerical",
                         boolean: "bool",
                         string: "categorical",
                         undefined: "?"
-                    } [String(Ie(a))])
+                    } [String(He(a))])
                 }
                 "?" === c && (i = !0, l = "Evaluation error!"), "numerical" === c && isNaN(a) && (i = !0, l = "Evaluation error!");
                 var f = {
                         value: a,
                         error: i,
                         message: l,
                         type: c
@@ -16114,15 +16114,15 @@
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
-    var bt = n(27),
+    var bt = n(28),
         vt = n.n(bt);
 
     function yt(e) {
         return (yt = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
@@ -16440,17 +16440,17 @@
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
                 return !1
             }
         }();
         return function() {
-            var n, r = Ht(e);
+            var n, r = It(e);
             if (t) {
-                var a = Ht(this).constructor;
+                var a = It(this).constructor;
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return Nt(this, n)
         }
     }
 
     function Nt(e, t) {
@@ -16458,28 +16458,28 @@
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
-    function Ht(e) {
-        return (Ht = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+    function It(e) {
+        return (It = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
     Pt.defaultProps = {}, Pt.propTypes = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
-    var It = function(e) {
+    var Ht = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             Object.defineProperty(e, "prototype", {
                 value: Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
@@ -16671,15 +16671,15 @@
     }
 
     function Jt(e) {
         return (Jt = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
             return e.__proto__ || Object.getPrototypeOf(e)
         })(e)
     }
-    It.defaultProps = {}, It.propTypes = {
+    Ht.defaultProps = {}, Ht.propTypes = {
         config: PropTypes.any,
         meta: PropTypes.any.isRequired,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
     };
@@ -17695,31 +17695,31 @@
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function Hn(e, t) {
+    function In(e, t) {
         var n = Object.keys(e);
         if (Object.getOwnPropertySymbols) {
             var r = Object.getOwnPropertySymbols(e);
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function In(e) {
+    function Hn(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
-            t % 2 ? Hn(Object(n), !0).forEach((function(t) {
+            t % 2 ? In(Object(n), !0).forEach((function(t) {
                 Ln(e, t, n[t])
-            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Hn(Object(n)).forEach((function(t) {
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : In(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
     function Ln(e, t, n) {
@@ -17803,22 +17803,22 @@
         }(o, e);
         var t, n, r, a = Fn(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-            }(this, o), (t = a.call(this, e)).state = In(In({}, t.state), {}, {
+            }(this, o), (t = a.call(this, e)).state = Hn(Hn({}, t.state), {}, {
                 cols: [],
                 name: "",
                 binning: [],
                 binning_string: "[]",
                 overlapping: !1,
                 parse_error: !1
-            }), "config" in e && (t.state = In(In({}, t.state), {}, {
+            }), "config" in e && (t.state = Hn(Hn({}, t.state), {}, {
                 cols: "cols" in e.config ? e.config.cols : [],
                 name: "name" in e.config ? e.config.name : "",
                 binning: "binning" in e.config ? e.config.binning : [],
                 binning_string: "binning" in e.config ? JSON.stringify(e.config.binning) : "[]",
                 overlapping: "overlapping" in e.config && e.config.overlapping
             })), t
         }
@@ -17839,15 +17839,15 @@
                         value: "",
                         error: !1,
                         message: "",
                         type: "categorical"
                     };
                 if (0 == r.length) return i.error = !0, i.message = "Please enter some bins", i;
                 var l = "min" in r[0],
-                    c = In({}, t);
+                    c = Hn({}, t);
                 if (o) l && n.length > 1 ? n.forEach((function(e) {
                     return r.forEach((function(t) {
                         c[e + "_" + a + "_" + t.name] = {
                             type: "bool"
                         }
                     }))
                 })) : r.forEach((function(e) {
@@ -17916,15 +17916,15 @@
                     className: "color-helper-green"
                 }, "Select the columns to bin:"), React.createElement(J.a, Nn({
                     className: "mb-3",
                     options: l,
                     styles: U.d,
                     components: U.b
                 }, Object(U.c)(this, (function(t) {
-                    return e.setStateConfig(In(In({}, t), {}, {
+                    return e.setStateConfig(Hn(Hn({}, t), {}, {
                         name: n,
                         binning: a,
                         overlapping: i
                     }))
                 }), "cols", c))), React.createElement(Q.a, {
                     className: "mb-3"
                 }, React.createElement(Q.a.Text, {
@@ -19263,27 +19263,27 @@
         d: "M42.598 4.763h13.229v2.646H42.598zM42.598 7.673h13.229v2.646H42.598zM42.598 10.583h13.229v2.646H42.598zM42.598 13.494h13.229v2.646H42.598zM42.598 16.404h13.229v2.646H42.598zM42.598 19.315h13.229v2.646H42.598zM42.598 22.225h13.229v2.646H42.598z"
     }), a.a.createElement("path", {
         d: "M57.755 13.078h4.914v.983h-4.914z"
     }), a.a.createElement("path", {
         d: "M60.703 11.113v4.914h-.983v-4.914z"
     })));
 
-    function Hr() {
-        return (Hr = Object.assign || function(e) {
+    function Ir() {
+        return (Ir = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
-    var Ir = ({
+    var Hr = ({
         styles: e = {},
         ...t
-    }) => a.a.createElement("svg", Hr({
+    }) => a.a.createElement("svg", Ir({
         xmlns: "http://www.w3.org/2000/svg",
         width: "300",
         height: "100",
         viewBox: "0 0 79.375 26.458"
     }, t), a.a.createElement("path", {
         d: "M36.43 11.88h4.473L39.2 10.179h1.413l2.28 2.222-2.28 2.222h-1.413l1.702-1.703H36.43z",
         "aria-label": "➔",
@@ -21014,17 +21014,17 @@
         type: "catlookup",
         class: Pt,
         label: "Apply a lookup on a categorical column",
         svg: a.a.createElement(Nr, null)
     }, {
         group: "missing",
         type: "dropna",
-        class: It,
+        class: Ht,
         label: "Remove rows with nan values",
-        svg: a.a.createElement(Ir, null)
+        svg: a.a.createElement(Hr, null)
     }, {
         group: "missing",
         type: "zerostonan",
         class: un,
         label: "Replace zero values with nan values",
         svg: a.a.createElement(Fr, null)
     }, {
@@ -21332,15 +21332,15 @@
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    var Ha = function(e) {
+    var Ia = function(e) {
         ! function(e, t) {
             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
             Object.defineProperty(e, "prototype", {
                 value: Object.create(t && t.prototype, {
                     constructor: {
                         value: e,
                         writable: !0,
@@ -22087,16 +22087,16 @@
                 })))
             }
         }]) && Ca(t.prototype, n), r && Ca(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
     }(r.Component);
 
-    function Ia(e) {
-        return (Ia = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function Ha(e) {
+        return (Ha = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
 
     function La(e, t) {
@@ -22153,15 +22153,15 @@
                 n = Reflect.construct(r, arguments, a)
             } else n = r.apply(this, arguments);
             return Va(this, n)
         }
     }
 
     function Va(e, t) {
-        if (t && ("object" === Ia(t) || "function" == typeof t)) return t;
+        if (t && ("object" === Ha(t) || "function" == typeof t)) return t;
         if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
         return function(e) {
             if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
             return e
         }(e)
     }
 
@@ -22175,22 +22175,22 @@
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
-    Na(Ha, "icon", React.createElement("svg", {
+    Na(Ia, "icon", React.createElement("svg", {
         fill: "currentColor",
         preserveAspectRatio: "xMidYMid meet",
         viewBox: "0 0 46 46"
     }, React.createElement("path", {
         fill: "none",
         d: "M0 0h46v46H0z"
-    }))), Na(Ha, "label", "Empty plot"), Na(Ha, "type", "base"), Ha.defaultProps = {}, Ha.propTypes = {
+    }))), Na(Ia, "label", "Empty plot"), Na(Ia, "type", "base"), Ia.defaultProps = {}, Ia.propTypes = {
         id: PropTypes.string,
         config: PropTypes.any,
         allColOptions: PropTypes.any.isRequired,
         catColOptions: PropTypes.any.isRequired,
         numColOptions: PropTypes.any.isRequired,
         numOptions: PropTypes.any.isRequired,
         setProps: PropTypes.func
@@ -22239,15 +22239,15 @@
                     r = e.numColOptions,
                     a = e.optionsbar;
                 return React.createElement("div", null, this.multiSelect("X", "x", t), this.multiSelect("Y", "y", t), this.singleSelect("Color", "color", t), this.singleSelect("Symb.", "symbol", n), this.singleSelect("Size", "size", r), this.optionsBar(a), this.commonOptionBarControlls())
             }
         }]) && qa(t.prototype, n), r && qa(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function Qa(e) {
         return (Qa = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -22491,15 +22491,15 @@
                 })).map((function(t) {
                     if ("boxoptions" === t.id) return React.createElement("div", null, React.createElement("h5", null, t.label), e.singleSelect_ExtraOption("Mode", "boxmode", e.boxmode_options), e.singleSelect_ExtraOption("Points", "points", e.points_options), e.multiSelect_ExtraOption("Stats", "aggr", e.aggr_options), e.multiSelect("Lines", "lines", r))
                 })))
             }
         }]) && Za(t.prototype, n), r && Za(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function ao(e) {
         return (ao = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -22693,15 +22693,15 @@
                 })).map((function(t) {
                     if ("boxoptions" === t.id) return React.createElement("div", null, React.createElement("h5", null, t.label), e.singleSelect_ExtraOption("Points", "points", e.points_options))
                 })))
             }
         }]) && lo(t.prototype, n), r && lo(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function mo(e) {
         return (mo = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -22851,15 +22851,15 @@
                 return React.createElement("div", {
                     key: "div-" + this.props.id
                 }, this.singleSelect("X", "x", n), this.singleSelect("Y", "y", n), this.multiSelect("Dim", "dimensions", t), this.optionsBar(r), this.commonOptionBarControlls())
             }
         }]) && yo(t.prototype, n), r && yo(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function Mo(e) {
         return (Mo = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -23037,15 +23037,15 @@
                     id: "extra-box-options",
                     className: "w-100 mb-1"
                 }, this.toggleSelect("Text", "text_auto", [null, !0])), this.optionsBar(r), this.commonOptionBarControlls())
             }
         }]) && xo(t.prototype, n), r && xo(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function To(e) {
         return (To = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -23058,27 +23058,27 @@
             t && (r = r.filter((function(t) {
                 return Object.getOwnPropertyDescriptor(e, t).enumerable
             }))), n.push.apply(n, r)
         }
         return n
     }
 
-    function Ho(e) {
+    function Io(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? No(Object(n), !0).forEach((function(t) {
                 Wo(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : No(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function Io(e, t) {
+    function Ho(e, t) {
         for (var n = 0; n < t.length; n++) {
             var r = t[n];
             r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
         }
     }
 
     function Lo(e, t) {
@@ -23170,40 +23170,40 @@
         }(o, e);
         var t, n, r, a = Bo(o);
 
         function o(e) {
             var t;
             return function(e, t) {
                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-            }(this, o), (t = a.call(this, e)).state = Ho(Ho({}, t.state), {}, {
+            }(this, o), (t = a.call(this, e)).state = Io(Io({}, t.state), {}, {
                 optionsbar: [t.option_dict.facet, t.option_dict.axis, t.option_dict.render]
             }), t.copy_params("bar_count"), t.init_check_options(!0), t
         }
         return t = o, (n = [{
             key: "config_from_state",
             value: function(e) {
-                var t = Ho(Ho({}, this.base_config_from_state()), e);
+                var t = Io(Io({}, this.base_config_from_state()), e);
                 return "hover_data" in (t = this.preferSimple(t)) && "string" == typeof t.hover_data && (t.hover_data = [t.hover_data]), {
                     type: "bar_count",
                     params: t
                 }
             }
         }, {
             key: "render",
             value: function() {
                 var e = this.state,
                     t = e.allColOptions,
                     n = e.catColOptions,
                     r = e.optionsbar;
                 return React.createElement("div", null, this.multiSelect("X", "x", n), this.singleSelect("Color", "color", t), this.optionsBar(r), this.commonOptionBarControlls())
             }
-        }]) && Io(t.prototype, n), r && Io(t, r), Object.defineProperty(t, "prototype", {
+        }]) && Ho(t.prototype, n), r && Ho(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function Uo(e) {
         return (Uo = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -23374,15 +23374,15 @@
                     r = e.numColOptions,
                     a = e.optionsbar;
                 return React.createElement("div", null, this.multiSelect("Dim", "dimensions", t), this.singleSelect("Color", "color", t), this.singleSelect("Symb.", "symbol", n), this.singleSelect("Size", "size", r), this.optionsBar(a), this.commonOptionBarControlls())
             }
         }]) && Qo(t.prototype, n), r && Qo(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function ti(e) {
         return (ti = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -23663,15 +23663,15 @@
                     id: "extra-hist-options",
                     className: "w-100 mb-1"
                 }, this.toggleSelect("Cumulative", "cumulative", [null, !0])), this.optionsBar(r), this.commonOptionBarControlls())
             }
         }]) && ai(t.prototype, n), r && ai(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function fi(e) {
         return (fi = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -23827,15 +23827,15 @@
                     id: "show-fit-option",
                     className: "w-100 mb-1"
                 }, this.toggleSelect("Linear fit", "trendline", [null, "ols"])), this.optionsBar(r), this.commonOptionBarControlls())
             }
         }]) && hi(t.prototype, n), r && hi(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function _i(e) {
         return (_i = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -24081,15 +24081,15 @@
             value: function() {
                 var e = this.state.allColOptions;
                 return React.createElement("div", null, this.multiSelect("Dim", "dimensions", e))
             }
         }]) && ji(t.prototype, n), r && ji(t, r), Object.defineProperty(t, "prototype", {
             writable: !1
         }), o
-    }(Ha);
+    }(Ia);
 
     function Ci(e) {
         return (Ci = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
@@ -24136,21 +24136,21 @@
     }
 
     function Ni(e, t) {
         for (; !Object.prototype.hasOwnProperty.call(e, t) && null !== (e = Bi(e)););
         return e
     }
 
-    function Hi(e, t) {
-        return (Hi = Object.setPrototypeOf || function(e, t) {
+    function Ii(e, t) {
+        return (Ii = Object.setPrototypeOf || function(e, t) {
             return e.__proto__ = t, e
         })(e, t)
     }
 
-    function Ii(e) {
+    function Hi(e) {
         var t = function() {
             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
             if (Reflect.construct.sham) return !1;
             if ("function" == typeof Proxy) return !0;
             try {
                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
             } catch (e) {
@@ -24304,17 +24304,17 @@
                         constructor: {
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
                     }),
                     writable: !1
-                }), t && Hi(e, t)
+                }), t && Ii(e, t)
             }(i, e);
-            var t, n, r, o = Ii(i);
+            var t, n, r, o = Hi(i);
 
             function i(e) {
                 var t;
                 return function(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }(this, i), (t = o.call(this, {}, e)).state = zi(zi({}, t.state), {}, {
                     showModal: !1,
@@ -25003,15 +25003,15 @@
                         i = n.showEditModal,
                         l = n.eventGraphId,
                         c = this.state,
                         u = c.config,
                         s = c.config_filter,
                         f = c.config_transform,
                         p = c.config_plot;
-                    return React.createElement(I, {
+                    return React.createElement(H, {
                         id: t,
                         key: t,
                         defaultActiveKey: "plotter"
                     }, this.props.showFilter && React.createElement(Ol, {
                         title: "Filter"
                     }, React.createElement(me, {
                         id: "".concat(t, "-filter"),
@@ -25273,32 +25273,32 @@
     };
     var Cl = n(15),
         Rl = n.n(Cl),
         zl = n(88),
         Dl = n.n(zl),
         Tl = n(89),
         Nl = n.n(Tl),
-        Hl = function(e, t) {
-            return (Hl = Object.setPrototypeOf || {
+        Il = function(e, t) {
+            return (Il = Object.setPrototypeOf || {
                     __proto__: []
                 }
                 instanceof Array && function(e, t) {
                     e.__proto__ = t
                 } || function(e, t) {
                     for (var n in t) Object.prototype.hasOwnProperty.call(t, n) && (e[n] = t[n])
                 })(e, t)
         };
 
-    function Il(e, t) {
+    function Hl(e, t) {
         if ("function" != typeof t && null !== t) throw new TypeError("Class extends value " + String(t) + " is not a constructor or null");
 
         function n() {
             this.constructor = e
         }
-        Hl(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
+        Il(e, t), e.prototype = null === t ? Object.create(t) : (n.prototype = t.prototype, new n)
     }
 
     function Ll(e, t) {
         var n = {};
         for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
         if (null != e && "function" == typeof Object.getOwnPropertySymbols) {
             var a = 0;
@@ -25401,15 +25401,15 @@
                     l = void 0 === i ? 1e3 : i,
                     c = t.refreshOptions;
                 return n.state = {
                     width: void 0,
                     height: void 0
                 }, n.skipOnMount = a, n.targetRef = Object(r.createRef)(), n.observableElement = null, Fl() || (n.resizeHandler = Bl(n.createResizeHandler, o, l, c), n.resizeObserver = new window.ResizeObserver(n.resizeHandler)), n
             }
-            return Il(t, e), t.prototype.componentDidMount = function() {
+            return Hl(t, e), t.prototype.componentDidMount = function() {
                 this.attachObserver()
             }, t.prototype.componentDidUpdate = function() {
                 this.attachObserver()
             }, t.prototype.componentWillUnmount = function() {
                 Fl() || (this.resizeObserver.disconnect(), this.cancelHandler())
             }, t.prototype.render = function() {
                 var e, t = this.props,
@@ -26862,15 +26862,534 @@
     Sc.propTypes = {
         id: V.a.string.isRequired,
         token: V.a.string.isRequired,
         config: V.a.any,
         setProps: V.a.func
     };
     var Ac = Sc;
-    n.d(t, "Configurator", (function() {
+
+    function Cc(e) {
+        return null != e && "object" == typeof e && !0 === e["@@functional/placeholder"]
+    }
+
+    function Rc(e) {
+        return function t(n) {
+            return 0 === arguments.length || Cc(n) ? t : e.apply(this, arguments)
+        }
+    }
+    var zc = Rc((function(e) {
+        return null == e
+    }));
+
+    function Dc(e) {
+        return function t(n, r) {
+            switch (arguments.length) {
+                case 0:
+                    return t;
+                case 1:
+                    return Cc(n) ? t : Rc((function(t) {
+                        return e(n, t)
+                    }));
+                default:
+                    return Cc(n) && Cc(r) ? t : Cc(n) ? Rc((function(t) {
+                        return e(t, r)
+                    })) : Cc(r) ? Rc((function(t) {
+                        return e(n, t)
+                    })) : e(n, r)
+            }
+        }
+    }
+
+    function Tc(e) {
+        for (var t, n = []; !(t = e.next()).done;) n.push(t.value);
+        return n
+    }
+
+    function Nc(e, t, n) {
+        for (var r = 0, a = n.length; r < a;) {
+            if (e(t, n[r])) return !0;
+            r += 1
+        }
+        return !1
+    }
+
+    function Ic(e, t) {
+        return Object.prototype.hasOwnProperty.call(t, e)
+    }
+    var Hc = "function" == typeof Object.is ? Object.is : function(e, t) {
+            return e === t ? 0 !== e || 1 / e == 1 / t : e != e && t != t
+        },
+        Lc = Object.prototype.toString,
+        Bc = function() {
+            return "[object Arguments]" === Lc.call(arguments) ? function(e) {
+                return "[object Arguments]" === Lc.call(e)
+            } : function(e) {
+                return Ic("callee", e)
+            }
+        }(),
+        qc = !{
+            toString: null
+        }.propertyIsEnumerable("toString"),
+        Fc = ["constructor", "valueOf", "isPrototypeOf", "toString", "propertyIsEnumerable", "hasOwnProperty", "toLocaleString"],
+        Wc = function() {
+            return arguments.propertyIsEnumerable("length")
+        }(),
+        Vc = function(e, t) {
+            for (var n = 0; n < e.length;) {
+                if (e[n] === t) return !0;
+                n += 1
+            }
+            return !1
+        },
+        Uc = "function" != typeof Object.keys || Wc ? Rc((function(e) {
+            if (Object(e) !== e) return [];
+            var t, n, r = [],
+                a = Wc && Bc(e);
+            for (t in e) !Ic(t, e) || a && "length" === t || (r[r.length] = t);
+            if (qc)
+                for (n = Fc.length - 1; n >= 0;) Ic(t = Fc[n], e) && !Vc(r, t) && (r[r.length] = t), n -= 1;
+            return r
+        })) : Rc((function(e) {
+            return Object(e) !== e ? [] : Object.keys(e)
+        })),
+        Kc = Rc((function(e) {
+            return null === e ? "Null" : void 0 === e ? "Undefined" : Object.prototype.toString.call(e).slice(8, -1)
+        }));
+
+    function Yc(e, t, n, r) {
+        var a = Tc(e);
+
+        function o(e, t) {
+            return Qc(e, t, n.slice(), r.slice())
+        }
+        return !Nc((function(e, t) {
+            return !Nc(o, t, e)
+        }), Tc(t), a)
+    }
+
+    function Qc(e, t, n, r) {
+        if (Hc(e, t)) return !0;
+        var a, o, i = Kc(e);
+        if (i !== Kc(t)) return !1;
+        if (null == e || null == t) return !1;
+        if ("function" == typeof e["fantasy-land/equals"] || "function" == typeof t["fantasy-land/equals"]) return "function" == typeof e["fantasy-land/equals"] && e["fantasy-land/equals"](t) && "function" == typeof t["fantasy-land/equals"] && t["fantasy-land/equals"](e);
+        if ("function" == typeof e.equals || "function" == typeof t.equals) return "function" == typeof e.equals && e.equals(t) && "function" == typeof t.equals && t.equals(e);
+        switch (i) {
+            case "Arguments":
+            case "Array":
+            case "Object":
+                if ("function" == typeof e.constructor && "Promise" === (a = e.constructor, null == (o = String(a).match(/^function (\w*)/)) ? "" : o[1])) return e === t;
+                break;
+            case "Boolean":
+            case "Number":
+            case "String":
+                if (typeof e != typeof t || !Hc(e.valueOf(), t.valueOf())) return !1;
+                break;
+            case "Date":
+                if (!Hc(e.valueOf(), t.valueOf())) return !1;
+                break;
+            case "Error":
+                return e.name === t.name && e.message === t.message;
+            case "RegExp":
+                if (e.source !== t.source || e.global !== t.global || e.ignoreCase !== t.ignoreCase || e.multiline !== t.multiline || e.sticky !== t.sticky || e.unicode !== t.unicode) return !1
+        }
+        for (var l = n.length - 1; l >= 0;) {
+            if (n[l] === e) return r[l] === t;
+            l -= 1
+        }
+        switch (i) {
+            case "Map":
+                return e.size === t.size && Yc(e.entries(), t.entries(), n.concat([e]), r.concat([t]));
+            case "Set":
+                return e.size === t.size && Yc(e.values(), t.values(), n.concat([e]), r.concat([t]));
+            case "Arguments":
+            case "Array":
+            case "Object":
+            case "Boolean":
+            case "Number":
+            case "String":
+            case "Date":
+            case "Error":
+            case "RegExp":
+            case "Int8Array":
+            case "Uint8Array":
+            case "Uint8ClampedArray":
+            case "Int16Array":
+            case "Uint16Array":
+            case "Int32Array":
+            case "Uint32Array":
+            case "Float32Array":
+            case "Float64Array":
+            case "ArrayBuffer":
+                break;
+            default:
+                return !1
+        }
+        var c = Uc(e);
+        if (c.length !== Uc(t).length) return !1;
+        var u = n.concat([e]),
+            s = r.concat([t]);
+        for (l = c.length - 1; l >= 0;) {
+            var f = c[l];
+            if (!Ic(f, t) || !Qc(t[f], e[f], u, s)) return !1;
+            l -= 1
+        }
+        return !0
+    }
+    var Gc = Dc((function(e, t) {
+        return Qc(e, t, [], [])
+    }));
+
+    function Jc(e) {
+        return (Jc = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+            return typeof e
+        } : function(e) {
+            return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+        })(e)
+    }
+
+    function Zc(e, t) {
+        var n = Object.keys(e);
+        if (Object.getOwnPropertySymbols) {
+            var r = Object.getOwnPropertySymbols(e);
+            t && (r = r.filter((function(t) {
+                return Object.getOwnPropertyDescriptor(e, t).enumerable
+            }))), n.push.apply(n, r)
+        }
+        return n
+    }
+
+    function Xc(e) {
+        for (var t = 1; t < arguments.length; t++) {
+            var n = null != arguments[t] ? arguments[t] : {};
+            t % 2 ? Zc(Object(n), !0).forEach((function(t) {
+                $c(e, t, n[t])
+            })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Zc(Object(n)).forEach((function(t) {
+                Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
+            }))
+        }
+        return e
+    }
+
+    function $c(e, t, n) {
+        return t in e ? Object.defineProperty(e, t, {
+            value: n,
+            enumerable: !0,
+            configurable: !0,
+            writable: !0
+        }) : e[t] = n, e
+    }
+
+    function eu(e, t, n, r, a, o, i) {
+        try {
+            var l = e[o](i),
+                c = l.value
+        } catch (e) {
+            return void n(e)
+        }
+        l.done ? t(c) : Promise.resolve(c).then(r, a)
+    }
+
+    function tu(e, t) {
+        return (tu = Object.setPrototypeOf || function(e, t) {
+            return e.__proto__ = t, e
+        })(e, t)
+    }
+
+    function nu(e) {
+        var t = function() {
+            if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
+            if (Reflect.construct.sham) return !1;
+            if ("function" == typeof Proxy) return !0;
+            try {
+                return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+            } catch (e) {
+                return !1
+            }
+        }();
+        return function() {
+            var n, r = ou(e);
+            if (t) {
+                var a = ou(this).constructor;
+                n = Reflect.construct(r, arguments, a)
+            } else n = r.apply(this, arguments);
+            return ru(this, n)
+        }
+    }
+
+    function ru(e, t) {
+        if (t && ("object" === Jc(t) || "function" == typeof t)) return t;
+        if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
+        return au(e)
+    }
+
+    function au(e) {
+        if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+        return e
+    }
+
+    function ou(e) {
+        return (ou = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+            return e.__proto__ || Object.getPrototypeOf(e)
+        })(e)
+    }
+
+    function iu(e, t) {
+        if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+    }
+
+    function lu(e, t) {
+        for (var n = 0; n < t.length; n++) {
+            var r = t[n];
+            r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
+        }
+    }
+
+    function cu(e, t, n) {
+        return t && lu(e.prototype, t), n && lu(e, n), Object.defineProperty(e, "prototype", {
+            writable: !1
+        }), e
+    }
+    var uu = function() {
+            function e() {
+                iu(this, e), this._data = {}, this._modified = -1
+            }
+            return cu(e, [{
+                key: "getItem",
+                value: function(e) {
+                    return this._data[e]
+                }
+            }, {
+                key: "setItem",
+                value: function(e, t) {
+                    this._data[e] = t, this.setModified(e)
+                }
+            }, {
+                key: "removeItem",
+                value: function(e) {
+                    delete this._data[e], this.setModified(e)
+                }
+            }, {
+                key: "setModified",
+                value: function(e) {
+                    this._modified = Date.now()
+                }
+            }, {
+                key: "getModified",
+                value: function(e) {
+                    return this._modified
+                }
+            }]), e
+        }(),
+        su = function() {
+            function e(t) {
+                iu(this, e), this._storage = t
+            }
+            return cu(e, [{
+                key: "getItem",
+                value: function(e) {
+                    try {
+                        return JSON.parse(this._storage.getItem(e))
+                    } catch (e) {
+                        return null
+                    }
+                }
+            }, {
+                key: "setItem",
+                value: function(e, t) {
+                    this._storage.setItem(e, JSON.stringify(t)), this.setModified(e)
+                }
+            }, {
+                key: "removeItem",
+                value: function(e) {
+                    this._storage.removeItem(e), this._storage.removeItem("".concat(e, "-timestamp"))
+                }
+            }, {
+                key: "setModified",
+                value: function(e) {
+                    this._storage.setItem("".concat(e, "-timestamp"), Date.now())
+                }
+            }, {
+                key: "getModified",
+                value: function(e) {
+                    return Number.parseInt(this._storage.getItem("".concat(e, "-timestamp")), 10) || -1
+                }
+            }]), e
+        }(),
+        fu = function(e) {
+            ! function(e, t) {
+                if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+                Object.defineProperty(e, "prototype", {
+                    value: Object.create(t && t.prototype, {
+                        constructor: {
+                            value: e,
+                            writable: !0,
+                            configurable: !0
+                        }
+                    }),
+                    writable: !1
+                }), t && tu(e, t)
+            }(a, e);
+            var t, n, r = nu(a);
+
+            function a(e) {
+                var t;
+                return iu(this, a), t = r.call(this, e), "local" === e.storage_type ? t._backstore = new su(window.localStorage) : "session" === e.storage_type ? t._backstore = new su(window.sessionStorage) : "memory" === e.storage_type && (t._backstore = new uu), t.onStorageChange = t.onStorageChange.bind(au(t)), t
+            }
+            return cu(a, [{
+                key: "fetchData",
+                value: (t = regeneratorRuntime.mark((function e(t, n) {
+                    var r, a, o, i, l, c = this;
+                    return regeneratorRuntime.wrap((function(e) {
+                        for (;;) switch (e.prev = e.next) {
+                            case 0:
+                                return e.prev = 0, e.next = 3, fetch(t, {
+                                    method: "POST",
+                                    headers: Xc({
+                                        "Content-Type": "application/json"
+                                    }, this.props.longCallback && {
+                                        "X-Longcallback": "true"
+                                    }),
+                                    body: JSON.stringify(n)
+                                });
+                            case 3:
+                                if (202 !== (r = e.sent).status) {
+                                    e.next = 7;
+                                    break
+                                }
+                                return setTimeout((function() {
+                                    c.fetchData(t, n)
+                                }), 1e3), e.abrupt("return");
+                            case 7:
+                                if (r.ok) {
+                                    e.next = 9;
+                                    break
+                                }
+                                throw new Error("Error fetching data: ".concat(r.statusText));
+                            case 9:
+                                return e.next = 11, r.json();
+                            case 11:
+                                a = e.sent, o = this.props, i = o.id, l = o.setProps, this._backstore.setItem(i, a), l({
+                                    data: a,
+                                    modified_timestamp: this._backstore.getModified(i)
+                                }), e.next = 20;
+                                break;
+                            case 17:
+                                e.prev = 17, e.t0 = e.catch(0), console.error("Failed to fetch data:", e.t0);
+                            case 20:
+                            case "end":
+                                return e.stop()
+                        }
+                    }), e, this, [
+                        [0, 17]
+                    ])
+                })), n = function() {
+                    var e = this,
+                        n = arguments;
+                    return new Promise((function(r, a) {
+                        var o = t.apply(e, n);
+
+                        function i(e) {
+                            eu(o, r, a, i, l, "next", e)
+                        }
+
+                        function l(e) {
+                            eu(o, r, a, i, l, "throw", e)
+                        }
+                        i(void 0)
+                    }))
+                }, function(e, t) {
+                    return n.apply(this, arguments)
+                })
+            }, {
+                key: "onStorageChange",
+                value: function(e) {
+                    var t = this.props,
+                        n = t.id,
+                        r = t.setProps;
+                    e.key === n && r && e.newValue !== e.oldValue && r({
+                        data: JSON.parse(e.newValue),
+                        modified_timestamp: this._backstore.getModified(n)
+                    })
+                }
+            }, {
+                key: "UNSAFE_componentWillMount",
+                value: function() {
+                    var e = this.props,
+                        t = e.setProps,
+                        n = e.id,
+                        r = e.data;
+                    "memory" !== e.storage_type && window.addEventListener("storage", this.onStorageChange);
+                    var a = this._backstore.getItem(n);
+                    if (zc(a) && !zc(r)) return this._backstore.setItem(n, r), void t({
+                        modified_timestamp: this._backstore.getModified(n)
+                    });
+                    Gc(a, r) || t({
+                        data: a,
+                        modified_timestamp: this._backstore.getModified(n)
+                    })
+                }
+            }, {
+                key: "componentDidMount",
+                value: function() {
+                    var e = this.props,
+                        t = e.url,
+                        n = e.config;
+                    t && n && this.fetchData(t, n)
+                }
+            }, {
+                key: "componentDidUpdate",
+                value: function(e) {
+                    var t = this.props,
+                        n = t.data,
+                        r = t.id,
+                        a = t.clear_data,
+                        o = t.setProps,
+                        i = t.url,
+                        l = t.config;
+                    if (a) return this._backstore.removeItem(r), void o({
+                        clear_data: !1,
+                        data: null,
+                        modified_timestamp: this._backstore.getModified(r)
+                    });
+                    var c = this._backstore.getItem(r);
+                    Gc(n, c) || (void 0 === n ? o({
+                        data: c
+                    }) : (this._backstore.setItem(r, n), o({
+                        modified_timestamp: this._backstore.getModified(r)
+                    }))), i === e.url && Gc(l, e.config) || i && l && this.fetchData(i, l)
+                }
+            }, {
+                key: "componentWillUnmount",
+                value: function() {
+                    "memory" !== this.props.storage_type && window.removeEventListener("storage", this.onStorageChange)
+                }
+            }, {
+                key: "render",
+                value: function() {
+                    return null
+                }
+            }]), a
+        }(a.a.Component);
+    fu.defaultProps = {
+        storage_type: "memory",
+        clear_data: !1,
+        modified_timestamp: -1,
+        longCallback: !1
+    }, fu.propTypes = {
+        id: V.a.string.isRequired,
+        storage_type: V.a.oneOf(["local", "session", "memory"]),
+        data: V.a.oneOfType([V.a.object, V.a.array, V.a.number, V.a.string, V.a.bool]),
+        clear_data: V.a.bool,
+        modified_timestamp: V.a.number,
+        setProps: V.a.func,
+        url: V.a.string,
+        config: V.a.object,
+        longCallback: V.a.bool
+    }, n.d(t, "Configurator", (function() {
         return wl
     })), n.d(t, "Filter", (function() {
         return me
     })), n.d(t, "Transform", (function() {
         return ma
     })), n.d(t, "Plotter", (function() {
         return Yi
@@ -26880,14 +27399,16 @@
         return wc
     })), n.d(t, "MetaCheck", (function() {
         return Ea
     })), n.d(t, "Localstore", (function() {
         return il
     })), n.d(t, "ConfigReceiver", (function() {
         return Ac
+    })), n.d(t, "RequestStore", (function() {
+        return fu
     }))
 }, function(e, t, n) {
     "use strict";
     n.r(t);
     var r, a = n(0),
         o = n.n(a),
         i = n(1),
@@ -27083,53 +27604,53 @@
         })).join(" – ")
     }
 
     function N(e, t, n) {
         return T(e, t, Object(s.getDecadeRange)(n))
     }
 
-    function H(e) {
+    function I(e) {
         var t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : h.ISO_8601,
             n = e.getDay();
         switch (t) {
             case h.ARABIC:
             case h.HEBREW:
                 return n === k || n === P;
             case h.ISO_8601:
             case h.US:
                 return n === P || n === M;
             default:
                 throw new Error("Unsupported calendar type.")
         }
     }
 
-    function I(e) {
-        return (I = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+    function H(e) {
+        return (H = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
             return typeof e
         } : function(e) {
             return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
         })(e)
     }
     var L = Object.values(h),
         B = ["century", "decade", "year", "month"],
         q = l.a.oneOf(L),
         F = l.a.oneOfType([l.a.string, l.a.arrayOf(l.a.string)]),
         W = function(e, t, n) {
             var r = e[t];
             if (!r) return null;
-            if (!(r instanceof Date)) return new Error("Invalid prop `".concat(t, "` of type `").concat(I(r), "` supplied to `").concat(n, "`, expected instance of `Date`."));
+            if (!(r instanceof Date)) return new Error("Invalid prop `".concat(t, "` of type `").concat(H(r), "` supplied to `").concat(n, "`, expected instance of `Date`."));
             var a = e.maxDate;
-            return a && r > a ? new Error("Invalid prop `".concat(t, "` of type `").concat(I(r), "` supplied to `").concat(n, "`, minDate cannot be larger than maxDate.")) : null
+            return a && r > a ? new Error("Invalid prop `".concat(t, "` of type `").concat(H(r), "` supplied to `").concat(n, "`, minDate cannot be larger than maxDate.")) : null
         },
         V = function(e, t, n) {
             var r = e[t];
             if (!r) return null;
-            if (!(r instanceof Date)) return new Error("Invalid prop `".concat(t, "` of type `").concat(I(r), "` supplied to `").concat(n, "`, expected instance of `Date`."));
+            if (!(r instanceof Date)) return new Error("Invalid prop `".concat(t, "` of type `").concat(H(r), "` supplied to `").concat(n, "`, expected instance of `Date`."));
             var a = e.minDate;
-            return a && r < a ? new Error("Invalid prop `".concat(t, "` of type `").concat(I(r), "` supplied to `").concat(n, "`, maxDate cannot be smaller than minDate.")) : null
+            return a && r < a ? new Error("Invalid prop `".concat(t, "` of type `").concat(H(r), "` supplied to `").concat(n, "`, maxDate cannot be smaller than minDate.")) : null
         },
         U = l.a.oneOfType([l.a.func, l.a.shape({
             current: l.a.any
         })]),
         K = l.a.oneOfType([l.a.instanceOf(Date), l.a.arrayOf(l.a.instanceOf(Date))]),
         Y = l.a.arrayOf(l.a.oneOf(B)),
         Q = function(e, t, n) {
@@ -27196,16 +27717,16 @@
             P = void 0 === k ? "›" : k,
             x = e.prev2AriaLabel,
             S = void 0 === x ? "" : x,
             A = e.prev2Label,
             R = void 0 === A ? "«" : A,
             z = e.prevAriaLabel,
             D = void 0 === z ? "" : z,
-            H = e.prevLabel,
-            I = void 0 === H ? "‹" : H,
+            I = e.prevLabel,
+            H = void 0 === I ? "‹" : I,
             L = e.setActiveStartDate,
             B = e.showDoubleView,
             q = e.view,
             F = e.views.indexOf(q) > 0,
             W = "century" !== q,
             V = function(e, t) {
                 switch (e) {
@@ -27313,23 +27834,23 @@
             "aria-label": S,
             className: "".concat(Z, "__arrow ").concat(Z, "__prev2-button"),
             disabled: G,
             onClick: function() {
                 L(U, "prev2")
             },
             type: "button"
-        }, R), null !== I && o.a.createElement("button", {
+        }, R), null !== H && o.a.createElement("button", {
             "aria-label": D,
             className: "".concat(Z, "__arrow ").concat(Z, "__prev-button"),
             disabled: Q,
             onClick: function() {
                 L(V, "prev")
             },
             type: "button"
-        }, I), (t = "".concat(Z, "__label"), o.a.createElement("button", {
+        }, H), (t = "".concat(Z, "__label"), o.a.createElement("button", {
             "aria-label": m,
             "aria-live": b,
             className: t,
             disabled: !F,
             onClick: r,
             style: {
                 flexGrow: 1
@@ -27847,33 +28368,33 @@
         return n
     }
 
     function Ne(e) {
         for (var t = 1; t < arguments.length; t++) {
             var n = null != arguments[t] ? arguments[t] : {};
             t % 2 ? Te(Object(n), !0).forEach((function(t) {
-                He(e, t, n[t])
+                Ie(e, t, n[t])
             })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : Te(Object(n)).forEach((function(t) {
                 Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
             }))
         }
         return e
     }
 
-    function He(e, t, n) {
+    function Ie(e, t, n) {
         return t in e ? Object.defineProperty(e, t, {
             value: n,
             enumerable: !0,
             configurable: !0,
             writable: !0
         }) : e[t] = n, e
     }
 
-    function Ie() {
-        return (Ie = Object.assign || function(e) {
+    function He() {
+        return (He = Object.assign || function(e) {
             for (var t = 1; t < arguments.length; t++) {
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
@@ -27897,15 +28418,15 @@
     function Be(e) {
         var t = e.classes,
             n = e.formatYear,
             r = void 0 === n ? j : n,
             a = Le(e, De),
             i = a.date,
             l = a.locale;
-        return o.a.createElement(ze, Ie({}, a, {
+        return o.a.createElement(ze, He({}, a, {
             classes: [].concat(t, "react-calendar__century-view__decades__decade"),
             maxDateTransform: s.getDecadeEnd,
             minDateTransform: s.getDecadeStart,
             view: "century"
         }), N(l, r, i))
     }
 
@@ -28328,15 +28849,15 @@
             i = e.calendarType,
             l = e.classes,
             c = e.currentMonthIndex,
             u = wt(e, vt),
             f = u.date,
             p = u.locale;
         return o.a.createElement(ze, _t({}, u, {
-            classes: [].concat(l, Et, H(f, i) ? "".concat(Et, "--weekend") : null, f.getMonth() !== c ? "".concat(Et, "--neighboringMonth") : null),
+            classes: [].concat(l, Et, I(f, i) ? "".concat(Et, "--weekend") : null, f.getMonth() !== c ? "".concat(Et, "--neighboringMonth") : null),
             formatAbbr: a,
             maxDateTransform: s.getDayEnd,
             minDateTransform: s.getDayStart,
             view: "month"
         }), n(p, f))
     }
     jt.propTypes = gt(gt({}, J), {}, {
@@ -28563,15 +29084,15 @@
                 var n = arguments[t];
                 for (var r in n) Object.prototype.hasOwnProperty.call(n, r) && (e[r] = n[r])
             }
             return e
         }).apply(this, arguments)
     }
 
-    function Ht(e, t) {
+    function It(e, t) {
         if (null == e) return {};
         var n, r, a = function(e, t) {
             if (null == e) return {};
             var n, r, a = {},
                 o = Object.keys(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || (a[n] = e[n]);
             return a
@@ -28579,29 +29100,29 @@
         if (Object.getOwnPropertySymbols) {
             var o = Object.getOwnPropertySymbols(e);
             for (r = 0; r < o.length; r++) n = o[r], t.indexOf(n) >= 0 || Object.prototype.propertyIsEnumerable.call(e, n) && (a[n] = e[n])
         }
         return a
     }
 
-    function It(e) {
+    function Ht(e) {
         var t = e.activeStartDate,
             n = e.locale,
             r = e.onMouseLeave,
             a = e.showFixedNumberOfWeeks,
             i = e.calendarType,
             l = void 0 === i ? function(e) {
                 return Object.keys(m).find((function(t) {
                     return m[t].includes(e)
                 })) || h.ISO_8601
             }(n) : i,
             u = e.formatShortWeekday,
             s = e.onClickWeekNumber,
             f = e.showWeekNumbers,
-            p = Ht(e, Tt);
+            p = It(e, Tt);
         return o.a.createElement("div", {
             className: Object(c.default)("react-calendar__month-view", f ? "".concat("react-calendar__month-view", "--weekNumbers") : "")
         }, o.a.createElement("div", {
             style: {
                 display: "flex",
                 alignItems: "flex-end"
             }
@@ -28621,15 +29142,15 @@
             formatShortWeekday: u,
             locale: n,
             onMouseLeave: r
         }), o.a.createElement(At, Nt({
             calendarType: l
         }, p)))))
     }
-    It.propTypes = {
+    Ht.propTypes = {
         activeStartDate: l.a.instanceOf(Date).isRequired,
         calendarType: q,
         formatShortWeekday: l.a.func,
         locale: l.a.string,
         onClickWeekNumber: l.a.func,
         onMouseLeave: l.a.func,
         showFixedNumberOfWeeks: l.a.bool,
@@ -29128,15 +29649,15 @@
                                 k = E.formatShortWeekday,
                                 P = E.onClickWeekNumber,
                                 x = E.showDoubleView,
                                 S = E.showFixedNumberOfWeeks,
                                 R = E.showNeighboringMonth,
                                 z = E.showWeekNumbers,
                                 D = this.onMouseLeave;
-                            return o.a.createElement(It, Bt({
+                            return o.a.createElement(Ht, Bt({
                                 calendarType: c,
                                 formatDay: j,
                                 formatLongDate: M,
                                 formatShortWeekday: k,
                                 onClickWeekNumber: P,
                                 onMouseLeave: p ? D : null,
                                 showFixedNumberOfWeeks: S || x,
@@ -29288,15 +29809,15 @@
     })), n.d(t, "CenturyView", (function() {
         return Ue
     })), n.d(t, "DecadeView", (function() {
         return rt
     })), n.d(t, "YearView", (function() {
         return bt
     })), n.d(t, "MonthView", (function() {
-        return It
+        return Ht
     }));
     t.default = mn
 }, function(e, t, n) {
     "use strict";
     n.r(t);
     var r = n(0),
         a = n.n(r),
@@ -29420,17 +29941,17 @@
             A = e.renderMinuteMarks,
             C = void 0 === A || A,
             R = e.renderNumbers,
             z = e.renderSecondHand,
             D = void 0 === z || z,
             T = e.secondHandLength,
             N = void 0 === T ? 90 : T,
-            H = e.secondHandOppositeLength,
-            I = e.secondHandWidth,
-            L = void 0 === I ? 1 : I,
+            I = e.secondHandOppositeLength,
+            H = e.secondHandWidth,
+            L = void 0 === H ? 1 : H,
             B = e.size,
             q = void 0 === B ? 150 : B,
             F = e.value;
         return a.a.createElement("time", {
             className: Object(l.default)("react-clock", n),
             dateTime: F instanceof Date ? F.toISOString() : F,
             style: {
@@ -29479,15 +30000,15 @@
         }(), function() {
             if (!D) return null;
             var e = F ? 360 * Object(c.getMinutes)(F) + 6 * Object(c.getSeconds)(F) : 0;
             return a.a.createElement(v, {
                 angle: e,
                 length: N,
                 name: "second",
-                oppositeLength: H,
+                oppositeLength: I,
                 width: L
             })
         }())
     }
     v.propTypes = {
         angle: i.a.number,
         length: p,
@@ -29747,17 +30268,17 @@
             return n && t(), n
         }
 
         function N() {
             return T(S, z)
         }
 
-        function H() {
+        function I() {
             return T(C, D)
-        }(a ? N() || H() : H() || N()) || function() {
+        }(a ? N() || I() : I() || N()) || function() {
             var e = S > C,
                 t = c[M] && parseInt(c[M], 10);
 
             function n(e) {
                 t && e < t && f("<Fit />'s child will not fit anywhere with its current ".concat(M, " of ").concat(t, "px."));
                 var n = Math.max(e, t || 0);
                 f("<Fit />'s child needed to have its ".concat(v, " decreased to ").concat(n, "px.")), r.style[v] = "".concat(n, "px")
```

### Comparing `dash_express_components-0.0.97/dash_express_components/metadata.json` & `dash_express_components-0.0.98/dash_express_components/metadata.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'src/lib/components/RequestStore.react.js'": "OrderedDict([('description', 'Easily keep data on "*

 * *                                               'the client side with this component.\\nThe data is '*

 * *                                               'not inserted in the DOM.\\nData can be in memory, '*

 * *                                               'localStorage or sessionStorage.\\nThe data will be '*

 * *                                               'kept with the id as key.\\nThe data will be '*

 * *                 […]*

```diff
@@ -870,14 +870,162 @@
                 "required": false,
                 "type": {
                     "name": "func"
                 }
             }
         }
     },
+    "src/lib/components/RequestStore.react.js": {
+        "description": "Easily keep data on the client side with this component.\nThe data is not inserted in the DOM.\nData can be in memory, localStorage or sessionStorage.\nThe data will be kept with the id as key.\nThe data will be collected from the url with additional info from the config\nWe use a longCallback feature, if set",
+        "displayName": "RequestStore",
+        "methods": [
+            {
+                "docblock": null,
+                "modifiers": [
+                    "async"
+                ],
+                "name": "fetchData",
+                "params": [
+                    {
+                        "name": "url",
+                        "type": null
+                    },
+                    {
+                        "name": "config",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            },
+            {
+                "docblock": null,
+                "modifiers": [],
+                "name": "onStorageChange",
+                "params": [
+                    {
+                        "name": "e",
+                        "type": null
+                    }
+                ],
+                "returns": null
+            }
+        ],
+        "props": {
+            "clear_data": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "config": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "data": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "union",
+                    "value": [
+                        {
+                            "name": "object"
+                        },
+                        {
+                            "name": "array"
+                        },
+                        {
+                            "name": "number"
+                        },
+                        {
+                            "name": "string"
+                        },
+                        {
+                            "name": "bool"
+                        }
+                    ]
+                }
+            },
+            "id": {
+                "description": "",
+                "required": true,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "longCallback": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "false"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "modified_timestamp": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "-1"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "setProps": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "storage_type": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'memory'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'local'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'session'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'memory'"
+                        }
+                    ]
+                }
+            },
+            "url": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            }
+        }
+    },
     "src/lib/components/Transform.react.js": {
         "description": "<div style=\"width:450px; margin-left: 20px; float: right;  margin-top: -150px;\">\n<img src=\"https://raw.githubusercontent.com/VK/dash-express-components/main/.media/transform.png\"/>\n<img src=\"https://raw.githubusercontent.com/VK/dash-express-components/main/.media/transform-modal.png\"/>\n<img src=\"https://raw.githubusercontent.com/VK/dash-express-components/main/.media/transform-types.png\"/>\n</div>\n\nThe `Transform` component helps to create user defined data transformations.\nCurrently basic transformations are available, like:\n\n<ul style=\"margin-left: 20px;\">\n   <li><b>eval</b></li>\n   <li><b>groupby([...]).aggr([...])</b></li>\n   <li><b>melt</b></li>\n   <li><b>wide_to_long</b></li>\n   <li><b>replace</b></li>\n   <li><b>rename</b></li>\n</ul>\n@hideconstructor\n\n@example\nimport dash_express_components as dxc\nimport plotly.express as px\n\nmeta = dxc.get_meta(px.data.gapminder())\n\ndxc.Transform(\n   id=\"transform\",\n   meta=meta\n)\n@public",
         "displayName": "Transform",
         "methods": [
             {
                 "docblock": null,
                 "modifiers": [],
```

### Comparing `dash_express_components-0.0.97/dash_express_components/package-info.json` & `dash_express_components-0.0.98/dash_express_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.98'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.97"
+    "version": "0.0.98"
 }
```

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_bar_count.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_box.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_histogram_line.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_imshow.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_probability.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/plottypes/_scatter.py` & `dash_express_components-0.0.98/dash_express_components/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_aggr.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_bin.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_eval.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_strsplit.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.98/dash_express_components/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components/utils.py` & `dash_express_components-0.0.98/dash_express_components/utils.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components.egg-info/PKG-INFO` & `dash_express_components-0.0.98/dash_express_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-express-components
-Version: 0.0.97
+Version: 0.0.98
 Summary: Simple widgets to add plotly express style plotting to dash
 Home-page: https://github.com/VK/dash-express-components
 Author: Viktor Krückl <viktor@krueckl.de>
 License: MIT
 Description: # Dash Express Components
         ![Publish release](https://github.com/VK/dash-express-components/workflows/Publish%20release/badge.svg)
         [![PyPI](https://img.shields.io/pypi/v/dash-express-components?logo=pypi)](https://pypi.org/project/dash-express-components)
```

### Comparing `dash_express_components-0.0.97/dash_express_components.egg-info/SOURCES.txt` & `dash_express_components-0.0.98/dash_express_components.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 dash_express_components/MeltTransform.py
 dash_express_components/MetaCheck.py
 dash_express_components/Parameterize.py
 dash_express_components/Plotter.py
 dash_express_components/PlotterBase.py
 dash_express_components/Probability.py
 dash_express_components/RenameTransform.py
+dash_express_components/RequestStore.py
 dash_express_components/Scatter.py
 dash_express_components/ScatterMatrix.py
 dash_express_components/StrSplitTransform.py
 dash_express_components/SubComponentBase.py
 dash_express_components/Table.py
 dash_express_components/Transform.py
 dash_express_components/Violin.py
```

### Comparing `dash_express_components-0.0.97/dash_express_components_base/__init__.py` & `dash_express_components-0.0.98/dash_express_components_base/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_bar_count.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_bar_count.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_box.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_box.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_histogram_line.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_histogram_line.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_imshow.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_imshow.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_probability.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_probability.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/plottypes/_scatter.py` & `dash_express_components-0.0.98/dash_express_components_base/plottypes/_scatter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_aggr.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_aggr.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_bin.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_bin.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_eval.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_eval.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_groupby_sample.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_groupby_sample.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_iqrfilter.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_iqrfilter.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_strsplit.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_strsplit.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/transformationtypes/_wide_to_long.py` & `dash_express_components-0.0.98/dash_express_components_base/transformationtypes/_wide_to_long.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/dash_express_components_base/utils.py` & `dash_express_components-0.0.98/dash_express_components_base/utils.py`

 * *Files identical despite different names*

### Comparing `dash_express_components-0.0.97/package.json` & `dash_express_components-0.0.98/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.0.98'"}*

```diff
@@ -59,9 +59,9 @@
         "build:patch": "python _patch.py",
         "doc": "jsdoc -c ./jsdoc.conf.json -a public",
         "prepublishOnly": "npm run validate-init",
         "start": "webpack-serve --config ./webpack.serve.config.js --open",
         "test": "pytest --cov=dash_express_components tests --cov-report term-missing",
         "validate-init": "python _validate_init.py"
     },
-    "version": "0.0.97"
+    "version": "0.0.98"
 }
```

### Comparing `dash_express_components-0.0.97/setup.py` & `dash_express_components-0.0.98/setup.py`

 * *Files identical despite different names*

