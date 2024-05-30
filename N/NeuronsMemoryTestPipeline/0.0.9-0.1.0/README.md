# Comparing `tmp/neuronsmemorytestpipeline-0.0.9.tar.gz` & `tmp/neuronsmemorytestpipeline-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuronsmemorytestpipeline-0.0.9.tar", max compression
+gzip compressed data, was "neuronsmemorytestpipeline-0.1.0.tar", max compression
```

## Comparing `neuronsmemorytestpipeline-0.0.9.tar` & `neuronsmemorytestpipeline-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1073 2024-03-18 10:43:12.257440 neuronsmemorytestpipeline-0.0.9/LICENSE
--rw-r--r--   0        0        0     1115 2024-03-19 13:13:11.252224 neuronsmemorytestpipeline-0.0.9/README.md
--rw-r--r--   0        0        0      908 2024-03-22 12:35:51.567866 neuronsmemorytestpipeline-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    15955 2024-03-18 12:58:02.824909 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/FRT_metric.py
--rw-r--r--   0        0        0     5058 2024-03-21 10:02:05.037136 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py
--rw-r--r--   0        0        0    15564 2024-03-20 10:29:23.298502 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_recognition_metric.py
--rw-r--r--   0        0        0     5713 2024-03-18 12:58:02.829954 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_text_processing.py
--rw-r--r--   0        0        0     3496 2024-03-18 12:58:02.833281 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/QA_modules.py
--rw-r--r--   0        0        0        0 2024-03-19 13:56:49.945585 neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/__init__.py
--rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 neuronsmemorytestpipeline-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-18 10:43:12.257440 neuronsmemorytestpipeline-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1115 2024-03-19 13:13:11.252224 neuronsmemorytestpipeline-0.1.0/README.md
+-rw-r--r--   0        0        0      908 2024-05-30 08:52:42.980664 neuronsmemorytestpipeline-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    16417 2024-04-23 15:34:57.928061 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/FRT_metric.py
+-rw-r--r--   0        0        0     5294 2024-05-30 08:47:41.735336 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py
+-rw-r--r--   0        0        0    18027 2024-05-30 08:46:24.947788 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/MRT_recognition_metric.py
+-rw-r--r--   0        0        0     8806 2024-05-30 08:47:59.754851 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/MRT_text_processing.py
+-rw-r--r--   0        0        0     3496 2024-03-18 12:58:02.833281 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/QA_modules.py
+-rw-r--r--   0        0        0        0 2024-03-19 13:56:49.945585 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-07 09:54:55.761697 neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/constants.py
+-rw-r--r--   0        0        0     2196 1970-01-01 00:00:00.000000 neuronsmemorytestpipeline-0.1.0/PKG-INFO
```

### Comparing `neuronsmemorytestpipeline-0.0.9/LICENSE` & `neuronsmemorytestpipeline-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.9/README.md` & `neuronsmemorytestpipeline-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.9/pyproject.toml` & `neuronsmemorytestpipeline-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "NeuronsMemoryTestPipeline"
-version = "0.0.9"
+version = "0.1.0"
 description = "Package provides QA, MRT and FRT metrics calculation for frt and mrt scores."
 authors = [
     "Irina White <i.white@neuronsinc.com>",
     "Theo Sell <t.sell@neuronsinc.com>"
 ]
 license = "MIT"
 homepage = "https://gitlab.com/neurons-inc1/data-analyst/neurons_metrics_package"
