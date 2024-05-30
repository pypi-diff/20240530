# Comparing `tmp/AnnoMate-0.0.3.tar.gz` & `tmp/annomate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnnoMate-0.0.3.tar", last modified: Mon Mar  4 20:57:30 2024, max compression
+gzip compressed data, was "dist/annomate-1.0.0.tar", last modified: Thu May 30 13:42:24 2024, max compression
```

## Comparing `AnnoMate-0.0.3.tar` & `annomate-1.0.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.621771 AnnoMate-0.0.3/
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.606336 AnnoMate-0.0.3/AnnoMate/
--rw-r--r--   0 cchu       (502) staff       (20)     4840 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/AnnotationDisplayComponent.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.606668 AnnoMate-0.0.3/AnnoMate/AnnotationDisplayComponents/
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/AnnotationDisplayComponents/__init__.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.612236 AnnoMate-0.0.3/AnnoMate/AppComponents/
--rw-r--r--   0 cchu       (502) staff       (20)    23899 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/CNVPlotComponent.py
--rw-r--r--   0 cchu       (502) staff       (20)     2972 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/DataTableComponents.py
--rw-r--r--   0 cchu       (502) staff       (20)    22351 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/MutationTableComponent.py
--rw-r--r--   0 cchu       (502) staff       (20)    33988 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/PhylogicNDTComponents.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)     4963 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/AppComponents/utils.py
--rw-r--r--   0 cchu       (502) staff       (20)     4731 2023-07-28 14:33:44.000000 AnnoMate-0.0.3/AnnoMate/Data.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.614925 AnnoMate-0.0.3/AnnoMate/DataTypes/
--rw-r--r--   0 cchu       (502) staff       (20)     1101 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/DataTypes/GenericData.py
--rw-r--r--   0 cchu       (502) staff       (20)      885 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/DataTypes/PatientSampleData.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/DataTypes/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)    49787 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/ReviewDataApp.py
--rw-r--r--   0 cchu       (502) staff       (20)     7395 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/ReviewDataInterface.py
--rw-r--r--   0 cchu       (502) staff       (20)    20416 2024-03-03 19:45:57.000000 AnnoMate-0.0.3/AnnoMate/ReviewerTemplate.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.617770 AnnoMate-0.0.3/AnnoMate/Reviewers/
--rw-r--r--   0 cchu       (502) staff       (20)     5900 2023-07-30 20:54:42.000000 AnnoMate-0.0.3/AnnoMate/Reviewers/ExampleReviewer.py
--rw-r--r--   0 cchu       (502) staff       (20)       43 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/Reviewers/__init__.py
--rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 AnnoMate-0.0.3/AnnoMate/__init__.py
-drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-03-04 20:57:30.621263 AnnoMate-0.0.3/AnnoMate.egg-info/
--rw-r--r--   0 cchu       (502) staff       (20)     5834 2024-03-04 20:57:30.000000 AnnoMate-0.0.3/AnnoMate.egg-info/PKG-INFO
--rw-r--r--   0 cchu       (502) staff       (20)      890 2024-03-04 20:57:30.000000 AnnoMate-0.0.3/AnnoMate.egg-info/SOURCES.txt
--rw-r--r--   0 cchu       (502) staff       (20)        1 2024-03-04 20:57:30.000000 AnnoMate-0.0.3/AnnoMate.egg-info/dependency_links.txt
--rw-r--r--   0 cchu       (502) staff       (20)      269 2024-03-04 20:57:30.000000 AnnoMate-0.0.3/AnnoMate.egg-info/requires.txt
--rw-r--r--   0 cchu       (502) staff       (20)        9 2024-03-04 20:57:30.000000 AnnoMate-0.0.3/AnnoMate.egg-info/top_level.txt
--rw-r--r--   0 cchu       (502) staff       (20)     1074 2023-06-26 16:14:26.000000 AnnoMate-0.0.3/LICENSE.txt
--rw-r--r--   0 cchu       (502) staff       (20)     5834 2024-03-04 20:57:30.622088 AnnoMate-0.0.3/PKG-INFO
--rw-r--r--   0 cchu       (502) staff       (20)     5309 2023-09-01 19:49:15.000000 AnnoMate-0.0.3/README.md
--rw-r--r--   0 cchu       (502) staff       (20)       86 2023-06-26 16:14:26.000000 AnnoMate-0.0.3/pyproject.toml
--rw-r--r--   0 cchu       (502) staff       (20)       79 2024-03-04 20:57:30.622944 AnnoMate-0.0.3/setup.cfg
--rw-r--r--   0 cchu       (502) staff       (20)     1966 2023-09-09 18:34:50.000000 AnnoMate-0.0.3/setup.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.020385 annomate-1.0.0/
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.005711 annomate-1.0.0/AnnoMate/
+-rw-r--r--   0 cchu       (502) staff       (20)     4840 2024-03-03 19:45:57.000000 annomate-1.0.0/AnnoMate/AnnotationDisplayComponent.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.006105 annomate-1.0.0/AnnoMate/AnnotationDisplayComponents/
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/AnnotationDisplayComponents/__init__.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.011193 annomate-1.0.0/AnnoMate/AppComponents/
+-rw-r--r--   0 cchu       (502) staff       (20)    23899 2024-03-03 19:45:57.000000 annomate-1.0.0/AnnoMate/AppComponents/CNVPlotComponent.py
+-rw-r--r--   0 cchu       (502) staff       (20)     2972 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/AppComponents/DataTableComponents.py
+-rw-r--r--   0 cchu       (502) staff       (20)    22351 2024-03-03 19:45:57.000000 annomate-1.0.0/AnnoMate/AppComponents/MutationTableComponent.py
+-rw-r--r--   0 cchu       (502) staff       (20)    33950 2024-05-30 13:41:26.000000 annomate-1.0.0/AnnoMate/AppComponents/PhylogicNDTComponents.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/AppComponents/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)     4963 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/AppComponents/utils.py
+-rw-r--r--   0 cchu       (502) staff       (20)     4731 2023-07-28 14:33:44.000000 annomate-1.0.0/AnnoMate/Data.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.013216 annomate-1.0.0/AnnoMate/DataTypes/
+-rw-r--r--   0 cchu       (502) staff       (20)     1101 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/DataTypes/GenericData.py
+-rw-r--r--   0 cchu       (502) staff       (20)      885 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/DataTypes/PatientSampleData.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/DataTypes/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)      842 2024-05-30 13:41:26.000000 annomate-1.0.0/AnnoMate/MetadataHandler.py
+-rw-r--r--   0 cchu       (502) staff       (20)    55384 2024-05-30 13:41:26.000000 annomate-1.0.0/AnnoMate/ReviewDataApp.py
+-rw-r--r--   0 cchu       (502) staff       (20)     7539 2024-05-30 13:41:26.000000 annomate-1.0.0/AnnoMate/ReviewDataInterface.py
+-rw-r--r--   0 cchu       (502) staff       (20)    21592 2024-05-30 13:41:26.000000 annomate-1.0.0/AnnoMate/ReviewerTemplate.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.014586 annomate-1.0.0/AnnoMate/Reviewers/
+-rw-r--r--   0 cchu       (502) staff       (20)     5900 2023-07-30 20:54:42.000000 annomate-1.0.0/AnnoMate/Reviewers/ExampleReviewer.py
+-rw-r--r--   0 cchu       (502) staff       (20)       43 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/Reviewers/__init__.py
+-rw-r--r--   0 cchu       (502) staff       (20)        0 2023-07-07 22:14:15.000000 annomate-1.0.0/AnnoMate/__init__.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.019426 annomate-1.0.0/AnnoMate.egg-info/
+-rw-r--r--   0 cchu       (502) staff       (20)     7606 2024-05-30 13:42:23.000000 annomate-1.0.0/AnnoMate.egg-info/PKG-INFO
+-rw-r--r--   0 cchu       (502) staff       (20)      951 2024-05-30 13:42:23.000000 annomate-1.0.0/AnnoMate.egg-info/SOURCES.txt
+-rw-r--r--   0 cchu       (502) staff       (20)        1 2024-05-30 13:42:23.000000 annomate-1.0.0/AnnoMate.egg-info/dependency_links.txt
+-rw-r--r--   0 cchu       (502) staff       (20)      269 2024-05-30 13:42:23.000000 annomate-1.0.0/AnnoMate.egg-info/requires.txt
+-rw-r--r--   0 cchu       (502) staff       (20)        9 2024-05-30 13:42:23.000000 annomate-1.0.0/AnnoMate.egg-info/top_level.txt
+-rw-r--r--   0 cchu       (502) staff       (20)     1074 2023-06-26 16:14:26.000000 annomate-1.0.0/LICENSE.txt
+-rw-r--r--   0 cchu       (502) staff       (20)     7606 2024-05-30 13:42:24.020175 annomate-1.0.0/PKG-INFO
+-rw-r--r--   0 cchu       (502) staff       (20)     6452 2024-05-30 13:41:26.000000 annomate-1.0.0/README.md
+-rw-r--r--   0 cchu       (502) staff       (20)       86 2023-06-26 16:14:26.000000 annomate-1.0.0/pyproject.toml
+-rw-r--r--   0 cchu       (502) staff       (20)       79 2024-05-30 13:42:24.021196 annomate-1.0.0/setup.cfg
+-rw-r--r--   0 cchu       (502) staff       (20)     1973 2024-05-30 13:41:26.000000 annomate-1.0.0/setup.py
+drwxr-xr-x   0 cchu       (502) staff       (20)        0 2024-05-30 13:42:24.018344 annomate-1.0.0/tests/
+-rw-r--r--   0 cchu       (502) staff       (20)      989 2024-05-30 13:41:26.000000 annomate-1.0.0/tests/test_example_reviewer.py
```

### Comparing `AnnoMate-0.0.3/AnnoMate/AnnotationDisplayComponent.py` & `annomate-1.0.0/AnnoMate/AnnotationDisplayComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/AppComponents/CNVPlotComponent.py` & `annomate-1.0.0/AnnoMate/AppComponents/CNVPlotComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/AppComponents/DataTableComponents.py` & `annomate-1.0.0/AnnoMate/AppComponents/DataTableComponents.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/AppComponents/MutationTableComponent.py` & `annomate-1.0.0/AnnoMate/AppComponents/MutationTableComponent.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/AppComponents/PhylogicNDTComponents.py` & `annomate-1.0.0/AnnoMate/AppComponents/PhylogicNDTComponents.py`

 * *Files 0% similar despite different names*

```diff
@@ -749,15 +749,15 @@
         row_titles=[i for i in mut_counts_df_mod['type'].unique()]
     )
     for i, annotations in enumerate(zip(['non-coding', 'synonymous'], ['coding', 'non-synonymous'])):
         for j, clust in enumerate(mut_counts_df_mod[maf_cluster_col].unique()):
             filterby_annotation_df = mut_counts_df_mod[mut_counts_df_mod['annotation'].isin(annotations)]
             filterby_cluster_df = filterby_annotation_df[filterby_annotation_df[maf_cluster_col] == clust]
             filterby_cluster_df.set_index('annotation', inplace=True)
