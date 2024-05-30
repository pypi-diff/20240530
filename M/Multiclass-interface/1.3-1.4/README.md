# Comparing `tmp/multiclass_interface-1.3.tar.gz` & `tmp/multiclass_interface-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiclass_interface-1.3.tar", last modified: Tue May 28 11:49:19 2024, max compression
+gzip compressed data, was "multiclass_interface-1.4.tar", last modified: Thu May 30 05:45:59 2024, max compression
```

## Comparing `multiclass_interface-1.3.tar` & `multiclass_interface-1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.3/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/Multiclass_interface.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-28 11:49:19.000000 multiclass_interface-1.3/Multiclass_interface.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1578 2024-05-28 11:49:19.662954 multiclass_interface-1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/multiclass_interface/
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.3/multiclass_interface/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6088 2024-05-28 09:44:04.000000 multiclass_interface-1.3/multiclass_interface/mpi_interface.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/multi_object_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.3/multiclass_interface/multiprocess_interface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-28 11:49:19.662954 multiclass_interface-1.3/multiclass_interface/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 11:47:05.000000 multiclass_interface-1.3/multiclass_interface/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/tests/my_test_cls.py
--rw-rw-rw-   0 root         (0) root         (0)     2826 2024-05-28 09:44:04.000000 multiclass_interface-1.3/multiclass_interface/tests/test_mpi.py
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.3/multiclass_interface/tests/test_multiclass_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.3/multiclass_interface/tests/test_multiprocessinterface.py
--rw-r--r--   0 root         (0) root         (0)      406 2024-05-28 11:49:19.000000 multiclass_interface-1.3/multiclass_interface/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     6561 2024-05-28 10:04:03.000000 multiclass_interface-1.3/sequence_diagrams.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-28 11:49:19.662954 multiclass_interface-1.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:45:59.385102 multiclass_interface-1.4/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-03-18 14:23:06.000000 multiclass_interface-1.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2124 2024-05-24 05:52:15.000000 multiclass_interface-1.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1094 2024-03-19 07:05:00.000000 multiclass_interface-1.4/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:45:59.385102 multiclass_interface-1.4/Multiclass_interface.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-30 05:45:59.000000 multiclass_interface-1.4/Multiclass_interface.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-30 05:45:59.000000 multiclass_interface-1.4/Multiclass_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 05:45:59.000000 multiclass_interface-1.4/Multiclass_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-30 05:45:59.000000 multiclass_interface-1.4/Multiclass_interface.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-30 05:45:59.000000 multiclass_interface-1.4/Multiclass_interface.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1578 2024-05-30 05:45:59.385102 multiclass_interface-1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      899 2024-03-19 07:07:38.000000 multiclass_interface-1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:45:59.385102 multiclass_interface-1.4/multiclass_interface/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-03-18 12:26:49.000000 multiclass_interface-1.4/multiclass_interface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6584 2024-05-30 05:42:04.000000 multiclass_interface-1.4/multiclass_interface/mpi_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-18 19:36:25.000000 multiclass_interface-1.4/multiclass_interface/multi_object_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8169 2024-03-21 09:39:37.000000 multiclass_interface-1.4/multiclass_interface/multiprocess_interface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 05:45:59.385102 multiclass_interface-1.4/multiclass_interface/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-30 05:44:37.000000 multiclass_interface-1.4/multiclass_interface/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2024-03-18 19:36:25.000000 multiclass_interface-1.4/multiclass_interface/tests/my_test_cls.py
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2024-05-28 09:44:04.000000 multiclass_interface-1.4/multiclass_interface/tests/test_mpi.py
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-03-18 19:36:25.000000 multiclass_interface-1.4/multiclass_interface/tests/test_multiclass_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-21 09:39:37.000000 multiclass_interface-1.4/multiclass_interface/tests/test_multiprocessinterface.py
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-30 05:45:59.000000 multiclass_interface-1.4/multiclass_interface/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-03-19 07:05:00.000000 multiclass_interface-1.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     6561 2024-05-28 10:04:03.000000 multiclass_interface-1.4/sequence_diagrams.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 05:45:59.385102 multiclass_interface-1.4/setup.cfg
```

### Comparing `multiclass_interface-1.3/.gitlab-ci.yml` & `multiclass_interface-1.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/LICENSE` & `multiclass_interface-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/Multiclass_interface.egg-info/PKG-INFO` & `multiclass_interface-1.4/Multiclass_interface.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.3
+Version: 1.4
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.3/Multiclass_interface.egg-info/SOURCES.txt` & `multiclass_interface-1.4/Multiclass_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/PKG-INFO` & `multiclass_interface-1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Multiclass_interface
-Version: 1.3
+Version: 1.4
 Summary: Multiclass interface
 Author-email: "Mads M. Pedersen" <mmpe@dtu.dk>
 Project-URL: Homepage, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface
 Project-URL: Bug Tracker, https://gitlab.windenergy.dtu.dk/DYNAMIKS/multiclass_interface/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `multiclass_interface-1.3/README.md` & `multiclass_interface-1.4/README.md`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/mpi_interface.py` & `multiclass_interface-1.4/multiclass_interface/mpi_interface.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 import traceback
 import inspect
 
 comm = None
 size = 1
 rank = 0
 name = ""
