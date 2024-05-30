# Comparing `tmp/asposecellscloud-24.3.tar.gz` & `tmp/asposecellscloud-24.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asposecellscloud-24.3.tar", last modified: Fri Mar 22 07:34:35 2024, max compression
+gzip compressed data, was "asposecellscloud-24.4.tar", last modified: Sun Apr 28 05:59:29 2024, max compression
```

## Comparing `asposecellscloud-24.3.tar` & `asposecellscloud-24.4.tar`

### file list

```diff
@@ -1,795 +1,805 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:35.436655 asposecellscloud-24.3/
--rw-rw-rw-   0        0        0     1090 2024-01-16 20:47:48.000000 asposecellscloud-24.3/LICENSE
--rw-rw-rw-   0        0        0    17451 2024-03-22 07:34:35.415575 asposecellscloud-24.3/PKG-INFO
--rw-rw-rw-   0        0        0    16471 2024-03-22 07:23:40.000000 asposecellscloud-24.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:21.498364 asposecellscloud-24.3/asposecellscloud/
--rw-rw-rw-   0        0        0    63889 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/__init__.py
--rw-rw-rw-   0        0        0    30582 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/api_client.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:21.620364 asposecellscloud-24.3/asposecellscloud/apis/
--rw-rw-rw-   0        0        0      128 2023-12-23 14:58:26.000000 asposecellscloud-24.3/asposecellscloud/apis/__init__.py
--rw-rw-rw-   0        0        0   811615 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/apis/cells_api.py
--rw-rw-rw-   0        0        0     8822 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/configuration.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:29.497044 asposecellscloud-24.3/asposecellscloud/models/
--rw-rw-rw-   0        0        0    29734 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/__init__.py
--rw-rw-rw-   0        0        0     5492 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/above_average.py
--rw-rw-rw-   0        0        0     6246 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/abstract_calculation_engine.py
--rw-rw-rw-   0        0        0     5645 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/abstract_calculation_monitor.py
--rw-rw-rw-   0        0        0    10538 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/access_token_response.py
--rw-rw-rw-   0        0        0     5581 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyze_excel_request.py
--rw-rw-rw-   0        0        0     4463 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyze_excel_response.py
--rw-rw-rw-   0        0        0     8098 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyze_suggestion.py
--rw-rw-rw-   0        0        0     9168 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyzed_column_description.py
--rw-rw-rw-   0        0        0     6461 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyzed_result.py
--rw-rw-rw-   0        0        0    13139 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/analyzed_table_description.py
--rw-rw-rw-   0        0        0    26547 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/arc_shape.py
--rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/arc_shape_response.py
--rw-rw-rw-   0        0        0     7072 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/area.py
--rw-rw-rw-   0        0        0     6264 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_filter.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_filter_response.py
--rw-rw-rw-   0        0        0     8740 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/auto_fitter_options.py
--rw-rw-rw-   0        0        0    22619 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_shape.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_shape_response.py
--rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_shapes.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/auto_shapes_response.py
--rw-rw-rw-   0        0        0    23440 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/axis.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/axis_response.py
--rw-rw-rw-   0        0        0     9433 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/batch_convert_request.py
--rw-rw-rw-   0        0        0     7012 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/batch_lock_request.py
--rw-rw-rw-   0        0        0     7596 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/batch_protect_request.py
--rw-rw-rw-   0        0        0     8849 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/batch_split_request.py
--rw-rw-rw-   0        0        0     6224 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/border.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/border_response.py
--rw-rw-rw-   0        0        0    22601 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/button.py
--rw-rw-rw-   0        0        0     5102 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/button_response.py
--rw-rw-rw-   0        0        0     5176 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/calculate_formula_response.py
--rw-rw-rw-   0        0        0     7951 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/calculation_options.py
--rw-rw-rw-   0        0        0    11535 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cell.py
--rw-rw-rw-   0        0        0     5762 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cell_area.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cell_response.py
--rw-rw-rw-   0        0        0     6464 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cell_value.py
--rw-rw-rw-   0        0        0     6932 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells.py
--rw-rw-rw-   0        0        0     5537 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_cloud_file_info.py
--rw-rw-rw-   0        0        0     5253 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_cloud_file_info_response.py
--rw-rw-rw-   0        0        0     4726 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_cloud_response.py
--rw-rw-rw-   0        0        0     7495 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_color.py
--rw-rw-rw-   0        0        0     4670 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_document_properties.py
--rw-rw-rw-   0        0        0     5458 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_document_properties_response.py
--rw-rw-rw-   0        0        0     6769 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_document_property.py
--rw-rw-rw-   0        0        0     5410 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_document_property_response.py
--rw-rw-rw-   0        0        0    22637 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_drawing.py
--rw-rw-rw-   0        0        0     5144 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_drawing_response.py
--rw-rw-rw-   0        0        0     5840 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_object_operate_task_parameter.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/cells_response.py
--rw-rw-rw-   0        0        0    26326 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart.py
--rw-rw-rw-   0        0        0     9800 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_area.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_area_response.py
--rw-rw-rw-   0        0        0     8702 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_data_table.py
--rw-rw-rw-   0        0        0     5343 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_data_table_response.py
--rw-rw-rw-   0        0        0     9806 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_frame.py
--rw-rw-rw-   0        0        0     3982 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_globalization_settings.py
--rw-rw-rw-   0        0        0    10280 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_operate_parameter.py
--rw-rw-rw-   0        0        0     7723 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_point.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_point_response.py
--rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_points.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_points_response.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_response.py
--rw-rw-rw-   0        0        0    22625 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/chart_shape.py
--rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/charts.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/charts_response.py
--rw-rw-rw-   0        0        0    23958 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/check_box.py
--rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/check_box_response.py
--rw-rw-rw-   0        0        0     5170 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/color.py
--rw-rw-rw-   0        0        0     6656 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/color_filter.py
--rw-rw-rw-   0        0        0     5543 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/color_filter_request.py
--rw-rw-rw-   0        0        0     6692 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/color_scale.py
--rw-rw-rw-   0        0        0     6405 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/column.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/column_response.py
--rw-rw-rw-   0        0        0     5789 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/columns.py
--rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/columns_response.py
--rw-rw-rw-   0        0        0    25729 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/combo_box.py
--rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/combo_box_response.py
--rw-rw-rw-   0        0        0     9830 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comment.py
--rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comment_response.py
--rw-rw-rw-   0        0        0    23076 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comment_shape.py
--rw-rw-rw-   0        0        0     5178 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comment_shape_response.py
--rw-rw-rw-   0        0        0     4782 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comments.py
--rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/comments_response.py
--rw-rw-rw-   0        0        0     5346 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formatting.py
--rw-rw-rw-   0        0        0     5232 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_icon.py
--rw-rw-rw-   0        0        0     5495 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_response.py
--rw-rw-rw-   0        0        0     5171 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_value.py
--rw-rw-rw-   0        0        0     5527 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formattings.py
--rw-rw-rw-   0        0        0     5519 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/conditional_formattings_response.py
--rw-rw-rw-   0        0        0     4697 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/convert_parameter.py
--rw-rw-rw-   0        0        0     5919 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/convert_task_parameter.py
--rw-rw-rw-   0        0        0     7848 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/convert_worksheet_task_parameter.py
--rw-rw-rw-   0        0        0     8164 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/copy_options.py
--rw-rw-rw-   0        0        0     7769 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/create_pivot_table_request.py
--rw-rw-rw-   0        0        0     4404 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/criteria_multiple_filter.py
--rw-rw-rw-   0        0        0     4994 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/custom_filter.py
--rw-rw-rw-   0        0        0     5477 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/custom_parser_config.py
--rw-rw-rw-   0        0        0     9798 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_bar.py
--rw-rw-rw-   0        0        0     4681 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_bar_border.py
--rw-rw-rw-   0        0        0     5342 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_cleansing.py
--rw-rw-rw-   0        0        0     6569 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_cleansing_request.py
--rw-rw-rw-   0        0        0     5028 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_column_fill_value.py
--rw-rw-rw-   0        0        0     6701 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_deduplication_request.py
--rw-rw-rw-   0        0        0     5793 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_fill.py
--rw-rw-rw-   0        0        0     6449 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_fill_request.py
--rw-rw-rw-   0        0        0     6633 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/data_fill_value.py
--rw-rw-rw-   0        0        0    20157 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_labels.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_labels_response.py
--rw-rw-rw-   0        0        0     6951 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_sorter.py
--rw-rw-rw-   0        0        0     6436 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/data_sorter_key.py
--rw-rw-rw-   0        0        0     6974 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/date_time_group_item.py
--rw-rw-rw-   0        0        0     4999 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/deduplication_region.py
--rw-rw-rw-   0        0        0     6474 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/delete_incomplete_rows_request.py
--rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/dif_save_options.py
--rw-rw-rw-   0        0        0     7488 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/digital_signature.py
--rw-rw-rw-   0        0        0     4823 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/disc_usage.py
--rw-rw-rw-   0        0        0     6486 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/discover_chart.py
--rw-rw-rw-   0        0        0     7470 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/discover_pivot_table.py
--rw-rw-rw-   0        0        0    13288 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/display_unit_label.py
--rw-rw-rw-   0        0        0     5391 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/display_unit_label_response.py
--rw-rw-rw-   0        0        0    20165 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/docx_save_options.py
--rw-rw-rw-   0        0        0     5049 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/drop_bars.py
--rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/drop_bars_response.py
--rw-rw-rw-   0        0        0     5396 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/dynamic_filter.py
--rw-rw-rw-   0        0        0     3856 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/error.py
--rw-rw-rw-   0        0        0    16604 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/error_bar.py
--rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/error_bar_response.py
--rw-rw-rw-   0        0        0     3898 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/error_details.py
--rw-rw-rw-   0        0        0     5197 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/excel_data_statistics.py
--rw-rw-rw-   0        0        0     5299 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/file_info.py
--rw-rw-rw-   0        0        0     4930 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/file_source.py
--rw-rw-rw-   0        0        0     6978 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/file_version.py
--rw-rw-rw-   0        0        0     4307 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/file_versions.py
--rw-rw-rw-   0        0        0     4289 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/files_list.py
--rw-rw-rw-   0        0        0     4298 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/files_result.py
--rw-rw-rw-   0        0        0     4802 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/files_upload_result.py
--rw-rw-rw-   0        0        0     6819 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/fill_format.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/fill_format_response.py
--rw-rw-rw-   0        0        0     8728 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/filter_column.py
--rw-rw-rw-   0        0        0     5574 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/find_response.py
--rw-rw-rw-   0        0        0     7493 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/floor.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/floor_response.py
--rw-rw-rw-   0        0        0     8450 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/font.py
--rw-rw-rw-   0        0        0     6086 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/font_setting.py
--rw-rw-rw-   0        0        0    31682 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/form.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/form_response.py
--rw-rw-rw-   0        0        0    10606 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/format_condition.py
--rw-rw-rw-   0        0        0     4713 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/forms.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/forms_response.py
--rw-rw-rw-   0        0        0     5300 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/formula_format_condition.py
--rw-rw-rw-   0        0        0    10839 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/formula_settings.py
--rw-rw-rw-   0        0        0     7330 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/globalization_settings.py
--rw-rw-rw-   0        0        0     6562 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/google_drive_storage_file.py
--rw-rw-rw-   0        0        0     5876 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/gradient_fill.py
--rw-rw-rw-   0        0        0     5287 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/gradient_fill_stop.py
--rw-rw-rw-   0        0        0    23028 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/group_box.py
--rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/group_box_response.py
--rw-rw-rw-   0        0        0    22625 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/group_shape.py
--rw-rw-rw-   0        0        0     5297 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/horizontal_page_break.py
--rw-rw-rw-   0        0        0     5463 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/horizontal_page_break_response.py
--rw-rw-rw-   0        0        0     4325 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/horizontal_page_breaks.py
--rw-rw-rw-   0        0        0     5487 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/horizontal_page_breaks_response.py
--rw-rw-rw-   0        0        0    33972 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/html_save_options.py
--rw-rw-rw-   0        0        0     6585 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/hyperlink.py
--rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/hyperlink_response.py
--rw-rw-rw-   0        0        0     5225 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/hyperlinks.py
--rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/hyperlinks_response.py
--rw-rw-rw-   0        0        0     4845 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/icon_filter.py
--rw-rw-rw-   0        0        0     6677 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/icon_set.py
--rw-rw-rw-   0        0        0    19550 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/image_or_print_options.py
--rw-rw-rw-   0        0        0    15645 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/image_save_options.py
--rw-rw-rw-   0        0        0     7525 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import2_dimension_double_array_option.py
--rw-rw-rw-   0        0        0     7505 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import2_dimension_int_array_option.py
--rw-rw-rw-   0        0        0     7523 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import2_dimension_string_array_option.py
--rw-rw-rw-   0        0        0     6579 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_batch_data_option.py
--rw-rw-rw-   0        0        0     9355 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_csv_data_option.py
--rw-rw-rw-   0        0        0     5616 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_data_task_parameter.py
--rw-rw-rw-   0        0        0     7964 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_double_array_option.py
--rw-rw-rw-   0        0        0     7944 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_int_array_option.py
--rw-rw-rw-   0        0        0     5607 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_json_request.py
--rw-rw-rw-   0        0        0     6032 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_option.py
--rw-rw-rw-   0        0        0     9230 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_picture_option.py
--rw-rw-rw-   0        0        0     5368 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_position.py
--rw-rw-rw-   0        0        0     7962 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_string_array_option.py
--rw-rw-rw-   0        0        0     5567 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/import_xml_request.py
--rw-rw-rw-   0        0        0    10629 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/json_save_options.py
--rw-rw-rw-   0        0        0    22595 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/label.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/label_response.py
--rw-rw-rw-   0        0        0    10787 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend.py
--rw-rw-rw-   0        0        0     4896 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend_entries.py
--rw-rw-rw-   0        0        0     5303 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend_entries_response.py
--rw-rw-rw-   0        0        0     6264 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend_entry.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend_entry_response.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/legend_response.py
--rw-rw-rw-   0        0        0    13310 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/line.py
--rw-rw-rw-   0        0        0    13093 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/line_format.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/line_response.py
--rw-rw-rw-   0        0        0    26553 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/line_shape.py
--rw-rw-rw-   0        0        0     5123 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/line_shape_response.py
--rw-rw-rw-   0        0        0     5368 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/link.py
--rw-rw-rw-   0        0        0     4271 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/link_element.py
--rw-rw-rw-   0        0        0    26160 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_box.py
--rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_box_response.py
--rw-rw-rw-   0        0        0     6293 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_column.py
--rw-rw-rw-   0        0        0    16354 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_object.py
--rw-rw-rw-   0        0        0     5000 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_object_operate_parameter.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_object_response.py
--rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_objects.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/list_objects_response.py
--rw-rw-rw-   0        0        0    10283 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/load_options.py
--rw-rw-rw-   0        0        0    16670 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/m_html_save_options.py
--rw-rw-rw-   0        0        0    10167 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/markdown_save_options.py
--rw-rw-rw-   0        0        0     5669 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/marker.py
--rw-rw-rw-   0        0        0     5155 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/match_condition_request.py
--rw-rw-rw-   0        0        0     6155 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/merged_cell.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/merged_cell_response.py
--rw-rw-rw-   0        0        0     5264 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/merged_cells.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/merged_cells_response.py
--rw-rw-rw-   0        0        0     3910 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/multiple_filter.py
--rw-rw-rw-   0        0        0     5080 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/multiple_filters.py
--rw-rw-rw-   0        0        0     7615 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/name.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/name_response.py
--rw-rw-rw-   0        0        0     5110 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/names.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/names_response.py
--rw-rw-rw-   0        0        0     5922 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/negative_bar_format.py
--rw-rw-rw-   0        0        0     4770 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/object_exist.py
--rw-rw-rw-   0        0        0     3958 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/object_exists_extensions.py
--rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ods_save_options.py
--rw-rw-rw-   0        0        0    26408 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ole_object.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ole_object_response.py
--rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ole_objects.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ole_objects_response.py
--rw-rw-rw-   0        0        0    11501 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ooxml_save_options.py
--rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/operate_object.py
--rw-rw-rw-   0        0        0     6945 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/operate_object_position.py
--rw-rw-rw-   0        0        0     4435 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/operate_parameter.py
--rw-rw-rw-   0        0        0    22589 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/oval.py
--rw-rw-rw-   0        0        0     5088 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/oval_response.py
--rw-rw-rw-   0        0        0     7190 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_break_operate_parameter.py
--rw-rw-rw-   0        0        0     6398 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_section.py
--rw-rw-rw-   0        0        0     5284 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_sections_response.py
--rw-rw-rw-   0        0        0    22807 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_setup.py
--rw-rw-rw-   0        0        0     4976 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_setup_operate_parameter.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/page_setup_response.py
--rw-rw-rw-   0        0        0    20195 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/paginated_save_options.py
--rw-rw-rw-   0        0        0     4362 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/password_request.py
--rw-rw-rw-   0        0        0     5959 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/paste_options.py
--rw-rw-rw-   0        0        0     8077 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pattern_fill.py
--rw-rw-rw-   0        0        0    19511 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pdf_save_options.py
--rw-rw-rw-   0        0        0    10047 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/pdf_security_options.py
--rw-rw-rw-   0        0        0     6255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pic_format_option.py
--rw-rw-rw-   0        0        0    25954 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/picture.py
--rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/picture_response.py
--rw-rw-rw-   0        0        0     4782 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pictures.py
--rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pictures_response.py
--rw-rw-rw-   0        0        0    25716 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_field.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_field_response.py
--rw-rw-rw-   0        0        0     8549 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_filter.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_filter_response.py
--rw-rw-rw-   0        0        0     5284 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_filters_response.py
--rw-rw-rw-   0        0        0     3982 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_globalization_settings.py
--rw-rw-rw-   0        0        0     5517 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_item.py
--rw-rw-rw-   0        0        0    44381 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_table.py
--rw-rw-rw-   0        0        0     4342 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_table_field_request.py
--rw-rw-rw-   0        0        0     9002 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_table_operate_parameter.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_table_response.py
--rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_tables.py
--rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pivot_tables_response.py
--rw-rw-rw-   0        0        0    11667 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/plot_area.py
--rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/plot_area_response.py
--rw-rw-rw-   0        0        0    22164 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/pptx_save_options.py
--rw-rw-rw-   0        0        0    14256 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/protect_sheet_parameter.py
--rw-rw-rw-   0        0        0     7844 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/protect_workbook_request.py
--rw-rw-rw-   0        0        0    15070 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/protection.py
--rw-rw-rw-   0        0        0     6582 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/query_table.py
--rw-rw-rw-   0        0        0    23997 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/radio_button.py
--rw-rw-rw-   0        0        0     5137 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/radio_button_response.py
--rw-rw-rw-   0        0        0     8121 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range.py
--rw-rw-rw-   0        0        0     5724 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_copy_request.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_response.py
--rw-rw-rw-   0        0        0     5921 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_set_outline_border_request.py
--rw-rw-rw-   0        0        0     4742 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_set_style_request.py
--rw-rw-rw-   0        0        0     4891 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_sort_request.py
--rw-rw-rw-   0        0        0     5214 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/range_value_response.py
--rw-rw-rw-   0        0        0     4349 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ranges.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/ranges_response.py
--rw-rw-rw-   0        0        0    22649 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rectangle_shape.py
--rw-rw-rw-   0        0        0     5158 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rectangle_shape_response.py
--rw-rw-rw-   0        0        0     5859 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rendering_font.py
--rw-rw-rw-   0        0        0     9081 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rendering_watermark.py
--rw-rw-rw-   0        0        0     5488 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/result_destination.py
--rw-rw-rw-   0        0        0     7452 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/row.py
--rw-rw-rw-   0        0        0     5047 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/row_response.py
--rw-rw-rw-   0        0        0     5618 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rows.py
--rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/rows_response.py
--rw-rw-rw-   0        0        0     5504 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_files_to_cloud_result.py
--rw-rw-rw-   0        0        0     5567 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_files_to_cloud_result_response.py
--rw-rw-rw-   0        0        0     8556 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_options.py
--rw-rw-rw-   0        0        0     5195 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_response.py
--rw-rw-rw-   0        0        0     4370 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_result.py
--rw-rw-rw-   0        0        0     5125 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/save_result_task_parameter.py
--rw-rw-rw-   0        0        0    25940 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/scroll_bar.py
--rw-rw-rw-   0        0        0     5123 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/scroll_bar_response.py
--rw-rw-rw-   0        0        0    28722 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/series.py
--rw-rw-rw-   0        0        0     6548 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/series_items.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/series_response.py
--rw-rw-rw-   0        0        0     5170 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/serieses_response.py
--rw-rw-rw-   0        0        0     6929 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shadow_effect.py
--rw-rw-rw-   0        0        0    22595 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shape.py
--rw-rw-rw-   0        0        0     4864 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shape_operate_parameter.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shape_response.py
--rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shapes.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/shapes_response.py
--rw-rw-rw-   0        0        0     4768 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/single_value.py
--rw-rw-rw-   0        0        0     5137 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/single_value_response.py
--rw-rw-rw-   0        0        0     5653 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/smart_marker_task_parameter.py
--rw-rw-rw-   0        0        0     5300 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/solid_fill.py
--rw-rw-rw-   0        0        0     6388 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sort_key.py
--rw-rw-rw-   0        0        0     5136 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sparkline.py
--rw-rw-rw-   0        0        0    20368 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sparkline_group.py
--rw-rw-rw-   0        0        0     5327 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sparkline_group_response.py
--rw-rw-rw-   0        0        0     4581 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sparkline_groups.py
--rw-rw-rw-   0        0        0     5351 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sparkline_groups_response.py
--rw-rw-rw-   0        0        0    24897 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/spinner.py
--rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/spinner_response.py
--rw-rw-rw-   0        0        0     4376 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/split_result.py
--rw-rw-rw-   0        0        0     4665 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/split_result_document.py
--rw-rw-rw-   0        0        0     5154 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/split_result_response.py
--rw-rw-rw-   0        0        0     7745 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/split_workbook_task_parameter.py
--rw-rw-rw-   0        0        0    10626 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/spreadsheet_m_l2003_save_options.py
--rw-rw-rw-   0        0        0    16432 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/sql_script_save_options.py
--rw-rw-rw-   0        0        0     4311 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/storage_exist.py
--rw-rw-rw-   0        0        0     6032 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/storage_file.py
--rw-rw-rw-   0        0        0    16124 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/style.py
--rw-rw-rw-   0        0        0    10636 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/style_format_condition.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/style_response.py
--rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/styles.py
--rw-rw-rw-   0        0        0     9072 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/svg_save_options.py
--rw-rw-rw-   0        0        0     5691 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/table_total_request.py
--rw-rw-rw-   0        0        0     4287 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_data.py
--rw-rw-rw-   0        0        0     4937 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_description.py
--rw-rw-rw-   0        0        0     3904 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_parameter.py
--rw-rw-rw-   0        0        0     3940 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_result_parameter.py
--rw-rw-rw-   0        0        0     4945 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_run_result.py
--rw-rw-rw-   0        0        0     5319 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/task_run_result_response.py
--rw-rw-rw-   0        0        0    22607 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_box.py
--rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_box_response.py
--rw-rw-rw-   0        0        0     5662 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_format_condition.py
--rw-rw-rw-   0        0        0     4633 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_item.py
--rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_item_response.py
--rw-rw-rw-   0        0        0     4818 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_items.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_items_response.py
--rw-rw-rw-   0        0        0    11179 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_options.py
--rw-rw-rw-   0        0        0     6075 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/text_water_marker_request.py
--rw-rw-rw-   0        0        0     6778 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/texture_fill.py
--rw-rw-rw-   0        0        0     4747 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/theme_color.py
--rw-rw-rw-   0        0        0     9968 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/tick_labels.py
--rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/tick_labels_response.py
--rw-rw-rw-   0        0        0     6711 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/tile_pic_option.py
--rw-rw-rw-   0        0        0     4472 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/time_period_format_condition.py
--rw-rw-rw-   0        0        0    13704 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/title.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/title_response.py
--rw-rw-rw-   0        0        0     5181 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/top10.py
--rw-rw-rw-   0        0        0     5631 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/top10_filter.py
--rw-rw-rw-   0        0        0    19370 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/trendline.py
--rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/trendline_response.py
--rw-rw-rw-   0        0        0     4828 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/trendlines.py
--rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/trendlines_response.py
--rw-rw-rw-   0        0        0    10636 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/txt_save_options.py
--rw-rw-rw-   0        0        0    11929 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/validation.py
--rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/validation_response.py
--rw-rw-rw-   0        0        0     5248 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/validations.py
--rw-rw-rw-   0        0        0     5239 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/validations_response.py
--rw-rw-rw-   0        0        0     5234 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/vertical_page_break.py
--rw-rw-rw-   0        0        0     5415 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/vertical_page_break_response.py
--rw-rw-rw-   0        0        0     4313 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/vertical_page_breaks.py
--rw-rw-rw-   0        0        0     5439 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/vertical_page_breaks_response.py
--rw-rw-rw-   0        0        0     9595 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/walls.py
--rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/walls_response.py
--rw-rw-rw-   0        0        0     9384 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook.py
--rw-rw-rw-   0        0        0     5469 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_encryption_request.py
--rw-rw-rw-   0        0        0     4483 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_operate_parameter.py
--rw-rw-rw-   0        0        0     4988 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_protection_request.py
--rw-rw-rw-   0        0        0     5643 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_replace_response.py
--rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_response.py
--rw-rw-rw-   0        0        0    39915 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_settings.py
--rw-rw-rw-   0        0        0     5144 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_settings_operate_parameter.py
--rw-rw-rw-   0        0        0     5223 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbook_settings_response.py
--rw-rw-rw-   0        0        0     5199 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/workbooks_response.py
--rw-rw-rw-   0        0        0    20781 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet.py
--rw-rw-rw-   0        0        0     9532 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet_data_statistics.py
--rw-rw-rw-   0        0        0     5072 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet_moving_request.py
--rw-rw-rw-   0        0        0     6365 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet_operate_parameter.py
--rw-rw-rw-   0        0        0     5666 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet_replace_response.py
--rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheet_response.py
--rw-rw-rw-   0        0        0     4828 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheets.py
--rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/worksheets_response.py
--rw-rw-rw-   0        0        0     6027 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/write_protection.py
--rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/xls_save_options.py
--rw-rw-rw-   0        0        0     8580 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/xlsb_save_options.py
--rw-rw-rw-   0        0        0     4271 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/xml_data_binding.py
--rw-rw-rw-   0        0        0     5365 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/xml_map.py
--rw-rw-rw-   0        0        0    20159 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/models/xps_save_options.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:34.993549 asposecellscloud-24.3/asposecellscloud/requests/
--rw-rw-rw-   0        0        0    35331 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/__init__.py
--rw-rw-rw-   0        0        0     4290 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/copy_file_request.py
--rw-rw-rw-   0        0        0     4137 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/copy_folder_request.py
--rw-rw-rw-   0        0        0     3513 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/create_folder_request.py
--rw-rw-rw-   0        0        0     4058 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_decrypt_workbook_request.py
--rw-rw-rw-   0        0        0     3715 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_document_properties_request.py
--rw-rw-rw-   0        0        0     4246 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_document_property_request.py
--rw-rw-rw-   0        0        0     3745 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py
--rw-rw-rw-   0        0        0     3671 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_file_request.py
--rw-rw-rw-   0        0        0     3674 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_folder_request.py
--rw-rw-rw-   0        0        0     4092 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_header_footer_request.py
--rw-rw-rw-   0        0        0     4450 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4241 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_horizontal_page_breaks_request.py
--rw-rw-rw-   0        0        0     4250 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_metadata_request.py
--rw-rw-rw-   0        0        0     5464 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4072 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_un_protect_workbook_request.py
--rw-rw-rw-   0        0        0     4518 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_unprotect_worksheet_request.py
--rw-rw-rw-   0        0        0     4438 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4249 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_vertical_page_breaks_request.py
--rw-rw-rw-   0        0        0     3707 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_background_request.py
--rw-rw-rw-   0        0        0     4049 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_name_request.py
--rw-rw-rw-   0        0        0     3687 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_names_request.py
--rw-rw-rw-   0        0        0     4103 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_background_request.py
--rw-rw-rw-   0        0        0     4785 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_cells_range_request.py
--rw-rw-rw-   0        0        0     4506 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4466 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4083 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_charts_request.py
--rw-rw-rw-   0        0        0     5285 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4458 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4093 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_comments_request.py
--rw-rw-rw-   0        0        0     5828 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py
--rw-rw-rw-   0        0        0     4507 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     4165 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py
--rw-rw-rw-   0        0        0     5804 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_date_filter_request.py
--rw-rw-rw-   0        0        0     4636 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_filter_request.py
--rw-rw-rw-   0        0        0     5624 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py
--rw-rw-rw-   0        0        0     4530 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     4103 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py
--rw-rw-rw-   0        0        0     4557 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4110 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_list_objects_request.py
--rw-rw-rw-   0        0        0     4541 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4105 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_ole_objects_request.py
--rw-rw-rw-   0        0        0     4498 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_picture_request.py
--rw-rw-rw-   0        0        0     4093 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pictures_request.py
--rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4812 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py
--rw-rw-rw-   0        0        0     4557 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     4110 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py
--rw-rw-rw-   0        0        0     4050 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_request.py
--rw-rw-rw-   0        0        0     4440 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4804 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     4458 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     4083 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_shapes_request.py
--rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4130 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py
--rw-rw-rw-   0        0        0     4546 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4108 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_validations_request.py
--rw-rw-rw-   0        0        0     3849 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/delete_worksheets_request.py
--rw-rw-rw-   0        0        0     3678 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/download_file_request.py
--rw-rw-rw-   0        0        0     4426 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_cell_html_string_request.py
--rw-rw-rw-   0        0        0     3073 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_cells_cloud_service_status_request.py
--rw-rw-rw-   0        0        0     3072 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py
--rw-rw-rw-   0        0        0     4467 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_border_request.py
--rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_fill_format_request.py
--rw-rw-rw-   0        0        0     4432 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_request.py
--rw-rw-rw-   0        0        0     4473 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_category_axis_request.py
--rw-rw-rw-   0        0        0     4512 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_second_category_axis_request.py
--rw-rw-rw-   0        0        0     4494 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_second_value_axis_request.py
--rw-rw-rw-   0        0        0     4461 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_series_axis_request.py
--rw-rw-rw-   0        0        0     4455 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_chart_value_axis_request.py
--rw-rw-rw-   0        0        0     3212 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_disc_usage_request.py
--rw-rw-rw-   0        0        0     3844 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_document_properties_request.py
--rw-rw-rw-   0        0        0     4114 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_document_property_request.py
--rw-rw-rw-   0        0        0     3536 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_file_versions_request.py
--rw-rw-rw-   0        0        0     3340 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_files_list_request.py
--rw-rw-rw-   0        0        0     4042 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_footer_request.py
--rw-rw-rw-   0        0        0     4042 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_header_request.py
--rw-rw-rw-   0        0        0     4441 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4114 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_horizontal_page_breaks_request.py
--rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_metadata_request.py
--rw-rw-rw-   0        0        0     4068 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_named_range_value_request.py
--rw-rw-rw-   0        0        0     3677 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_named_ranges_request.py
--rw-rw-rw-   0        0        0     3652 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_page_count_request.py
--rw-rw-rw-   0        0        0     4046 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_page_setup_request.py
--rw-rw-rw-   0        0        0     5403 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4427 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4102 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_vertical_page_breaks_request.py
--rw-rw-rw-   0        0        0     3699 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_default_style_request.py
--rw-rw-rw-   0        0        0     4028 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_name_request.py
--rw-rw-rw-   0        0        0     4062 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_name_value_request.py
--rw-rw-rw-   0        0        0     3670 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_names_request.py
--rw-rw-rw-   0        0        0     5530 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_request.py
--rw-rw-rw-   0        0        0     3693 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_settings_request.py
--rw-rw-rw-   0        0        0     3691 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_workbook_text_items_request.py
--rw-rw-rw-   0        0        0     4090 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_auto_filter_request.py
--rw-rw-rw-   0        0        0     4704 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py
--rw-rw-rw-   0        0        0     4088 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_autoshapes_request.py
--rw-rw-rw-   0        0        0     4481 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4503 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cell_request.py
--rw-rw-rw-   0        0        0     4451 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cell_style_request.py
--rw-rw-rw-   0        0        0     4936 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cells_range_value_request.py
--rw-rw-rw-   0        0        0     4332 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cells_request.py
--rw-rw-rw-   0        0        0     4484 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4584 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4477 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4064 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_charts_request.py
--rw-rw-rw-   0        0        0     4466 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_column_request.py
--rw-rw-rw-   0        0        0     3951 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4437 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4076 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_comments_request.py
--rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     4162 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py
--rw-rw-rw-   0        0        0     4511 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     4088 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_hyperlinks_request.py
--rw-rw-rw-   0        0        0     4649 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_list_objects_request.py
--rw-rw-rw-   0        0        0     4539 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_merged_cell_request.py
--rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_merged_cells_request.py
--rw-rw-rw-   0        0        0     4621 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4090 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_ole_objects_request.py
--rw-rw-rw-   0        0        0     4070 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_page_count_request.py
--rw-rw-rw-   0        0        0     4888 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_picture_with_format_request.py
--rw-rw-rw-   0        0        0     4076 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pictures_request.py
--rw-rw-rw-   0        0        0     4993 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4592 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py
--rw-rw-rw-   0        0        0     4531 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_tables_request.py
--rw-rw-rw-   0        0        0     4415 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4333 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     4435 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     4064 2024-01-16 20:47:48.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_shapes_request.py
--rw-rw-rw-   0        0        0     4549 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4120 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py
--rw-rw-rw-   0        0        0     4084 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_text_items_request.py
--rw-rw-rw-   0        0        0     4528 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4094 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_validations_request.py
--rw-rw-rw-   0        0        0     4942 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_with_format_request.py
--rw-rw-rw-   0        0        0     3670 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/get_worksheets_request.py
--rw-rw-rw-   0        0        0     4290 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/move_file_request.py
--rw-rw-rw-   0        0        0     4137 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/move_folder_request.py
--rw-rw-rw-   0        0        0     3686 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/object_exists_request.py
--rw-rw-rw-   0        0        0     3491 2024-02-22 10:48:54.000000 asposecellscloud-24.3/asposecellscloud/requests/post_analyze_excel_request.py
--rw-rw-rw-   0        0        0     4621 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_assemble_request.py
--rw-rw-rw-   0        0        0     4054 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_autofit_workbook_columns_request.py
--rw-rw-rw-   0        0        0     4163 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_autofit_workbook_rows_request.py
--rw-rw-rw-   0        0        0     4610 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5265 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4559 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3481 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_batch_convert_request.py
--rw-rw-rw-   0        0        0     3445 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_batch_lock_request.py
--rw-rw-rw-   0        0        0     3481 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_batch_protect_request.py
--rw-rw-rw-   0        0        0     3457 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_batch_split_request.py
--rw-rw-rw-   0        0        0     3453 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_batch_unlock_request.py
--rw-rw-rw-   0        0        0     4565 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_cell_calculate_request.py
--rw-rw-rw-   0        0        0     4571 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_cell_characters_request.py
--rw-rw-rw-   0        0        0     4798 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_chart_category_axis_request.py
--rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_chart_second_category_axis_request.py
--rw-rw-rw-   0        0        0     4823 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_chart_second_value_axis_request.py
--rw-rw-rw-   0        0        0     4784 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_chart_series_axis_request.py
--rw-rw-rw-   0        0        0     4777 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_chart_value_axis_request.py
--rw-rw-rw-   0        0        0     4852 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_clear_contents_request.py
--rw-rw-rw-   0        0        0     4847 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_clear_formats_request.py
--rw-rw-rw-   0        0        0     4801 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_clear_objects_request.py
--rw-rw-rw-   0        0        0     4776 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_column_style_request.py
--rw-rw-rw-   0        0        0     4133 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_compress_request.py
--rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_csv_request.py
--rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_docx_request.py
--rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_html_request.py
--rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_json_request.py
--rw-rw-rw-   0        0        0     4145 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py
--rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py
--rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_png_request.py
--rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py
--rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_sql_request.py
--rw-rw-rw-   0        0        0     5290 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_copy_cell_into_cell_request.py
--rw-rw-rw-   0        0        0     5652 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5164 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_request.py
--rw-rw-rw-   0        0        0     5547 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3496 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_data_cleansing_request.py
--rw-rw-rw-   0        0        0     3544 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_data_deduplication_request.py
--rw-rw-rw-   0        0        0     3436 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_data_fill_request.py
--rw-rw-rw-   0        0        0     3589 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_delete_incomplete_rows_request.py
--rw-rw-rw-   0        0        0     4533 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_digital_signature_request.py
--rw-rw-rw-   0        0        0     4048 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_encrypt_workbook_request.py
--rw-rw-rw-   0        0        0     4387 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_export_request.py
--rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_fit_tall_to_pages_request.py
--rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_fit_wide_to_pages_request.py
--rw-rw-rw-   0        0        0     5117 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_footer_request.py
--rw-rw-rw-   0        0        0     5021 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_group_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5000 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_group_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5117 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_header_request.py
--rw-rw-rw-   0        0        0     4922 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_hide_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4839 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_hide_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3972 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_import_data_request.py
--rw-rw-rw-   0        0        0     4241 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_import_request.py
--rw-rw-rw-   0        0        0     3888 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_lock_request.py
--rw-rw-rw-   0        0        0     4443 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_merge_request.py
--rw-rw-rw-   0        0        0     4549 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_metadata_request.py
--rw-rw-rw-   0        0        0     4391 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_move_worksheet_request.py
--rw-rw-rw-   0        0        0     4404 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_page_setup_request.py
--rw-rw-rw-   0        0        0     5756 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_cell_style_request.py
--rw-rw-rw-   0        0        0     6386 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py
--rw-rw-rw-   0        0        0     5634 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_field_move_to_request.py
--rw-rw-rw-   0        0        0     5058 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_style_request.py
--rw-rw-rw-   0        0        0     6086 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py
--rw-rw-rw-   0        0        0     5635 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py
--rw-rw-rw-   0        0        0     4048 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_protect_request.py
--rw-rw-rw-   0        0        0     4160 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_protect_workbook_request.py
--rw-rw-rw-   0        0        0     4426 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_rename_worksheet_request.py
--rw-rw-rw-   0        0        0     3709 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_repair_request.py
--rw-rw-rw-   0        0        0     4761 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_replace_request.py
--rw-rw-rw-   0        0        0     4624 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_reverse_request.py
--rw-rw-rw-   0        0        0     4619 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_rotate_request.py
--rw-rw-rw-   0        0        0     4725 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_row_style_request.py
--rw-rw-rw-   0        0        0     3363 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_run_task_request.py
--rw-rw-rw-   0        0        0     4415 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_search_request.py
--rw-rw-rw-   0        0        0     4465 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_set_cell_html_string_request.py
--rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_set_cell_range_value_request.py
--rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_set_worksheet_column_width_request.py
--rw-rw-rw-   0        0        0     4691 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_split_request.py
--rw-rw-rw-   0        0        0     4907 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     5025 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5070 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_unhide_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4993 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_unhide_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     3898 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_unlock_request.py
--rw-rw-rw-   0        0        0     4824 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_cell_style_request.py
--rw-rw-rw-   0        0        0     4875 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     4427 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_property_request.py
--rw-rw-rw-   0        0        0     4799 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_range_style_request.py
--rw-rw-rw-   0        0        0     4735 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4429 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_zoom_request.py
--rw-rw-rw-   0        0        0     4900 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_watermark_request.py
--rw-rw-rw-   0        0        0     4026 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4631 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_cleansing_request.py
--rw-rw-rw-   0        0        0     4699 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_deduplication_request.py
--rw-rw-rw-   0        0        0     4566 2024-03-22 07:23:40.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_fill_request.py
--rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_export_xml_request.py
--rw-rw-rw-   0        0        0     4219 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py
--rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_import_json_request.py
--rw-rw-rw-   0        0        0     4988 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_import_xml_request.py
--rw-rw-rw-   0        0        0     4378 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_name_request.py
--rw-rw-rw-   0        0        0     5719 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_save_as_request.py
--rw-rw-rw-   0        0        0     4034 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_settings_request.py
--rw-rw-rw-   0        0        0     5068 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_split_request.py
--rw-rw-rw-   0        0        0     4459 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbook_text_replace_request.py
--rw-rw-rw-   0        0        0     4274 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbooks_merge_request.py
--rw-rw-rw-   0        0        0     4031 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_workbooks_text_search_request.py
--rw-rw-rw-   0        0        0     4133 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_calculate_formula_request.py
--rw-rw-rw-   0        0        0     4876 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cell_set_value_request.py
--rw-rw-rw-   0        0        0     4840 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py
--rw-rw-rw-   0        0        0     4448 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py
--rw-rw-rw-   0        0        0     5232 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py
--rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py
--rw-rw-rw-   0        0        0     4826 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py
--rw-rw-rw-   0        0        0     4546 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_sort_request.py
--rw-rw-rw-   0        0        0     4512 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_style_request.py
--rw-rw-rw-   0        0        0     4463 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py
--rw-rw-rw-   0        0        0     5126 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_value_request.py
--rw-rw-rw-   0        0        0     4511 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_ranges_copy_request.py
--rw-rw-rw-   0        0        0     4826 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     4771 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4811 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     4781 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4460 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_group_shape_request.py
--rw-rw-rw-   0        0        0     4871 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     5329 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_column_request.py
--rw-rw-rw-   0        0        0     5046 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_columns_total_request.py
--rw-rw-rw-   0        0        0     4639 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py
--rw-rw-rw-   0        0        0     5473 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_insert_slicer_request.py
--rw-rw-rw-   0        0        0     4648 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_remove_duplicates_request.py
--rw-rw-rw-   0        0        0     4916 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     4983 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py
--rw-rw-rw-   0        0        0     5661 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py
--rw-rw-rw-   0        0        0     4505 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_match_blanks_request.py
--rw-rw-rw-   0        0        0     4526 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py
--rw-rw-rw-   0        0        0     5622 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_merge_request.py
--rw-rw-rw-   0        0        0     4821 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_picture_request.py
--rw-rw-rw-   0        0        0     4603 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py
--rw-rw-rw-   0        0        0     5021 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py
--rw-rw-rw-   0        0        0     4829 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_range_sort_request.py
--rw-rw-rw-   0        0        0     4747 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     5016 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4858 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_text_replace_request.py
--rw-rw-rw-   0        0        0     4423 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_text_search_request.py
--rw-rw-rw-   0        0        0     4492 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py
--rw-rw-rw-   0        0        0     5640 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_unmerge_request.py
--rw-rw-rw-   0        0        0     4896 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     4068 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_active_worksheet_request.py
--rw-rw-rw-   0        0        0     4373 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_add_new_worksheet_request.py
--rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_change_visibility_worksheet_request.py
--rw-rw-rw-   0        0        0     5253 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_convert_workbook_request.py
--rw-rw-rw-   0        0        0     4047 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_document_property_request.py
--rw-rw-rw-   0        0        0     4080 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_document_protect_from_changes_request.py
--rw-rw-rw-   0        0        0     4852 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_horizontal_page_break_request.py
--rw-rw-rw-   0        0        0     4973 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_insert_new_worksheet_request.py
--rw-rw-rw-   0        0        0     5067 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_columns_request.py
--rw-rw-rw-   0        0        0     4455 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_row_request.py
--rw-rw-rw-   0        0        0     4819 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_rows_request.py
--rw-rw-rw-   0        0        0     5644 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_pivot_table_field_request.py
--rw-rw-rw-   0        0        0     4490 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_protect_worksheet_request.py
--rw-rw-rw-   0        0        0     4806 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_vertical_page_break_request.py
--rw-rw-rw-   0        0        0     4182 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_workbook_background_request.py
--rw-rw-rw-   0        0        0     4430 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_workbook_create_request.py
--rw-rw-rw-   0        0        0     4010 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_workbook_name_request.py
--rw-rw-rw-   0        0        0     4182 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_workbook_water_marker_request.py
--rw-rw-rw-   0        0        0     5182 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_add_picture_request.py
--rw-rw-rw-   0        0        0     4575 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_background_request.py
--rw-rw-rw-   0        0        0     4764 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_cells_range_request.py
--rw-rw-rw-   0        0        0     4488 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_legend_request.py
--rw-rw-rw-   0        0        0     6876 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_request.py
--rw-rw-rw-   0        0        0     4599 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_title_request.py
--rw-rw-rw-   0        0        0     5539 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_color_filter_request.py
--rw-rw-rw-   0        0        0     4771 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_comment_request.py
--rw-rw-rw-   0        0        0     4944 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py
--rw-rw-rw-   0        0        0     6443 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_custom_filter_request.py
--rw-rw-rw-   0        0        0     6443 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_date_filter_request.py
--rw-rw-rw-   0        0        0     5640 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py
--rw-rw-rw-   0        0        0     5482 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_filter_request.py
--rw-rw-rw-   0        0        0     6276 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_filter_top10_request.py
--rw-rw-rw-   0        0        0     4871 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_area_request.py
--rw-rw-rw-   0        0        0     6049 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py
--rw-rw-rw-   0        0        0     6330 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_request.py
--rw-rw-rw-   0        0        0     5597 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_freeze_panes_request.py
--rw-rw-rw-   0        0        0     5999 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_hyperlink_request.py
--rw-rw-rw-   0        0        0     5918 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_icon_filter_request.py
--rw-rw-rw-   0        0        0     5244 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_list_object_request.py
--rw-rw-rw-   0        0        0     5064 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_ole_object_request.py
--rw-rw-rw-   0        0        0     5126 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py
--rw-rw-rw-   0        0        0     4801 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_pivot_table_request.py
--rw-rw-rw-   0        0        0     5290 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_shape_request.py
--rw-rw-rw-   0        0        0     5651 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_sparkline_group_request.py
--rw-rw-rw-   0        0        0     4223 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_validation_request.py
--rw-rw-rw-   0        0        0     3428 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/storage_exists_request.py
--rw-rw-rw-   0        0        0     4127 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/requests/upload_file_request.py
--rw-rw-rw-   0        0        0    14234 2024-01-16 20:47:49.000000 asposecellscloud-24.3/asposecellscloud/rest.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:35.405868 asposecellscloud-24.3/asposecellscloud.egg-info/
--rw-rw-rw-   0        0        0    17451 2024-03-22 07:34:20.000000 asposecellscloud-24.3/asposecellscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    40331 2024-03-22 07:34:21.000000 asposecellscloud-24.3/asposecellscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 07:34:20.000000 asposecellscloud-24.3/asposecellscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-03-22 07:34:20.000000 asposecellscloud-24.3/asposecellscloud.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-22 07:34:20.000000 asposecellscloud-24.3/asposecellscloud.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      894 2024-03-22 07:32:25.000000 asposecellscloud-24.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 07:34:35.436655 asposecellscloud-24.3/setup.cfg
--rw-rw-rw-   0        0        0     1473 2024-03-22 07:31:45.000000 asposecellscloud-24.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-22 07:34:35.378563 asposecellscloud-24.3/test/
--rw-rw-rw-   0        0        0     7996 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_auto_filter_controller.py
--rw-rw-rw-   0        0        0     4635 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_batch_controller.py
--rw-rw-rw-   0        0        0    21475 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_cells_controller.py
--rw-rw-rw-   0        0        0     1774 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_cells_status_controller.py
--rw-rw-rw-   0        0        0     2297 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_chart_area_controller.py
--rw-rw-rw-   0        0        0     8031 2024-01-16 20:47:49.000000 asposecellscloud-24.3/test/tests_charts_controller.py
--rw-rw-rw-   0        0        0     5842 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_conditional_formattings_controller.py
--rw-rw-rw-   0        0        0    47339 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_conversion.py
--rw-rw-rw-   0        0        0    11416 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_conversion_json.py
--rw-rw-rw-   0        0        0     8122 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_conversion_png.py
--rw-rw-rw-   0        0        0     3069 2024-03-22 07:23:40.000000 asposecellscloud-24.3/test/tests_data_processing_controller.py
--rw-rw-rw-   0        0        0     3361 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_file_controller.py
--rw-rw-rw-   0        0        0     3094 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_folder_controller.py
--rw-rw-rw-   0        0        0     3932 2023-12-23 14:58:33.000000 asposecellscloud-24.3/test/tests_hypelinks_controller.py
--rw-rw-rw-   0        0        0   119156 2024-01-16 20:47:49.000000 asposecellscloud-24.3/test/tests_light_cells.py
--rw-rw-rw-   0        0        0     8709 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_list_objects_controller.py
--rw-rw-rw-   0        0        0     4326 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_ole_objects_controller.py
--rw-rw-rw-   0        0        0     1308 2023-11-25 21:14:26.000000 asposecellscloud-24.3/test/tests_one.py
--rw-rw-rw-   0        0        0     5884 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_page_breaks_controller.py
--rw-rw-rw-   0        0        0     5151 2024-01-16 20:47:49.000000 asposecellscloud-24.3/test/tests_page_setup_controller.py
--rw-rw-rw-   0        0        0     4182 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_pictures_controller.py
--rw-rw-rw-   0        0        0    12668 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_pivot_tables_controller.py
--rw-rw-rw-   0        0        0     3363 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_properties_controller.py
--rw-rw-rw-   0        0        0     9553 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_ranges_controller.py
--rw-rw-rw-   0        0        0     4970 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_shapes_controller.py
--rw-rw-rw-   0        0        0     4073 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_sparkline_groups_controller.py
--rw-rw-rw-   0        0        0     2573 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_storage_controller.py
--rw-rw-rw-   0        0        0    18942 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_workbook_controller.py
--rw-rw-rw-   0        0        0    21083 2024-01-16 20:47:49.000000 asposecellscloud-24.3/test/tests_worksheet_controller.py
--rw-rw-rw-   0        0        0     3912 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_worksheet_validations_controller.py
--rw-rw-rw-   0        0        0     2397 2023-12-23 14:58:34.000000 asposecellscloud-24.3/test/tests_xml_controller.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:29.286884 asposecellscloud-24.4/
+-rw-rw-rw-   0        0        0     1090 2024-01-16 20:47:48.000000 asposecellscloud-24.4/LICENSE
+-rw-rw-rw-   0        0        0    17545 2024-04-28 05:59:29.282991 asposecellscloud-24.4/PKG-INFO
+-rw-rw-rw-   0        0        0    16540 2024-04-28 05:57:35.000000 asposecellscloud-24.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:13.764568 asposecellscloud-24.4/asposecellscloud/
+-rw-rw-rw-   0        0        0    64572 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/__init__.py
+-rw-rw-rw-   0        0        0    30582 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:13.895500 asposecellscloud-24.4/asposecellscloud/apis/
+-rw-rw-rw-   0        0        0      128 2023-12-23 14:58:26.000000 asposecellscloud-24.4/asposecellscloud/apis/__init__.py
+-rw-rw-rw-   0        0        0   814059 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/apis/cells_api.py
+-rw-rw-rw-   0        0        0     8822 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/configuration.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:21.808231 asposecellscloud-24.4/asposecellscloud/models/
+-rw-rw-rw-   0        0        0    30315 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/__init__.py
+-rw-rw-rw-   0        0        0     5492 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/above_average.py
+-rw-rw-rw-   0        0        0     6246 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/abstract_calculation_engine.py
+-rw-rw-rw-   0        0        0     5645 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/abstract_calculation_monitor.py
+-rw-rw-rw-   0        0        0    10538 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/access_token_response.py
+-rw-rw-rw-   0        0        0     5581 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyze_excel_request.py
+-rw-rw-rw-   0        0        0     4463 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyze_excel_response.py
+-rw-rw-rw-   0        0        0     8098 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyze_suggestion.py
+-rw-rw-rw-   0        0        0     9168 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyzed_column_description.py
+-rw-rw-rw-   0        0        0     6461 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyzed_result.py
+-rw-rw-rw-   0        0        0    13139 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/analyzed_table_description.py
+-rw-rw-rw-   0        0        0    26547 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/arc_shape.py
+-rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/arc_shape_response.py
+-rw-rw-rw-   0        0        0     7072 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/area.py
+-rw-rw-rw-   0        0        0     6264 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_filter.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_filter_response.py
+-rw-rw-rw-   0        0        0     8740 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/auto_fitter_options.py
+-rw-rw-rw-   0        0        0    22619 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_shape.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_shape_response.py
+-rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_shapes.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/auto_shapes_response.py
+-rw-rw-rw-   0        0        0    23440 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/axis.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/axis_response.py
+-rw-rw-rw-   0        0        0     9433 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/batch_convert_request.py
+-rw-rw-rw-   0        0        0     7012 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/batch_lock_request.py
+-rw-rw-rw-   0        0        0     7596 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/batch_protect_request.py
+-rw-rw-rw-   0        0        0     8849 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/batch_split_request.py
+-rw-rw-rw-   0        0        0     6224 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/border.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/border_response.py
+-rw-rw-rw-   0        0        0    22601 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/button.py
+-rw-rw-rw-   0        0        0     5102 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/button_response.py
+-rw-rw-rw-   0        0        0     5176 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/calculate_formula_response.py
+-rw-rw-rw-   0        0        0     7951 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/calculation_options.py
+-rw-rw-rw-   0        0        0    11535 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cell.py
+-rw-rw-rw-   0        0        0     5762 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cell_area.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cell_response.py
+-rw-rw-rw-   0        0        0     6464 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cell_value.py
+-rw-rw-rw-   0        0        0     6932 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells.py
+-rw-rw-rw-   0        0        0     5537 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_cloud_file_info.py
+-rw-rw-rw-   0        0        0     5253 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_cloud_file_info_response.py
+-rw-rw-rw-   0        0        0     4726 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_cloud_response.py
+-rw-rw-rw-   0        0        0     7495 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_color.py
+-rw-rw-rw-   0        0        0     4670 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_document_properties.py
+-rw-rw-rw-   0        0        0     5458 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_document_properties_response.py
+-rw-rw-rw-   0        0        0     6769 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_document_property.py
+-rw-rw-rw-   0        0        0     5410 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_document_property_response.py
+-rw-rw-rw-   0        0        0    22637 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_drawing.py
+-rw-rw-rw-   0        0        0     5144 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_drawing_response.py
+-rw-rw-rw-   0        0        0     6531 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/cells_object_operate_task_parameter.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/cells_response.py
+-rw-rw-rw-   0        0        0    26326 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart.py
+-rw-rw-rw-   0        0        0     9800 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_area.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_area_response.py
+-rw-rw-rw-   0        0        0     8702 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_data_table.py
+-rw-rw-rw-   0        0        0     5343 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_data_table_response.py
+-rw-rw-rw-   0        0        0     9806 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_frame.py
+-rw-rw-rw-   0        0        0     3982 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_globalization_settings.py
+-rw-rw-rw-   0        0        0    10280 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_operate_parameter.py
+-rw-rw-rw-   0        0        0     7723 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_point.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_point_response.py
+-rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_points.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_points_response.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_response.py
+-rw-rw-rw-   0        0        0    22625 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/chart_shape.py
+-rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/charts.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/charts_response.py
+-rw-rw-rw-   0        0        0    23958 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/check_box.py
+-rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/check_box_response.py
+-rw-rw-rw-   0        0        0     5170 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/color.py
+-rw-rw-rw-   0        0        0     6656 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/color_filter.py
+-rw-rw-rw-   0        0        0     5543 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/color_filter_request.py
+-rw-rw-rw-   0        0        0     6692 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/color_scale.py
+-rw-rw-rw-   0        0        0     6405 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/column.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/column_response.py
+-rw-rw-rw-   0        0        0     5789 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/columns.py
+-rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/columns_response.py
+-rw-rw-rw-   0        0        0    25729 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/combo_box.py
+-rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/combo_box_response.py
+-rw-rw-rw-   0        0        0     9830 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comment.py
+-rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comment_response.py
+-rw-rw-rw-   0        0        0    23076 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comment_shape.py
+-rw-rw-rw-   0        0        0     5178 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comment_shape_response.py
+-rw-rw-rw-   0        0        0     4782 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comments.py
+-rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/comments_response.py
+-rw-rw-rw-   0        0        0     5346 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formatting.py
+-rw-rw-rw-   0        0        0     5232 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_icon.py
+-rw-rw-rw-   0        0        0     5495 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_response.py
+-rw-rw-rw-   0        0        0     5171 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_value.py
+-rw-rw-rw-   0        0        0     5527 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formattings.py
+-rw-rw-rw-   0        0        0     5519 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/conditional_formattings_response.py
+-rw-rw-rw-   0        0        0     4697 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/convert_parameter.py
+-rw-rw-rw-   0        0        0     6424 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/convert_task_parameter.py
+-rw-rw-rw-   0        0        0     8976 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/convert_worksheet_task_parameter.py
+-rw-rw-rw-   0        0        0     8164 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/copy_options.py
+-rw-rw-rw-   0        0        0     7769 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/create_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4404 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/criteria_multiple_filter.py
+-rw-rw-rw-   0        0        0     4994 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/custom_filter.py
+-rw-rw-rw-   0        0        0     5477 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/custom_parser_config.py
+-rw-rw-rw-   0        0        0     9798 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_bar.py
+-rw-rw-rw-   0        0        0     4681 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_bar_border.py
+-rw-rw-rw-   0        0        0     5342 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_cleansing.py
+-rw-rw-rw-   0        0        0     6569 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_cleansing_request.py
+-rw-rw-rw-   0        0        0     5028 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_column_fill_value.py
+-rw-rw-rw-   0        0        0     6701 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_deduplication_request.py
+-rw-rw-rw-   0        0        0     5793 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_fill.py
+-rw-rw-rw-   0        0        0     6449 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_fill_request.py
+-rw-rw-rw-   0        0        0     6633 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/data_fill_value.py
+-rw-rw-rw-   0        0        0     4817 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/data_item.py
+-rw-rw-rw-   0        0        0    20157 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_labels.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_labels_response.py
+-rw-rw-rw-   0        0        0     6951 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_sorter.py
+-rw-rw-rw-   0        0        0     6436 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/data_sorter_key.py
+-rw-rw-rw-   0        0        0     4930 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/data_source.py
+-rw-rw-rw-   0        0        0     6368 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/data_transformation_request.py
+-rw-rw-rw-   0        0        0     6974 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/date_time_group_item.py
+-rw-rw-rw-   0        0        0     4999 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/deduplication_region.py
+-rw-rw-rw-   0        0        0     6474 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/delete_incomplete_rows_request.py
+-rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/dif_save_options.py
+-rw-rw-rw-   0        0        0     7488 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/digital_signature.py
+-rw-rw-rw-   0        0        0     4823 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/disc_usage.py
+-rw-rw-rw-   0        0        0     6486 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/discover_chart.py
+-rw-rw-rw-   0        0        0     7470 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/discover_pivot_table.py
+-rw-rw-rw-   0        0        0    13288 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/display_unit_label.py
+-rw-rw-rw-   0        0        0     5391 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/display_unit_label_response.py
+-rw-rw-rw-   0        0        0    20165 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/docx_save_options.py
+-rw-rw-rw-   0        0        0     5049 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/drop_bars.py
+-rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/drop_bars_response.py
+-rw-rw-rw-   0        0        0     5396 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/dynamic_filter.py
+-rw-rw-rw-   0        0        0     3856 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/error.py
+-rw-rw-rw-   0        0        0    16604 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/error_bar.py
+-rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/error_bar_response.py
+-rw-rw-rw-   0        0        0     3898 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/error_details.py
+-rw-rw-rw-   0        0        0     5197 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/excel_data_statistics.py
+-rw-rw-rw-   0        0        0     5299 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/file_info.py
+-rw-rw-rw-   0        0        0     4930 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/file_source.py
+-rw-rw-rw-   0        0        0     6978 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/file_version.py
+-rw-rw-rw-   0        0        0     4307 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/file_versions.py
+-rw-rw-rw-   0        0        0     4289 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/files_list.py
+-rw-rw-rw-   0        0        0     4298 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/files_result.py
+-rw-rw-rw-   0        0        0     4802 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/files_upload_result.py
+-rw-rw-rw-   0        0        0     6819 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/fill_format.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/fill_format_response.py
+-rw-rw-rw-   0        0        0     8728 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/filter_column.py
+-rw-rw-rw-   0        0        0     5574 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/find_response.py
+-rw-rw-rw-   0        0        0     7493 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/floor.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/floor_response.py
+-rw-rw-rw-   0        0        0     8450 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/font.py
+-rw-rw-rw-   0        0        0     6086 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/font_setting.py
+-rw-rw-rw-   0        0        0    31682 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/form.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/form_response.py
+-rw-rw-rw-   0        0        0    10606 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/format_condition.py
+-rw-rw-rw-   0        0        0     4713 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/forms.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/forms_response.py
+-rw-rw-rw-   0        0        0     5300 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/formula_format_condition.py
+-rw-rw-rw-   0        0        0    10839 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/formula_settings.py
+-rw-rw-rw-   0        0        0     7330 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/globalization_settings.py
+-rw-rw-rw-   0        0        0     6562 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/google_drive_storage_file.py
+-rw-rw-rw-   0        0        0     5876 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/gradient_fill.py
+-rw-rw-rw-   0        0        0     5287 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/gradient_fill_stop.py
+-rw-rw-rw-   0        0        0    23028 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/group_box.py
+-rw-rw-rw-   0        0        0     5116 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/group_box_response.py
+-rw-rw-rw-   0        0        0    22625 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/group_shape.py
+-rw-rw-rw-   0        0        0     5297 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/horizontal_page_break.py
+-rw-rw-rw-   0        0        0     5463 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/horizontal_page_break_response.py
+-rw-rw-rw-   0        0        0     4325 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/horizontal_page_breaks.py
+-rw-rw-rw-   0        0        0     5487 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/horizontal_page_breaks_response.py
+-rw-rw-rw-   0        0        0    33972 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/html_save_options.py
+-rw-rw-rw-   0        0        0     6585 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/hyperlink.py
+-rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/hyperlink_response.py
+-rw-rw-rw-   0        0        0     5225 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/hyperlinks.py
+-rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/hyperlinks_response.py
+-rw-rw-rw-   0        0        0     4845 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/icon_filter.py
+-rw-rw-rw-   0        0        0     6677 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/icon_set.py
+-rw-rw-rw-   0        0        0    19550 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/image_or_print_options.py
+-rw-rw-rw-   0        0        0    15645 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/image_save_options.py
+-rw-rw-rw-   0        0        0     8030 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import2_dimension_double_array_option.py
+-rw-rw-rw-   0        0        0     8010 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import2_dimension_int_array_option.py
+-rw-rw-rw-   0        0        0     8028 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import2_dimension_string_array_option.py
+-rw-rw-rw-   0        0        0     7084 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_batch_data_option.py
+-rw-rw-rw-   0        0        0     9860 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_csv_data_option.py
+-rw-rw-rw-   0        0        0     6744 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_data_task_parameter.py
+-rw-rw-rw-   0        0        0     8469 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_double_array_option.py
+-rw-rw-rw-   0        0        0     8449 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_int_array_option.py
+-rw-rw-rw-   0        0        0     5607 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_json_request.py
+-rw-rw-rw-   0        0        0     6537 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_option.py
+-rw-rw-rw-   0        0        0     9735 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_picture_option.py
+-rw-rw-rw-   0        0        0     5368 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/import_position.py
+-rw-rw-rw-   0        0        0     8467 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_string_array_option.py
+-rw-rw-rw-   0        0        0     5567 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/import_xml_request.py
+-rw-rw-rw-   0        0        0    10629 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/json_save_options.py
+-rw-rw-rw-   0        0        0    22595 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/label.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/label_response.py
+-rw-rw-rw-   0        0        0    10787 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend.py
+-rw-rw-rw-   0        0        0     4896 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend_entries.py
+-rw-rw-rw-   0        0        0     5303 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend_entries_response.py
+-rw-rw-rw-   0        0        0     6264 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend_entry.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend_entry_response.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/legend_response.py
+-rw-rw-rw-   0        0        0    13310 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/line.py
+-rw-rw-rw-   0        0        0    13093 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/line_format.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/line_response.py
+-rw-rw-rw-   0        0        0    26553 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/line_shape.py
+-rw-rw-rw-   0        0        0     5123 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/line_shape_response.py
+-rw-rw-rw-   0        0        0     5368 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/link.py
+-rw-rw-rw-   0        0        0     4271 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/link_element.py
+-rw-rw-rw-   0        0        0    26160 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_box.py
+-rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_box_response.py
+-rw-rw-rw-   0        0        0     6293 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_column.py
+-rw-rw-rw-   0        0        0    16354 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_object.py
+-rw-rw-rw-   0        0        0     5000 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_object_operate_parameter.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_object_response.py
+-rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_objects.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/list_objects_response.py
+-rw-rw-rw-   0        0        0     5748 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/load_data.py
+-rw-rw-rw-   0        0        0    10283 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/load_options.py
+-rw-rw-rw-   0        0        0     5506 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/load_to.py
+-rw-rw-rw-   0        0        0    16670 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/m_html_save_options.py
+-rw-rw-rw-   0        0        0    10167 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/markdown_save_options.py
+-rw-rw-rw-   0        0        0     5669 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/marker.py
+-rw-rw-rw-   0        0        0     5155 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/match_condition_request.py
+-rw-rw-rw-   0        0        0     6155 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/merged_cell.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/merged_cell_response.py
+-rw-rw-rw-   0        0        0     5264 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/merged_cells.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/merged_cells_response.py
+-rw-rw-rw-   0        0        0     3910 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/multiple_filter.py
+-rw-rw-rw-   0        0        0     5080 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/multiple_filters.py
+-rw-rw-rw-   0        0        0     7615 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/name.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/name_response.py
+-rw-rw-rw-   0        0        0     5110 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/names.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/names_response.py
+-rw-rw-rw-   0        0        0     5922 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/negative_bar_format.py
+-rw-rw-rw-   0        0        0     4770 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/object_exist.py
+-rw-rw-rw-   0        0        0     3958 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/object_exists_extensions.py
+-rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ods_save_options.py
+-rw-rw-rw-   0        0        0    26408 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ole_object.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ole_object_response.py
+-rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ole_objects.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ole_objects_response.py
+-rw-rw-rw-   0        0        0    11501 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ooxml_save_options.py
+-rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/operate_object.py
+-rw-rw-rw-   0        0        0     7450 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/operate_object_position.py
+-rw-rw-rw-   0        0        0     4435 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/operate_parameter.py
+-rw-rw-rw-   0        0        0    22589 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/oval.py
+-rw-rw-rw-   0        0        0     5088 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/oval_response.py
+-rw-rw-rw-   0        0        0     7190 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_break_operate_parameter.py
+-rw-rw-rw-   0        0        0     6398 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_section.py
+-rw-rw-rw-   0        0        0     5284 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_sections_response.py
+-rw-rw-rw-   0        0        0    22807 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_setup.py
+-rw-rw-rw-   0        0        0     4976 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_setup_operate_parameter.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/page_setup_response.py
+-rw-rw-rw-   0        0        0    20195 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/paginated_save_options.py
+-rw-rw-rw-   0        0        0     4362 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/password_request.py
+-rw-rw-rw-   0        0        0     5959 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/paste_options.py
+-rw-rw-rw-   0        0        0     8077 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pattern_fill.py
+-rw-rw-rw-   0        0        0    19511 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pdf_save_options.py
+-rw-rw-rw-   0        0        0    10047 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/pdf_security_options.py
+-rw-rw-rw-   0        0        0     6255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pic_format_option.py
+-rw-rw-rw-   0        0        0    25954 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/picture.py
+-rw-rw-rw-   0        0        0     5143 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/picture_response.py
+-rw-rw-rw-   0        0        0     4782 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pictures.py
+-rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pictures_response.py
+-rw-rw-rw-   0        0        0     5111 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_column.py
+-rw-rw-rw-   0        0        0    25716 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_field.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_field_response.py
+-rw-rw-rw-   0        0        0     8549 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_filter.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_filter_response.py
+-rw-rw-rw-   0        0        0     5284 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_filters_response.py
+-rw-rw-rw-   0        0        0     3982 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_globalization_settings.py
+-rw-rw-rw-   0        0        0     5517 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_item.py
+-rw-rw-rw-   0        0        0    44381 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_table.py
+-rw-rw-rw-   0        0        0     4342 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     9002 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_table_operate_parameter.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_table_response.py
+-rw-rw-rw-   0        0        0     4867 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_tables.py
+-rw-rw-rw-   0        0        0     5255 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pivot_tables_response.py
+-rw-rw-rw-   0        0        0    11667 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/plot_area.py
+-rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/plot_area_response.py
+-rw-rw-rw-   0        0        0    22164 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/pptx_save_options.py
+-rw-rw-rw-   0        0        0    14256 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/protect_sheet_parameter.py
+-rw-rw-rw-   0        0        0     7844 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/protect_workbook_request.py
+-rw-rw-rw-   0        0        0    15070 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/protection.py
+-rw-rw-rw-   0        0        0     5549 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/query_data_source.py
+-rw-rw-rw-   0        0        0     6582 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/query_table.py
+-rw-rw-rw-   0        0        0    23997 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/radio_button.py
+-rw-rw-rw-   0        0        0     5137 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/radio_button_response.py
+-rw-rw-rw-   0        0        0     8121 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range.py
+-rw-rw-rw-   0        0        0     5724 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_copy_request.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_response.py
+-rw-rw-rw-   0        0        0     5921 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_set_outline_border_request.py
+-rw-rw-rw-   0        0        0     4742 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_set_style_request.py
+-rw-rw-rw-   0        0        0     4891 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_sort_request.py
+-rw-rw-rw-   0        0        0     5214 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/range_value_response.py
+-rw-rw-rw-   0        0        0     4349 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ranges.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/ranges_response.py
+-rw-rw-rw-   0        0        0    22649 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rectangle_shape.py
+-rw-rw-rw-   0        0        0     5158 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rectangle_shape_response.py
+-rw-rw-rw-   0        0        0     5859 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rendering_font.py
+-rw-rw-rw-   0        0        0     9081 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rendering_watermark.py
+-rw-rw-rw-   0        0        0     5488 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/result_destination.py
+-rw-rw-rw-   0        0        0     7452 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/row.py
+-rw-rw-rw-   0        0        0     5047 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/row_response.py
+-rw-rw-rw-   0        0        0     5618 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rows.py
+-rw-rw-rw-   0        0        0     5071 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/rows_response.py
+-rw-rw-rw-   0        0        0     5504 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/save_files_to_cloud_result.py
+-rw-rw-rw-   0        0        0     5567 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/save_files_to_cloud_result_response.py
+-rw-rw-rw-   0        0        0     8556 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/save_options.py
+-rw-rw-rw-   0        0        0     5195 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/save_response.py
+-rw-rw-rw-   0        0        0     4370 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/save_result.py
+-rw-rw-rw-   0        0        0     5125 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/save_result_task_parameter.py
+-rw-rw-rw-   0        0        0    25940 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/scroll_bar.py
+-rw-rw-rw-   0        0        0     5123 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/scroll_bar_response.py
+-rw-rw-rw-   0        0        0    28722 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/series.py
+-rw-rw-rw-   0        0        0     6548 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/series_items.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/series_response.py
+-rw-rw-rw-   0        0        0     5170 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/serieses_response.py
+-rw-rw-rw-   0        0        0     6929 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shadow_effect.py
+-rw-rw-rw-   0        0        0    22595 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shape.py
+-rw-rw-rw-   0        0        0     4864 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shape_operate_parameter.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shape_response.py
+-rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shapes.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/shapes_response.py
+-rw-rw-rw-   0        0        0     4768 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/single_value.py
+-rw-rw-rw-   0        0        0     5137 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/single_value_response.py
+-rw-rw-rw-   0        0        0     7437 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/smart_marker_task_parameter.py
+-rw-rw-rw-   0        0        0     5300 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/solid_fill.py
+-rw-rw-rw-   0        0        0     6388 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sort_key.py
+-rw-rw-rw-   0        0        0     5136 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sparkline.py
+-rw-rw-rw-   0        0        0    20368 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sparkline_group.py
+-rw-rw-rw-   0        0        0     5327 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sparkline_group_response.py
+-rw-rw-rw-   0        0        0     4581 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sparkline_groups.py
+-rw-rw-rw-   0        0        0     5351 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sparkline_groups_response.py
+-rw-rw-rw-   0        0        0    24897 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/spinner.py
+-rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/spinner_response.py
+-rw-rw-rw-   0        0        0     4376 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/split_result.py
+-rw-rw-rw-   0        0        0     4665 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/split_result_document.py
+-rw-rw-rw-   0        0        0     5154 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/split_result_response.py
+-rw-rw-rw-   0        0        0     8873 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/split_workbook_task_parameter.py
+-rw-rw-rw-   0        0        0    10626 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/spreadsheet_m_l2003_save_options.py
+-rw-rw-rw-   0        0        0    16432 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/sql_script_save_options.py
+-rw-rw-rw-   0        0        0     4311 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/storage_exist.py
+-rw-rw-rw-   0        0        0     6032 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/storage_file.py
+-rw-rw-rw-   0        0        0    16124 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/style.py
+-rw-rw-rw-   0        0        0    10636 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/style_format_condition.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/style_response.py
+-rw-rw-rw-   0        0        0     4736 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/styles.py
+-rw-rw-rw-   0        0        0     9072 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/svg_save_options.py
+-rw-rw-rw-   0        0        0     5691 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/table_total_request.py
+-rw-rw-rw-   0        0        0     4287 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/task_data.py
+-rw-rw-rw-   0        0        0     4937 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/task_description.py
+-rw-rw-rw-   0        0        0     3904 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/task_parameter.py
+-rw-rw-rw-   0        0        0     3940 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/task_result_parameter.py
+-rw-rw-rw-   0        0        0     4945 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/task_run_result.py
+-rw-rw-rw-   0        0        0     5319 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/task_run_result_response.py
+-rw-rw-rw-   0        0        0    22607 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_box.py
+-rw-rw-rw-   0        0        0     5109 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_box_response.py
+-rw-rw-rw-   0        0        0     5662 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_format_condition.py
+-rw-rw-rw-   0        0        0     4633 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_item.py
+-rw-rw-rw-   0        0        0     5183 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_item_response.py
+-rw-rw-rw-   0        0        0     4818 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_items.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_items_response.py
+-rw-rw-rw-   0        0        0    11179 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_options.py
+-rw-rw-rw-   0        0        0     6075 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/text_water_marker_request.py
+-rw-rw-rw-   0        0        0     6778 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/texture_fill.py
+-rw-rw-rw-   0        0        0     4747 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/theme_color.py
+-rw-rw-rw-   0        0        0     9968 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/tick_labels.py
+-rw-rw-rw-   0        0        0     5231 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/tick_labels_response.py
+-rw-rw-rw-   0        0        0     6711 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/tile_pic_option.py
+-rw-rw-rw-   0        0        0     4472 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/time_period_format_condition.py
+-rw-rw-rw-   0        0        0    13704 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/title.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/title_response.py
+-rw-rw-rw-   0        0        0     5181 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/top10.py
+-rw-rw-rw-   0        0        0     5631 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/top10_filter.py
+-rw-rw-rw-   0        0        0     4990 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/transformation.py
+-rw-rw-rw-   0        0        0    19370 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/trendline.py
+-rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/trendline_response.py
+-rw-rw-rw-   0        0        0     4828 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/trendlines.py
+-rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/trendlines_response.py
+-rw-rw-rw-   0        0        0    10636 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/txt_save_options.py
+-rw-rw-rw-   0        0        0     5671 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/models/unpivot_column.py
+-rw-rw-rw-   0        0        0    11929 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/validation.py
+-rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/validation_response.py
+-rw-rw-rw-   0        0        0     5248 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/validations.py
+-rw-rw-rw-   0        0        0     5239 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/validations_response.py
+-rw-rw-rw-   0        0        0     5234 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/vertical_page_break.py
+-rw-rw-rw-   0        0        0     5415 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/vertical_page_break_response.py
+-rw-rw-rw-   0        0        0     4313 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/vertical_page_breaks.py
+-rw-rw-rw-   0        0        0     5439 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/vertical_page_breaks_response.py
+-rw-rw-rw-   0        0        0     9595 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/walls.py
+-rw-rw-rw-   0        0        0     5095 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/walls_response.py
+-rw-rw-rw-   0        0        0     9384 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook.py
+-rw-rw-rw-   0        0        0     5469 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_encryption_request.py
+-rw-rw-rw-   0        0        0     4483 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_operate_parameter.py
+-rw-rw-rw-   0        0        0     4988 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_protection_request.py
+-rw-rw-rw-   0        0        0     5643 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_replace_response.py
+-rw-rw-rw-   0        0        0     5167 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_response.py
+-rw-rw-rw-   0        0        0    39915 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_settings.py
+-rw-rw-rw-   0        0        0     5144 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_settings_operate_parameter.py
+-rw-rw-rw-   0        0        0     5223 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbook_settings_response.py
+-rw-rw-rw-   0        0        0     5199 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/workbooks_response.py
+-rw-rw-rw-   0        0        0    20781 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet.py
+-rw-rw-rw-   0        0        0     9532 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet_data_statistics.py
+-rw-rw-rw-   0        0        0     5072 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet_moving_request.py
+-rw-rw-rw-   0        0        0     6365 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet_operate_parameter.py
+-rw-rw-rw-   0        0        0     5666 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet_replace_response.py
+-rw-rw-rw-   0        0        0     5191 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheet_response.py
+-rw-rw-rw-   0        0        0     4828 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheets.py
+-rw-rw-rw-   0        0        0     5215 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/worksheets_response.py
+-rw-rw-rw-   0        0        0     6027 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/write_protection.py
+-rw-rw-rw-   0        0        0     8574 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/xls_save_options.py
+-rw-rw-rw-   0        0        0     8580 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/xlsb_save_options.py
+-rw-rw-rw-   0        0        0     4271 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/xml_data_binding.py
+-rw-rw-rw-   0        0        0     5365 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/xml_map.py
+-rw-rw-rw-   0        0        0    20159 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/models/xps_save_options.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:28.655786 asposecellscloud-24.4/asposecellscloud/requests/
+-rw-rw-rw-   0        0        0    35433 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/requests/__init__.py
+-rw-rw-rw-   0        0        0     4290 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/copy_file_request.py
+-rw-rw-rw-   0        0        0     4137 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/copy_folder_request.py
+-rw-rw-rw-   0        0        0     3513 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/create_folder_request.py
+-rw-rw-rw-   0        0        0     4058 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_decrypt_workbook_request.py
+-rw-rw-rw-   0        0        0     3715 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_document_properties_request.py
+-rw-rw-rw-   0        0        0     4246 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_document_property_request.py
+-rw-rw-rw-   0        0        0     3745 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py
+-rw-rw-rw-   0        0        0     3671 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_file_request.py
+-rw-rw-rw-   0        0        0     3674 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_folder_request.py
+-rw-rw-rw-   0        0        0     4092 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_header_footer_request.py
+-rw-rw-rw-   0        0        0     4450 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4241 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_horizontal_page_breaks_request.py
+-rw-rw-rw-   0        0        0     4250 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_metadata_request.py
+-rw-rw-rw-   0        0        0     5464 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4072 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_un_protect_workbook_request.py
+-rw-rw-rw-   0        0        0     4518 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_unprotect_worksheet_request.py
+-rw-rw-rw-   0        0        0     4438 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4249 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_vertical_page_breaks_request.py
+-rw-rw-rw-   0        0        0     3707 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_background_request.py
+-rw-rw-rw-   0        0        0     4049 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_name_request.py
+-rw-rw-rw-   0        0        0     3687 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_names_request.py
+-rw-rw-rw-   0        0        0     4103 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_background_request.py
+-rw-rw-rw-   0        0        0     4785 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_cells_range_request.py
+-rw-rw-rw-   0        0        0     4506 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4466 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4083 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_charts_request.py
+-rw-rw-rw-   0        0        0     5285 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4458 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4093 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_comments_request.py
+-rw-rw-rw-   0        0        0     5828 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py
+-rw-rw-rw-   0        0        0     4507 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     4165 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py
+-rw-rw-rw-   0        0        0     5804 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_date_filter_request.py
+-rw-rw-rw-   0        0        0     4636 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_filter_request.py
+-rw-rw-rw-   0        0        0     5624 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py
+-rw-rw-rw-   0        0        0     4530 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     4103 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py
+-rw-rw-rw-   0        0        0     4557 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4110 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_list_objects_request.py
+-rw-rw-rw-   0        0        0     4541 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4105 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_ole_objects_request.py
+-rw-rw-rw-   0        0        0     4498 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_picture_request.py
+-rw-rw-rw-   0        0        0     4093 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pictures_request.py
+-rw-rw-rw-   0        0        0     5207 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4812 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py
+-rw-rw-rw-   0        0        0     4557 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4110 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py
+-rw-rw-rw-   0        0        0     4050 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_request.py
+-rw-rw-rw-   0        0        0     4440 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4804 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     4458 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     4083 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_shapes_request.py
+-rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4130 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py
+-rw-rw-rw-   0        0        0     4546 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4108 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_validations_request.py
+-rw-rw-rw-   0        0        0     3849 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/delete_worksheets_request.py
+-rw-rw-rw-   0        0        0     3678 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/download_file_request.py
+-rw-rw-rw-   0        0        0     4426 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_cell_html_string_request.py
+-rw-rw-rw-   0        0        0     3073 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_cells_cloud_service_status_request.py
+-rw-rw-rw-   0        0        0     3072 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py
+-rw-rw-rw-   0        0        0     4467 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_border_request.py
+-rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_fill_format_request.py
+-rw-rw-rw-   0        0        0     4432 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_request.py
+-rw-rw-rw-   0        0        0     4473 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_category_axis_request.py
+-rw-rw-rw-   0        0        0     4512 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_second_category_axis_request.py
+-rw-rw-rw-   0        0        0     4494 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_second_value_axis_request.py
+-rw-rw-rw-   0        0        0     4461 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_series_axis_request.py
+-rw-rw-rw-   0        0        0     4455 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_chart_value_axis_request.py
+-rw-rw-rw-   0        0        0     3212 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_disc_usage_request.py
+-rw-rw-rw-   0        0        0     3844 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_document_properties_request.py
+-rw-rw-rw-   0        0        0     4114 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_document_property_request.py
+-rw-rw-rw-   0        0        0     3536 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_file_versions_request.py
+-rw-rw-rw-   0        0        0     3340 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_files_list_request.py
+-rw-rw-rw-   0        0        0     4042 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_footer_request.py
+-rw-rw-rw-   0        0        0     4042 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_header_request.py
+-rw-rw-rw-   0        0        0     4441 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4114 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_horizontal_page_breaks_request.py
+-rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_metadata_request.py
+-rw-rw-rw-   0        0        0     4068 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_named_range_value_request.py
+-rw-rw-rw-   0        0        0     3677 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_named_ranges_request.py
+-rw-rw-rw-   0        0        0     3652 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_page_count_request.py
+-rw-rw-rw-   0        0        0     4046 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_page_setup_request.py
+-rw-rw-rw-   0        0        0     5403 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4427 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4102 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_vertical_page_breaks_request.py
+-rw-rw-rw-   0        0        0     3699 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_default_style_request.py
+-rw-rw-rw-   0        0        0     4028 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_name_request.py
+-rw-rw-rw-   0        0        0     4062 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_name_value_request.py
+-rw-rw-rw-   0        0        0     3670 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_names_request.py
+-rw-rw-rw-   0        0        0     5530 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_request.py
+-rw-rw-rw-   0        0        0     3693 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_settings_request.py
+-rw-rw-rw-   0        0        0     3691 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_workbook_text_items_request.py
+-rw-rw-rw-   0        0        0     4090 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_auto_filter_request.py
+-rw-rw-rw-   0        0        0     4704 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py
+-rw-rw-rw-   0        0        0     4088 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_autoshapes_request.py
+-rw-rw-rw-   0        0        0     4481 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4503 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cell_request.py
+-rw-rw-rw-   0        0        0     4451 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cell_style_request.py
+-rw-rw-rw-   0        0        0     4936 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cells_range_value_request.py
+-rw-rw-rw-   0        0        0     4332 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cells_request.py
+-rw-rw-rw-   0        0        0     4484 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4584 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4477 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4064 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_charts_request.py
+-rw-rw-rw-   0        0        0     4466 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_column_request.py
+-rw-rw-rw-   0        0        0     3951 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4437 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4076 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_comments_request.py
+-rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     4162 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py
+-rw-rw-rw-   0        0        0     4511 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     4088 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_hyperlinks_request.py
+-rw-rw-rw-   0        0        0     4649 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_list_objects_request.py
+-rw-rw-rw-   0        0        0     4539 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_merged_cell_request.py
+-rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_merged_cells_request.py
+-rw-rw-rw-   0        0        0     4621 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4090 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_ole_objects_request.py
+-rw-rw-rw-   0        0        0     4070 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_page_count_request.py
+-rw-rw-rw-   0        0        0     4888 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_picture_with_format_request.py
+-rw-rw-rw-   0        0        0     4076 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pictures_request.py
+-rw-rw-rw-   0        0        0     4993 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4592 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py
+-rw-rw-rw-   0        0        0     4531 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4096 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_tables_request.py
+-rw-rw-rw-   0        0        0     4415 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4333 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     4435 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     4064 2024-01-16 20:47:48.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_shapes_request.py
+-rw-rw-rw-   0        0        0     4549 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4120 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py
+-rw-rw-rw-   0        0        0     4084 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_text_items_request.py
+-rw-rw-rw-   0        0        0     4528 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4094 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_validations_request.py
+-rw-rw-rw-   0        0        0     4942 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_with_format_request.py
+-rw-rw-rw-   0        0        0     3670 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/get_worksheets_request.py
+-rw-rw-rw-   0        0        0     4290 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/move_file_request.py
+-rw-rw-rw-   0        0        0     4137 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/move_folder_request.py
+-rw-rw-rw-   0        0        0     3686 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/object_exists_request.py
+-rw-rw-rw-   0        0        0     3491 2024-02-22 10:48:54.000000 asposecellscloud-24.4/asposecellscloud/requests/post_analyze_excel_request.py
+-rw-rw-rw-   0        0        0     4621 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_assemble_request.py
+-rw-rw-rw-   0        0        0     4054 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_autofit_workbook_columns_request.py
+-rw-rw-rw-   0        0        0     4163 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_autofit_workbook_rows_request.py
+-rw-rw-rw-   0        0        0     4610 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5265 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4559 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3481 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_batch_convert_request.py
+-rw-rw-rw-   0        0        0     3445 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_batch_lock_request.py
+-rw-rw-rw-   0        0        0     3481 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_batch_protect_request.py
+-rw-rw-rw-   0        0        0     3457 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_batch_split_request.py
+-rw-rw-rw-   0        0        0     3453 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_batch_unlock_request.py
+-rw-rw-rw-   0        0        0     4565 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_cell_calculate_request.py
+-rw-rw-rw-   0        0        0     4571 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_cell_characters_request.py
+-rw-rw-rw-   0        0        0     4798 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_chart_category_axis_request.py
+-rw-rw-rw-   0        0        0     4844 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_chart_second_category_axis_request.py
+-rw-rw-rw-   0        0        0     4823 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_chart_second_value_axis_request.py
+-rw-rw-rw-   0        0        0     4784 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_chart_series_axis_request.py
+-rw-rw-rw-   0        0        0     4777 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_chart_value_axis_request.py
+-rw-rw-rw-   0        0        0     4852 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_clear_contents_request.py
+-rw-rw-rw-   0        0        0     4847 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_clear_formats_request.py
+-rw-rw-rw-   0        0        0     4801 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_clear_objects_request.py
+-rw-rw-rw-   0        0        0     4776 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_column_style_request.py
+-rw-rw-rw-   0        0        0     4133 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_compress_request.py
+-rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_csv_request.py
+-rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_docx_request.py
+-rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_html_request.py
+-rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_json_request.py
+-rw-rw-rw-   0        0        0     4145 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py
+-rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py
+-rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_png_request.py
+-rw-rw-rw-   0        0        0     4129 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py
+-rw-rw-rw-   0        0        0     4125 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_sql_request.py
+-rw-rw-rw-   0        0        0     5290 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_copy_cell_into_cell_request.py
+-rw-rw-rw-   0        0        0     5652 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5164 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_request.py
+-rw-rw-rw-   0        0        0     5547 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3496 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_data_cleansing_request.py
+-rw-rw-rw-   0        0        0     3544 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_data_deduplication_request.py
+-rw-rw-rw-   0        0        0     3436 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_data_fill_request.py
+-rw-rw-rw-   0        0        0     3556 2024-04-28 05:57:35.000000 asposecellscloud-24.4/asposecellscloud/requests/post_data_transformation_request.py
+-rw-rw-rw-   0        0        0     3589 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_delete_incomplete_rows_request.py
+-rw-rw-rw-   0        0        0     4533 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_digital_signature_request.py
+-rw-rw-rw-   0        0        0     4048 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_encrypt_workbook_request.py
+-rw-rw-rw-   0        0        0     4387 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_export_request.py
+-rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_fit_tall_to_pages_request.py
+-rw-rw-rw-   0        0        0     4091 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_fit_wide_to_pages_request.py
+-rw-rw-rw-   0        0        0     5117 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_footer_request.py
+-rw-rw-rw-   0        0        0     5021 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_group_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5000 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_group_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5117 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_header_request.py
+-rw-rw-rw-   0        0        0     4922 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_hide_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4839 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_hide_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3972 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_import_data_request.py
+-rw-rw-rw-   0        0        0     4241 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_import_request.py
+-rw-rw-rw-   0        0        0     3888 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_lock_request.py
+-rw-rw-rw-   0        0        0     4443 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_merge_request.py
+-rw-rw-rw-   0        0        0     4549 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_metadata_request.py
+-rw-rw-rw-   0        0        0     4391 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_move_worksheet_request.py
+-rw-rw-rw-   0        0        0     4404 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_page_setup_request.py
+-rw-rw-rw-   0        0        0     5756 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_cell_style_request.py
+-rw-rw-rw-   0        0        0     6386 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py
+-rw-rw-rw-   0        0        0     5634 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_field_move_to_request.py
+-rw-rw-rw-   0        0        0     5058 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_style_request.py
+-rw-rw-rw-   0        0        0     6086 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py
+-rw-rw-rw-   0        0        0     5635 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py
+-rw-rw-rw-   0        0        0     4048 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_protect_request.py
+-rw-rw-rw-   0        0        0     4160 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_protect_workbook_request.py
+-rw-rw-rw-   0        0        0     4426 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_rename_worksheet_request.py
+-rw-rw-rw-   0        0        0     3709 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_repair_request.py
+-rw-rw-rw-   0        0        0     4761 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_replace_request.py
+-rw-rw-rw-   0        0        0     4624 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_reverse_request.py
+-rw-rw-rw-   0        0        0     4619 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_rotate_request.py
+-rw-rw-rw-   0        0        0     4725 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_row_style_request.py
+-rw-rw-rw-   0        0        0     3363 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_run_task_request.py
+-rw-rw-rw-   0        0        0     4415 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_search_request.py
+-rw-rw-rw-   0        0        0     4465 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_set_cell_html_string_request.py
+-rw-rw-rw-   0        0        0     5119 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_set_cell_range_value_request.py
+-rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_set_worksheet_column_width_request.py
+-rw-rw-rw-   0        0        0     4691 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_split_request.py
+-rw-rw-rw-   0        0        0     4907 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     5025 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5070 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_unhide_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4993 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_unhide_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     3898 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_unlock_request.py
+-rw-rw-rw-   0        0        0     4824 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_cell_style_request.py
+-rw-rw-rw-   0        0        0     4875 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     4427 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_property_request.py
+-rw-rw-rw-   0        0        0     4799 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_range_style_request.py
+-rw-rw-rw-   0        0        0     4735 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4429 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_zoom_request.py
+-rw-rw-rw-   0        0        0     4900 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_watermark_request.py
+-rw-rw-rw-   0        0        0     4026 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4631 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_cleansing_request.py
+-rw-rw-rw-   0        0        0     4699 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_deduplication_request.py
+-rw-rw-rw-   0        0        0     4566 2024-03-22 07:23:40.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_fill_request.py
+-rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_export_xml_request.py
+-rw-rw-rw-   0        0        0     4219 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py
+-rw-rw-rw-   0        0        0     5001 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_import_json_request.py
+-rw-rw-rw-   0        0        0     4988 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_import_xml_request.py
+-rw-rw-rw-   0        0        0     4378 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_name_request.py
+-rw-rw-rw-   0        0        0     5719 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_save_as_request.py
+-rw-rw-rw-   0        0        0     4034 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_settings_request.py
+-rw-rw-rw-   0        0        0     5068 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_split_request.py
+-rw-rw-rw-   0        0        0     4459 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbook_text_replace_request.py
+-rw-rw-rw-   0        0        0     4274 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbooks_merge_request.py
+-rw-rw-rw-   0        0        0     4031 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_workbooks_text_search_request.py
+-rw-rw-rw-   0        0        0     4133 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_calculate_formula_request.py
+-rw-rw-rw-   0        0        0     4876 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cell_set_value_request.py
+-rw-rw-rw-   0        0        0     4840 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py
+-rw-rw-rw-   0        0        0     4448 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py
+-rw-rw-rw-   0        0        0     5232 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py
+-rw-rw-rw-   0        0        0     4563 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py
+-rw-rw-rw-   0        0        0     4826 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py
+-rw-rw-rw-   0        0        0     4546 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_sort_request.py
+-rw-rw-rw-   0        0        0     4512 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_style_request.py
+-rw-rw-rw-   0        0        0     4463 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py
+-rw-rw-rw-   0        0        0     5126 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_value_request.py
+-rw-rw-rw-   0        0        0     4511 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_ranges_copy_request.py
+-rw-rw-rw-   0        0        0     4826 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     4771 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4811 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     4781 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4460 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_group_shape_request.py
+-rw-rw-rw-   0        0        0     4871 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     5329 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_column_request.py
+-rw-rw-rw-   0        0        0     5046 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_columns_total_request.py
+-rw-rw-rw-   0        0        0     4639 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py
+-rw-rw-rw-   0        0        0     5473 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_insert_slicer_request.py
+-rw-rw-rw-   0        0        0     4648 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_remove_duplicates_request.py
+-rw-rw-rw-   0        0        0     4916 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     4983 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py
+-rw-rw-rw-   0        0        0     5661 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py
+-rw-rw-rw-   0        0        0     4505 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_match_blanks_request.py
+-rw-rw-rw-   0        0        0     4526 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py
+-rw-rw-rw-   0        0        0     5622 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_merge_request.py
+-rw-rw-rw-   0        0        0     4821 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_picture_request.py
+-rw-rw-rw-   0        0        0     4603 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py
+-rw-rw-rw-   0        0        0     5021 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py
+-rw-rw-rw-   0        0        0     4829 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_range_sort_request.py
+-rw-rw-rw-   0        0        0     4747 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     5016 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4858 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_text_replace_request.py
+-rw-rw-rw-   0        0        0     4423 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_text_search_request.py
+-rw-rw-rw-   0        0        0     4492 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py
+-rw-rw-rw-   0        0        0     5640 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_unmerge_request.py
+-rw-rw-rw-   0        0        0     4896 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     4068 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_active_worksheet_request.py
+-rw-rw-rw-   0        0        0     4373 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_add_new_worksheet_request.py
+-rw-rw-rw-   0        0        0     4500 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_change_visibility_worksheet_request.py
+-rw-rw-rw-   0        0        0     5253 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_convert_workbook_request.py
+-rw-rw-rw-   0        0        0     4047 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_document_property_request.py
+-rw-rw-rw-   0        0        0     4080 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_document_protect_from_changes_request.py
+-rw-rw-rw-   0        0        0     4852 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_horizontal_page_break_request.py
+-rw-rw-rw-   0        0        0     4973 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_insert_new_worksheet_request.py
+-rw-rw-rw-   0        0        0     5067 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_columns_request.py
+-rw-rw-rw-   0        0        0     4455 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_row_request.py
+-rw-rw-rw-   0        0        0     4819 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_rows_request.py
+-rw-rw-rw-   0        0        0     5644 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_pivot_table_field_request.py
+-rw-rw-rw-   0        0        0     4490 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_protect_worksheet_request.py
+-rw-rw-rw-   0        0        0     4806 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_vertical_page_break_request.py
+-rw-rw-rw-   0        0        0     4182 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_workbook_background_request.py
+-rw-rw-rw-   0        0        0     4430 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_workbook_create_request.py
+-rw-rw-rw-   0        0        0     4010 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_workbook_name_request.py
+-rw-rw-rw-   0        0        0     4182 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_workbook_water_marker_request.py
+-rw-rw-rw-   0        0        0     5182 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_add_picture_request.py
+-rw-rw-rw-   0        0        0     4575 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_background_request.py
+-rw-rw-rw-   0        0        0     4764 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_cells_range_request.py
+-rw-rw-rw-   0        0        0     4488 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_legend_request.py
+-rw-rw-rw-   0        0        0     6876 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_request.py
+-rw-rw-rw-   0        0        0     4599 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_title_request.py
+-rw-rw-rw-   0        0        0     5539 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_color_filter_request.py
+-rw-rw-rw-   0        0        0     4771 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_comment_request.py
+-rw-rw-rw-   0        0        0     4944 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py
+-rw-rw-rw-   0        0        0     6443 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_custom_filter_request.py
+-rw-rw-rw-   0        0        0     6443 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_date_filter_request.py
+-rw-rw-rw-   0        0        0     5640 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py
+-rw-rw-rw-   0        0        0     5482 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_filter_request.py
+-rw-rw-rw-   0        0        0     6276 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_filter_top10_request.py
+-rw-rw-rw-   0        0        0     4871 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_area_request.py
+-rw-rw-rw-   0        0        0     6049 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py
+-rw-rw-rw-   0        0        0     6330 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_request.py
+-rw-rw-rw-   0        0        0     5597 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_freeze_panes_request.py
+-rw-rw-rw-   0        0        0     5999 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_hyperlink_request.py
+-rw-rw-rw-   0        0        0     5918 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_icon_filter_request.py
+-rw-rw-rw-   0        0        0     5244 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_list_object_request.py
+-rw-rw-rw-   0        0        0     5064 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_ole_object_request.py
+-rw-rw-rw-   0        0        0     5126 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py
+-rw-rw-rw-   0        0        0     4801 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_pivot_table_request.py
+-rw-rw-rw-   0        0        0     5290 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_shape_request.py
+-rw-rw-rw-   0        0        0     5651 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_sparkline_group_request.py
+-rw-rw-rw-   0        0        0     4223 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_validation_request.py
+-rw-rw-rw-   0        0        0     3428 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/storage_exists_request.py
+-rw-rw-rw-   0        0        0     4127 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/requests/upload_file_request.py
+-rw-rw-rw-   0        0        0    14234 2024-01-16 20:47:49.000000 asposecellscloud-24.4/asposecellscloud/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:29.279879 asposecellscloud-24.4/asposecellscloud.egg-info/
+-rw-rw-rw-   0        0        0    17545 2024-04-28 05:59:13.000000 asposecellscloud-24.4/asposecellscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    40765 2024-04-28 05:59:13.000000 asposecellscloud-24.4/asposecellscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 05:59:13.000000 asposecellscloud-24.4/asposecellscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-28 05:59:13.000000 asposecellscloud-24.4/asposecellscloud.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-28 05:59:13.000000 asposecellscloud-24.4/asposecellscloud.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      936 2024-04-28 05:57:35.000000 asposecellscloud-24.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 05:59:29.287972 asposecellscloud-24.4/setup.cfg
+-rw-rw-rw-   0        0        0     1515 2024-04-28 05:57:35.000000 asposecellscloud-24.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 05:59:29.275903 asposecellscloud-24.4/test/
+-rw-rw-rw-   0        0        0     7996 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_auto_filter_controller.py
+-rw-rw-rw-   0        0        0     4635 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_batch_controller.py
+-rw-rw-rw-   0        0        0    21475 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_cells_controller.py
+-rw-rw-rw-   0        0        0     1774 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_cells_status_controller.py
+-rw-rw-rw-   0        0        0     2297 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_chart_area_controller.py
+-rw-rw-rw-   0        0        0     8031 2024-01-16 20:47:49.000000 asposecellscloud-24.4/test/tests_charts_controller.py
+-rw-rw-rw-   0        0        0     5842 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_conditional_formattings_controller.py
+-rw-rw-rw-   0        0        0    47339 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_conversion.py
+-rw-rw-rw-   0        0        0    11416 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_conversion_json.py
+-rw-rw-rw-   0        0        0     8122 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_conversion_png.py
+-rw-rw-rw-   0        0        0     3110 2024-04-28 05:57:35.000000 asposecellscloud-24.4/test/tests_data_processing_controller.py
+-rw-rw-rw-   0        0        0     3361 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_file_controller.py
+-rw-rw-rw-   0        0        0     3094 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_folder_controller.py
+-rw-rw-rw-   0        0        0     3932 2023-12-23 14:58:33.000000 asposecellscloud-24.4/test/tests_hypelinks_controller.py
+-rw-rw-rw-   0        0        0   119156 2024-01-16 20:47:49.000000 asposecellscloud-24.4/test/tests_light_cells.py
+-rw-rw-rw-   0        0        0     8709 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_list_objects_controller.py
+-rw-rw-rw-   0        0        0     4326 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_ole_objects_controller.py
+-rw-rw-rw-   0        0        0     1308 2023-11-25 21:14:26.000000 asposecellscloud-24.4/test/tests_one.py
+-rw-rw-rw-   0        0        0     5884 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_page_breaks_controller.py
+-rw-rw-rw-   0        0        0     5151 2024-01-16 20:47:49.000000 asposecellscloud-24.4/test/tests_page_setup_controller.py
+-rw-rw-rw-   0        0        0     4182 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_pictures_controller.py
+-rw-rw-rw-   0        0        0    12668 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_pivot_tables_controller.py
+-rw-rw-rw-   0        0        0     3363 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_properties_controller.py
+-rw-rw-rw-   0        0        0     9553 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_ranges_controller.py
+-rw-rw-rw-   0        0        0     4970 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_shapes_controller.py
+-rw-rw-rw-   0        0        0     4073 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_sparkline_groups_controller.py
+-rw-rw-rw-   0        0        0     2573 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_storage_controller.py
+-rw-rw-rw-   0        0        0    18942 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_workbook_controller.py
+-rw-rw-rw-   0        0        0    21083 2024-01-16 20:47:49.000000 asposecellscloud-24.4/test/tests_worksheet_controller.py
+-rw-rw-rw-   0        0        0     3912 2023-12-23 14:58:34.000000 asposecellscloud-24.4/test/tests_worksheet_validations_controller.py
+-rw-rw-rw-   0        0        0     2397 2024-04-28 05:57:35.000000 asposecellscloud-24.4/test/tests_xml_controller.py
```

### Comparing `asposecellscloud-24.3/LICENSE` & `asposecellscloud-24.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/PKG-INFO` & `asposecellscloud-24.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: asposecellscloud
-Version: 24.3
+Version: 24.4
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: Aspose Cloud <aspose.cloud@aspose.com>
 Project-URL: Homepage, https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
