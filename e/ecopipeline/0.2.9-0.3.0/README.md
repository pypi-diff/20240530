# Comparing `tmp/ecopipeline-0.2.9.tar.gz` & `tmp/ecopipeline-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecopipeline-0.2.9.tar", last modified: Mon Apr 29 22:10:05 2024, max compression
+gzip compressed data, was "ecopipeline-0.3.0.tar", last modified: Thu May 30 20:09:53 2024, max compression
```

## Comparing `ecopipeline-0.2.9.tar` & `ecopipeline-0.3.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32173 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/extract/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.041734 ecopipeline-0.2.9/src/ecopipeline/load/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13181 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/load/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline/transform/
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17319 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/bayview.py
--rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/lbnl.py
--rw-r--r--   0 runner    (1001) docker     (127)    30170 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/transform/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-29 22:09:31.000000 ecopipeline-0.2.9/src/ecopipeline/utils/unit_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 22:10:05.045734 ecopipeline-0.2.9/src/ecopipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 22:10:05.000000 ecopipeline-0.2.9/src/ecopipeline.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.817597 ecopipeline-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.817597 ecopipeline-0.3.0/src/ecopipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/src/ecopipeline/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37908 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/extract/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/src/ecopipeline/load/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10444 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/load/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/src/ecopipeline/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17409 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/transform/bayview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33400 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/transform/lbnl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33960 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/transform/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/src/ecopipeline/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/utils/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-05-30 20:09:22.000000 ecopipeline-0.3.0/src/ecopipeline/utils/unit_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 20:09:53.821597 ecopipeline-0.3.0/src/ecopipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-30 20:09:53.000000 ecopipeline-0.3.0/src/ecopipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-30 20:09:53.000000 ecopipeline-0.3.0/src/ecopipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 20:09:53.000000 ecopipeline-0.3.0/src/ecopipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 20:09:53.000000 ecopipeline-0.3.0/src/ecopipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-30 20:09:53.000000 ecopipeline-0.3.0/src/ecopipeline.egg-info/top_level.txt
```

### Comparing `ecopipeline-0.2.9/PKG-INFO` & `ecopipeline-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.9
+Version: 0.3.0
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.9/README.md` & `ecopipeline-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.9/setup.cfg` & `ecopipeline-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ecopipeline
-version = 0.2.9
+version = 0.3.0
 authors = ["Carlos Bello, <bellocarlos@seattleu.edu>, Emil Fahrig <fahrigemil@seattleu.edu>, Casey Mang <cmang@seattleu.edu>, Julian Harris <harrisjulian@seattleu.edu>, Roger Tram <rtram@seattleu.edu>, Nolan Price <nolan@ecotope.com>"]
 description = Contains functions for use in Ecotope Datapipelines
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/extract/extract.py` & `ecopipeline-0.3.0/src/ecopipeline/extract/extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -142,35 +142,39 @@
 
 
     else: 
         startTime_int = int(startTime.strftime("%Y%m%d%H%M%S"))
         return_list = list(filter(lambda filename: int(filename[-17:-3]) >= startTime_int and (endTime is None or int(filename[-17:-3]) < int(endTime.strftime("%Y%m%d%H%M%S"))), filenames))
     return return_list
 
-def extract_files(extension: str, config: ConfigManager) -> List[str]:
+def extract_files(extension: str, config: ConfigManager, data_sub_dir : str = "") -> List[str]:
     """
     Function takes in a file extension and subdirectory and returns a list of paths files in the directory of that type.
 
     Parameters
     ----------  
     extension : str
         File extension of raw data files as string (e.g. ".csv", ".gz", ...)
     config : ecopipeline.ConfigManager
         The ConfigManager object that holds configuration data for the pipeline 
+    data_sub_dir : str
+        defaults to an empty string. If the files being accessed are in a sub directory of the configured data directory, use this parameter to point there.
+        e.g. if the data files you want to extract are in "path/to/data/DENT/" and your configured data directory is "path/to/data/", put "DENT/" as the data_sub_dir
     
     Returns
     ------- 
     List[str]: 
         List of filenames 
     """
     os.chdir(os.getcwd())
     filenames = []
-    for file in os.listdir(config.data_directory):
+    full_data_path = f"{config.data_directory}{data_sub_dir}"
+    for file in os.listdir(full_data_path):
         if file.endswith(extension):