-            print(filterby_cluster_df)
+
             fig.add_trace(go.Pie(
                 values=filterby_cluster_df['count'],
                 domain=dict(x=[i/num_clusters, (i+1)/num_clusters]),
                 labels=filterby_cluster_df['count'].index,
                 legendgroup=i,
                 textinfo='value',
             ), row=(i+1), col=(j+1))
```

### Comparing `AnnoMate-0.0.3/AnnoMate/AppComponents/utils.py` & `annomate-1.0.0/AnnoMate/AppComponents/utils.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/Data.py` & `annomate-1.0.0/AnnoMate/Data.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/DataTypes/GenericData.py` & `annomate-1.0.0/AnnoMate/DataTypes/GenericData.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/DataTypes/PatientSampleData.py` & `annomate-1.0.0/AnnoMate/DataTypes/PatientSampleData.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate/ReviewDataApp.py` & `annomate-1.0.0/AnnoMate/ReviewDataApp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from datetime import datetime
 import pandas as pd
 import numpy as np
 # from jupyter_dash import JupyterDash
 from dash import jupyter_dash
-from dash import dcc
+from dash import dcc, ctx
 from dash import html, Dash
 from dash.dependencies import Input, Output, State
 from dash.exceptions import PreventUpdate
 import dash
 import dash_bootstrap_components as dbc
 import inspect
 from collections import OrderedDict