```

### Comparing `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/FRT_metric.py` & `neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/FRT_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,19 @@
     """
     age_demographics = df[['group_id','Age']].drop_duplicates()
     age_demographics= age_demographics.groupby(['group_id'], observed=False)['Age'].agg(['min', 'max', 'mean', 'std']).reset_index()
     age_demographics.rename(columns={'group_id': 'group_id Age'}, inplace=True)
     age_demographics.set_index('group_id Age', inplace=True)
     print(f'AGE Statistics: \n {age_demographics}')
 
+    age_group_count = df[['group_id','Age_Group','participant_id']].drop_duplicates()
+    age_group_count= age_group_count.groupby(['group_id', 'Age_Group'], observed=False)['participant_id'].agg(['count']).reset_index()
     age_group_split = df[['group_id','Age_Group','Age']].drop_duplicates()
-    age_group_split= age_group_split.groupby(['group_id', 'Age_Group'], observed=False)['Age'].agg(['count', 'min', 'max', 'mean', 'std'])
+    age_group_split= age_group_split.groupby(['group_id', 'Age_Group'], observed=False)['Age'].agg(['min', 'max', 'mean', 'std']).reset_index()
+    age_group_split = age_group_split.merge(age_group_count, on=['group_id','Age_Group'], how='left')
     print(f'\nAGE GROUP Statistics: \n {age_group_split}')
 
     df['total_participants'] = df.groupby('group_id')['participant_id'].transform('nunique')
     gender_demographics = df[['group_id', 'Gender', 'participant_id', 'total_participants']].drop_duplicates()
     gender_demographics= gender_demographics.groupby(['group_id', 'Gender', 'total_participants'], observed=False)['participant_id'].agg(['count']).reset_index()
     gender_demographics['percentage'] = np.round(100 * gender_demographics['count']/gender_demographics['total_participants'], 2)
     gender_demographics.reset_index(drop = True, inplace=True)
@@ -144,18 +147,19 @@
         df (dataframe): working dataframe
         group_columns (list, optional): grouping parameter. Defaults to ['frt_stimulus', 'frt_association', 'module_name', 'group_id'].
     Returns:
         dataframe: updated with the new column positive_negative
     """
     grouped = df.groupby(group_columns)['frt_response'].value_counts().reset_index(name="positive_negative")
     pivot = grouped.pivot_table(index=['frt_association', 'module_name'], columns='frt_response', values="positive_negative").reset_index()
+    pivot['Yes'] = 0 if 'Yes' not in pivot.columns else pivot['Yes']
+    pivot['No'] = 0 if 'No' not in pivot.columns else pivot['No']
     pivot["positive_negative"]=np.where(pivot['Yes']>pivot["No"],"Positive", "Negative")
     return (pivot)
 
