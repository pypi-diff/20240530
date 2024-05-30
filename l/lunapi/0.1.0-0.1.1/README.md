# Comparing `tmp/lunapi-0.1.0-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/lunapi-0.1.1-pp310-pypy310_pp73-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,10 @@
-Zip file size: 10401563 bytes, number of entries: 12
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-28 03:22 lunapi-0.1.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-28 03:22 lunapi/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-28 03:22 lunapi.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-28 03:22 lunapi-0.1.0.dist-info/licenses/
--rw-rw-r--  2.0 unx      165 b- defN 24-May-28 03:22 lunapi-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx      641 b- defN 24-May-28 03:22 lunapi-0.1.0.dist-info/RECORD
--rw-rw-r--  2.0 unx     1398 b- defN 24-May-28 03:22 lunapi-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx    35149 b- defN 24-May-28 03:22 lunapi-0.1.0.dist-info/licenses/LICENSE
--rwxr-xr-x  2.0 unx 27481472 b- defN 24-May-28 03:22 lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      352 b- defN 24-May-28 03:22 lunapi/__init__.py
--rw-r--r--  2.0 unx    84522 b- defN 24-May-28 03:22 lunapi/lunapi1.py
--rw-r--r--  2.0 unx    12728 b- defN 24-May-28 03:22 lunapi/lunapi0.cpp
-12 files, 27616427 bytes uncompressed, 10400029 bytes compressed:  62.3%
+Zip file size: 6870490 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      352 b- defN 24-May-30 15:03 lunapi/__init__.py
+-rw-r--r--  2.0 unx    90993 b- defN 24-May-30 15:03 lunapi/lunapi1.py
+-rwxr-xr-x  2.0 unx 15173200 b- defN 24-May-30 15:03 lunapi/lunapi0.pypy310-pp73-darwin.so
+-rw-r--r--  2.0 unx    12728 b- defN 24-May-30 15:03 lunapi/lunapi0.cpp
+-rw-rw-r--  2.0 unx      632 b- defN 24-May-30 15:03 lunapi-0.1.1.dist-info/RECORD
+-rw-rw-r--  2.0 unx      120 b- defN 24-May-30 15:03 lunapi-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     1422 b- defN 24-May-30 15:03 lunapi-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx    35149 b- defN 24-May-30 15:03 lunapi-0.1.1.dist-info/licenses/LICENSE
+8 files, 15314596 bytes uncompressed, 6869426 bytes compressed:  55.1%
```

## zipnote {}

```diff
@@ -1,37 +1,25 @@
-Filename: lunapi-0.1.0.dist-info/
-Comment: 
-
-Filename: lunapi/
-Comment: 
-
-Filename: lunapi.libs/
-Comment: 
-
-Filename: lunapi-0.1.0.dist-info/licenses/
-Comment: 
-
-Filename: lunapi-0.1.0.dist-info/WHEEL
+Filename: lunapi/__init__.py
 Comment: 
 
-Filename: lunapi-0.1.0.dist-info/RECORD
+Filename: lunapi/lunapi1.py
 Comment: 
 
-Filename: lunapi-0.1.0.dist-info/METADATA
+Filename: lunapi/lunapi0.pypy310-pp73-darwin.so
 Comment: 
 
-Filename: lunapi-0.1.0.dist-info/licenses/LICENSE
+Filename: lunapi/lunapi0.cpp
 Comment: 
 
-Filename: lunapi/lunapi0.pypy39-pp73-x86_64-linux-gnu.so
+Filename: lunapi-0.1.1.dist-info/RECORD
 Comment: 
 
-Filename: lunapi/__init__.py
+Filename: lunapi-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: lunapi/lunapi1.py
+Filename: lunapi-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: lunapi/lunapi0.cpp
+Filename: lunapi-0.1.1.dist-info/licenses/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## lunapi/lunapi1.py