@@ -291,15 +292,17 @@
                 autofill_dict,
                 review_data_table_df=review_data_table_df,
                 review_data_table_page_size=review_data_table_page_size,
                 collapsable=collapsable,
                 multi_type_columns=multi_type_columns
             )
         
-        app.title = review_data.data_pkl_fn.split('/')[-1].split('.')[0]
+        # data_pkl_fn = data_path/data.pkl where data_path is the path to data that is set in set_review_data
+        # e.g. if data_path = './reviewer_data' then data_pkl_fn = './reviewer_data/data.pkl' and app.title = 'reviewer_data'
+        app.title = review_data.data_pkl_fn.split('/')[-2] 
 
         if auto_export:
             if auto_export_path is None:
                 auto_export_path = f"{review_data.data_pkl_fn.rsplit('.', 1)[0]}.auto_export"
                 print(f'Setting auto_export_path to {auto_export_path}')
             if not os.path.exists(auto_export_path):
                 print(f'Making directory {auto_export_path} for auto exporting.')
@@ -371,15 +374,84 @@
                         (annot_app_display_types_dict[annot_name].default_display_value is not None)
                     ):
                         current_annotations[annot_name] = annot_app_display_types_dict[annot_name].default_display_value
                     
                 output_dict['annot_panel'] = current_annotations
             return output_dict
 
