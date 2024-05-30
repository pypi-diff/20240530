# Comparing `tmp/nslsii-0.9.0.tar.gz` & `tmp/nslsii-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nslsii-0.9.0.tar", last modified: Fri Jan 20 20:39:08 2023, max compression
+gzip compressed data, was "nslsii-0.9.1.tar", last modified: Thu Jun  8 16:17:30 2023, max compression
```

## Comparing `nslsii-0.9.0.tar` & `nslsii-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-01-20 20:38:58.000000 nslsii-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-01-20 20:38:58.000000 nslsii-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-20 20:39:08.183467 nslsii-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-20 20:38:58.000000 nslsii-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.179467 nslsii-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.179467 nslsii-0.9.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-01-20 20:38:58.000000 nslsii-0.9.0/docs/source/release-history.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/
--rw-r--r--   0 runner    (1001) docker     (123)    22271 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/ad33.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/areadetector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40050 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/areadetector/xspress3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/common/ipynb/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/ipynb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/ipynb/animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/ipynb/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/ipynb/logutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/common/ipynb/nbviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/detectors/
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/QEPro.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/trigger_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/xspress3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/detectors/zebra.py
--rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii/iocs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/iocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/iocs/eps_two_state_ioc_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/iocs/thermo_sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/kafka_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/md_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/temperature_controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-20 20:38:58.000000 nslsii-0.9.0/nslsii/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 20:39:08.183467 nslsii-0.9.0/nslsii.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-01-20 20:39:08.000000 nslsii-0.9.0/nslsii.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-20 20:39:08.000000 nslsii-0.9.0/nslsii.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 20:39:08.000000 nslsii-0.9.0/nslsii.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-20 20:39:08.000000 nslsii-0.9.0/nslsii.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-20 20:39:08.000000 nslsii-0.9.0/nslsii.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-20 20:38:58.000000 nslsii-0.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-20 20:39:08.183467 nslsii-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-01-20 20:38:58.000000 nslsii-0.9.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-01-20 20:38:58.000000 nslsii-0.9.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.704851 nslsii-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-08 16:17:21.000000 nslsii-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 16:17:21.000000 nslsii-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 16:17:30.704851 nslsii-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-08 16:17:21.000000 nslsii-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.700851 nslsii-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.700851 nslsii-0.9.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-08 16:17:21.000000 nslsii-0.9.1/docs/source/release-history.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.704851 nslsii-0.9.1/nslsii/
+-rw-r--r--   0 runner    (1001) docker     (123)    22539 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 16:17:30.704851 nslsii-0.9.1/nslsii/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/ad33.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.700851 nslsii-0.9.1/nslsii/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42478 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/areadetector/xspress3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.700851 nslsii-0.9.1/nslsii/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.704851 nslsii-0.9.1/nslsii/common/ipynb/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/ipynb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/ipynb/animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/ipynb/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/ipynb/logutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/common/ipynb/nbviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.704851 nslsii-0.9.1/nslsii/detectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/QEPro.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/trigger_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/webcam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/xspress3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9737 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/detectors/zebra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4227 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.704851 nslsii-0.9.1/nslsii/iocs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/iocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/iocs/eps_two_state_ioc_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/iocs/thermo_sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/kafka_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11646 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/md_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/temperature_controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 16:17:21.000000 nslsii-0.9.1/nslsii/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:30.700851 nslsii-0.9.1/nslsii.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-08 16:17:30.000000 nslsii-0.9.1/nslsii.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-08 16:17:30.000000 nslsii-0.9.1/nslsii.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:17:30.000000 nslsii-0.9.1/nslsii.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 16:17:30.000000 nslsii-0.9.1/nslsii.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 16:17:30.000000 nslsii-0.9.1/nslsii.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-08 16:17:21.000000 nslsii-0.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-08 16:17:30.704851 nslsii-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-08 16:17:21.000000 nslsii-0.9.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-06-08 16:17:21.000000 nslsii-0.9.1/versioneer.py
```

### Comparing `nslsii-0.9.0/LICENSE` & `nslsii-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/PKG-INFO` & `nslsii-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nslsii
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for data collection and analysis at NSLS-II
 Author: Brookhaven National Laboratory
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NSLS-II
```

### Comparing `nslsii-0.9.0/docs/source/release-history.rst` & `nslsii-0.9.1/docs/source/release-history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ***************
 Release History
 ***************
 