-            full_filename = os.path.join(config.data_directory, file)
+            full_filename = os.path.join(full_data_path, file)
             filenames.append(full_filename)
 
     return filenames
 
 
 def json_to_df(json_filenames: List[str], time_zone: str = 'US/Pacific') -> pd.DataFrame:
     """
@@ -213,31 +217,35 @@
             # Iterate over the index and round up if necessary (work around for json format from sensors)
             for i in range(len(norm_data.index)):
                 if norm_data.index[i].minute == 59 and norm_data.index[i].second == 59:
                     norm_data.index.values[i] = norm_data.index[i] + pd.Timedelta(seconds=1)
             temp_dfs.append(norm_data)
 
     df = pd.concat(temp_dfs, ignore_index=False)
-    return df
-
+    return df  
 
-def csv_to_df(csv_filenames: List[str], mb_prefix : bool = False, round_time_index : bool = True) -> pd.DataFrame:
+def csv_to_df(csv_filenames: List[str], mb_prefix : bool = False, round_time_index : bool = True, create_time_pt_idx : bool = False, original_time_columns : str = 'DateTime', time_format : str ='%Y/%m/%d %H:%M:%S') -> pd.DataFrame:
     """
     Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for aquisuite data. 
 
     Parameters
     ----------  
     csv_filenames: List[str]
         List of filenames to be processed into a single dataframe 
     mb_prefix: bool
         A boolean that signifys if the data is in modbus form- if set to true, will prepend modbus prefix to each raw varriable name
     round_time_index: bool
         A boolean that signifys if the dataframe timestamp indexes should be rounded down to the nearest minute.
         Should be set to False if there is no column in the data frame called 'time(UTC)' to index on.
         Defaults to True.
