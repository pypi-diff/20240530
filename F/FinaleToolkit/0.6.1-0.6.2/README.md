# Comparing `tmp/finaletoolkit-0.6.1.tar.gz` & `tmp/finaletoolkit-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finaletoolkit-0.6.1.tar", last modified: Mon May 27 03:35:36 2024, max compression
+gzip compressed data, was "finaletoolkit-0.6.2.tar", last modified: Thu May 30 16:36:55 2024, max compression
```

## Comparing `finaletoolkit-0.6.1.tar` & `finaletoolkit-0.6.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.806887 finaletoolkit-0.6.1/
--rw-r--r--   0 jamesli    (501) staff       (20)     1067 2024-04-01 19:28:48.000000 finaletoolkit-0.6.1/LICENSE
--rw-r--r--   0 jamesli    (501) staff       (20)     5548 2024-05-27 03:35:36.806670 finaletoolkit-0.6.1/PKG-INFO
--rw-r--r--   0 jamesli    (501) staff       (20)     2965 2024-05-23 03:36:53.000000 finaletoolkit-0.6.1/README.md
--rw-r--r--   0 jamesli    (501) staff       (20)     1595 2024-05-27 03:35:23.000000 finaletoolkit-0.6.1/pyproject.toml
--rw-r--r--   0 jamesli    (501) staff       (20)       38 2024-05-27 03:35:36.806925 finaletoolkit-0.6.1/setup.cfg
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.793733 finaletoolkit-0.6.1/src/
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.806399 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/
--rw-r--r--   0 jamesli    (501) staff       (20)     5548 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/PKG-INFO
--rw-r--r--   0 jamesli    (501) staff       (20)     1154 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/SOURCES.txt
--rw-r--r--   0 jamesli    (501) staff       (20)        1 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/dependency_links.txt
--rw-r--r--   0 jamesli    (501) staff       (20)       61 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/entry_points.txt
--rw-r--r--   0 jamesli    (501) staff       (20)       81 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/requires.txt
--rw-r--r--   0 jamesli    (501) staff       (20)       14 2024-05-27 03:35:36.000000 finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/top_level.txt
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.798442 finaletoolkit-0.6.1/src/finaletoolkit/
--rw-r--r--   0 jamesli    (501) staff       (20)      147 2024-05-27 03:32:46.000000 finaletoolkit-0.6.1/src/finaletoolkit/__init__.py
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.798869 finaletoolkit-0.6.1/src/finaletoolkit/cli/
--rw-r--r--   0 jamesli    (501) staff       (20)       40 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/cli/__init__.py
--rw-r--r--   0 jamesli    (501) staff       (20)    21973 2024-05-27 03:34:10.000000 finaletoolkit-0.6.1/src/finaletoolkit/cli/main_cli.py
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.802789 finaletoolkit-0.6.1/src/finaletoolkit/frag/
--rw-r--r--   0 jamesli    (501) staff       (20)      547 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/__init__.py
--rw-r--r--   0 jamesli    (501) staff       (20)     9719 2024-05-23 03:36:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/adjust_wps.py
--rw-r--r--   0 jamesli    (501) staff       (20)    10071 2024-05-23 03:36:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/cleavage_profile.py
--rw-r--r--   0 jamesli    (501) staff       (20)     9042 2024-05-23 03:36:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/coverage.py
--rw-r--r--   0 jamesli    (501) staff       (20)    14535 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi.py
--rw-r--r--   0 jamesli    (501) staff       (20)     3973 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi_gc_correct.py
--rw-r--r--   0 jamesli    (501) staff       (20)     2516 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi_merge_bins.py
--rw-r--r--   0 jamesli    (501) staff       (20)    30236 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/end_motifs.py
--rw-r--r--   0 jamesli    (501) staff       (20)    14835 2024-05-26 21:27:44.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/frag_length.py
--rw-r--r--   0 jamesli    (501) staff       (20)     8468 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/multi_wps.py
--rw-r--r--   0 jamesli    (501) staff       (20)     6568 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/frag/wps.py
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.803325 finaletoolkit-0.6.1/src/finaletoolkit/genome/
--rw-r--r--   0 jamesli    (501) staff       (20)       39 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/genome/__init__.py
--rw-r--r--   0 jamesli    (501) staff       (20)    15032 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/genome/gaps.py
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.804667 finaletoolkit-0.6.1/src/finaletoolkit/utils/
--rw-r--r--   0 jamesli    (501) staff       (20)      139 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/utils/__init__.py
--rw-r--r--   0 jamesli    (501) staff       (20)     4889 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/utils/agg_bw.py
--rw-r--r--   0 jamesli    (501) staff       (20)     1649 2024-05-14 20:16:53.000000 finaletoolkit-0.6.1/src/finaletoolkit/utils/cli_hist.py
--rw-r--r--   0 jamesli    (501) staff       (20)     3119 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/utils/filter_bam.py
--rw-r--r--   0 jamesli    (501) staff       (20)    19501 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/src/finaletoolkit/utils/utils.py
-drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-27 03:35:36.806138 finaletoolkit-0.6.1/tests/
--rw-r--r--   0 jamesli    (501) staff       (20)      742 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/tests/test_cleavage_profile.py
--rw-r--r--   0 jamesli    (501) staff       (20)     2324 2024-05-18 04:54:35.000000 finaletoolkit-0.6.1/tests/test_cli_entry.py
--rw-r--r--   0 jamesli    (501) staff       (20)     9163 2024-05-18 04:54:35.000000 finaletoolkit-0.6.1/tests/test_end_motifs.py
--rw-r--r--   0 jamesli    (501) staff       (20)     3601 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/tests/test_frag_io.py
--rw-r--r--   0 jamesli    (501) staff       (20)      718 2024-05-26 21:27:09.000000 finaletoolkit-0.6.1/tests/test_wps.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.068897 finaletoolkit-0.6.2/
+-rw-r--r--   0 jamesli    (501) staff       (20)     1067 2024-04-01 19:28:48.000000 finaletoolkit-0.6.2/LICENSE
+-rw-r--r--   0 jamesli    (501) staff       (20)     5548 2024-05-30 16:36:55.068704 finaletoolkit-0.6.2/PKG-INFO
+-rw-r--r--   0 jamesli    (501) staff       (20)     2965 2024-05-23 03:36:53.000000 finaletoolkit-0.6.2/README.md
+-rw-r--r--   0 jamesli    (501) staff       (20)     1595 2024-05-27 03:35:23.000000 finaletoolkit-0.6.2/pyproject.toml
+-rw-r--r--   0 jamesli    (501) staff       (20)       38 2024-05-30 16:36:55.068935 finaletoolkit-0.6.2/setup.cfg
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.058769 finaletoolkit-0.6.2/src/
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.068351 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/
+-rw-r--r--   0 jamesli    (501) staff       (20)     5548 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/PKG-INFO
+-rw-r--r--   0 jamesli    (501) staff       (20)     1177 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)        1 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       61 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/entry_points.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       81 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/requires.txt
+-rw-r--r--   0 jamesli    (501) staff       (20)       14 2024-05-30 16:36:55.000000 finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/top_level.txt
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.060560 finaletoolkit-0.6.2/src/finaletoolkit/
+-rw-r--r--   0 jamesli    (501) staff       (20)      147 2024-05-30 16:36:25.000000 finaletoolkit-0.6.2/src/finaletoolkit/__init__.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.060970 finaletoolkit-0.6.2/src/finaletoolkit/cli/
+-rw-r--r--   0 jamesli    (501) staff       (20)       40 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/cli/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    21973 2024-05-27 03:34:10.000000 finaletoolkit-0.6.2/src/finaletoolkit/cli/main_cli.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.064234 finaletoolkit-0.6.2/src/finaletoolkit/frag/
+-rw-r--r--   0 jamesli    (501) staff       (20)      547 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9719 2024-05-23 03:36:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/adjust_wps.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    10071 2024-05-23 03:36:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/cleavage_profile.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9042 2024-05-23 03:36:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/coverage.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    14535 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3973 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi_gc_correct.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     2516 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi_merge_bins.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    30236 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/end_motifs.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    14835 2024-05-26 21:27:44.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/frag_length.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     8468 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/multi_wps.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     6568 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/src/finaletoolkit/frag/wps.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.065029 finaletoolkit-0.6.2/src/finaletoolkit/genome/
+-rw-r--r--   0 jamesli    (501) staff       (20)       39 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/genome/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    15032 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/src/finaletoolkit/genome/gaps.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.066426 finaletoolkit-0.6.2/src/finaletoolkit/utils/
+-rw-r--r--   0 jamesli    (501) staff       (20)      139 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/utils/__init__.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     4889 2024-05-30 16:14:41.000000 finaletoolkit-0.6.2/src/finaletoolkit/utils/agg_bw.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     1649 2024-05-14 20:16:53.000000 finaletoolkit-0.6.2/src/finaletoolkit/utils/cli_hist.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3119 2024-05-27 04:02:12.000000 finaletoolkit-0.6.2/src/finaletoolkit/utils/filter_bam.py
+-rw-r--r--   0 jamesli    (501) staff       (20)    20075 2024-05-30 16:14:41.000000 finaletoolkit-0.6.2/src/finaletoolkit/utils/utils.py
+drwxr-xr-x   0 jamesli    (501) staff       (20)        0 2024-05-30 16:36:55.068098 finaletoolkit-0.6.2/tests/
+-rw-r--r--   0 jamesli    (501) staff       (20)      742 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/tests/test_cleavage_profile.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     2324 2024-05-18 04:54:35.000000 finaletoolkit-0.6.2/tests/test_cli_entry.py
+-rw-r--r--   0 jamesli    (501) staff       (20)      602 2024-05-30 16:32:11.000000 finaletoolkit-0.6.2/tests/test_coverage.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     9163 2024-05-18 04:54:35.000000 finaletoolkit-0.6.2/tests/test_end_motifs.py
+-rw-r--r--   0 jamesli    (501) staff       (20)     3601 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/tests/test_frag_io.py
+-rw-r--r--   0 jamesli    (501) staff       (20)      718 2024-05-26 21:27:09.000000 finaletoolkit-0.6.2/tests/test_wps.py
```

### Comparing `finaletoolkit-0.6.1/LICENSE` & `finaletoolkit-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/PKG-INFO` & `finaletoolkit-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: FinaleToolkit is a package and standalone program to extract fragmentation features of cell-free DNA from paired-end sequencing data.
 Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hzhe9oxg_/tmp5afcr6c0_TarContainer/0/2", line 54, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FinaleToolkit Version: 0.6.1 Summary: FinaleToolkit