-main = True
+mpi = False
 
 
-def activate_mpi():
-    global comm, size, rank, name, main
+def activate_mpi(collective_mpi=True, loop_until_close=True, terminate_on_close=True):
+    global comm, size, rank, name, mpi, LOOP_UNTIL_CLOSE, TERMINATE_ON_CLOSE, COLLECTIVE_MPI
     from mpi4py import MPI
     comm = MPI.COMM_WORLD
     size = MPI.COMM_WORLD.Get_size()
     rank = MPI.COMM_WORLD.Get_rank()
     name = MPI.Get_processor_name()
-    main = rank == 0
+    mpi = True
+    COLLECTIVE_MPI = collective_mpi
+    LOOP_UNTIL_CLOSE = loop_until_close
+    TERMINATE_ON_CLOSE = terminate_on_close
 
 
 MPIClassInterfaceAttributes = {
     'close',
     'use_rank',
     'cls',
     'work_loop',
@@ -29,17 +32,17 @@
     '__class__',
     'get_input',
     'do_task',
     'run_task',
     'closed'}
 
 
-LOOP_UNTIL_CLOSE = True
-TERMINATE_ON_CLOSE = True
-COLLECTIVE_MPI = True
+LOOP_UNTIL_CLOSE = True  # MPI workers (rank>0) will enter the work loop and wait for commands from rank 0
+TERMINATE_ON_CLOSE = True  # MPI workers (rank>0) will terminate (sys.exit) when the close command is called via rank0
+COLLECTIVE_MPI = True  # rank0 acts as a single point of contact (scatters command+arg and gathers results)
 
 
 class MPIClassInterface():
     def __init__(self, cls, args_lst):
         if len(args_lst) > size:
             if rank == 0:
                 raise Exception(f"Not enough mpi slots. Slots: {size}, Requested: {len(args_lst)}")
```

### Comparing `multiclass_interface-1.3/multiclass_interface/multi_object_list.py` & `multiclass_interface-1.4/multiclass_interface/multi_object_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/multiprocess_interface.py` & `multiclass_interface-1.4/multiclass_interface/multiprocess_interface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/tests/my_test_cls.py` & `multiclass_interface-1.4/multiclass_interface/tests/my_test_cls.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/tests/test_mpi.py` & `multiclass_interface-1.4/multiclass_interface/tests/test_mpi.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/tests/test_multiclass_list.py` & `multiclass_interface-1.4/multiclass_interface/tests/test_multiclass_list.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/multiclass_interface/tests/test_multiprocessinterface.py` & `multiclass_interface-1.4/multiclass_interface/tests/test_multiprocessinterface.py`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/pyproject.toml` & `multiclass_interface-1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `multiclass_interface-1.3/sequence_diagrams.md` & `multiclass_interface-1.4/sequence_diagrams.md`

 * *Files identical despite different names*