+    create_time_pt_idx: bool
+        set to true if there is a time column in the csv that you wish to convert to a 'time_pt' index. False otherwise
+        defaults to false.
+    original_time_columns : str
+        The name of the time column in the raw datafiles. defaults to 'DateTime'. Only used if create_time_pt_idx is True
         
     Returns
     ------- 
     pd.DataFrame: 
         Pandas Dataframe containing data from all files with column headers the same as the variable names in the files 
         (with prepended modbus prefix if mb_prefix = True)
     """
@@ -262,16 +270,130 @@
                     data = data.set_index("time(UTC)")
                     data = data.rename(columns={col: f"{prefix}_{col}".replace(" ","_") for col in data.columns})
                 else:
                     print(f"Error reading {file}: No 'time(UTC)' column found.")
                     continue
                 
             temp_dfs.append(data)
+    df = pd.concat(temp_dfs, ignore_index=False)
+
+    if create_time_pt_idx:
+        df['time_pt'] = pd.to_datetime(df[original_time_columns], format=time_format)
+        df.set_index('time_pt', inplace=True)
+
+    if round_time_index:
+        #round down all seconds, 99% of points come in between 0 and 30 seconds but there are a few that are higher
+        df.index = df.index.floor('T')
+        
+        #group and sort index
+        df = df.groupby(df.index).mean(numeric_only=True)
+        df.sort_index(inplace = True)
 
-    df = pd.concat(temp_dfs, ignore_index=False) 
+    return df
+
+def dent_csv_to_df(csv_filenames: List[str], round_time_index : bool = True) -> pd.DataFrame:
+    """
+    Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for aquisuite data. 
+
+    Parameters
+    ----------  
+    csv_filenames: List[str]
+        List of filenames to be processed into a single dataframe 
+    round_time_index: bool
+        A boolean that signifys if the dataframe timestamp indexes should be rounded down to the nearest minute.
+        Should be set to False if there is no column in the data frame called 'time(UTC)' to index on.
+        Defaults to True.
+        
+    Returns
+    ------- 
+    pd.DataFrame: 
+        Pandas Dataframe containing data from all files with column headers the same as the variable names in the files 
+        (with prepended modbus prefix if mb_prefix = True)
+    """
+    temp_dfs = []
+    for file in csv_filenames:
+        try:
+            # data headers are on row 13
+            data = pd.read_csv(file, skiprows=12)
+        except FileNotFoundError:
+            print("File Not Found: ", file)
+            return
+        except Exception as e:
+            print(f"Error reading {file}: {e}")
+            #raise e  # Raise the caught exception again
+            continue
+
+        if len(data) != 0:
+            if len(data.columns) >= 3:
+                # in dent file format, the first column can be removed and the second and third columns are date and time respectively
+                data.columns = ['temp', 'date', 'time'] + data.columns.tolist()[3:]
+                data = data.drop(columns=['temp'])
+                data['time_pt'] = pd.to_datetime(data['date'] + ' ' + data['time'])
+                data = data.set_index("time_pt")
+            else:
+                print(f"Error reading {file}: No time columns found.")
+                continue
+                
+            temp_dfs.append(data)
+    df = pd.concat(temp_dfs, ignore_index=False)
+    
+    if round_time_index:
+        #round down all seconds, 99% of points come in between 0 and 30 seconds but there are a few that are higher
+        df.index = df.index.floor('T')
+        
+        #group and sort index
+        df = df.groupby(df.index).mean(numeric_only=True)
+        df.sort_index(inplace = True)
+
+    return df
+
+def flow_csv_to_df(csv_filenames: List[str], round_time_index : bool = True) -> pd.DataFrame:
+    """
+    Function takes a list of csv filenames and reads all files into a singular dataframe. Use this for aquisuite data. 
+
+    Parameters
+    ----------  
+    csv_filenames: List[str]
+        List of filenames to be processed into a single dataframe 
+    round_time_index: bool
+        A boolean that signifys if the dataframe timestamp indexes should be rounded down to the nearest minute.
+        Should be set to False if there is no column in the data frame called 'time(UTC)' to index on.
+        Defaults to True.
+        
+    Returns
+    ------- 
+    pd.DataFrame: 
+        Pandas Dataframe containing data from all files with column headers the same as the variable names in the files 
+        (with prepended modbus prefix if mb_prefix = True)
+    """
+    temp_dfs = []
+    for file in csv_filenames:
+        try:
+            # data headers are on row 6
+            data = pd.read_csv(file, skiprows=6)
+        except FileNotFoundError:
+            print("File Not Found: ", file)
+            return
+        except Exception as e:
+            print(f"Error reading {file}: {e}")
+            #raise e  # Raise the caught exception again
+            continue
+
+        if len(data) != 0:
+            if all(x in data.columns.to_list() for x in ['Month','Day','Year','Hour','Minute','Second']):
+                # Convert the datetime string to datetime
+                date_str = data['Year'].astype(str) + '-' + data['Month'].astype(str).str.zfill(2) + '-' + data['Day'].astype(str).str.zfill(2) + ' ' + data['Hour'].astype(str).str.zfill(2) + ':' + data['Minute'].astype(str).str.zfill(2) + ':' + data['Second'].astype(str).str.zfill(2)
+                data['time_pt'] = pd.to_datetime(date_str, format='%Y-%m-%d %H:%M:%S')
+                data = data.set_index("time_pt")
+            else:
+                print(f"Error reading {file}: No time columns found.")
+                continue
+                
+            temp_dfs.append(data)
+    df = pd.concat(temp_dfs, ignore_index=False)
     
     if round_time_index:
         #round down all seconds, 99% of points come in between 0 and 30 seconds but there are a few that are higher
         df.index = df.index.floor('T')
         
         #group and sort index
         df = df.groupby(df.index).mean(numeric_only=True)
@@ -374,15 +496,15 @@
         variable_data = variable_data.loc[variable_data['system'].str.contains(system, na=False)]
 
     variable_data = variable_data.loc[:, ['variable_alias', 'variable_name']]
     variable_data.dropna(axis=0, inplace=True)
     variable_alias = list(variable_data["variable_alias"])
     variable_true = list(variable_data["variable_name"])
     variable_alias_true_dict = dict(zip(variable_alias, variable_true))
-    
+
     temp_dfs = []
     for file in csv_filenames:
         # each file contains a single variable in this format
         try:
             data = pd.read_csv(file)
         except FileNotFoundError:
             print("File Not Found: ", file)
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/load/load.py` & `ecopipeline-0.3.0/src/ecopipeline/load/load.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,89 +15,14 @@
             'int32':'float',
             'float64': 'float',
             'M8[ns]':'datetime',
             'datetime64[ns]':'datetime',
             'object':'varchar(25)',
             'bool': 'boolean'}
 
-# def get_login_info(table_headers: list, config_file_path : str) -> dict:
-#     """
-#     Reads the config.ini file stored in the config_file_path file path.   
-
-#     Parameters
-#     ---------- 
-#     table_headers : list
-#         A list of table headers. These headers must correspond to the 
-#         section headers in the config.ini file. Your list must contain the section
-#         header for each table you wish to write into. The first header must correspond 
-#         to the login information of the database. The other are the tables which you wish
-#         to write to. 
-#     config : ecopipeline.ConfigManager
-#         The ConfigManager object that holds configuration data for the pipeline
-
-#     Returns
-#     ------- 
-#     dict: 
-#         A dictionary containing all relevant information is returned. This
-#         includes information used to create a connection with a mySQL server and
-#         information (table names and column names) used to load the data into 
-#         tables. 
-#     """
-
-#     if not os.path.exists(config_file_path):
-#         print(f"File path '{config_file_path}' does not exist.")
-#         sys.exit()
-
-#     configure = configparser.ConfigParser()
-#     configure.read(config_file_path)
-
-#     db_connection_info = {
-#         "database": {'user': configure.get('database', 'user'),
-#                      'password': configure.get('database', 'password'),
-#                      'host': configure.get('database', 'host'),
-#                      'database': configure.get('database', 'database')}
-#     }
-
-#     db_table_info = {header: {"table_name": configure.get(header, 'table_name')} for header in table_headers} 
-    
-#     db_connection_info.update(db_table_info)
-
-#     print(f"Successfully fetched configuration information from file path {config_file_path}.")
-#     return db_connection_info
-    
-
-# def connect_db(config_info: dict):
-#     """
-#     Create a connection with the mySQL server. 
-
-#     Parameters
-#     ----------  
-#     config_info : dict 
-#         The dictionary containing the credential information. This is
-#         contained in the 'database' section of the dictionary. 
-
-#     Returns
-#     ------- 
-#     mysql.connector.cursor.MySQLCursor: 
-#         A connection and cursor object. THe cursor can be used to execute
-#         mySQL queries and the connection object can be used to save those changes. 
-#     """
-
-#     connection = None
-
-#     try:
-#         connection = mysql.connector.connect(**config_info)
-#     except mysql.connector.Error:
-#         print("Unable to connect to database with given credentials.")
-#         return None, None
-
-#     print(f"Successfully connected to database.")
-#     return connection, connection.cursor()
-
-
 def check_table_exists(cursor : mysql.connector.cursor.MySQLCursor, table_name: str, dbname: str) -> int:
     """
     Check if the given table name already exists in database.
 
     Parameters
     ---------- 
     cursor : mysql.connector.cursor.MySQLCursor
@@ -222,16 +147,16 @@
         boolean indicating if the the column were successfully added to the database. 
     """
     alter_table_statements = [f"ALTER TABLE {table_name} ADD COLUMN {column} {data_type} DEFAULT NULL;" for column, data_type in zip(new_columns, data_types)]
 
     for sql_statement in alter_table_statements:
         try:
             cursor.execute(sql_statement)