-
 def calculate_certainty_formula(row, group_columns, iqr_col):
     """ Calculation of the certainty on the group_columns level, using incoded formula.
     Args:
         row (str or int):row of the dataframe to use for calculation
         group_columns (list): list of the name of the columns use for grouping
         iqr_col (str): name of the column use for calculation of the certianty (mainly group_iqr_yes or group_iqr_no)
     Returns:
```

### Comparing `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py` & `neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/MRT_free_recall_metric.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,99 @@
-
+#%%
 import pandas as pd
+pd.options.display.show_dimensions = False
 import numpy as np
 from neuronsmemorytestpipeline import MRT_text_processing
 
-def process_recall(df, filter_task, model, group=['group_id']):
+def alias_group_define(df):
+    """obtain all group values, split them and create a new column for each group_id
+    Args:
+        df (_type_): the alias dataframe
+    Returns:
+        _type_: updated dataframe with new group_id column
+    """
+    df.group_id = df.group_id.astype(str)
+    new_rows = []
+    for _, row in df.iterrows():
+        groups = row['group_id'].split(',')
+        for group in groups:
+            new_row = row.copy()
+            new_row['group_id_new'] = group
+            new_rows.append(new_row)
+
+    # Concatenate the new rows with the original DataFrame
+    new_df = pd.concat([df, pd.DataFrame(new_rows)], ignore_index=True)
+    new_df['group_id'] = new_df['group_id_new']
+    new_df.drop('group_id_new', axis=1, inplace=True)
+    new_df.dropna(subset=['group_id'], inplace=True)
+    new_df.drop_duplicates(inplace=True)
+    new_df = new_df.sort_values('group_id').reset_index(drop=True)
+    return new_df
+
+def process_recall(df, filter_task, model, alias_df, group=['group_id']):
     """ Prepares the data, process it using text cleaning module, calculates free recall scores per group, including average position and average recall %.
     Args:
         df: dataframe with data from Jatos and identified MRT module plus task_name
         group (list): group by list that provides filter for grouping dataset
     Returns:
         df: updated data frame with the score column
     """
 
-    df = df.copy()
+    df = df.loc[(df['task_name'] == filter_task) & (df['trial_name'].str.startswith('R-'))].copy()
+    df['position'] = df['trial_name'].apply(lambda x: int(x.split('-')[-1]))
     df_cleaned = pd.DataFrame()
     corrected_entries = pd.DataFrame()
-    original_corrected = pd.DataFrame()
-    not_mentioned = pd.DataFrame()
+
+    
     for group in sorted(df.group_id.unique().tolist(), reverse=False):
         print(f'\n\n *** Group ID: {group} ***')
         df_group = df[df.group_id == group].copy()
+        target_brands = alias_df[alias_df['group_id'] == group]['mrt_stimulus'].dropna().unique().tolist()
 
-        #preparing the list of brand used as template for aitext
-        mask = (df_group['expected_response'].str.endswith(('Video', 'Image')) | df_group['expected_response'].notna())
-        total_stimulus = df_group[mask]['expected_response'].dropna().unique().tolist()
-        mask = ~(df['expected_response'].str.endswith(('Video', 'Image')) | df['expected_response'].isna())
-        target_brands = df_group.loc[mask, 'expected_response'].dropna().unique().tolist()
         print(f'\nBRANDS used in the project for group {group}:')
         for brand in sorted(target_brands):
             print('  ', brand)
-
-        #preparing the list of responses and dataframe for processing 
-        df_group = df_group.loc[(df_group['task_name'] == filter_task) & (df_group['trial_name'].str.startswith('R-'))]
-        responses_to_clean = df_group.given_response_label_presented.dropna().unique().tolist()
-        df_group, corrected_counts, corrected_df = MRT_text_processing.clean_free_recall(df_group, target_brands, responses_to_clean, model)
-    
+        
+        total_responses = len(df_group.given_response_label_presented.dropna())
+        print('*'*50)
+        print(f'\nThere are {total_responses} entries in total.\n')
+        print('Identified prior to adjustment: \n', df_group[df_group.given_response_label_presented.isin(target_brands)].given_response_label_presented.value_counts())
+        df_group_tocorrect = df_group[~df_group.given_response_label_presented.isin(target_brands)].copy()
+        df_group_tocorrect = df_group_tocorrect.dropna(subset=['given_response_label_presented'])
+        df_group = df_group[df_group['given_response_label_presented'].isin(target_brands) | pd.isna(df_group['given_response_label_presented'])].copy()
+        df_group['corrected'] = df_group['given_response_label_presented']
+        df_group['method'] = 'original'
+        responses_to_clean = df_group_tocorrect.given_response_label_presented.dropna().unique().tolist()
+        print(f'\nThere are {len(responses_to_clean)} entries to clean further.')
+        
+        corrected_df = MRT_text_processing.clean_free_recall(df_group_tocorrect, target_brands, responses_to_clean, model)
+        df_group = pd.concat([df_group, corrected_df], axis=0, ignore_index=True)
         corrected_df['group_id'] = group
+        corrected_entries =  corrected_df[['group_id', 'given_response_label_presented', 'corrected', 'method']].copy()
+        corrected_entries = corrected_entries[corrected_entries['method'] != 'not_match']
+        corrected_entries = corrected_entries.sort_values('method', ascending=True).reset_index(drop=True)
+        not_match = corrected_df[corrected_df['method'] == 'not_match']
+        
+    print('*'*50)
+    return df_group, corrected_entries, not_match
 
-        corrected_entries = pd.concat([corrected_entries, corrected_counts], axis=0, ignore_index=True)
-        original_corrected = pd.concat([original_corrected, corrected_df], axis=0, ignore_index=True)
-
-        #score calculation
-        df_group['position'] = df_group['trial_name'].apply(lambda x: int(x.split('-')[-1]))
-        df_group = df_group[df_group.recalled_brand.isin(target_brands)]
-        df_cleaned = pd.concat([df_cleaned, df_group], axis=0, ignore_index=True)
-        not_there = pd.DataFrame({'recalled_brand': list(set(target_brands) - set(original_corrected['corrected'].unique()))})
-        not_there['group_id'] = group
-        not_mentioned = pd.concat([not_mentioned, not_there], axis=0, ignore_index=True)
-    original_corrected = original_corrected.sort_values(['group_id', 'method', 'original']).reset_index(drop = True)
-    return df_cleaned, corrected_entries, original_corrected, not_mentioned
-
-def compute_scores(df_given: pd.DataFrame, no_recall: pd.DataFrame, group = ['group_id', 'project_identifier', 'task_name', 'recalled_brand','total_participants']):
+def compute_scores(df_given: pd.DataFrame, group = ['group_id', 'project_identifier', 'task_name', 'corrected','total_participants']):
     """ Calculates: Average % , Average position, Average Log score based on position
     Args:
         df (dataframe): processed data frame with cleaned text
         no_recall (dataframe): dataset with brands that were not mentioned
     Returns:
         dataframe: updated dataframe with the scores columns
     """
     df = df_given.copy()
+    df['corrected'] = df['corrected'].fillna(df['given_response_label_presented'])
     df['position_mean'] = df.groupby(group, observed=False)['position'].transform('mean')
     df['brand_count'] = df.groupby(group, observed=False)['position'].transform('count')
     df['recall_%'] = df['brand_count'] / df['total_participants'] * 100
-    
-    df['mrt_score_freerecall'] = df.apply(lambda row: (1 / (np.log(row['position'] + 1))) * (row['recall_%']), axis=1)
-    df = df[group + ['brand_count', 'position_mean', 'recall_%', 'mrt_score_freerecall']].copy()
-
-    pivot_df = df.pivot_table(index=group, values='mrt_score_freerecall', aggfunc='mean', observed=False).reset_index()
-    df = df.merge(pivot_df, on=group, suffixes=('_single', ''))
-    df.drop('mrt_score_freerecall_single', axis = 1, inplace = True)
-    df = np.round(df, 2)
-    df = df.drop_duplicates().copy()
-
-    columns_to_fill_zeros = ['brand_count', 'position_mean', 'recall_%', 'mrt_score_freerecall', 'total_participants' ]
-    no_recall['project_identifier'] = df['project_identifier'].iloc[0]
-    no_recall['task_name'] = df['task_name'].unique()[0]
-    no_recall[columns_to_fill_zeros] = 0.0
-    no_recall = no_recall[['group_id', 'project_identifier', 'task_name', 'recalled_brand',
-       'total_participants', 'brand_count', 'position_mean', 'recall_%',
-       'mrt_score_freerecall']].copy()
-    
-    result = pd.concat([no_recall, df], axis=0, ignore_index=True, sort=True)
-    result=result.sort_values(['group_id','mrt_score_freerecall'], ascending=[True, False]).reset_index(drop= True)
-    order_group = group + ['brand_count','position_mean',  'recall_%', 'mrt_score_freerecall']
-    result = result[order_group]
-    return result
-
+    df['log_position'] = np.log(df['position_mean'] + 1)
+    df['Freerecall'] = 1 / np.log(df['position_mean']+1) * df['recall_%']
+    df['Freerecall'] = df['Freerecall'].clip(0, 100)
+    df = df.sort_values('Freerecall', ascending=False).drop_duplicates().reset_index(drop=True)
+    df = df [group + ['position_mean', 'brand_count', 'recall_%', 'log_position', 'Freerecall']].copy()
+    df.rename(columns={'corrected':'mrt_stimulus'}, inplace=True)
+    df = df.drop_duplicates().reset_index(drop=True)    
+    return df
```

### Comparing `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/MRT_recognition_metric.py` & `neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/MRT_recognition_metric.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 import numpy as np
 import pandas as pd
+pd.options.display.show_dimensions = False
 
 def produce_demographics(df):
     """ Calculate age, gender, age_group bins demographics for the current 'group_id'
     Args:
         df (dataframe): given jatops dataframe
         id_col (str, optional): name of the column for participant id. Defaults to 'participant_id'.
         age_col (str, optional): name of the column for age data. Defaults to 'Age'.
