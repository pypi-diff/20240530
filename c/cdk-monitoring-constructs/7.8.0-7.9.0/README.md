# Comparing `tmp/cdk-monitoring-constructs-7.8.0.tar.gz` & `tmp/cdk-monitoring-constructs-7.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-monitoring-constructs-7.8.0.tar", last modified: Fri Mar 22 21:58:35 2024, max compression
+gzip compressed data, was "cdk-monitoring-constructs-7.9.0.tar", last modified: Thu May  9 18:45:01 2024, max compression
```

## Comparing `cdk-monitoring-constructs-7.8.0.tar` & `cdk-monitoring-constructs-7.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:58:35.908098 cdk-monitoring-constructs-7.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-03-22 21:58:35.908098 cdk-monitoring-constructs-7.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 21:58:35.908098 cdk-monitoring-constructs-7.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:58:35.896098 cdk-monitoring-constructs-7.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:58:35.904098 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/
--rw-r--r--   0 runner    (1001) docker     (127)  5350203 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:58:35.904098 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   874831 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@7.8.0.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:58:25.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 21:58:35.904098 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-03-22 21:58:35.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-22 21:58:35.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 21:58:35.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-03-22 21:58:35.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 21:58:35.000000 cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20293 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:45:01.594472 cdk-monitoring-constructs-7.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)  5356559 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   876089 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@7.9.0.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:44:50.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 18:45:01.602472 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21242 2024-05-09 18:45:01.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 18:45:01.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 18:45:01.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 18:45:01.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 18:45:01.000000 cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/top_level.txt
```

### Comparing `cdk-monitoring-constructs-7.8.0/LICENSE` & `cdk-monitoring-constructs-7.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-7.8.0/PKG-INFO` & `cdk-monitoring-constructs-7.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 7.8.0
+Version: 7.9.0
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-7.8.0/README.md` & `cdk-monitoring-constructs-7.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cdk-monitoring-constructs-7.8.0/setup.py` & `cdk-monitoring-constructs-7.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-monitoring-constructs",
-    "version": "7.8.0",
+    "version": "7.9.0",
     "description": "cdk-monitoring-constructs",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-monitoring-constructs",
     "long_description_content_type": "text/markdown",
     "author": "CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,26 +22,26 @@
     },
     "packages": [
         "cdk_monitoring_constructs",
         "cdk_monitoring_constructs._jsii"
     ],
     "package_data": {
         "cdk_monitoring_constructs._jsii": [
-            "cdk-monitoring-constructs@7.8.0.jsii.tgz"
+            "cdk-monitoring-constructs@7.9.0.jsii.tgz"
         ],
         "cdk_monitoring_constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.112.0, <3.0.0",
         "aws-cdk.aws-redshift-alpha>=2.112.0.a0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.95.0, <2.0.0",
+        "jsii>=1.98.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs/__init__.py` & `cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,14 +450,17 @@
 
 See [SECURITY](SECURITY.md) for more information.
 
 ## License
 
 This project is licensed under the Apache-2.0 License.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
@@ -6869,48 +6872,54 @@
         "title": "title",
         "add_to_summary_dashboard": "addToSummaryDashboard",
         "graph_widget_axis": "graphWidgetAxis",
         "graph_widget_legend": "graphWidgetLegend",
         "graph_widget_right_axis": "graphWidgetRightAxis",
         "graph_widget_set_period_to_time_range": "graphWidgetSetPeriodToTimeRange",
         "graph_widget_type": "graphWidgetType",
+        "graph_widget_width": "graphWidgetWidth",
         "horizontal_annotations": "horizontalAnnotations",
         "horizontal_right_annotations": "horizontalRightAnnotations",
         "important": "important",
+        "vertical_annotations": "verticalAnnotations",
     },
 )
 class CustomMetricGroup:
     def __init__(
         self,
         *,
         metrics: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.Metric, _aws_cdk_aws_cloudwatch_ceddda9d.MathExpression, typing.Union["CustomMetricWithAlarm", typing.Dict[builtins.str, typing.Any]], typing.Union["CustomMetricWithAnomalyDetection", typing.Dict[builtins.str, typing.Any]], typing.Union["CustomMetricSearch", typing.Dict[builtins.str, typing.Any]]]],
         title: builtins.str,
         add_to_summary_dashboard: typing.Optional[builtins.bool] = None,
         graph_widget_axis: typing.Optional[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]]] = None,
         graph_widget_legend: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.LegendPosition] = None,
         graph_widget_right_axis: typing.Optional[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]]] = None,
         graph_widget_set_period_to_time_range: typing.Optional[builtins.bool] = None,
         graph_widget_type: typing.Optional["GraphWidgetType"] = None,
