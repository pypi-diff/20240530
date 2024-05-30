# Comparing `tmp/ds20kdb_avt-1.0.8.tar.gz` & `tmp/ds20kdb_avt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ds20kdb_avt-1.0.8.tar", last modified: Sat Apr 13 18:03:13 2024, max compression
+gzip compressed data, was "ds20kdb_avt-1.0.9.tar", last modified: Sun Apr 14 11:04:22 2024, max compression
```

## Comparing `ds20kdb_avt-1.0.8.tar` & `ds20kdb_avt-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 18:03:13.694486 ds20kdb_avt-1.0.8/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.8/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 18:03:13.693480 ds20kdb_avt-1.0.8/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb_avt-1.0.8/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.8/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-13 18:03:13.694683 ds20kdb_avt-1.0.8/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-13 18:00:27.000000 ds20kdb_avt-1.0.8/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 18:03:13.666029 ds20kdb_avt-1.0.8/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 18:03:13.686520 ds20kdb_avt-1.0.8/src/ds20kdb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.8/src/ds20kdb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb_avt-1.0.8/src/ds20kdb/auth.py
--rw-r--r--   0 avt        (501) staff       (20)    38424 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.8/src/ds20kdb/common.py
--rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb/constants.py
--rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.8/src/ds20kdb/create_credentials_file.py
--rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb_avt-1.0.8/src/ds20kdb/gen_tray_files_gui.py
--rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb_avt-1.0.8/src/ds20kdb/interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb_avt-1.0.8/src/ds20kdb/qr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb_avt-1.0.8/src/ds20kdb/qrgen.py
--rwxr-xr-x   0 avt        (501) staff       (20)    32509 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.8/src/ds20kdb/scanner_auto.py
--rwxr-xr-x   0 avt        (501) staff       (20)   120367 2024-04-13 18:00:15.000000 ds20kdb_avt-1.0.8/src/ds20kdb/submit_vtile.py
--rwxr-xr-x   0 avt        (501) staff       (20)    22398 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.8/src/ds20kdb/submit_vtile_json.py
--rwxr-xr-x   0 avt        (501) staff       (20)    11674 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.8/src/ds20kdb/veto_location.py
--rwxr-xr-x   0 avt        (501) staff       (20)    19987 2024-03-21 17:12:00.000000 ds20kdb_avt-1.0.8/src/ds20kdb/veto_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb_avt-1.0.8/src/ds20kdb/visual.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb_avt-1.0.8/src/ds20kdb/vtile_test_submit_cr.py
--rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb_avt-1.0.8/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
--rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb_avt-1.0.8/src/ds20kdb/wafer_location_gui.py
--rwxr-xr-x   0 avt        (501) staff       (20)    24651 2024-02-29 13:53:11.000000 ds20kdb_avt-1.0.8/src/ds20kdb/wafer_map_from_db.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-13 18:03:13.692181 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-13 18:03:13.000000 ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-14 11:04:22.487091 ds20kdb_avt-1.0.9/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.9/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-14 11:04:22.486307 ds20kdb_avt-1.0.9/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     5281 2023-10-13 14:30:24.000000 ds20kdb_avt-1.0.9/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.9/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2024-04-14 11:04:22.487264 ds20kdb_avt-1.0.9/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     3208 2024-04-14 11:04:06.000000 ds20kdb_avt-1.0.9/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-14 11:04:22.453578 ds20kdb_avt-1.0.9/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-14 11:04:22.480836 ds20kdb_avt-1.0.9/src/ds20kdb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.9/src/ds20kdb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)     9414 2023-09-17 11:41:52.000000 ds20kdb_avt-1.0.9/src/ds20kdb/auth.py
+-rw-r--r--   0 avt        (501) staff       (20)    38425 2024-04-14 09:30:46.000000 ds20kdb_avt-1.0.9/src/ds20kdb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)      182 2023-04-01 13:34:13.000000 ds20kdb_avt-1.0.9/src/ds20kdb/constants.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     2123 2023-02-09 15:44:46.000000 ds20kdb_avt-1.0.9/src/ds20kdb/create_credentials_file.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    35945 2024-04-10 17:47:51.000000 ds20kdb_avt-1.0.9/src/ds20kdb/gen_tray_files_gui.py
+-rw-r--r--   0 avt        (501) staff       (20)    93425 2024-04-13 12:39:23.000000 ds20kdb_avt-1.0.9/src/ds20kdb/interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6936 2023-09-06 15:42:42.000000 ds20kdb_avt-1.0.9/src/ds20kdb/qr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7876 2023-09-09 12:18:43.000000 ds20kdb_avt-1.0.9/src/ds20kdb/qrgen.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    32494 2024-04-14 10:18:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb/scanner_auto.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   120404 2024-04-14 10:21:41.000000 ds20kdb_avt-1.0.9/src/ds20kdb/submit_vtile.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    22397 2024-04-14 09:22:10.000000 ds20kdb_avt-1.0.9/src/ds20kdb/submit_vtile_json.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    11400 2024-04-14 10:24:43.000000 ds20kdb_avt-1.0.9/src/ds20kdb/veto_location.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    19946 2024-04-14 10:19:43.000000 ds20kdb_avt-1.0.9/src/ds20kdb/veto_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14551 2024-01-10 17:21:38.000000 ds20kdb_avt-1.0.9/src/ds20kdb/visual.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9030 2024-04-12 15:27:49.000000 ds20kdb_avt-1.0.9/src/ds20kdb/vtile_test_submit_cr.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     8222 2024-03-31 13:35:23.000000 ds20kdb_avt-1.0.9/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py
+-rwx------   0 avt        (501) staff       (20)    10441 2023-12-09 19:41:04.000000 ds20kdb_avt-1.0.9/src/ds20kdb/wafer_location_gui.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     6366 2024-04-14 11:00:08.000000 ds20kdb_avt-1.0.9/src/ds20kdb/wafer_map_from_db.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2024-04-14 11:04:22.485694 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     6889 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      830 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      868 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      111 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        8 2024-04-14 11:04:22.000000 ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/top_level.txt
```

### Comparing `ds20kdb_avt-1.0.8/PKG-INFO` & `ds20kdb_avt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.8
+Version: 1.0.9
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb_avt-1.0.8/README.md` & `ds20kdb_avt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/setup.py` & `ds20kdb_avt-1.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="ds20kdb-avt",
-    version="1.0.8",
+    version="1.0.9",
     author="Alan Taylor, Paolo Franchini, Seraphim Koulosousas",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="A cross-platform Python interface to the DarkSide-20k production database",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/auth.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/auth.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/common.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,15 +424,15 @@
 class SiPMCheck:
     """
     Class of functions to check a sipm test values against the NOA test
     distributions.
     """
     def __init__(self, dbi):
         """
-        loading the database separetely to allow the following functions to be
+        loading the database separately to allow the following functions to be
         able to loop over multiple sipms. If more tables are needed can
         thread the loading and save in a list
         """
         self.dbi = dbi
         self.df_sipm_qc = self.dbi.get('sipm_test').data
 
         # Get Latest QA/QC criteria