```diff
@@ -1,34 +1,43 @@
-"""lunapi1 module provides a high-level convenience wrapper around lunapi0 module functions."""
+"""lunapi1 module: a high-level wrapper around lunapi0 module functions"""
 
-# Luna Python wrapper
-# v0.1.0, 27-May-2024
+# Luna Python interface (lunapi)
+# v0.1.1, 30-May-2024
 
 import lunapi.lunapi0 as _luna
 
 import pandas as pd
 import numpy as np
 from scipy.stats.mstats import winsorize
-
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from IPython.core import display as ICD
 import plotly.graph_objects as go
 import plotly.express as px
 from ipywidgets import widgets, AppLayout
 from itertools import cycle
+import re
+import requests
+import io
+import tempfile
+import os
+import tempfile
+from ipywidgets import IntProgress
+from IPython.display import display
+import time
+import pathlib
 
 
 # resource set for Docker container version
 class resources:
    POPS_PATH = '/build/nsrr/common/resources/pops/'
    POPS_LIB = 's2'
    MODEL_PATH = '/build/luna-models/'
 
-lp_version = "v0.1.0"
+lp_version = "v0.1.1"
    
 # C++ singleton class (engine & sample list)
 # lunapi_t      --> luna
 
 # one observation
 # lunapi_inst_T --> inst
 
@@ -89,15 +98,15 @@
       ----------
       filename : str
           optional filename of a sample-list to read
 
       path : str
           optional path to preprend to the sample-list when reading (sets the 'path' variable)
 
-      df : boolean
+      df : bool
           if returning a sample-list, return as a Pandas dataframe
       
       Returns
       -------
       list
           a list of strings representing the sample-list (IDs, EDFs, annotations for each individual)
       """
@@ -602,18 +611,18 @@
       """Returns of dataframe of current annotations"""
       t = pd.DataFrame( self.edf.annots() )
       if len( t ) == 0: return t
       t.columns = ["Annotations"]
       return t
 
    #------------------------------------------------------------------------   
-   def fetch_annots( self , anns ):
+   def fetch_annots( self , anns , interp = -1 ):
       """Returns of dataframe of annotation events"""
       if type( anns ) is not list: anns = [ anns ]
-      t = pd.DataFrame( self.edf.fetch_annots( anns ) )
+      t = pd.DataFrame( self.edf.fetch_annots( anns , interp ) )
       if len( t ) == 0: return t
       t.columns = ['Class', 'Start', 'Stop' ]
       t = t.sort_values(by=['Start', 'Stop', 'Class'])
       t['Start'] = t['Start'].round(decimals=3)
       t['Stop'] = t['Stop'].round(decimals=3)
       return t
 
@@ -1072,44 +1081,44 @@
       if self.has_staging() is not True:
          print( "no staging attached" )
          return
       return hypno( self.stages()[ 'STAGE' ] )
 
    # --------------------------------------------------------------------------------
    def has_staging(self):
-      """Returns boolean for whether staging is present"""
+      """Returns bool for whether staging is present"""
       _proj = proj(False)
       silence_mode = _proj.is_silenced()
       _proj.silence(True,False)
       res = self.edf.has_staging()
       _proj.silence( silence_mode , False )
       return res
 
    # --------------------------------------------------------------------------------
    def has_annots(self,anns):
-      """Returns boolean for which annotations are present"""
+      """Returns bool for which annotations are present"""
       if anns is None: return
       if type( anns ) is not list: anns = [ anns ]
       return self.edf.has_annots( anns )
 
    # --------------------------------------------------------------------------------
    def has_annot(self,anns):
-      """Returns boolean for which annotations are present"""
+      """Returns bool for which annotations are present"""
       return self.has_annots(anns)
 
    # --------------------------------------------------------------------------------
    def has_channels(self,ch):
-      """Return a boolean to indicate whether a given channel exists"""
+      """Return a bool to indicate whether a given channel exists"""
       if ch is None: return
       if type(ch) is not list: ch = [ ch ]
       return self.edf.has_channels( ch )
 
    # --------------------------------------------------------------------------------
    def has(self,ch):
-      """Return a boolean to indicate whether a given channel exists"""
+      """Return a bool to indicate whether a given channel exists"""
       if ch is None: return
       if type(ch) is not list: ch = [ ch ]
       return self.edf.has_channels( ch )
 
    # --------------------------------------------------------------------------------                                                                  
    def spec(self,ch,mine = None , maxe = None , minf = None, maxf = None, w = 0.025 ):
       """PSD given channel 'ch'"""
@@ -1917,35 +1926,37 @@
 
     # --------------------- hypnogram-level summary
 
     stgs = [ 'N1' , 'N2' , 'N3' , 'R' , 'W' , '?' , 'L' ]
     stgcols = { 'N1':'rgba(32, 178, 218, 1)' , 'N2':'blue', 'N3':'navy','R':'red','W':'green','?':'gray','L':'yellow' }
     stgns = { 'N1':-1 , 'N2':-2, 'N3':-3,'R':0,'W':1,'?':2,'L':2 }
 
-    # clock-time stage info
-    stg_evts = p.fetch_annots( stgs ) 
+    # clock-time stage info (in units no larger than 30 seconds)
+    stg_evts = p.fetch_annots( stgs , 30 ) 
     if len( stg_evts ) != 0:
          stg_evts2 = stg_evts.copy()
          stg_evts2[ 'Start' ] = stg_evts2[ 'Stop' ]
+         stg_evts[ 'IDX' ] = range(len(stg_evts))
+         stg_evts2[ 'IDX' ] = range(len(stg_evts)) 
          stg_evts = pd.concat( [stg_evts2, stg_evts] )
-         stg_evts = stg_evts.sort_values(by=['Start', 'Class'])
+         stg_evts = stg_evts.sort_values(by=['Start', 'IDX'])
          times = stg_evts['Start'].to_numpy()    
          ys = [ stgns[c] for c in stg_evts['Class'].tolist() ]
          cols = [ stgcols[c] for c in stg_evts['Class'].tolist() ]
     else:
         times = None
         ys = None
         cols = None
         
     hypfig = [ go.Scatter( x = times, y=ys, mode='lines', line=dict(color='gray')) ]  
     
     hypfig.append( go.Scatter(x = times, 
                               y = ys , 
                               mode = 'markers' , 
-                              marker=dict( color = cols , size=2),
+                              marker=dict( color = cols , size=2),                              
                               hoverinfo='none' )  )
     
     hyplayout =  go.Layout( margin=dict(l=8, r=8, t=0, b=0),
                             showlegend=False,
                             xaxis=dict(range=[0,nsecs_clk]),
                             yaxis=dict(range=[-4,3]),
                             yaxis_visible=False, 
@@ -2264,8 +2275,165 @@
     # ---------------------  display
     update_bandpower(None)
     ss.set_scaling( len(chbox.value) , len( anbox.value) , 2**float(yscale.value) , float(yspace.value) , header_height, footer_height , annot_height )
 
     return container_app
 
 
-   
+# --------------------------------------------------------------------------------
+# moonbeam
+
+class moonbeam:
+   """Moonbeam utility to pull NSRR data"""
+
+   df1 = None  # available cohorts
+   df2 = None  # available files for current cohort
+   curr_cohort = None
+   
+   def __init__(self, nsrr_tok , cdir = None ):
+      """ Initiate Moonbeam with an NSRR token """
+      self.nsrr_tok = nsrr_tok
+      self.df1 = self.cohorts()
+      if cdir is None: cdir = os.path.join( tempfile.gettempdir() , 'luna-mmonbeam' )
+      self.set_cache(cdir)
+
+   def set_cache(self,cdir):
+      """ Set the folder for caching downloaded records """
+      self.cdir = cdir
+      print( 'using cache folder for downloads: ' + self.cdir )
+      os.makedirs( os.path.dirname(self.cdir), exist_ok=True)
+
+   def cached(self,file):
+      """ Check whether a file is already cached """ 
+      return os.path.exists( os.path.join( self.cdir , file ) )
+
+   def cohorts(self):
+      """ List all available cohorts accessible from the given NSRR user token """ 
+      req = requests.get( 'https://zzz.bwh.harvard.edu/cgi-bin/moonbeam.cgi?t=' + self.nsrr_tok ).content
+      self.df1 = pd.read_csv(io.StringIO(req.decode('utf-8')),sep='\t',header=None)
+      self.df1.columns = ['Cohort','Description']
+      return self.df1
+
+   def cohort(self,cohort1):
+      """ List all files (EDFs and annotations) available for a given cohort """
+      if type(cohort1) is int: cohort1 = self.df1.loc[cohort1,'Cohort']
+      if type(cohort1) is not str: return
+      self.curr_cohort = cohort1
+      req = requests.get( 'https://zzz.bwh.harvard.edu/cgi-bin/moonbeam.cgi?t=' + self.nsrr_tok + "&c=" + cohort1).content
+      df = pd.read_csv(io.StringIO(req.decode('utf-8')),sep='\t',header=None)
+      df.columns = [ 'cohort' , 'IID' , 'file' ]
+
+      #  get EDFs, annots then merge
+      df_edfs = df[ df['file'].str.contains(".edf$|.edf.gz$" , case = False ) ][[ 'IID' , 'file' ]]
+      df_annots = df[ ~ df['file'].str.contains(".edf$|.edf.gz$" , case = False ) ][[ 'IID' , 'file' ]]
+      self.df2 = pd.merge( df_edfs , df_annots , on='IID' , how='left' )
+      self.df2.columns = [ 'ID' , 'EDF' , 'Annot' ]
+      return self.df2
+
+   
+   def inst(self, iid, cohort = None ):
+      """ Create an instance of a record, either downloaded or cached """    
+      if self.df2 is None: return
+      if self.curr_cohort is None: return
+      
+      # ensure we have this file 
+      self.pull( iid , cohort )
+
+      # initiate an instance (from singleton proj)
+      proj1 = proj()
+      p = proj1.inst( self.curr_id )
+
+      edf1 = str( pathlib.Path( self.cdir ).joinpath( self.curr_edf ).expanduser().resolve() )      
+      p.attach_edf( edf1 ) 
+
+      if self.curr_annot is not None:
+         annot1 = str( pathlib.Path( self.cdir ).joinpath( self.curr_annot ).expanduser().resolve() )
+         p.attach_annot( annot1 )
+
+      # return handle back
+      return p
+
+    
+   def pull(self, iid , cohort = None ):
+      """ Download an individual record (if not already cached) """    
+      if cohort is None and self.df2.empty: return False
+      if self.df2.empty: files( cohort )
+      if self.df2.empty: return False
+
+      # iid
+      if type(iid) is int: iid = self.df2.loc[iid,'ID']
+      self.curr_id = iid
+
+      # EDF
+      self.curr_edf = self.df2.loc[ self.df2['ID'] == iid,'EDF'].item()
+      self.pull_file( self.curr_edf )
+
+      # EDFZ .idx
+      if re.search('\.edf\.gz$',self.curr_edf,re.IGNORECASE) or re.search('\.edfz$',self.curr_edf,re.IGNORECASE):
+         self.pull_file( self.curr_edf + '.idx' )
+
+      # annots (optional)
+      self.curr_annot = self.df2.loc[ self.df2['ID'] == iid,'Annot'].item()
+      if self.curr_annot is not None:
+         self.pull_file( self.curr_annot )
+
+   def pull_file( self , file ):
+      import functools
+      import pathlib
+      import shutil
+      import requests
+      from tqdm.auto import tqdm
+
+      if self.cached( file ) is True: 
+          print( file + ' is already cached' )
+          return
+
+      # save file to cdir/{path/}file, e.g. path will be cohort
+      path = pathlib.Path( self.cdir ).joinpath( file ).expanduser().resolve() 
+      path.parent.mkdir(parents=True, exist_ok=True)
+
+      print( '\nbeaming ' + self.curr_id + ' : ' + file  )
+
+      url = 'https://zzz.bwh.harvard.edu/cgi-bin/moonbeam.cgi?t=' + self.nsrr_tok + "&f=" + file    
+      r = requests.get(url, stream=True, allow_redirects=True)
+
+      if r.status_code != 200:
+         r.raise_for_status()  # Will only raise for 4xx codes, so...
+         raise RuntimeError(f"Request to {url} returned status code {r.status_code}")
+      file_size = int(r.headers.get('Content-Length', 0))
+
+      desc = "(Unknown total file size)" if file_size == 0 else ""
+      r.raw.read = functools.partial(r.raw.read, decode_content=True)  # Decompress if needed
+      with tqdm.wrapattr(r.raw, "read", total=file_size, desc=desc) as r_raw:
+          with path.open("wb") as f:
+              shutil.copyfileobj(r_raw, f)
+
+
+   def pheno(self, cohort = None, iid = None):
+      """ Pull phenotypes for a given individual """
+
+      coh1 = cohort
+      id1 = iid
+
+      if coh1 is None:
+         if self.curr_cohort is None: return
+         coh1 = self.curr_cohort
+         
+      if id1 is None:
+         if self.curr_id is None: return
+         id1 = self.curr_id
+            
+      url = 'https://zzz.bwh.harvard.edu/cgi-bin/moonbeam.cgi?t=' + self.nsrr_tok + '&c=' + self.curr_cohort + '&p=' + id1 
+      req = requests.get( url )
+
+      if req.status_code != 200:
+         req.raise_for_status()  # Will only raise for 4xx codes, so...
+         raise RuntimeError(f"Moonbeam returned status code {req.status_code}")
+      
+      df = pd.read_csv(io.StringIO(req.content.decode('utf-8')),sep='\t',header=None)
+      df.columns = ['Variable', 'Value', 'Units', 'Description' ]
+      pri = [ "nsrr_age", "nsrr_sex", "nsrr_bmi", "nsrr_flag_spsw", "nsrr_ahi_hp3r_aasm15", "nsrr_ahi_hp4u_aasm15" ] 
+      df1 = df[   df['Variable'].isin( pri ) ]
+      df2 = df[ ~ df['Variable'].isin( pri ) ] 
+      df = pd.concat( [ df1 , df2 ] )
+      return df
+
```

## Comparing `lunapi-0.1.0.dist-info/METADATA` & `lunapi-0.1.1.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lunapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python interface to the Luna toolset for sleep signal analysis
 Keywords: Sleep,EEG,PSG,Luna,Signal processing
 Author-Email: Shaun Purcell <smpurcell@bwh.harvard.edu>, Senthil Palanivelu <spalanivelu@mgh.harvard.edu>, Nataliia Kozhemiako <nkozhemiako@bwh.harvard.edu>
 Maintainer-Email: Senthil Palanivelu <spalanivelu@mgh.harvard.edu>
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
@@ -21,14 +21,15 @@
 Project-URL: Github, http://github.com/remnrem/luna-api
 Requires-Python: >=3.9
 Requires-Dist: matplotlib
 Requires-Dist: pandas
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: plotly
+Requires-Dist: nbformat
 Requires-Dist: ipywidgets
 Requires-Dist: IPython
 Description-Content-Type: text/markdown
 
 # lunapi
 
 Python bindings for C/C++ Luna library
```

## Comparing `lunapi-0.1.0.dist-info/licenses/LICENSE` & `lunapi-0.1.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

