# Comparing `tmp/used_addr_check-0.1.3.tar.gz` & `tmp/used_addr_check-0.1.4.tar.gz`

## Comparing `used_addr_check-0.1.3.tar` & `used_addr_check-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.cspell/custom-dictionary-workspace.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.vscode/extensions.json
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.vscode/settings.json
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/__main__.py
--rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/cli.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/download_list.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_create.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_search.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/index_types.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/src/used_addr_check/scan_file.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_1.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_scan_file.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_data/scan_file_sample_1.txt
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/tests/test_data/scan_file_sample_2.txt
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/LICENSE
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 used_addr_check-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/.cspell/custom-dictionary-workspace.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/.vscode/extensions.json
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/__main__.py
+-rw-r--r--   0        0        0     3742 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/cli.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/download_list.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/index_create.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/index_search.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/index_types.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/src/used_addr_check/scan_file.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/tests/test_1.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/tests/test_scan_file.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/tests/test_data/scan_file_sample_1.txt
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/tests/test_data/scan_file_sample_2.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 used_addr_check-0.1.4/PKG-INFO
```

### Comparing `used_addr_check-0.1.3/.vscode/settings.json` & `used_addr_check-0.1.4/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/src/used_addr_check/cli.py` & `used_addr_check-0.1.4/src/used_addr_check/cli.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/src/used_addr_check/download_list.py` & `used_addr_check-0.1.4/src/used_addr_check/download_list.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/src/used_addr_check/index_create.py` & `used_addr_check-0.1.4/src/used_addr_check/index_create.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/src/used_addr_check/index_search.py` & `used_addr_check-0.1.4/src/used_addr_check/index_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,9 +116,9 @@
     found_needles = []
     for needle in tqdm(needles, desc="Searching needles", unit="needle"):
         if search_in_file_with_index(haystack_file_path, needle, index=index):
             found_needles.append(needle)
     logger.info(
         f"Found {len(found_needles):,}/{len(needles):,} needles in the file"
     )
-    logger.info(f"Needles found: {found_needles}")
+    logger.info(f"Needles found: {sorted(found_needles)}")
     return found_needles
```

### Comparing `used_addr_check-0.1.3/src/used_addr_check/scan_file.py` & `used_addr_check-0.1.4/src/used_addr_check/scan_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,23 @@
     """
 
     logger.info("Trying using ripgrep search")
     rg = Ripgrepy(
         regex_pattern=BITCOIN_ADDR_REGEX,
         path=str(text_file_path.absolute()),
     )
-    results = rg.only_matching().json().run().as_dict
+    results = (
+        rg.only_matching()
+        .json()
+        .unrestricted()
+        .unrestricted()
+        .unrestricted()
+        .run()
+        .as_dict
+    )
 
     matches = []
     for result in results:
         matches.extend(
             [
                 sub_match["match"]["text"]
                 for sub_match in result["data"]["submatches"]
@@ -122,15 +130,16 @@
         to search for in the haystack file.
     """
     assert isinstance(haystack_file_path, Path)
     assert isinstance(needle_file_path, Path)
 
     needle_addresses = extract_addresses_from_file(needle_file_path)
     logger.info(
-        f"Extracted {len(needle_addresses):,} addresses from the needle file"
+        f"Extracted {len(needle_addresses):,} addresses from the needle file "
+        f" ({needle_file_path})"
     )
 
     # remove duplicates (get distinct addresses)
     count_before_distinct = len(needle_addresses)
     needle_addresses = list(set(needle_addresses))
     count_after_distinct = len(needle_addresses)
     addr_count_change = count_after_distinct - count_before_distinct  # neg
```

### Comparing `used_addr_check-0.1.3/tests/test_scan_file.py` & `used_addr_check-0.1.4/tests/test_scan_file.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/tests/test_data/scan_file_sample_1.txt` & `used_addr_check-0.1.4/tests/test_data/scan_file_sample_1.txt`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/tests/test_data/scan_file_sample_2.txt` & `used_addr_check-0.1.4/tests/test_data/scan_file_sample_2.txt`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/.gitignore` & `used_addr_check-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/LICENSE` & `used_addr_check-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/README.md` & `used_addr_check-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.3/pyproject.toml` & `used_addr_check-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "used_addr_check"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name="RecRanger", email="RecRanger+package@proton.me" },
 ]
 description = "A tool to efficiently check if a Bitcoin Address has ever been used before"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `used_addr_check-0.1.3/PKG-INFO` & `used_addr_check-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: used_addr_check
-Version: 0.1.3
+Version: 0.1.4
 Summary: A tool to efficiently check if a Bitcoin Address has ever been used before
 Project-URL: Homepage, https://github.com/RecRanger/used-addr-check
 Project-URL: Issues, https://github.com/RecRanger/used-addr-check/issues
 Author-email: RecRanger <RecRanger+package@proton.me>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