@@ -16,16 +17,19 @@
     """
     age_demographics = df[['group_id','Age']].drop_duplicates()
     age_demographics= age_demographics.groupby(['group_id'], observed=False)['Age'].agg(['min', 'max', 'mean', 'std']).reset_index()
     age_demographics.rename(columns={'group_id': 'group_id Age'}, inplace=True)
     age_demographics.set_index('group_id Age', inplace=True)
     print(f'AGE Statistics: \n {age_demographics}')
 
+    age_group_count = df[['group_id','Age_Group','participant_id']].drop_duplicates()
+    age_group_count= age_group_count.groupby(['group_id', 'Age_Group'], observed=False)['participant_id'].agg(['count']).reset_index()
     age_group_split = df[['group_id','Age_Group','Age']].drop_duplicates()
-    age_group_split= age_group_split.groupby(['group_id', 'Age_Group'], observed=False)['Age'].agg(['count', 'min', 'max', 'mean', 'std'])
+    age_group_split= age_group_split.groupby(['group_id', 'Age_Group'], observed=False)['Age'].agg(['min', 'max', 'mean', 'std']).reset_index()
+    age_group_split = age_group_split.merge(age_group_count, on=['group_id','Age_Group'], how='left')
     print(f'\nAGE GROUP Statistics: \n {age_group_split}')
 
     gender_demographics = df[['group_id', 'Gender', 'participant_id', 'total_participants']].drop_duplicates()
     gender_demographics= gender_demographics.groupby(['group_id', 'Gender', 'total_participants'], observed=False)['participant_id'].agg(['count']).reset_index()
     gender_demographics['percentage'] = np.round(100 * gender_demographics['count']/gender_demographics['total_participants'], 2)
     gender_demographics.reset_index(drop = True, inplace=True)
     gender_demographics.set_index(['group_id', 'total_participants', 'Gender'], inplace=True)
@@ -80,15 +84,14 @@
         ub (int, optional): _description_. Defaults to 25000.
         group_columns (list, optional): Columns to be used for grouping. Defaults to ['mrt_stimulus', 'mrt_association', 'module_name', 'mrt_response', 'group_id'].
     Returns:
         dataframe: pivoted dataframe with total count of Yes and No responces
     """
     df.loc[:, 'certainty'] = ub - df['reaction_time'].copy()
     df.loc[:, 'mean_per_p'] = df.groupby(['participant_id', 'module_name'])['certainty'].transform('mean')