+        graph_widget_width: typing.Optional[jsii.Number] = None,
         horizontal_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         horizontal_right_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         important: typing.Optional[builtins.bool] = None,
+        vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''(experimental) Custom metric group represents a single widget.
 
         :param metrics: (experimental) list of metrics in the group (can be defined in different ways, see the type documentation).
         :param title: (experimental) title of the whole group.
         :param add_to_summary_dashboard: (experimental) Flag indicating this metric group should be included in the summary as well. Default: - addToSummaryDashboard from CustomMonitoringProps, defaulting to false
         :param graph_widget_axis: (experimental) optional axis. Default: undefined
         :param graph_widget_legend: (experimental) graph widget legend. Default: BOTTOM
         :param graph_widget_right_axis: (experimental) optional right axis. Default: undefined
         :param graph_widget_set_period_to_time_range: 
         :param graph_widget_type: (experimental) type of the widget. Default: line
-        :param horizontal_annotations: (experimental) optional custom horizontal annotations which will be displayed over the metrics on the left axis (if there are any alarms, any existing annotations will be merged together).
-        :param horizontal_right_annotations: (experimental) optional custom horizontal annotations which will be displayed over the metrics on the right axis (if there are any alarms, any existing annotations will be merged together).
+        :param graph_widget_width: (experimental) Width of graph widget. Note that widgets will overflow into new rows if the summed width exceeds 24. Default: - Automatically calculcated width, generally as wide as possible considering all metrics' widgets.
+        :param horizontal_annotations: (experimental) Optional custom horizontal annotations which will be displayed over the metrics on the left axis (if there are any alarms, any existing annotations will be merged together).
+        :param horizontal_right_annotations: (experimental) Optional custom horizontal annotations which will be displayed over the metrics on the right axis (if there are any alarms, any existing annotations will be merged together).
         :param important: 