-        except mysqlerrors.DatabaseError:
-            print("Error communicating with the mysql database.")
+        except mysqlerrors.DatabaseError as e:
+            print(f"Error communicating with the mysql database: {e}")
             return False
 
     return True
 
 def load_overwrite_database(cursor : mysql.connector.cursor.MySQLCursor, dataframe: pd.DataFrame, config_info: dict, data_type: str, primary_key: str = "time_pt", table_name: str = None):
     """
     Loads given pandas DataFrame into a MySQL table overwriting any conflicting data. Uses an UPSERT strategy to ensure any gaps in data are filled.
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/transform/__init__.py` & `ecopipeline-0.3.0/src/ecopipeline/transform/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, nullify_erroneous, sensor_adjustment, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, cop_method_1, cop_method_2, create_summary_tables, remove_partial_days
+from .transform import rename_sensors, avg_duplicate_times, remove_outliers, ffill_missing, nullify_erroneous, sensor_adjustment, round_time, aggregate_df, join_to_hourly, concat_last_row, join_to_daily, cop_method_1, cop_method_2, create_summary_tables, remove_partial_days,convert_c_to_f,convert_l_to_g, convert_on_off_col_to_bool
 from .lbnl import nclarity_filter_new, site_specific, condensate_calculations, gas_valve_diff, gather_outdoor_conditions, aqsuite_prep_time, nclarity_csv_to_df, _add_date, add_local_time, aqsuite_filter_new, get_refrig_charge, elev_correction, change_ID_to_HVAC, get_hvac_state, get_cop_values, get_cfm_values, replace_humidity, create_fan_curves, lbnl_temperature_conversions, lbnl_pressure_conversions, lbnl_sat_calculations, get_site_cfm_info, get_site_info, merge_indexlike_rows
 from .bayview import calculate_cop_values, aggregate_values, get_energy_by_min, verify_power_energy, get_temp_zones120, get_storage_gals120
 __all__ = ["rename_sensors", "avg_duplicate_times", "remove_outliers", "ffill_missing", "nullify_erroneous", "sensor_adjustment", "round_time", "aggregate_df", "join_to_hourly", "concat_last_row", "join_to_daily", 
            "cop_method_1", "cop_method_2", "create_summary_tables", "remove_partial_days", "nclarity_filter_new", "site_specific", "condensate_calculations", "gas_valve_diff", "gather_outdoor_conditions", "aqsuite_prep_time", 
            "nclarity_csv_to_df", "_add_date", "add_local_time", "aqsuite_filter_new", "get_refrig_charge", "elev_correction", "change_ID_to_HVAC", "get_hvac_state", "get_cop_values", "get_cfm_values", "replace_humidity", 
            "create_fan_curves", "lbnl_temperature_conversions", "lbnl_pressure_conversions", "lbnl_sat_calculations", "get_site_cfm_info", "get_site_info", "merge_indexlike_rows", "calculate_cop_values", "aggregate_values", 
-           "get_energy_by_min", "verify_power_energy", "get_temp_zones120", "get_storage_gals120"]
+           "get_energy_by_min", "verify_power_energy", "get_temp_zones120", "get_storage_gals120","convert_c_to_f","convert_l_to_g", "convert_on_off_col_to_bool"]
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/transform/bayview.py` & `ecopipeline-0.3.0/src/ecopipeline/transform/bayview.py`

 * *Files 1% similar despite different names*

```diff
@@ -373,19 +373,19 @@
     df['EnergyIn_SecLoopPump'] = df['PowerIn_SecLoopPump'] * (1/60)
     df['EnergyIn_HPWH'] = df['EnergyIn_HPWH']
 
     cop_inter = df [['Temp_RecircSupply_avg', 'HeatOut_PrimaryPlant', 'HeatOut_SecLoop', 'HeatOut_HW', 'HeatLoss_TempMaint_MXV1', 'HeatLoss_TempMaint_MXV2', 'EnergyIn_SecLoopPump', 'EnergyIn_HPWH']].resample('D').mean()
 
     cop_inter['HeatOut_HW_dyavg'] = energy_kwh_to_kbtu(avg_sd['Flow_CityWater'], cop_inter['Temp_RecircSupply_avg'] -
                                                        avg_sd_6['Temp_CityWater'])
+    # in case of negative heat out or negligable temperature delta, set to zero
     cop_inter['HeatOut_PrimaryPlant_dyavg'] = energy_kwh_to_kbtu(avg_sd['Flow_CityWater_atSkid'],
-                                                                 avg_sd['Temp_PrimaryStorageOutTop'] -
-                                                                 avg_sd_6['Temp_CityWater_atSkid'])
-    # in case of negative heat out, set to zero
-    cop_inter.loc['HeatOut_PrimaryPlant_dyavg'] = cop_inter.loc['HeatOut_PrimaryPlant_dyavg'].apply(lambda x: max(x, 0))
+                                                                 avg_sd['Temp_PrimaryStorageOutTop'] - avg_sd_6['Temp_CityWater_atSkid'])
+    cop_inter.loc[(avg_sd['Temp_PrimaryStorageOutTop'] - avg_sd_6['Temp_CityWater_atSkid']) < 2, 'HeatOut_PrimaryPlant_dyavg'] = 0
+    cop_inter['HeatOut_PrimaryPlant_dyavg'] = cop_inter['HeatOut_PrimaryPlant_dyavg'].apply(lambda x: max(x, 0))
 
     return cop_inter
 
 
 def calculate_cop_values(df: pd.DataFrame, heatLoss_fixed: int, thermo_slice: str) -> pd.DataFrame:
     """
     Performs COP calculations using the daily aggregated data.
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/transform/lbnl.py` & `ecopipeline-0.3.0/src/ecopipeline/transform/lbnl.py`

 * *Files identical despite different names*

### Comparing `ecopipeline-0.2.9/src/ecopipeline/transform/transform.py` & `ecopipeline-0.3.0/src/ecopipeline/transform/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 import numpy as np
 import datetime as dt
 import csv
 import os