@@ -883,15 +883,15 @@
     We will not create a new file from the data already held in memory, since
     this will remove any comments/formatting that the user may have made.
     Since the files are tiny, read it into memory, modify just the lines that
     need to change, and overwrite the file.
 
     Existing SiPM entries may be present, or missing altogether.
 
-    If the file contains any broken lines they will be propogated into the
+    If the file contains any broken lines they will be propagated into the
     new file.
 
     Try to make minimal changes to the file, to avoid creating confusing
     commit diffs.
 
     --------------------------------------------------------------------------
     args
@@ -990,15 +990,15 @@
         lot : int
         wafer_number : int
     --------------------------------------------------------------------------
     returns : none
         external file amended
     --------------------------------------------------------------------------
     """
-    sipm_type, existing_tray_files, new_sipms = var
+    _sipm_type, existing_tray_files, new_sipms = var
 
     lines_for_all_files = []
     for filename, (_contents, missing_sipms) in existing_tray_files.items():
 
         sipm_allocation = []
         for _ in itertools.repeat(None, len(missing_sipms)):
             try:
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/create_credentials_file.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/create_credentials_file.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/gen_tray_files_gui.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/gen_tray_files_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/interface.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/interface.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/qr.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/qr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/qrgen.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/qrgen.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/scanner_auto.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/scanner_auto.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             'optical_inspection': self.optical_inspection,
             'configuration': self.configuration,
             'institute_id': self.institute_id,
         }
 
         self.table = lut[self.component](table_common)
 
-        return False if self.table is None else True
+        return self.table is not None
 
     def table_vtile(self, table_common):
         """
         Build the table to suit measurement: vtile_test.
 
         ----------------------------------------------------------------------
         args
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/submit_vtile.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/submit_vtile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1592,15 +1592,15 @@
 
     def generic_load_json(self, filename):
         """
         Load JSON file.
 
         ----------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
             filename : string
         ----------------------------------------------------------------------
         returns
             table_json : dict
                 e.g. {
                     'sipm_19|lot_number': '9262109',
@@ -1647,15 +1647,15 @@
     def save_file(self, filename):
         """
         Save file with a time-stamped filename containing the values from all
         drop-down menus.
 
         ----------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
             filename : string
         ----------------------------------------------------------------------
         returns : none
             file written to mass storage
         ----------------------------------------------------------------------
         """
@@ -1691,15 +1691,15 @@
         """
         Save file with a time-stamped filename.
 
         --------------------------------------------------------------------------
         args
             session_timestamp : string
                 e.g. '20221119_144629'
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
         --------------------------------------------------------------------------
         returns : none
             file written to mass storage
         --------------------------------------------------------------------------
         """
         suggested_filename = f'{self.session_timestamp}_post_vtile.json'
@@ -1992,14 +1992,17 @@
         sid = syringe['syringe_id']
         try:
             int(sid)
         except (TypeError, ValueError):
             self.print_to_console(f'solder syringe syringe_id incorrect: {sid}')
             return
 
+        if fail:
+            return
+
         post_successful = self.dbi.post_solder(syringe)
 
         # get solder id for the last syringe submitted
         solder_id = int(
             self.dbi.get(
                 'solder',
                 institute_id=syringe['institute_id']
@@ -2383,15 +2386,15 @@
     def clear_gui(self):
         """
         Return all drop-down menus and labels to their default state, discarding
         all user-entered information. Disable the submit button.
 
         --------------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
         --------------------------------------------------------------------------
         returns : none
             GUI state affected
         --------------------------------------------------------------------------
         """
         for widget in self.widgets:
@@ -2404,15 +2407,15 @@
 
     def clear_gui_load_defaults(self):
         """
         Return the GUI state to that set at application start.
 
         --------------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
             defaults_file_path : string
                 e.g. '/Users/avt/.ds20kdb_defaults'
         --------------------------------------------------------------------------
         returns : none
             GUI state affected
         --------------------------------------------------------------------------
