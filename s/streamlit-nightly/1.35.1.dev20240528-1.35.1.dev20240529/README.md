# Comparing `tmp/streamlit_nightly-1.35.1.dev20240528.tar.gz` & `tmp/streamlit_nightly-1.35.1.dev20240529.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_nightly-1.35.1.dev20240528.tar", last modified: Wed May 29 07:31:56 2024, max compression
+gzip compressed data, was "streamlit_nightly-1.35.1.dev20240529.tar", last modified: Thu May 30 06:54:39 2024, max compression
```

## Comparing `streamlit_nightly-1.35.1.dev20240528.tar` & `streamlit_nightly-1.35.1.dev20240529.tar`

### file list

```diff
@@ -1,572 +1,572 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.732163 streamlit_nightly-1.35.1.dev20240528/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-29 07:31:56.732163 streamlit_nightly-1.35.1.dev20240528/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.612163 streamlit_nightly-1.35.1.dev20240528/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/bin/streamlit.cmd
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 07:31:56.732163 streamlit_nightly-1.35.1.dev20240528/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.620163 streamlit_nightly-1.35.1.dev20240528/streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/case_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/cli_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/code_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/color_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/column_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.620163 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/execution_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/experimental_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/logo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/commands/page_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.620163 streamlit_nightly-1.35.1.dev20240528/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.624163 streamlit_nightly-1.35.1.dev20240528/streamlit/components/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/lib/local_component_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.624163 streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/base_component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/base_custom_component.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.624163 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/component_arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/component_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/custom_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    43657 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/config_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/config_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.624163 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/snowflake_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/snowpark_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/sql_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/connections/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/delta_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/deprecation_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/development.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/echo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.632163 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/balloons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/bokeh_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/deck_gl_json_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/dialog_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/doc_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/graphviz_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/heading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/iframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/layouts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.632163 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30696 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/built_in_chart_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/column_config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/dicttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/mutable_status_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/pandas_styler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/streamlit_plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/subtitle_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/map.py
--rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/plotly_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/pyplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/snow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/toast.py
--rw-r--r--   0 runner    (1001) docker     (127)    69887 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/vega_charts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.636163 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/camera_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/color_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)    36465 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/data_editor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/multiselect.py
--rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/number_input.py
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/radio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/select_slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/selectbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    26704 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/slider.py
--rw-r--r--   0 runner    (1001) docker     (127)    22376 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/text_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    30085 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/time_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/elements/write.py
--rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/emojis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/env_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/error_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.636163 streamlit_nightly-1.35.1.dev20240528/streamlit/external/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.636163 streamlit_nightly-1.35.1.dev20240528/streamlit/external/langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/external/langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/external/langchain/streamlit_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/file_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/folder_black_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/git_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.636163 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/Hello.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.636163 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/0_Animation_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/1_Plotting_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/2_Mapping_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/3_DataFrame_Demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/hello/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/js_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/material_icon_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/net_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.664163 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Alert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Alert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AppPage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AppPage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowNamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowNamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowVegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Arrow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Arrow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Audio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Audio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AutoRerun_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AutoRerun_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BackMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BackMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Balloons_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Balloons_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Block_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Block_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BokehChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BokehChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Button_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Button_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/CameraInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/CameraInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ChatInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ChatInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Checkbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Checkbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ClientState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ClientState_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Code_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Code_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ColorPicker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ColorPicker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Components_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DataFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DataFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DateInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DateInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DeckGlJsonChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DeckGlJsonChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Delta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Delta_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DocString_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DocString_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DownloadButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DownloadButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Element_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Element_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Empty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Empty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Exception_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Exception_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Favicon_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Favicon_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/FileUploader_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/FileUploader_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ForwardMsg_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12312 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ForwardMsg_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GitInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GitInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GraphVizChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GraphVizChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Heading_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Heading_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Html_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Html_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/IFrame_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/IFrame_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Json_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Json_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LabelVisibilityMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LabelVisibilityMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LinkButton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LinkButton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Logo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Logo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Markdown_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Markdown_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Metric_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Metric_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/MultiSelect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/MultiSelect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NamedDataSet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NamedDataSet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NewSession_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NewSession_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NumberInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NumberInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageConfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageConfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageInfo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageInfo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageLink_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageLink_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageNotFound_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageNotFound_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageProfile_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageProfile_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PagesChanged_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PagesChanged_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ParentMessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ParentMessage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PlotlyChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PlotlyChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Progress_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Progress_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Radio_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Radio_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/RootContainer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/RootContainer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Selectbox_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Selectbox_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionEvent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionEvent_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionStatus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Skeleton_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Skeleton_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Slider_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Slider_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Snow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Snow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Spinner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Spinner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextArea_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextArea_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Text_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Text_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TimeInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TimeInput_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Toast_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Toast_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/VegaLiteChart_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/VegaLiteChart_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Video_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Video_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/WidgetStates_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/WidgetStates_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/openmetrics_data_model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-29 07:28:07.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/proto/openmetrics_data_model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.664163 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36663 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/app_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.668163 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_data_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cached_message_replay.py
--rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/legacy_cache_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.668163 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/cache_storage_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/dummy_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/local_disk_cache_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/connection_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/forward_msg_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/forward_msg_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/media_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_media_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_session_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14267 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/metrics_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/runtime_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.668163 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/magic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/magic_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_run_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/session_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.672163 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/query_params_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/safe_session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/session_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/session_state_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/uploaded_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/websocket_session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/source_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.672163 streamlit_nightly-1.35.1.dev20240528/streamlit/static/
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 07:28:36.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.612163 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.672163 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/3466.8b8f33d6.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/5441.e3b876c5.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/8148.49dfd2ce.chunk.css
--rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/main.3aaaea00.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.704163 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1074.73973756.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1168.14f7c6ff.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1307.0f0cca93.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1451.3b0a3e31.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1479.6709db03.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/178.7bea8c5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2178.90362aae.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2187.9469f035.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2469.09ea79bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2634.1249dc7a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2736.4336e2b9.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3053.7e70ec3b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/329.464ed8ec.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3301.1d1b10bb.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3466.05d62820.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3513.7dedbda2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4113.99983645.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4132.49bf3f2c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4177.69f9f18d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4319.bf1c86bf.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4477.1bd49702.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4500.b6f348d1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4666.c4b22a63.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/474.7eb0c6cd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5106.44f0ff51.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5117.04bfe5d3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5249.f2f4070d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5345.73d26e5d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5379.f08eddd1.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5441.1b94928f.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5791.9a42fb4b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6013.4ba2d616.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6405.ac5a6f23.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6718.802da17e.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6853.93dd1c4c.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6950.70fe55c2.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7142.83028745.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7175.583ff733.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7323.b74cc85b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7483.64f23be7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7602.e8abc06b.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7805.acc6316a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8005.43974a35.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    51165 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8148.293984e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8477.de889fe5.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8492.0d93bd08.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8536.f8de3d9a.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8570.6de19120.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8691.4211c305.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9330.2b4c99e0.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9336.3e046ad7.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/937.a1248039.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9656.8c935274.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9865.fd93213d.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)  4405383 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/main.206766ee.js
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/main.206766ee.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
--rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
--rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
--rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
--rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
--rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-29 07:31:53.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/temporary_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/app_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/element_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/local_script_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/type_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/url_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/user_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/ipython/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/ipython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/ipython/modified_sys_path.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.724163 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/pympler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/pympler/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/pympler/asizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.728163 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/event_based_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/local_sources_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/polling_path_watcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.728163 streamlit_nightly-1.35.1.dev20240528/streamlit/web/
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/cache_storage_manager_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.728163 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/app_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/browser_websocket_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/component_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/media_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/server_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/stats_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/upload_file_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/websocket_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.732163 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23268 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 07:28:02.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 07:31:55.000000 streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 07:31:56.732163 streamlit_nightly-1.35.1.dev20240528/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-29 07:26:31.000000 streamlit_nightly-1.35.1.dev20240528/tests/testutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.565821 streamlit_nightly-1.35.1.dev20240529/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-30 06:54:39.565821 streamlit_nightly-1.35.1.dev20240529/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.441820 streamlit_nightly-1.35.1.dev20240529/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/bin/streamlit.cmd
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:54:39.565821 streamlit_nightly-1.35.1.dev20240529/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.445820 streamlit_nightly-1.35.1.dev20240529/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/case_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/cli_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/code_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/color_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/column_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/execution_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/experimental_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12997 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/commands/page_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/components/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/lib/local_component_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/base_component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/base_custom_component.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/component_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/component_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9320 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/custom_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43657 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11469 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/config_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/config_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.449820 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/snowflake_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/snowpark_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12234 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/sql_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/connections/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/delta_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/deprecation_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/development.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/echo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.457820 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27609 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/balloons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/bokeh_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/deck_gl_json_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8020 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/dialog_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/doc_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12079 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4887 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/graphviz_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11268 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/iframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28251 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/layouts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.461820 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30696 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/built_in_chart_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17374 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/column_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/dicttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6634 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/mutable_status_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/pandas_styler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8307 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/streamlit_plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/subtitle_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16638 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29678 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19229 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/plotly_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/snow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/toast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69887 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/vega_charts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.461820 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9184 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/camera_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14327 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36465 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/data_editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17699 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/multiselect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18079 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/number_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/radio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/select_slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11717 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/selectbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26704 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/slider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22376 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/text_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30085 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/time_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20804 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/elements/write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73749 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/emojis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/env_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/error_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.465820 streamlit_nightly-1.35.1.dev20240529/streamlit/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.465820 streamlit_nightly-1.35.1.dev20240529/streamlit/external/langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/external/langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15280 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/external/langchain/streamlit_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/file_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/folder_black_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/git_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.465820 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/Hello.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.465820 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/0_Animation_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/1_Plotting_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/2_Mapping_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/3_DataFrame_Demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/hello/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/js_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57136 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/material_icon_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/net_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.493820 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Alert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Alert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AppPage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AppPage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowNamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowNamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowVegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowVegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Arrow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Arrow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Audio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Audio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AutoRerun_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AutoRerun_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BackMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BackMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Balloons_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Balloons_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Block_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12049 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Block_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BokehChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BokehChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Button_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Button_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/CameraInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/CameraInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ChatInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ChatInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Checkbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Checkbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ClientState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ClientState_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Code_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Code_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ColorPicker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ColorPicker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Components_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DataFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15040 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DataFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DateInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DateInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DeckGlJsonChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DeckGlJsonChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Delta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Delta_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DocString_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DocString_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DownloadButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DownloadButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10146 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Element_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16972 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Element_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Empty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Empty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Exception_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Exception_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Favicon_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Favicon_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/FileUploader_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/FileUploader_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ForwardMsg_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12304 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ForwardMsg_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GitInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GitInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GraphVizChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GraphVizChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Heading_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Heading_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Html_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Html_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/IFrame_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/IFrame_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Json_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Json_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LabelVisibilityMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LabelVisibilityMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LinkButton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LinkButton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Logo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Logo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Markdown_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Markdown_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Metric_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4041 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Metric_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/MultiSelect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/MultiSelect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NamedDataSet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NamedDataSet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NewSession_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18437 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NewSession_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NumberInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NumberInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageConfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageConfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageInfo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageInfo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageLink_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageLink_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageNotFound_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageNotFound_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageProfile_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageProfile_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PagesChanged_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PagesChanged_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ParentMessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ParentMessage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PlotlyChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PlotlyChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Progress_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Progress_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Radio_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Radio_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/RootContainer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/RootContainer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Selectbox_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Selectbox_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionEvent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionEvent_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionStatus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Skeleton_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Skeleton_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Slider_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6044 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Slider_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Snow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Snow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Spinner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Spinner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextArea_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextArea_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Text_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Text_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TimeInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TimeInput_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Toast_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Toast_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/VegaLiteChart_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/VegaLiteChart_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Video_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Video_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/WidgetStates_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6240 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/WidgetStates_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/openmetrics_data_model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-05-30 06:50:55.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/proto/openmetrics_data_model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.497820 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36663 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/app_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.497820 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_data_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18329 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17358 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cached_message_replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18986 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/legacy_cache_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.501820 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/cache_storage_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/dummy_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/local_disk_cache_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/connection_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11500 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9805 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/forward_msg_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/forward_msg_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12029 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8510 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/media_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_media_file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_session_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4422 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14329 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/metrics_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29318 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/runtime_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.501820 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/magic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/magic_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_run_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13017 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.501820 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7192 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/query_params_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5169 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/safe_session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27500 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/session_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/session_state_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/uploaded_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/websocket_session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5749 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/source_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.501820 streamlit_nightly-1.35.1.dev20240529/streamlit/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    14353 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-30 06:51:24.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.437820 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.505820 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    33275 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/3466.8b8f33d6.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/5441.e3b876c5.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12090 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/8148.49dfd2ce.chunk.css
+-rw-r--r--   0 runner    (1001) docker     (127)    29246 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/main.3aaaea00.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.537820 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     5446 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1074.73973756.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15023 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1168.14f7c6ff.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1307.0f0cca93.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1451.3b0a3e31.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9618 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1479.6709db03.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/178.7bea8c5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1792.8bd6ce2a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33075 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2178.90362aae.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32468 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2187.9469f035.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2469.09ea79bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2634.1249dc7a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65522 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2736.4336e2b9.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3053.7e70ec3b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3637630 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/329.464ed8ec.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3301.1d1b10bb.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2306325 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3466.05d62820.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3513.7dedbda2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4113.99983645.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4132.49bf3f2c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4132.49bf3f2c.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4177.69f9f18d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4319.bf1c86bf.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4477.1bd49702.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4500.b6f348d1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14830 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4666.c4b22a63.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/474.7eb0c6cd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5106.44f0ff51.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    21681 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5117.04bfe5d3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  2263616 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5249.f2f4070d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15117 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5345.73d26e5d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5379.f08eddd1.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5441.1b94928f.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   107585 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5791.9a42fb4b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11449 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6013.4ba2d616.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6405.ac5a6f23.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24494 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6718.802da17e.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6853.93dd1c4c.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)   398809 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6950.70fe55c2.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6950.70fe55c2.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    88545 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7142.83028745.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7175.583ff733.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  3388121 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7323.b74cc85b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   936700 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7483.64f23be7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7483.64f23be7.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7602.e8abc06b.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7805.acc6316a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8005.43974a35.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    51165 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8148.293984e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8427.bd0a7cf3.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8477.de889fe5.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15493 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8492.0d93bd08.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8536.f8de3d9a.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12214 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8570.6de19120.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8691.4211c305.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9330.2b4c99e0.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13574 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9336.3e046ad7.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20791 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/937.a1248039.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/937.a1248039.chunk.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    22113 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9656.8c935274.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9865.fd93213d.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)  4405383 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/main.206766ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/main.206766ee.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.553820 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   247332 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74492 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    63060 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62096 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74052 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    74132 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    62988 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    76860 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44640 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44748 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77664 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    77452 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    44608 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72892 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30756 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29384 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    68356 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    72668 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    30628 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/checkmark.29851c8e9e6ef0c3d6c1e4efe3c1bb9e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   101906 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    73528 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    86179 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92182 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    39315 2024-05-30 06:54:36.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/temporary_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.553820 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36577 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/app_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59854 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/element_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/local_script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48389 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/url_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/user_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6379 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/ipython/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/ipython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/ipython/modified_sys_path.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/pympler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/pympler/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    87925 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/pympler/asizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13980 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/event_based_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/local_sources_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/polling_path_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5203 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.557820 streamlit_nightly-1.35.1.dev20240529/streamlit/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14233 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/cache_storage_manager_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.561821 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/app_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/browser_websocket_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/component_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/media_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14834 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/server_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/stats_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/upload_file_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/websocket_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.561821 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23268 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:50:51.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 06:54:38.000000 streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:54:39.561821 streamlit_nightly-1.35.1.dev20240529/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-05-30 06:49:17.000000 streamlit_nightly-1.35.1.dev20240529/tests/testutil.py
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240529/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.35.1.dev20240528
+Version: 1.35.1.dev20240529
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/bin/streamlit.cmd` & `streamlit_nightly-1.35.1.dev20240529/bin/streamlit.cmd`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/setup.py` & `streamlit_nightly-1.35.1.dev20240529/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 
 THIS_DIRECTORY = Path(__file__).parent
 
-VERSION = "1.35.1.dev20240528"  # PEP-440
+VERSION = "1.35.1.dev20240529"  # PEP-440
 
 # IMPORTANT: We should try very hard *not* to add dependencies to Streamlit.
 # And if you do add one, make the required version as general as possible:
 # - Include relevant lower bound for any features we use from our dependencies
 # - Always include the lower bound as >= VERSION, to keep testing min versions easy
 # - And include an upper bound that's < NEXT_MAJOR_VERSION
 INSTALL_REQUIRES = [
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/__main__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/__main__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/case_converters.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/case_converters.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/cli_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/cli_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/code_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/code_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/color_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/color_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/column_config.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/column_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/commands/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/commands/execution_control.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/commands/execution_control.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/commands/experimental_query_params.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/commands/experimental_query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/commands/logo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/commands/logo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/commands/page_config.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/commands/page_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/lib/local_component_registry.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/lib/local_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/base_component_registry.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/base_component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/types/base_custom_component.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/types/base_custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/component_arrow.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/component_arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/component_registry.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/component_registry.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/components.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/components.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/components/v1/custom_component.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/components/v1/custom_component.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/config.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/config_option.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/config_option.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/config_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/config_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/base_connection.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/base_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/snowflake_connection.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/snowpark_connection.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/snowpark_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/sql_connection.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/sql_connection.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/connections/util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/connections/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/constants.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/constants.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/cursor.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/cursor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/delta_generator.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/delta_generator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/deprecation_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/deprecation_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/development.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/development.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/echo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/echo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/alert.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/alert.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/arrow.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/arrow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/balloons.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/balloons.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/bokeh_chart.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/bokeh_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/code.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/code.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/deck_gl_json_chart.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/deck_gl_json_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/dialog_decorator.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/dialog_decorator.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/doc_string.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/doc_string.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/empty.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/empty.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from streamlit.runtime.metrics_util import gather_metrics
 
 if TYPE_CHECKING:
     from streamlit.delta_generator import DeltaGenerator
 
 
 class EmptyMixin:
+    @gather_metrics("empty")
     def empty(self) -> DeltaGenerator:
         """Insert a single-element container.
 
         Inserts a container into your app that can be used to hold a single element.
         This allows you to, for example, remove elements at any point, or replace
         several elements at once (using a child multi-element container).
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/exception.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/exception.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/form.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/form.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/graphviz_chart.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/graphviz_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/heading.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/heading.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/html.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/html.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/iframe.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/iframe.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/image.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/image.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/json.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/json.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/layouts.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/layouts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/built_in_chart_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/built_in_chart_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/column_config_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/column_config_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/column_types.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/column_types.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/dialog.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/dialog.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/dicttools.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/dicttools.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/event_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/event_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/mutable_status_container.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/mutable_status_container.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/pandas_styler_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/pandas_styler_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/policies.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/policies.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/streamlit_plotly_theme.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/streamlit_plotly_theme.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/subtitle_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/subtitle_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/lib/utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/lib/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/map.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/map.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/markdown.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/markdown.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/media.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/media.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/metric.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/metric.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/plotly_chart.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/progress.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/progress.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/pyplot.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/pyplot.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/snow.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/snow.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/spinner.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/spinner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/text.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/text.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/toast.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/toast.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/vega_charts.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/vega_charts.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/button.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/button.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/camera_input.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/camera_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/chat.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/chat.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/checkbox.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/color_picker.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/color_picker.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/data_editor.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/data_editor.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/file_uploader.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/file_uploader.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/multiselect.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/multiselect.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/number_input.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/number_input.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/radio.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/radio.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/select_slider.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/select_slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/selectbox.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/selectbox.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/slider.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/text_widgets.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/text_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/widgets/time_widgets.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/widgets/time_widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/elements/write.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/elements/write.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/emojis.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/emojis.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/env_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/env_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/error_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/error_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/errors.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/external/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/external/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/external/langchain/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/external/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/external/langchain/streamlit_callback_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/external/langchain/streamlit_callback_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/file_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/file_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/folder_black_list.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/folder_black_list.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/git_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/git_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/Hello.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/Hello.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/0_Animation_Demo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/0_Animation_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/1_Plotting_Demo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/1_Plotting_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/2_Mapping_Demo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/2_Mapping_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/pages/3_DataFrame_Demo.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/pages/3_DataFrame_Demo.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/hello/utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/hello/utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/js_number.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/js_number.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/logger.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/logger.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/material_icon_names.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/material_icon_names.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/net_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/net_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/platform.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/platform.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Alert_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Alert_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Alert_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AppPage_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AppPage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AppPage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AppPage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowNamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowNamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowNamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowNamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowVegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowVegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ArrowVegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ArrowVegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Arrow_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Arrow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Arrow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Arrow_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -99,17 +99,17 @@
     SELECTION_MODE_FIELD_NUMBER: builtins.int
     data: builtins.bytes
     """The serialized arrow dataframe"""
     @property
     def styler(self) -> global___Styler:
         """Pandas styler information"""
     width: builtins.int
-    """Width in CSS points"""
+    """Width in pixels"""
     height: builtins.int
-    """Height in CSS points"""
+    """Height in pixels"""
     use_container_width: builtins.bool
     """If True, will overwrite the dataframe width to fit to container."""
     id: builtins.str
     """The id of the widget, this is required if the dataframe is editable"""
     columns: builtins.str
     """Column configuration as JSON"""
     editing_mode: global___Arrow.EditingMode.ValueType
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Audio_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Audio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Audio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Audio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AutoRerun_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AutoRerun_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/AutoRerun_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/AutoRerun_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BackMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BackMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BackMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BackMsg_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Balloons_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Balloons_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Balloons_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Balloons_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Block_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Block_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Block_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BokehChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BokehChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/BokehChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/BokehChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Button_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Button_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Button_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Button_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/CameraInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/CameraInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/CameraInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/CameraInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ChatInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ChatInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ChatInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ChatInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Checkbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Checkbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Checkbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Checkbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ClientState_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ClientState_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ClientState_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ClientState_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Code_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Code_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Code_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ColorPicker_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ColorPicker_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ColorPicker_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ColorPicker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Common_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Common_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Common_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Components_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Components_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Components_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Components_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DataFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DataFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DataFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DataFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DateInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DateInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DateInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DateInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DeckGlJsonChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DeckGlJsonChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DeckGlJsonChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DeckGlJsonChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Delta_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Delta_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Delta_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Delta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DocString_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DocString_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DocString_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DocString_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DownloadButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DownloadButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/DownloadButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/DownloadButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Element_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Element_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Element_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Element_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Empty_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Empty_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Empty_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Empty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Exception_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Exception_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Exception_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Exception_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Favicon_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Favicon_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Favicon_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Favicon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/FileUploader_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/FileUploader_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/FileUploader_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/FileUploader_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ForwardMsg_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ForwardMsg_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ForwardMsg_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ForwardMsg_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -221,17 +221,17 @@
     """
 
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     WIDTH_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
     width: builtins.int
-    """width in CSS points"""
+    """width in pixels"""
     height: builtins.int
-    """height in CSS points"""
+    """height in pixels"""
     def __init__(
         self,
         *,
         width: builtins.int = ...,
         height: builtins.int = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["height", b"height", "width", b"width"]) -> None: ...
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GitInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GitInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GitInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GitInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GraphVizChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GraphVizChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/GraphVizChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/GraphVizChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Heading_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Heading_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Heading_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Heading_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Html_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Html_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Html_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Html_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/IFrame_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/IFrame_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/IFrame_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/IFrame_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Image_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Image_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Image_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Json_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Json_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Json_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Json_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LabelVisibilityMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LabelVisibilityMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LabelVisibilityMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LabelVisibilityMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LinkButton_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LinkButton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/LinkButton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/LinkButton_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Logo_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Logo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Logo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Logo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Markdown_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Markdown_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Markdown_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Markdown_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Metric_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Metric_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Metric_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Metric_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/MultiSelect_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/MultiSelect_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/MultiSelect_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/MultiSelect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NamedDataSet_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NamedDataSet_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NamedDataSet_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NamedDataSet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NewSession_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NewSession_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NewSession_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NewSession_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NumberInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NumberInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/NumberInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/NumberInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageConfig_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageConfig_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageConfig_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageConfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageInfo_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageInfo_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageInfo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageLink_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageLink_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageLink_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageLink_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageNotFound_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageNotFound_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageNotFound_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageNotFound_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageProfile_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageProfile_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PageProfile_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PageProfile_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PagesChanged_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PagesChanged_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PagesChanged_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PagesChanged_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ParentMessage_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ParentMessage_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/ParentMessage_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/ParentMessage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PlotlyChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PlotlyChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/PlotlyChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/PlotlyChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Progress_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Progress_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Progress_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Progress_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Radio_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Radio_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Radio_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Radio_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/RootContainer_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/RootContainer_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/RootContainer_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/RootContainer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Selectbox_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Selectbox_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Selectbox_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Selectbox_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionEvent_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionEvent_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionEvent_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionEvent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionStatus_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/SessionStatus_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/SessionStatus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Skeleton_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Skeleton_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Skeleton_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Skeleton_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     """internal-only, for now"""
 
     STYLE_FIELD_NUMBER: builtins.int
     HEIGHT_FIELD_NUMBER: builtins.int
     style: global___Skeleton.SkeletonStyle.ValueType
     """Skeleton visual style"""
     height: builtins.int
-    """Height in CSS points"""
+    """Height in pixels"""
     def __init__(
         self,
         *,
         style: global___Skeleton.SkeletonStyle.ValueType = ...,
         height: builtins.int | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["_height", b"_height", "height", b"height"]) -> builtins.bool: ...
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Slider_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Slider_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Slider_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Slider_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Snow_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Snow_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Snow_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Snow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Spinner_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Spinner_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Spinner_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Spinner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextArea_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextArea_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextArea_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextArea_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TextInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TextInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Text_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Text_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Text_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Text_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TimeInput_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TimeInput_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/TimeInput_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/TimeInput_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Toast_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Toast_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Toast_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Toast_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/VegaLiteChart_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/VegaLiteChart_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/VegaLiteChart_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/VegaLiteChart_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Video_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Video_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/Video_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/Video_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/WidgetStates_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/WidgetStates_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/WidgetStates_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/WidgetStates_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/openmetrics_data_model_pb2.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/openmetrics_data_model_pb2.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/proto/openmetrics_data_model_pb2.pyi` & `streamlit_nightly-1.35.1.dev20240529/streamlit/proto/openmetrics_data_model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/app_session.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/app_session.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_data_api.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_data_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_errors.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_errors.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_resource_api.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_resource_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_type.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_type.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cache_utils.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cache_utils.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/cached_message_replay.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/cached_message_replay.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/hashing.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/hashing.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/legacy_cache_api.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/legacy_cache_api.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/cache_storage_protocol.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/cache_storage_protocol.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/dummy_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/dummy_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/in_memory_cache_storage_wrapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/caching/storage/local_disk_cache_storage.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/caching/storage/local_disk_cache_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/connection_factory.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/connection_factory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/credentials.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/credentials.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/forward_msg_cache.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/forward_msg_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/forward_msg_queue.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/forward_msg_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/fragment.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/fragment.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/media_file_manager.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/media_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_media_file_storage.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_media_file_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_session_storage.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_session_storage.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/memory_uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/memory_uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/metrics_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/metrics_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,18 @@
     "vllm",
     "alpa",
     "jinaai",
     "guidance",
     "litellm",
     "comet_llm",
     "instructor",
+    "xgboost",
+    "lightgbm",
+    "catboost",
+    "sklearn",
     # Workflow Tools:
     "prefect",
     "luigi",
     "airflow",
     "dagster",
     # Vector Stores:
     "pgvector",
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/runtime.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/runtime.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/runtime_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/runtime_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/script_data.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/script_data.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/magic.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/magic.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/magic_funcs.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/magic_funcs.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_cache.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_cache.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_requests.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_requests.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_run_context.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_run_context.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/scriptrunner/script_runner.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/scriptrunner/script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/secrets.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/secrets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/session_manager.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/common.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/common.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/query_params.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/query_params.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/query_params_proxy.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/query_params_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/safe_session_state.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/safe_session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/session_state.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/session_state.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/session_state_proxy.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/session_state_proxy.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/state/widgets.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/state/widgets.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/stats.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/stats.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/uploaded_file_manager.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/uploaded_file_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/runtime/websocket_session_manager.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/runtime/websocket_session_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/source_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/source_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/asset-manifest.json` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/favicon.png` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/index.html` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/3466.8b8f33d6.chunk.css` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/3466.8b8f33d6.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/5441.e3b876c5.chunk.css` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/5441.e3b876c5.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/8148.49dfd2ce.chunk.css` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/8148.49dfd2ce.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/css/main.3aaaea00.css` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/css/main.3aaaea00.css`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1074.73973756.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1074.73973756.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1168.14f7c6ff.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1168.14f7c6ff.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1307.0f0cca93.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1307.0f0cca93.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1451.3b0a3e31.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1451.3b0a3e31.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1479.6709db03.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1479.6709db03.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/178.7bea8c5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/178.7bea8c5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/1792.8bd6ce2a.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/1792.8bd6ce2a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2178.90362aae.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2178.90362aae.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2187.9469f035.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2187.9469f035.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2469.09ea79bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2469.09ea79bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2634.1249dc7a.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2634.1249dc7a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/2736.4336e2b9.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/2736.4336e2b9.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3053.7e70ec3b.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3053.7e70ec3b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/329.464ed8ec.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/329.464ed8ec.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/329.464ed8ec.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3301.1d1b10bb.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3301.1d1b10bb.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3466.05d62820.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3466.05d62820.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3466.05d62820.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/3513.7dedbda2.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/3513.7dedbda2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4113.99983645.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4113.99983645.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4132.49bf3f2c.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4132.49bf3f2c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4177.69f9f18d.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4177.69f9f18d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4319.bf1c86bf.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4319.bf1c86bf.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4477.1bd49702.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4477.1bd49702.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4500.b6f348d1.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4500.b6f348d1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/4666.c4b22a63.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/4666.c4b22a63.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/474.7eb0c6cd.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/474.7eb0c6cd.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5106.44f0ff51.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5106.44f0ff51.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5117.04bfe5d3.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5117.04bfe5d3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5249.f2f4070d.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5249.f2f4070d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5345.73d26e5d.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5345.73d26e5d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5379.f08eddd1.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5379.f08eddd1.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5441.1b94928f.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5441.1b94928f.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/5791.9a42fb4b.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/5791.9a42fb4b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6013.4ba2d616.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6013.4ba2d616.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6405.ac5a6f23.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6405.ac5a6f23.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6718.802da17e.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6718.802da17e.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6853.93dd1c4c.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6853.93dd1c4c.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/6950.70fe55c2.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/6950.70fe55c2.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7142.83028745.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7142.83028745.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7175.583ff733.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7175.583ff733.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7323.b74cc85b.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7323.b74cc85b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7323.b74cc85b.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7483.64f23be7.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7483.64f23be7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7602.e8abc06b.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7602.e8abc06b.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/7805.acc6316a.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/7805.acc6316a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8005.43974a35.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8005.43974a35.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8148.293984e0.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8148.293984e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8427.bd0a7cf3.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8427.bd0a7cf3.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8477.de889fe5.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8477.de889fe5.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8492.0d93bd08.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8492.0d93bd08.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8536.f8de3d9a.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8536.f8de3d9a.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8570.6de19120.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8570.6de19120.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/8691.4211c305.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/8691.4211c305.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9330.2b4c99e0.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9330.2b4c99e0.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9336.3e046ad7.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9336.3e046ad7.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/937.a1248039.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/937.a1248039.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9656.8c935274.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9656.8c935274.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/9865.fd93213d.chunk.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/9865.fd93213d.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/main.206766ee.js` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/main.206766ee.js`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/js/main.206766ee.js.LICENSE.txt` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/js/main.206766ee.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.73ea273a72f4aca30ca5.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.853be92419a6c3766b9a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_AMS-Regular.d562e886c52f12660a41.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.7489a2fbfb9bfe704420.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.a1abf90dfd72792a577a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Bold.d757c535a2e5902f1325.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.7e873d3833eb108a0758.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.d6484fce1ef428d5bd94.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Caligraphic-Regular.db074fa22cf224af93d7.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.354501bac435c3264834.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.4c761b3711973ab04edf.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Bold.931d67ea207ab37ee693.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.172d3529b26f8cedef6b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.6fdf0ac577be0ba82a4c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Fraktur-Regular.ed305b5434865e06ffde.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.0c3b8929d377c0e9b2f3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.39890742bc957b368704.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Bold.8169508bf58f8bd92ad8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.20f389c4120be058d80a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.428978dc7837d46de091.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-BoldItalic.828abcb200061cffbaae.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fa675e5e4bec9eb250b6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fd947498bc16392e76c2.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Italic.fe2176f79edaa716e621.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.4f35fbcc9ee8614c2bcc.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.9eba1d77abcf2aa6e94e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Main-Regular.f650f111a3b890d116f1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.3f07ed67f06c720120ce.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.bf2d440b3a42ea78a998.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-BoldItalic.dcbcbd93bac0470b462d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.6d3d25f4820d0da8f01f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.8a5f936332e8028c7278.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Math-Italic.96759856b4e70f3a8338.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.5b49f4993ae22d7975b4.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.95591a929f0d32aa282a.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Bold.b9cd458ac6d5889ff9c3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.7d393d382f3e7fb1c637.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.8d593cfaa96238d5e2f8.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Italic.b257a18c016f37ee4543.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.02271ec5cb9f5b4588ac.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.2f7bc363fc5424ebda59.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_SansSerif-Regular.cd5e231e0cc53b2cb2c0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.073b3402d036714b4370.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.c81d1b2a4b75d3eded60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Script-Regular.fc9ba5249878cd8f8d88.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.0108e89c9003e8c14ea3.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.6de7d4b539221a49e9e2.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size1-Regular.6eec866c69313624be60.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.2960900c4f271311eb36.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.3a99e70aee4076660d38.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size2-Regular.57f5c1837853986ea1db.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.7947224e8a9914fa332b.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.8d6b6822586eea3d3b20.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size3-Regular.e1951519f6f0596f7356.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.4ad7c7e8bb8d10a34bb7.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.aeffd8025cba3647f1a6.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Size4-Regular.e418bf257af1052628d8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.4c6b94fd1d07f8beff7c.woff`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.c295e7f71970f03c0549.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/KaTeX_Typewriter-Regular.c5c02d763c89380dcb4e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/MaterialSymbols-Outlined.909d2dce4aba724ad02f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Bold.17a68a0751a813474a0e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-BoldItalic.d45b7a3df103d441d78b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Italic.ec122a420df4175e74f2.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-Regular.84b900b88d09398d86b0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-SemiBold.17291d1c493cb25eb2c3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceCodePro-SemiBoldItalic.f879ae27307c3926522b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Bold.118dea98980e20a81ced.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-BoldItalic.1d664be59d2eb5fef029.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Italic.8a9bfea74d43927d6eec.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-Regular.0d69e5ff5e92ac64a0c9.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-SemiBold.abed79cd0df1827e18cf.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSansPro-SemiBoldItalic.befb0a2824eabc5ce36b.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Bold.d7975b56594770699ae0.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-BoldItalic.913697a7178b128caa4c.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Italic.d3529cb5797663ac5d88.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-Regular.e6c37aa3926474cc93e1.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-SemiBold.5c1d378dd5990ef334ca.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/SourceSerifPro-SemiBoldItalic.249e948b885d0c7d30a8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/fireworks.0906f02ea43f1018a6d2.gif`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-0.beded754e8024c73d9d2.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-1.8077dc154e0bf900aa73.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/flake-2.e3f07d06933dd0e84c24.png`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/logo.83ae4f2fb87e38be7cbb8a5d2beb64d2.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg` & `streamlit_nightly-1.35.1.dev20240529/streamlit/static/static/media/rocket.b75b17d2b0a063c6cea230d1a9d77f1e.svg`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/string_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/string_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/temporary_directory.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/temporary_directory.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/app_test.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/app_test.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/element_tree.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/element_tree.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/local_script_runner.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/local_script_runner.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/testing/v1/util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/testing/v1/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/time_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/time_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/type_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/type_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/url_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/url_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/user_info.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/user_info.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/ipython/modified_sys_path.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/ipython/modified_sys_path.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/vendor/pympler/asizeof.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/vendor/pympler/asizeof.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/version.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/version.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/event_based_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/event_based_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/local_sources_watcher.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/local_sources_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/path_watcher.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/polling_path_watcher.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/polling_path_watcher.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/watcher/util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/watcher/util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/bootstrap.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/bootstrap.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/cache_storage_manager_config.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/cache_storage_manager_config.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/cli.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/cli.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/__init__.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/app_static_file_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/app_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/browser_websocket_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/browser_websocket_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/component_request_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/component_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/media_file_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/media_file_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/routes.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/routes.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/server.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/server.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/server_util.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/server_util.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/stats_request_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/stats_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/upload_file_request_handler.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/upload_file_request_handler.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit/web/server/websocket_headers.py` & `streamlit_nightly-1.35.1.dev20240529/streamlit/web/server/websocket_headers.py`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/PKG-INFO` & `streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-nightly
-Version: 1.35.1.dev20240528
+Version: 1.35.1.dev20240529
 Summary: A faster way to build and share data apps
 Home-page: https://streamlit.io
 Author: Snowflake Inc
 Author-email: hello@streamlit.io
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/streamlit/streamlit
 Project-URL: Bug Tracker, https://github.com/streamlit/streamlit/issues
```

### Comparing `streamlit_nightly-1.35.1.dev20240528/streamlit_nightly.egg-info/SOURCES.txt` & `streamlit_nightly-1.35.1.dev20240529/streamlit_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamlit_nightly-1.35.1.dev20240528/tests/testutil.py` & `streamlit_nightly-1.35.1.dev20240529/tests/testutil.py`

 * *Files identical despite different names*