+        :param vertical_annotations: (experimental) Optional custom vertical annotations which will be displayed over the metrics.
 
         :stability: experimental
         '''
         if isinstance(graph_widget_axis, dict):
             graph_widget_axis = _aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps(**graph_widget_axis)
         if isinstance(graph_widget_right_axis, dict):
             graph_widget_right_axis = _aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps(**graph_widget_right_axis)
@@ -6920,17 +6929,19 @@
             check_type(argname="argument title", value=title, expected_type=type_hints["title"])
             check_type(argname="argument add_to_summary_dashboard", value=add_to_summary_dashboard, expected_type=type_hints["add_to_summary_dashboard"])
             check_type(argname="argument graph_widget_axis", value=graph_widget_axis, expected_type=type_hints["graph_widget_axis"])
             check_type(argname="argument graph_widget_legend", value=graph_widget_legend, expected_type=type_hints["graph_widget_legend"])
             check_type(argname="argument graph_widget_right_axis", value=graph_widget_right_axis, expected_type=type_hints["graph_widget_right_axis"])
             check_type(argname="argument graph_widget_set_period_to_time_range", value=graph_widget_set_period_to_time_range, expected_type=type_hints["graph_widget_set_period_to_time_range"])
             check_type(argname="argument graph_widget_type", value=graph_widget_type, expected_type=type_hints["graph_widget_type"])
+            check_type(argname="argument graph_widget_width", value=graph_widget_width, expected_type=type_hints["graph_widget_width"])
             check_type(argname="argument horizontal_annotations", value=horizontal_annotations, expected_type=type_hints["horizontal_annotations"])
             check_type(argname="argument horizontal_right_annotations", value=horizontal_right_annotations, expected_type=type_hints["horizontal_right_annotations"])
             check_type(argname="argument important", value=important, expected_type=type_hints["important"])
+            check_type(argname="argument vertical_annotations", value=vertical_annotations, expected_type=type_hints["vertical_annotations"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "metrics": metrics,
             "title": title,
         }
         if add_to_summary_dashboard is not None:
             self._values["add_to_summary_dashboard"] = add_to_summary_dashboard
         if graph_widget_axis is not None:
@@ -6939,20 +6950,24 @@
             self._values["graph_widget_legend"] = graph_widget_legend
         if graph_widget_right_axis is not None:
             self._values["graph_widget_right_axis"] = graph_widget_right_axis
         if graph_widget_set_period_to_time_range is not None:
             self._values["graph_widget_set_period_to_time_range"] = graph_widget_set_period_to_time_range
         if graph_widget_type is not None:
             self._values["graph_widget_type"] = graph_widget_type
+        if graph_widget_width is not None:
+            self._values["graph_widget_width"] = graph_widget_width
         if horizontal_annotations is not None:
             self._values["horizontal_annotations"] = horizontal_annotations
         if horizontal_right_annotations is not None:
             self._values["horizontal_right_annotations"] = horizontal_right_annotations
         if important is not None:
             self._values["important"] = important
+        if vertical_annotations is not None:
+            self._values["vertical_annotations"] = vertical_annotations
 
     @builtins.property
     def metrics(
         self,
     ) -> typing.List[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.Metric, _aws_cdk_aws_cloudwatch_ceddda9d.MathExpression, "CustomMetricWithAlarm", "CustomMetricWithAnomalyDetection", "CustomMetricSearch"]]:
         '''(experimental) list of metrics in the group (can be defined in different ways, see the type documentation).
 
@@ -7039,29 +7054,43 @@
 
         :stability: experimental
         '''
         result = self._values.get("graph_widget_type")
         return typing.cast(typing.Optional["GraphWidgetType"], result)
 
     @builtins.property
+    def graph_widget_width(self) -> typing.Optional[jsii.Number]:
+        '''(experimental) Width of graph widget.
+
+        Note that widgets will overflow into new rows if the summed width
+        exceeds 24.
+
+        :default: - Automatically calculcated width, generally as wide as possible considering all metrics' widgets.
+
+        :stability: experimental
+        '''
+        result = self._values.get("graph_widget_width")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
     def horizontal_annotations(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation]]:
-        '''(experimental) optional custom horizontal annotations which will be displayed over the metrics on the left axis (if there are any alarms, any existing annotations will be merged together).
+        '''(experimental) Optional custom horizontal annotations which will be displayed over the metrics on the left axis (if there are any alarms, any existing annotations will be merged together).
 
         :stability: experimental
         '''
         result = self._values.get("horizontal_annotations")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation]], result)
 
     @builtins.property
     def horizontal_right_annotations(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation]]:
-        '''(experimental) optional custom horizontal annotations which will be displayed over the metrics on the right axis (if there are any alarms, any existing annotations will be merged together).
+        '''(experimental) Optional custom horizontal annotations which will be displayed over the metrics on the right axis (if there are any alarms, any existing annotations will be merged together).
 
         :stability: experimental
         '''
         result = self._values.get("horizontal_right_annotations")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation]], result)
 
     @builtins.property
@@ -7071,14 +7100,25 @@
 
         :see: addToSummaryDashboard
         :stability: deprecated
         '''
         result = self._values.get("important")
         return typing.cast(typing.Optional[builtins.bool], result)
 
