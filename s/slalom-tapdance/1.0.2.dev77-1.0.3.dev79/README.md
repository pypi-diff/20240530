# Comparing `tmp/slalom_tapdance-1.0.2.dev77.tar.gz` & `tmp/slalom_tapdance-1.0.3.dev79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slalom_tapdance-1.0.2.dev77.tar", max compression
+gzip compressed data, was "slalom_tapdance-1.0.3.dev79.tar", max compression
```

## Comparing `slalom_tapdance-1.0.2.dev77.tar` & `slalom_tapdance-1.0.3.dev79.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-10 19:34:35.432125 slalom_tapdance-1.0.2.dev77/LICENSE
--rw-r--r--   0        0        0     1220 2024-05-10 19:34:54.444296 slalom_tapdance-1.0.2.dev77/pyproject.toml
--rw-r--r--   0        0        0      288 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/__init__.py
--rw-r--r--   0        0        0      714 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/cli.py
--rw-r--r--   0        0        0    15604 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/config.py
--rw-r--r--   0        0        0    14381 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/install_helper.py
--rw-r--r--   0        0        0    38838 2024-05-10 19:34:35.436125 slalom_tapdance-1.0.2.dev77/tapdance/plans.py
--rw-r--r--   0        0        0     3180 2024-05-10 19:34:35.440125 slalom_tapdance-1.0.2.dev77/tapdance/states.py
--rw-r--r--   0        0        0    11998 2024-05-10 19:34:35.440125 slalom_tapdance-1.0.2.dev77/tapdance/syncs.py
--rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.2.dev77/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-30 16:21:13.850980 slalom_tapdance-1.0.3.dev79/LICENSE
+-rw-r--r--   0        0        0     1220 2024-05-30 16:21:28.259131 slalom_tapdance-1.0.3.dev79/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-05-30 16:21:13.854980 slalom_tapdance-1.0.3.dev79/tapdance/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-30 16:21:13.854980 slalom_tapdance-1.0.3.dev79/tapdance/cli.py
+-rw-r--r--   0        0        0    15604 2024-05-30 16:21:13.854980 slalom_tapdance-1.0.3.dev79/tapdance/config.py
+-rw-r--r--   0        0        0    14381 2024-05-30 16:21:13.854980 slalom_tapdance-1.0.3.dev79/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2024-05-30 16:21:13.854980 slalom_tapdance-1.0.3.dev79/tapdance/install_helper.py
+-rw-r--r--   0        0        0    39788 2024-05-30 16:21:13.858980 slalom_tapdance-1.0.3.dev79/tapdance/plans.py
+-rw-r--r--   0        0        0     3180 2024-05-30 16:21:13.858980 slalom_tapdance-1.0.3.dev79/tapdance/states.py
+-rw-r--r--   0        0        0    11998 2024-05-30 16:21:13.858980 slalom_tapdance-1.0.3.dev79/tapdance/syncs.py
+-rw-r--r--   0        0        0     1357 1970-01-01 00:00:00.000000 slalom_tapdance-1.0.3.dev79/PKG-INFO
```

### Comparing `slalom_tapdance-1.0.2.dev77/LICENSE` & `slalom_tapdance-1.0.3.dev79/LICENSE`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/pyproject.toml` & `slalom_tapdance-1.0.3.dev79/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slalom-tapdance"
-version = "1.0.2-dev.77"
+version = "1.0.3-dev.79"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["Michael Baillergeon <michael.baillergeon@slalom.com>","John Timeus <john.timeus@slalom.com>"]
 license = "MIT"
 packages = [
     {include = "tapdance"}
 ]
```

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/cli.py` & `slalom_tapdance-1.0.3.dev79/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/config.py` & `slalom_tapdance-1.0.3.dev79/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/docker.py` & `slalom_tapdance-1.0.3.dev79/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/install_helper.py` & `slalom_tapdance-1.0.3.dev79/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/plans.py` & `slalom_tapdance-1.0.3.dev79/tapdance/plans.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     taps_dir: str,
     *,
     config_file: str,
     catalog_dir: str,
     dockerized: bool,
     tap_exe: str,
 ) -> None:
+    """
+    Create command that runs a discover on the tap to generate a
+    catalog raw file.
+    """
     catalog_file = config.get_raw_catalog_file(
         taps_dir, catalog_dir, tap_name, allow_custom=False
     )
     uio.create_folder(catalog_dir)
     img = f"{docker.BASE_DOCKER_REPO}:{tap_exe}"
     hide_cmd = False
     if dockerized:
@@ -70,14 +74,15 @@
             capture_stderr=False,
             hide=hide_cmd,
         )
         if not _is_valid_json(output_text):
             raise RuntimeError(f"Could not parse json file from output:\n{output_text}")
         uio.create_text_file(catalog_file, output_text)
     else:
+        # Run the discover
         runnow.run(
             f"{tap_exe} --config {config_file} --discover > {catalog_file}",
             hide=hide_cmd,
         )
 
 
 @logged("running custom schema inference on a dry run of '{tap_name}'")
@@ -590,14 +595,15 @@
     tap_exe = tap_exe or tap_settings.get("EXE", f"tap-{tap_name}")
     replication_strategy = replication_strategy or tap_settings.get(
         "REPLICATION_STRATEGY", "INCREMENTAL"
     )
     config.validate_replication_strategy(replication_strategy)
     catalog_dir = config.get_tap_output_dir(tap_name, taps_dir)
     log_dir = config.get_log_dir(log_dir)
+    # Get the file path for Catalog Raw
     raw_catalog_file = config.get_raw_catalog_file(
         taps_dir, catalog_dir, tap_name, allow_custom=True
     )
     selected_catalog_file = f"{catalog_dir}/{tap_name}-catalog-selected.json"
     plan_file = config.get_plan_file(tap_name, taps_dir, required=False)
     if rescan or not uio.file_exists(raw_catalog_file):
         # Run discover, if needed, to get catalog.json (raw)
@@ -607,14 +613,17 @@
             config_file=config_file,
             catalog_dir=catalog_dir,
             dockerized=dockerized,
             tap_exe=tap_exe,
         )
     config.push_logs(log_dir, [raw_catalog_file])
     logging.info(f"Using catalog file for initial plan: {raw_catalog_file}")
+
+    _sort_catalog_raw(raw_catalog_file)
+
     rules_file = config.get_rules_file(taps_dir, tap_name)
     _check_rules(
         tap_name=tap_name,
         catalog_file=raw_catalog_file,
         rules_file=rules_file,
         plan_file_out=plan_file,
         selected_catalog_file_out=selected_catalog_file,
@@ -640,14 +649,31 @@
             plan_file_out=plan_file,
             selected_catalog_file_out=selected_catalog_file,
             replication_strategy=replication_strategy,
             log_dir=log_dir,
         )
     _validate_selected_catalog(tap_name, selected_catalog_file=selected_catalog_file)
 
+def _sort_catalog_raw(raw_catalog_file_path):
+    """
+    Loads the Catalog Raw file, sorts it on the tap_stream_id and column name, then replaces the file.  
+    """
+    logging.info("Sorting the catalog raw")
+    logging.info(raw_catalog_file_path)
+    catalog_raw = json.loads(Path(raw_catalog_file_path).read_text())
+
+    catalog_raw['streams'] = sorted(catalog_raw['streams'], key=lambda x: x['tap_stream_id'])
+
+    for stream in catalog_raw['streams']:
+        properties = stream['schema']['properties']
+        sorted_properties = {k: properties[k] for k in sorted(properties)}
+        stream['schema']['properties'] = sorted_properties
+
+    with open(raw_catalog_file_path, "w") as f:
+        json.dump(catalog_raw, f, indent=2)
 
 def _make_plan_file_text(
     matches: Dict[str, Dict[str, bool]],
     primary_keys: Dict[str, List[str]],
     replication_keys: Dict[str, List[str]],
     table_stream_ids: Dict[str, str],
     excluded_table_stream_ids: Dict[str, List[str]],
```

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/states.py` & `slalom_tapdance-1.0.3.dev79/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/tapdance/syncs.py` & `slalom_tapdance-1.0.3.dev79/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `slalom_tapdance-1.0.2.dev77/PKG-INFO` & `slalom_tapdance-1.0.3.dev79/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slalom-tapdance
-Version: 1.0.2.dev77
+Version: 1.0.3.dev79
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: Michael Baillergeon
 Author-email: michael.baillergeon@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

