# Comparing `tmp/pygcap-0.0.1.tar.gz` & `tmp/pygcap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygcap-0.0.1.tar", last modified: Thu May 30 07:36:08 2024, max compression
+gzip compressed data, was "pygcap-0.0.2.tar", last modified: Thu May 30 08:43:45 2024, max compression
```

## Comparing `pygcap-0.0.1.tar` & `pygcap-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 07:36:08.459641 pygcap-0.0.1/
--rw-r--r--   0 jrim       (501) staff       (20)      613 2024-05-30 07:36:08.459372 pygcap-0.0.1/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)     2164 2024-05-30 05:44:23.000000 pygcap-0.0.1/README.md
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 07:36:08.457833 pygcap-0.0.1/pygcap/
--rw-r--r--   0 jrim       (501) staff       (20)      426 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    13289 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10046 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)     8060 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4297 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     6190 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6514 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)      507 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/cli.py
--rw-r--r--   0 jrim       (501) staff       (20)     6511 2024-05-30 05:44:23.000000 pygcap-0.0.1/pygcap/main.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 07:36:08.459146 pygcap-0.0.1/pygcap.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      613 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      479 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)       43 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/entry_points.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)       27 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-30 07:36:08.000000 pygcap-0.0.1/pygcap.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-30 07:36:08.459703 pygcap-0.0.1/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      934 2024-05-30 07:35:50.000000 pygcap-0.0.1/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 08:43:45.879644 pygcap-0.0.2/
+-rw-r--r--   0 jrim       (501) staff       (20)      613 2024-05-30 08:43:45.879426 pygcap-0.0.2/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)     3328 2024-05-30 08:39:56.000000 pygcap-0.0.2/README.md
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 08:43:45.878079 pygcap-0.0.2/pygcap/
+-rw-r--r--   0 jrim       (501) staff       (20)      425 2024-05-30 08:43:08.000000 pygcap-0.0.2/pygcap/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    13289 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10045 2024-05-30 08:39:56.000000 pygcap-0.0.2/pygcap/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     8060 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4296 2024-05-30 08:39:56.000000 pygcap-0.0.2/pygcap/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6190 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6514 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)      507 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/cli.py
+-rw-r--r--   0 jrim       (501) staff       (20)     6511 2024-05-30 05:44:23.000000 pygcap-0.0.2/pygcap/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-30 08:43:45.879210 pygcap-0.0.2/pygcap.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      613 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      479 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       43 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/entry_points.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)       27 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-30 08:43:45.000000 pygcap-0.0.2/pygcap.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-30 08:43:45.879702 pygcap-0.0.2/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      934 2024-05-30 08:43:01.000000 pygcap-0.0.2/setup.py
```

### Comparing `pygcap-0.0.1/PKG-INFO` & `pygcap-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygcap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for probe-based gene cluster finding in large microbial genome database
 Home-page: https://github.com/jrim42/pyGCAP
 Author: jsrim
 Author-email: comfortindex@naver.com
 Keywords: gene,cluster,genomics,bioinformatics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pygcap-0.0.1/pygcap/_accessory.py` & `pygcap-0.0.2/pygcap/_accessory.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_blast.py` & `pygcap-0.0.2/pygcap/_blast.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_cluster.py` & `pygcap-0.0.2/pygcap/_cluster.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_count.py` & `pygcap-0.0.2/pygcap/_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def count_blastp_result(project_info):
     output_dir = project_info['output']
 
     result_df = pd.read_csv(f"{project_info['seqlib']}/blast_output1.tsv", sep='\t')
     target_df = pd.read_csv(f"{project_info['data']}/metadata_target.tsv", sep='\t')
     assembly_df = pd.read_csv(f"{project_info['output']}/tsv/assembly_report_sum.tsv", sep='\t')
 
-    target = target_df['target name'].values.tolist()
+    target = target_df['Probe Name'].values.tolist()
     target2 = target_df['Prediction'].values.tolist()
 
     name = assembly_df['Organism Name'].values.tolist() 
     accession = assembly_df['Accession'].values.tolist() 
     
     new_df = pd.DataFrame({
         'accession': accession,
```

### Comparing `pygcap-0.0.1/pygcap/_parse.py` & `pygcap-0.0.2/pygcap/_parse.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_profile.py` & `pygcap-0.0.2/pygcap/_profile.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_search.py` & `pygcap-0.0.2/pygcap/_search.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_seqlib.py` & `pygcap-0.0.2/pygcap/_seqlib.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_target.py` & `pygcap-0.0.2/pygcap/_target.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 def save_fasta(df, filename):
     print("<< Processing target data into FASTA file...")
 
     with open(filename, "w") as file:
         for index, row in df.iterrows():
             if row['protein_id'] == '-' or pd.isna(row['protein_id']):
                 continue
-            header = f">{row['target name']} {row['protein_id']} [{row['organism_name']}]\n"
+            header = f">{row['Probe Name']} {row['protein_id']} [{row['organism_name']}]\n"
             sequence = str(row['sequence'])
             seq_lines = [sequence[i:i+50] for i in range(0, len(sequence), 50)]
             file.write(header)
             for line in seq_lines:
                 file.write(line + "\n")
 
 def process_target_data(project_info, target_original_path):
```

### Comparing `pygcap-0.0.1/pygcap/_utils.py` & `pygcap-0.0.2/pygcap/_utils.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/_visualize.py` & `pygcap-0.0.2/pygcap/_visualize.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap/main.py` & `pygcap-0.0.2/pygcap/main.py`

 * *Files identical despite different names*

### Comparing `pygcap-0.0.1/pygcap.egg-info/PKG-INFO` & `pygcap-0.0.2/pygcap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygcap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python package for probe-based gene cluster finding in large microbial genome database
 Home-page: https://github.com/jrim42/pyGCAP
 Author: jsrim
 Author-email: comfortindex@naver.com
 Keywords: gene,cluster,genomics,bioinformatics
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pygcap-0.0.1/setup.py` & `pygcap-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pygcap',
-    version='0.0.1',
+    version='0.0.2',
     description='Python package for probe-based gene cluster finding in large microbial genome database',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/pyGCAP',
     install_requires=['pandas', 'matplotlib', 'requests'],
     packages=find_packages(),
     keywords=['gene', 'cluster', 'genomics', 'bioinformatics'],
```