+v0.9.1 (2023-06-08)
+====================
+* add optional call_returns_result parameter to be propagated to the RunEngine
+* add an ophyd class for a webcam streaming to a URL (Axis cameras)
+* update data handling for flyscaning with Xspress3
+
 v0.9.0 (2023-01-20)
 ===================
 * fix incorrect usage of ``prefix=`` keyword argument in tests 
 * add ``nslsii.areadetector.xspress3.Xspress3ExternalFileReference.dtype_str``
 
 v0.8.0 (2022-12-19)
 ===================
```

### Comparing `nslsii-0.9.0/nslsii/__init__.py` & `nslsii-0.9.1/nslsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 def configure_base(
     user_ns,
     broker_name,
     *,
     bec=True,
     bec_derivative=False,
+    call_returns_result=False,
     epics_context=False,
     magics=True,
     mpl=True,
     configure_logging=True,
     pbar=True,
     ipython_logging=True,
     publish_documents_with_kafka=False,
@@ -74,14 +75,17 @@
     broker_name : Union[str, Broker]
         Name of databroker configuration or a Broker instance.
     bec : boolean, optional
         True by default. Set False to skip BestEffortCallback.
     bec_derivative : boolean, optional
         False by default. Set True to enable derivative and its stats
         calculation in BestEffortCallback.
+    call_returns_result: boolean, optional
+        False by default. Set True to have RunEngine return a RunEngineResult
+        object that contains the plan result, error status, and uuid list.
     epics_context : boolean, optional
         True by default. Set False to skip ``setup_ophyd()``.
     magics : boolean, optional
         True by default. Set False to skip registration of custom IPython
         magics.
     mpl : boolean, optional
         True by default. Set False to skip matplotlib ``ion()`` at event-loop
@@ -135,15 +139,15 @@
 
         md = get_history()
     # if RunEngine already defined grab it
     # useful when users make their own custom RunEngine
     if "RE" in user_ns:
         RE = user_ns["RE"]
     else:
-        RE = RunEngine(md)
+        RE = RunEngine(md, call_returns_result=call_returns_result)
         ns["RE"] = RE
 
     # Set up SupplementalData.
     # (This is a no-op until devices are added to it,
     # so there is no need to provide a 'skip_sd' switch.)
     from bluesky import SupplementalData
```

### Comparing `nslsii-0.9.0/nslsii/ad33.py` & `nslsii-0.9.1/nslsii/ad33.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/areadetector/xspress3.py` & `nslsii-0.9.1/nslsii/areadetector/xspress3.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,16 @@
     path_template = Cpt(Signal, kind=Kind.config)
 
     def __init__(
         self,
         *args,
         root_path,
         path_template,
-        resource_kwargs,
+        resource_kwargs=None,
+        spec=Xspress3HDF5Handler.HANDLER_NAME,
         **kwargs,
     ):
         """
 
         Parameters
         ----------
         args:
@@ -178,25 +179,37 @@
             the "non-semantic" part of the data path, for example /nsls2/data
         path_template:
             path to the data directory, which must include the root_path,
             and may include %Y, %m, %d and other strftime replacements,
             for example /nsls2/data/tst/xspress3/2020/01/01
         resource_kwargs:
             placed in resource documents
+        spec:
+            data handler name for resource documents,
+            Xspress3HDF5Handler.HANDLER_NAME by default
         kwargs:
             passed to the parent class
         """
         super().__init__(*args, **kwargs)
         self._resource = None
         self._datum_factory = None
 
+        # TODO: be certain this handler is widely available
+        self.bulk_data_spec = "XSP3_FLY"
+        self.bulk_data_resource_kwargs = {}
+        self._bulk_data_resource = None
+        self._bulk_data_datum_factory = None
+
         self._asset_docs_cache = None
 
         self.root_path.put(root_path)
         self.path_template.put(path_template)
+        self.spec = spec
+        if resource_kwargs is None:
+            resource_kwargs = {}
         self.resource_kwargs = resource_kwargs
 
         self.stage_sigs[self.create_directory] = -3
         self.stage_sigs[self.auto_increment] = "Yes"
         self.stage_sigs[self.auto_save] = "Yes"
         self.stage_sigs[self.num_capture] = 0  # 0 means take as many as you want
         self.stage_sigs[self.enable] = 1
@@ -276,28 +289,42 @@
         # for example, if
         #   full_file_path is /a/b/c/d_0.h5
         #   root_path is /a/b
         # then
         #   resource_path is c/d_0.h5
         resource_path = full_file_path.relative_to(self.root_path.get())
 
+        self._asset_docs_cache = deque()
+
+        self._bulk_data_resource, self._bulk_data_datum_factory, _ = compose_resource(
+            # a UID is _required_ here, so we provide a fake and then remove it from
+            #   the resource document; later a RunEngine will provide a real id
+            start={"uid": "to be replaced"},
+            spec=self.bulk_data_spec,
+            root=self.root_path.get(),
+            resource_path=str(resource_path),
+            resource_kwargs=self.bulk_data_resource_kwargs,
+        )
+        # remove the fake id specified above from the resource document; later
+        #   a RunEngine will provide a real one
+        self._bulk_data_resource.pop("run_start")
+        self._asset_docs_cache.append(("resource", self._bulk_data_resource))
+
         self._resource, self._datum_factory, _ = compose_resource(
             # a UID is _required_ here, so we provide a fake and then remove it from
             #   the resource document; later a RunEngine will provide a real id
             start={"uid": "to be replaced"},
-            spec=Xspress3HDF5Handler.HANDLER_NAME,
+            spec=self.spec,
             root=self.root_path.get(),
             resource_path=str(resource_path),
             resource_kwargs=self.resource_kwargs,
         )
         # remove the fake id specified above from the resource document; later
         #   a RunEngine will provide a real one
         self._resource.pop("run_start")
-
-        self._asset_docs_cache = deque()
         self._asset_docs_cache.append(("resource", self._resource))
 
         # this should be the last thing we do here
         self.capture.set(1).wait()
 
         return staged_devices
 
@@ -307,14 +334,22 @@
 
         return super().unstage()
 
     def generate_datum(self, key, timestamp, datum_kwargs):
         if key is not None:
             raise ValueError(f"'key' must be None but key='{key}'")
 
+        # generate datum document for "bulk" image data (the whole array)
+        if self.parent.get_external_file_ref() and self.parent.get_external_file_ref().kind & Kind.normal:
+            bulk_data_datum = self._bulk_data_datum_factory(
+                datum_kwargs={}
+            )
+            self._asset_docs_cache.append(("datum", bulk_data_datum))
+            self.parent.get_external_file_ref().put(bulk_data_datum["datum_id"])
+
         # generate datum documents for all channels of Kind.normal
         for channel in self.parent.iterate_channels():
             if channel.get_external_file_ref().kind & Kind.normal:
                 datum = self._datum_factory(
                     datum_kwargs={
                         **datum_kwargs,
                         "channel": channel.channel_number,
@@ -883,16 +918,23 @@
 
     def clear_all_rois(self):
         """Clear all MCAROIs"""
         for mcaroi in self.iterate_mcarois():
             mcaroi.clear()
 
     def get_external_file_ref(self):
-        """Return the Xspress3ExternalFileReference."""
-        return getattr(self, image_data_key)
+        """Return the Xspress3ExternalFileReference.
+        
+           image_data_key is an optional attribute
+           if it is not present return None
+        """
+        if image_data_key:
+            return getattr(self, image_data_key)
+        else:
+            return None
 
     channel_fields_and_methods = {
         "__init__": __init__,
         "__repr__": __repr__,
         # keep the read and configuration attrs defined by the Components
         "_default_read_attrs": None,
         "_default_configuration_attrs": None,
@@ -1094,14 +1136,25 @@
         channel : GeneratedXspress3Channel
         """
 
         for channel_attr_name in self.__dir__():
             if channel_attr_name_re.match(channel_attr_name):
                 yield getattr(self, channel_attr_name)
 
+    def get_external_file_ref(self):
+        """Return the Xspress3ExternalFileReference.
+        
+           image_data_key is an optional attribute
+           if it is not present return None
+        """
+        if image_data_key:
+            return getattr(self, image_data_key)
+        else:
+            return None
+
     xspress3_fields_and_methods = dict(
         **{
             "channel_numbers": tuple(sorted(channel_numbers)),
             "external_trig": Cpt(Signal, value=False, doc="Use external triggering"),
             "total_points": Cpt(
                 Signal,
                 value=-1,
@@ -1118,18 +1171,25 @@
                 value=False,
                 doc="Xspress3 cannot safely be rewound in bluesky",
             ),
             "__repr__": __repr__,
             "get_channel_count": get_channel_count,
             "get_channel": get_channel,
             "iterate_channels": iterate_channels,
+            "get_external_file_ref": get_external_file_ref,
         },
         **extra_class_members,
     )
 
+    # Xspress3ExternalFileReference is optional
+    if image_data_key:
+        xspress3_fields_and_methods[image_data_key] = Cpt(
+            Xspress3ExternalFileReference, kind=Kind.normal
+        )
+
     xspress3_fields_and_methods.update(
         {
             f"channel{c:02d}": Cpt(
                 build_channel_class(
                     channel_number=c,
                     mcaroi_numbers=mcaroi_numbers,
                     image_data_key=image_data_key,
```

### Comparing `nslsii-0.9.0/nslsii/common/ipynb/animation.py` & `nslsii-0.9.1/nslsii/common/ipynb/animation.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/common/ipynb/info.py` & `nslsii-0.9.1/nslsii/common/ipynb/info.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/common/ipynb/logutils.py` & `nslsii-0.9.1/nslsii/common/ipynb/logutils.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/common/ipynb/nbviewer.py` & `nslsii-0.9.1/nslsii/common/ipynb/nbviewer.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/detectors/QEPro.py` & `nslsii-0.9.1/nslsii/detectors/QEPro.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/detectors/trigger_mixins.py` & `nslsii-0.9.1/nslsii/detectors/trigger_mixins.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/detectors/utils.py` & `nslsii-0.9.1/nslsii/detectors/utils.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/detectors/xspress3.py` & `nslsii-0.9.1/nslsii/detectors/xspress3.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/detectors/zebra.py` & `nslsii-0.9.1/nslsii/detectors/zebra.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/devices.py` & `nslsii-0.9.1/nslsii/devices.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/iocs/eps_two_state_ioc_sim.py` & `nslsii-0.9.1/nslsii/iocs/eps_two_state_ioc_sim.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/iocs/thermo_sim.py` & `nslsii-0.9.1/nslsii/iocs/thermo_sim.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/kafka_utils.py` & `nslsii-0.9.1/nslsii/kafka_utils.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/md_dict.py` & `nslsii-0.9.1/nslsii/md_dict.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/temperature_controllers.py` & `nslsii-0.9.1/nslsii/temperature_controllers.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii/transforms.py` & `nslsii-0.9.1/nslsii/transforms.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/nslsii.egg-info/PKG-INFO` & `nslsii-0.9.1/nslsii.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nslsii
-Version: 0.9.0
+Version: 0.9.1
 Summary: Tools for data collection and analysis at NSLS-II
 Author: Brookhaven National Laboratory
 License: BSD (3-clause)
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # NSLS-II
```

### Comparing `nslsii-0.9.0/nslsii.egg-info/SOURCES.txt` & `nslsii-0.9.1/nslsii.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,13 @@
 nslsii/common/ipynb/info.py
 nslsii/common/ipynb/logutils.py
 nslsii/common/ipynb/nbviewer.py
 nslsii/detectors/QEPro.py
 nslsii/detectors/__init__.py
 nslsii/detectors/trigger_mixins.py
 nslsii/detectors/utils.py
+nslsii/detectors/webcam.py
 nslsii/detectors/xspress3.py
 nslsii/detectors/zebra.py
 nslsii/iocs/__init__.py
 nslsii/iocs/eps_two_state_ioc_sim.py
 nslsii/iocs/thermo_sim.py
```

### Comparing `nslsii-0.9.0/setup.py` & `nslsii-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `nslsii-0.9.0/versioneer.py` & `nslsii-0.9.1/versioneer.py`

 * *Files identical despite different names*