@@ -2423,15 +2426,15 @@
     def clear_gui_sipms_only(self):
         """
         Return all SiPM drop-down menus and labels to their default state,
         discarding all user-entered information.
 
         ----------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
         ----------------------------------------------------------------------
         returns : none
             GUI state affected
         ----------------------------------------------------------------------
         """
 
@@ -2441,15 +2444,15 @@
 
     def clear_submit_button(self):
         """
         Disable the submit button.
 
         ----------------------------------------------------------------------
         args
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
         ----------------------------------------------------------------------
         returns : none
             GUI state affected
         ----------------------------------------------------------------------
         """
         for widget in self.widgets:
@@ -2761,15 +2764,15 @@
                     e.g.
                         {
                             'year': {'label': tk.Label, 'year': '2022'},
                             'month': {'label': tk.Label, 'month': '12'},
                             ...
                         }
                 Contains user-entered values from date/time related comboboxes.
-            widgets : list of class Widgit
+            widgets : list of class Widget
                 Contains details of GUI widgets.
             table : dict
         ----------------------------------------------------------------------
         returns
             table : dict
                 no explicit return, mutable type amended in place
         ----------------------------------------------------------------------
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/submit_vtile_json.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/submit_vtile_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -409,15 +409,15 @@
 
             # Issue warning if this SiPM is not production standard.
             #
             # This check should have been done upstream, given that the data
             # from NOA/LFoundry in the database (electrical/visual testing)
             # should prevent suspect devices being represented in a wafer
             # map, so they should never be picked for production use. At this