-
     gr_n = df.groupby(group_columns).size().reset_index(name='count')
     pivot_index = [x for x in group_columns if x != 'mrt_response']
     gr_n_p = gr_n.pivot(index=pivot_index, columns='mrt_response', values='count')
     gr_n_p = gr_n_p.reset_index()
 
     gr_n_p = gr_n_p.fillna(0)
     gr_n_p['Yes'] = 0 if 'Yes' not in gr_n_p.columns else gr_n_p['Yes']
@@ -165,14 +168,18 @@
 def calculate_certainty_score(row):
     """ Identifies the parameters of the row for further calculation of the certainty score
     Args:
         row (str or int): row of the dataframe
     Returns:
         float: value of the certianty score with the specific parameters
     """
+    if row['N_grouping_No'] < 3:
+        return 'small_no'
+    if row['N_grouping_Yes'] < 3:
+        return 'small_yes'
     if row['mrt_response'] == "Yes":
         return calculate_certainty_formula(row, 'N_grouping_Yes', 'g_iqr_yes')
     elif row['mrt_response'] == "No":
         return calculate_certainty_formula(row, 'N_grouping_Yes', 'g_iqr_no')
     
 
 def produce_mrt_score(df, group_columns=['mrt_stimulus', 'mrt_association', 'module_name', 'group_id', 'positive_negative'], certainty_col='certainty_score', response_col='mrt_response', certainty='certainty'):