+    @builtins.property
+    def vertical_annotations(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]]:
+        '''(experimental) Optional custom vertical annotations which will be displayed over the metrics.
+
+        :stability: experimental
+        '''
+        result = self._values.get("vertical_annotations")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -7091,50 +7131,55 @@
     jsii_type="cdk-monitoring-constructs.CustomMetricGroupWithAnnotations",
     jsii_struct_bases=[],
     name_mapping={
         "annotations": "annotations",
         "metric_group": "metricGroup",
         "right_annotations": "rightAnnotations",
         "title_addons": "titleAddons",
+        "vertical_annotations": "verticalAnnotations",
         "height": "height",
     },
 )
 class CustomMetricGroupWithAnnotations:
     def __init__(
         self,
         *,
         annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]],
         metric_group: typing.Union[CustomMetricGroup, typing.Dict[builtins.str, typing.Any]],
         right_annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]],
         title_addons: typing.Sequence[builtins.str],
+        vertical_annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]],
         height: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
         :param annotations: 
         :param metric_group: 
         :param right_annotations: 
         :param title_addons: 
+        :param vertical_annotations: 
         :param height: 
 
         :stability: experimental
         '''
         if isinstance(metric_group, dict):
             metric_group = CustomMetricGroup(**metric_group)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7619d758dc272ff2b4dce9aa14e3ace0f18384f3dc45801e8569a8e01ebe8da9)
             check_type(argname="argument annotations", value=annotations, expected_type=type_hints["annotations"])
             check_type(argname="argument metric_group", value=metric_group, expected_type=type_hints["metric_group"])
             check_type(argname="argument right_annotations", value=right_annotations, expected_type=type_hints["right_annotations"])
             check_type(argname="argument title_addons", value=title_addons, expected_type=type_hints["title_addons"])
+            check_type(argname="argument vertical_annotations", value=vertical_annotations, expected_type=type_hints["vertical_annotations"])
             check_type(argname="argument height", value=height, expected_type=type_hints["height"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "annotations": annotations,
             "metric_group": metric_group,
             "right_annotations": right_annotations,
             "title_addons": title_addons,
+            "vertical_annotations": vertical_annotations,
         }
         if height is not None:
             self._values["height"] = height
 
     @builtins.property
     def annotations(
         self,
@@ -7172,14 +7217,25 @@
         :stability: experimental
         '''
         result = self._values.get("title_addons")
         assert result is not None, "Required property 'title_addons' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
+    def vertical_annotations(
+        self,
+    ) -> typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("vertical_annotations")
+        assert result is not None, "Required property 'vertical_annotations' is missing"
+        return typing.cast(typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation], result)
+
+    @builtins.property
     def height(self) -> typing.Optional[jsii.Number]:
         '''
         :stability: experimental
         '''
         result = self._values.get("height")
         return typing.cast(typing.Optional[jsii.Number], result)
 
@@ -9474,38 +9530,41 @@
         left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         right_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
         right_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         width: jsii.Number,
         left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         right_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         title: typing.Optional[builtins.str] = None,
+        vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param height: 
         :param left_axis: 
         :param left_metrics: 
         :param right_axis: 
         :param right_metrics: 
         :param width: 
         :param left_annotations: 
         :param right_annotations: 
         :param title: 
+        :param vertical_annotations: 
 
         :stability: experimental
         '''
         props = DoubleAxisGraphWidgetProps(
             height=height,
             left_axis=left_axis,
             left_metrics=left_metrics,
             right_axis=right_axis,
             right_metrics=right_metrics,
             width=width,
             left_annotations=left_annotations,
             right_annotations=right_annotations,
             title=title,
+            vertical_annotations=vertical_annotations,
         )
 
         jsii.create(self.__class__, self, [props])
 
 
 @jsii.data_type(
     jsii_type="cdk-monitoring-constructs.DoubleAxisGraphWidgetProps",
@@ -9516,14 +9575,15 @@
         "left_metrics": "leftMetrics",
         "right_axis": "rightAxis",
         "right_metrics": "rightMetrics",
         "width": "width",
         "left_annotations": "leftAnnotations",
         "right_annotations": "rightAnnotations",
         "title": "title",
+        "vertical_annotations": "verticalAnnotations",
     },
 )
 class DoubleAxisGraphWidgetProps:
     def __init__(
         self,
         *,
         height: jsii.Number,
@@ -9531,25 +9591,27 @@
         left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         right_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
         right_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         width: jsii.Number,
         left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         right_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         title: typing.Optional[builtins.str] = None,
+        vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param height: 
         :param left_axis: 
         :param left_metrics: 
         :param right_axis: 
         :param right_metrics: 
         :param width: 
         :param left_annotations: 
         :param right_annotations: 
         :param title: 
+        :param vertical_annotations: 
 
         :stability: experimental
         '''
         if isinstance(left_axis, dict):
             left_axis = _aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps(**left_axis)
         if isinstance(right_axis, dict):
             right_axis = _aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps(**right_axis)