-from ecopipeline.utils.unit_convert import energy_to_power, energy_btu_to_kwh, energy_kwh_to_kbtu, power_flow_to_kW
+from ecopipeline.utils.unit_convert import temp_c_to_f_non_noaa, volume_l_to_g
 from ecopipeline import ConfigManager
 
 pd.set_option('display.max_columns', None)
 
 
 def concat_last_row(df: pd.DataFrame, last_row: pd.DataFrame) -> pd.DataFrame:
     """
@@ -99,22 +99,21 @@
         variable_data = variable_data.loc[variable_data['system'].str.contains(system, na=False)]
 
     variable_data = variable_data.loc[:, ['variable_alias', 'variable_name']]
     variable_data.dropna(axis=0, inplace=True)
     variable_alias = list(variable_data["variable_alias"])
     variable_true = list(variable_data["variable_name"])
     variable_alias_true_dict = dict(zip(variable_alias, variable_true))
-
     # Create a copy of the original DataFrame
     df = original_df.copy()
 
     df.rename(columns=variable_alias_true_dict, inplace=True)
 
     # drop columns that do not have a corresponding true name
-    df.drop(columns=[col for col in df if col in variable_alias], inplace=True)
+    df.drop(columns=[col for col in df if col in variable_alias and col not in variable_true], inplace=True)
 
     # drop columns that are not documented in variable names csv file at all
     df.drop(columns=[col for col in df if col not in variable_true], inplace=True)
     #drop null columns
     df = df.dropna(how='all')
 
     return df
@@ -471,14 +470,91 @@
                                     'PowerIn_TM': df[sum_tm_cols].sum(axis=1)
                                     })
 
     df['COP_DHWSys_2'] = (df[cop_primary_column_name] * (sum_power_in_df['PowerIn_Primary']/df['PowerIn_Total'])) + (cop_tm * (sum_power_in_df['PowerIn_TM']/df['PowerIn_Total']))
 
     return df
 
+def convert_on_off_col_to_bool(df: pd.DataFrame, column_names: list) -> pd.DataFrame:
+    """
+    Function takes in a pandas dataframe of data and a list of column names to convert from the strings 
+    "ON" and "OFF" to boolean values True and False resperctively.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Single pandas dataframe of sensor data.
+    column_names : list of stings
+        list of columns with data currently in strings "ON" and "OFF" that need to be converted to boolean values
+
+    Returns
+    -------
+    pd.DataFrame: Dataframe with specified columns converted from Celsius to Farenhiet.
+    """
+    
+    mapping = {'ON': True, 'OFF': False}
+    
+    for column_name in column_names: 
+        df[column_name] = df[column_name].map(mapping).where(df[column_name].notna(), df[column_name])
+    
+    return df
+
+def convert_c_to_f(df: pd.DataFrame, column_names: list) -> pd.DataFrame:
+    """
+    Function takes in a pandas dataframe of data and a list of column names to convert from degrees Celsius to Farenhiet.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Single pandas dataframe of sensor data.
+    column_names : list of stings
+        list of columns with data currently in Celsius that need to be converted to Farenhiet
+
+    Returns
+    -------
+    pd.DataFrame: Dataframe with specified columns converted from Celsius to Farenhiet.
+    """
+    for col in column_names:
+        if col in df.columns.to_list():
+            try:
+                pd.to_numeric(df[col])
+                df[col] = df[col].apply(temp_c_to_f_non_noaa)
+            except ValueError:
+                print(f"{col} is not a numeric value column and could not be converted.")
+        else:
+            print(f"{col} is not included in this data set.")
+    return df
+
+def convert_l_to_g(df: pd.DataFrame, column_names: list) -> pd.DataFrame:
+    """
+    Function takes in a pandas dataframe of data and a list of column names to convert from Liters to Gallons.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Single pandas dataframe of sensor data.
+    column_names : list of stings
+        list of columns with data currently in Liters that need to be converted to Gallons
+
+    Returns
+    -------
+    pd.DataFrame: Dataframe with specified columns converted from Liters to Gallons.
+    """
+    for col in column_names:
+        if col in df.columns.to_list():
+            try:
+                pd.to_numeric(df[col])
+                df[col] = df[col].apply(volume_l_to_g)
+            except ValueError:
+                print(f"{col} is not a numeric value column and could not be converted.")
+        else:
+            print(f"{col} is not included in this data set.")
+    return df
+
+
 def aggregate_df(df: pd.DataFrame, ls_filename: str = "", complete_hour_threshold : float = 0.8, complete_day_threshold : float = 1.0, remove_partial : bool = True) -> (pd.DataFrame, pd.DataFrame):
     """
     Function takes in a pandas dataframe of minute data, aggregates it into hourly and daily 
     dataframes, appends 'load_shift_day' column onto the daily_df and the 'system_state' column to
     hourly_df to keep track of the loadshift schedule for the system, and then returns those dataframes.
     The function will only trim the returned dataframes such that only averages from complete hours and
     complete days are returned rather than agregated data from partial datasets.