-Keywords: excel,spreadsheet,xlsx,convert,aspose.cells,cloud
+Keywords: excel,spreadsheet,convert,xlsx,pdf,json,cloud,rest api,merge,split,protect
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
 Requires-Dist: six>=1.10
 Requires-Dist: certifi
 Requires-Dist: python-dateutil
 
-![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.3)
+![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.4)
 
 Aspose.Cells Cloud for Python enables you to handle various aspects of Excel files, including cell data, styles, formulas, charts, pivot tables, data validation, comments, drawing objects, images, hyperlinks, and so on. Additionally, it supports operations such as splitting, merging, repairing, and converting to other compatible file formats.
 
 # Python package for Aspose.Cells Cloud
 
 
 Enhance your Python applications with the [Aspose.Cells Cloud](https://products.aspose.cloud/cells/python) , enabling seamless integration with [Excel, ODS, CSV, Json and other spreadsheet document formats](https://docs.aspose.cloud/cells/supported-file-formats/). With its powerful APIs, developers can effortlessly read, convert, create, edit, and manipulate the contents of Excel documents without the need for any office software installed on the machine.
@@ -40,22 +40,19 @@
 - Data Verification: Includes data verification function to set cell data type, range, uniqueness, ensuring data accuracy and integrity.
 - Batch Processing: Supports batch processing of multiple Excel documents, such as batch format conversion, data extraction, and style application..
 - Import/Export: Facilitates importing data from various sources into spreadsheets and exporting spreadsheet data to other formats.
 - Security Management: Offers a range of security features like data encryption, access control, and permission management to safeguard the security and integrity of spreadsheet data.
 
 
 
-## Feature & Enhancements in Version 24.3
+## Feature & Enhancements in Version 24.4
 
 Full list of issues covering all changes in this release:
 
-- Support data deduplication.
-- Support data filling.
-- Support to delete incomplete rows.
-- Support data cleansing.
+- Support data transformation.
 
 ## Support file format
 
 |**Format**|**Description**|**Load**|**Save**|
 | :- | :- | :- | :- |
 |[XLS](https://docs.fileformat.com/spreadsheet/xls/)|Excel 95/5.0 - 2003 Workbook.|&radic;|&radic;|
 |[XLSX](https://docs.fileformat.com/spreadsheet/xlsx/)|Office Open XML SpreadsheetML Workbook or template file, with or without macros.|&radic;|&radic;|
@@ -145,14 +142,21 @@
 
 
 [Product Page](https://products.aspose.cloud/cells/python) | [Documentation](https://docs.aspose.cloud/cells/) | [Live Demo](https://products.aspose.app/cells/family) | [API Reference](https://apireference.aspose.cloud/cells/) | [Code Samples](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/tree/master/test) | [Blog](https://blog.aspose.cloud/category/cells/) | [Free Support](https://forum.aspose.cloud/c/cells) | [Free Trial](https://dashboard.aspose.cloud/#/apps)
 
 
 # Release history version
 
+## Enhancements in Version 24.3
+
+- Support data deduplication.
+- Support data filling.
+- Support to delete incomplete rows.
+- Support data cleansing.
+
 ## Enhancements in Version 24.2.1
 
 - Support data deduplication.
 
 ## Enhancements in Version 24.1.1
 
 - Fixed spelling mistakes for several functions.
```

### Comparing `asposecellscloud-24.3/README.md` & `asposecellscloud-24.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.3)
+![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.4)
 
 Aspose.Cells Cloud for Python enables you to handle various aspects of Excel files, including cell data, styles, formulas, charts, pivot tables, data validation, comments, drawing objects, images, hyperlinks, and so on. Additionally, it supports operations such as splitting, merging, repairing, and converting to other compatible file formats.
 
 # Python package for Aspose.Cells Cloud
 
 
 Enhance your Python applications with the [Aspose.Cells Cloud](https://products.aspose.cloud/cells/python) , enabling seamless integration with [Excel, ODS, CSV, Json and other spreadsheet document formats](https://docs.aspose.cloud/cells/supported-file-formats/). With its powerful APIs, developers can effortlessly read, convert, create, edit, and manipulate the contents of Excel documents without the need for any office software installed on the machine.
@@ -19,22 +19,19 @@
 - Data Verification: Includes data verification function to set cell data type, range, uniqueness, ensuring data accuracy and integrity.
 - Batch Processing: Supports batch processing of multiple Excel documents, such as batch format conversion, data extraction, and style application..
 - Import/Export: Facilitates importing data from various sources into spreadsheets and exporting spreadsheet data to other formats.
 - Security Management: Offers a range of security features like data encryption, access control, and permission management to safeguard the security and integrity of spreadsheet data.
 
 
 
-## Feature & Enhancements in Version 24.3
+## Feature & Enhancements in Version 24.4
 
 Full list of issues covering all changes in this release:
 
-- Support data deduplication.
-- Support data filling.
-- Support to delete incomplete rows.
-- Support data cleansing.
+- Support data transformation.
 
 ## Support file format
 
 |**Format**|**Description**|**Load**|**Save**|
 | :- | :- | :- | :- |
 |[XLS](https://docs.fileformat.com/spreadsheet/xls/)|Excel 95/5.0 - 2003 Workbook.|&radic;|&radic;|
 |[XLSX](https://docs.fileformat.com/spreadsheet/xlsx/)|Office Open XML SpreadsheetML Workbook or template file, with or without macros.|&radic;|&radic;|
@@ -124,14 +121,21 @@
 
 
 [Product Page](https://products.aspose.cloud/cells/python) | [Documentation](https://docs.aspose.cloud/cells/) | [Live Demo](https://products.aspose.app/cells/family) | [API Reference](https://apireference.aspose.cloud/cells/) | [Code Samples](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/tree/master/test) | [Blog](https://blog.aspose.cloud/category/cells/) | [Free Support](https://forum.aspose.cloud/c/cells) | [Free Trial](https://dashboard.aspose.cloud/#/apps)
 
 
 # Release history version
 
+## Enhancements in Version 24.3
+
+- Support data deduplication.
+- Support data filling.
+- Support to delete incomplete rows.
+- Support data cleansing.
+
 ## Enhancements in Version 24.2.1
 
 - Support data deduplication.
 
 ## Enhancements in Version 24.1.1
 
 - Fixed spelling mistakes for several functions.
```

### Comparing `asposecellscloud-24.3/asposecellscloud/__init__.py` & `asposecellscloud-24.4/asposecellscloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,20 +66,23 @@
 from asposecellscloud.models.custom_filter import CustomFilter
 from asposecellscloud.models.data_bar import DataBar
 from asposecellscloud.models.data_bar_border import DataBarBorder
 from asposecellscloud.models.data_cleansing import DataCleansing
 from asposecellscloud.models.data_column_fill_value import DataColumnFillValue
 from asposecellscloud.models.data_fill import DataFill
 from asposecellscloud.models.data_fill_value import DataFillValue
+from asposecellscloud.models.data_item import DataItem
 from asposecellscloud.models.data_sorter import DataSorter
 from asposecellscloud.models.data_sorter_key import DataSorterKey
+from asposecellscloud.models.data_source import DataSource
 from asposecellscloud.models.date_time_group_item import DateTimeGroupItem
 from asposecellscloud.models.deduplication_region import DeduplicationRegion
 from asposecellscloud.models.dynamic_filter import DynamicFilter
 from asposecellscloud.models.file_info import FileInfo
+from asposecellscloud.models.file_source import FileSource
 from asposecellscloud.models.files_result import FilesResult
 from asposecellscloud.models.filter_column import FilterColumn
 from asposecellscloud.models.font import Font
 from asposecellscloud.models.font_setting import FontSetting
 from asposecellscloud.models.format_condition import FormatCondition
 from asposecellscloud.models.formula_format_condition import FormulaFormatCondition
 from asposecellscloud.models.formula_settings import FormulaSettings
@@ -102,15 +105,14 @@
 from asposecellscloud.models.negative_bar_format import NegativeBarFormat
 from asposecellscloud.models.page_section import PageSection
 from asposecellscloud.models.page_setup import PageSetup
 from asposecellscloud.models.paste_options import PasteOptions
 from asposecellscloud.models.pdf_security_options import PdfSecurityOptions
 from asposecellscloud.models.protection import Protection
 from asposecellscloud.models.protect_sheet_parameter import ProtectSheetParameter
-from asposecellscloud.models.query_table import QueryTable
 from asposecellscloud.models.range import Range
 from asposecellscloud.models.ranges import Ranges
 from asposecellscloud.models.row import Row
 from asposecellscloud.models.rows import Rows
 from asposecellscloud.models.save_result import SaveResult
 from asposecellscloud.models.paginated_save_options import PaginatedSaveOptions
 from asposecellscloud.models.single_value import SingleValue
@@ -138,15 +140,14 @@
 from asposecellscloud.models.worksheets import Worksheets
 from asposecellscloud.models.write_protection import WriteProtection
 from asposecellscloud.models.xml_data_binding import XmlDataBinding
 from asposecellscloud.models.xml_map import XmlMap
 from asposecellscloud.models.cells_object_operate_task_parameter import CellsObjectOperateTaskParameter
 from asposecellscloud.models.convert_task_parameter import ConvertTaskParameter
 from asposecellscloud.models.convert_worksheet_task_parameter import ConvertWorksheetTaskParameter
-from asposecellscloud.models.file_source import FileSource
 from asposecellscloud.models.import_data_task_parameter import ImportDataTaskParameter
 from asposecellscloud.models.result_destination import ResultDestination
 from asposecellscloud.models.save_files_to_cloud_result import SaveFilesToCloudResult
 from asposecellscloud.models.save_result_task_parameter import SaveResultTaskParameter
 from asposecellscloud.models.smart_marker_task_parameter import SmartMarkerTaskParameter
 from asposecellscloud.models.split_workbook_task_parameter import SplitWorkbookTaskParameter
 from asposecellscloud.models.task_data import TaskData
@@ -307,14 +308,15 @@
 from asposecellscloud.models.batch_split_request import BatchSplitRequest
 from asposecellscloud.models.color_filter_request import ColorFilterRequest
 from asposecellscloud.models.convert_parameter import ConvertParameter
 from asposecellscloud.models.create_pivot_table_request import CreatePivotTableRequest
 from asposecellscloud.models.data_cleansing_request import DataCleansingRequest
 from asposecellscloud.models.data_deduplication_request import DataDeduplicationRequest
 from asposecellscloud.models.data_fill_request import DataFillRequest
+from asposecellscloud.models.data_transformation_request import DataTransformationRequest
 from asposecellscloud.models.delete_incomplete_rows_request import DeleteIncompleteRowsRequest
 from asposecellscloud.models.import_json_request import ImportJsonRequest
 from asposecellscloud.models.import_xml_request import ImportXMLRequest
 from asposecellscloud.models.match_condition_request import MatchConditionRequest
 from asposecellscloud.models.password_request import PasswordRequest
 from asposecellscloud.models.pivot_table_field_request import PivotTableFieldRequest
 from asposecellscloud.models.protect_workbook_request import ProtectWorkbookRequest
@@ -326,14 +328,21 @@
 from asposecellscloud.models.text_water_marker_request import TextWaterMarkerRequest
 from asposecellscloud.models.workbook_encryption_request import WorkbookEncryptionRequest
 from asposecellscloud.models.workbook_protection_request import WorkbookProtectionRequest
 from asposecellscloud.models.worksheet_moving_request import WorksheetMovingRequest
 from asposecellscloud.models.image_or_print_options import ImageOrPrintOptions
 from asposecellscloud.models.rendering_font import RenderingFont
 from asposecellscloud.models.rendering_watermark import RenderingWatermark
+from asposecellscloud.models.load_data import LoadData
+from asposecellscloud.models.load_to import LoadTo
+from asposecellscloud.models.pivot_column import PivotColumn
+from asposecellscloud.models.query_data_source import QueryDataSource
+from asposecellscloud.models.query_table import QueryTable
+from asposecellscloud.models.transformation import Transformation
+from asposecellscloud.models.unpivot_column import UnpivotColumn
 from asposecellscloud.models.pivot_field import PivotField
 from asposecellscloud.models.pivot_filter import PivotFilter
 from asposecellscloud.models.pivot_item import PivotItem
 from asposecellscloud.models.pivot_table import PivotTable
 from asposecellscloud.models.pivot_tables import PivotTables
 from asposecellscloud.models.custom_parser_config import CustomParserConfig
 from asposecellscloud.models.import2_dimension_double_array_option import Import2DimensionDoubleArrayOption
@@ -548,14 +557,15 @@
 from asposecellscloud.requests.post_workbook_data_cleansing_request import PostWorkbookDataCleansingRequest
 from asposecellscloud.requests.post_data_cleansing_request import PostDataCleansingRequest
 from asposecellscloud.requests.post_workbook_data_deduplication_request import PostWorkbookDataDeduplicationRequest
 from asposecellscloud.requests.post_data_deduplication_request import PostDataDeduplicationRequest
 from asposecellscloud.requests.post_workbook_data_fill_request import PostWorkbookDataFillRequest
 from asposecellscloud.requests.post_data_fill_request import PostDataFillRequest
 from asposecellscloud.requests.post_delete_incomplete_rows_request import PostDeleteIncompleteRowsRequest
+from asposecellscloud.requests.post_data_transformation_request import PostDataTransformationRequest
 from asposecellscloud.requests.get_worksheet_hyperlinks_request import GetWorksheetHyperlinksRequest
 from asposecellscloud.requests.get_worksheet_hyperlink_request import GetWorksheetHyperlinkRequest
 from asposecellscloud.requests.delete_worksheet_hyperlink_request import DeleteWorksheetHyperlinkRequest
 from asposecellscloud.requests.post_worksheet_hyperlink_request import PostWorksheetHyperlinkRequest
 from asposecellscloud.requests.put_worksheet_hyperlink_request import PutWorksheetHyperlinkRequest
 from asposecellscloud.requests.delete_worksheet_hyperlinks_request import DeleteWorksheetHyperlinksRequest
 from asposecellscloud.requests.post_assemble_request import PostAssembleRequest
```

### Comparing `asposecellscloud-24.3/asposecellscloud/api_client.py` & `asposecellscloud-24.4/asposecellscloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
             self.default_headers[header_name] = header_value
         if host is None:
             self.host = Configuration().host
         else:
             self.host = host
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Aspose.Cells.Cloud/24.3/python'
+        self.user_agent = 'Aspose.Cells.Cloud/24.4/python'
 
     @property
     def user_agent(self):
         """
         Gets user agent.
         """
         return self.default_headers['User-Agent']
```

### Comparing `asposecellscloud-24.3/asposecellscloud/apis/cells_api.py` & `asposecellscloud-24.4/asposecellscloud/apis/cells_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -5982,14 +5982,62 @@
                                         _preload_content=params.get('_preload_content', True),
                                         _request_timeout=params.get('_request_timeout'),
                                         collection_formats=http_params['collection_formats'])
 
 
 
     # <summary>
+    # Transform spreadsheet data is mainly used to pivot columns, unpivot columns.
+    # </summary>
+    # <param name="request">Request. <see cref="PostDataTransformationRequest" /></param>
+    def post_data_transformation(self, request, **kwargs):
+
+        kwargs['_return_http_data_only'] = True
+        self.check_access_token()
+        if kwargs.get('callback'):
+            return self.post_data_transformation_with_http_info(request,**kwargs)
+        else:
+            (data) = self.post_data_transformation_with_http_info(request,**kwargs)
+            return data
+
+    def post_data_transformation_with_http_info(self, request, **kwargs):
+        all_params = []
+        all_params.append('callback')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+        params = locals()
+        for key, val in iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method post_data_transformation" % key
+                )
+            params[key] = val
+        del params['kwargs'] 
+
+        http_params = request.create_http_request(self.api_client)
+        return self.api_client.call_api(http_params['path'], http_params['method'],
+                                        None,
+                                        http_params['query_params'],
+                                        http_params['header_params'],
+                                        body=http_params['body'],
+                                        post_params=http_params['form_params'],
+                                        files=http_params['files'],
+                                        response_type=http_params['response_type'],
+                                        auth_settings=http_params['auth_settings'],
+                                        callback=params.get('callback'),
+                                        _return_http_data_only=params.get('_return_http_data_only'),
+                                        _preload_content=params.get('_preload_content', True),
+                                        _request_timeout=params.get('_request_timeout'),
+                                        collection_formats=http_params['collection_formats'])
+
+
+
+    # <summary>
     # Retrieve descriptions of hyperlinks in the worksheet.
     # </summary>
     # <param name="request">Request. <see cref="GetWorksheetHyperlinksRequest" /></param>
     def get_worksheet_hyperlinks(self, request, **kwargs):
 
         kwargs['_return_http_data_only'] = True
         self.check_access_token()
```

### Comparing `asposecellscloud-24.3/asposecellscloud/configuration.py` & `asposecellscloud-24.4/asposecellscloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,9 +255,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3.0\n"\
-               "SDK Package Version: 24.3".\
+               "SDK Package Version: 24.4".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/__init__.py` & `asposecellscloud-24.4/asposecellscloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,20 +67,23 @@
 from asposecellscloud.models.custom_filter import CustomFilter
 from asposecellscloud.models.data_bar import DataBar
 from asposecellscloud.models.data_bar_border import DataBarBorder
 from asposecellscloud.models.data_cleansing import DataCleansing
 from asposecellscloud.models.data_column_fill_value import DataColumnFillValue
 from asposecellscloud.models.data_fill import DataFill
 from asposecellscloud.models.data_fill_value import DataFillValue
+from asposecellscloud.models.data_item import DataItem
 from asposecellscloud.models.data_sorter import DataSorter
 from asposecellscloud.models.data_sorter_key import DataSorterKey
+from asposecellscloud.models.data_source import DataSource
 from asposecellscloud.models.date_time_group_item import DateTimeGroupItem
 from asposecellscloud.models.deduplication_region import DeduplicationRegion
 from asposecellscloud.models.dynamic_filter import DynamicFilter
 from asposecellscloud.models.file_info import FileInfo
+from asposecellscloud.models.file_source import FileSource
 from asposecellscloud.models.files_result import FilesResult
 from asposecellscloud.models.filter_column import FilterColumn
 from asposecellscloud.models.font import Font
 from asposecellscloud.models.font_setting import FontSetting
 from asposecellscloud.models.format_condition import FormatCondition
 from asposecellscloud.models.formula_format_condition import FormulaFormatCondition
 from asposecellscloud.models.formula_settings import FormulaSettings
@@ -103,15 +106,14 @@
 from asposecellscloud.models.negative_bar_format import NegativeBarFormat
 from asposecellscloud.models.page_section import PageSection
 from asposecellscloud.models.page_setup import PageSetup
 from asposecellscloud.models.paste_options import PasteOptions
 from asposecellscloud.models.pdf_security_options import PdfSecurityOptions
 from asposecellscloud.models.protection import Protection
 from asposecellscloud.models.protect_sheet_parameter import ProtectSheetParameter
-from asposecellscloud.models.query_table import QueryTable
 from asposecellscloud.models.range import Range
 from asposecellscloud.models.ranges import Ranges
 from asposecellscloud.models.row import Row
 from asposecellscloud.models.rows import Rows
 from asposecellscloud.models.save_result import SaveResult
 from asposecellscloud.models.paginated_save_options import PaginatedSaveOptions
 from asposecellscloud.models.single_value import SingleValue
@@ -139,15 +141,14 @@
 from asposecellscloud.models.worksheets import Worksheets
 from asposecellscloud.models.write_protection import WriteProtection
 from asposecellscloud.models.xml_data_binding import XmlDataBinding
 from asposecellscloud.models.xml_map import XmlMap
 from asposecellscloud.models.cells_object_operate_task_parameter import CellsObjectOperateTaskParameter
 from asposecellscloud.models.convert_task_parameter import ConvertTaskParameter
 from asposecellscloud.models.convert_worksheet_task_parameter import ConvertWorksheetTaskParameter
-from asposecellscloud.models.file_source import FileSource
 from asposecellscloud.models.import_data_task_parameter import ImportDataTaskParameter
 from asposecellscloud.models.result_destination import ResultDestination
 from asposecellscloud.models.save_files_to_cloud_result import SaveFilesToCloudResult
 from asposecellscloud.models.save_result_task_parameter import SaveResultTaskParameter
 from asposecellscloud.models.smart_marker_task_parameter import SmartMarkerTaskParameter
 from asposecellscloud.models.split_workbook_task_parameter import SplitWorkbookTaskParameter
 from asposecellscloud.models.task_data import TaskData
@@ -308,14 +309,15 @@
 from asposecellscloud.models.batch_split_request import BatchSplitRequest
 from asposecellscloud.models.color_filter_request import ColorFilterRequest
 from asposecellscloud.models.convert_parameter import ConvertParameter
 from asposecellscloud.models.create_pivot_table_request import CreatePivotTableRequest
 from asposecellscloud.models.data_cleansing_request import DataCleansingRequest
 from asposecellscloud.models.data_deduplication_request import DataDeduplicationRequest
 from asposecellscloud.models.data_fill_request import DataFillRequest
+from asposecellscloud.models.data_transformation_request import DataTransformationRequest
 from asposecellscloud.models.delete_incomplete_rows_request import DeleteIncompleteRowsRequest
 from asposecellscloud.models.import_json_request import ImportJsonRequest
 from asposecellscloud.models.import_xml_request import ImportXMLRequest
 from asposecellscloud.models.match_condition_request import MatchConditionRequest
 from asposecellscloud.models.password_request import PasswordRequest
 from asposecellscloud.models.pivot_table_field_request import PivotTableFieldRequest
 from asposecellscloud.models.protect_workbook_request import ProtectWorkbookRequest
@@ -327,14 +329,21 @@
 from asposecellscloud.models.text_water_marker_request import TextWaterMarkerRequest
 from asposecellscloud.models.workbook_encryption_request import WorkbookEncryptionRequest
 from asposecellscloud.models.workbook_protection_request import WorkbookProtectionRequest
 from asposecellscloud.models.worksheet_moving_request import WorksheetMovingRequest
 from asposecellscloud.models.image_or_print_options import ImageOrPrintOptions
 from asposecellscloud.models.rendering_font import RenderingFont
 from asposecellscloud.models.rendering_watermark import RenderingWatermark
+from asposecellscloud.models.load_data import LoadData
+from asposecellscloud.models.load_to import LoadTo
+from asposecellscloud.models.pivot_column import PivotColumn
+from asposecellscloud.models.query_data_source import QueryDataSource
+from asposecellscloud.models.query_table import QueryTable
+from asposecellscloud.models.transformation import Transformation
+from asposecellscloud.models.unpivot_column import UnpivotColumn
 from asposecellscloud.models.pivot_field import PivotField
 from asposecellscloud.models.pivot_filter import PivotFilter
 from asposecellscloud.models.pivot_item import PivotItem
 from asposecellscloud.models.pivot_table import PivotTable
 from asposecellscloud.models.pivot_tables import PivotTables
 from asposecellscloud.models.custom_parser_config import CustomParserConfig
 from asposecellscloud.models.import2_dimension_double_array_option import Import2DimensionDoubleArrayOption
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/above_average.py` & `asposecellscloud-24.4/asposecellscloud/models/above_average.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/abstract_calculation_engine.py` & `asposecellscloud-24.4/asposecellscloud/models/abstract_calculation_engine.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/abstract_calculation_monitor.py` & `asposecellscloud-24.4/asposecellscloud/models/abstract_calculation_monitor.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/access_token_response.py` & `asposecellscloud-24.4/asposecellscloud/models/access_token_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyze_excel_request.py` & `asposecellscloud-24.4/asposecellscloud/models/analyze_excel_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyze_excel_response.py` & `asposecellscloud-24.4/asposecellscloud/models/analyze_excel_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyze_suggestion.py` & `asposecellscloud-24.4/asposecellscloud/models/analyze_suggestion.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyzed_column_description.py` & `asposecellscloud-24.4/asposecellscloud/models/analyzed_column_description.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyzed_result.py` & `asposecellscloud-24.4/asposecellscloud/models/analyzed_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/analyzed_table_description.py` & `asposecellscloud-24.4/asposecellscloud/models/analyzed_table_description.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/arc_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/arc_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/arc_shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/arc_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/area.py` & `asposecellscloud-24.4/asposecellscloud/models/area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_filter_response.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_fitter_options.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_fitter_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_shapes.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/auto_shapes_response.py` & `asposecellscloud-24.4/asposecellscloud/models/auto_shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/axis.py` & `asposecellscloud-24.4/asposecellscloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/axis_response.py` & `asposecellscloud-24.4/asposecellscloud/models/axis_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/batch_convert_request.py` & `asposecellscloud-24.4/asposecellscloud/models/batch_convert_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/batch_lock_request.py` & `asposecellscloud-24.4/asposecellscloud/models/batch_lock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/batch_protect_request.py` & `asposecellscloud-24.4/asposecellscloud/models/batch_protect_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/batch_split_request.py` & `asposecellscloud-24.4/asposecellscloud/models/batch_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/border.py` & `asposecellscloud-24.4/asposecellscloud/models/border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/border_response.py` & `asposecellscloud-24.4/asposecellscloud/models/border_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/button.py` & `asposecellscloud-24.4/asposecellscloud/models/button.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/button_response.py` & `asposecellscloud-24.4/asposecellscloud/models/button_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/calculate_formula_response.py` & `asposecellscloud-24.4/asposecellscloud/models/calculate_formula_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/calculation_options.py` & `asposecellscloud-24.4/asposecellscloud/models/calculation_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cell.py` & `asposecellscloud-24.4/asposecellscloud/models/cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cell_area.py` & `asposecellscloud-24.4/asposecellscloud/models/cell_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cell_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cell_value.py` & `asposecellscloud-24.4/asposecellscloud/models/cell_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells.py` & `asposecellscloud-24.4/asposecellscloud/models/cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_cloud_file_info.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_cloud_file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_cloud_file_info_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_cloud_file_info_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_cloud_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_cloud_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_color.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_document_properties.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_document_properties.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_document_properties_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_document_properties_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_document_property.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_document_property.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_document_property_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_document_property_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_drawing.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_drawing.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_drawing_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_drawing_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_object_operate_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_object_operate_task_parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,20 +43,22 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'operate_object' : 'OperateObject',
         'operate_parameter' : 'OperateParameter',
+        'destinatio_data_source' : 'DataSource',
         'destination_workbook' : 'FileSource'
     }
 
     attribute_map = {
         'operate_object' : 'OperateObject' ,
         'operate_parameter' : 'OperateParameter' ,
+        'destinatio_data_source' : 'DestinatioDataSource' ,
         'destination_workbook' : 'DestinationWorkbook' 
     }
 
     @staticmethod
     def get_swagger_types():
         return CellsObjectOperateTaskParameter.swagger_types
 
@@ -65,39 +67,46 @@
         return CellsObjectOperateTaskParameter.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,operate_object=None ,operate_parameter=None ,destination_workbook=None   ,**kw):
+    def __init__(self,operate_object=None ,operate_parameter=None ,destinatio_data_source=None ,destination_workbook=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         CellsObjectOperateTaskParameter - a model defined in Swagger
         """
         self.container['operate_object'] = None 
         self.container['operate_parameter'] = None 
+        self.container['destinatio_data_source'] = None 
         self.container['destination_workbook'] = None 
         params = locals()
         self.operate_object = operate_object
         if 'operate_object' in params:
             self.operate_object = params["operate_object"]
 
 
              
         self.operate_parameter = operate_parameter
         if 'operate_parameter' in params:
             self.operate_parameter = params["operate_parameter"]
 
 
              
+        self.destinatio_data_source = destinatio_data_source
+        if 'destinatio_data_source' in params:
+            self.destinatio_data_source = params["destinatio_data_source"]
+
+
+             
         self.destination_workbook = destination_workbook
         if 'destination_workbook' in params:
             self.destination_workbook = params["destination_workbook"]
 
 
              
 
@@ -112,14 +121,21 @@
     def operate_parameter(self):
         return self.container['operate_parameter']
 
     @operate_parameter.setter
     def operate_parameter(self, operate_parameter):
         self.container['operate_parameter'] = operate_parameter 
     @property
+    def destinatio_data_source(self):
+        return self.container['destinatio_data_source']
+
+    @destinatio_data_source.setter
+    def destinatio_data_source(self, destinatio_data_source):
+        self.container['destinatio_data_source'] = destinatio_data_source 
+    @property
     def destination_workbook(self):
         return self.container['destination_workbook']
 
     @destination_workbook.setter
     def destination_workbook(self, destination_workbook):
         self.container['destination_workbook'] = destination_workbook
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/cells_response.py` & `asposecellscloud-24.4/asposecellscloud/models/cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart.py` & `asposecellscloud-24.4/asposecellscloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_area.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_area_response.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_area_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_data_table.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_data_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_data_table_response.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_data_table_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_frame.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_frame.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_globalization_settings.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_globalization_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_point.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_point.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_point_response.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_point_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_points.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_points.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_points_response.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_points_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_response.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/chart_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/chart_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/charts.py` & `asposecellscloud-24.4/asposecellscloud/models/charts.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/charts_response.py` & `asposecellscloud-24.4/asposecellscloud/models/charts_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/check_box.py` & `asposecellscloud-24.4/asposecellscloud/models/check_box.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/check_box_response.py` & `asposecellscloud-24.4/asposecellscloud/models/check_box_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/color.py` & `asposecellscloud-24.4/asposecellscloud/models/color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/color_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/color_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/color_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/models/color_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/color_scale.py` & `asposecellscloud-24.4/asposecellscloud/models/color_scale.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/column.py` & `asposecellscloud-24.4/asposecellscloud/models/column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/column_response.py` & `asposecellscloud-24.4/asposecellscloud/models/column_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/columns.py` & `asposecellscloud-24.4/asposecellscloud/models/columns.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/columns_response.py` & `asposecellscloud-24.4/asposecellscloud/models/columns_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/combo_box.py` & `asposecellscloud-24.4/asposecellscloud/models/combo_box.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/combo_box_response.py` & `asposecellscloud-24.4/asposecellscloud/models/combo_box_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comment.py` & `asposecellscloud-24.4/asposecellscloud/models/comment.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comment_response.py` & `asposecellscloud-24.4/asposecellscloud/models/comment_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comment_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/comment_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comment_shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/comment_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comments.py` & `asposecellscloud-24.4/asposecellscloud/models/comments.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/comments_response.py` & `asposecellscloud-24.4/asposecellscloud/models/comments_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formatting.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formatting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_icon.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_icon.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_response.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formatting_value.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formatting_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formattings.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formattings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/conditional_formattings_response.py` & `asposecellscloud-24.4/asposecellscloud/models/conditional_formattings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/convert_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/convert_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/convert_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/validations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="ConvertTaskParameterpy.cs">
+<copyright company="Aspose" file="Validationspy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class ConvertTaskParameter(object):
+class Validations(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,107 +41,91 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'workbook' : 'FileSource',
-        'destination_file' : 'str',
-        'region' : 'str',
-        'save_options' : 'SaveOptions'
+        'count' : 'int',
+        'validation_list' : 'list[LinkElement]',
+        'link' : 'Link'
     }
 
     attribute_map = {
-        'workbook' : 'Workbook' ,
-        'destination_file' : 'DestinationFile' ,
-        'region' : 'Region' ,
-        'save_options' : 'SaveOptions' 
+        'count' : 'Count' ,
+        'validation_list' : 'ValidationList' ,
+        'link' : 'link' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return ConvertTaskParameter.swagger_types
+        return Validations.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return ConvertTaskParameter.attribute_map
+        return Validations.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbook=None ,destination_file=None ,region=None ,save_options=None   ,**kw):
+    def __init__(self,count=None ,validation_list=None ,link=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        ConvertTaskParameter - a model defined in Swagger
+        Validations - a model defined in Swagger
         """
-        self.container['workbook'] = None 
-        self.container['destination_file'] = None 
-        self.container['region'] = None 
-        self.container['save_options'] = None 
+        self.container['count'] = None 
+        self.container['validation_list'] = None 
+        self.container['link'] = None 
         params = locals()
-        self.workbook = workbook
-        if 'workbook' in params:
-            self.workbook = params["workbook"]
+        self.count = count
+        if 'count' in params:
+            self.count = params["count"]
 
 
              
-        self.destination_file = destination_file
-        if 'destination_file' in params:
-            self.destination_file = params["destination_file"]
+        self.validation_list = validation_list
+        if 'validation_list' in params:
+            self.validation_list = params["validation_list"]
 
 
              
-        self.region = region
-        if 'region' in params:
-            self.region = params["region"]
+        self.link = link
+        if 'link' in params:
+            self.link = params["link"]
 
 
              
-        self.save_options = save_options
-        if 'save_options' in params:
-            self.save_options = params["save_options"]
 
-
-             
-
-    @property
-    def workbook(self):
-        return self.container['workbook']
-
-    @workbook.setter
-    def workbook(self, workbook):
-        self.container['workbook'] = workbook 
     @property
-    def destination_file(self):
-        return self.container['destination_file']
+    def count(self):
+        return self.container['count']
 
-    @destination_file.setter
-    def destination_file(self, destination_file):
-        self.container['destination_file'] = destination_file 
+    @count.setter
+    def count(self, count):
+        self.container['count'] = count 
     @property
-    def region(self):
-        return self.container['region']
+    def validation_list(self):
+        return self.container['validation_list']
 
-    @region.setter
-    def region(self, region):
-        self.container['region'] = region 
+    @validation_list.setter
+    def validation_list(self, validation_list):
+        self.container['validation_list'] = validation_list 
     @property
-    def save_options(self):
-        return self.container['save_options']
+    def link(self):
+        return self.container['link']
 
-    @save_options.setter
-    def save_options(self, save_options):
-        self.container['save_options'] = save_options 
+    @link.setter
+    def link(self, link):
+        self.container['link'] = link 
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -177,15 +161,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ConvertTaskParameter):
+        if not isinstance(other, Validations):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/convert_worksheet_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/convert_worksheet_task_parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,27 +41,31 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
+        'data_source' : 'DataSource',
         'workbook' : 'FileSource',
         'sheet' : 'str',
+        'target_data_source' : 'DataSource',
         'target' : 'FileSource',
         'format' : 'str',
         'area' : 'str',
         'page_index' : 'int',
         'vertical_resolution' : 'int',
         'horizontal_resolution' : 'int'
     }
 
     attribute_map = {
+        'data_source' : 'DataSource' ,
         'workbook' : 'Workbook' ,
         'sheet' : 'Sheet' ,
+        'target_data_source' : 'TargetDataSource' ,
         'target' : 'Target' ,
         'format' : 'Format' ,
         'area' : 'Area' ,
         'page_index' : 'PageIndex' ,
         'vertical_resolution' : 'VerticalResolution' ,
         'horizontal_resolution' : 'HorizontalResolution' 
     }
@@ -75,44 +79,58 @@
         return ConvertWorksheetTaskParameter.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbook=None ,sheet=None ,target=None ,format=None ,area=None ,page_index=None ,vertical_resolution=None ,horizontal_resolution=None   ,**kw):
+    def __init__(self,data_source=None ,workbook=None ,sheet=None ,target_data_source=None ,target=None ,format=None ,area=None ,page_index=None ,vertical_resolution=None ,horizontal_resolution=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ConvertWorksheetTaskParameter - a model defined in Swagger
         """
+        self.container['data_source'] = None 
         self.container['workbook'] = None 
         self.container['sheet'] = None 
+        self.container['target_data_source'] = None 
         self.container['target'] = None 
         self.container['format'] = None 
         self.container['area'] = None 
         self.container['page_index'] = None 
         self.container['vertical_resolution'] = None 
         self.container['horizontal_resolution'] = None 
         params = locals()
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.workbook = workbook
         if 'workbook' in params:
             self.workbook = params["workbook"]
 
 
              
         self.sheet = sheet
         if 'sheet' in params:
             self.sheet = params["sheet"]
 
 
              
+        self.target_data_source = target_data_source
+        if 'target_data_source' in params:
+            self.target_data_source = params["target_data_source"]
+
+
+             
         self.target = target
         if 'target' in params:
             self.target = params["target"]
 
 
              
         self.format = format
@@ -143,28 +161,42 @@
         if 'horizontal_resolution' in params:
             self.horizontal_resolution = params["horizontal_resolution"]
 
 
              
 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def workbook(self):
         return self.container['workbook']
 
     @workbook.setter
     def workbook(self, workbook):
         self.container['workbook'] = workbook 
     @property
     def sheet(self):
         return self.container['sheet']
 
     @sheet.setter
     def sheet(self, sheet):
         self.container['sheet'] = sheet 
     @property
+    def target_data_source(self):
+        return self.container['target_data_source']
+
+    @target_data_source.setter
+    def target_data_source(self, target_data_source):
+        self.container['target_data_source'] = target_data_source 
+    @property
     def target(self):
         return self.container['target']
 
     @target.setter
     def target(self, target):
         self.container['target'] = target 
     @property
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/copy_options.py` & `asposecellscloud-24.4/asposecellscloud/models/copy_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/create_pivot_table_request.py` & `asposecellscloud-24.4/asposecellscloud/models/create_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/criteria_multiple_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/criteria_multiple_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/custom_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/custom_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/custom_parser_config.py` & `asposecellscloud-24.4/asposecellscloud/models/custom_parser_config.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_bar.py` & `asposecellscloud-24.4/asposecellscloud/models/data_bar.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_bar_border.py` & `asposecellscloud-24.4/asposecellscloud/models/data_bar_border.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_cleansing.py` & `asposecellscloud-24.4/asposecellscloud/models/data_cleansing.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_cleansing_request.py` & `asposecellscloud-24.4/asposecellscloud/models/data_cleansing_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_column_fill_value.py` & `asposecellscloud-24.4/asposecellscloud/models/data_column_fill_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_deduplication_request.py` & `asposecellscloud-24.4/asposecellscloud/models/data_deduplication_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_fill.py` & `asposecellscloud-24.4/asposecellscloud/models/data_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_fill_request.py` & `asposecellscloud-24.4/asposecellscloud/models/data_fill_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_fill_value.py` & `asposecellscloud-24.4/asposecellscloud/models/data_fill_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_labels.py` & `asposecellscloud-24.4/asposecellscloud/models/data_labels.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_labels_response.py` & `asposecellscloud-24.4/asposecellscloud/models/data_labels_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_sorter.py` & `asposecellscloud-24.4/asposecellscloud/models/data_sorter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/data_sorter_key.py` & `asposecellscloud-24.4/asposecellscloud/models/data_sorter_key.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/date_time_group_item.py` & `asposecellscloud-24.4/asposecellscloud/models/date_time_group_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/deduplication_region.py` & `asposecellscloud-24.4/asposecellscloud/models/deduplication_region.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/delete_incomplete_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/models/delete_incomplete_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/dif_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/dif_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/digital_signature.py` & `asposecellscloud-24.4/asposecellscloud/models/digital_signature.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/disc_usage.py` & `asposecellscloud-24.4/asposecellscloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/discover_chart.py` & `asposecellscloud-24.4/asposecellscloud/models/discover_chart.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/discover_pivot_table.py` & `asposecellscloud-24.4/asposecellscloud/models/discover_pivot_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/display_unit_label.py` & `asposecellscloud-24.4/asposecellscloud/models/display_unit_label.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/display_unit_label_response.py` & `asposecellscloud-24.4/asposecellscloud/models/display_unit_label_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/docx_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/docx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/drop_bars.py` & `asposecellscloud-24.4/asposecellscloud/models/drop_bars.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/drop_bars_response.py` & `asposecellscloud-24.4/asposecellscloud/models/drop_bars_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/dynamic_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/dynamic_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/error.py` & `asposecellscloud-24.4/asposecellscloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/error_bar.py` & `asposecellscloud-24.4/asposecellscloud/models/error_bar.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/error_bar_response.py` & `asposecellscloud-24.4/asposecellscloud/models/error_bar_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/error_details.py` & `asposecellscloud-24.4/asposecellscloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/excel_data_statistics.py` & `asposecellscloud-24.4/asposecellscloud/models/excel_data_statistics.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/file_info.py` & `asposecellscloud-24.4/asposecellscloud/models/file_info.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/file_source.py` & `asposecellscloud-24.4/asposecellscloud/models/file_source.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/file_version.py` & `asposecellscloud-24.4/asposecellscloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/file_versions.py` & `asposecellscloud-24.4/asposecellscloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/files_list.py` & `asposecellscloud-24.4/asposecellscloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/files_result.py` & `asposecellscloud-24.4/asposecellscloud/models/files_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/files_upload_result.py` & `asposecellscloud-24.4/asposecellscloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/fill_format.py` & `asposecellscloud-24.4/asposecellscloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/fill_format_response.py` & `asposecellscloud-24.4/asposecellscloud/models/fill_format_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/filter_column.py` & `asposecellscloud-24.4/asposecellscloud/models/filter_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/find_response.py` & `asposecellscloud-24.4/asposecellscloud/models/find_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/floor.py` & `asposecellscloud-24.4/asposecellscloud/models/floor.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/floor_response.py` & `asposecellscloud-24.4/asposecellscloud/models/floor_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/font.py` & `asposecellscloud-24.4/asposecellscloud/models/font.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/font_setting.py` & `asposecellscloud-24.4/asposecellscloud/models/font_setting.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/form.py` & `asposecellscloud-24.4/asposecellscloud/models/form.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/form_response.py` & `asposecellscloud-24.4/asposecellscloud/models/form_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/format_condition.py` & `asposecellscloud-24.4/asposecellscloud/models/format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/forms.py` & `asposecellscloud-24.4/asposecellscloud/models/forms.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/forms_response.py` & `asposecellscloud-24.4/asposecellscloud/models/forms_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/formula_format_condition.py` & `asposecellscloud-24.4/asposecellscloud/models/formula_format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/formula_settings.py` & `asposecellscloud-24.4/asposecellscloud/models/formula_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/globalization_settings.py` & `asposecellscloud-24.4/asposecellscloud/models/globalization_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/google_drive_storage_file.py` & `asposecellscloud-24.4/asposecellscloud/models/google_drive_storage_file.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/gradient_fill.py` & `asposecellscloud-24.4/asposecellscloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/gradient_fill_stop.py` & `asposecellscloud-24.4/asposecellscloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/group_box.py` & `asposecellscloud-24.4/asposecellscloud/models/group_box.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/group_box_response.py` & `asposecellscloud-24.4/asposecellscloud/models/group_box_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/group_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/horizontal_page_break.py` & `asposecellscloud-24.4/asposecellscloud/models/horizontal_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/horizontal_page_break_response.py` & `asposecellscloud-24.4/asposecellscloud/models/horizontal_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/horizontal_page_breaks.py` & `asposecellscloud-24.4/asposecellscloud/models/horizontal_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/horizontal_page_breaks_response.py` & `asposecellscloud-24.4/asposecellscloud/models/horizontal_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/html_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/hyperlink.py` & `asposecellscloud-24.4/asposecellscloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/hyperlink_response.py` & `asposecellscloud-24.4/asposecellscloud/models/hyperlink_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/hyperlinks.py` & `asposecellscloud-24.4/asposecellscloud/models/hyperlinks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/hyperlinks_response.py` & `asposecellscloud-24.4/asposecellscloud/models/hyperlinks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/icon_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/icon_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/icon_set.py` & `asposecellscloud-24.4/asposecellscloud/models/icon_set.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/image_or_print_options.py` & `asposecellscloud-24.4/asposecellscloud/models/image_or_print_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/image_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/image_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import2_dimension_double_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import2_dimension_double_array_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,24 +47,26 @@
     swagger_types = {
         'first_row' : 'int',
         'first_column' : 'int',
         'data' : 'list[float]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return Import2DimensionDoubleArrayOption.swagger_types
 
@@ -73,29 +75,30 @@
         return Import2DimensionDoubleArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         Import2DimensionDoubleArrayOption - a model defined in Swagger
         """
         self.container['first_row'] = None 
         self.container['first_column'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
@@ -126,14 +129,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -176,14 +185,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import2_dimension_int_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import2_dimension_int_array_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,24 +47,26 @@
     swagger_types = {
         'first_row' : 'int',
         'first_column' : 'int',
         'data' : 'list[int]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return Import2DimensionIntArrayOption.swagger_types
 
@@ -73,29 +75,30 @@
         return Import2DimensionIntArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         Import2DimensionIntArrayOption - a model defined in Swagger
         """
         self.container['first_row'] = None 
         self.container['first_column'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
@@ -126,14 +129,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -176,14 +185,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import2_dimension_string_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_double_array_option.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="Import2DimensionStringArrayOptionpy.cs">
+<copyright company="Aspose" file="ImportDoubleArrayOptionpy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class Import2DimensionStringArrayOption(object):
+class ImportDoubleArrayOption(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -43,73 +43,85 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'first_row' : 'int',
         'first_column' : 'int',
-        'data' : 'list[str]',
+        'is_vertical' : 'bool',
+        'data' : 'list[float]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
+        'is_vertical' : 'IsVertical' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return Import2DimensionStringArrayOption.swagger_types
+        return ImportDoubleArrayOption.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return Import2DimensionStringArrayOption.attribute_map
+        return ImportDoubleArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        Import2DimensionStringArrayOption - a model defined in Swagger
+        ImportDoubleArrayOption - a model defined in Swagger
         """
         self.container['first_row'] = None 
         self.container['first_column'] = None 
+        self.container['is_vertical'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
              
         self.first_column = first_column
         if 'first_column' in params:
             self.first_column = params["first_column"]
 
 
              
+        self.is_vertical = is_vertical
+        if 'is_vertical' in params:
+            self.is_vertical = params["is_vertical"]
+
+
+             
         self.data = data
         if 'data' in params:
             self.data = params["data"]
 
 
              
         self.destination_worksheet = destination_worksheet
@@ -126,14 +138,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -148,14 +166,21 @@
     def first_column(self):
         return self.container['first_column']
 
     @first_column.setter
     def first_column(self, first_column):
         self.container['first_column'] = first_column 
     @property
+    def is_vertical(self):
+        return self.container['is_vertical']
+
+    @is_vertical.setter
+    def is_vertical(self, is_vertical):
+        self.container['is_vertical'] = is_vertical 
+    @property
     def data(self):
         return self.container['data']
 
     @data.setter
     def data(self, data):
         self.container['data'] = data 
     @property
@@ -176,14 +201,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source 
 
@@ -225,15 +257,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, Import2DimensionStringArrayOption):
+        if not isinstance(other, ImportDoubleArrayOption):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_batch_data_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_batch_data_option.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,22 +45,24 @@
     """
 
     swagger_types = {
         'batch_data' : 'list[CellValue]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'batch_data' : 'BatchData' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportBatchDataOption.swagger_types
 
@@ -69,27 +71,28 @@
         return ImportBatchDataOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,batch_data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,batch_data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportBatchDataOption - a model defined in Swagger
         """
         self.container['batch_data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.batch_data = batch_data
         if 'batch_data' in params:
             self.batch_data = params["batch_data"]
 
 
@@ -108,14 +111,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -144,14 +153,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_csv_data_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_csv_data_option.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,27 +50,29 @@
         'first_row' : 'int',
         'first_column' : 'int',
         'source_file' : 'str',
         'custom_parsers' : 'list[CustomParserConfig]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'separator_string' : 'SeparatorString' ,
         'convert_numeric_data' : 'ConvertNumericData' ,
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
         'source_file' : 'SourceFile' ,
         'custom_parsers' : 'CustomParsers' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportCSVDataOption.swagger_types
 
@@ -79,15 +81,15 @@
         return ImportCSVDataOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,separator_string=None ,convert_numeric_data=None ,first_row=None ,first_column=None ,source_file=None ,custom_parsers=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,separator_string=None ,convert_numeric_data=None ,first_row=None ,first_column=None ,source_file=None ,custom_parsers=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportCSVDataOption - a model defined in Swagger
@@ -97,14 +99,15 @@
         self.container['first_row'] = None 
         self.container['first_column'] = None 
         self.container['source_file'] = None 
         self.container['custom_parsers'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.separator_string = separator_string
         if 'separator_string' in params:
             self.separator_string = params["separator_string"]
 
 
@@ -153,14 +156,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -224,14 +233,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_data_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/import_data_task_parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,22 +41,26 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
+        'data_source' : 'DataSource',
         'workbook' : 'FileSource',
         'import_option' : 'ImportOption',
+        'target_data_source' : 'DataSource',
         'destination_workbook' : 'FileSource'
     }
 
     attribute_map = {
+        'data_source' : 'DataSource' ,
         'workbook' : 'Workbook' ,
         'import_option' : 'ImportOption' ,
+        'target_data_source' : 'TargetDataSource' ,
         'destination_workbook' : 'DestinationWorkbook' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportDataTaskParameter.swagger_types
 
@@ -65,61 +69,89 @@
         return ImportDataTaskParameter.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbook=None ,import_option=None ,destination_workbook=None   ,**kw):
+    def __init__(self,data_source=None ,workbook=None ,import_option=None ,target_data_source=None ,destination_workbook=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportDataTaskParameter - a model defined in Swagger
         """
+        self.container['data_source'] = None 
         self.container['workbook'] = None 
         self.container['import_option'] = None 
+        self.container['target_data_source'] = None 
         self.container['destination_workbook'] = None 
         params = locals()
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.workbook = workbook
         if 'workbook' in params:
             self.workbook = params["workbook"]
 
 
              
         self.import_option = import_option
         if 'import_option' in params:
             self.import_option = params["import_option"]
 
 
              
+        self.target_data_source = target_data_source
+        if 'target_data_source' in params:
+            self.target_data_source = params["target_data_source"]
+
+
+             
         self.destination_workbook = destination_workbook
         if 'destination_workbook' in params:
             self.destination_workbook = params["destination_workbook"]
 
 
              
 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def workbook(self):
         return self.container['workbook']
 
     @workbook.setter
     def workbook(self, workbook):
         self.container['workbook'] = workbook 
     @property
     def import_option(self):
         return self.container['import_option']
 
     @import_option.setter
     def import_option(self, import_option):
         self.container['import_option'] = import_option 
     @property
+    def target_data_source(self):
+        return self.container['target_data_source']
+
+    @target_data_source.setter
+    def target_data_source(self, target_data_source):
+        self.container['target_data_source'] = target_data_source 
+    @property
     def destination_workbook(self):
         return self.container['destination_workbook']
 
     @destination_workbook.setter
     def destination_workbook(self, destination_workbook):
         self.container['destination_workbook'] = destination_workbook
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_double_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_string_array_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="ImportDoubleArrayOptionpy.cs">
+<copyright company="Aspose" file="ImportStringArrayOptionpy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class ImportDoubleArrayOption(object):
+class ImportStringArrayOption(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -44,61 +44,64 @@
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'first_row' : 'int',
         'first_column' : 'int',
         'is_vertical' : 'bool',
-        'data' : 'list[float]',
+        'data' : 'list[str]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
         'is_vertical' : 'IsVertical' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return ImportDoubleArrayOption.swagger_types
+        return ImportStringArrayOption.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return ImportDoubleArrayOption.attribute_map
+        return ImportStringArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        ImportDoubleArrayOption - a model defined in Swagger
+        ImportStringArrayOption - a model defined in Swagger
         """
         self.container['first_row'] = None 
         self.container['first_column'] = None 
         self.container['is_vertical'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
@@ -135,14 +138,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -192,14 +201,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source 
 
@@ -241,15 +257,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ImportDoubleArrayOption):
+        if not isinstance(other, ImportStringArrayOption):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_int_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_int_array_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,25 +48,27 @@
         'first_row' : 'int',
         'first_column' : 'int',
         'is_vertical' : 'bool',
         'data' : 'list[int]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
         'is_vertical' : 'IsVertical' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportIntArrayOption.swagger_types
 
@@ -75,15 +77,15 @@
         return ImportIntArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportIntArrayOption - a model defined in Swagger
@@ -91,14 +93,15 @@
         self.container['first_row'] = None 
         self.container['first_column'] = None 
         self.container['is_vertical'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
@@ -135,14 +138,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -192,14 +201,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_json_request.py` & `asposecellscloud-24.4/asposecellscloud/models/import_json_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'json_file_source' : 'FileSource',
+        'json_file_source' : 'DataSource',
         'import_position' : 'ImportPosition',
         'json_content' : 'str'
     }
 
     attribute_map = {
         'json_file_source' : 'JsonFileSource' ,
         'import_position' : 'ImportPosition' ,
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_option.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,21 +44,23 @@
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportOption.swagger_types
 
@@ -67,26 +69,27 @@
         return ImportOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportOption - a model defined in Swagger
         """
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.destination_worksheet = destination_worksheet
         if 'destination_worksheet' in params:
             self.destination_worksheet = params["destination_worksheet"]
 
 
@@ -99,14 +102,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -128,14 +137,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_picture_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import_picture_option.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,27 +50,29 @@
         'lower_right_row' : 'int',
         'lower_right_column' : 'int',
         'filename' : 'str',
         'data' : 'str',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'upper_left_row' : 'UpperLeftRow' ,
         'upper_left_column' : 'UpperLeftColumn' ,
         'lower_right_row' : 'LowerRightRow' ,
         'lower_right_column' : 'LowerRightColumn' ,
         'filename' : 'Filename' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
         return ImportPictureOption.swagger_types
 
@@ -79,15 +81,15 @@
         return ImportPictureOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,upper_left_row=None ,upper_left_column=None ,lower_right_row=None ,lower_right_column=None ,filename=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,upper_left_row=None ,upper_left_column=None ,lower_right_row=None ,lower_right_column=None ,filename=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         ImportPictureOption - a model defined in Swagger
@@ -97,14 +99,15 @@
         self.container['lower_right_row'] = None 
         self.container['lower_right_column'] = None 
         self.container['filename'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.upper_left_row = upper_left_row
         if 'upper_left_row' in params:
             self.upper_left_row = params["upper_left_row"]
 
 
@@ -153,14 +156,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -224,14 +233,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_position.py` & `asposecellscloud-24.4/asposecellscloud/models/import_position.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_string_array_option.py` & `asposecellscloud-24.4/asposecellscloud/models/import2_dimension_string_array_option.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="ImportStringArrayOptionpy.cs">
+<copyright company="Aspose" file="Import2DimensionStringArrayOptionpy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class ImportStringArrayOption(object):
+class Import2DimensionStringArrayOption(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -43,82 +43,76 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'first_row' : 'int',
         'first_column' : 'int',
-        'is_vertical' : 'bool',
         'data' : 'list[str]',
         'destination_worksheet' : 'str',
         'is_insert' : 'bool',
         'import_data_type' : 'str',
+        'data_source' : 'DataSource',
         'source' : 'FileSource'
     }
 
     attribute_map = {
         'first_row' : 'FirstRow' ,
         'first_column' : 'FirstColumn' ,
-        'is_vertical' : 'IsVertical' ,
         'data' : 'Data' ,
         'destination_worksheet' : 'DestinationWorksheet' ,
         'is_insert' : 'IsInsert' ,
         'import_data_type' : 'ImportDataType' ,
+        'data_source' : 'DataSource' ,
         'source' : 'Source' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return ImportStringArrayOption.swagger_types
+        return Import2DimensionStringArrayOption.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return ImportStringArrayOption.attribute_map
+        return Import2DimensionStringArrayOption.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,first_row=None ,first_column=None ,is_vertical=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,source=None   ,**kw):
+    def __init__(self,first_row=None ,first_column=None ,data=None ,destination_worksheet=None ,is_insert=None ,import_data_type=None ,data_source=None ,source=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        ImportStringArrayOption - a model defined in Swagger
+        Import2DimensionStringArrayOption - a model defined in Swagger
         """
         self.container['first_row'] = None 
         self.container['first_column'] = None 
-        self.container['is_vertical'] = None 
         self.container['data'] = None 
         self.container['destination_worksheet'] = None 
         self.container['is_insert'] = None 
         self.container['import_data_type'] = None 
+        self.container['data_source'] = None 
         self.container['source'] = None 
         params = locals()
         self.first_row = first_row
         if 'first_row' in params:
             self.first_row = params["first_row"]
 
 
              
         self.first_column = first_column
         if 'first_column' in params:
             self.first_column = params["first_column"]
 
 
              
-        self.is_vertical = is_vertical
-        if 'is_vertical' in params:
-            self.is_vertical = params["is_vertical"]
-
-
-             
         self.data = data
         if 'data' in params:
             self.data = params["data"]
 
 
              
         self.destination_worksheet = destination_worksheet
@@ -135,14 +129,20 @@
              
         self.import_data_type = import_data_type
         if 'import_data_type' in params:
             self.import_data_type = params["import_data_type"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.source = source
         if 'source' in params:
             self.source = params["source"]
 
 
              
 
@@ -157,21 +157,14 @@
     def first_column(self):
         return self.container['first_column']
 
     @first_column.setter
     def first_column(self, first_column):
         self.container['first_column'] = first_column 
     @property
-    def is_vertical(self):
-        return self.container['is_vertical']
-
-    @is_vertical.setter
-    def is_vertical(self, is_vertical):
-        self.container['is_vertical'] = is_vertical 
-    @property
     def data(self):
         return self.container['data']
 
     @data.setter
     def data(self, data):
         self.container['data'] = data 
     @property
@@ -192,14 +185,21 @@
     def import_data_type(self):
         return self.container['import_data_type']
 
     @import_data_type.setter
     def import_data_type(self, import_data_type):
         self.container['import_data_type'] = import_data_type 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def source(self):
         return self.container['source']
 
     @source.setter
     def source(self, source):
         self.container['source'] = source 
 
@@ -241,15 +241,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ImportStringArrayOption):
+        if not isinstance(other, Import2DimensionStringArrayOption):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/import_xml_request.py` & `asposecellscloud-24.4/asposecellscloud/models/import_xml_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'xml_file_source' : 'FileSource',
+        'xml_file_source' : 'DataSource',
         'import_position' : 'ImportPosition',
         'xml_content' : 'str'
     }
 
     attribute_map = {
         'xml_file_source' : 'XMLFileSource' ,
         'import_position' : 'ImportPosition' ,
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/json_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/json_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/label.py` & `asposecellscloud-24.4/asposecellscloud/models/label.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/label_response.py` & `asposecellscloud-24.4/asposecellscloud/models/label_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend.py` & `asposecellscloud-24.4/asposecellscloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend_entries.py` & `asposecellscloud-24.4/asposecellscloud/models/legend_entries.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend_entries_response.py` & `asposecellscloud-24.4/asposecellscloud/models/legend_entries_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend_entry.py` & `asposecellscloud-24.4/asposecellscloud/models/legend_entry.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend_entry_response.py` & `asposecellscloud-24.4/asposecellscloud/models/legend_entry_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/legend_response.py` & `asposecellscloud-24.4/asposecellscloud/models/legend_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/line.py` & `asposecellscloud-24.4/asposecellscloud/models/line.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/line_format.py` & `asposecellscloud-24.4/asposecellscloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/line_response.py` & `asposecellscloud-24.4/asposecellscloud/models/line_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/line_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/line_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/line_shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/line_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/link.py` & `asposecellscloud-24.4/asposecellscloud/models/link.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/link_element.py` & `asposecellscloud-24.4/asposecellscloud/models/link_element.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_box.py` & `asposecellscloud-24.4/asposecellscloud/models/list_box.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_box_response.py` & `asposecellscloud-24.4/asposecellscloud/models/list_box_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_column.py` & `asposecellscloud-24.4/asposecellscloud/models/list_column.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_object.py` & `asposecellscloud-24.4/asposecellscloud/models/list_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_object_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/list_object_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_object_response.py` & `asposecellscloud-24.4/asposecellscloud/models/list_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_objects.py` & `asposecellscloud-24.4/asposecellscloud/models/list_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/list_objects_response.py` & `asposecellscloud-24.4/asposecellscloud/models/list_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/load_options.py` & `asposecellscloud-24.4/asposecellscloud/models/load_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/m_html_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/m_html_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/markdown_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/markdown_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/marker.py` & `asposecellscloud-24.4/asposecellscloud/models/marker.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/match_condition_request.py` & `asposecellscloud-24.4/asposecellscloud/models/match_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/merged_cell.py` & `asposecellscloud-24.4/asposecellscloud/models/merged_cell.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/merged_cell_response.py` & `asposecellscloud-24.4/asposecellscloud/models/merged_cell_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/merged_cells.py` & `asposecellscloud-24.4/asposecellscloud/models/merged_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/merged_cells_response.py` & `asposecellscloud-24.4/asposecellscloud/models/merged_cells_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/multiple_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/multiple_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/multiple_filters.py` & `asposecellscloud-24.4/asposecellscloud/models/multiple_filters.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/name.py` & `asposecellscloud-24.4/asposecellscloud/models/name.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/name_response.py` & `asposecellscloud-24.4/asposecellscloud/models/name_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/names.py` & `asposecellscloud-24.4/asposecellscloud/models/names.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/names_response.py` & `asposecellscloud-24.4/asposecellscloud/models/names_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/negative_bar_format.py` & `asposecellscloud-24.4/asposecellscloud/models/negative_bar_format.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/object_exist.py` & `asposecellscloud-24.4/asposecellscloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/object_exists_extensions.py` & `asposecellscloud-24.4/asposecellscloud/models/object_exists_extensions.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ods_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/ods_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ole_object.py` & `asposecellscloud-24.4/asposecellscloud/models/ole_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ole_object_response.py` & `asposecellscloud-24.4/asposecellscloud/models/ole_object_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ole_objects.py` & `asposecellscloud-24.4/asposecellscloud/models/ole_objects.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ole_objects_response.py` & `asposecellscloud-24.4/asposecellscloud/models/ole_objects_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ooxml_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/ooxml_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/operate_object.py` & `asposecellscloud-24.4/asposecellscloud/models/operate_object.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/operate_object_position.py` & `asposecellscloud-24.4/asposecellscloud/models/operate_object_position.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,23 +41,25 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
+        'data_source' : 'DataSource',
         'workbook' : 'FileSource',
         'sheet_name' : 'str',
         'chart_index' : 'int',
         'shape_index' : 'int',
         'cell_name' : 'str',
         'list_object_index' : 'int'
     }
 
     attribute_map = {
+        'data_source' : 'DataSource' ,
         'workbook' : 'Workbook' ,
         'sheet_name' : 'SheetName' ,
         'chart_index' : 'ChartIndex' ,
         'shape_index' : 'ShapeIndex' ,
         'cell_name' : 'CellName' ,
         'list_object_index' : 'ListObjectIndex' 
     }
@@ -71,30 +73,37 @@
         return OperateObjectPosition.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbook=None ,sheet_name=None ,chart_index=None ,shape_index=None ,cell_name=None ,list_object_index=None   ,**kw):
+    def __init__(self,data_source=None ,workbook=None ,sheet_name=None ,chart_index=None ,shape_index=None ,cell_name=None ,list_object_index=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         OperateObjectPosition - a model defined in Swagger
         """
+        self.container['data_source'] = None 
         self.container['workbook'] = None 
         self.container['sheet_name'] = None 
         self.container['chart_index'] = None 
         self.container['shape_index'] = None 
         self.container['cell_name'] = None 
         self.container['list_object_index'] = None 
         params = locals()
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
         self.workbook = workbook
         if 'workbook' in params:
             self.workbook = params["workbook"]
 
 
              
         self.sheet_name = sheet_name
@@ -125,14 +134,21 @@
         if 'list_object_index' in params:
             self.list_object_index = params["list_object_index"]
 
 
              
 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
     def workbook(self):
         return self.container['workbook']
 
     @workbook.setter
     def workbook(self, workbook):
         self.container['workbook'] = workbook 
     @property
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/oval.py` & `asposecellscloud-24.4/asposecellscloud/models/oval.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/oval_response.py` & `asposecellscloud-24.4/asposecellscloud/models/oval_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_break_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/page_break_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_section.py` & `asposecellscloud-24.4/asposecellscloud/models/page_section.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_sections_response.py` & `asposecellscloud-24.4/asposecellscloud/models/page_sections_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_setup.py` & `asposecellscloud-24.4/asposecellscloud/models/page_setup.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_setup_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/page_setup_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/page_setup_response.py` & `asposecellscloud-24.4/asposecellscloud/models/page_setup_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/paginated_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/paginated_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/password_request.py` & `asposecellscloud-24.4/asposecellscloud/models/password_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/paste_options.py` & `asposecellscloud-24.4/asposecellscloud/models/paste_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pattern_fill.py` & `asposecellscloud-24.4/asposecellscloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pdf_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/pdf_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pdf_security_options.py` & `asposecellscloud-24.4/asposecellscloud/models/pdf_security_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pic_format_option.py` & `asposecellscloud-24.4/asposecellscloud/models/pic_format_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/picture.py` & `asposecellscloud-24.4/asposecellscloud/models/picture.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/picture_response.py` & `asposecellscloud-24.4/asposecellscloud/models/picture_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pictures.py` & `asposecellscloud-24.4/asposecellscloud/models/pictures.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pictures_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pictures_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_field.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_field.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_field_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_field_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_filter_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_filter_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_filters_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_filters_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_globalization_settings.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_globalization_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_item.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_table.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_table_field_request.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_table_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_table_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_table_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_table_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_tables.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_tables.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pivot_tables_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_tables_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/plot_area.py` & `asposecellscloud-24.4/asposecellscloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/plot_area_response.py` & `asposecellscloud-24.4/asposecellscloud/models/plot_area_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/pptx_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/pptx_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/protect_sheet_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/protect_sheet_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/protect_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/models/protect_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/protection.py` & `asposecellscloud-24.4/asposecellscloud/models/protection.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/query_table.py` & `asposecellscloud-24.4/asposecellscloud/models/query_table.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/radio_button.py` & `asposecellscloud-24.4/asposecellscloud/models/radio_button.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/radio_button_response.py` & `asposecellscloud-24.4/asposecellscloud/models/radio_button_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range.py` & `asposecellscloud-24.4/asposecellscloud/models/range.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_copy_request.py` & `asposecellscloud-24.4/asposecellscloud/models/range_copy_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_response.py` & `asposecellscloud-24.4/asposecellscloud/models/range_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_set_outline_border_request.py` & `asposecellscloud-24.4/asposecellscloud/models/range_set_outline_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_set_style_request.py` & `asposecellscloud-24.4/asposecellscloud/models/range_set_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_sort_request.py` & `asposecellscloud-24.4/asposecellscloud/models/range_sort_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/range_value_response.py` & `asposecellscloud-24.4/asposecellscloud/models/range_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ranges.py` & `asposecellscloud-24.4/asposecellscloud/models/ranges.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/ranges_response.py` & `asposecellscloud-24.4/asposecellscloud/models/ranges_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rectangle_shape.py` & `asposecellscloud-24.4/asposecellscloud/models/rectangle_shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rectangle_shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/rectangle_shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rendering_font.py` & `asposecellscloud-24.4/asposecellscloud/models/rendering_font.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rendering_watermark.py` & `asposecellscloud-24.4/asposecellscloud/models/rendering_watermark.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/result_destination.py` & `asposecellscloud-24.4/asposecellscloud/models/result_destination.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/row.py` & `asposecellscloud-24.4/asposecellscloud/models/row.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/row_response.py` & `asposecellscloud-24.4/asposecellscloud/models/row_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rows.py` & `asposecellscloud-24.4/asposecellscloud/models/rows.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/rows_response.py` & `asposecellscloud-24.4/asposecellscloud/models/rows_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_files_to_cloud_result.py` & `asposecellscloud-24.4/asposecellscloud/models/save_files_to_cloud_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'saved_files' : 'list[Link]',
         'description' : 'str',
-        'out_file_list' : 'list[FileSource]'
+        'out_file_list' : 'list[DataSource]'
     }
 
     attribute_map = {
         'saved_files' : 'SavedFiles' ,
         'description' : 'Description' ,
         'out_file_list' : 'OutFileList' 
     }
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_files_to_cloud_result_response.py` & `asposecellscloud-24.4/asposecellscloud/models/save_files_to_cloud_result_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_response.py` & `asposecellscloud-24.4/asposecellscloud/models/save_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_result.py` & `asposecellscloud-24.4/asposecellscloud/models/save_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/save_result_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/save_result_task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/scroll_bar.py` & `asposecellscloud-24.4/asposecellscloud/models/scroll_bar.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/scroll_bar_response.py` & `asposecellscloud-24.4/asposecellscloud/models/scroll_bar_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/series.py` & `asposecellscloud-24.4/asposecellscloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/series_items.py` & `asposecellscloud-24.4/asposecellscloud/models/series_items.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/series_response.py` & `asposecellscloud-24.4/asposecellscloud/models/series_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/serieses_response.py` & `asposecellscloud-24.4/asposecellscloud/models/serieses_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shadow_effect.py` & `asposecellscloud-24.4/asposecellscloud/models/shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shape.py` & `asposecellscloud-24.4/asposecellscloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shape_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/shape_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shape_response.py` & `asposecellscloud-24.4/asposecellscloud/models/shape_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shapes.py` & `asposecellscloud-24.4/asposecellscloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/shapes_response.py` & `asposecellscloud-24.4/asposecellscloud/models/shapes_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/single_value.py` & `asposecellscloud-24.4/asposecellscloud/models/single_value.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/single_value_response.py` & `asposecellscloud-24.4/asposecellscloud/models/single_value_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/smart_marker_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/convert_task_parameter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="SmartMarkerTaskParameterpy.cs">
+<copyright company="Aspose" file="ConvertTaskParameterpy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class SmartMarkerTaskParameter(object):
+class ConvertTaskParameter(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,91 +41,123 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'source_workbook' : 'FileSource',
-        'destination_workbook' : 'FileSource',
-        'xml_file' : 'FileSource'
+        'data_source' : 'DataSource',
+        'workbook' : 'FileSource',
+        'destination_file' : 'str',
+        'region' : 'str',
+        'save_options' : 'SaveOptions'
     }
 
     attribute_map = {
-        'source_workbook' : 'SourceWorkbook' ,
-        'destination_workbook' : 'DestinationWorkbook' ,
-        'xml_file' : 'xmlFile' 
+        'data_source' : 'DataSource' ,
+        'workbook' : 'Workbook' ,
+        'destination_file' : 'DestinationFile' ,
+        'region' : 'Region' ,
+        'save_options' : 'SaveOptions' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return SmartMarkerTaskParameter.swagger_types
+        return ConvertTaskParameter.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return SmartMarkerTaskParameter.attribute_map
+        return ConvertTaskParameter.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,source_workbook=None ,destination_workbook=None ,xml_file=None   ,**kw):
+    def __init__(self,data_source=None ,workbook=None ,destination_file=None ,region=None ,save_options=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        SmartMarkerTaskParameter - a model defined in Swagger
+        ConvertTaskParameter - a model defined in Swagger
         """
-        self.container['source_workbook'] = None 
-        self.container['destination_workbook'] = None 
-        self.container['xml_file'] = None 
+        self.container['data_source'] = None 
+        self.container['workbook'] = None 
+        self.container['destination_file'] = None 
+        self.container['region'] = None 
+        self.container['save_options'] = None 
         params = locals()
-        self.source_workbook = source_workbook
-        if 'source_workbook' in params:
-            self.source_workbook = params["source_workbook"]
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
 
 
              
-        self.destination_workbook = destination_workbook
-        if 'destination_workbook' in params:
-            self.destination_workbook = params["destination_workbook"]
+        self.workbook = workbook
+        if 'workbook' in params:
+            self.workbook = params["workbook"]
 
 
              
-        self.xml_file = xml_file
-        if 'xml_file' in params:
-            self.xml_file = params["xml_file"]
+        self.destination_file = destination_file
+        if 'destination_file' in params:
+            self.destination_file = params["destination_file"]
 
 
              
+        self.region = region
+        if 'region' in params:
+            self.region = params["region"]
 
+
+             
+        self.save_options = save_options
+        if 'save_options' in params:
+            self.save_options = params["save_options"]
+
+
+             
+
+    @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
+    def workbook(self):
+        return self.container['workbook']
+
+    @workbook.setter
+    def workbook(self, workbook):
+        self.container['workbook'] = workbook 
     @property
-    def source_workbook(self):
-        return self.container['source_workbook']
+    def destination_file(self):
+        return self.container['destination_file']
 
-    @source_workbook.setter
-    def source_workbook(self, source_workbook):
-        self.container['source_workbook'] = source_workbook 
+    @destination_file.setter
+    def destination_file(self, destination_file):
+        self.container['destination_file'] = destination_file 
     @property
-    def destination_workbook(self):
-        return self.container['destination_workbook']
+    def region(self):
+        return self.container['region']
 
-    @destination_workbook.setter
-    def destination_workbook(self, destination_workbook):
-        self.container['destination_workbook'] = destination_workbook 
+    @region.setter
+    def region(self, region):
+        self.container['region'] = region 
     @property
-    def xml_file(self):
-        return self.container['xml_file']
+    def save_options(self):
+        return self.container['save_options']
 
-    @xml_file.setter
-    def xml_file(self, xml_file):
-        self.container['xml_file'] = xml_file 
+    @save_options.setter
+    def save_options(self, save_options):
+        self.container['save_options'] = save_options 
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -161,15 +193,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, SmartMarkerTaskParameter):
+        if not isinstance(other, ConvertTaskParameter):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/solid_fill.py` & `asposecellscloud-24.4/asposecellscloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sort_key.py` & `asposecellscloud-24.4/asposecellscloud/models/sort_key.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sparkline.py` & `asposecellscloud-24.4/asposecellscloud/models/sparkline.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sparkline_group.py` & `asposecellscloud-24.4/asposecellscloud/models/sparkline_group.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sparkline_group_response.py` & `asposecellscloud-24.4/asposecellscloud/models/sparkline_group_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sparkline_groups.py` & `asposecellscloud-24.4/asposecellscloud/models/sparkline_groups.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sparkline_groups_response.py` & `asposecellscloud-24.4/asposecellscloud/models/sparkline_groups_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/spinner.py` & `asposecellscloud-24.4/asposecellscloud/models/spinner.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/spinner_response.py` & `asposecellscloud-24.4/asposecellscloud/models/spinner_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/split_result.py` & `asposecellscloud-24.4/asposecellscloud/models/split_result.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/split_result_document.py` & `asposecellscloud-24.4/asposecellscloud/models/split_result_document.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/split_result_response.py` & `asposecellscloud-24.4/asposecellscloud/models/split_result_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/split_workbook_task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/split_workbook_task_parameter.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,23 +43,27 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'workbook' : 'FileSource',
         'destination_file_position' : 'FileSource',
+        'data_source' : 'DataSource',
+        'target_data_source' : 'DataSource',
         'destination_file_format' : 'str',
         'split_name_rule' : 'str',
         'vertical_resolution' : 'int',
         'horizontal_resolution' : 'int'
     }
 
     attribute_map = {
         'workbook' : 'Workbook' ,
         'destination_file_position' : 'DestinationFilePosition' ,
+        'data_source' : 'DataSource' ,
+        'target_data_source' : 'TargetDataSource' ,
         'destination_file_format' : 'DestinationFileFormat' ,
         'split_name_rule' : 'SplitNameRule' ,
         'vertical_resolution' : 'VerticalResolution' ,
         'horizontal_resolution' : 'HorizontalResolution' 
     }
 
     @staticmethod
@@ -71,25 +75,27 @@
         return SplitWorkbookTaskParameter.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbook=None ,destination_file_position=None ,destination_file_format=None ,split_name_rule=None ,vertical_resolution=None ,horizontal_resolution=None   ,**kw):
+    def __init__(self,workbook=None ,destination_file_position=None ,data_source=None ,target_data_source=None ,destination_file_format=None ,split_name_rule=None ,vertical_resolution=None ,horizontal_resolution=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
         SplitWorkbookTaskParameter - a model defined in Swagger
         """
         self.container['workbook'] = None 
         self.container['destination_file_position'] = None 
+        self.container['data_source'] = None 
+        self.container['target_data_source'] = None 
         self.container['destination_file_format'] = None 
         self.container['split_name_rule'] = None 
         self.container['vertical_resolution'] = None 
         self.container['horizontal_resolution'] = None 
         params = locals()
         self.workbook = workbook
         if 'workbook' in params:
@@ -99,14 +105,26 @@
              
         self.destination_file_position = destination_file_position
         if 'destination_file_position' in params:
             self.destination_file_position = params["destination_file_position"]
 
 
              
+        self.data_source = data_source
+        if 'data_source' in params:
+            self.data_source = params["data_source"]
+
+
+             
+        self.target_data_source = target_data_source
+        if 'target_data_source' in params:
+            self.target_data_source = params["target_data_source"]
+
+
+             
         self.destination_file_format = destination_file_format
         if 'destination_file_format' in params:
             self.destination_file_format = params["destination_file_format"]
 
 
              
         self.split_name_rule = split_name_rule
@@ -139,14 +157,28 @@
     def destination_file_position(self):
         return self.container['destination_file_position']
 
     @destination_file_position.setter
     def destination_file_position(self, destination_file_position):
         self.container['destination_file_position'] = destination_file_position 
     @property
+    def data_source(self):
+        return self.container['data_source']
+
+    @data_source.setter
+    def data_source(self, data_source):
+        self.container['data_source'] = data_source 
+    @property
+    def target_data_source(self):
+        return self.container['target_data_source']
+
+    @target_data_source.setter
+    def target_data_source(self, target_data_source):
+        self.container['target_data_source'] = target_data_source 
+    @property
     def destination_file_format(self):
         return self.container['destination_file_format']
 
     @destination_file_format.setter
     def destination_file_format(self, destination_file_format):
         self.container['destination_file_format'] = destination_file_format 
     @property
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/spreadsheet_m_l2003_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/spreadsheet_m_l2003_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/sql_script_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/sql_script_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/storage_exist.py` & `asposecellscloud-24.4/asposecellscloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/storage_file.py` & `asposecellscloud-24.4/asposecellscloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/style.py` & `asposecellscloud-24.4/asposecellscloud/models/style.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/style_format_condition.py` & `asposecellscloud-24.4/asposecellscloud/models/style_format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/style_response.py` & `asposecellscloud-24.4/asposecellscloud/models/style_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/styles.py` & `asposecellscloud-24.4/asposecellscloud/models/styles.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/svg_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/svg_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/table_total_request.py` & `asposecellscloud-24.4/asposecellscloud/models/table_total_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_data.py` & `asposecellscloud-24.4/asposecellscloud/models/task_data.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_description.py` & `asposecellscloud-24.4/asposecellscloud/models/task_description.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/task_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_result_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/task_result_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_run_result.py` & `asposecellscloud-24.4/asposecellscloud/models/task_run_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
         'description' : 'str',
-        'out_file_list' : 'list[FileSource]'
+        'out_file_list' : 'list[DataSource]'
     }
 
     attribute_map = {
         'description' : 'Description' ,
         'out_file_list' : 'OutFileList' 
     }
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/task_run_result_response.py` & `asposecellscloud-24.4/asposecellscloud/models/task_run_result_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_box.py` & `asposecellscloud-24.4/asposecellscloud/models/text_box.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_box_response.py` & `asposecellscloud-24.4/asposecellscloud/models/text_box_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_format_condition.py` & `asposecellscloud-24.4/asposecellscloud/models/text_format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_item.py` & `asposecellscloud-24.4/asposecellscloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_item_response.py` & `asposecellscloud-24.4/asposecellscloud/models/text_item_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_items.py` & `asposecellscloud-24.4/asposecellscloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_items_response.py` & `asposecellscloud-24.4/asposecellscloud/models/text_items_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_options.py` & `asposecellscloud-24.4/asposecellscloud/models/text_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/text_water_marker_request.py` & `asposecellscloud-24.4/asposecellscloud/models/text_water_marker_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/texture_fill.py` & `asposecellscloud-24.4/asposecellscloud/models/texture_fill.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/theme_color.py` & `asposecellscloud-24.4/asposecellscloud/models/theme_color.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/tick_labels.py` & `asposecellscloud-24.4/asposecellscloud/models/tick_labels.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/tick_labels_response.py` & `asposecellscloud-24.4/asposecellscloud/models/tick_labels_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/tile_pic_option.py` & `asposecellscloud-24.4/asposecellscloud/models/tile_pic_option.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/time_period_format_condition.py` & `asposecellscloud-24.4/asposecellscloud/models/time_period_format_condition.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/title.py` & `asposecellscloud-24.4/asposecellscloud/models/title.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/title_response.py` & `asposecellscloud-24.4/asposecellscloud/models/title_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/top10.py` & `asposecellscloud-24.4/asposecellscloud/models/top10.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/top10_filter.py` & `asposecellscloud-24.4/asposecellscloud/models/top10_filter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/trendline.py` & `asposecellscloud-24.4/asposecellscloud/models/trendline.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/trendline_response.py` & `asposecellscloud-24.4/asposecellscloud/models/trendline_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/trendlines.py` & `asposecellscloud-24.4/asposecellscloud/models/trendlines.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/trendlines_response.py` & `asposecellscloud-24.4/asposecellscloud/models/trendlines_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/txt_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/txt_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/validation.py` & `asposecellscloud-24.4/asposecellscloud/models/validation.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/validation_response.py` & `asposecellscloud-24.4/asposecellscloud/models/validation_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/validations.py` & `asposecellscloud-24.4/asposecellscloud/models/validations_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="Validationspy.cs">
+<copyright company="Aspose" file="ValidationsResponsepy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class Validations(object):
+class ValidationsResponse(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,91 +41,91 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'count' : 'int',
-        'validation_list' : 'list[LinkElement]',
-        'link' : 'Link'
+        'validations' : 'Validations',
+        'code' : 'int',
+        'status' : 'str'
     }
 
     attribute_map = {
-        'count' : 'Count' ,
-        'validation_list' : 'ValidationList' ,
-        'link' : 'link' 
+        'validations' : 'Validations' ,
+        'code' : 'Code' ,
+        'status' : 'Status' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return Validations.swagger_types
+        return ValidationsResponse.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return Validations.attribute_map
+        return ValidationsResponse.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,count=None ,validation_list=None ,link=None   ,**kw):
+    def __init__(self,validations=None ,code=None ,status=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        Validations - a model defined in Swagger
+        ValidationsResponse - a model defined in Swagger
         """
-        self.container['count'] = None 
-        self.container['validation_list'] = None 
-        self.container['link'] = None 
+        self.container['validations'] = None 
+        self.container['code'] = None 
+        self.container['status'] = None 
         params = locals()
-        self.count = count
-        if 'count' in params:
-            self.count = params["count"]
+        self.validations = validations
+        if 'validations' in params:
+            self.validations = params["validations"]
 
 
              
-        self.validation_list = validation_list
-        if 'validation_list' in params:
-            self.validation_list = params["validation_list"]
+        self.code = code
+        if 'code' in params:
+            self.code = params["code"]
 
 
              
-        self.link = link
-        if 'link' in params:
-            self.link = params["link"]
+        self.status = status
+        if 'status' in params:
+            self.status = params["status"]
 
 
              
 
     @property
-    def count(self):
-        return self.container['count']
+    def validations(self):
+        return self.container['validations']
 
-    @count.setter
-    def count(self, count):
-        self.container['count'] = count 
+    @validations.setter
+    def validations(self, validations):
+        self.container['validations'] = validations 
     @property
-    def validation_list(self):
-        return self.container['validation_list']
+    def code(self):
+        return self.container['code']
 
-    @validation_list.setter
-    def validation_list(self, validation_list):
-        self.container['validation_list'] = validation_list 
+    @code.setter
+    def code(self, code):
+        self.container['code'] = code 
     @property
-    def link(self):
-        return self.container['link']
+    def status(self):
+        return self.container['status']
 
-    @link.setter
-    def link(self, link):
-        self.container['link'] = link 
+    @status.setter
+    def status(self, status):
+        self.container['status'] = status 
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -161,15 +161,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, Validations):
+        if not isinstance(other, ValidationsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/validations_response.py` & `asposecellscloud-24.4/asposecellscloud/models/workbooks_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="ValidationsResponsepy.cs">
+<copyright company="Aspose" file="WorkbooksResponsepy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class ValidationsResponse(object):
+class WorkbooksResponse(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,54 +41,54 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'validations' : 'Validations',
+        'workbooks' : 'list[LinkElement]',
         'code' : 'int',
         'status' : 'str'
     }
 
     attribute_map = {
-        'validations' : 'Validations' ,
+        'workbooks' : 'Workbooks' ,
         'code' : 'Code' ,
         'status' : 'Status' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return ValidationsResponse.swagger_types
+        return WorkbooksResponse.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return ValidationsResponse.attribute_map
+        return WorkbooksResponse.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,validations=None ,code=None ,status=None   ,**kw):
+    def __init__(self,workbooks=None ,code=None ,status=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        ValidationsResponse - a model defined in Swagger
+        WorkbooksResponse - a model defined in Swagger
         """
-        self.container['validations'] = None 
+        self.container['workbooks'] = None 
         self.container['code'] = None 
         self.container['status'] = None 
         params = locals()
-        self.validations = validations
-        if 'validations' in params:
-            self.validations = params["validations"]
+        self.workbooks = workbooks
+        if 'workbooks' in params:
+            self.workbooks = params["workbooks"]
 
 
              
         self.code = code
         if 'code' in params:
             self.code = params["code"]
 
@@ -98,20 +98,20 @@
         if 'status' in params:
             self.status = params["status"]
 
 
              
 
     @property
-    def validations(self):
-        return self.container['validations']
+    def workbooks(self):
+        return self.container['workbooks']
 
-    @validations.setter
-    def validations(self, validations):
-        self.container['validations'] = validations 
+    @workbooks.setter
+    def workbooks(self, workbooks):
+        self.container['workbooks'] = workbooks 
     @property
     def code(self):
         return self.container['code']
 
     @code.setter
     def code(self, code):
         self.container['code'] = code 
@@ -161,15 +161,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, ValidationsResponse):
+        if not isinstance(other, WorkbooksResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/vertical_page_break.py` & `asposecellscloud-24.4/asposecellscloud/models/vertical_page_break.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/vertical_page_break_response.py` & `asposecellscloud-24.4/asposecellscloud/models/vertical_page_break_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/vertical_page_breaks.py` & `asposecellscloud-24.4/asposecellscloud/models/vertical_page_breaks.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/vertical_page_breaks_response.py` & `asposecellscloud-24.4/asposecellscloud/models/vertical_page_breaks_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/walls.py` & `asposecellscloud-24.4/asposecellscloud/models/walls.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/walls_response.py` & `asposecellscloud-24.4/asposecellscloud/models/walls_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_encryption_request.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_encryption_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_protection_request.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_protection_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_replace_response.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_response.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_settings.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_settings.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_settings_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_settings_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbook_settings_response.py` & `asposecellscloud-24.4/asposecellscloud/models/workbook_settings_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/workbooks_response.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="WorkbooksResponsepy.cs">
+<copyright company="Aspose" file="WorksheetResponsepy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class WorkbooksResponse(object):
+class WorksheetResponse(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,54 +41,54 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'workbooks' : 'list[LinkElement]',
+        'worksheet' : 'Worksheet',
         'code' : 'int',
         'status' : 'str'
     }
 
     attribute_map = {
-        'workbooks' : 'Workbooks' ,
+        'worksheet' : 'Worksheet' ,
         'code' : 'Code' ,
         'status' : 'Status' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return WorkbooksResponse.swagger_types
+        return WorksheetResponse.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return WorkbooksResponse.attribute_map
+        return WorksheetResponse.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,workbooks=None ,code=None ,status=None   ,**kw):
+    def __init__(self,worksheet=None ,code=None ,status=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        WorkbooksResponse - a model defined in Swagger
+        WorksheetResponse - a model defined in Swagger
         """
-        self.container['workbooks'] = None 
+        self.container['worksheet'] = None 
         self.container['code'] = None 
         self.container['status'] = None 
         params = locals()
-        self.workbooks = workbooks
-        if 'workbooks' in params:
-            self.workbooks = params["workbooks"]
+        self.worksheet = worksheet
+        if 'worksheet' in params:
+            self.worksheet = params["worksheet"]
 
 
              
         self.code = code
         if 'code' in params:
             self.code = params["code"]
 
@@ -98,20 +98,20 @@
         if 'status' in params:
             self.status = params["status"]
 
 
              
 
     @property
-    def workbooks(self):
-        return self.container['workbooks']
+    def worksheet(self):
+        return self.container['worksheet']
 
-    @workbooks.setter
-    def workbooks(self, workbooks):
-        self.container['workbooks'] = workbooks 
+    @worksheet.setter
+    def worksheet(self, worksheet):
+        self.container['worksheet'] = worksheet 
     @property
     def code(self):
         return self.container['code']
 
     @code.setter
     def code(self, code):
         self.container['code'] = code 
@@ -161,15 +161,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorkbooksResponse):
+        if not isinstance(other, WorksheetResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet_data_statistics.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet_data_statistics.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet_moving_request.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet_moving_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet_operate_parameter.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet_operate_parameter.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet_replace_response.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheet_replace_response.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheet_response.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheets_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="WorksheetResponsepy.cs">
+<copyright company="Aspose" file="WorksheetsResponsepy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class WorksheetResponse(object):
+class WorksheetsResponse(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,54 +41,54 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'worksheet' : 'Worksheet',
+        'worksheets' : 'Worksheets',
         'code' : 'int',
         'status' : 'str'
     }
 
     attribute_map = {
-        'worksheet' : 'Worksheet' ,
+        'worksheets' : 'Worksheets' ,
         'code' : 'Code' ,
         'status' : 'Status' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return WorksheetResponse.swagger_types
+        return WorksheetsResponse.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return WorksheetResponse.attribute_map
+        return WorksheetsResponse.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,worksheet=None ,code=None ,status=None   ,**kw):
+    def __init__(self,worksheets=None ,code=None ,status=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        WorksheetResponse - a model defined in Swagger
+        WorksheetsResponse - a model defined in Swagger
         """
-        self.container['worksheet'] = None 
+        self.container['worksheets'] = None 
         self.container['code'] = None 
         self.container['status'] = None 
         params = locals()
-        self.worksheet = worksheet
-        if 'worksheet' in params:
-            self.worksheet = params["worksheet"]
+        self.worksheets = worksheets
+        if 'worksheets' in params:
+            self.worksheets = params["worksheets"]
 
 
              
         self.code = code
         if 'code' in params:
             self.code = params["code"]
 
@@ -98,20 +98,20 @@
         if 'status' in params:
             self.status = params["status"]
 
 
              
 
     @property
-    def worksheet(self):
-        return self.container['worksheet']
+    def worksheets(self):
+        return self.container['worksheets']
 
-    @worksheet.setter
-    def worksheet(self, worksheet):
-        self.container['worksheet'] = worksheet 
+    @worksheets.setter
+    def worksheets(self, worksheets):
+        self.container['worksheets'] = worksheets 
     @property
     def code(self):
         return self.container['code']
 
     @code.setter
     def code(self, code):
         self.container['code'] = code 
@@ -161,15 +161,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorksheetResponse):
+        if not isinstance(other, WorksheetsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheets.py` & `asposecellscloud-24.4/asposecellscloud/models/worksheets.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/worksheets_response.py` & `asposecellscloud-24.4/asposecellscloud/models/pivot_column.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding: utf-8
 """
-<copyright company="Aspose" file="WorksheetsResponsepy.cs">
+<copyright company="Aspose" file="PivotColumnpy.cs">
   Copyright (c) 2024 Aspose.Cells Cloud
 </copyright>
 <summary>
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -24,15 +24,15 @@
 </summary>
 """
 
 from pprint import pformat
 from six import iteritems
 import re
 
-class WorksheetsResponse(object):
+class PivotColumn(object):
 
     """
     NOTE: This class is auto generated by the swagger code generator program.
     Do not edit the class manually.
     """
 
 
@@ -41,91 +41,75 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
 
     swagger_types = {
-        'worksheets' : 'Worksheets',
-        'code' : 'int',
-        'status' : 'str'
+        'pivot_column_name' : 'str',
+        'value_column_names' : 'list[str]'
     }
 
     attribute_map = {
-        'worksheets' : 'Worksheets' ,
-        'code' : 'Code' ,
-        'status' : 'Status' 
+        'pivot_column_name' : 'PivotColumnName' ,
+        'value_column_names' : 'ValueColumnNames' 
     }
 
     @staticmethod
     def get_swagger_types():
-        return WorksheetsResponse.swagger_types
+        return PivotColumn.swagger_types
 
     @staticmethod
     def get_attribute_map():
-        return WorksheetsResponse.attribute_map
+        return PivotColumn.attribute_map
 
     def get_from_container(self, attr):
         if attr in self.container:
             return self.container[attr]
         return None
 
-    def __init__(self,worksheets=None ,code=None ,status=None   ,**kw):
+    def __init__(self,pivot_column_name=None ,value_column_names=None   ,**kw):
         """
         Associative dict for storing property values
         """
         self.container = {}
 
         """
-        WorksheetsResponse - a model defined in Swagger
+        PivotColumn - a model defined in Swagger
         """
-        self.container['worksheets'] = None 
-        self.container['code'] = None 
-        self.container['status'] = None 
+        self.container['pivot_column_name'] = None 
+        self.container['value_column_names'] = None 
         params = locals()
-        self.worksheets = worksheets
-        if 'worksheets' in params:
-            self.worksheets = params["worksheets"]
+        self.pivot_column_name = pivot_column_name
+        if 'pivot_column_name' in params:
+            self.pivot_column_name = params["pivot_column_name"]
 
 
              
-        self.code = code
-        if 'code' in params:
-            self.code = params["code"]
+        self.value_column_names = value_column_names
+        if 'value_column_names' in params:
+            self.value_column_names = params["value_column_names"]
 
 
              
-        self.status = status
-        if 'status' in params:
-            self.status = params["status"]
 
-
-             
-
-    @property
-    def worksheets(self):
-        return self.container['worksheets']
-
-    @worksheets.setter
-    def worksheets(self, worksheets):
-        self.container['worksheets'] = worksheets 
     @property
-    def code(self):
-        return self.container['code']
+    def pivot_column_name(self):
+        return self.container['pivot_column_name']
 
-    @code.setter
-    def code(self, code):
-        self.container['code'] = code 
+    @pivot_column_name.setter
+    def pivot_column_name(self, pivot_column_name):
+        self.container['pivot_column_name'] = pivot_column_name 
     @property
-    def status(self):
-        return self.container['status']
+    def value_column_names(self):
+        return self.container['value_column_names']
 
-    @status.setter
-    def status(self, status):
-        self.container['status'] = status 
+    @value_column_names.setter
+    def value_column_names(self, value_column_names):
+        self.container['value_column_names'] = value_column_names 
 
     def to_dict(self):
         """
         Returns the model properties as a dict
         """
         result = {}
 
@@ -161,15 +145,15 @@
         """
         return self.to_str()
 
     def __eq__(self, other):
         """
         Returns true if both objects are equal
         """
-        if not isinstance(other, WorksheetsResponse):
+        if not isinstance(other, PivotColumn):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """
         Returns true if both objects are not equal
```

### Comparing `asposecellscloud-24.3/asposecellscloud/models/write_protection.py` & `asposecellscloud-24.4/asposecellscloud/models/write_protection.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/xls_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/xls_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/xlsb_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/xlsb_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/xml_data_binding.py` & `asposecellscloud-24.4/asposecellscloud/models/xml_data_binding.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/xml_map.py` & `asposecellscloud-24.4/asposecellscloud/models/xml_map.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/models/xps_save_options.py` & `asposecellscloud-24.4/asposecellscloud/models/xps_save_options.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/__init__.py` & `asposecellscloud-24.4/asposecellscloud/requests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,15 @@
 from asposecellscloud.requests.post_workbook_data_cleansing_request import PostWorkbookDataCleansingRequest
 from asposecellscloud.requests.post_data_cleansing_request import PostDataCleansingRequest
 from asposecellscloud.requests.post_workbook_data_deduplication_request import PostWorkbookDataDeduplicationRequest
 from asposecellscloud.requests.post_data_deduplication_request import PostDataDeduplicationRequest
 from asposecellscloud.requests.post_workbook_data_fill_request import PostWorkbookDataFillRequest
 from asposecellscloud.requests.post_data_fill_request import PostDataFillRequest
 from asposecellscloud.requests.post_delete_incomplete_rows_request import PostDeleteIncompleteRowsRequest
+from asposecellscloud.requests.post_data_transformation_request import PostDataTransformationRequest
 from asposecellscloud.requests.get_worksheet_hyperlinks_request import GetWorksheetHyperlinksRequest
 from asposecellscloud.requests.get_worksheet_hyperlink_request import GetWorksheetHyperlinkRequest
 from asposecellscloud.requests.delete_worksheet_hyperlink_request import DeleteWorksheetHyperlinkRequest
 from asposecellscloud.requests.post_worksheet_hyperlink_request import PostWorksheetHyperlinkRequest
 from asposecellscloud.requests.put_worksheet_hyperlink_request import PutWorksheetHyperlinkRequest
 from asposecellscloud.requests.delete_worksheet_hyperlinks_request import DeleteWorksheetHyperlinksRequest
 from asposecellscloud.requests.post_assemble_request import PostAssembleRequest
```

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/copy_file_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/copy_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/copy_folder_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/copy_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/create_folder_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/create_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_decrypt_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_decrypt_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_document_properties_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_document_property_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_document_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_document_un_protect_from_changes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_file_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_folder_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_header_footer_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_header_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_horizontal_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_horizontal_page_breaks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_horizontal_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_metadata_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_pivot_table_field_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_un_protect_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_un_protect_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_unprotect_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_unprotect_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_vertical_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_vertical_page_breaks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_vertical_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_background_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_name_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_workbook_names_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_workbook_names_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_background_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_cells_range_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_cells_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_legend_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_chart_title_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_charts_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_charts_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_comment_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_comments_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_comments_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formatting_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_conditional_formattings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_date_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_date_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_freeze_panes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_hyperlink_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_list_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_list_objects_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_list_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_ole_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_ole_objects_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_ole_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_picture_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_picture_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pictures_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pictures_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_filters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_table_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_pivot_tables_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_row_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_shapes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_shapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_sparkline_groups_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_validation_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheet_validations_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheet_validations_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/delete_worksheets_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/delete_worksheets_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/download_file_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/download_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_cell_html_string_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_cell_html_string_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_cells_cloud_service_status_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_cells_cloud_service_status_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_cells_cloud_services_health_check_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_border_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_fill_format_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_fill_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_area_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_category_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_second_category_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_second_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_second_value_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_second_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_series_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_series_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_chart_value_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_chart_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_disc_usage_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_disc_usage_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_document_properties_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_document_properties_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_document_property_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_document_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_file_versions_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_file_versions_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_files_list_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_files_list_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_footer_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_header_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_header_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_horizontal_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_horizontal_page_breaks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_horizontal_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_metadata_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_named_range_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_named_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_named_ranges_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_named_ranges_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_page_count_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_page_count_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_page_setup_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_pivot_table_field_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_vertical_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_vertical_page_breaks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_vertical_page_breaks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_default_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_default_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_name_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_name_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_name_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_names_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_names_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_settings_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_settings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_workbook_text_items_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_workbook_text_items_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_auto_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_auto_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_autoshape_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_autoshapes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_autoshapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_calculate_formula_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cell_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cell_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cells_range_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cells_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_cells_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_cells_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_legend_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_chart_title_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_charts_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_charts_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_column_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_column_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_comment_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_comments_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_comments_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_conditional_formattings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_hyperlink_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_hyperlinks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_hyperlinks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_list_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_list_objects_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_list_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_merged_cell_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_merged_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_merged_cells_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_merged_cells_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_ole_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_ole_objects_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_ole_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_page_count_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_page_count_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_picture_with_format_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_picture_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pictures_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pictures_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_filters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_table_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_pivot_tables_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_pivot_tables_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_row_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_shapes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_shapes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_sparkline_group_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_sparkline_groups_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_text_items_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_text_items_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_validation_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_validations_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_validations_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheet_with_format_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheet_with_format_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/get_worksheets_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/get_worksheets_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/move_file_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/move_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/move_folder_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/move_folder_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/object_exists_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/object_exists_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_analyze_excel_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_analyze_excel_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_assemble_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_assemble_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_autofit_workbook_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_autofit_workbook_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_autofit_workbook_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_autofit_workbook_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_row_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_autofit_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_autofit_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_batch_convert_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_batch_convert_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_batch_lock_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_batch_lock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_batch_protect_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_batch_protect_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_batch_split_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_batch_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_batch_unlock_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_batch_unlock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_cell_calculate_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_cell_calculate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_cell_characters_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_cell_characters_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_chart_category_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_chart_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_chart_second_category_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_chart_second_category_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_chart_second_value_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_chart_second_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_chart_series_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_chart_series_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_chart_value_axis_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_chart_value_axis_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_clear_contents_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_clear_contents_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_clear_formats_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_clear_formats_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_clear_objects_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_clear_objects_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_column_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_column_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_compress_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_compress_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_csv_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_csv_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_docx_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_docx_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_html_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_html_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_json_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_json_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_markdown_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_pdf_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_png_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_png_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_pptx_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_convert_workbook_to_sql_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_convert_workbook_to_sql_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_copy_cell_into_cell_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_copy_cell_into_cell_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_copy_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_copy_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_data_cleansing_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_data_cleansing_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_data_deduplication_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_data_deduplication_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_data_fill_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_data_fill_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_delete_incomplete_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_delete_incomplete_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_digital_signature_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_digital_signature_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_encrypt_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_encrypt_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_export_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_export_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_fit_tall_to_pages_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_fit_tall_to_pages_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_fit_wide_to_pages_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_fit_wide_to_pages_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_footer_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_footer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_group_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_group_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_group_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_group_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_header_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_header_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_hide_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_hide_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_hide_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_hide_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_import_data_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_import_data_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_import_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_import_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_lock_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_lock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_merge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_metadata_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_metadata_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_move_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_move_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_page_setup_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_page_setup_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_cell_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_field_hide_item_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_field_move_to_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_field_move_to_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_update_pivot_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_pivot_table_update_pivot_fields_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_protect_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_protect_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_protect_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_protect_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_rename_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_rename_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_repair_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_repair_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_replace_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_reverse_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_reverse_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_rotate_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_rotate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_row_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_row_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_run_task_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_run_task_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_search_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_set_cell_html_string_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_set_cell_html_string_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_set_cell_range_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_set_cell_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_set_worksheet_column_width_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_set_worksheet_column_width_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_split_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_ungroup_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_ungroup_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_unhide_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_unhide_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_unhide_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_unhide_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_unlock_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_unlock_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_cell_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_cell_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_ole_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_property_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_range_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_range_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_row_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_update_worksheet_zoom_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_update_worksheet_zoom_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_watermark_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_watermark_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_calculate_formula_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_cleansing_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_cleansing_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_deduplication_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_deduplication_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_data_fill_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_data_fill_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_export_xml_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_export_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_get_smart_marker_result_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_import_json_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_import_json_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_import_xml_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_import_xml_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_name_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_save_as_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_save_as_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_settings_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_settings_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_split_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_split_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbook_text_replace_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbook_text_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbooks_merge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbooks_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_workbooks_text_search_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_workbooks_text_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_auto_filter_refresh_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_calculate_formula_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_calculate_formula_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cell_set_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cell_set_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_column_width_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_move_to_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_outline_border_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_row_height_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_sort_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_sort_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_style_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_style_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_un_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_range_value_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_range_value_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_cells_ranges_copy_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_cells_ranges_copy_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_legend_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_chart_title_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_comment_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_group_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_group_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_hyperlink_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_column_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_column_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_columns_total_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_columns_total_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_convert_to_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_insert_slicer_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_insert_slicer_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_remove_duplicates_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_remove_duplicates_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_sort_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_list_object_summarize_with_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_match_blanks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_match_blanks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_match_non_blanks_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_merge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_picture_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_picture_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_pivot_table_calculate_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_pivot_table_move_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_range_sort_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_range_sort_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_sparkline_group_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_text_replace_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_text_replace_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_text_search_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_text_search_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_ungroup_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_unmerge_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_unmerge_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/post_worksheet_validation_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/post_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_active_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_active_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_add_new_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_add_new_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_change_visibility_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_change_visibility_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_convert_workbook_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_convert_workbook_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_document_property_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_document_property_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_document_protect_from_changes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_document_protect_from_changes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_horizontal_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_horizontal_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_insert_new_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_insert_new_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_columns_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_columns_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_row_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_row_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_insert_worksheet_rows_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_insert_worksheet_rows_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_pivot_table_field_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_pivot_table_field_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_protect_worksheet_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_protect_worksheet_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_vertical_page_break_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_vertical_page_break_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_workbook_background_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_workbook_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_workbook_create_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_workbook_create_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_workbook_name_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_workbook_name_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_workbook_water_marker_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_workbook_water_marker_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_add_picture_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_add_picture_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_background_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_background_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_cells_range_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_cells_range_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_legend_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_legend_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_chart_title_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_chart_title_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_color_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_color_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_comment_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_comment_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_conditional_formatting_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_custom_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_custom_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_date_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_date_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_dynamic_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_filter_top10_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_filter_top10_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_area_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_area_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_format_condition_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_format_condition_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_freeze_panes_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_freeze_panes_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_hyperlink_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_hyperlink_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_icon_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_icon_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_list_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_list_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_ole_object_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_ole_object_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_pivot_table_filter_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_pivot_table_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_pivot_table_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_shape_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_shape_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_sparkline_group_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_sparkline_group_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/put_worksheet_validation_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/put_worksheet_validation_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/storage_exists_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/storage_exists_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/requests/upload_file_request.py` & `asposecellscloud-24.4/asposecellscloud/requests/upload_file_request.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud/rest.py` & `asposecellscloud-24.4/asposecellscloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/asposecellscloud.egg-info/PKG-INFO` & `asposecellscloud-24.4/asposecellscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: asposecellscloud
-Version: 24.3
+Version: 24.4
 Summary: Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications.
 Home-page: https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
 Author: Aspose Cloud
 Author-email: Aspose Cloud <aspose.cloud@aspose.com>
 Project-URL: Homepage, https://github.com/aspose-cells-cloud/aspose-cells-cloud-python
-Keywords: excel,spreadsheet,xlsx,convert,aspose.cells,cloud
+Keywords: excel,spreadsheet,convert,xlsx,pdf,json,cloud,rest api,merge,split,protect
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
 Requires-Dist: six>=1.10
 Requires-Dist: certifi
 Requires-Dist: python-dateutil
 
-![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.3)
+![](https://img.shields.io/badge/REST%20API-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposecellscloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposecellscloud) ![PyPI - Downloads](https://img.shields.io/pypi/dm/asposecellscloud)  [![GitHub license](https://img.shields.io/github/license/aspose-cells-cloud/aspose-cells-cloud-python)](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/blob/master/LICENSE) ![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/aspose-cells-cloud/aspose-cells-cloud-python/24.4)
 
 Aspose.Cells Cloud for Python enables you to handle various aspects of Excel files, including cell data, styles, formulas, charts, pivot tables, data validation, comments, drawing objects, images, hyperlinks, and so on. Additionally, it supports operations such as splitting, merging, repairing, and converting to other compatible file formats.
 
 # Python package for Aspose.Cells Cloud
 
 
 Enhance your Python applications with the [Aspose.Cells Cloud](https://products.aspose.cloud/cells/python) , enabling seamless integration with [Excel, ODS, CSV, Json and other spreadsheet document formats](https://docs.aspose.cloud/cells/supported-file-formats/). With its powerful APIs, developers can effortlessly read, convert, create, edit, and manipulate the contents of Excel documents without the need for any office software installed on the machine.
@@ -40,22 +40,19 @@
 - Data Verification: Includes data verification function to set cell data type, range, uniqueness, ensuring data accuracy and integrity.
 - Batch Processing: Supports batch processing of multiple Excel documents, such as batch format conversion, data extraction, and style application..
 - Import/Export: Facilitates importing data from various sources into spreadsheets and exporting spreadsheet data to other formats.
 - Security Management: Offers a range of security features like data encryption, access control, and permission management to safeguard the security and integrity of spreadsheet data.
 
 
 
-## Feature & Enhancements in Version 24.3
+## Feature & Enhancements in Version 24.4
 
 Full list of issues covering all changes in this release:
 
-- Support data deduplication.
-- Support data filling.
-- Support to delete incomplete rows.
-- Support data cleansing.
+- Support data transformation.
 
 ## Support file format
 
 |**Format**|**Description**|**Load**|**Save**|
 | :- | :- | :- | :- |
 |[XLS](https://docs.fileformat.com/spreadsheet/xls/)|Excel 95/5.0 - 2003 Workbook.|&radic;|&radic;|
 |[XLSX](https://docs.fileformat.com/spreadsheet/xlsx/)|Office Open XML SpreadsheetML Workbook or template file, with or without macros.|&radic;|&radic;|
@@ -145,14 +142,21 @@
 
 
 [Product Page](https://products.aspose.cloud/cells/python) | [Documentation](https://docs.aspose.cloud/cells/) | [Live Demo](https://products.aspose.app/cells/family) | [API Reference](https://apireference.aspose.cloud/cells/) | [Code Samples](https://github.com/aspose-cells-cloud/aspose-cells-cloud-python/tree/master/test) | [Blog](https://blog.aspose.cloud/category/cells/) | [Free Support](https://forum.aspose.cloud/c/cells) | [Free Trial](https://dashboard.aspose.cloud/#/apps)
 
 
 # Release history version
 
+## Enhancements in Version 24.3
+
+- Support data deduplication.
+- Support data filling.
+- Support to delete incomplete rows.
+- Support data cleansing.
+
 ## Enhancements in Version 24.2.1
 
 - Support data deduplication.
 
 ## Enhancements in Version 24.1.1
 
 - Fixed spelling mistakes for several functions.
```

### Comparing `asposecellscloud-24.3/asposecellscloud.egg-info/SOURCES.txt` & `asposecellscloud-24.4/asposecellscloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -116,18 +116,21 @@
 asposecellscloud/models/data_cleansing.py
 asposecellscloud/models/data_cleansing_request.py
 asposecellscloud/models/data_column_fill_value.py
 asposecellscloud/models/data_deduplication_request.py
 asposecellscloud/models/data_fill.py
 asposecellscloud/models/data_fill_request.py
 asposecellscloud/models/data_fill_value.py
+asposecellscloud/models/data_item.py
 asposecellscloud/models/data_labels.py
 asposecellscloud/models/data_labels_response.py
 asposecellscloud/models/data_sorter.py
 asposecellscloud/models/data_sorter_key.py
+asposecellscloud/models/data_source.py
+asposecellscloud/models/data_transformation_request.py
 asposecellscloud/models/date_time_group_item.py
 asposecellscloud/models/deduplication_region.py
 asposecellscloud/models/delete_incomplete_rows_request.py
 asposecellscloud/models/dif_save_options.py
 asposecellscloud/models/digital_signature.py
 asposecellscloud/models/disc_usage.py
 asposecellscloud/models/discover_chart.py
@@ -219,15 +222,17 @@
 asposecellscloud/models/list_box_response.py
 asposecellscloud/models/list_column.py
 asposecellscloud/models/list_object.py
 asposecellscloud/models/list_object_operate_parameter.py
 asposecellscloud/models/list_object_response.py
 asposecellscloud/models/list_objects.py
 asposecellscloud/models/list_objects_response.py
+asposecellscloud/models/load_data.py
 asposecellscloud/models/load_options.py
+asposecellscloud/models/load_to.py
 asposecellscloud/models/m_html_save_options.py
 asposecellscloud/models/markdown_save_options.py
 asposecellscloud/models/marker.py
 asposecellscloud/models/match_condition_request.py
 asposecellscloud/models/merged_cell.py
 asposecellscloud/models/merged_cell_response.py
 asposecellscloud/models/merged_cells.py
@@ -265,14 +270,15 @@
 asposecellscloud/models/pdf_save_options.py
 asposecellscloud/models/pdf_security_options.py
 asposecellscloud/models/pic_format_option.py
 asposecellscloud/models/picture.py
 asposecellscloud/models/picture_response.py
 asposecellscloud/models/pictures.py
 asposecellscloud/models/pictures_response.py
+asposecellscloud/models/pivot_column.py
 asposecellscloud/models/pivot_field.py
 asposecellscloud/models/pivot_field_response.py
 asposecellscloud/models/pivot_filter.py
 asposecellscloud/models/pivot_filter_response.py
 asposecellscloud/models/pivot_filters_response.py
 asposecellscloud/models/pivot_globalization_settings.py
 asposecellscloud/models/pivot_item.py
@@ -284,14 +290,15 @@
 asposecellscloud/models/pivot_tables_response.py
 asposecellscloud/models/plot_area.py
 asposecellscloud/models/plot_area_response.py
 asposecellscloud/models/pptx_save_options.py
 asposecellscloud/models/protect_sheet_parameter.py
 asposecellscloud/models/protect_workbook_request.py
 asposecellscloud/models/protection.py
+asposecellscloud/models/query_data_source.py
 asposecellscloud/models/query_table.py
 asposecellscloud/models/radio_button.py
 asposecellscloud/models/radio_button_response.py
 asposecellscloud/models/range.py
 asposecellscloud/models/range_copy_request.py
 asposecellscloud/models/range_response.py
 asposecellscloud/models/range_set_outline_border_request.py
@@ -374,19 +381,21 @@
 asposecellscloud/models/tick_labels_response.py
 asposecellscloud/models/tile_pic_option.py
 asposecellscloud/models/time_period_format_condition.py
 asposecellscloud/models/title.py
 asposecellscloud/models/title_response.py
 asposecellscloud/models/top10.py
 asposecellscloud/models/top10_filter.py
+asposecellscloud/models/transformation.py
 asposecellscloud/models/trendline.py
 asposecellscloud/models/trendline_response.py
 asposecellscloud/models/trendlines.py
 asposecellscloud/models/trendlines_response.py
 asposecellscloud/models/txt_save_options.py
+asposecellscloud/models/unpivot_column.py
 asposecellscloud/models/validation.py
 asposecellscloud/models/validation_response.py
 asposecellscloud/models/validations.py
 asposecellscloud/models/validations_response.py
 asposecellscloud/models/vertical_page_break.py
 asposecellscloud/models/vertical_page_break_response.py
 asposecellscloud/models/vertical_page_breaks.py
@@ -595,14 +604,15 @@
 asposecellscloud/requests/post_copy_cell_into_cell_request.py
 asposecellscloud/requests/post_copy_worksheet_columns_request.py
 asposecellscloud/requests/post_copy_worksheet_request.py
 asposecellscloud/requests/post_copy_worksheet_rows_request.py
 asposecellscloud/requests/post_data_cleansing_request.py
 asposecellscloud/requests/post_data_deduplication_request.py
 asposecellscloud/requests/post_data_fill_request.py
+asposecellscloud/requests/post_data_transformation_request.py
 asposecellscloud/requests/post_delete_incomplete_rows_request.py
 asposecellscloud/requests/post_digital_signature_request.py
 asposecellscloud/requests/post_encrypt_workbook_request.py
 asposecellscloud/requests/post_export_request.py
 asposecellscloud/requests/post_fit_tall_to_pages_request.py
 asposecellscloud/requests/post_fit_wide_to_pages_request.py
 asposecellscloud/requests/post_footer_request.py
```

### Comparing `asposecellscloud-24.3/pyproject.toml` & `asposecellscloud-24.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
 name = "asposecellscloud"
-version = "24.3"
+version = "24.4"
 authors = [
   { name="Aspose Cloud", email="aspose.cloud@aspose.com" },
 ]
 description = "Python Cloud SDK wraps Aspose.Cells REST API so you could seamlessly integrate Microsoft Excel® spreadsheet generation, manipulation, conversion & inspection features into your own Python applications."
-keywords = ["excel", "spreadsheet", "xlsx", "convert", "aspose.cells","cloud"]
+keywords = ["excel", "spreadsheet",  "convert", "xlsx", "pdf", "json", "cloud", "rest api", "merge", "split", "protect"]
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `asposecellscloud-24.3/setup.py` & `asposecellscloud-24.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "asposecellscloud"
-VERSION = "24.3"
+VERSION = "24.4"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -17,15 +17,15 @@
 setup(
     name=NAME,
     version=VERSION,
     description="Python Cloud SDK wraps Aspose.Cells Cloud API so you could seamlessly integrate Microsoft Excel file generation, manipulation, conversion & inspection features into your own Python applications.",
     author="Aspose Cloud",
     author_email="aspose.cloud@aspose.com",
     url="https://github.com/aspose-cells-cloud/aspose-cells-cloud-python",
-    keywords=["excel", "spreadsheet", "xlsx", "convert", "aspose.cells","cloud"],
+    keywords=["excel", "spreadsheet", "xlsx", "convert", "merge", "split", "protect", "rest api", "cloud", "aspose.cells"],
     install_requires=REQUIRES,
     packages=['asposecellscloud', 'asposecellscloud.apis', 'asposecellscloud.models','asposecellscloud.requests'],
     include_package_data=True,
     long_description="Python Cloud SDK wraps Aspose.Cells Cloud API so you could seamlessly integrate Microsoft Excel file generation, manipulation, conversion & inspection features into your own Python applications.",
     classifiers=[
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.6',
```

### Comparing `asposecellscloud-24.3/test/tests_auto_filter_controller.py` & `asposecellscloud-24.4/test/tests_auto_filter_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_batch_controller.py` & `asposecellscloud-24.4/test/tests_batch_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_cells_controller.py` & `asposecellscloud-24.4/test/tests_cells_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_cells_status_controller.py` & `asposecellscloud-24.4/test/tests_cells_status_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_chart_area_controller.py` & `asposecellscloud-24.4/test/tests_chart_area_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_charts_controller.py` & `asposecellscloud-24.4/test/tests_charts_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_conditional_formattings_controller.py` & `asposecellscloud-24.4/test/tests_conditional_formattings_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_conversion.py` & `asposecellscloud-24.4/test/tests_conversion.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_conversion_json.py` & `asposecellscloud-24.4/test/tests_conversion_json.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_conversion_png.py` & `asposecellscloud-24.4/test/tests_conversion_png.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_data_processing_controller.py` & `asposecellscloud-24.4/test/tests_data_processing_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     def test_post_workbook_data_deduplication(self):
         remote_folder = 'TestData/In'
 
         local_name = 'BookCsvDuplicateData.csv'
         remote_name = 'BookCsvDuplicateData.csv'
 
         deduplicationRegion = DeduplicationRegion()
+        deduplicationRegion.ranges = []
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
      
         request =  PostWorkbookDataDeduplicationRequest( remote_name, deduplicationRegion,folder= remote_folder,storage_name= '')
         self.api.post_workbook_data_deduplication(request)
```

### Comparing `asposecellscloud-24.3/test/tests_file_controller.py` & `asposecellscloud-24.4/test/tests_file_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_folder_controller.py` & `asposecellscloud-24.4/test/tests_folder_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_hypelinks_controller.py` & `asposecellscloud-24.4/test/tests_hypelinks_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_light_cells.py` & `asposecellscloud-24.4/test/tests_light_cells.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_list_objects_controller.py` & `asposecellscloud-24.4/test/tests_list_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_ole_objects_controller.py` & `asposecellscloud-24.4/test/tests_ole_objects_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_one.py` & `asposecellscloud-24.4/test/tests_one.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_page_breaks_controller.py` & `asposecellscloud-24.4/test/tests_page_breaks_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_page_setup_controller.py` & `asposecellscloud-24.4/test/tests_page_setup_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_pictures_controller.py` & `asposecellscloud-24.4/test/tests_pictures_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_pivot_tables_controller.py` & `asposecellscloud-24.4/test/tests_pivot_tables_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_properties_controller.py` & `asposecellscloud-24.4/test/tests_properties_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_ranges_controller.py` & `asposecellscloud-24.4/test/tests_ranges_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_shapes_controller.py` & `asposecellscloud-24.4/test/tests_shapes_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_sparkline_groups_controller.py` & `asposecellscloud-24.4/test/tests_sparkline_groups_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_storage_controller.py` & `asposecellscloud-24.4/test/tests_storage_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_workbook_controller.py` & `asposecellscloud-24.4/test/tests_workbook_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_worksheet_controller.py` & `asposecellscloud-24.4/test/tests_worksheet_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_worksheet_validations_controller.py` & `asposecellscloud-24.4/test/tests_worksheet_validations_controller.py`

 * *Files identical despite different names*

### Comparing `asposecellscloud-24.3/test/tests_xml_controller.py` & `asposecellscloud-24.4/test/tests_xml_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     def test_post_workbook_import_xml(self):
         remote_folder = 'TestData/In'
 
         local_name = 'Template.xlsx'
         data_xml = 'data.xml'
         remote_name = 'Template.xlsx'
 
-        importXMLRequestXMLFileSource = FileSource(file_source_type= 'CloudFileSystem' ,file_path= remote_folder + '/data.xml' )
+        importXMLRequestXMLFileSource = DataSource(data_source_type= 'CloudFileSystem' ,data_path= remote_folder + '/data.xml' )
         importXMLRequestImportPosition = ImportPosition(sheet_name= 'Sheet1' ,row_index= 3 ,column_index= 4 )
         importXMLRequest = ImportXMLRequest(xml_file_source= importXMLRequestXMLFileSource ,import_position= importXMLRequestImportPosition )
         result = AuthUtil.Ready(self.api, local_name, remote_folder + '/' + remote_name ,  '')
         self.assertTrue(len(result.uploaded)>0) 
         result = AuthUtil.Ready(self.api, data_xml, remote_folder + '/data.xml' ,  '')
         self.assertTrue(len(result.uploaded)>0)
```