@@ -9560,28 +9622,31 @@
             check_type(argname="argument left_metrics", value=left_metrics, expected_type=type_hints["left_metrics"])
             check_type(argname="argument right_axis", value=right_axis, expected_type=type_hints["right_axis"])
             check_type(argname="argument right_metrics", value=right_metrics, expected_type=type_hints["right_metrics"])
             check_type(argname="argument width", value=width, expected_type=type_hints["width"])
             check_type(argname="argument left_annotations", value=left_annotations, expected_type=type_hints["left_annotations"])
             check_type(argname="argument right_annotations", value=right_annotations, expected_type=type_hints["right_annotations"])
             check_type(argname="argument title", value=title, expected_type=type_hints["title"])
+            check_type(argname="argument vertical_annotations", value=vertical_annotations, expected_type=type_hints["vertical_annotations"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "height": height,
             "left_axis": left_axis,
             "left_metrics": left_metrics,
             "right_axis": right_axis,
             "right_metrics": right_metrics,
             "width": width,
         }
         if left_annotations is not None:
             self._values["left_annotations"] = left_annotations
         if right_annotations is not None:
             self._values["right_annotations"] = right_annotations
         if title is not None:
             self._values["title"] = title
+        if vertical_annotations is not None:
+            self._values["vertical_annotations"] = vertical_annotations
 
     @builtins.property
     def height(self) -> jsii.Number:
         '''
         :stability: experimental
         '''
         result = self._values.get("height")
@@ -9657,14 +9722,24 @@
     def title(self) -> typing.Optional[builtins.str]:
         '''
         :stability: experimental
         '''
         result = self._values.get("title")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def vertical_annotations(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("vertical_annotations")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -42168,32 +42243,35 @@
         *,
         height: jsii.Number,
         left_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
         left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         width: jsii.Number,
         left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         title: typing.Optional[builtins.str] = None,
+        vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param height: 
         :param left_axis: 
         :param left_metrics: 
         :param width: 
         :param left_annotations: 
         :param title: 
+        :param vertical_annotations: 
 
         :stability: experimental
         '''
         props = SingleAxisGraphWidgetProps(
             height=height,
             left_axis=left_axis,
             left_metrics=left_metrics,
             width=width,
             left_annotations=left_annotations,
             title=title,
+            vertical_annotations=vertical_annotations,
         )
 
         jsii.create(self.__class__, self, [props])
 
 
 @jsii.data_type(
     jsii_type="cdk-monitoring-constructs.SingleAxisGraphWidgetProps",
@@ -42201,57 +42279,63 @@
     name_mapping={
         "height": "height",
         "left_axis": "leftAxis",
         "left_metrics": "leftMetrics",
         "width": "width",
         "left_annotations": "leftAnnotations",
         "title": "title",
+        "vertical_annotations": "verticalAnnotations",
     },
 )
 class SingleAxisGraphWidgetProps:
     def __init__(
         self,
         *,
         height: jsii.Number,
         left_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
         left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
         width: jsii.Number,
         left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
         title: typing.Optional[builtins.str] = None,
+        vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param height: 
         :param left_axis: 
         :param left_metrics: 
         :param width: 
         :param left_annotations: 
         :param title: 
+        :param vertical_annotations: 
 
         :stability: experimental
         '''
         if isinstance(left_axis, dict):
             left_axis = _aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps(**left_axis)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d72bf22c52f04fd226d58000182c7e1cc0ffaace8ad51a30f291b9867034aa68)
             check_type(argname="argument height", value=height, expected_type=type_hints["height"])
             check_type(argname="argument left_axis", value=left_axis, expected_type=type_hints["left_axis"])
             check_type(argname="argument left_metrics", value=left_metrics, expected_type=type_hints["left_metrics"])
             check_type(argname="argument width", value=width, expected_type=type_hints["width"])
             check_type(argname="argument left_annotations", value=left_annotations, expected_type=type_hints["left_annotations"])
             check_type(argname="argument title", value=title, expected_type=type_hints["title"])
+            check_type(argname="argument vertical_annotations", value=vertical_annotations, expected_type=type_hints["vertical_annotations"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "height": height,
             "left_axis": left_axis,
             "left_metrics": left_metrics,
             "width": width,
         }
         if left_annotations is not None:
             self._values["left_annotations"] = left_annotations
         if title is not None:
             self._values["title"] = title
+        if vertical_annotations is not None:
+            self._values["vertical_annotations"] = vertical_annotations
 
     @builtins.property
     def height(self) -> jsii.Number:
         '''
         :stability: experimental
         '''
         result = self._values.get("height")
@@ -42299,14 +42383,24 @@
     def title(self) -> typing.Optional[builtins.str]:
         '''
         :stability: experimental
         '''
         result = self._values.get("title")
         return typing.cast(typing.Optional[builtins.str], result)
 
+    @builtins.property
+    def vertical_annotations(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("vertical_annotations")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -57277,17 +57371,17 @@
         add_to_alarm_dashboard: typing.Optional[builtins.bool] = None,
         add_to_detail_dashboard: typing.Optional[builtins.bool] = None,
         add_to_summary_dashboard: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param scope: -
         :param metric_groups: (experimental) define metric groups and metrics inside them (each metric group represents a widget).
-        :param description: (experimental) optional description of the whole section, in markdown. Default: no description
-        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: minimum height (should fit one or two lines of text)
-        :param height: (experimental) height override. Default: default height
+        :param description: (experimental) optional description of the whole section, in markdown. Default: - no description
+        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: - minimum height (should fit one or two lines of text)
+        :param height: (experimental) Height override. Default: - default height
         :param use_created_alarms: (experimental) Calls provided function to process all alarms created.
         :param alarm_friendly_name: (experimental) Plain name, used in naming alarms. This unique among other resources, and respect the AWS CDK restriction posed on alarm names. The length must be 1 - 255 characters and although the validation rules are undocumented, we recommend using ASCII and hyphens. Default: - derives name from the construct itself
         :param human_readable_name: (experimental) Human-readable name is a freeform string, used as a caption or description. There are no limitations on what it can be. Default: - use alarmFriendlyName
         :param local_alarm_name_prefix_override: (experimental) If this is defined, the local alarm name prefix used in naming alarms for the construct will be set to this value. The length must be 1 - 255 characters and although the validation rules are undocumented, we recommend using ASCII and hyphens.
         :param add_to_alarm_dashboard: (experimental) Flag indicating if the widgets should be added to alarm dashboard. Default: - true
         :param add_to_detail_dashboard: (experimental) Flag indicating if the widgets should be added to detailed dashboard. Default: - true
         :param add_to_summary_dashboard: (experimental) Flag indicating if the widgets should be added to summary dashboard. Default: - true
@@ -57432,17 +57526,17 @@
         :param human_readable_name: (experimental) Human-readable name is a freeform string, used as a caption or description. There are no limitations on what it can be. Default: - use alarmFriendlyName
         :param local_alarm_name_prefix_override: (experimental) If this is defined, the local alarm name prefix used in naming alarms for the construct will be set to this value. The length must be 1 - 255 characters and although the validation rules are undocumented, we recommend using ASCII and hyphens.
         :param add_to_alarm_dashboard: (experimental) Flag indicating if the widgets should be added to alarm dashboard. Default: - true
         :param add_to_detail_dashboard: (experimental) Flag indicating if the widgets should be added to detailed dashboard. Default: - true
         :param add_to_summary_dashboard: (experimental) Flag indicating if the widgets should be added to summary dashboard. Default: - true
         :param use_created_alarms: (experimental) Calls provided function to process all alarms created.
         :param metric_groups: (experimental) define metric groups and metrics inside them (each metric group represents a widget).
-        :param description: (experimental) optional description of the whole section, in markdown. Default: no description
-        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: minimum height (should fit one or two lines of text)
-        :param height: (experimental) height override. Default: default height
+        :param description: (experimental) optional description of the whole section, in markdown. Default: - no description
+        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: - minimum height (should fit one or two lines of text)
+        :param height: (experimental) Height override. Default: - default height
 
         :stability: experimental
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__34981c330536725daac1b224ffb995800483868db8f6c76aee1c38ee2dbac848)
             check_type(argname="argument alarm_friendly_name", value=alarm_friendly_name, expected_type=type_hints["alarm_friendly_name"])
             check_type(argname="argument human_readable_name", value=human_readable_name, expected_type=type_hints["human_readable_name"])
@@ -57570,37 +57664,37 @@
         assert result is not None, "Required property 'metric_groups' is missing"
         return typing.cast(typing.List[CustomMetricGroup], result)
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         '''(experimental) optional description of the whole section, in markdown.
 
-        :default: no description
+        :default: - no description
 
         :stability: experimental
         '''
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def description_widget_height(self) -> typing.Optional[jsii.Number]:
         '''(experimental) optional height of the description widget, so the content fits.
 
-        :default: minimum height (should fit one or two lines of text)
+        :default: - minimum height (should fit one or two lines of text)
 
         :stability: experimental
         '''
         result = self._values.get("description_widget_height")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def height(self) -> typing.Optional[jsii.Number]:
-        '''(experimental) height override.
+        '''(experimental) Height override.
 
-        :default: default height
+        :default: - default height
 
         :stability: experimental
         '''
         result = self._values.get("height")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
@@ -72417,17 +72511,17 @@
         local_alarm_name_prefix_override: typing.Optional[builtins.str] = None,
         add_to_alarm_dashboard: typing.Optional[builtins.bool] = None,
         add_to_detail_dashboard: typing.Optional[builtins.bool] = None,
         add_to_summary_dashboard: typing.Optional[builtins.bool] = None,
     ) -> "MonitoringFacade":
         '''
         :param metric_groups: (experimental) define metric groups and metrics inside them (each metric group represents a widget).
-        :param description: (experimental) optional description of the whole section, in markdown. Default: no description
-        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: minimum height (should fit one or two lines of text)
-        :param height: (experimental) height override. Default: default height
+        :param description: (experimental) optional description of the whole section, in markdown. Default: - no description
+        :param description_widget_height: (experimental) optional height of the description widget, so the content fits. Default: - minimum height (should fit one or two lines of text)
+        :param height: (experimental) Height override. Default: - default height
         :param use_created_alarms: (experimental) Calls provided function to process all alarms created.
         :param alarm_friendly_name: (experimental) Plain name, used in naming alarms. This unique among other resources, and respect the AWS CDK restriction posed on alarm names. The length must be 1 - 255 characters and although the validation rules are undocumented, we recommend using ASCII and hyphens. Default: - derives name from the construct itself
         :param human_readable_name: (experimental) Human-readable name is a freeform string, used as a caption or description. There are no limitations on what it can be. Default: - use alarmFriendlyName
         :param local_alarm_name_prefix_override: (experimental) If this is defined, the local alarm name prefix used in naming alarms for the construct will be set to this value. The length must be 1 - 255 characters and although the validation rules are undocumented, we recommend using ASCII and hyphens.
         :param add_to_alarm_dashboard: (experimental) Flag indicating if the widgets should be added to alarm dashboard. Default: - true
         :param add_to_detail_dashboard: (experimental) Flag indicating if the widgets should be added to detailed dashboard. Default: - true
         :param add_to_summary_dashboard: (experimental) Flag indicating if the widgets should be added to summary dashboard. Default: - true
@@ -89538,27 +89632,30 @@
     title: builtins.str,
     add_to_summary_dashboard: typing.Optional[builtins.bool] = None,
     graph_widget_axis: typing.Optional[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]]] = None,
     graph_widget_legend: typing.Optional[_aws_cdk_aws_cloudwatch_ceddda9d.LegendPosition] = None,
     graph_widget_right_axis: typing.Optional[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]]] = None,
     graph_widget_set_period_to_time_range: typing.Optional[builtins.bool] = None,
     graph_widget_type: typing.Optional[GraphWidgetType] = None,