@@ -182,33 +189,53 @@
         group_columns (list, optional): Columns requried for grouping. Defaults to ['mrt_stimulus', 'mrt_association', 'module_name', 'group_id', 'positive_negative'].
         certainty_col (str, optional): name of the column. Defaults to 'certainty_score'.
         response_col (str, optional): name of the column. Defaults to 'mrt_response'.
         certainty (str, optional): name of the column. Defaults to 'certainty'.
     Returns:
         dataframe: the dataframe that contains mrt_scores for each stimilus.
     """
+        # BREAK CERTAINTY
+    df_edge = df[(df[certainty_col] == 'small_no') | (df[certainty_col] == 'small_yes')].copy()
+    df = df[(df[certainty_col] != 'small_no') & (df[certainty_col] != 'small_yes')].copy()
     grouped_df = df.groupby(group_columns).agg(
         certainty_sum_Yes = (certainty_col, lambda x: x[df[response_col] == 'Yes'].sum()),
         certainty_sum_No = (certainty_col, lambda x: x[df[response_col] == 'No'].sum()),
-        certianty_Yes = (certainty, lambda x: x[df[response_col] == 'Yes'].mean()),
-        certainty_No = (certainty, lambda x: x[df[response_col] == 'No'].mean()),
         agreement_Yes = ('g_iqr_yes', 'mean'),
         agreement_No = ('g_iqr_no', 'mean'),
         N_Yes = (response_col, lambda x: (x == 'Yes').sum()),
         N_No = (response_col, lambda x: (x == 'No').sum()),
         N_Total = (response_col, 'count'),
         ).reset_index()
     
     grouped_df['%_Yes'] = (grouped_df['N_Yes'] / grouped_df['N_Total']) * 100
     grouped_df['%_No'] = (grouped_df['N_No'] / grouped_df['N_Total']) * 100
     grouped_df['mrt_summation'] = grouped_df['certainty_sum_Yes'] + grouped_df['certainty_sum_No']
     grouped_df['mrt_score'] = (grouped_df['certainty_sum_Yes'] / grouped_df['mrt_summation']) * 100
     grouped_df['Scaling'] = (grouped_df['mrt_score'] - grouped_df['%_Yes'])
+    grouped_df['Scaling'] = pd.to_numeric(grouped_df['Scaling'], errors='coerce')
     print('\n***** PLEASE CHECK: distribution of Scaling! *****')
-    print(grouped_df['Scaling'].describe())
+    print(grouped_df['Scaling'].astype('float').describe().to_frame().T)
+    
+    if df_edge.shape[0] > 0:
+        df_edge['mrt_score'] = 0
+        df_edge['Scaling'] = 0
+        df_edge.loc[df_edge[certainty_col] == 'small_no', 'mrt_score'] = 100
+        df_edge.loc[df_edge[certainty_col] == 'small_yes', 'mrt_score'] = 0
+        df_edge.loc[df_edge[certainty_col] == 'small_no', 'Scaling'] = 0
+        df_edge.loc[df_edge[certainty_col] == 'small_yes', 'Scaling'] = 100
+        df_edge['N_Yes'] = df_edge['N_grouping_Yes']
+        df_edge['N_No'] = df_edge['N_grouping_No']
+        df_edge['N_Total'] = df_edge['N_grouping_Yes'] + df_edge['N_grouping_No']
+        df_edge['%_Yes'] = (df_edge['N_grouping_Yes'] / df_edge['N_Total']) * 100
+        df_edge['%_No'] = (df_edge['N_grouping_No'] / df_edge['N_Total']) * 100
+        df_edge = df_edge[group_columns + ['mrt_score', 'N_Yes', 'N_No', 'N_Total', '%_Yes', '%_No', 'Scaling']].copy()
+        df_edge.drop_duplicates(inplace=True)
+        df_edge = df_edge.dropna(axis=1, how='all')
+        grouped_df = grouped_df.dropna(axis=1, how='all')  
+        grouped_df = pd.concat([grouped_df, df_edge], axis=0)
     return grouped_df
 
 
 def recognition_scores(df):
     """Step-by-step application of the memory recognition computation.
     Args:
         df (dataframe): initial dataframe
@@ -220,26 +247,24 @@
     merged = merge_dfs(mrt, mrt_pr)
     overall_quartiles = group_quartiles(merged)
     overall_quartiles['group_IQR'].describe()
     overall_response_d = groupby_and_tabulate(overall_quartiles)
     merged_iqr_n = merge_dfs(overall_quartiles, overall_response_d)
     merged_iqr_n["positive_negative"] = "Positive"
     merged_iqr_n['certainty_score']  = merged_iqr_n.apply(calculate_certainty_score, axis=1)
+    
     print('\n***** PLEASE CHECK: distribution of the certainty scores! *****')
-    print(merged_iqr_n['certainty_score'].describe())
-    overall_mrt = produce_mrt_score(merged_iqr_n, certainty_col='certainty_score', response_col='mrt_response')
-    memory_score = overall_mrt[['group_id', 'mrt_stimulus', 'mrt_association','mrt_score']].round(2)
-    memory_score.sort_values(['group_id','mrt_stimulus']).reset_index(drop=True)
-
-    # If Needed to use for overall % instead of reaction time based scores.
-    #total_percent = recognition_rate(df)
-    #recognition_df = pd.merge(total_percent, remember_ad_scores, on = ['group_id', 'mrt_stimulus', 'mrt_association'])
+    print(merged_iqr_n[(merged_iqr_n['certainty_score'] != 'small_no') & (merged_iqr_n['certainty_score'] != 'small_yes')]['certainty_score'].astype('float').describe().to_frame().T)
     