+Metadata-Version: 2.1 Name: FinaleToolkit Version: 0.6.2 Summary: FinaleToolkit
 is a package and standalone program to extract fragmentation features of cell-
 free DNA from paired-end sequencing data. Author-email: James Li
 wfu.edu>, Ravi Bandaru
 northwestern.edu>, Yaping Liu
 northwestern.edu> License: MIT License Copyright (c) 2024 EpiFluidLab
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

### Comparing `finaletoolkit-0.6.1/README.md` & `finaletoolkit-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/pyproject.toml` & `finaletoolkit-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/PKG-INFO` & `finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinaleToolkit
-Version: 0.6.1
+Version: 0.6.2
 Summary: FinaleToolkit is a package and standalone program to extract fragmentation features of cell-free DNA from paired-end sequencing data.
 Author-email: James Li <lijw21@wfu.edu>, Ravi Bandaru <ravi.bandaru@northwestern.edu>, Yaping Liu <yaping@northwestern.edu>
 License: MIT License
         
         Copyright (c) 2024 EpiFluidLab
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_hzhe9oxg_/tmp5afcr6c0_TarContainer/0/8", line 54, column 35: Levels of opening and closing headings don't match*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: FinaleToolkit Version: 0.6.1 Summary: FinaleToolkit
+Metadata-Version: 2.1 Name: FinaleToolkit Version: 0.6.2 Summary: FinaleToolkit
 is a package and standalone program to extract fragmentation features of cell-
 free DNA from paired-end sequencing data. Author-email: James Li
 wfu.edu>, Ravi Bandaru
 northwestern.edu>, Yaping Liu
 northwestern.edu> License: MIT License Copyright (c) 2024 EpiFluidLab
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
```

### Comparing `finaletoolkit-0.6.1/src/FinaleToolkit.egg-info/SOURCES.txt` & `finaletoolkit-0.6.2/src/FinaleToolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,10 +26,11 @@
 src/finaletoolkit/utils/__init__.py
 src/finaletoolkit/utils/agg_bw.py
 src/finaletoolkit/utils/cli_hist.py
 src/finaletoolkit/utils/filter_bam.py
 src/finaletoolkit/utils/utils.py
 tests/test_cleavage_profile.py
 tests/test_cli_entry.py