+    graph_widget_width: typing.Optional[jsii.Number] = None,
     horizontal_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     horizontal_right_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     important: typing.Optional[builtins.bool] = None,
+    vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7619d758dc272ff2b4dce9aa14e3ace0f18384f3dc45801e8569a8e01ebe8da9(
     *,
     annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]],
     metric_group: typing.Union[CustomMetricGroup, typing.Dict[builtins.str, typing.Any]],
     right_annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]],
     title_addons: typing.Sequence[builtins.str],
+    vertical_annotations: typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]],
     height: typing.Optional[jsii.Number] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__63182d2487fd8c5519734296bd6fa20b09a86af420cdcfc68cf5fdce11729f57(
     *,
@@ -89753,14 +89850,15 @@
     left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
     right_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
     right_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
     width: jsii.Number,
     left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     right_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     title: typing.Optional[builtins.str] = None,
+    vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__24b978702f49c7ab143fcb30e1776a46fffc7f211ee09c8723117cae8f591c13(
     *,
     action_override: typing.Optional[IAlarmActionStrategy] = None,
@@ -92568,14 +92666,15 @@
     *,
     height: jsii.Number,
     left_axis: typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.YAxisProps, typing.Dict[builtins.str, typing.Any]],
     left_metrics: typing.Sequence[_aws_cdk_aws_cloudwatch_ceddda9d.IMetric],
     width: jsii.Number,
     left_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.HorizontalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
     title: typing.Optional[builtins.str] = None,
+    vertical_annotations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_cloudwatch_ceddda9d.VerticalAnnotation, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8e0eb186116c26e720fe3990d6b02393d658c0ebb7b269c251f984e195974e7c(
     widget: _aws_cdk_aws_cloudwatch_ceddda9d.IWidget,
     dashboards_to_include: typing.Optional[typing.Sequence[builtins.str]] = None,
```

### Comparing `cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO` & `cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-monitoring-constructs
-Version: 7.8.0
+Version: 7.9.0
 Summary: cdk-monitoring-constructs
 Home-page: https://github.com/cdklabs/cdk-monitoring-constructs
 Author: CDK Monitoring Constructs Team<monitoring-cdk-constructs@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-monitoring-constructs
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-monitoring-constructs-7.8.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt` & `cdk-monitoring-constructs-7.9.0/src/cdk_monitoring_constructs.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 src/cdk_monitoring_constructs/py.typed
 src/cdk_monitoring_constructs.egg-info/PKG-INFO
 src/cdk_monitoring_constructs.egg-info/SOURCES.txt
 src/cdk_monitoring_constructs.egg-info/dependency_links.txt
 src/cdk_monitoring_constructs.egg-info/requires.txt
 src/cdk_monitoring_constructs.egg-info/top_level.txt
 src/cdk_monitoring_constructs/_jsii/__init__.py
-src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@7.8.0.jsii.tgz
+src/cdk_monitoring_constructs/_jsii/cdk-monitoring-constructs@7.9.0.jsii.tgz
```