@@ -515,47 +591,50 @@
     # Start by splitting the dataframe into sum, which has all energy related vars, and mean, which has everything else. Time is calc'd differently because it's the index
     sum_df = (df.filter(regex=".*Energy.*")).filter(regex="^(?!.*EnergyRate).*(?<!BTU)$")
     # NEEDS TO INCLUDE: EnergyOut_PrimaryPlant_BTU
     mean_df = df.filter(regex="^((?!Energy)(?!EnergyOut_PrimaryPlant_BTU).)*$")
 
     # Resample downsamples the columns of the df into 1 hour bins and sums/means the values of the timestamps falling within that bin
     hourly_sum = sum_df.resample('H').sum()
-    hourly_mean = mean_df.resample('H').mean()
+    hourly_mean = mean_df.resample('H').mean(numeric_only=True)
     # Same thing as for hours, but for a whole day
     daily_sum = sum_df.resample("D").sum()
-    daily_mean = mean_df.resample('D').mean()
+    daily_mean = mean_df.resample('D').mean(numeric_only=True)
 
     # combine sum_df and mean_df into one hourly_df, then try and print that and see if it breaks
     hourly_df = pd.concat([hourly_sum, hourly_mean], axis=1)
     daily_df = pd.concat([daily_sum, daily_mean], axis=1)
 