-        ####### Callbacks
+        ###### Callbacks
+        @app.callback(
+            output=dict(
+                is_open=Output('APP-freeze-modal', 'is_open')
+            ),
+            inputs=dict(
+                freeze_button=Input('APP-freeze-button', 'n_clicks'),
+                freeze_close=Input('APP-freeze-close', 'n_clicks'),
+                freeze_confirm=Input('APP-freeze-confirm', 'n_clicks')
+            ),
+            prevent_initial_call=True,
+        )
+        def toggle_freeze_modal(freeze_button, freeze_close, freeze_confirm):
+            if ctx.triggered_id=='APP-freeze-button':
+                return {'is_open': True}
+            return {'is_open': False}
+        
+        @app.callback(
+            output=dict(
+                subscript=Output('APP-title-subscript', 'children'),
+                subscript_color=Output('APP-title-subscript', 'style'),
+                button=Output('APP-freeze-button', 'children'),
+                history_display_table=Output('APP-history-table', 'data', allow_duplicate=True),
+                dropdown_options=Output('APP-dropdown-data-state', 'options', allow_duplicate=True),
+                annot_panel=annotation_panel_component.callback_output
+            ),
+            inputs=dict(
+                freeze_confirm=Input('APP-freeze-confirm', 'n_clicks'),
+                annotations_confirm=State('APP-annotations-checkbox', 'value'),
+                history_display_table=State('APP-history-table', 'data'),
+                dropdown_options=State('APP-dropdown-data-state', 'options'),
+                annot_panel=annotation_panel_component.callback_state 
+            ),
+            prevent_initial_call=True,
+        )
+        def freeze_data(freeze_confirm, annotations_confirm, history_display_table, dropdown_options, annot_panel):
+            subscript = '  TEST MODE'
+            subscript_color = {'color': 'red'}
+            button = dbc.Button('Freeze Data', id='APP-freeze-button')
+
+            if freeze_confirm:
+                if not annotations_confirm:
+                    # remove data
+                    annot_cols = review_data.data.annot_df.columns.tolist()
+                    review_data.data.annot_df = pd.DataFrame(index=review_data.data.index, columns=annot_cols)
+                    review_data.data.history_df = pd.DataFrame(columns=['index', 'timestamp', 'source_data_fn']+annot_cols)
+                    review_data.save_data()
+
+                    # removed displayed data
+                    history_display_table = pd.DataFrame().to_dict('records')
+                    reviewed_data_df['label'] = reviewed_data_df.index
+                    dropdown_options = reviewed_data_df.reset_index().to_dict('records')
+                    annot_panel = {annot_name: '' for annot_name in annot_app_display_types_dict.keys()}
+                    
+                review_data.mh.set_attribute('freeze_data', True)
+                review_data.mh.set_attribute('freeze_data_timestamp', datetime.now().strftime("%Y-%m-%d %H:%M:%S"))
+
+            if review_data.mh.metadata['freeze_data']:
+                subscript = f'  Frozen at {review_data.mh.metadata["freeze_data_timestamp"]}'
+                subscript_color = {'color': 'black'}
+                button = html.Div([])
+
+            return {
+                'subscript': subscript, 
+                'subscript_color': subscript_color, 
+                'button': button, 
+                'history_display_table': history_display_table,
+                'dropdown_options': dropdown_options, 
+                'annot_panel': annot_panel
+            }
 
         @app.callback(
             output=dict(
                 more_component_outputs=more_component_outputs,
                 history_table=Output('APP-history-table', 'data', allow_duplicate=True),
                 history_table_selected_row_state=Output('APP-history-table', 'selected_rows', allow_duplicate=True),
                 annot_panel=annotation_panel_component.callback_output,
@@ -464,15 +536,16 @@
             return output_dict
             
 
         @app.callback(
             output=dict(
                 history_table=Output('APP-history-table', 'data', allow_duplicate=True),
                 dropdown_list_options=Output('APP-dropdown-data-state', 'options', allow_duplicate=True),
-                review_data_table_data=Output('APP-review-data-table', 'data', allow_duplicate=True)
+                review_data_table_data=Output('APP-review-data-table', 'data', allow_duplicate=True),
+                test_mode_alert=Output('APP-test-mode-alert', 'is_open')
             ),
             inputs=dict(
                 submit_annot_button=Input('APP-submit-button-state', 'n_clicks'),
                 annot_input_state=annotation_panel_component.callback_state,
                 dropdown_value=State('APP-dropdown-data-state', 'value'),
                 review_data_table_state=State('APP-review-data-table', 'data'),
             ),
@@ -483,15 +556,17 @@
             annot_input_state,
             dropdown_value,
             review_data_table_state
         ):
             """
             Save current annotations to the annot_df field, and update the dropdown menu timestamp and history table
             """
-            output_dict = {'review_data_table_data': dash.no_update}
+            output_dict = {'review_data_table_data': dash.no_update, 'test_mode_alert': False}
+            if not review_data.mh.metadata['freeze_data']:
+                output_dict['test_mode_alert'] = True
             for annot_name in annot_app_display_types_dict.keys():
                 annot_type = review_data.data.annot_col_config_dict[annot_name]
                 # Convert type
                 if annot_app_display_types_dict[annot_name].display_output_format is not None:
                     annot_input_state[annot_name] = annot_app_display_types_dict[annot_name].display_output_format(
                         annot_input_state[annot_name]
                     )
@@ -654,14 +729,19 @@
                             dropdown_value,
                             *more_component_inputs[component.name]
                         )
 
                         validate_callback_outputs(component_output, component, which_callback='internal_callback')
                         output_dict['more_component_outputs'][component.name] = component_output
             return output_dict
+        
+        if not review_data.mh.metadata['freeze_data']:
+            warnings.warn(
+                'You are in test mode. Your data will not be saved.'
+            )
 
         jupyter_dash.default_mode = mode
         app.run(host=host, port=port, debug=True)
         
     def gen_layout(
         self,
         review_data: ReviewDataInterface,
@@ -672,15 +752,30 @@
         review_data_table_page_size: int = 10,
         collapsable=True,
         multi_type_columns=[]
     ):
         """
         Generate layout of the dashboard
         """
-        review_data_title = html.Div([html.H1(review_data.data_pkl_fn.split('/')[-1].split('.')[0])])
+        review_data_title = html.Div([
+            dbc.Alert('This is a test mode. You must freeze your data to save your annotations.', color='danger', id='APP-test-mode-alert', is_open=False, duration=4000),
+            html.H1(review_data.data_pkl_fn.split('/')[-2], style={'display': 'inline'}),
+            dbc.Modal([
+                dbc.ModalHeader("Are you sure you want to freeze the data?"),
+                dbc.ModalBody("Input data will not be changable once data is frozen."),
+                html.Div([
+                    dbc.Checkbox(id='APP-annotations-checkbox', label='Save current annotations', value=True)
+                ], style={'margin-left': '15px'}),
+                dbc.ModalFooter([
+                    dbc.Button("Freeze data", id="APP-freeze-confirm", n_clicks=0, className="ml-auto"),
+                    dbc.Button("Cancel, I am still testing", id="APP-freeze-close", n_clicks=0, className="ml-auto")
+                ]),
+            ], id="APP-freeze-modal"),
+            html.Div(children=html.Button('Freeze data') if not review_data.mh.metadata['freeze_data'] else html.Div([]), id='APP-freeze-button')
+        ])
         review_data_path = html.Div([html.P(f'Path: {review_data.data_pkl_fn}')])
         review_data_description = html.Div([html.P(f'Description: {review_data.data.description}')])
         dropdown = html.Div(dcc.Dropdown(options=reviewed_data_df.reset_index().to_dict('records'),
                                          value=None, 
                                          id='APP-dropdown-data-state'))
         
         dropdown_component = AppComponent(name='APP-dropdown-component',
@@ -912,18 +1007,30 @@
 
         if len(annot_app_display_types_dict) == 0:
             raise ValueError(
                 f'annot_app_display_types_dict is empty. '
                 f'Make sure to run reviewer.set_default_review_data_annotations_configuration(), '
                 f'or manually set up your annotations'
             )
-        submit_annot_button = html.Button(id='APP-submit-button-state', 
-                                          n_clicks=0, 
-                                          children='Submit', 
-                                          style={"marginBottom": "15px"})
+        submit_annot_button = html.Div([
+            html.Button(id='APP-submit-button-state', 
+                n_clicks=0, 
+                children='Submit', 
+                style={"marginBottom": "15px"}
+            ),
+            html.Sub(
+                '  TEST MODE', 
+                style={'color': 'red'}, 
+                id='APP-title-subscript'
+            ) if not review_data.mh.metadata['freeze_data'] else html.Sub(
+                f'  Frozen at {review_data.mh.metadata["freeze_data_timestamp"]}', 
+                style={'color': 'black'}, 
+                id='APP-title-subscript'
+            ),
+        ])
         
         def annotation_display_component_input(annot_name, annot, annot_app_display_type):
             input_component_id = f"APP-{annot_name}-{annot_app_display_type}-input-state"
             
             input_component = annot_app_display_type.gen_input_component(
                 annot, 
                 component_id=input_component_id,
```

### Comparing `AnnoMate-0.0.3/AnnoMate/ReviewDataInterface.py` & `annomate-1.0.0/AnnoMate/ReviewDataInterface.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import os
 import numpy as np
 import warnings
 import pickle
 from pathlib import Path
 from typing import List, Dict, Union
 from AnnoMate.Data import Data, DataAnnotation, validate_annot_data
+from AnnoMate.MetadataHandler import MetadataHandler
 
 
 class ReviewDataInterface:
     
     def __init__(self,
                  data_pkl_fn: Union[str, Path],
-                 data: Data):
+                 data: Data,
+                 mh: MetadataHandler,):
         """
         Object that saves, loads, and edits Data objects
 
         Parameters
         ----------
         data_pkl_fn: Union[str, Path]
             pickle file to save/load data object from
@@ -27,15 +29,16 @@
         Notes
         -----
 
         If data_pkl_fn already exists, it will only load that file and ignore whatever the parameter data is.
         This is to prevent accidentally overwriting annotations and the data being currently reviewed.
         """
         self.data_pkl_fn = data_pkl_fn
-        if os.path.exists(data_pkl_fn):
+        self.mh = mh
+        if os.path.exists(data_pkl_fn) and mh.metadata['freeze_data']:
             f = open(data_pkl_fn, 'rb')
             self.data = pickle.load(f)
             f.close()
             warnings.warn(f"Loading existing data pkl file")
         else:
             self.data = data
```

### Comparing `AnnoMate-0.0.3/AnnoMate/ReviewerTemplate.py` & `annomate-1.0.0/AnnoMate/ReviewerTemplate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .ReviewDataInterface import ReviewDataInterface, DataAnnotation, Data
 from .Data import validate_annot_data
 from .ReviewDataApp import ReviewDataApp, valid_annotation_app_display_types, AnnotationDisplayComponent
 from AnnoMate.AnnotationDisplayComponent import *
+from AnnoMate.MetadataHandler import MetadataHandler
 import pandas as pd
 import os
 from dash.dependencies import State
 from typing import Union, Dict, List
 from pathlib import Path
 from abc import ABC, abstractmethod
 import pathlib
@@ -126,28 +127,29 @@
         Call self.add_autofill() to set custom autofill options
 
         """
         pass
     
     # Public methods
     def set_review_data(self,
-                        data_pkl_fn: pathlib.Path,
+                        data_path: pathlib.Path,
                         description: str = None,
                         annot_df: pd.DataFrame = None,
                         annot_col_config_dict: pd.DataFrame = None,
                         history_df: pd.DataFrame = None,
                         load_existing_data_pkl_fn: Union[str, pathlib.Path] = None,
                         load_existing_exported_data_dir: Union[str, pathlib.Path] = None,
                         **kwargs):
         """Sets the review session ReviewData Object.
 
         Parameters
         ----------
-        data_pkl_fn : Union[str, Path]
-            path to pickle file to save data for current review session
+        data_path : Union[str, Path]
+            path to a directory where data pickle file and metadata 
+            config file will be saved for current review session
 
         description : str,
             description of the data being reviewed
 
         annot_df : pd.DataFrame, optional
             dataframe of annotations from previous review sessions.
 
@@ -165,15 +167,27 @@
             tables from a previous review session's data object
 
         **kwargs: dict
                   See additional parameters from self.gen_data() below
 
         """
 
-        if os.path.exists(data_pkl_fn):
+        data_pkl_fn = f'{data_path}/data.pkl'
+        metadata_config_fn = f'{data_path}/metadata_config.yaml'
+
+        if not os.path.exists(data_path):
+            os.makedirs(data_path)
+        if not os.path.exists(metadata_config_fn) or not os.path.exists(data_pkl_fn):
+            mh = MetadataHandler(metadata_config_fn, overwrite=True)
+            mh.set_attribute('freeze_data', False)
+            # can also add future defaults here 
+        else:
+            mh = MetadataHandler(metadata_config_fn)
+
+        if os.path.exists(data_pkl_fn) and mh.metadata['freeze_data']:
             f = open(data_pkl_fn, 'rb')
             data = pickle.load(f)
         else:
             if description is None:
                 raise ValueError(f'description is None. Provide a description if you are setting a new data object.')
             if (load_existing_data_pkl_fn is not None) and \
                     os.path.exists(load_existing_data_pkl_fn):
@@ -216,14 +230,15 @@
                 history_df=history_df,
                 **kwargs
             )
 
         self.review_data_interface = ReviewDataInterface(
             data_pkl_fn=data_pkl_fn,
             data=data,
+            mh=mh
         )
 
     def set_default_review_data_annotations_configuration(self):
         """
         Sets preconfigured annotation columns and display settings
 
         Notes
@@ -454,17 +469,27 @@
     def get_data_attribute(self, attribute: str):
         return getattr(self.review_data_interface.data, attribute)
 
     def list_data_attributes(self):
         return vars(self.review_data_interface.data).keys()
 
     def get_annot(self):
+        if not self.review_data_interface.mh.metadata['freeze_data']:
+            warnings.warn(
+                'Data is not frozen. Annotations will not be saved. '
+                'Please freeze data in the dashboard to save annotations.'
+            )
         return self.get_data_attribute('annot_df')
 
     def get_history(self):
+        if not self.review_data_interface.mh.metadata['freeze_data']:
+            warnings.warn(
+                'Data is not frozen. History will not be saved. '
+                'Please freeze data in the dashboard to save history.'
+            )
         return self.get_data_attribute('history_df')
     
     def export_data(self, path: Union[str, Path], export_by_day=False, dry_run=True, **kwargs):
         """
         Export annotation and history tables to tsv files
         
         Parameters
```

### Comparing `AnnoMate-0.0.3/AnnoMate/Reviewers/ExampleReviewer.py` & `annomate-1.0.0/AnnoMate/Reviewers/ExampleReviewer.py`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/AnnoMate.egg-info/PKG-INFO` & `annomate-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: AnnoMate
-Version: 0.0.3
-Summary: A general tool to create dashboards for manual review
-Home-page: https://github.com/getzlab/AnnoMate
-Author: Claudia Chu
-Author-email: cchu@broadinstitute.org
-Project-URL: Bug Tracker, https://github.com/getzlab/AnnoMate/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # AnnoMate
 
 A package for using and creating interactive dashboards for manual review.
 
 ![Purity AnnoMate Reviewer](https://github.com/getzlab/AnnoMate/blob/master/images/ezgif.com-gif-maker.gif)
 
 # Quick Start
@@ -117,7 +102,29 @@
 Most ACBs use jupyter notebooks for their analysis. So why not keep the review process in jupyter notebooks too? Additionally, there already exist great tools for making interactive figures and dashboards. We can use these packages to help automatically consildate information and create figures that will make it easier to review, enforce annotation standards, and track changes over time.
 
 The `AnnoMate` package makes it simple to create dashboards for reviewing data. Developers and users can easily customize their dashboards to incorpate any data they like, and automatically provides a reviewer an easy way to annotate their data, track changes, and share their annotations with others.
 
 ### Get Started
 
 See `tutorial_notebooks/` for documentation and tutorials.
+
+# For AnnoMate Developers
+
+New features to AnnoMate are pushed to `dev_branch`. Any separate large features being developed simultaneously can be done in separate branches, and merged to `dev_branch` first. 
+
+Only when we merge the `dev_branch` to master, we also push to pypi. At this time we decide the new version number.
+
+Semantic versioning (https://packaging.python.org/en/latest/discussions/versioning/)
+The idea of semantic versioning (or SemVer) is to use 3-part version numbers, major.minor.patch, where the project author increments:
+- major when they make incompatible API changes,
+- minor when they add functionality in a backwards-compatible manner, and
+- patch, when they make backwards-compatible bug fixes.
+
+For AnnoMate:
+- Major: Not backwards compatible
+- Minor: up to 3 functionality changes with backwards compatibility within a year
+    - pickle versioning in reviewdatainterface
+    - hot keys
+    - Adding components or new custom pre-built reviewers 
+- Patch: up to 5 bug fixes within 6 months
+
+Github continuous integration: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
```

### Comparing `AnnoMate-0.0.3/AnnoMate.egg-info/SOURCES.txt` & `annomate-1.0.0/AnnoMate.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./AnnoMate/AnnotationDisplayComponent.py
 ./AnnoMate/Data.py
+./AnnoMate/MetadataHandler.py
 ./AnnoMate/ReviewDataApp.py
 ./AnnoMate/ReviewDataInterface.py
 ./AnnoMate/ReviewerTemplate.py
 ./AnnoMate/__init__.py
 ./AnnoMate/AnnotationDisplayComponents/__init__.py
 ./AnnoMate/AppComponents/CNVPlotComponent.py
 ./AnnoMate/AppComponents/DataTableComponents.py
@@ -21,8 +22,9 @@
 ./AnnoMate/DataTypes/__init__.py
 ./AnnoMate/Reviewers/ExampleReviewer.py
 ./AnnoMate/Reviewers/__init__.py
 AnnoMate.egg-info/PKG-INFO
 AnnoMate.egg-info/SOURCES.txt
 AnnoMate.egg-info/dependency_links.txt
 AnnoMate.egg-info/requires.txt
-AnnoMate.egg-info/top_level.txt
+AnnoMate.egg-info/top_level.txt
+tests/test_example_reviewer.py
```

### Comparing `AnnoMate-0.0.3/LICENSE.txt` & `annomate-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `AnnoMate-0.0.3/PKG-INFO` & `annomate-1.0.0/AnnoMate.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,45 @@
 Metadata-Version: 2.1
 Name: AnnoMate
-Version: 0.0.3
+Version: 1.0.0
 Summary: A general tool to create dashboards for manual review
 Home-page: https://github.com/getzlab/AnnoMate
 Author: Claudia Chu
 Author-email: cchu@broadinstitute.org
 Project-URL: Bug Tracker, https://github.com/getzlab/AnnoMate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: cnv-suite
+Requires-Dist: dash>=2.11.0
+Requires-Dist: dash-bootstrap-components
+Requires-Dist: dash-cytoscape
+Requires-Dist: dash-daq
+Requires-Dist: fsspec
+Requires-Dist: gcsfs
+Requires-Dist: google-auth
+Requires-Dist: google-api-core
+Requires-Dist: hound
+Requires-Dist: ipykernel
+Requires-Dist: ipython
+Requires-Dist: jupyterlab>=4.0.2
+Requires-Dist: matplotlib
+Requires-Dist: pandas
+Requires-Dist: pickleshare
+Requires-Dist: pillow
+Requires-Dist: pip
+Requires-Dist: plotly>=5.15.0
+Requires-Dist: scipy
+Requires-Dist: setuptools
+Requires-Dist: frozendict
+Requires-Dist: flask>=3.0.3
+Requires-Dist: werkzeug>=2.3.3
 
 # AnnoMate
 
 A package for using and creating interactive dashboards for manual review.
 
 ![Purity AnnoMate Reviewer](https://github.com/getzlab/AnnoMate/blob/master/images/ezgif.com-gif-maker.gif)
 
@@ -117,7 +141,29 @@
 Most ACBs use jupyter notebooks for their analysis. So why not keep the review process in jupyter notebooks too? Additionally, there already exist great tools for making interactive figures and dashboards. We can use these packages to help automatically consildate information and create figures that will make it easier to review, enforce annotation standards, and track changes over time.
 
 The `AnnoMate` package makes it simple to create dashboards for reviewing data. Developers and users can easily customize their dashboards to incorpate any data they like, and automatically provides a reviewer an easy way to annotate their data, track changes, and share their annotations with others.
 
 ### Get Started
 
 See `tutorial_notebooks/` for documentation and tutorials.
+
+# For AnnoMate Developers
+
+New features to AnnoMate are pushed to `dev_branch`. Any separate large features being developed simultaneously can be done in separate branches, and merged to `dev_branch` first. 
+
+Only when we merge the `dev_branch` to master, we also push to pypi. At this time we decide the new version number.
+
+Semantic versioning (https://packaging.python.org/en/latest/discussions/versioning/)
+The idea of semantic versioning (or SemVer) is to use 3-part version numbers, major.minor.patch, where the project author increments:
+- major when they make incompatible API changes,
+- minor when they add functionality in a backwards-compatible manner, and
+- patch, when they make backwards-compatible bug fixes.
+
+For AnnoMate:
+- Major: Not backwards compatible
+- Minor: up to 3 functionality changes with backwards compatibility within a year
+    - pickle versioning in reviewdatainterface
+    - hot keys
+    - Adding components or new custom pre-built reviewers 
+- Patch: up to 5 bug fixes within 6 months
+
+Github continuous integration: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
```

### Comparing `AnnoMate-0.0.3/setup.py` & `annomate-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AnnoMate",
-    version="0.0.3",
+    version="1.0.0",
     author="Claudia Chu",
     author_email="cchu@broadinstitute.org",
     description="A general tool to create dashboards for manual review",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/getzlab/AnnoMate",
     project_urls={
@@ -18,15 +18,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "."},
     packages=setuptools.find_packages(where=".", exclude=['zeption.examples', '']),
-    python_requires=">=3.6",
+    python_requires=">=3.8", # last tested version: 3.9
     install_requires = ['cnv-suite',
                         'dash>=2.11.0',
                         'dash-bootstrap-components',
                         'dash-cytoscape',
                         'dash-daq',
                         'fsspec',
                         'gcsfs',
@@ -42,12 +42,12 @@
                         'pillow',
                         'pip',
                         'plotly>=5.15.0',
                         'scipy',
                         'setuptools',
                         'frozendict',
                         # fixes jupyter-dash bug when repeat calls to run_server hangs
-                        # see: https://github.com/plotly/jupyter-dash/issues/103
-                        'flask<=2.2.1',
-                        'werkzeug<=2.2.1']
+                        'flask>=3.0.3',
+                        'werkzeug>=2.3.3', # security vulnerability with 2.2.2
+                       ]
 )
```