-            # time - in December 2023 - there is the slim possibiility that a
+            # time - in December 2023 - there is the slim possibility that a
             # problematic device was incorrectly marked as good on a wafer
             # map. Really, it's too late at this point, since the vTile has
             # already had SiPMs bonded to it, so the best that can be done is
             # to warn the user that the vTile may be suspect.
 
             dfr_tmp = dbi.get('sipm_test', sipm_id=sipm_pid).data
             columns = ['classification', 'quality_flag', 'sipm_qc_id']
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/veto_location.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/veto_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,20 +70,15 @@
 
     return response.data
 
 
 def check_qrcode(qrcode):
     """
     Check whether the QR code supplied is formatted correctly. No check is
-    made to confirm its existance in the database.
-
-    No attempt is made to sort the returned items by QR code or serial number,
-    since the order isn't important and the ID sequence is unlikely to be
-    fully sequential anyway. The non-sequential order is due to the order
-    PCBs were QR-coded and processed.
+    made to confirm its existence in the database.
     """
     if not interface.qr_code_valid(qrcode):
         raise argparse.ArgumentTypeError(f'{qrcode}: invalid QR-code')
 
     return qrcode
 
 
@@ -353,15 +348,15 @@
     status with the date and time the script is run.
     """
     status = types.SimpleNamespace(success=0, unreserved_error_code=3)
     dbi = interface.Database()
 
     args = check_arguments(dbi)
 
-    # need to explicitly create the list so all submissions are processed
+    # explicitly create the list so all submissions are processed
     success = all(
         [
             Object(dbi, args, qrcode).submit_command()
             for qrcode in args.qrcode
         ]
     )
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/veto_location_gui.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/veto_location_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 Output: history of the object and post on the DB object>_location table
 
 ---
 
 Author: P.Franchini - p.franchini@lancaster.ac.uk
 """
 
-import contextlib
 import datetime
 import itertools
 import platform
 import sys
 import tkinter as tk
 from tkinter import ttk
 from tkinter import scrolledtext
@@ -244,23 +243,25 @@
 
         Windows 10:
         send_event=True state=Control keysym=v keycode=86 char='\x16'
         """
         if self.system == 'Darwin':
             # macOS Ventura 13.6.5
             return event.keycode == 17 and event.state == 16
-        elif self.system == 'Linux':
+
+        if self.system == 'Linux':
             # Pop!_OS 22.04 LTS x86_64 + Debian GNU/Linux 12 (bookworm) aarch64
             return event.keycode == 55 and event.state == 20
-        elif self.system == 'Windows':
+
+        if self.system == 'Windows':
             # MWS Windows 10
             return event.keycode == 17 and event.state == 16
-        else:
-            # ASSUME anything else is related to Linux
-            return event.keycode == 55 and event.state == 20
+
+        # ASSUME anything else is related to Linux
+        return event.keycode == 55 and event.state == 20
 
     @staticmethod
     def is_valid_date_format(input_string):
         """
         Dates supplied from tkcalendar.Calendar will be valid and in the
         correct format. The GUI also supports manually entered dates, so we
         have to detect plausible-looking but invalid entries such as
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/visual.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/visual.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/vtile_test_submit_cr.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/vtile_test_submit_cr.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/wafer_heat_map_from_vtile_qrcodes.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb/wafer_location_gui.py` & `ds20kdb_avt-1.0.9/src/ds20kdb/wafer_location_gui.py`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/PKG-INFO` & `ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ds20kdb-avt
-Version: 1.0.8
+Version: 1.0.9
 Summary: A cross-platform Python interface to the DarkSide-20k production database
 Home-page: https://gitlab.in2p3.fr/darkside/productiondb_software/
 Author: Alan Taylor, Paolo Franchini, Seraphim Koulosousas
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/SOURCES.txt` & `ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ds20kdb_avt-1.0.8/src/ds20kdb_avt.egg-info/entry_points.txt` & `ds20kdb_avt-1.0.9/src/ds20kdb_avt.egg-info/entry_points.txt`

 * *Files identical despite different names*