+    partial_day_removal_exclusion = []
+
     # appending loadshift data
     if ls_filename != "" and os.path.exists(ls_filename):
         ls_df = pd.read_csv(ls_filename)
         # Parse 'date' and 'startTime' columns to create 'startDateTime'
         ls_df['startDateTime'] = pd.to_datetime(ls_df['date'] + ' ' + ls_df['startTime'])
         # Parse 'date' and 'endTime' columns to create 'endDateTime'
         ls_df['endDateTime'] = pd.to_datetime(ls_df['date'] + ' ' + ls_df['endTime'])
         daily_df["load_shift_day"] = False
         hourly_df["system_state"] = 'normal'
+        partial_day_removal_exclusion = ["load_shift_day","system_state"]
         for index, row in ls_df.iterrows():
             startDateTime = row['startDateTime']
             endDateTime = row['endDateTime']
             event = row['event']
 
             # Update 'system_state' in 'hourly_df' and 'load_shift_day' in 'daily_df' based on conditions
             hourly_df.loc[(hourly_df.index >= startDateTime) & (hourly_df.index < endDateTime), 'system_state'] = event
             daily_df.loc[daily_df.index.date == startDateTime.date(), 'load_shift_day'] = True
             daily_df.loc[daily_df.index.date == endDateTime.date(), 'load_shift_day'] = True
     else:
         print(f"The loadshift file '{ls_filename}' does not exist. Thus loadshifting will not be added to daily dataframe.")
     
     # if any day in hourly table is incomplete, we should delete that day from the daily table as the averaged data it contains will be from an incomplete day.
     if remove_partial:
-        hourly_df, daily_df = remove_partial_days(df, hourly_df, daily_df, complete_hour_threshold, complete_day_threshold)
+        hourly_df, daily_df = remove_partial_days(df, hourly_df, daily_df, complete_hour_threshold, complete_day_threshold, partial_day_removal_exclusion = partial_day_removal_exclusion)
     return hourly_df, daily_df
 
 
 def create_summary_tables(df: pd.DataFrame):
     """
     Revamped version of "aggregate_data" function. Creates hourly and daily summary tables.
 
@@ -575,15 +654,15 @@
     
     hourly_df = df.resample('H').mean()
     daily_df = df.resample('D').mean()
 
     hourly_df, daily_df = remove_partial_days(df, hourly_df, daily_df)
     return hourly_df, daily_df
 
-def remove_partial_days(df, hourly_df, daily_df, complete_hour_threshold : float = 0.8, complete_day_threshold : float = 1.0):
+def remove_partial_days(df, hourly_df, daily_df, complete_hour_threshold : float = 0.8, complete_day_threshold : float = 1.0, partial_day_removal_exclusion : list = []):
     '''
     Helper function for removing daily and hourly values that are calculated from incomplete data.
 
     Parameters
     ----------
     df : pd.DataFrame
         Single pandas dataframe of minute-by-minute sensor data.
@@ -591,36 +670,51 @@
         agregated daily dataframe that contains all daily information.
     hourly_df : pd.DataFrame
         agregated hourly dataframe that contains all hourly information.
     complete_hour_threshold : float
         Default to 0.8. percent of minutes in an hour needed to count as a complete hour. Percent as a float (e.g. 80% = 0.8)
     complete_day_threshold : float
         Default to 1.0. percent of hours in a day needed to count as a complete day. Percent as a float (e.g. 80% = 0.8)
+    partial_day_removal_exclusion : list[str]
+        List of column names to ignore when searching through columns to remove sections without enough data
     '''
     if complete_hour_threshold < 0.0 or complete_hour_threshold > 1.0:
         raise Exception("complete_hour_threshold must be a float between 0 and 1 to represent a percent (e.g. 80% = 0.8)")
     if complete_day_threshold < 0.0 or complete_day_threshold > 1.0:
         raise Exception("complete_day_threshold must be a float between 0 and 1 to represent a percent (e.g. 80% = 0.8)")
     
     num_minutes_required = 60.0 * complete_hour_threshold
     incomplete_hours = []
     for hour in hourly_df.index:
         next_hour = hour + pd.Timedelta(hours=1)
         filtered_df = df.loc[(df.index >= hour) & (df.index < next_hour)]
         if len(filtered_df.index) < num_minutes_required:
             incomplete_hours.append(hour)
+        else:
+            for column in hourly_df.columns.to_list():
+                if column not in partial_day_removal_exclusion:
+                    not_null_count = filtered_df[column].notna().sum()
+                    if not_null_count < num_minutes_required:
+                        hourly_df.loc[hour, column] = np.nan
+
     hourly_df = hourly_df.drop(incomplete_hours)
     
     num_complete_hours_required = 24.0 * complete_day_threshold
     incomplete_days = []
     for day in daily_df.index:
         next_day = day + pd.Timedelta(days=1)
         filtered_df = hourly_df.loc[(hourly_df.index >= day) & (hourly_df.index < next_day)]
         if len(filtered_df.index) < num_complete_hours_required:
             incomplete_days.append(day)
+        else:
+            for column in daily_df.columns.to_list():
+                if column not in partial_day_removal_exclusion:
+                    not_null_count = filtered_df[column].notna().sum()
+                    if not_null_count < num_complete_hours_required:
+                        daily_df.loc[day, column] = np.nan
     daily_df = daily_df.drop(incomplete_days)
 
     return hourly_df, daily_df
 
 
 def join_to_hourly(hourly_data: pd.DataFrame, noaa_data: pd.DataFrame) -> pd.DataFrame:
     """
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/utils/ConfigManager.py` & `ecopipeline-0.3.0/src/ecopipeline/utils/ConfigManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,14 @@
         ------- 
         mysql.connector.MySQLConnection, mysql.connector.cursor.MySQLCursor: 
             A connection and cursor object. THe cursor can be used to execute
             mySQL queries and the connection object can be used to save those changes. 
         """
 
         connection = None
-        print(self.db_connection_info)
         try:
             connection = mysql.connector.connect(
                 host=self.db_connection_info['host'],
                 user=self.db_connection_info['user'],
                 password=self.db_connection_info['password'],
                 database=self.db_connection_info['database']
             )
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline/utils/unit_convert.py` & `ecopipeline-0.3.0/src/ecopipeline/utils/unit_convert.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 # Ex. temp_c_to_f(temp_c)
 
 # Used in NOAA Data
 def temp_c_to_f(temp_c : float):
     temp_f = 32 + (temp_c/10)* 9/5
     return temp_f
 
+def temp_c_to_f_non_noaa(temp_c : float):
+    temp_f = 32 + (temp_c * 1.8)
+    return temp_f
+
+def volume_l_to_g(liters : float):
+    gallons = 0.2641729 * liters
+    return gallons
+
 # Used in NOAA Data
 def divide_num_by_ten(num : float):
     return (num/10)
 
 # Used in NOAA Data
 def windspeed_mps_to_knots(speed : float):
     speed_kts = 1.9438445 * speed/10
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline.egg-info/PKG-INFO` & `ecopipeline-0.3.0/src/ecopipeline.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecopipeline
-Version: 0.2.9
+Version: 0.3.0
 Summary: Contains functions for use in Ecotope Datapipelines
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ecopipeline-0.2.9/src/ecopipeline.egg-info/SOURCES.txt` & `ecopipeline-0.3.0/src/ecopipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