+tests/test_coverage.py
 tests/test_end_motifs.py
 tests/test_frag_io.py
 tests/test_wps.py
```

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/cli/main_cli.py` & `finaletoolkit-0.6.2/src/finaletoolkit/cli/main_cli.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/__init__.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/__init__.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/adjust_wps.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/adjust_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/cleavage_profile.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/coverage.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/coverage.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi_gc_correct.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi_gc_correct.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/delfi_merge_bins.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/delfi_merge_bins.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/end_motifs.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/end_motifs.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/frag_length.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/frag_length.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/multi_wps.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/multi_wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/frag/wps.py` & `finaletoolkit-0.6.2/src/finaletoolkit/frag/wps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/genome/gaps.py` & `finaletoolkit-0.6.2/src/finaletoolkit/genome/gaps.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/utils/agg_bw.py` & `finaletoolkit-0.6.2/src/finaletoolkit/utils/agg_bw.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/utils/cli_hist.py` & `finaletoolkit-0.6.2/src/finaletoolkit/utils/cli_hist.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/utils/filter_bam.py` & `finaletoolkit-0.6.2/src/finaletoolkit/utils/filter_bam.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/src/finaletoolkit/utils/utils.py` & `finaletoolkit-0.6.2/src/finaletoolkit/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,50 @@
 from tqdm import tqdm
 
 
 def chrom_sizes_to_list(
     chrom_sizes_file: Union[str, Path]) -> list[tuple[str][int]]:
     """
     Reads chromosome names and sizes from a CHROMSIZE file into a list.
+
+    Parameters
+    ----------
+    chrom_sizes_file: str or Path
+        Tab-delimited file with column for chrom names and column for
+        chrom sizes.
+    
+    Returns
+    -------
+    list of string, int tuples
+        chrom names and sizes.
     """
     chrom_sizes = []
     with open(chrom_sizes_file, 'r') as file:
         for line in file:
             if line != '\n':
                 chrom, size = line.strip().split('\t')
                 chrom_sizes.append((chrom, int(size)))
     return chrom_sizes
 
 
 def chrom_sizes_to_dict(
     chrom_sizes_file: Union[str, Path]) -> list[tuple[str][int]]:
     """
-    Reads chromosome names and sizes from a CHROMSIZE file into a list.
+    Reads chromosome names and sizes from a CHROMSIZE file into a dict.
+
+    Parameters
+    ----------
+    chrom_sizes_file: str or Path
+        Tab-delimited file with column for chrom names and column for
+        chrom sizes.
+    
+    Returns
+    -------
+    dict
+        Chrom names are keys and values are int chrom sizes.
     """
     chrom_sizes = {}
     with open(chrom_sizes_file, 'r') as file:
         for line in file:
             if line != '\n':
                 chrom, size = line.strip().split('\t')
                 chrom_sizes[chrom] = size
@@ -265,16 +287,18 @@
                 and (r_stop is None or f_start < r_stop)
             )
         else:
             raise ValueError(f'{intersect_policy} is not a valid policy')
 
         # Raise exception if start and stop specified but not contig
         if contig is None and not (start is None and stop is None):
-            raise ValueError("contig should be specified if start or "
-                             "stop given.")
+            if contig is None and start==0 and stop is None:
+                pass
+            else:
+                raise ValueError("contig should be specified if start or stop given.")
 
         if is_sam:
             for read in sam_file.fetch(contig, start, stop):
                 # Only select read1 and filter out non-paired-end
                 # reads and low-quality reads
                 try:
                     if (low_quality_read_pairs(read, quality_threshold)
```

### Comparing `finaletoolkit-0.6.1/tests/test_cleavage_profile.py` & `finaletoolkit-0.6.2/tests/test_cleavage_profile.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/tests/test_cli_entry.py` & `finaletoolkit-0.6.2/tests/test_cli_entry.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/tests/test_end_motifs.py` & `finaletoolkit-0.6.2/tests/test_end_motifs.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/tests/test_frag_io.py` & `finaletoolkit-0.6.2/tests/test_frag_io.py`

 * *Files identical despite different names*

### Comparing `finaletoolkit-0.6.1/tests/test_wps.py` & `finaletoolkit-0.6.2/tests/test_wps.py`

 * *Files identical despite different names*