-    recognition_df = memory_score.sort_values(['group_id','mrt_score']).reset_index(drop=True)
-    return recognition_df
+    print('\n***** PLEASE CHECK: edge cases! *****')
+    print('Small number of No: ', merged_iqr_n[merged_iqr_n['certainty_score'] == 'small_no']['N_grouping_No'].unique())
+    print('Small number of Yes: ', merged_iqr_n[merged_iqr_n['certainty_score'] == 'small_yes']['N_grouping_Yes'].unique())
+
+    overall_mrt = produce_mrt_score(merged_iqr_n, certainty_col='certainty_score', response_col='mrt_response')
+    return overall_mrt
 
 
 def split_score(df, filter_list, column):
     """ Applies the filters, calculates recognition scores for each filtered DataFrame, 
         and merges them based on specific columns and suffixes.
     Args:
         df (DataFrame): DataFrame
@@ -249,28 +274,37 @@
         DataFrame: DataFrame with the mrt_scores based on the filters
     """
     split = pd.DataFrame()
     for filter_value in filter_list:
         filtered_df = df[df[column] == filter_value]
         split_part = recognition_scores(filtered_df)
         split_part[column] = filter_value
+        split_part = split_part.dropna(axis=1, how='all')  
         split = pd.concat([split, split_part], axis=0)
         split[column] = pd.Categorical(split[column], categories=filter_list, ordered=True)
 
     split.sort_values(['group_id','mrt_stimulus']+[column], inplace=True)
     index_cols = ['group_id', 'mrt_association', 'mrt_stimulus'] + [column]
     split.set_index(index_cols, inplace=True)
     return split    
 
-def create_combined_score(df, alpha = 1.1, beta = 1.5):
+def create_combined_score(freerecall, recognition, alpha = 1.1, beta = 1.5, type=[]):
     """creates combined score for all mrt partial scores
     Args:
         df (dataframe): given data with 3 mrt scores
         alpha (float, optional): weight for BRAND memory recall. Defaults to 1.1.
         beta (float, optional): weight for AD memory recall. Defaults to 1.5.
     Returns:
         dataframe: updated with the combined score
     """
-    df_updated = df.copy()
-    df_updated['mrt_score_brand_freerecall_AVG'] = alpha * ((df_updated['mrt_score_freerecall'] + df_updated['mrt_score_brand_recognition']) / 2)
-    df_updated['mrt_score_FINAL'] = ( df_updated['mrt_score_brand_freerecall_AVG'] + beta * df_updated['mrt_score_ad_recognition']) / 2
-    return df_updated
+    wide_df = recognition.pivot_table(index=['group_id', 'mrt_stimulus'] + type, columns='mrt_association', values=['mrt_score_recognition'], aggfunc='first', observed=False)
+    wide_df.columns = [f'{col[1]}' for col in wide_df.columns]
+    wide_df.reset_index(drop=False, inplace=True)
+    df_updated = freerecall.merge(wide_df, on = ['group_id', 'mrt_stimulus'] + type, how = 'outer')
+    df_updated['Brand&Freerecall AVG'] = ((df_updated['Freerecall'] + df_updated['Which Brand?']) / 2)
+    df_updated['Brand&Freerecall AVG'] = df_updated['Brand&Freerecall AVG'].clip(0, 100)
+    df_updated['Overall_Score'] = (alpha * (df_updated['Brand&Freerecall AVG']) + beta * df_updated['Remember Ad?']) / 2
+    df_updated['Overall_Score'] = df_updated['Overall_Score'].clip(0, 100)
+    col1 = ['group_id', 'project_identifier', 'total_participants','mrt_stimulus']
+    col2 = ['position_mean', 'brand_count', 'recall_%', 'Freerecall', 'Remember Ad?', 'Which Brand?', 'Overall_Score']
+    df_updated = df_updated[col1 + type + col2].copy()
+    return df_updated
```

### Comparing `neuronsmemorytestpipeline-0.0.9/src/neuronsmemorytestpipeline/QA_modules.py` & `neuronsmemorytestpipeline-0.1.0/src/neuronsmemorytestpipeline/QA_modules.py`

 * *Files identical despite different names*

### Comparing `neuronsmemorytestpipeline-0.0.9/PKG-INFO` & `neuronsmemorytestpipeline-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NeuronsMemoryTestPipeline
-Version: 0.0.9
+Version: 0.1.0
 Summary: Package provides QA, MRT and FRT metrics calculation for frt and mrt scores.
 Home-page: https://gitlab.com/neurons-inc1/data-analyst/neurons_metrics_package
 License: MIT
 Keywords: metrics,QA,MRT,FRT,freerecall
 Author: Irina White
 Author-email: i.white@neuronsinc.com
 Requires-Python: >=3.8,<4.0
```

